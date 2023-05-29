# Comparing `tmp/async_websocket_client-0.0.0a6.tar.gz` & `tmp/async_websocket_client-0.0.0a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_websocket_client-0.0.0a6.tar", max compression
+gzip compressed data, was "async_websocket_client-0.0.0a7.tar", max compression
```

## Comparing `async_websocket_client-0.0.0a6.tar` & `async_websocket_client-0.0.0a7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1056 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a6/LICENSE
--rw-r--r--   0        0        0        0 2023-05-14 19:46:39.511004 async_websocket_client-0.0.0a6/async_websocket_client/__init__.py
--rw-r--r--   0        0        0     2624 2023-05-10 13:08:56.327036 async_websocket_client-0.0.0a6/async_websocket_client/apps.py
--rw-r--r--   0        0        0      924 2023-05-11 06:20:55.592215 async_websocket_client-0.0.0a6/async_websocket_client/dispatchers.py
--rw-r--r--   0        0        0     1822 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a6/pyproject.toml
--rw-r--r--   0        0        0     1706 2023-05-08 05:59:55.233187 async_websocket_client-0.0.0a6/readme.md
--rw-r--r--   0        0        0     2279 1970-01-01 00:00:00.000000 async_websocket_client-0.0.0a6/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-29 17:42:21.444066 async_websocket_client-0.0.0a7/LICENSE
+-rw-r--r--   0        0        0        0 2023-05-29 17:42:21.480066 async_websocket_client-0.0.0a7/async_websocket_client/__init__.py
+-rw-r--r--   0        0        0     2162 2023-05-29 17:42:21.444066 async_websocket_client-0.0.0a7/async_websocket_client/apps.py
+-rw-r--r--   0        0        0     1026 2023-05-29 17:42:21.444066 async_websocket_client-0.0.0a7/async_websocket_client/dispatchers.py
+-rw-r--r--   0        0        0     1822 2023-05-29 17:42:21.448066 async_websocket_client-0.0.0a7/pyproject.toml
+-rw-r--r--   0        0        0     1966 2023-05-29 17:42:21.448066 async_websocket_client-0.0.0a7/readme.md
+-rw-r--r--   0        0        0     2539 1970-01-01 00:00:00.000000 async_websocket_client-0.0.0a7/PKG-INFO
```

### Comparing `async_websocket_client-0.0.0a6/LICENSE` & `async_websocket_client-0.0.0a7/LICENSE`

 * *Files identical despite different names*

### Comparing `async_websocket_client-0.0.0a6/async_websocket_client/apps.py` & `async_websocket_client-0.0.0a7/async_websocket_client/apps.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,31 +24,40 @@
     is_running: bool
 
     def __init__(self, url: str, dispatcher: BaseDispatcher):
         self.url = url
         self.dispatcher = dispatcher
         self.dispatcher.set_app(self)
 
-        self.is_running = True
+        self.is_running = False
 
     async def connect(self):
         await self.dispatcher.before_connect()
         self.ws = await websockets.connect(self.url)
         await self.dispatcher.set_websocket(self.ws)
         await self.dispatcher.on_connect()
 
+        self.is_running = True
+
     async def disconnect(self):
         self.is_running = False
 
         await self.dispatcher.before_disconnect()
         await self.ws.close()
         await self.dispatcher.on_disconnect()
 
     async def send(self, message: str) -> Any:
-        return asyncio.create_task(self.ws.send(message))
+        return await self.ws.send(message)
+
+    async def ws_recv_message(self) -> str | None:
+        try:
+            return await asyncio.wait_for(self.ws.recv(), 1)
+
+        except asyncio.TimeoutError:
+            return None
 
     async def ws_recv_loop(self):
         while self.is_running:
             message = await self.ws.recv()
             if message is None:
                 continue
 
@@ -62,42 +71,15 @@
 
         except asyncio.exceptions.CancelledError as ex:
             logger.error([type(ex), ex])
 
         except ConnectionClosedError as e:
             logger.error(f'Connection closed with error: {e}')
 
-        self.is_running = False
-
         await self.disconnect()
 
     def asyncio_run(self):
         try:
             asyncio.run(self.run())
 
         except KeyboardInterrupt:
             logger.info('Correct exit')
-
-
-class TasksMixin(AsyncWebSocketApp):
-
-    tasks: list[Coroutine]
-    _tasks: list[asyncio.Task]
-
-    async def start_tasks(self):
-        self._tasks = []
-        for cor in self.tasks:
-            logger.error(f'Start: {cor}')
-            self._tasks.append(asyncio.create_task(cor))
-
-    async def stop_tasks(self):
-        for task in self._tasks:
-            logger.error(f'Stop: {task}')
-            await asyncio.wait_for(task, 10)
-
-    async def connect(self):
-        await super().connect()
-        await self.start_tasks()
-
-    async def disconnect(self):
-        await self.stop_tasks()
-        await super().disconnect()
```

### Comparing `async_websocket_client-0.0.0a6/pyproject.toml` & `async_websocket_client-0.0.0a7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `async_websocket_client-0.0.0a6/readme.md` & `async_websocket_client-0.0.0a7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,26 @@
-# WebSockets Groups
+Metadata-Version: 2.1
+Name: async-websocket-client
+Version: 0.0.0a7
+Summary: 
+Author: irocshers
+Author-email: develop.iam@rocshers.com
+Requires-Python: >=3.8,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: websockets (>=11.0.2,<12.0.0)
+Description-Content-Type: text/markdown
 
-Модуль реализующих менеджер групп WebSocket подключений
+# Async WebSocket client
+
+A module that implements an asynchronous interface based on [websockets](https://github.com/python-websockets/websockets) for working with websockets
 
 [![PyPI](https://img.shields.io/pypi/v/async-websocket-client)](https://pypi.org/project/async-websocket-client/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/async-websocket-client)](https://pypi.org/project/async-websocket-client/)
 [![GitLab last commit](https://img.shields.io/gitlab/last-commit/rocshers/python/async-websocket-client)](https://gitlab.com/rocshers/python/async-websocket-client)
 
 [![Test coverage](https://codecov.io/gitlab/rocshers:python/async-websocket-client/branch/release/graph/badge.svg?token=RPFNZ8SBQ6)](https://codecov.io/gitlab/rocshers:python/async-websocket-client)
 [![Downloads](https://static.pepy.tech/badge/async-websocket-client)](https://pepy.tech/project/async-websocket-client)
@@ -18,25 +34,30 @@
 - Поддержка реестров: memory, redis
 
 ## Quick start
 
 Установка:
 
 ```sh
-pip install websockets-groups
+pip install async-websocket-client
 ```
 
 Подключение:
 
 ```python
-from fastapi import WebSocket
-from websockets_groups import WSGroupsManager, MemoryStorage, BaseDispatcher
-
-ws_groups_manager = WSGroupsManager(MemoryStorage())
-
-class ChatDispatcher(BaseDispatcher):
-    pass
-
-@app.websocket('/chats/')
-async def ws_view(webdocket: WebSocket, chat_name: str):
-    await ws_groups_manager.register_ws(websocket, ChatDispatcher())
+import asyncio
+from async_websocket_client.apps import AsyncWebSocketApp
+from async_websocket_client.dispatchers import BaseDispatcher
+
+class SomeDispatcher(BaseDispatcher):
+    async def on_connect(self):
+        return await self.ws.send('hello, server')
+
+    async def on_message(self, message: str):
+        return await self.ws.send(f'server, I received your message. len(message)=={len(message)}')
+
+client = AsyncWebSocketApp('ws://localhost:8001/ws', SomeDispatcher())
+client.asyncio_run() # quick run
+# or
+asyncio.run(client.run()) # Run with asyncio
 ```
+
```

### Comparing `async_websocket_client-0.0.0a6/PKG-INFO` & `async_websocket_client-0.0.0a7/readme.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,10 @@
-Metadata-Version: 2.1
-Name: async-websocket-client
-Version: 0.0.0a6
-Summary: 
-Author: irocshers
-Author-email: develop.iam@rocshers.com
-Requires-Python: >=3.8,<4.0
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: websockets (>=11.0.2,<12.0.0)
-Description-Content-Type: text/markdown
+# Async WebSocket client
 
-# WebSockets Groups
-
-Модуль реализующих менеджер групп WebSocket подключений
+A module that implements an asynchronous interface based on [websockets](https://github.com/python-websockets/websockets) for working with websockets
 
 [![PyPI](https://img.shields.io/pypi/v/async-websocket-client)](https://pypi.org/project/async-websocket-client/)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/async-websocket-client)](https://pypi.org/project/async-websocket-client/)
 [![GitLab last commit](https://img.shields.io/gitlab/last-commit/rocshers/python/async-websocket-client)](https://gitlab.com/rocshers/python/async-websocket-client)
 
 [![Test coverage](https://codecov.io/gitlab/rocshers:python/async-websocket-client/branch/release/graph/badge.svg?token=RPFNZ8SBQ6)](https://codecov.io/gitlab/rocshers:python/async-websocket-client)
 [![Downloads](https://static.pepy.tech/badge/async-websocket-client)](https://pepy.tech/project/async-websocket-client)
@@ -34,26 +18,29 @@
 - Поддержка реестров: memory, redis
 
 ## Quick start
 
 Установка:
 
 ```sh
-pip install websockets-groups
+pip install async-websocket-client
 ```
 
 Подключение:
 
 ```python
-from fastapi import WebSocket
-from websockets_groups import WSGroupsManager, MemoryStorage, BaseDispatcher
-
-ws_groups_manager = WSGroupsManager(MemoryStorage())
-
-class ChatDispatcher(BaseDispatcher):
-    pass
-
-@app.websocket('/chats/')
-async def ws_view(webdocket: WebSocket, chat_name: str):
-    await ws_groups_manager.register_ws(websocket, ChatDispatcher())
+import asyncio
+from async_websocket_client.apps import AsyncWebSocketApp
+from async_websocket_client.dispatchers import BaseDispatcher
+
+class SomeDispatcher(BaseDispatcher):
+    async def on_connect(self):
+        return await self.ws.send('hello, server')
+
+    async def on_message(self, message: str):
+        return await self.ws.send(f'server, I received your message. len(message)=={len(message)}')
+
+client = AsyncWebSocketApp('ws://localhost:8001/ws', SomeDispatcher())
+client.asyncio_run() # quick run
+# or
+asyncio.run(client.run()) # Run with asyncio
 ```
-
```


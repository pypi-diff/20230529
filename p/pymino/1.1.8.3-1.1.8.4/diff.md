# Comparing `tmp/pymino-1.1.8.3.tar.gz` & `tmp/pymino-1.1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\submitpypi\dist\.tmp-ibrvdd1p\pymino-1.1.8.3.tar", last modified: Sat May 27 20:45:02 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.8.3\dist\.tmp-_g53xax8\pymino-1.1.8.4.tar", last modified: Mon May 29 00:37:41 2023, max compression
```

## Comparing `pymino-1.1.8.3.tar` & `pymino-1.1.8.4.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.502750 pymino-1.1.8.3/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.3/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-05-27 20:45:02.502750 pymino-1.1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.458606 pymino-1.1.8.3/pymino/
--rw-rw-rw-   0        0        0      676 2023-05-27 20:44:15.000000 pymino-1.1.8.3/pymino/__init__.py
--rw-rw-rw-   0        0        0    26133 2023-05-17 23:36:26.000000 pymino-1.1.8.3/pymino/bot.py
--rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.8.3/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.483407 pymino-1.1.8.3/pymino/ext/
--rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.8.3/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.8.3/pymino/ext/account.py
--rw-rw-rw-   0        0        0   271224 2023-05-25 22:50:46.000000 pymino-1.1.8.3/pymino/ext/community.py
--rw-rw-rw-   0        0        0    44587 2023-05-27 20:44:04.000000 pymino-1.1.8.3/pymino/ext/context.py
--rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.8.3/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.495806 pymino-1.1.8.3/pymino/ext/entities/
--rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.8.3/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.3/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    14662 2023-05-27 20:43:58.000000 pymino-1.1.8.3/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    52847 2023-05-27 20:44:10.000000 pymino-1.1.8.3/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     2653 2023-05-17 23:34:15.000000 pymino-1.1.8.3/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.8.3/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     6185 2023-05-25 23:01:02.000000 pymino-1.1.8.3/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.3/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.3/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0     7900 2023-05-17 02:59:28.000000 pymino-1.1.8.3/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.501758 pymino-1.1.8.3/pymino/ext/utilities/
--rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.8.3/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.3/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.3/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.8.3/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-27 20:45:02.475470 pymino-1.1.8.3/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-05-27 20:45:02.000000 pymino-1.1.8.3/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-05-27 20:45:02.000000 pymino-1.1.8.3/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 20:45:02.000000 pymino-1.1.8.3/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-27 20:45:02.000000 pymino-1.1.8.3/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-27 20:45:02.000000 pymino-1.1.8.3/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-05-27 20:45:02.504734 pymino-1.1.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-05-18 00:06:54.000000 pymino-1.1.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.656715 pymino-1.1.8.4/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.4/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-05-29 00:37:41.656715 pymino-1.1.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.613563 pymino-1.1.8.4/pymino/
+-rw-rw-rw-   0        0        0      721 2023-05-29 00:12:00.000000 pymino-1.1.8.4/pymino/__init__.py
+-rw-rw-rw-   0        0        0     8112 2023-05-29 00:01:55.000000 pymino-1.1.8.4/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    27542 2023-05-29 00:04:00.000000 pymino-1.1.8.4/pymino/bot.py
+-rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.8.4/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.637867 pymino-1.1.8.4/pymino/ext/
+-rw-rw-rw-   0        0        0      469 2023-05-28 22:44:43.000000 pymino-1.1.8.4/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.8.4/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   273924 2023-05-29 00:08:42.000000 pymino-1.1.8.4/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18163 2023-05-28 22:59:05.000000 pymino-1.1.8.4/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24194 2023-05-28 22:29:38.000000 pymino-1.1.8.4/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7299 2023-05-29 00:25:30.000000 pymino-1.1.8.4/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   271224 2023-05-25 22:50:46.000000 pymino-1.1.8.4/pymino/ext/community.py
+-rw-rw-rw-   0        0        0    44587 2023-05-29 00:03:54.000000 pymino-1.1.8.4/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.8.4/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.648779 pymino-1.1.8.4/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.8.4/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.4/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    14847 2023-05-28 23:41:49.000000 pymino-1.1.8.4/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    52847 2023-05-27 20:44:10.000000 pymino-1.1.8.4/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4763 2023-05-29 00:33:12.000000 pymino-1.1.8.4/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.8.4/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     6185 2023-05-25 23:01:02.000000 pymino-1.1.8.4/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.4/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.4/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.8.4/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     7088 2023-05-29 00:33:01.000000 pymino-1.1.8.4/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.655723 pymino-1.1.8.4/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      118 2023-05-28 22:35:54.000000 pymino-1.1.8.4/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11330 2023-05-28 22:35:37.000000 pymino-1.1.8.4/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.4/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.4/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.8.4/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.623483 pymino-1.1.8.4/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-05-29 00:37:41.000000 pymino-1.1.8.4/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1011 2023-05-29 00:37:41.000000 pymino-1.1.8.4/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 00:37:41.000000 pymino-1.1.8.4/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-29 00:37:41.000000 pymino-1.1.8.4/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 00:37:41.000000 pymino-1.1.8.4/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-05-29 00:37:41.663163 pymino-1.1.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.8.4/setup.py
```

### Comparing `pymino-1.1.8.3/LICENSE` & `pymino-1.1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/PKG-INFO` & `pymino-1.1.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.3
+Version: 1.1.8.4
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.3 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.4 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.3/README.md` & `pymino-1.1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/bot.py` & `pymino-1.1.8.4/pymino/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,31 @@
-from time import time
+from time import perf_counter, time
 from typing import Optional, Union
 
 from .ext.socket import WSClient
 from .ext.account import Account
 from .ext.community import Community
 from .ext.entities.handlers import *
 from .ext.utilities.generate import device_id
 from .ext.entities.userprofile import UserProfile
 from .ext.utilities.request_handler import RequestHandler
 from .ext.entities.general import ApiResponse, CCommunity
 from .ext.entities.exceptions import (
-    LoginFailed, MissingEmailPasswordOrSid, VerifyCommunityIdIsCorrect
+    LoginFailed, MissingEmailPasswordOrSid,
+    VerifyCommunityIdIsCorrect, PingFailed
     )
 
 class Bot(WSClient):
     """
     `Bot` - This is the main client.
 
     `**Parameters**``
     - `command_prefix` - The prefix to use for commands. `Defaults` to `!`.
     - `community_id` - The community id to use for the bot. `Defaults` to `None`.
+    - `online_status` - Whether to set the bot's online status to `online`. `Defaults` to `True`.
     - `**kwargs` - Any other parameters to use for the bot.
 
         - `device_id` - The device id to use for the bot.
 
         - `proxy` - The proxy to use for the bot. `proxy` must be `str`.
 
         - `disable_socket` - Whether to disable the socket.
@@ -208,24 +210,31 @@
         @bot.command(command_name="ping", command_description="This command will return pong.")
         def ping_command(ctx: Context):
             ctx.send("Pong!")
 
         bot.run(email="email", password="password")
         ```
     """
-    def __init__(self, command_prefix: Optional[str] = "!", community_id: Union[str, int] = None, **kwargs):
+    def __init__(
+        self,
+        command_prefix: Optional[str] = "!",
+        community_id: Union[str, int] = None,
+        online_status: bool = True, 
+        **kwargs):
+
         for key, value in kwargs.items(): setattr(self, key, value)
         self._debug:            bool = check_debugger()
         self._is_ready:         bool = False
         self._userId:           str = None
         self._sid:              str = None
         self._cached:           bool = False
         self.cache:             Cache = Cache("cache")
         self.command_prefix:    Optional[str] = command_prefix
         self.community_id:      Union[str, int] = community_id
+        self.online_status:     bool = online_status
         self.device_id:         Optional[str] = kwargs.get("device_id") or device_id()
         self.request:           RequestHandler = RequestHandler(
                                 bot = self,
                                 proxy=kwargs.get("proxy")
                                 )
         self.community:         Community = Community(
                                 bot = self,
@@ -667,8 +676,41 @@
                 community_id = int(community_id)
         except VerifyCommunityIdIsCorrect as e:
             raise VerifyCommunityIdIsCorrect from e
 
         self.community_id = community_id
         self.community.community_id = community_id
 
-        return community_id
+        return community_id
+    
+    def ping(self) -> float:
+        """
+        Pings the server and returns the elapsed time in milliseconds.
+        
+        :return: The elapsed time in milliseconds.
+        :rtype: float
+        
+        This method pings the server by sending a GET request to the account endpoint. It then calculates the elapsed
+        time in milliseconds and returns it.
+        
+        If the ping fails, the method raises a PingFailed exception.
+        
+        **Note:** This method is not recommended for production use. It is intended for testing purposes only.
+        
+        **Example usage:**
+        
+        ```python
+        bot = Bot()
+        @bot.command("ping")
+        def ping_command(ctx: Context):
+            ping = bot.ping()
+            ctx.reply(f"Pong! {ping}ms")
+        ```
+        """
+        try:
+            start = perf_counter()
+            self.request.handler(method="GET", url="/g/s/account")
+            end = perf_counter()
+            elapsed_time_ms = (end - start) * 1000
+            return round(elapsed_time_ms, 2)
+        except Exception:
+            raise PingFailed
```

### Comparing `pymino-1.1.8.3/pymino/client.py` & `pymino-1.1.8.4/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/account.py` & `pymino-1.1.8.4/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/community.py` & `pymino-1.1.8.4/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/context.py` & `pymino-1.1.8.4/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/dispatcher.py` & `pymino-1.1.8.4/pymino/ext/dispatcher.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Callable
 
+
 class MessageDispatcher:
     """
     `MessageDispatcher` - Simple message dispatcher that allows you to register handlers for specific message types.
  
     `**Example**`
 
     ```py
@@ -25,8 +26,40 @@
     def register(self, message_type: int, handler: Callable):
         self.dispatch_table[message_type] = handler
 
     def handle(self, message: dict):
         message_type = message.get("t")
         if message_type not in self.dispatch_table:
             return
-        self.dispatch_table[message_type](message)
+        self.dispatch_table[message_type](message)
+
+
+class AsyncMessageDispatcher:
+    """
+    `AsyncMessageDispatcher` - Simple async message dispatcher that allows you to register handlers for specific message types.
+ 
+    `**Example**`
+
+    ```py
+
+    dispatcher = AsyncMessageDispatcher()
+
+    message_type = 1000
+    message = {"t": message_type, "d": {"foo": "bar"}}
+    handler = lambda message: print(message)
+
+    dispatcher.register(message_type, handler)
+    await dispatcher.handle(message)
+    ```
+
+    """
+    def __init__(self):
+        self.dispatch_table = {}
+
+    def register(self, message_type: int, handler: Callable):
+        self.dispatch_table[message_type] = handler
+
+    async def handle(self, message: dict):
+        message_type = message.get("t")
+        if message_type not in self.dispatch_table:
+            return
+        await self.dispatch_table[message_type](message)
```

### Comparing `pymino-1.1.8.3/pymino/ext/entities/enums.py` & `pymino-1.1.8.4/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/entities/exceptions.py` & `pymino-1.1.8.4/pymino/ext/entities/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -454,8 +454,14 @@
             "\nPlease restart your bot.\n"
             )
         
 class NullResponse(Exception):
     def __init__(self):
         super().__init__(
             "Server returned a null response. Possible crash content in the requested data."
+            )
+        
+class PingFailed(Exception):
+    def __init__(self):
+        super().__init__(
+            "Ping failed. Please make sure you are logged in and try again."
             )
```

### Comparing `pymino-1.1.8.3/pymino/ext/entities/general.py` & `pymino-1.1.8.4/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/entities/messages.py` & `pymino-1.1.8.4/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/entities/threads.py` & `pymino-1.1.8.4/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/entities/userprofile.py` & `pymino-1.1.8.4/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/entities/wsevents.py` & `pymino-1.1.8.4/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/socket.py` & `pymino-1.1.8.4/pymino/ext/socket.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,28 +10,30 @@
 from .context import EventHandler
 from .dispatcher import MessageDispatcher
 from .entities.wsevents import EventTypes, NotifTypes
 from .entities.userprofile import OnlineMembers
 from .entities.messages import Channel, Message, NNotification
 from .entities.exceptions import WrongWebSocketPackage
 from .utilities.generate import device_id, generate_signature
-from .entities.handlers import is_android, is_repl, notify, orjson_exists
+from .entities.handlers import run_alive_loop, orjson_exists
 
 if orjson_exists():
     from orjson import (
         loads as orjson_loads, dumps as orjson_dumps
         )
 
+
 try:
     from websocket import WebSocket, WebSocketApp
 except ImportError as e:
     system("pip uninstall websocket -y")
-    system("pip install websocket-client==1.4.1")
+    system("pip install websocket-client==1.5.2")
     raise WrongWebSocketPackage from e
 
+
 class WSClient(EventHandler):
     """
     `WSClient` is a class that handles the websocket.
     """
     def __init__(self):
         self.ws:            WebSocketApp = None
         self.online_status: bool = True        
@@ -43,23 +45,26 @@
         self.orjson:        bool = orjson_exists()
         
         self.dispatcher.register(10, self._handle_notification)
         self.dispatcher.register(201, self._handle_agora_channel)
         self.dispatcher.register(400, self._handle_user_online)
         self.dispatcher.register(1000, self._handle_message)
         EventHandler.__init__(self)
-        
+
+
     def fetch_ws_url(self) -> str:
         return f"wss://ws{randint(1, 4)}.aminoapps.com"
 
+
     def connect(self) -> None:
         """Connects to the websocket."""
         self.run_forever()
         return self.emit("ready")
 
+
     def run_forever(self) -> None:
         """Runs the websocket forever."""
         ws_data = f"{device_id()}|{int(time() * 1000)}"
         self.ws = WebSocketApp(
             url = f"{self.fetch_ws_url()}/?{urlencode({'signbody': ws_data})}",
             on_open=self.on_websocket_open,
             on_message=self.on_websocket_message,
@@ -68,136 +73,127 @@
             header={
             "NDCDEVICEID": device_id(),
             "NDCAUTH": f"sid={self.sid}",
             "NDC-MSG-SIG": generate_signature(ws_data)
             })
         return self.start_processes()
 
+
     def start_processes(self) -> None:
         """Starts the websocket processes."""
-        for process in[self.ws.run_forever, self.heartbeat]:
-            Thread(target=process).start()
+        websocket_thread = Thread(target=self.ws.run_forever)
+        websocket_thread.start()
+
+        aalive_thread = Thread(target=run_alive_loop, args=(self,))
+        aalive_thread.start()
+
 
     def on_websocket_error(self, ws: WebSocket, error: Exception) -> None:
         """Handles websocket errors."""
         with suppress(KeyError):
             self._events["error"](error)
 
+
     def on_websocket_message(self, ws: WebSocket, message: dict) -> None:
         """Handles websocket messages."""
         try:
             raw_message = orjson_loads(message) if self.orjson else loads(message)
         except JSONDecodeError:
             raw_message = loads(message)
 
         self.dispatcher.handle(raw_message)
 
+
     def _handle_message(self, message: dict) -> None:
         """Sends the message to the event handler."""
         _message: Message = Message(message)
 
         if self.userId == _message.userId: return None
         None if any(
             [_message.ndcId is None, _message.ndcId == 0]
         ) else self._communities.add(_message.ndcId)
 
         key = self.event_types.get(f"{_message.type}:{_message.mediaType}")
         if key != None:
             return Thread(target=self._handle_event, args=(key, _message)).start()
 
+
     def _handle_notification(self, message: dict) -> None:
         """Handles notifications."""
         notification: NNotification = NNotification(message)
         key = self.notif_types.get(notification.notifType)
         if key != None:
             return Thread(target=self._handle_event, args=(key, notification)).start()
-    
+
+
     def _handle_agora_channel(self, message: dict) -> None:
         """Sets the agora channel."""
         self.channel: Channel = Channel(message)
 
+
     def _handle_user_online(self, message: dict) -> None:
         """Handles user online events."""
         return self._handle_event("user_online", OnlineMembers(message))
 
+
     def on_websocket_close(self, ws: WebSocket, close_status_code: int, close_msg: str) -> None:
         """Handles websocket close events."""
         if [close_status_code, close_msg] == [None, None]:
             return self.run_forever() 
-        
+
+
     def send_websocket_message(self, message: dict) -> None:
         """Sends a websocket message."""
         return self.ws.send(orjson_dumps(message).decode() if self.orjson else dumps(message))
 
+
     def stop_websocket(self) -> None:
         """Stops the websocket."""
         return self.ws.close()
 
+
     def on_websocket_open(self, ws: WebSocket) -> None:
         """Handles websocket open events."""
         if all([self.community_id != None, "user_online" in self._events]):
             return self.send_websocket_message({
                 "t": 300,
                 "o": {
                     "ndcId": self.community_id,
                     "topic": f"ndtopic:x{self.community_id}:online-members",
                     "id": int(time() * 1000)
                 }})
 
+
     def _last_active(self, last_activity_time: float) -> bool:
         """Returns True if the last activity was 5 minutes ago."""""
         return time() - last_activity_time >= 300
 
+
     def _last_message(self, last_message_time: float) -> bool:
         """Returns True if the last message was 30 seconds ago."""
         return time() - last_message_time >= 30
 
+
     def _send_message(self) -> None:
         """Sends a message to the websocket."""
         self.send_websocket_message({
             "o":{
                 "threadChannelUserInfoList": [],
                 "id": randint(1, 100)},
                 "t": 116
                 })
 
+
     def _activity_status(self) -> None:
         """Sets the user's activity status to online."""
         for comId in self._communities:
 
             if self.online_status:
                 try:
                     self.community.online_status(comId=comId)
                     self.community.send_active(comId=comId,
                     timers=[{"start": int(time()), "end": int(time()) + 300}]
                     )
                 except Exception:
                     self.online_status = False
 
-            delay(randint(5, 10))
-
-    def heartbeat(self) -> None:
-        """Runs a few background processes."""
-        run_check = any([is_android(), is_repl()])
-
-        start_time          = time()
-        last_activity_time  = start_time
-        last_message_time   = start_time
-
-        while True:
-            current_time = time()
-            notify() if run_check else None
-
-            with suppress(Exception):
-
-                if self._last_message(last_message_time):
-                    self._send_message()
-                    last_message_time = current_time
-
-                if current_time - start_time >= 86400:
-                    start_time = current_time
-
-                if all([self._last_active(last_activity_time), current_time - start_time <= 36000]):
-                    self._activity_status()
-                    last_activity_time = current_time
-
-                delay(randint(25, 50))
+            delay(randint(5, 10))
```

### Comparing `pymino-1.1.8.3/pymino/ext/utilities/commands.py` & `pymino-1.1.8.4/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/utilities/generate.py` & `pymino-1.1.8.4/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino/ext/utilities/request_handler.py` & `pymino-1.1.8.4/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.3/pymino.egg-info/PKG-INFO` & `pymino-1.1.8.4/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.3
+Version: 1.1.8.4
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.3 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.4 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.3/pymino.egg-info/SOURCES.txt` & `pymino-1.1.8.4/pymino.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,38 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 pymino/__init__.py
+pymino/async_bot.py
 pymino/bot.py
 pymino/client.py
 pymino.egg-info/PKG-INFO
 pymino.egg-info/SOURCES.txt
 pymino.egg-info/dependency_links.txt
 pymino.egg-info/requires.txt
 pymino.egg-info/top_level.txt
 pymino/ext/__init__.py
 pymino/ext/account.py
+pymino/ext/async_community.py
+pymino/ext/async_context.py
+pymino/ext/async_event_handler.py
+pymino/ext/async_socket.py
 pymino/ext/community.py
 pymino/ext/context.py
 pymino/ext/dispatcher.py
+pymino/ext/handle_queue.py
 pymino/ext/socket.py
 pymino/ext/entities/__init__.py
 pymino/ext/entities/enums.py
 pymino/ext/entities/exceptions.py
 pymino/ext/entities/general.py
 pymino/ext/entities/handlers.py
 pymino/ext/entities/messages.py
 pymino/ext/entities/threads.py
 pymino/ext/entities/userprofile.py
 pymino/ext/entities/wsevents.py
 pymino/ext/utilities/__init__.py
+pymino/ext/utilities/async_request_handler.py
 pymino/ext/utilities/commands.py
 pymino/ext/utilities/generate.py
 pymino/ext/utilities/request_handler.py
```

### Comparing `pymino-1.1.8.3/setup.cfg` & `pymino-1.1.8.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e38 2e33 0d0a 6175  on = 1.1.8.3..au
+00000020: 6f6e 203d 2031 2e31 2e38 2e34 0d0a 6175  on = 1.1.8.4..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.8.3/setup.py` & `pymino-1.1.8.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -13,19 +13,20 @@
     description="Easily create a bot for Amino Apps using a modern easy to use synchronous library.",
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     url="https://github.com/forevercynical/pymino",
     version = config.get('metadata', 'version'),
     packages=find_packages(),
     install_requires=[
-        "requests==2.28.2",
-        "ujson==5.5.0",
+        "requests==2.31.0",
+        "ujson==5.7.0",
         "colorama==0.4.6",
-        "websocket-client==1.4.1",
-        "diskcache==5.4.0"
+        "websocket-client==1.5.2",
+        "diskcache==5.4.0",
+        "aiohttp==3.8.4"
     ],
     keywords=[
         "amino",
         "pymino",
         "narvii",
         "amino-api",
         "narvii-bots",
```


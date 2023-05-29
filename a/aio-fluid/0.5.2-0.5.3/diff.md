# Comparing `tmp/aio_fluid-0.5.2.tar.gz` & `tmp/aio_fluid-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aio_fluid-0.5.2.tar", max compression
+gzip compressed data, was "aio_fluid-0.5.3.tar", max compression
```

## Comparing `aio_fluid-0.5.2.tar` & `aio_fluid-0.5.3.tar`

### file list

```diff
@@ -1,43 +1,45 @@
--rw-r--r--   0        0        0     1517 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/LICENSE
--rw-r--r--   0        0        0       64 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/__init__.py
--rw-r--r--   0        0        0     1633 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/backdoor.py
--rw-r--r--   0        0        0      593 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/cors.py
--rw-r--r--   0        0        0     2165 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/datajson.py
--rw-r--r--   0        0        0     1493 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/db.py
--rw-r--r--   0        0        0      218 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/dev.py
--rw-r--r--   0        0        0      575 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/executor.py
--rw-r--r--   0        0        0     1225 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/fields.py
--rw-r--r--   0        0        0       75 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/github/__init__.py
--rw-r--r--   0        0        0      866 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/github/client.py
--rw-r--r--   0        0        0     4084 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/github/repo.py
--rw-r--r--   0        0        0    11637 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/http.py
--rw-r--r--   0        0        0      138 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/json.py
--rw-r--r--   0        0        0     2326 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/kernel.py
--rw-r--r--   0        0        0      296 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/kong.py
--rw-r--r--   0        0        0     2920 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/log.py
--rw-r--r--   0        0        0     9481 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/node.py
--rw-r--r--   0        0        0     3784 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/redis.py
--rw-r--r--   0        0        0      620 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/redis_status.py
--rw-r--r--   0        0        0      758 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/__init__.py
--rw-r--r--   0        0        0     8413 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/broker.py
--rw-r--r--   0        0        0      347 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/constants.py
--rw-r--r--   0        0        0     9532 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/consumer.py
--rw-r--r--   0        0        0     2746 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/cpubound.py
--rw-r--r--   0        0        0     4209 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/crontab.py
--rw-r--r--   0        0        0     1280 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/every.py
--rw-r--r--   0        0        0     2306 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/readme.md
--rw-r--r--   0        0        0     1424 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/scheduler.py
--rw-r--r--   0        0        0     4546 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/task.py
--rw-r--r--   0        0        0     1547 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/task_run.py
--rw-r--r--   0        0        0      363 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/scheduler/utils.py
--rw-r--r--   0        0        0     2023 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/service.py
--rw-r--r--   0        0        0      429 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/settings.py
--rw-r--r--   0        0        0     6692 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/stacksampler.py
--rw-r--r--   0        0        0     1003 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/status.py
--rw-r--r--   0        0        0      399 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/sync_run.py
--rw-r--r--   0        0        0      526 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/text.py
--rw-r--r--   0        0        0      599 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/types.py
--rw-r--r--   0        0        0     2584 2023-05-28 18:10:59.716717 aio_fluid-0.5.2/fluid/utils.py
--rw-r--r--   0        0        0     1875 2023-05-28 18:10:59.720717 aio_fluid-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1213 2023-05-28 18:10:59.720717 aio_fluid-0.5.2/readme.md
--rw-r--r--   0        0        0     3082 1970-01-01 00:00:00.000000 aio_fluid-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/LICENSE
+-rw-r--r--   0        0        0       64 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/__init__.py
+-rw-r--r--   0        0        0     1633 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/backdoor.py
+-rw-r--r--   0        0        0      593 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/cors.py
+-rw-r--r--   0        0        0     2165 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/datajson.py
+-rw-r--r--   0        0        0     1493 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/db.py
+-rw-r--r--   0        0        0      218 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/dev.py
+-rw-r--r--   0        0        0      575 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/executor.py
+-rw-r--r--   0        0        0     1225 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/fields.py
+-rw-r--r--   0        0        0       75 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/github/__init__.py
+-rw-r--r--   0        0        0      866 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/github/client.py
+-rw-r--r--   0        0        0     4084 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/github/repo.py
+-rw-r--r--   0        0        0    11637 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/http.py
+-rw-r--r--   0        0        0      138 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/json.py
+-rw-r--r--   0        0        0     2471 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/kernel.py
+-rw-r--r--   0        0        0      296 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/kong.py
+-rw-r--r--   0        0        0     2936 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/log.py
+-rw-r--r--   0        0        0     9519 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/node.py
+-rw-r--r--   0        0        0        0 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/py.typed
+-rw-r--r--   0        0        0     3784 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/redis.py
+-rw-r--r--   0        0        0      620 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/redis_status.py
+-rw-r--r--   0        0        0      758 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/__init__.py
+-rw-r--r--   0        0        0     8327 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/broker.py
+-rw-r--r--   0        0        0      347 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/constants.py
+-rw-r--r--   0        0        0     9568 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/consumer.py
+-rw-r--r--   0        0        0     2788 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/cpubound.py
+-rw-r--r--   0        0        0     4209 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/crontab.py
+-rw-r--r--   0        0        0     1263 2023-05-29 11:33:08.983718 aio_fluid-0.5.3/fluid/scheduler/every.py
+-rw-r--r--   0        0        0     2306 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/readme.md
+-rw-r--r--   0        0        0     1491 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/scheduler.py
+-rw-r--r--   0        0        0      170 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/settings.py
+-rw-r--r--   0        0        0     4676 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/task.py
+-rw-r--r--   0        0        0     1547 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/task_run.py
+-rw-r--r--   0        0        0      363 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/scheduler/utils.py
+-rw-r--r--   0        0        0     2023 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/service.py
+-rw-r--r--   0        0        0      429 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/settings.py
+-rw-r--r--   0        0        0     6692 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/stacksampler.py
+-rw-r--r--   0        0        0     1003 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/status.py
+-rw-r--r--   0        0        0      399 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/sync_run.py
+-rw-r--r--   0        0        0      526 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/text.py
+-rw-r--r--   0        0        0      599 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/types.py
+-rw-r--r--   0        0        0     2605 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/fluid/utils.py
+-rw-r--r--   0        0        0     2383 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1213 2023-05-29 11:33:08.987718 aio_fluid-0.5.3/readme.md
+-rw-r--r--   0        0        0     3085 1970-01-01 00:00:00.000000 aio_fluid-0.5.3/PKG-INFO
```

### Comparing `aio_fluid-0.5.2/LICENSE` & `aio_fluid-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/backdoor.py` & `aio_fluid-0.5.3/fluid/backdoor.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/cors.py` & `aio_fluid-0.5.3/fluid/cors.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/datajson.py` & `aio_fluid-0.5.3/fluid/datajson.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/db.py` & `aio_fluid-0.5.3/fluid/db.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/executor.py` & `aio_fluid-0.5.3/fluid/executor.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/fields.py` & `aio_fluid-0.5.3/fluid/fields.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/github/client.py` & `aio_fluid-0.5.3/fluid/github/client.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/github/repo.py` & `aio_fluid-0.5.3/fluid/github/repo.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/http.py` & `aio_fluid-0.5.3/fluid/http.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/kernel.py` & `aio_fluid-0.5.3/fluid/kernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 import asyncio
 import sys
-from typing import Callable, Dict, Optional
+from typing import Any, Callable, Dict, Optional
 
 KernelCallback = Callable[[bytes], None]
 READ_LIMIT = 2**16  # 64 KiB
 
 
-async def run_python(*args: str) -> str:
+async def run_python(*args: str) -> int:
     return await run(sys.executable, *args)
 
 
 async def run(
     executable: str,
     *args: str,
     result_callback: Optional[KernelCallback] = None,
     error_callback: Optional[KernelCallback] = None,
     env: Optional[Dict[str, str]] = None,
     stream_output: bool = False,
     stream_error: bool = False,
-):
+) -> int:
     process = await asyncio.create_subprocess_exec(
         executable,
         *args,
         stdin=asyncio.subprocess.PIPE,
         stdout=asyncio.subprocess.PIPE,
         stderr=asyncio.subprocess.PIPE,
         limit=READ_LIMIT,
         env=env,
     )
+    if not process.stdout or not process.stderr:
+        raise RuntimeError("Failed to create subprocess")
     await asyncio.wait(
         [
             asyncio.create_task(
                 _read_stream(process.stdout, stream_output, result_callback or noop)
             ),
             asyncio.create_task(
                 _read_stream(process.stderr, stream_error, error_callback or noop)
@@ -56,15 +58,15 @@
             chunks.append(chunk)
             break
     return b"".join(chunks)
 
 
 async def _read_stream(
     stream: asyncio.StreamReader, stream_output: bool, cb: KernelCallback
-):
+) -> None:
     while True:
         if stream_output:
             chunk = await _read_line(stream)
         else:
             chunk = await stream.read()
         if chunk:
             cb(chunk)
@@ -73,17 +75,17 @@
 
 
 def noop(data: bytes) -> None:
     pass
 
 
 class EncodedLog:
-    def __init__(self, log: Callable[[str], None] = sys.stdout.write):
+    def __init__(self, log: Callable[[str], Any] = sys.stdout.write) -> None:
         self.log = log
-        self.data = []
+        self.data: list[str] = []
 
     def __call__(self, data: bytes) -> None:
         msg = data.decode("utf-8")
         self.data.append(msg)
         self.log(msg)
```

### Comparing `aio_fluid-0.5.2/fluid/log.py` & `aio_fluid-0.5.3/fluid/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     return getattr(logging, level)
 
 
 def log_config(
     level: int,
     other_level: int = logging.WARNING,
     app_name: Optional[str] = None,
-    json=bool(K8S),
+    json: bool = bool(K8S),
 ) -> Dict:
     app_name = app_name if app_name is not None else APP_NAME
     other_level = max(level, other_level)
     handler = LOG_HANDLER or ("main" if json else "color")
     return {
         "version": 1,
         "disable_existing_loggers": False,
@@ -87,15 +87,15 @@
     }
 
 
 def log_name(name: str = "") -> str:
     return APP_NAME if not name else f"{APP_NAME}.{name}"
 
 
-def setup(level: str):
+def setup(level: str) -> None:
     dictConfig(log_config(level_num(level)))
 
 
 @click.pass_context
 def setup_logging(ctx: click.Context, verbose: bool, quiet: bool) -> None:
     if verbose:
         level = "DEBUG"
```

### Comparing `aio_fluid-0.5.2/fluid/node.py` & `aio_fluid-0.5.3/fluid/node.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import os
 import random
 import time
 import uuid
 from abc import ABC, abstractmethod
 from functools import cached_property, wraps
 from logging import Logger
-from typing import Any, Callable, Coroutine, Dict, List, Optional, Tuple
+from typing import Any, Callable, Coroutine, List, Optional, Tuple
 
 from aiohttp.client import ClientConnectionError, ClientConnectorError
 from aiohttp.web import Application, GracefulExit
 
 from .log import get_logger
 from .utils import close_task, dot_name, underscore
 
@@ -41,20 +41,20 @@
         return self.create_logger()
 
 
 class NodeBase(ABC, Id):
     exit_lag: int = 1
     app: Optional[Application] = None
 
-    async def start_app(self, app: Application) -> None:
+    async def start_app(self, app: Application | None = None) -> None:
         """Start application"""
         self.app = app
         await self.start()
 
-    async def close_app(self, app: Application) -> None:
+    async def close_app(self, app: Application | None = None) -> None:
         await self.close()
 
     @abstractmethod
     def is_running(self) -> bool:
         """True if the Node is running"""
 
     @abstractmethod
@@ -155,25 +155,25 @@
         except Exception:
             self.logger.exception("unhandled exception in worker")
             await self.system_exit()
         else:
             await self.close(close_worker=False)
 
 
-class WorkerApplication(Dict[str, Any]):
+class WorkerApplication(dict[str, Any]):
     def __init__(self):
         super().__init__()
         self.on_startup = []
         self.on_shutdown = []
 
-    async def startup(self):
+    async def startup(self) -> None:
         for on_startup in self.on_startup:
             await on_startup(self)
 
-    async def shutdown(self):
+    async def shutdown(self) -> None:
         for on_shutdown in self.on_shutdown:
             await on_shutdown(self)
 
 
 class NodeWorkers(NodeBase):
     def __init__(self, *workers: NodeWorker, logger: Optional[Logger] = None) -> None:
         self.logger: Logger = self.create_logger(logger)
```

### Comparing `aio_fluid-0.5.2/fluid/redis.py` & `aio_fluid-0.5.3/fluid/redis.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/redis_status.py` & `aio_fluid-0.5.3/fluid/redis_status.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/scheduler/__init__.py` & `aio_fluid-0.5.3/fluid/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/scheduler/broker.py` & `aio_fluid-0.5.3/fluid/scheduler/broker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,31 @@
-import os
+from __future__ import annotations
+
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from functools import cached_property
-from typing import (
-    Any,
-    Callable,
-    Dict,
-    Iterable,
-    List,
-    NamedTuple,
-    Optional,
-    Tuple,
-    Union,
-)
+from typing import Any, Dict, Iterable, List, NamedTuple, Optional
 from uuid import uuid4
 
 from yarl import URL
 
 from fluid import json
 from fluid.redis import FluidRedis
 from fluid.utils import microseconds
 
+from . import settings
 from .constants import TaskPriority, TaskState
 from .task import Task
 from .task_run import TaskRun
 
-_brokers = {}
-
-DEFAULT_BROKER_URL = "redis://localhost:6379/3"
+_brokers: dict[str, type[Broker]] = {}
 
 
 def broker_url_from_env() -> URL:
-    return URL(os.getenv("SCHEDULER_BROKER_URL", DEFAULT_BROKER_URL))
+    return URL(settings.SCHEDULER_BROKER_URL)
 
 
 class TaskError(RuntimeError):
     pass
 
 
 class UnknownTask(TaskError):
@@ -112,23 +102,22 @@
             if scheduled is not None and bool(task.schedule) is not scheduled:
                 continue
             if enabled is not None and task_map[task.name].enabled is not enabled:
                 continue
             tasks.append(task)
         return tasks
 
-    def task_from_registry(self, task: Union[str, Task]) -> Task:
+    def task_from_registry(self, task: str | Task) -> Task:
         if isinstance(task, Task):
             self.register_task(task)
-            task_ = task
+            return task
         else:
-            task_ = self.registry.get(task)
-            if not task_:
-                raise UnknownTask(task)
-        return task_
+            if task_ := self.registry.get(task):
+                return task_
+            raise UnknownTask(task)
 
     def register_task(self, task: Task) -> None:
         self.registry[task.name] = task
 
     async def enable_task(self, task_name: str, enable: bool = True) -> TaskInfo:
         """Enable or disable a registered task"""
         task = self.registry.get(task_name)
@@ -158,24 +147,23 @@
             priority=priority.name,
             state=state.name,
             params=queued_task.params,
             queued=microseconds(),
         )
 
     @classmethod
-    def from_url(cls, url: str = "") -> "Broker":
-        url = url or broker_url_from_env()
-        p = URL(url)
+    def from_url(cls, url: str = "") -> Broker:
+        p = URL(url or broker_url_from_env())
         Factory = _brokers.get(p.scheme)
         if not Factory:
-            raise RuntimeError(f"Invalid broker {url}")
+            raise RuntimeError(f"Invalid broker {p}")
         return Factory(p)
 
     @classmethod
-    def register_broker(cls, name: str, factory: Callable):
+    def register_broker(cls, name: str, factory: type[Broker]) -> None:
         _brokers[name] = factory
 
 
 class RedisBroker(Broker):
     """A simple broker based on redis lists"""
 
     @cached_property
@@ -183,15 +171,15 @@
         return FluidRedis(str(self.url.with_query({})), name=self.name)
 
     @property
     def name(self) -> str:
         return self.url.query.get("name", "redis-task-broker")
 
     @cached_property
-    def task_queue_names(self) -> Tuple[str, ...]:
+    def task_queue_names(self) -> tuple[str, ...]:
         priorities = self.url.query.get("queues")
         if priorities is None:
             return tuple(self.task_queue_name(p) for p in TaskPriority)
         elif priorities:
             return tuple(
                 self.task_queue_name(TaskPriority[p]) for p in priorities.split(",")
             )
@@ -252,15 +240,15 @@
     async def queue_task(self, queued_task: QueuedTask) -> TaskRun:
         task = self.task_from_registry(queued_task.task)
         priority = queued_task.priority or task.priority
         data = self.task_run_data(queued_task, TaskState.queued)
         await self.redis.cli.lpush(self.task_queue_name(priority), json.dumps(data))
         return self.task_run_from_data(data)
 
-    def _decode_task(self, task: Task, data: dict):
+    def _decode_task(self, task: Task, data: dict) -> TaskInfo:
         info = {name.decode(): json.loads(value) for name, value in data.items()}
         return TaskInfo(
             name=task.name,
             description=task.description,
             schedule=str(task.schedule) if task.schedule else None,
             priority=task.priority.name,
             enabled=info.get("enabled", True),
```

### Comparing `aio_fluid-0.5.2/fluid/scheduler/consumer.py` & `aio_fluid-0.5.3/fluid/scheduler/consumer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import asyncio
 import logging
 from collections import defaultdict, deque
 from dataclasses import dataclass
 from functools import cached_property
 from typing import Any, Callable, Coroutine, Deque, Dict, NamedTuple, Optional, Tuple
```

### Comparing `aio_fluid-0.5.2/fluid/scheduler/cpubound.py` & `aio_fluid-0.5.3/fluid/scheduler/cpubound.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import asyncio
 import logging
 import os
 import sys
 from logging.config import dictConfig
+from typing import Any
 
 from fluid import kernel, log
 from fluid.scheduler import (
     Task,
     TaskConstructor,
     TaskContext,
     TaskDecoratorError,
     TaskExecutor,
     TaskManager,
     TaskRun,
     create_task_app,
+    settings,
 )
 from fluid.scheduler.constants import TaskState
 
-TASK_MANAGER_SPAWN: str = os.getenv("TASK_MANAGER_SPAWN", "")
-
 
 class RemoteLog:
-    def __init__(self, out):
+    def __init__(self, out: Any) -> None:
         self.out = out
 
     def __call__(self, data: bytes) -> None:
         self.out.write(data.decode("utf-8"))
 
 
-async def spawn(ctx: TaskContext):
+async def spawn(ctx: TaskContext) -> None:
     env = dict(os.environ)
     env["TASK_MANAGER_SPAWN"] = "true"
     result = await kernel.run(
         "python",
         "-W",
         "ignore",
         "-m",
@@ -47,37 +47,37 @@
     )
     if result:
         ctx.task_run.set_state(TaskState.failure)
 
 
 class CpuTaskConstructor(TaskConstructor):
     def __call__(self, executor: TaskExecutor) -> Task:
-        if TASK_MANAGER_SPAWN == "true":
+        if settings.TASK_MANAGER_SPAWN == "true":
             cpu_executor = executor
         else:
             self.kwargs["name"] = executor.__name__
             cpu_executor = spawn
         return super().__call__(cpu_executor)
 
 
-def cpu_task(*args, **kwargs) -> Task:
+def cpu_task(*args: Any, **kwargs: Any) -> Task | CpuTaskConstructor:
     """Decorator for creating a CPU bound task"""
     if kwargs and args:
         raise TaskDecoratorError("cannot use positional parameters")
     elif kwargs:
         return CpuTaskConstructor(**kwargs)
     elif len(args) > 1:
         raise TaskDecoratorError("cannot use positional parameters")
     elif not args:
         raise TaskDecoratorError("this is a decorator cannot be invoked in this way")
     else:
         return CpuTaskConstructor()(args[0])
 
 
-async def main(name: str, run_id: str):
+async def main(name: str, run_id: str) -> int:
     dictConfig(
         log.log_config(logging.INFO, logging.CRITICAL, f"{log.APP_NAME}.task.{name}")
     )
     app = create_task_app()
     task_manager: TaskManager = app["task_manager"]
     await app.startup()
     logger = task_manager.logger
```

### Comparing `aio_fluid-0.5.2/fluid/scheduler/crontab.py` & `aio_fluid-0.5.3/fluid/scheduler/crontab.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/scheduler/every.py` & `aio_fluid-0.5.3/fluid/scheduler/every.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import random
 from datetime import datetime, timedelta
-from typing import Optional
 
 from .crontab import CronRun, Scheduler
 
 
 class every(Scheduler):
     def __init__(
         self,
@@ -12,22 +11,22 @@
         delay: timedelta = timedelta(),
         jitter: timedelta = timedelta(),
     ) -> None:
         self.delta: timedelta = delta
         self.delay: timedelta = delay
         self.jitter: timedelta = jitter
         self._delta: timedelta = self.next_delta()
-        self._started = None
+        self._started: datetime | None = None
 
     def info(self) -> str:
         return str(self.delta)
 
     def __call__(
-        self, timestamp: datetime, last_run: Optional[CronRun] = None
-    ) -> Optional[CronRun]:
+        self, timestamp: datetime, last_run: CronRun | None = None
+    ) -> CronRun | None:
         if not last_run and self.delay:
             if not self._started:
                 self._started = timestamp
             if timestamp - self._started < self.delay:
                 return None
         year, month, day, hour, minute, second, _, _, _ = timestamp.timetuple()
         run = CronRun(year, month, day, hour, minute, second)
```

### Comparing `aio_fluid-0.5.2/fluid/scheduler/readme.md` & `aio_fluid-0.5.3/fluid/scheduler/readme.md`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/scheduler/scheduler.py` & `aio_fluid-0.5.3/fluid/scheduler/scheduler.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,18 +29,19 @@
         if not self.task_manager.config.schedule_tasks:
             return
         now = datetime.utcnow()
         periodic_tasks = await self.task_manager.broker.filter_tasks(
             scheduled=True, enabled=True
         )
         for task in periodic_tasks:
-            run = task.schedule(now, self.last_run.get(task.name))
-            if run:
-                self.last_run[task.name] = run
-                from_now = task.randomize() if task.randomize else 0
-                if from_now:
-                    asyncio.get_event_loop().call_later(from_now, self._queue, task)
-                else:
-                    self._queue(task)
+            if task.schedule:
+                run = task.schedule(now, self.last_run.get(task.name))
+                if run:
+                    self.last_run[task.name] = run
+                    from_now = task.randomize() if task.randomize else 0
+                    if from_now:
+                        asyncio.get_event_loop().call_later(from_now, self._queue, task)
+                    else:
+                        self._queue(task)
 
     def _queue(self, task: Task) -> None:
-        self.task_manager.queue(task)
+        self.task_manager.queue(task.name)
```

### Comparing `aio_fluid-0.5.2/fluid/scheduler/task_run.py` & `aio_fluid-0.5.3/fluid/scheduler/task_run.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/service.py` & `aio_fluid-0.5.3/fluid/service.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/stacksampler.py` & `aio_fluid-0.5.3/fluid/stacksampler.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/status.py` & `aio_fluid-0.5.3/fluid/status.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/text.py` & `aio_fluid-0.5.3/fluid/text.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/types.py` & `aio_fluid-0.5.3/fluid/types.py`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/fluid/utils.py` & `aio_fluid-0.5.3/fluid/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,18 +13,19 @@
     if uid:
         if hasattr(uid, "hex"):
             uid = uid.hex
         try:
             return uuid.UUID(uid).hex
         except ValueError:
             return None
+    return None
 
 
 def add_api_url(
-    request, data: Union[List, Dict], path: Optional[str] = None, key: str = "id"
+    request: Any, data: Union[List, Dict], path: Optional[str] = None, key: str = "id"
 ) -> Union[List, Dict]:
     """Add api_url field to data"""
     datas = data
     path = path if path is not None else request.path
     if not isinstance(data, list):
         datas = [cast(dict, data)]
     paths = (f"{path}/{d[key]}" for d in datas if key in d)
```

### Comparing `aio_fluid-0.5.2/pyproject.toml` & `aio_fluid-0.5.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aio-fluid"
-version = "0.5.2"
+version = "0.5.3"
 description = "Tools for backend python services"
 license = "BSD"
 authors = ["Luca <luca@quantmind.com>"]
 readme = "readme.md"
 packages = [
     {include = "fluid"}
 ]
@@ -28,39 +28,73 @@
 ]
 
 [tool.poetry.urls]
 "Repository" = "https://github.com/quantmind/aio-fluid"
 "Issues" = "https://github.com/quantmind/aio-fluid/issues"
 
 [tool.poetry.dependencies]
-python = ">=3.10,<4"
+python = ">=3.10,<3.12"
 aio-openapi = "^3.2.0"
 ujson = "^5.1.0"
 inflection = "^0.5.1"
 prometheus-async = "^22.1.0"
 aioconsole = "^0.6.1"
 python-slugify = {version = "^8.0.1", extras = ["unidecode"]}
 python-json-logger = "^2.0.2"
 colorlog = "^6.6.0"
 aiohttp_cors = "^0.7.0"
-aiobotocore = {version = "~2.4.2", extras=["boto3"]}
-s3fs = {version = "^2023.3.0"}
+aiobotocore = {version = "~2.5.0", extras=["boto3"]}
+s3fs = {version = "^2023.5.0"}
 aio-kong = "^3.3.0"
 uvloop = "^0.17.0"
 pycountry = "^22.3.5"
 redis = "^4.4.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 isort = "^5.9.3"
 black = "^23.3.0"
-flake8 = "^6.0.0"
-flake8-builtins = "^2.0.0"
-flake8-commas = "^2.0.0"
 pytest-cov = "^4.0.0"
-codecov = "^2.1.12"
-mypy = "^1.1.1"
+mypy = "^1.3.0"
 pytest-asyncio = "^0.21.0"
+ruff = "^0.0.270"
+types-ujson = "^5.7.0.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+
+[tool.pytest.ini_options]
+asyncio_mode = "auto"
+testpaths = [
+    "tests"
+]
+markers = [
+    "flaky: marks test as flaky"
+]
+
+[tool.isort]
+profile = "black"
+
+[tool.ruff]
+select = ["E", "F"]
+line-length = 88
+
+[tool.mypy]
+disallow_untyped_calls = "true"
+warn_return_any = "false"
+disallow_untyped_defs = "true"
+warn_no_return = "true"
+
+[[tool.mypy.overrides]]
+module = "fluid.utils"
+ignore_errors = "true"
+
+
+[[tool.mypy.overrides]]
+module = "fluid.node"
+ignore_errors = "true"
+
+[[tool.mypy.overrides]]
+module = "fluid.redis"
+ignore_errors = "true"
```

### Comparing `aio_fluid-0.5.2/readme.md` & `aio_fluid-0.5.3/readme.md`

 * *Files identical despite different names*

### Comparing `aio_fluid-0.5.2/PKG-INFO` & `aio_fluid-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: aio-fluid
-Version: 0.5.2
+Version: 0.5.3
 Summary: Tools for backend python services
 License: BSD
 Author: Luca
 Author-email: luca@quantmind.com
-Requires-Python: >=3.10,<4
+Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
@@ -21,25 +21,25 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: aio-kong (>=3.3.0,<4.0.0)
 Requires-Dist: aio-openapi (>=3.2.0,<4.0.0)
-Requires-Dist: aiobotocore[boto3] (>=2.4.2,<2.5.0)
+Requires-Dist: aiobotocore[boto3] (>=2.5.0,<2.6.0)
 Requires-Dist: aioconsole (>=0.6.1,<0.7.0)
 Requires-Dist: aiohttp_cors (>=0.7.0,<0.8.0)
 Requires-Dist: colorlog (>=6.6.0,<7.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: prometheus-async (>=22.1.0,<23.0.0)
 Requires-Dist: pycountry (>=22.3.5,<23.0.0)
 Requires-Dist: python-json-logger (>=2.0.2,<3.0.0)
 Requires-Dist: python-slugify[unidecode] (>=8.0.1,<9.0.0)
 Requires-Dist: redis (>=4.4.0,<5.0.0)
-Requires-Dist: s3fs (>=2023.3.0,<2024.0.0)
+Requires-Dist: s3fs (>=2023.5.0,<2024.0.0)
 Requires-Dist: ujson (>=5.1.0,<6.0.0)
 Requires-Dist: uvloop (>=0.17.0,<0.18.0)
 Project-URL: Issues, https://github.com/quantmind/aio-fluid/issues
 Project-URL: Repository, https://github.com/quantmind/aio-fluid
 Description-Content-Type: text/markdown
 
 # Tools for backend python services
```


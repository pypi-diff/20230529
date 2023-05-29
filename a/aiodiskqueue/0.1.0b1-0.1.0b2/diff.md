# Comparing `tmp/aiodiskqueue-0.1.0b1.tar.gz` & `tmp/aiodiskqueue-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0b2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0b1.tar` & `aiodiskqueue-0.1.0b2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0b1/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0b1/.github/workflows/main.yml
--rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0b1/.github/workflows/release.yml
--rw-r--r--   0        0        0      113 2023-05-28 13:27:18.116278 aiodiskqueue-0.1.0b1/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0b1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0b1/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0b1/LICENSE
--rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0b1/Makefile
--rw-r--r--   0        0        0     2124 2023-05-29 15:23:28.059933 aiodiskqueue-0.1.0b1/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0b1/docs/Makefile
--rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0b1/docs/_static/custom.css
--rw-r--r--   0        0        0      110 2023-05-28 18:07:59.394553 aiodiskqueue-0.1.0b1/docs/api.rst
--rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0b1/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0b1/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0b1/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0b1/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b1/examples/basic_usage.py
--rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b1/examples/multiple_consumers.py
--rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b1/examples/single_consumer.py
--rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0      211 2023-05-29 15:25:04.099811 aiodiskqueue-0.1.0b1/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0     7836 2023-05-28 18:28:49.530087 aiodiskqueue-0.1.0b1/src/aiodiskqueue/core.py
--rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b1/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0b1/src/aiodiskqueue/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0b1/tests/__init__.py
--rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b1/tests/factories.py
--rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0b1/tests/helpers.py
--rw-r--r--   0        0        0     3158 2023-05-28 14:06:56.951355 aiodiskqueue-0.1.0b1/tests/loadtest.py
--rw-r--r--   0        0        0     6476 2023-05-28 18:50:55.148916 aiodiskqueue-0.1.0b1/tests/test_core.py
--rw-r--r--   0        0        0     2493 2023-05-28 18:39:49.776986 aiodiskqueue-0.1.0b1/tests/test_integration.py
--rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0b1/tests/test_utils.py
--rw-r--r--   0        0        0      413 2023-05-26 21:16:13.559594 aiodiskqueue-0.1.0b1/tox.ini
--rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0b2/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0b2/.github/workflows/main.yml
+-rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0b2/.github/workflows/release.yml
+-rw-r--r--   0        0        0      113 2023-05-28 13:27:18.116278 aiodiskqueue-0.1.0b2/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0b2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0b2/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0b2/LICENSE
+-rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0b2/Makefile
+-rw-r--r--   0        0        0     2124 2023-05-29 15:23:28.059933 aiodiskqueue-0.1.0b2/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0b2/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0b2/docs/_static/custom.css
+-rw-r--r--   0        0        0      110 2023-05-28 18:07:59.394553 aiodiskqueue-0.1.0b2/docs/api.rst
+-rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0b2/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0b2/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0b2/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0b2/examples/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b2/examples/basic_usage.py
+-rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b2/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b2/examples/single_consumer.py
+-rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-05-29 17:44:16.835425 aiodiskqueue-0.1.0b2/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0     8450 2023-05-29 17:46:19.163424 aiodiskqueue-0.1.0b2/src/aiodiskqueue/core.py
+-rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b2/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0b2/src/aiodiskqueue/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0b2/tests/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b2/tests/factories.py
+-rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0b2/tests/helpers.py
+-rw-r--r--   0        0        0     3158 2023-05-28 14:06:56.951355 aiodiskqueue-0.1.0b2/tests/loadtest.py
+-rw-r--r--   0        0        0     7528 2023-05-29 17:32:05.539083 aiodiskqueue-0.1.0b2/tests/test_core.py
+-rw-r--r--   0        0        0     2493 2023-05-28 18:39:49.776986 aiodiskqueue-0.1.0b2/tests/test_integration.py
+-rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0b2/tests/test_utils.py
+-rw-r--r--   0        0        0      413 2023-05-26 21:16:13.559594 aiodiskqueue-0.1.0b2/tox.ini
+-rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0b2/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0b1/.github/workflows/main.yml` & `aiodiskqueue-0.1.0b2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/.github/workflows/release.yml` & `aiodiskqueue-0.1.0b2/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/LICENSE` & `aiodiskqueue-0.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/README.rst` & `aiodiskqueue-0.1.0b2/README.rst`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/docs/Makefile` & `aiodiskqueue-0.1.0b2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/docs/conf.py` & `aiodiskqueue-0.1.0b2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/docs/make.bat` & `aiodiskqueue-0.1.0b2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0b2/examples/multiple_consumers.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/examples/single_consumer.py` & `aiodiskqueue-0.1.0b2/examples/single_consumer.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/pyproject.toml` & `aiodiskqueue-0.1.0b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/src/aiodiskqueue/core.py` & `aiodiskqueue-0.1.0b2/src/aiodiskqueue/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,24 +14,15 @@
 logger = logging.getLogger(__name__)
 
 
 class Queue(metaclass=NoDirectInstantiation):
     """A persistent AsyncIO FIFO queue.
 
     The content of a queue is stored on disk in a data file.
-    This file usually only exists temporarily while there are items in the queue.
-
-    An existing data file is used to recreate a queue,
-    e.g. to preserve the queue content after a process restart
-
-    However, should the data file be corrupted it will be discarded
-    so the queue can continue to function normally.
-
-    Using two different instances with the same data file simultaneously
-    is not recommended as it may lead to data corruption.
+    This file only exists temporarily while there are items in the queue.
 
     This class is not thread safe.
 
     To create a new object the factory method :func:`create` must be used.
     """
 
     def __init__(self, data_path: Path, maxsize: int, queue: list) -> None:
@@ -175,49 +166,69 @@
                 raise ValueError("task_done() called too many times")
 
             self._unfinished_tasks -= 1
             if self._unfinished_tasks == 0:
                 self._tasks_are_finished.notify_all()
 
     async def _write_queue(self):
-        async with aiofiles.open(
-            self._data_path, "wb", buffering=0
-        ) as fp:  # buffering is disabled to prevent the unclosed file issue.
-            await fp.write(pickle.dumps(self._queue))
+        await self._write_queue_to_path(self._data_path, self._queue)
         size = self.qsize()
         self._peak_size = max(self._peak_size, size)
         logger.debug("Wrote queue with %d items: %s", size, self._data_path)
 
     @staticmethod
-    async def _read_queue(data_path: Path) -> list:
+    async def _write_queue_to_path(data_path: Path, queue: list):
+        async with aiofiles.open(
+            data_path, "wb", buffering=0
+        ) as fp:  # buffering is disabled to prevent the unclosed file issue.
+            await fp.write(pickle.dumps(queue))
+
+    @classmethod
+    async def _read_queue(cls, data_path: Path) -> list:
         try:
             async with aiofiles.open(data_path, "rb", buffering=0) as fp:
                 data = await fp.read()
         except FileNotFoundError:
+            await cls._write_queue_to_path(data_path, [])  # ensuring early we can write
+            await aiofiles.os.remove(data_path)
             return []
 
         try:
             queue = pickle.loads(data)
         except pickle.PickleError:
-            logger.exception("Data file is corrupt. Will be discarded: %s", data_path)
+            backup_path = data_path.with_suffix(".bak")
+            await aiofiles.os.rename(data_path, backup_path)
+            logger.exception(
+                "Data file is corrupt and has been backed up: %s", backup_path
+            )
             return []
 
         logger.info(
-            "Resurrecting queue with %d items from file: %s",
+            "Resurrecting queue with %d items from: %s",
             len(queue),
             data_path,
         )
         return queue
 
     @classmethod
     async def create(cls, data_path: Union[str, Path], maxsize: int = 0) -> "Queue":
-        """Create a queue.
+        """Create a new queue instance.
+
+        A data file will be created at the given path if it does not already exist.
+
+        If the data file already exists, if will be used to recreate the queue if possible.
+        Should that fail, the existing data file will be backed up and the queue reset.
+
+        Please note that using two different instances with the same data file
+        simultaneously is not recommended as it may lead to data corruption.
 
         Args:
             data_path: Path of the data file for this queue. e.g. `queue.dat`
             maxsize: If maxsize is less than or equal to zero, the queue size is infinite.
                 If it is an integer greater than 0, then put() blocks
                 when the queue reaches maxsize until an item is removed by get().
         """
         data_path = Path(data_path)
+        if data_path.suffix == ".bak":
+            raise ValueError("Invalid file name: .bak suffix is reserved for backups")
         queue = await cls._read_queue(data_path)
         return cls._create(data_path, maxsize, queue)
```

### Comparing `aiodiskqueue-0.1.0b1/src/aiodiskqueue/utils.py` & `aiodiskqueue-0.1.0b2/src/aiodiskqueue/utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/tests/factories.py` & `aiodiskqueue-0.1.0b2/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/tests/loadtest.py` & `aiodiskqueue-0.1.0b2/tests/loadtest.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/tests/test_core.py` & `aiodiskqueue-0.1.0b2/tests/test_core.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 
 import aiofiles
+import aiofiles.os
 
 from aiodiskqueue import Queue, QueueEmpty, QueueFull
 
 from .factories import ItemFactory
 from .helpers import QueueAsyncioTestCase
 
 
@@ -22,34 +23,61 @@
 
     async def test_creating_queue_with_maxsize_below_0_yields_unlimited_queue(self):
         # when
         q = await Queue.create(self.data_path, maxsize=-1)
         # then
         self.assertEqual(q.maxsize, 0)
 
-    async def test_should_create_new_file_when_current_file_is_corrupt(self):
+    async def test_do_not_allow_data_file_ending_on_bak(self):
+        # given
+        invalid_path = self.data_path.with_name("data.bak")
+        # when/then
+        with self.assertRaises(ValueError):
+            await Queue.create(invalid_path)
+
+    async def test_fail_at_creation_when_data_file_can_not_be_written(self):
+        # given
+        invalid_path = self.data_path.parent / "dead-end" / "queue.dat"
+        # when/then
+        with self.assertRaises(OSError):
+            await Queue.create(invalid_path)
+
+    async def test_should_reset_queue_and_backup_data_file_when_not_usable(self):
         # given
         async with aiofiles.open(self.data_path, "wb") as fp:
             await fp.write(b"invalid-data")
+        # when
         q = await Queue.create(self.data_path)
+        # then
+        self.assertEqual(q.qsize(), 0)
+        backup_path = self.data_path.with_suffix(".bak")
+        self.assertTrue(backup_path.exists())
+
+    async def test_should_overwrite_existing_backup(self):
+        # given
+        async with aiofiles.open(self.data_path, "wb") as fp:
+            await fp.write(b"invalid-data")
+        backup_path = self.data_path.with_suffix(".bak")
+        backup_path.touch()
         # when
-        result = q.qsize()
+        q = await Queue.create(self.data_path)
         # then
-        self.assertEqual(result, 0)
+        self.assertEqual(q.qsize(), 0)
+        self.assertTrue(backup_path.exists())
 
     async def test_should_preserve_queue_content(self):
         # given
         queue_1 = await Queue.create(self.data_path)
         item = ItemFactory()
         await queue_1.put_nowait(item)
-        # when
         del queue_1
+        # when
         queue_2 = await Queue.create(self.data_path)
-        item_new = await queue_2.get()
         # then
+        item_new = await queue_2.get()
         self.assertEqual(item_new, item)
 
 
 class TestPutIntoQueue(QueueAsyncioTestCase):
     async def test_should_put_items_and_measure_size(self):
         # given
         q = await Queue.create(self.data_path)
```

### Comparing `aiodiskqueue-0.1.0b1/tests/test_integration.py` & `aiodiskqueue-0.1.0b2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/tests/test_utils.py` & `aiodiskqueue-0.1.0b2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0b1/PKG-INFO` & `aiodiskqueue-0.1.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Persistent queue for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```


# Comparing `tmp/elkpy-1.1.7.tar.gz` & `tmp/elkpy-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkpy-1.1.7.tar", last modified: Fri May 19 04:56:58 2023, max compression
+gzip compressed data, was "elkpy-1.1.8.tar", last modified: Mon May 29 15:48:09 2023, max compression
```

## Comparing `elkpy-1.1.7.tar` & `elkpy-1.1.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-19 04:56:58.181955 elkpy-1.1.7/
--rw-r--r--   0 max        (501) staff       (20)    35148 2023-03-30 13:19:14.000000 elkpy-1.1.7/COPYING
--rw-r--r--   0 max        (501) staff       (20)    35128 2023-03-30 13:19:14.000000 elkpy-1.1.7/LICENSE
--rw-r--r--   0 max        (501) staff       (20)     5142 2023-05-19 04:56:58.182009 elkpy-1.1.7/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)     4447 2023-03-30 13:19:14.000000 elkpy-1.1.7/README.md
--rw-r--r--   0 max        (501) staff       (20)      757 2023-05-19 04:55:44.000000 elkpy-1.1.7/pyproject.toml
--rw-r--r--   0 max        (501) staff       (20)      352 2023-05-19 04:56:58.182226 elkpy-1.1.7/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)       69 2023-03-30 13:19:14.000000 elkpy-1.1.7/setup.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-19 04:56:58.176044 elkpy-1.1.7/src/
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-19 04:56:58.181303 elkpy-1.1.7/src/elkpy/
--rw-r--r--   0 max        (501) staff       (20)        0 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/__init__.py
--rw-r--r--   0 max        (501) staff       (20)    19397 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/audiographcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     9934 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/audioroutingcontroller.py
--rw-r--r--   0 max        (501) staff       (20)    16365 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/cvgatecontroller.py
--rw-r--r--   0 max        (501) staff       (20)     1989 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/grpc_gen.py
--rw-r--r--   0 max        (501) staff       (20)     8021 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/keyboardcontroller.py
--rw-r--r--   0 max        (501) staff       (20)    19656 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/midicontroller.py
--rw-r--r--   0 max        (501) staff       (20)    16458 2023-05-19 04:52:31.000000 elkpy-1.1.7/src/elkpy/notificationcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     5032 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/osccontroller.py
--rw-r--r--   0 max        (501) staff       (20)    15841 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/parametercontroller.py
--rw-r--r--   0 max        (501) staff       (20)     6506 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/programcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     3056 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/sessioncontroller.py
--rw-r--r--   0 max        (501) staff       (20)    22973 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/sushi_info_types.py
--rw-r--r--   0 max        (501) staff       (20)     6148 2023-05-19 04:53:24.000000 elkpy-1.1.7/src/elkpy/sushicontroller.py
--rw-r--r--   0 max        (501) staff       (20)     2143 2023-05-19 04:42:11.000000 elkpy-1.1.7/src/elkpy/sushierrors.py
--rw-r--r--   0 max        (501) staff       (20)     9701 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/sushiprocessor.py
--rw-r--r--   0 max        (501) staff       (20)     3024 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/systemcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     6641 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/timingcontroller.py
--rw-r--r--   0 max        (501) staff       (20)     7011 2023-05-15 14:56:03.000000 elkpy-1.1.7/src/elkpy/transportcontroller.py
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-19 04:56:58.181862 elkpy-1.1.7/src/elkpy.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     5142 2023-05-19 04:56:58.000000 elkpy-1.1.7/src/elkpy.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      790 2023-05-19 04:56:58.000000 elkpy-1.1.7/src/elkpy.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-05-19 04:56:58.000000 elkpy-1.1.7/src/elkpy.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       29 2023-05-19 04:56:58.000000 elkpy-1.1.7/src/elkpy.egg-info/requires.txt
--rw-r--r--   0 max        (501) staff       (20)        6 2023-05-19 04:56:58.000000 elkpy-1.1.7/src/elkpy.egg-info/top_level.txt
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-29 15:48:09.344503 elkpy-1.1.8/
+-rw-r--r--   0 max        (501) staff       (20)    35148 2023-03-30 13:19:14.000000 elkpy-1.1.8/COPYING
+-rw-r--r--   0 max        (501) staff       (20)    35128 2023-03-30 13:19:14.000000 elkpy-1.1.8/LICENSE
+-rw-r--r--   0 max        (501) staff       (20)     5142 2023-05-29 15:48:09.344569 elkpy-1.1.8/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)     4447 2023-03-30 13:19:14.000000 elkpy-1.1.8/README.md
+-rw-r--r--   0 max        (501) staff       (20)      757 2023-05-29 15:44:56.000000 elkpy-1.1.8/pyproject.toml
+-rw-r--r--   0 max        (501) staff       (20)      352 2023-05-29 15:48:09.344821 elkpy-1.1.8/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)       69 2023-03-30 13:19:14.000000 elkpy-1.1.8/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-29 15:48:09.338207 elkpy-1.1.8/src/
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-29 15:48:09.343798 elkpy-1.1.8/src/elkpy/
+-rw-r--r--   0 max        (501) staff       (20)        0 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/__init__.py
+-rw-r--r--   0 max        (501) staff       (20)    19397 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/audiographcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     9934 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/audioroutingcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    16365 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/cvgatecontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     1989 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/grpc_gen.py
+-rw-r--r--   0 max        (501) staff       (20)     8021 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/keyboardcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    19656 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/midicontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    16458 2023-05-29 15:36:29.000000 elkpy-1.1.8/src/elkpy/notificationcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     5032 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/osccontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    15841 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/parametercontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     6506 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/programcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     3056 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/sessioncontroller.py
+-rw-r--r--   0 max        (501) staff       (20)    22973 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/sushi_info_types.py
+-rw-r--r--   0 max        (501) staff       (20)     6148 2023-05-19 04:53:24.000000 elkpy-1.1.8/src/elkpy/sushicontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     2139 2023-05-29 15:35:31.000000 elkpy-1.1.8/src/elkpy/sushierrors.py
+-rw-r--r--   0 max        (501) staff       (20)     9701 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/sushiprocessor.py
+-rw-r--r--   0 max        (501) staff       (20)     3024 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/systemcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     6641 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/timingcontroller.py
+-rw-r--r--   0 max        (501) staff       (20)     7011 2023-05-15 14:56:03.000000 elkpy-1.1.8/src/elkpy/transportcontroller.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-05-29 15:48:09.344404 elkpy-1.1.8/src/elkpy.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     5142 2023-05-29 15:48:09.000000 elkpy-1.1.8/src/elkpy.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      790 2023-05-29 15:48:09.000000 elkpy-1.1.8/src/elkpy.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-05-29 15:48:09.000000 elkpy-1.1.8/src/elkpy.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       29 2023-05-29 15:48:09.000000 elkpy-1.1.8/src/elkpy.egg-info/requires.txt
+-rw-r--r--   0 max        (501) staff       (20)        6 2023-05-29 15:48:09.000000 elkpy-1.1.8/src/elkpy.egg-info/top_level.txt
```

### Comparing `elkpy-1.1.7/COPYING` & `elkpy-1.1.8/COPYING`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/LICENSE` & `elkpy-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/PKG-INFO` & `elkpy-1.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkpy
-Version: 1.1.7
+Version: 1.1.8
 Summary: A basic controller for sushi using gRPC
 Home-page: https://github.com/elkaudio/elkpy
 Author: Ruben Svensson
 Author-email: Maxime Gendebien <max@elk.audio>, Ruben Svensson <ruben@elk.audio>
 Project-URL: Homepage, https://github.com/elkaudio/elkpy
 Project-URL: Bug Tracker, https://github.com/elkaudio/elkpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `elkpy-1.1.7/README.md` & `elkpy-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/pyproject.toml` & `elkpy-1.1.8/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=59.5.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "elkpy"
-version = "1.1.7"
+version = "1.1.8"
 authors = [
   { name="Maxime Gendebien", email="max@elk.audio" },
   { name="Ruben Svensson", email="ruben@elk.audio" },
 ]
 description = "A basic controller for sushi using gRPC"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `elkpy-1.1.7/src/elkpy/audiographcontroller.py` & `elkpy-1.1.8/src/elkpy/audiographcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/audioroutingcontroller.py` & `elkpy-1.1.8/src/elkpy/audioroutingcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/cvgatecontroller.py` & `elkpy-1.1.8/src/elkpy/cvgatecontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/grpc_gen.py` & `elkpy-1.1.8/src/elkpy/grpc_gen.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/keyboardcontroller.py` & `elkpy-1.1.8/src/elkpy/keyboardcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/midicontroller.py` & `elkpy-1.1.8/src/elkpy/midicontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/notificationcontroller.py` & `elkpy-1.1.8/src/elkpy/notificationcontroller.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self._sushi_proto, self._sushi_grpc = grpc_gen.modules_from_proto(sushi_proto_def)
         self.tasks = []
         try:
             self.loop = asyncio.get_running_loop()
             self._async = True
         except RuntimeError:
             self._async = False
-            self.loop = asyncio.get_event_loop()
+            self.loop = asyncio.new_event_loop()
             self.notification_thread = Thread(target=self._run_notification_loop, args=(self.loop,))
             self.notification_thread.setDaemon(True)
             self.notification_thread.start()
 
     @staticmethod
     def _run_notification_loop(loop):
         """ Attaches the asyncio event loop to the thread and start looping over it.
```

### Comparing `elkpy-1.1.7/src/elkpy/osccontroller.py` & `elkpy-1.1.8/src/elkpy/osccontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/parametercontroller.py` & `elkpy-1.1.8/src/elkpy/parametercontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/programcontroller.py` & `elkpy-1.1.8/src/elkpy/programcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/sessioncontroller.py` & `elkpy-1.1.8/src/elkpy/sessioncontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/sushi_info_types.py` & `elkpy-1.1.8/src/elkpy/sushi_info_types.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/sushicontroller.py` & `elkpy-1.1.8/src/elkpy/sushicontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/sushierrors.py` & `elkpy-1.1.8/src/elkpy/sushierrors.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,10 +61,10 @@
     elif e.code().name == 'INVALID_ARGUMENT':
         raise SushiInvalidArgumentError(e.details(), context_info) from e
     elif e.code().name == 'INTERNAL':
         raise SushiInternalError(e.details(), context_info) from e
     elif e.code().name == 'UNAVAILABLE':
         raise SushiUnavailableError(e.details(), context_info) from e
     else:
-        if context_info is not '':
+        if context_info != '':
             print(context_info)
         raise e
```

### Comparing `elkpy-1.1.7/src/elkpy/sushiprocessor.py` & `elkpy-1.1.8/src/elkpy/sushiprocessor.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/systemcontroller.py` & `elkpy-1.1.8/src/elkpy/systemcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/timingcontroller.py` & `elkpy-1.1.8/src/elkpy/timingcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy/transportcontroller.py` & `elkpy-1.1.8/src/elkpy/transportcontroller.py`

 * *Files identical despite different names*

### Comparing `elkpy-1.1.7/src/elkpy.egg-info/PKG-INFO` & `elkpy-1.1.8/src/elkpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elkpy
-Version: 1.1.7
+Version: 1.1.8
 Summary: A basic controller for sushi using gRPC
 Home-page: https://github.com/elkaudio/elkpy
 Author: Ruben Svensson
 Author-email: Maxime Gendebien <max@elk.audio>, Ruben Svensson <ruben@elk.audio>
 Project-URL: Homepage, https://github.com/elkaudio/elkpy
 Project-URL: Bug Tracker, https://github.com/elkaudio/elkpy/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `elkpy-1.1.7/src/elkpy.egg-info/SOURCES.txt` & `elkpy-1.1.8/src/elkpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/hkkang_utils-0.1.91.tar.gz` & `tmp/hkkang_utils-0.1.92.tar.gz`

## Comparing `hkkang_utils-0.1.91.tar` & `hkkang_utils-0.1.92.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/.github/workflows/deploy_doc.yml
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/.github/workflows/unittest.yml
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/.vscode/settings.json
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/__init__.py
--rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/concurrent.py
--rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/file.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/io.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/list.py
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/logger.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/metrics.py
--rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/misc.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/ml.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/pattern.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/pg.py
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/slack.py
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/socket.py
--rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/sql.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/string.py
--rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/tensor.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/testing.py
--rw-r--r--   0        0        0     3337 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/src/hkkang_utils/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/__init__.py
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_concurrent.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_design.py
--rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_file.py
--rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_io.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_list.py
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_metrics.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_misc.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_sql.py
--rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_string.py
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_tensor.py
--rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_testing.py
--rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/tests/test_time.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/LICENSE
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/pyproject.toml
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 hkkang_utils-0.1.91/PKG-INFO
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/.github/workflows/deploy_doc.yml
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/.github/workflows/unittest.yml
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/.vscode/settings.json
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/__init__.py
+-rw-r--r--   0        0        0     5268 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/concurrent.py
+-rw-r--r--   0        0        0     6525 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/file.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/io.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/list.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/logger.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/metrics.py
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/misc.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/ml.py
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/pattern.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/pg.py
+-rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/slack.py
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/socket.py
+-rw-r--r--   0        0        0     4809 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/sql.py
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/string.py
+-rw-r--r--   0        0        0     3940 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/tensor.py
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/testing.py
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/src/hkkang_utils/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/__init__.py
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_concurrent.py
+-rw-r--r--   0        0        0     4364 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_file.py
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_io.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_list.py
+-rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_metrics.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_misc.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_pattern.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_sql.py
+-rw-r--r--   0        0        0     2010 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_string.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_tensor.py
+-rw-r--r--   0        0        0      802 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_testing.py
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/tests/test_time.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/LICENSE
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/pyproject.toml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 hkkang_utils-0.1.92/PKG-INFO
```

### Comparing `hkkang_utils-0.1.91/.github/workflows/deploy_doc.yml` & `hkkang_utils-0.1.92/.github/workflows/deploy_doc.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/.github/workflows/unittest.yml` & `hkkang_utils-0.1.92/.github/workflows/unittest.yml`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/__init__.py` & `hkkang_utils-0.1.92/src/hkkang_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/concurrent.py` & `hkkang_utils-0.1.92/src/hkkang_utils/concurrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     return text
 
 
 class Thread(threading.Thread):
     """Please use start method to start thread. start method will call run method.
     If you are doing cpu intensive task, please use MultiProcessor class instead of this class. It's much faster.
 
-    example:
+    Example:
         # Initialize threads
         thread1 = concurrent_utils.Thread(count_million_and_print_name, 1, {"name":"name_1"})
         thread2 = concurrent_utils.Thread(count_million_and_print_name, 2, {"name":"name_2"})
 
         # Start threads
         thread1.start()
         thread2.start()
```

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/file.py` & `hkkang_utils-0.1.92/src/hkkang_utils/file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/list.py` & `hkkang_utils-0.1.92/src/hkkang_utils/list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/metrics.py` & `hkkang_utils-0.1.92/src/hkkang_utils/metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/misc.py` & `hkkang_utils-0.1.92/src/hkkang_utils/misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/ml.py` & `hkkang_utils-0.1.92/src/hkkang_utils/ml.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/pattern.py` & `hkkang_utils-0.1.92/src/hkkang_utils/pattern.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,52 @@
 import abc
-from typing import Dict
+from typing import Callable, Dict
 
 
 # This file containes design patterns
 class SingletonMeta(type):
     """Meta Singleton class"""
 
-    _instances: Dict = dict()
+    _instances: Dict[str, Callable] = dict()
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances.keys():
             cls._instances[cls] = super(SingletonMeta, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 class SingletonABCMeta(abc.ABCMeta):
     """Abstract and meta Singleton class"""
 
-    _instances: Dict = dict()
+    _instances: Dict[str, Callable] = dict()
 
     def __call__(cls, *args, **kwargs):
         if cls not in cls._instances.keys():
             cls._instances[cls] = super(SingletonABCMeta, cls).__call__(*args, **kwargs)
         return cls._instances[cls]
 
 
 # Decorator
 def singleton(cls):
     """Singleton decorator"""
-    instance: Dict = None
+    instance: Dict[str, Callable] = None
 
     def wrapper(*args, **kwargs):
         nonlocal instance
         if instance is None:
             instance = cls(*args, **kwargs)
         return instance
 
     return wrapper
 
 
 class SingletonMetaWithArgs(type):
     """Meta Singleton class with arguments. One object is created for each set of arguments"""
 
-    _instances: Dict = dict()
+    _instances: Dict[str, Dict[str, Callable]] = dict()
 
     def __call__(cls, *args, **kwargs):
         # Get instance key
         instance_key = cls.__repr_args__(*args, **kwargs)
         if cls not in cls._instances.keys():
             cls._instances[cls] = dict()
         # Create instance if not exists
@@ -60,15 +60,15 @@
     def __repr_args__(*args, **kwargs):
         return str(args) + str(kwargs)
 
 
 class SingletonABCMetaWithArgs(abc.ABCMeta):
     """Abstract and Meta Singleton class with arguments. One object is created for each set of arguments"""
 
-    _instances: Dict = dict()
+    _instances: Dict[str, Dict[str, Callable]] = dict()
 
     def __call__(cls, *args, **kwargs):
         # Get instance key
         instance_key = cls.__repr_args__(*args, **kwargs)
         if cls not in cls._instances.keys():
             cls._instances[cls] = dict()
         # Create instance if not exists
```

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/pg.py` & `hkkang_utils-0.1.92/src/hkkang_utils/pg.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/slack.py` & `hkkang_utils-0.1.92/src/hkkang_utils/slack.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/sql.py` & `hkkang_utils-0.1.92/src/hkkang_utils/sql.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/string.py` & `hkkang_utils-0.1.92/src/hkkang_utils/string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/src/hkkang_utils/tensor.py` & `hkkang_utils-0.1.92/src/hkkang_utils/tensor.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/tests/test_concurrent.py` & `hkkang_utils-0.1.92/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/tests/test_design.py` & `hkkang_utils-0.1.92/tests/test_pattern.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/tests/test_file.py` & `hkkang_utils-0.1.92/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/tests/test_io.py` & `hkkang_utils-0.1.92/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/tests/test_list.py` & `hkkang_utils-0.1.92/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/tests/test_metrics.py` & `hkkang_utils-0.1.92/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/tests/test_misc.py` & `hkkang_utils-0.1.92/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/tests/test_string.py` & `hkkang_utils-0.1.92/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/tests/test_testing.py` & `hkkang_utils-0.1.92/tests/test_testing.py`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/.gitignore` & `hkkang_utils-0.1.92/.gitignore`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/LICENSE` & `hkkang_utils-0.1.92/LICENSE`

 * *Files identical despite different names*

### Comparing `hkkang_utils-0.1.91/pyproject.toml` & `hkkang_utils-0.1.92/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hkkang_utils"
-version = "0.1.91"
+version = "0.1.92"
 authors = [{name="Hyukkyu Kang", email="hyukkyukang@gmail.com"}]
 description = "A collection of useful util functions"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `hkkang_utils-0.1.91/PKG-INFO` & `hkkang_utils-0.1.92/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hkkang_utils
-Version: 0.1.91
+Version: 0.1.92
 Summary: A collection of useful util functions
 Project-URL: Homepage, https://github.com/hyukkyukang/python_utils
 Project-URL: Bug Tracker, https://github.com/hyukkyukang/python_utils/issues
 Author-email: Hyukkyu Kang <hyukkyukang@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


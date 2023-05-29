# Comparing `tmp/fxn-0.0.2.tar.gz` & `tmp/fxn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fxn-0.0.2.tar", last modified: Mon May 29 01:02:25 2023, max compression
+gzip compressed data, was "fxn-0.0.3.tar", last modified: Mon May 29 01:08:36 2023, max compression
```

## Comparing `fxn-0.0.2.tar` & `fxn-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:25.681276 fxn-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 01:02:04.000000 fxn-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 01:02:25.677276 fxn-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 01:02:04.000000 fxn-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:25.677276 fxn-0.0.2/fxn/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:25.677276 fxn-0.0.2/fxn/api/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/featureinput.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:25.677276 fxn-0.0.2/fxn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:25.677276 fxn-0.0.2/fxn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 01:02:25.681276 fxn-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-29 01:02:04.000000 fxn-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:08:36.652347 fxn-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 01:08:20.000000 fxn-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 01:08:36.652347 fxn-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 01:08:20.000000 fxn-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:08:36.648347 fxn-0.0.3/fxn/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:08:36.652347 fxn-0.0.3/fxn/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/featureinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7719 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:08:36.652347 fxn-0.0.3/fxn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/cli/predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 01:08:20.000000 fxn-0.0.3/fxn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:08:36.648347 fxn-0.0.3/fxn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 01:08:36.000000 fxn-0.0.3/fxn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 01:08:36.000000 fxn-0.0.3/fxn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 01:08:36.000000 fxn-0.0.3/fxn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 01:08:36.000000 fxn-0.0.3/fxn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 01:08:36.000000 fxn-0.0.3/fxn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 01:08:36.000000 fxn-0.0.3/fxn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 01:08:36.652347 fxn-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-29 01:08:20.000000 fxn-0.0.3/setup.py
```

### Comparing `fxn-0.0.2/LICENSE` & `fxn-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/PKG-INFO` & `fxn-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.2
+Version: 0.0.3
 Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
```

### Comparing `fxn-0.0.2/fxn/api/api.py` & `fxn-0.0.3/fxn/api/api.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/api/dtype.py` & `fxn-0.0.3/fxn/api/dtype.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/api/featureinput.py` & `fxn-0.0.3/fxn/api/featureinput.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/api/predictor.py` & `fxn-0.0.3/fxn/api/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 from .api import query
 from .dtype import Dtype
 from .profile import Profile
 from .storage import Storage, UploadType
 
 @dataclass(frozen=True)
-class Predictor:
+class Predictor: # INCOMPLETE # `create`
     """
     Predictor.
 
     Members:
         tag (str): Predictor tag.
         owner (Profile): Predictor owner.
         name (str): Predictor name.
```

### Comparing `fxn-0.0.2/fxn/api/profile.py` & `fxn-0.0.3/fxn/api/profile.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/api/storage.py` & `fxn-0.0.3/fxn/api/storage.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/api/tag.py` & `fxn-0.0.3/fxn/api/tag.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/api/user.py` & `fxn-0.0.3/fxn/api/user.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/cli/__init__.py` & `fxn-0.0.3/fxn/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/cli/auth.py` & `fxn-0.0.3/fxn/cli/auth.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/cli/misc.py` & `fxn-0.0.3/fxn/cli/misc.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/cli/predictors.py` & `fxn-0.0.3/fxn/cli/predictors.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn/cli/users.py` & `fxn-0.0.3/fxn/cli/users.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/fxn.egg-info/PKG-INFO` & `fxn-0.0.3/fxn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.2
+Version: 0.0.3
 Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
```

### Comparing `fxn-0.0.2/fxn.egg-info/SOURCES.txt` & `fxn-0.0.3/fxn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fxn-0.0.2/setup.py` & `fxn-0.0.3/setup.py`

 * *Files identical despite different names*


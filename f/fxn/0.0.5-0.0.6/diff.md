# Comparing `tmp/fxn-0.0.5.tar.gz` & `tmp/fxn-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fxn-0.0.5.tar", last modified: Mon May 29 16:53:41 2023, max compression
+gzip compressed data, was "fxn-0.0.6.tar", last modified: Mon May 29 20:25:44 2023, max compression
```

## Comparing `fxn-0.0.5.tar` & `fxn-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:41.941251 fxn-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 16:53:24.000000 fxn-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 16:53:41.941251 fxn-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 16:53:24.000000 fxn-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:41.937251 fxn-0.0.5/fxn/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:41.937251 fxn-0.0.5/fxn/api/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/featureinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:41.941251 fxn-0.0.5/fxn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:41.937251 fxn-0.0.5/fxn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:53:41.941251 fxn-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-29 16:53:24.000000 fxn-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:25:44.134987 fxn-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 20:25:24.000000 fxn-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 20:25:44.134987 fxn-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 20:25:24.000000 fxn-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:25:44.130987 fxn-0.0.6/fxn/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:25:44.130987 fxn-0.0.6/fxn/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/featureinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:25:44.134987 fxn-0.0.6/fxn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/cli/predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 20:25:24.000000 fxn-0.0.6/fxn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:25:44.130987 fxn-0.0.6/fxn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 20:25:44.000000 fxn-0.0.6/fxn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 20:25:44.000000 fxn-0.0.6/fxn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:25:44.000000 fxn-0.0.6/fxn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 20:25:44.000000 fxn-0.0.6/fxn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 20:25:44.000000 fxn-0.0.6/fxn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 20:25:44.000000 fxn-0.0.6/fxn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 20:25:44.134987 fxn-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-29 20:25:24.000000 fxn-0.0.6/setup.py
```

### Comparing `fxn-0.0.5/LICENSE` & `fxn-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/PKG-INFO` & `fxn-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.5
+Version: 0.0.6
 Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
```

### Comparing `fxn-0.0.5/fxn/api/api.py` & `fxn-0.0.6/fxn/api/api.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/api/dtype.py` & `fxn-0.0.6/fxn/api/dtype.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/api/featureinput.py` & `fxn-0.0.6/fxn/api/featureinput.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/api/prediction.py` & `fxn-0.0.6/fxn/api/prediction.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/api/predictor.py` & `fxn-0.0.6/fxn/api/predictor.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/api/profile.py` & `fxn-0.0.6/fxn/api/profile.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/api/storage.py` & `fxn-0.0.6/fxn/api/storage.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/api/tag.py` & `fxn-0.0.6/fxn/api/tag.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/api/user.py` & `fxn-0.0.6/fxn/api/user.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/cli/__init__.py` & `fxn-0.0.6/fxn/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/cli/auth.py` & `fxn-0.0.6/fxn/cli/auth.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/cli/misc.py` & `fxn-0.0.6/fxn/cli/misc.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/cli/predict.py` & `fxn-0.0.6/fxn/cli/predict.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn/cli/predictors.py` & `fxn-0.0.6/fxn/cli/predictors.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,17 @@
     acceleration: Acceleration=Option(None, case_sensitive=False, help="Cloud predictor acceleration. This defaults to `CPU`."),
     environment: List[str]=Option([], help="Predictor environment variables."),
     license: str=Option(None, help="Predictor license URL."),
     overwrite: bool=Option(None, "--overwrite", help="Overwrite any existing predictor with the same tag.")
 ):
     environment = { e.split("=")[0].strip(): e.split("=")[1].strip() for e in environment }
     predictor = Predictor.create(
-        tag,
-        type,
-        notebook,
+        tag=tag
+        notebook=notebook,
+        type=type,
         access=access,
         description=description,
         media=media,
         acceleration=acceleration,
         environment=environment,
         license=license,
         overwrite=overwrite
```

### Comparing `fxn-0.0.5/fxn/cli/users.py` & `fxn-0.0.6/fxn/cli/users.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/fxn.egg-info/PKG-INFO` & `fxn-0.0.6/fxn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.5
+Version: 0.0.6
 Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
```

### Comparing `fxn-0.0.5/fxn.egg-info/SOURCES.txt` & `fxn-0.0.6/fxn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fxn-0.0.5/setup.py` & `fxn-0.0.6/setup.py`

 * *Files identical despite different names*


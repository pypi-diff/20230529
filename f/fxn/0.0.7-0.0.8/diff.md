# Comparing `tmp/fxn-0.0.7.tar.gz` & `tmp/fxn-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fxn-0.0.7.tar", last modified: Mon May 29 20:33:39 2023, max compression
+gzip compressed data, was "fxn-0.0.8.tar", last modified: Mon May 29 20:40:37 2023, max compression
```

## Comparing `fxn-0.0.7.tar` & `fxn-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:33:39.427903 fxn-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 20:33:23.000000 fxn-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 20:33:39.427903 fxn-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 20:33:23.000000 fxn-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:33:39.427903 fxn-0.0.7/fxn/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:33:39.427903 fxn-0.0.7/fxn/api/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/featureinput.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:33:39.427903 fxn-0.0.7/fxn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/cli/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/cli/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3242 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/cli/predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 20:33:23.000000 fxn-0.0.7/fxn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:33:39.427903 fxn-0.0.7/fxn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 20:33:39.000000 fxn-0.0.7/fxn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 20:33:39.000000 fxn-0.0.7/fxn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:33:39.000000 fxn-0.0.7/fxn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 20:33:39.000000 fxn-0.0.7/fxn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 20:33:39.000000 fxn-0.0.7/fxn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 20:33:39.000000 fxn-0.0.7/fxn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 20:33:39.427903 fxn-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-29 20:33:23.000000 fxn-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:40:37.663996 fxn-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 20:40:20.000000 fxn-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 20:40:37.663996 fxn-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 20:40:20.000000 fxn-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:40:37.659996 fxn-0.0.8/fxn/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:40:37.659996 fxn-0.0.8/fxn/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/featureinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:40:37.663996 fxn-0.0.8/fxn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 20:40:20.000000 fxn-0.0.8/fxn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:40:37.659996 fxn-0.0.8/fxn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 20:40:37.000000 fxn-0.0.8/fxn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 20:40:37.663996 fxn-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-29 20:40:20.000000 fxn-0.0.8/setup.py
```

### Comparing `fxn-0.0.7/LICENSE` & `fxn-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/PKG-INFO` & `fxn-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.7
+Version: 0.0.8
 Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
```

### Comparing `fxn-0.0.7/fxn/api/api.py` & `fxn-0.0.8/fxn/api/api.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/api/dtype.py` & `fxn-0.0.8/fxn/api/dtype.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/api/featureinput.py` & `fxn-0.0.8/fxn/api/featureinput.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/api/prediction.py` & `fxn-0.0.8/fxn/api/prediction.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/api/predictor.py` & `fxn-0.0.8/fxn/api/predictor.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/api/profile.py` & `fxn-0.0.8/fxn/api/profile.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/api/storage.py` & `fxn-0.0.8/fxn/api/storage.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/api/tag.py` & `fxn-0.0.8/fxn/api/tag.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/api/user.py` & `fxn-0.0.8/fxn/api/user.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/cli/__init__.py` & `fxn-0.0.8/fxn/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/cli/auth.py` & `fxn-0.0.8/fxn/cli/auth.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/cli/misc.py` & `fxn-0.0.8/fxn/cli/misc.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/fxn/cli/predict.py` & `fxn-0.0.8/fxn/cli/predict.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,20 @@
 def predict (
     tag: str = Argument(..., help="Predictor tag."),
     raw_outputs: bool = Option(False, "--raw-outputs", help="Generate raw output features instead of parsing."),
     context: Context = 0
 ):
     # Predict
     inputs = { context.args[i].replace("-", ""): _parse_value(context.args[i+1]) for i in range(0, len(context.args), 2) }
-    prediction = Prediction.create(tag, **inputs, raw_outputs=raw_outputs, access_key=get_access_key())
+    prediction = Prediction.create(
+        tag=tag,
+        **inputs,
+        raw_outputs=raw_outputs,
+        access_key=get_access_key()
+    )
     # Parse results
     if hasattr(prediction, "results"):
         images = [feature for feature in prediction.results if isinstance(feature, Image.Image)]
         results = [_serialize_feature(feature) for feature in prediction.results]
         object.__setattr__(prediction, "results", results)
     # Print
     print_json(data=asdict(prediction))
```

### Comparing `fxn-0.0.7/fxn/cli/predictors.py` & `fxn-0.0.8/fxn/cli/predictors.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,25 +15,33 @@
 
 app = Typer(no_args_is_help=True)
 
 @app.command(name="retrieve", help="Retrieve a predictor.")
 def retrieve_predictor (
     tag: str=Argument(..., help="Predictor tag.")
 ):
-    predictor = Predictor.retrieve(tag, access_key=get_access_key())
+    predictor = Predictor.retrieve(
+        tag=tag,
+        access_key=get_access_key()
+    )
     predictor = asdict(predictor) if predictor else None
     print_json(data=predictor)
 
 @app.command(name="search", help="Search predictors.")
 def search_predictors (
     query: str=Argument(..., help="Search query."),
     offset: int=Option(None, help="Pagination offset."),
     count: int=Option(None, help="Pagination count.")
 ):
-    predictors = Predictor.search(query=query, offset=offset, count=count, access_key=get_access_key())
+    predictors = Predictor.search(
+        query=query,
+        offset=offset,
+        count=count,
+        access_key=get_access_key()
+    )
     predictors = [asdict(predictor) for predictor in predictors]
     print_json(data=predictors)
 
 @app.command(name="create", help="Create a predictor.")
 def create_predictor (
     tag: str=Argument(..., help="Predictor tag."),
     notebook: Path=Argument(..., help="Path to predictor notebook."),
@@ -53,31 +61,38 @@
         type=type,
         access=access,
         description=description,
         media=media,
         acceleration=acceleration,
         environment=environment,
         license=license,
-        overwrite=overwrite
+        overwrite=overwrite,
+        access_key=get_access_key()
     )
     predictor = asdict(predictor)
     print_json(data=predictor)
 
 @app.command(name="delete", help="Delete a predictor.")
 def delete_predictor (
     tag: str=Argument(..., help="Predictor tag.")
 ):
-    result = Predictor.delete(tag, access_key=get_access_key())
+    result = Predictor.delete(
+        tag=tag,
+        access_key=get_access_key()
+    )
     print_json(data=result)
 
 @app.command(name="archive", help="Archive an active predictor.")
 def archive_predictor (
     tag: str=Argument(..., help="Predictor tag.")
 ):
-    predictor = Predictor.archive(tag, access_key=get_access_key())
+    predictor = Predictor.archive(
+        tag=tag,
+        access_key=get_access_key()
+    )
     print_json(data=asdict(predictor))
 
 @app.callback()
 def predictor_options (
     learn: bool = Option(None, "--learn", callback=create_learn_callback("https://docs.fxn.ai/predictors"), help="Learn about predictors in Function.")
 ):
     pass
```

### Comparing `fxn-0.0.7/fxn/cli/users.py` & `fxn-0.0.8/fxn/cli/users.py`

 * *Files 24% similar despite different names*

```diff
@@ -12,10 +12,13 @@
 
 app = Typer(no_args_is_help=True)
 
 @app.command(name="retrieve", help="Retrieve a user.")
 def retrieve_user (
     username: str=Argument(..., help="Username.")
 ):
-    user = User.retrieve(username, access_key=get_access_key())
+    user = User.retrieve(
+        username=username,
+        access_key=get_access_key()
+    )
     user = asdict(user) if user else None
     print_json(data=user)
```

### Comparing `fxn-0.0.7/fxn.egg-info/PKG-INFO` & `fxn-0.0.8/fxn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.7
+Version: 0.0.8
 Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
```

### Comparing `fxn-0.0.7/fxn.egg-info/SOURCES.txt` & `fxn-0.0.8/fxn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fxn-0.0.7/setup.py` & `fxn-0.0.8/setup.py`

 * *Files identical despite different names*


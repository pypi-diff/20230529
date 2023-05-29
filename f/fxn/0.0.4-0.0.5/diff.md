# Comparing `tmp/fxn-0.0.4.tar.gz` & `tmp/fxn-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fxn-0.0.4.tar", last modified: Mon May 29 11:46:10 2023, max compression
+gzip compressed data, was "fxn-0.0.5.tar", last modified: Mon May 29 16:53:41 2023, max compression
```

## Comparing `fxn-0.0.4.tar` & `fxn-0.0.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:46:10.869248 fxn-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 11:45:54.000000 fxn-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 11:46:10.869248 fxn-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 11:45:54.000000 fxn-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:46:10.865247 fxn-0.0.4/fxn/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:46:10.869248 fxn-0.0.4/fxn/api/
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/dtype.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/featureinput.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/prediction.py
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:46:10.869248 fxn-0.0.4/fxn/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/cli/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/cli/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/cli/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/cli/predictors.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/cli/users.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 11:45:54.000000 fxn-0.0.4/fxn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:46:10.865247 fxn-0.0.4/fxn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 11:46:10.000000 fxn-0.0.4/fxn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 11:46:10.000000 fxn-0.0.4/fxn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:46:10.000000 fxn-0.0.4/fxn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 11:46:10.000000 fxn-0.0.4/fxn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 11:46:10.000000 fxn-0.0.4/fxn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 11:46:10.000000 fxn-0.0.4/fxn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 11:46:10.869248 fxn-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-29 11:45:54.000000 fxn-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:41.941251 fxn-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 16:53:24.000000 fxn-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 16:53:41.941251 fxn-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 16:53:24.000000 fxn-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:41.937251 fxn-0.0.5/fxn/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:41.937251 fxn-0.0.5/fxn/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/featureinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:41.941251 fxn-0.0.5/fxn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 16:53:24.000000 fxn-0.0.5/fxn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:41.937251 fxn-0.0.5/fxn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 16:53:41.000000 fxn-0.0.5/fxn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:53:41.941251 fxn-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-29 16:53:24.000000 fxn-0.0.5/setup.py
```

### Comparing `fxn-0.0.4/LICENSE` & `fxn-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/PKG-INFO` & `fxn-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.4
+Version: 0.0.5
 Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
```

### Comparing `fxn-0.0.4/fxn/api/api.py` & `fxn-0.0.5/fxn/api/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,14 +21,17 @@
     """
     access_key = access_key or fxn.access_key
     headers = { "Authorization": f"Bearer {access_key}" } if access_key else { }
     response = post(
         fxn.api_url,
         json={ "query": query, "variables": variables },
         headers=headers
-    ).json()
+    )
+    # Check
+    response.raise_for_status()
+    response = response.json()
     # Check error
     if "errors" in response:
         raise RuntimeError(response["errors"][0]["message"])
     # Return
     result = response["data"]
     return result
```

### Comparing `fxn-0.0.4/fxn/api/dtype.py` & `fxn-0.0.5/fxn/api/dtype.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/fxn/api/featureinput.py` & `fxn-0.0.5/fxn/api/featureinput.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/fxn/api/predictor.py` & `fxn-0.0.5/fxn/api/predictor.py`

 * *Files 3% similar despite different names*

```diff
@@ -153,33 +153,33 @@
         # Return
         return predictors
     
     @classmethod
     def create (
         cls,
         tag: str,
-        type: PredictorType,
         notebook: Union[str, Path],
+        type: PredictorType=None,
         access: AccessMode=None,
         description: str=None,
         media: Union[str, Path]=None,
         acceleration: Acceleration=None,
         environment: Dict[str, str]=None,
         license: str=None,
         overwrite: bool=None,
         access_key: str=None
     ) -> Predictor:
         """
         Create a predictor.
 
         Parameters:
             tag (str): Predictor tag.
-            type (PredictorType): Predictor type.
             notebook (str | Path): Predictor notebook path or URL.
-            access (AccessMode): Predictor access mode. This defaults to public.
+            type (PredictorType): Predictor type. This defaults to `CLOUD`.
+            access (AccessMode): Predictor access mode. This defaults to `PUBLIC`.
             description (str): Predictor description. This supports Markdown.
             media (str | Path): Predictor media path or URL.
             acceleration (Acceleration): Predictor acceleration. This only applies for cloud predictors and defaults to `CPU`. 
             environment (dict): Predictor environment variables.
             license (str): Predictor license URL.
             overwrite (bool): Overwrite any existing predictor with the same tag. Existing predictor will be deleted.
             access_key (str): Function access key.
```

### Comparing `fxn-0.0.4/fxn/api/profile.py` & `fxn-0.0.5/fxn/api/profile.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/fxn/api/storage.py` & `fxn-0.0.5/fxn/api/storage.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/fxn/api/tag.py` & `fxn-0.0.5/fxn/api/tag.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/fxn/api/user.py` & `fxn-0.0.5/fxn/api/user.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/fxn/cli/__init__.py` & `fxn-0.0.5/fxn/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/fxn/cli/auth.py` & `fxn-0.0.5/fxn/cli/auth.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/fxn/cli/misc.py` & `fxn-0.0.5/fxn/cli/misc.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/fxn/cli/predictors.py` & `fxn-0.0.5/fxn/cli/predictors.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 #   Copyright © 2023 NatML Inc. All Rights Reserved.
 #
 
 from dataclasses import asdict
 from rich import print_json
 from pathlib import Path
 from typer import Argument, Option, Typer
-from typing import List, Optional, Tuple
-from typing_extensions import Annotated
+from typing import List
 
-from ..api import Acceleration, AccessMode, Predictor, PredictorStatus, PredictorType
+from ..api import Acceleration, AccessMode, Predictor, PredictorType
 from .auth import get_access_key
 from .misc import create_learn_callback
 
 app = Typer(no_args_is_help=True)
 
 @app.command(name="retrieve", help="Retrieve a predictor.")
 def retrieve_predictor (
@@ -33,23 +32,23 @@
     predictors = Predictor.search(query=query, offset=offset, count=count, access_key=get_access_key())
     predictors = [asdict(predictor) for predictor in predictors]
     print_json(data=predictors)
 
 @app.command(name="create", help="Create a predictor.")
 def create_predictor (
     tag: str=Argument(..., help="Predictor tag."),
-    type: PredictorType=Argument(..., case_sensitive=False, help="Predictor type."),
     notebook: Path=Argument(..., help="Path to predictor notebook."),
-    access: AccessMode=Option(None, case_sensitive=False, help="Predictor access mode."),
-    description: str=Option(None, help="Predictor description."),
-    media: Path=Option(None, help="Predictor image."),
-    acceleration: Acceleration=Option(None, case_sensitive=False, help="Predictor acceleration."),
-    environment: Annotated[Optional[List[str]], Option(default=[], help="Predictor environment variables.")] = None,
+    type: PredictorType=Option(None, case_sensitive=False, help="Predictor type. This defaults to `CLOUD`."),
+    access: AccessMode=Option(None, case_sensitive=False, help="Predictor access mode. This defaults to `PUBLIC`."),
+    description: str=Option(None, help="Predictor description. This supports Markdown."),
+    media: Path=Option(None, help="Predictor image path."),
+    acceleration: Acceleration=Option(None, case_sensitive=False, help="Cloud predictor acceleration. This defaults to `CPU`."),
+    environment: List[str]=Option([], help="Predictor environment variables."),
     license: str=Option(None, help="Predictor license URL."),
-    overwrite: Annotated[bool, Option("--overwrite")] = None
+    overwrite: bool=Option(None, "--overwrite", help="Overwrite any existing predictor with the same tag.")
 ):
     environment = { e.split("=")[0].strip(): e.split("=")[1].strip() for e in environment }
     predictor = Predictor.create(
         tag,
         type,
         notebook,
         access=access,
```

### Comparing `fxn-0.0.4/fxn/cli/users.py` & `fxn-0.0.5/fxn/cli/users.py`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/fxn.egg-info/PKG-INFO` & `fxn-0.0.5/fxn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.4
+Version: 0.0.5
 Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
```

### Comparing `fxn-0.0.4/fxn.egg-info/SOURCES.txt` & `fxn-0.0.5/fxn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fxn-0.0.4/setup.py` & `fxn-0.0.5/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/datasieve-0.0.8.tar.gz` & `tmp/datasieve-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.0.8.tar", max compression
+gzip compressed data, was "datasieve-0.0.9.tar", max compression
```

## Comparing `datasieve-0.0.8.tar` & `datasieve-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2023-05-29 13:19:56.825087 datasieve-0.0.8/LICENSE
--rw-r--r--   0        0        0    11157 2023-05-29 13:19:56.825087 datasieve-0.0.8/README.md
--rw-r--r--   0        0        0        0 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/__init__.py
--rw-r--r--   0        0        0     7153 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/pipeline.py
--rw-r--r--   0        0        0      575 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     5739 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     3137 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1158 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/minmax_scaler.py
--rw-r--r--   0        0        0     1567 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1725 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1432 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     3058 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/utils.py
--rw-r--r--   0        0        0      544 2023-05-29 13:19:56.825087 datasieve-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    11783 1970-01-01 00:00:00.000000 datasieve-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-29 14:46:28.629256 datasieve-0.0.9/LICENSE
+-rw-r--r--   0        0        0    11157 2023-05-29 14:46:28.629256 datasieve-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/__init__.py
+-rw-r--r--   0        0        0     7210 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/pipeline.py
+-rw-r--r--   0        0        0      575 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     5739 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     3137 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1158 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/minmax_scaler.py
+-rw-r--r--   0        0        0     1567 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1725 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1432 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3058 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/utils.py
+-rw-r--r--   0        0        0      544 2023-05-29 14:46:28.629256 datasieve-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    11783 1970-01-01 00:00:00.000000 datasieve-0.0.9/PKG-INFO
```

### Comparing `datasieve-0.0.8/LICENSE` & `datasieve-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.8/README.md` & `datasieve-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.8/datasieve/pipeline.py` & `datasieve-0.0.9/datasieve/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import logging
-from typing import List, Tuple
+from typing import List, Tuple, Dict
 import numpy.typing as npt
 import pandas as pd
 import numpy as np
 import copy
 
 logger = logging.getLogger('datasieve.pipeline')
 
 
 class Pipeline:
 
     def __init__(self, steps: List[Tuple] = [],
-                 fitparams: dict[str, dict] = {}):
+                 fitparams: Dict[str, dict] = {}):
         """
         Pipeline object which holds a list of fit/transform objects.
         :param steps: list of tuples (str, transform())
         :param fitparams: dictionary of dictionaries, where the string key
         matches the str used to name the step in the steps list.
         """
         self.steps: List[Tuple] = steps
-        self.fitparams: dict[str, dict] = self._validate_fitparams(fitparams, steps)
+        self.fitparams: Dict[str, dict] = self._validate_fitparams(fitparams, steps)
         self.pandas_types: bool = False
         self.feature_list: list = []
         self.label_list: list = []
 
-    def _validate_fitparams(self, fitparams: dict[str, dict], steps: List[Tuple]):
+    def _validate_fitparams(self, fitparams: Dict[str, dict], steps: List[Tuple]):
         for _, (name, _) in enumerate(steps):
             if name not in fitparams.keys():
                 fitparams[name] = {}  # add an empty dict
 
         return fitparams
-    
+
     def __getitem__(self, name: str):
         for _, (step_name, step) in enumerate(self.steps):
             if step_name == name:
                 return step
 
         logger.warning(f"Could not find step {name} in pipeline, returning None")
         return None
@@ -60,17 +60,18 @@
             )
 
         X, y, sample_weight = self._convert_back_to_df(X, y, sample_weight, feature_list)
 
         return X, y, sample_weight
 
     def transform(self, X, y=None, sample_weight=None, outlier_check=False) -> Tuple[npt.ArrayLike,
-                                                                npt.ArrayLike,
-                                                                npt.ArrayLike]:
-        X, y, sample_weight = self._validate_arguments(X, y, sample_weight, outlier_check=outlier_check)
+                                                                                     npt.ArrayLike,
+                                                                                     npt.ArrayLike]:
+        X, y, sample_weight = self._validate_arguments(
+            X, y, sample_weight, outlier_check=outlier_check)
         feature_list = copy.deepcopy(self.feature_list)
 
         for _, (name, trans) in enumerate(self.steps):
             logger.debug(f"Transforming {name}")
             X, y, sample_weight, feature_list = trans.transform(
                 X,
                 y,
```

### Comparing `datasieve-0.0.8/datasieve/transforms/__init__.py` & `datasieve-0.0.9/datasieve/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.8/datasieve/transforms/dbscan.py` & `datasieve-0.0.9/datasieve/transforms/dbscan.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.8/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.0.9/datasieve/transforms/dissimilarity_index.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.8/datasieve/transforms/minmax_scaler.py` & `datasieve-0.0.9/datasieve/transforms/minmax_scaler.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.8/datasieve/transforms/pca.py` & `datasieve-0.0.9/datasieve/transforms/pca.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.8/datasieve/transforms/svm_outlier_extractor.py` & `datasieve-0.0.9/datasieve/transforms/svm_outlier_extractor.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.8/datasieve/transforms/variance_threshold.py` & `datasieve-0.0.9/datasieve/transforms/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.8/datasieve/utils.py` & `datasieve-0.0.9/datasieve/utils.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.8/pyproject.toml` & `datasieve-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.0.8"
+version = "0.0.9"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `datasieve-0.0.8/PKG-INFO` & `datasieve-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasieve
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
 License: MIT
 Author: Robert Caulk
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


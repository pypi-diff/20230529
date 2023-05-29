# Comparing `tmp/datasieve-0.0.6.tar.gz` & `tmp/datasieve-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.0.6.tar", max compression
+gzip compressed data, was "datasieve-0.0.8.tar", max compression
```

## Comparing `datasieve-0.0.6.tar` & `datasieve-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2023-05-26 18:39:04.053830 datasieve-0.0.6/LICENSE
--rw-r--r--   0        0        0    11157 2023-05-26 18:39:04.053830 datasieve-0.0.6/README.md
--rw-r--r--   0        0        0        0 2023-05-26 18:39:04.053830 datasieve-0.0.6/datasieve/__init__.py
--rw-r--r--   0        0        0     7110 2023-05-26 18:39:04.053830 datasieve-0.0.6/datasieve/pipeline.py
--rw-r--r--   0        0        0      575 2023-05-26 18:39:04.053830 datasieve-0.0.6/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     5739 2023-05-26 18:39:04.053830 datasieve-0.0.6/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     3137 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1158 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/transforms/minmax_scaler.py
--rw-r--r--   0        0        0     1567 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1725 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1432 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     3058 2023-05-26 18:39:04.057830 datasieve-0.0.6/datasieve/utils.py
--rw-r--r--   0        0        0      542 2023-05-26 18:39:04.057830 datasieve-0.0.6/pyproject.toml
--rw-r--r--   0        0        0    11797 1970-01-01 00:00:00.000000 datasieve-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-29 13:19:56.825087 datasieve-0.0.8/LICENSE
+-rw-r--r--   0        0        0    11157 2023-05-29 13:19:56.825087 datasieve-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/__init__.py
+-rw-r--r--   0        0        0     7153 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/pipeline.py
+-rw-r--r--   0        0        0      575 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     5739 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     3137 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1158 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/minmax_scaler.py
+-rw-r--r--   0        0        0     1567 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1725 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1432 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3058 2023-05-29 13:19:56.825087 datasieve-0.0.8/datasieve/utils.py
+-rw-r--r--   0        0        0      544 2023-05-29 13:19:56.825087 datasieve-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    11783 1970-01-01 00:00:00.000000 datasieve-0.0.8/PKG-INFO
```

### Comparing `datasieve-0.0.6/LICENSE` & `datasieve-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.6/README.md` & `datasieve-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.6/datasieve/pipeline.py` & `datasieve-0.0.8/datasieve/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,21 @@
     def _validate_fitparams(self, fitparams: dict[str, dict], steps: List[Tuple]):
         for _, (name, _) in enumerate(steps):
             if name not in fitparams.keys():
                 fitparams[name] = {}  # add an empty dict
 
         return fitparams
     
-    def get_step(self, name: str):
+    def __getitem__(self, name: str):
         for _, (step_name, step) in enumerate(self.steps):
             if step_name == name:
                 return step
 
-        raise Exception(f"Step {name} not found in pipeline")
+        logger.warning(f"Could not find step {name} in pipeline, returning None")
+        return None
 
     def fit_transform(self, X, y=None, sample_weight=None) -> Tuple[npt.ArrayLike,
                                                                     npt.ArrayLike,
                                                                     npt.ArrayLike]:
         """
         Iterate through the pipeline calling fit_transform() on each of the
         transformations
```

### Comparing `datasieve-0.0.6/datasieve/transforms/__init__.py` & `datasieve-0.0.8/datasieve/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.6/datasieve/transforms/dbscan.py` & `datasieve-0.0.8/datasieve/transforms/dbscan.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.6/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.0.8/datasieve/transforms/dissimilarity_index.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.6/datasieve/transforms/minmax_scaler.py` & `datasieve-0.0.8/datasieve/transforms/minmax_scaler.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.6/datasieve/transforms/pca.py` & `datasieve-0.0.8/datasieve/transforms/pca.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.6/datasieve/transforms/svm_outlier_extractor.py` & `datasieve-0.0.8/datasieve/transforms/svm_outlier_extractor.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.6/datasieve/transforms/variance_threshold.py` & `datasieve-0.0.8/datasieve/transforms/variance_threshold.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.6/datasieve/utils.py` & `datasieve-0.0.8/datasieve/utils.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.6/PKG-INFO` & `datasieve-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: datasieve
-Version: 0.0.6
+Version: 0.0.8
 Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
 License: MIT
 Author: Robert Caulk
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pandas (>=1.3.3,<2.0.0)
-Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
+Requires-Dist: pandas (>=1.3.3)
+Requires-Dist: scikit-learn (>=1.1.3)
 Description-Content-Type: text/markdown
 
 # DataSieve
 
 DataSieve is very similar to the SKlearn Pipeline in that it:
 
 - fits an arbitrary series of transformations to an array X
```


# Comparing `tmp/datasieve-0.0.9.tar.gz` & `tmp/datasieve-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasieve-0.0.9.tar", max compression
+gzip compressed data, was "datasieve-0.1.0.tar", max compression
```

## Comparing `datasieve-0.0.9.tar` & `datasieve-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1059 2023-05-29 14:46:28.629256 datasieve-0.0.9/LICENSE
--rw-r--r--   0        0        0    11157 2023-05-29 14:46:28.629256 datasieve-0.0.9/README.md
--rw-r--r--   0        0        0        0 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/__init__.py
--rw-r--r--   0        0        0     7210 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/pipeline.py
--rw-r--r--   0        0        0      575 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/__init__.py
--rw-r--r--   0        0        0     5739 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/dbscan.py
--rw-r--r--   0        0        0     3137 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/dissimilarity_index.py
--rw-r--r--   0        0        0     1158 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/minmax_scaler.py
--rw-r--r--   0        0        0     1567 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/pca.py
--rw-r--r--   0        0        0     1725 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/svm_outlier_extractor.py
--rw-r--r--   0        0        0     1432 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/transforms/variance_threshold.py
--rw-r--r--   0        0        0     3058 2023-05-29 14:46:28.629256 datasieve-0.0.9/datasieve/utils.py
--rw-r--r--   0        0        0      544 2023-05-29 14:46:28.629256 datasieve-0.0.9/pyproject.toml
--rw-r--r--   0        0        0    11783 1970-01-01 00:00:00.000000 datasieve-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1059 2023-05-29 21:37:04.979482 datasieve-0.1.0/LICENSE
+-rw-r--r--   0        0        0    11157 2023-05-29 21:37:04.979482 datasieve-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/__init__.py
+-rw-r--r--   0        0        0     7210 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/pipeline.py
+-rw-r--r--   0        0        0      575 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/__init__.py
+-rw-r--r--   0        0        0     5739 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/dbscan.py
+-rw-r--r--   0        0        0     3137 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/dissimilarity_index.py
+-rw-r--r--   0        0        0     1197 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/minmax_scaler.py
+-rw-r--r--   0        0        0     1606 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/pca.py
+-rw-r--r--   0        0        0     1725 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/svm_outlier_extractor.py
+-rw-r--r--   0        0        0     1453 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/transforms/variance_threshold.py
+-rw-r--r--   0        0        0     3058 2023-05-29 21:37:04.979482 datasieve-0.1.0/datasieve/utils.py
+-rw-r--r--   0        0        0      544 2023-05-29 21:37:04.979482 datasieve-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    11783 1970-01-01 00:00:00.000000 datasieve-0.1.0/PKG-INFO
```

### Comparing `datasieve-0.0.9/LICENSE` & `datasieve-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.9/README.md` & `datasieve-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.9/datasieve/pipeline.py` & `datasieve-0.1.0/datasieve/pipeline.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.9/datasieve/transforms/__init__.py` & `datasieve-0.1.0/datasieve/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.9/datasieve/transforms/dbscan.py` & `datasieve-0.1.0/datasieve/transforms/dbscan.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.9/datasieve/transforms/dissimilarity_index.py` & `datasieve-0.1.0/datasieve/transforms/dissimilarity_index.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.9/datasieve/transforms/minmax_scaler.py` & `datasieve-0.1.0/datasieve/transforms/minmax_scaler.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,13 +19,14 @@
         X = super().transform(X)
         return X, y, sample_weight, feature_list
 
     def fit(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         super().fit(X)
         return X, y, sample_weight, feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+    def transform(self, X, y=None, sample_weight=None,
+                  feature_list=None, outlier_check=False, **kwargs):
         X = super().transform(X)
         return X, y, sample_weight, feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         return super().inverse_transform(X), y, sample_weight, feature_list
```

### Comparing `datasieve-0.0.9/datasieve/transforms/pca.py` & `datasieve-0.1.0/datasieve/transforms/pca.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,13 +25,14 @@
 
         n_keep_components = self.n_components_
         self.feature_list = [f"PC{i}" for i in range(0, n_keep_components)]
         logger.info(f"reduced feature dimension by {n_components - n_keep_components}")
         logger.info(f"explained variance {np.sum(self.explained_variance_ratio_)}")
         return X, y, sample_weight, self.feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
+    def transform(self, X, y=None, sample_weight=None,
+                  outlier_check=False, feature_list=None, **kwargs):
         X = super().transform(X)
         return X, y, sample_weight, self.feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None, **kwargs):
         return super().inverse_transform(X), y, sample_weight, feature_list
```

### Comparing `datasieve-0.0.9/datasieve/transforms/svm_outlier_extractor.py` & `datasieve-0.1.0/datasieve/transforms/svm_outlier_extractor.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.9/datasieve/transforms/variance_threshold.py` & `datasieve-0.1.0/datasieve/transforms/variance_threshold.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
                         f"{len(feature_list) - len(self.feature_list)} "
                         f"on transform. {np.array(feature_list)[~self.mask]}")
         else:
             self.feature_list = None
 
         return X, y, sample_weight, self.feature_list
 
-    def transform(self, X, y=None, sample_weight=None, feature_list=None):
+    def transform(self, X, y=None, sample_weight=None, outlier_check=False, feature_list=None):
 
         # use mask to filter X array
         X = X[:, self.mask]
 
         return X, y, sample_weight, self.feature_list
 
     def inverse_transform(self, X, y=None, sample_weight=None, feature_list=None):
```

### Comparing `datasieve-0.0.9/datasieve/utils.py` & `datasieve-0.1.0/datasieve/utils.py`

 * *Files identical despite different names*

### Comparing `datasieve-0.0.9/pyproject.toml` & `datasieve-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datasieve"
-version = "0.0.9"
+version = "0.1.0"
 description = "This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)"
 authors = ['Robert Caulk']
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
```

### Comparing `datasieve-0.0.9/PKG-INFO` & `datasieve-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasieve
-Version: 0.0.9
+Version: 0.1.0
 Summary: This package implements a flexible data pipeline to help organize row removal (e.g. outlier removal) and feature modification (e.g. PCA)
 License: MIT
 Author: Robert Caulk
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```


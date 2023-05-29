# Comparing `tmp/treeordination-1.3.1.tar.gz` & `tmp/treeordination-1.3.2.tar.gz`

## Comparing `treeordination-1.3.1.tar` & `treeordination-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 treeordination-1.3.1/environment.yml
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 treeordination-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 treeordination-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 treeordination-1.3.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 treeordination-1.3.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 treeordination-1.3.1/TreeOrdination/TreeOrdination.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 treeordination-1.3.1/TreeOrdination/__init__.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 treeordination-1.3.1/TreeOrdination/feature_importance_treeord.py
--rw-r--r--   0        0        0     4911 2020-02-02 00:00:00.000000 treeordination-1.3.1/TreeOrdination/transformers_treeord.py
--rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 treeordination-1.3.1/docs/API.md
--rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 treeordination-1.3.1/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.1/notebooks/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 treeordination-1.3.1/tests/test_treeord.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 treeordination-1.3.1/.gitignore
--rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 treeordination-1.3.1/LICENSE
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 treeordination-1.3.1/README.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 treeordination-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 treeordination-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 treeordination-1.3.2/environment.yml
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 treeordination-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 treeordination-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 treeordination-1.3.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 treeordination-1.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     8766 2020-02-02 00:00:00.000000 treeordination-1.3.2/TreeOrdination/TreeOrdination.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 treeordination-1.3.2/TreeOrdination/__init__.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 treeordination-1.3.2/TreeOrdination/feature_importance_treeord.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 treeordination-1.3.2/TreeOrdination/transformers_treeord.py
+-rw-r--r--   0        0        0     9119 2020-02-02 00:00:00.000000 treeordination-1.3.2/docs/API.md
+-rw-r--r--   0        0        0     4439 2020-02-02 00:00:00.000000 treeordination-1.3.2/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.2/notebooks/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 treeordination-1.3.2/tests/__init__.py
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 treeordination-1.3.2/tests/test_treeord.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 treeordination-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 treeordination-1.3.2/LICENSE
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 treeordination-1.3.2/README.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 treeordination-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     5821 2020-02-02 00:00:00.000000 treeordination-1.3.2/PKG-INFO
```

### Comparing `treeordination-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `treeordination-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `treeordination-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/.github/workflows/ci.yml` & `treeordination-1.3.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/.github/workflows/python-publish.yml` & `treeordination-1.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/TreeOrdination/TreeOrdination.py` & `treeordination-1.3.2/TreeOrdination/TreeOrdination.py`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/TreeOrdination/feature_importance_treeord.py` & `treeordination-1.3.2/TreeOrdination/feature_importance_treeord.py`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/TreeOrdination/transformers_treeord.py` & `treeordination-1.3.2/TreeOrdination/transformers_treeord.py`

 * *Files 1% similar despite different names*

```diff
@@ -133,10 +133,13 @@
             # Remove zero-variance features
             X_transform = self.zero_var_transformer.transform(X)
 
             # Transform data if a transformer is supplied
             if isinstance(self.transformer, type(None)) == False:
                 X_transform = self.transformer.transform(X_transform)
 
+            if X_transform.ndim == 1:
+                X_transform = np.asarray([X_transform])
+
             return X_transform
```

### Comparing `treeordination-1.3.1/docs/API.md` & `treeordination-1.3.2/docs/API.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/docs/CONTRIBUTING.md` & `treeordination-1.3.2/docs/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/tests/test_treeord.py` & `treeordination-1.3.2/tests/test_treeord.py`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/.gitignore` & `treeordination-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/LICENSE` & `treeordination-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/README.md` & `treeordination-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `treeordination-1.3.1/pyproject.toml` & `treeordination-1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "hatchling.build"
 requires = ["hatchling"]
 
 [project]
 name = "TreeOrdination"
-version = "1.3.1"
+version = "1.3.2"
 authors = [
     {name = "Josip Rudar", email = "rudarj@uoguelph.ca"},
     {name = "G. Brian Golding"},
     {name = "Stefan C. Kremer"},
     {name = "Mehrdad Hajibabaei", email = "mhajibab@uoguelph.ca"}
 ]
 description = "Projection of High-Dimensional Data Using Multivariate Decision Trees and UMAP"
```

### Comparing `treeordination-1.3.1/PKG-INFO` & `treeordination-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TreeOrdination
-Version: 1.3.1
+Version: 1.3.2
 Summary: Projection of High-Dimensional Data Using Multivariate Decision Trees and UMAP
 Project-URL: Homepage, https://github.com/jrudar/TreeOrdination
 Project-URL: Repository, https://github.com/jrudar/TreeOrdination.git
 Project-URL: Bug Tracker, https://github.com/jrudar/TreeOrdination/issues
 Author: G. Brian Golding, Stefan C. Kremer
 Author-email: Josip Rudar <rudarj@uoguelph.ca>, Mehrdad Hajibabaei <mhajibab@uoguelph.ca>
 License: MIT License
```


# Comparing `tmp/feature_store_utils-0.0.2.tar.gz` & `tmp/feature_store_utils-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feature_store_utils-0.0.2.tar", last modified: Mon May 29 12:55:27 2023, max compression
+gzip compressed data, was "feature_store_utils-0.0.3.tar", last modified: Mon May 29 18:31:44 2023, max compression
```

## Comparing `feature_store_utils-0.0.2.tar` & `feature_store_utils-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 12:55:27.835121 feature_store_utils-0.0.2/
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)    11357 2023-02-13 15:10:53.000000 feature_store_utils-0.0.2/LICENSE
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3561 2023-05-29 12:55:27.834927 feature_store_utils-0.0.2/PKG-INFO
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3163 2023-05-29 12:38:06.000000 feature_store_utils-0.0.2/README.md
-drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 12:55:27.832787 feature_store_utils-0.0.2/feature_store_utils.egg-info/
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3561 2023-05-29 12:55:27.000000 feature_store_utils-0.0.2/feature_store_utils.egg-info/PKG-INFO
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)      369 2023-05-29 12:55:27.000000 feature_store_utils-0.0.2/feature_store_utils.egg-info/SOURCES.txt
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)        1 2023-05-29 12:55:27.000000 feature_store_utils-0.0.2/feature_store_utils.egg-info/dependency_links.txt
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)       59 2023-05-29 12:55:27.000000 feature_store_utils-0.0.2/feature_store_utils.egg-info/requires.txt
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)        9 2023-05-29 12:55:27.000000 feature_store_utils-0.0.2/feature_store_utils.egg-info/top_level.txt
-drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 12:55:27.834562 feature_store_utils-0.0.2/features/
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)        0 2023-02-13 15:10:53.000000 feature_store_utils-0.0.2/features/__init__.py
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     5807 2023-05-22 13:30:53.000000 feature_store_utils-0.0.2/features/feature_generation.py
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1730 2023-05-22 13:30:53.000000 feature_store_utils-0.0.2/features/feature_spec.py
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1341 2023-02-13 15:10:53.000000 feature_store_utils-0.0.2/features/hyper_feature.py
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1779 2023-02-13 15:10:53.000000 feature_store_utils-0.0.2/features/sql_gen.py
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)      694 2023-05-29 12:55:23.000000 feature_store_utils-0.0.2/pyproject.toml
--rw-r--r--   0 ben.mackenzie   (502) staff       (20)       38 2023-05-29 12:55:27.835181 feature_store_utils-0.0.2/setup.cfg
+drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 18:31:44.267015 feature_store_utils-0.0.3/
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)    11357 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/LICENSE
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3593 2023-05-29 18:31:44.266809 feature_store_utils-0.0.3/PKG-INFO
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3195 2023-05-29 18:30:36.000000 feature_store_utils-0.0.3/README.md
+drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 18:31:44.262908 feature_store_utils-0.0.3/feature_store_utils.egg-info/
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     3593 2023-05-29 18:31:44.000000 feature_store_utils-0.0.3/feature_store_utils.egg-info/PKG-INFO
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)      561 2023-05-29 18:31:44.000000 feature_store_utils-0.0.3/feature_store_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)        1 2023-05-29 18:31:44.000000 feature_store_utils-0.0.3/feature_store_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)       59 2023-05-29 18:31:44.000000 feature_store_utils-0.0.3/feature_store_utils.egg-info/requires.txt
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)        9 2023-05-29 18:31:44.000000 feature_store_utils-0.0.3/feature_store_utils.egg-info/top_level.txt
+drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 18:31:44.264886 feature_store_utils-0.0.3/features/
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)        0 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/__init__.py
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     5807 2023-05-22 13:30:53.000000 feature_store_utils-0.0.3/features/feature_generation.py
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1730 2023-05-22 13:30:53.000000 feature_store_utils-0.0.3/features/feature_spec.py
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1341 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/hyper_feature.py
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1779 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/sql_gen.py
+drwxr-xr-x   0 ben.mackenzie   (502) staff       (20)        0 2023-05-29 18:31:44.266486 feature_store_utils-0.0.3/features/templates/
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1339 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/templates/fact_aggregations.j2
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     2656 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/templates/timeseries_growth.j2
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)     1721 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/templates/timeseries_growth_m.j2
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)      526 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/templates/type1_lookup.j2
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)      708 2023-02-13 15:10:53.000000 feature_store_utils-0.0.3/features/templates/type2_lookup.j2
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)      653 2023-05-29 18:31:38.000000 feature_store_utils-0.0.3/pyproject.toml
+-rw-r--r--   0 ben.mackenzie   (502) staff       (20)       38 2023-05-29 18:31:44.267068 feature_store_utils-0.0.3/setup.cfg
```

### Comparing `feature_store_utils-0.0.2/LICENSE` & `feature_store_utils-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.2/PKG-INFO` & `feature_store_utils-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature_store_utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: A utility to generate ML features from yaml
 Author-email: Example Author <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -50,14 +50,16 @@
 
 
 
 ```
 python3 -m build  
 python3 -m twine upload --repository testpypi dist/*
 
+python3 -m twine upload dist/*
+
 ```
 
 
 ### Running unit tests on databricks
 
 1. install the databricks extension for vscode
 2. use this repo as a template.  Note the following:
```

### Comparing `feature_store_utils-0.0.2/README.md` & `feature_store_utils-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,16 @@
 
 
 
 ```
 python3 -m build  
 python3 -m twine upload --repository testpypi dist/*
 
+python3 -m twine upload dist/*
+
 ```
 
 
 ### Running unit tests on databricks
 
 1. install the databricks extension for vscode
 2. use this repo as a template.  Note the following:
```

### Comparing `feature_store_utils-0.0.2/feature_store_utils.egg-info/PKG-INFO` & `feature_store_utils-0.0.3/feature_store_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: feature-store-utils
-Version: 0.0.2
+Version: 0.0.3
 Summary: A utility to generate ML features from yaml
 Author-email: Example Author <author@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -50,14 +50,16 @@
 
 
 
 ```
 python3 -m build  
 python3 -m twine upload --repository testpypi dist/*
 
+python3 -m twine upload dist/*
+
 ```
 
 
 ### Running unit tests on databricks
 
 1. install the databricks extension for vscode
 2. use this repo as a template.  Note the following:
```

### Comparing `feature_store_utils-0.0.2/features/feature_generation.py` & `feature_store_utils-0.0.3/features/feature_generation.py`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.2/features/feature_spec.py` & `feature_store_utils-0.0.3/features/feature_spec.py`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.2/features/hyper_feature.py` & `feature_store_utils-0.0.3/features/hyper_feature.py`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.2/features/sql_gen.py` & `feature_store_utils-0.0.3/features/sql_gen.py`

 * *Files identical despite different names*

### Comparing `feature_store_utils-0.0.2/pyproject.toml` & `feature_store_utils-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "feature_store_utils"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A utility to generate ML features from yaml"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -23,9 +23,7 @@
     'pandas',
     'pyaml'
     ]
 
 [tool.setuptools.package-data]
 "features.templates" = ["*.j2"]
 
-[tool.setuptools]
-packages = ["features"]
```


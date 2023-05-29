# Comparing `tmp/aib_logging-1.0.7.tar.gz` & `tmp/aib_logging-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aib_logging-1.0.7.tar", last modified: Thu May 25 13:05:44 2023, max compression
+gzip compressed data, was "aib_logging-1.0.8.tar", last modified: Mon May 29 10:21:20 2023, max compression
```

## Comparing `aib_logging-1.0.7.tar` & `aib_logging-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-25 13:05:44.164351 aib_logging-1.0.7/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.7/LICENSE.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-25 13:05:44.163351 aib_logging-1.0.7/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.7/README.md
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      623 2023-05-25 13:01:35.000000 aib_logging-1.0.7/pyproject.toml
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-05-25 13:05:44.164351 aib_logging-1.0.7/setup.cfg
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-25 13:05:44.146349 aib_logging-1.0.7/src/
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-25 13:05:44.162351 aib_logging-1.0.7/src/aib_logging/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.7/src/aib_logging/__init__.py
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    14570 2023-05-25 13:00:08.000000 aib_logging-1.0.7/src/aib_logging/logger.py
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-25 13:05:44.163351 aib_logging-1.0.7/src/aib_logging.egg-info/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-25 13:05:44.000000 aib_logging-1.0.7/src/aib_logging.egg-info/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-05-25 13:05:44.000000 aib_logging-1.0.7/src/aib_logging.egg-info/SOURCES.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-05-25 13:05:44.000000 aib_logging-1.0.7/src/aib_logging.egg-info/dependency_links.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       28 2023-05-25 13:05:44.000000 aib_logging-1.0.7/src/aib_logging.egg-info/requires.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-05-25 13:05:44.000000 aib_logging-1.0.7/src/aib_logging.egg-info/top_level.txt
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-29 10:21:20.731631 aib_logging-1.0.8/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.8/LICENSE.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-29 10:21:20.731631 aib_logging-1.0.8/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.8/README.md
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      623 2023-05-29 10:20:59.000000 aib_logging-1.0.8/pyproject.toml
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-05-29 10:21:20.731631 aib_logging-1.0.8/setup.cfg
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-29 10:21:20.724630 aib_logging-1.0.8/src/
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-29 10:21:20.728630 aib_logging-1.0.8/src/aib_logging/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.8/src/aib_logging/__init__.py
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    14590 2023-05-29 10:20:53.000000 aib_logging-1.0.8/src/aib_logging/logger.py
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-29 10:21:20.730631 aib_logging-1.0.8/src/aib_logging.egg-info/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-29 10:21:20.000000 aib_logging-1.0.8/src/aib_logging.egg-info/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-05-29 10:21:20.000000 aib_logging-1.0.8/src/aib_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-05-29 10:21:20.000000 aib_logging-1.0.8/src/aib_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       28 2023-05-29 10:21:20.000000 aib_logging-1.0.8/src/aib_logging.egg-info/requires.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-05-29 10:21:20.000000 aib_logging-1.0.8/src/aib_logging.egg-info/top_level.txt
```

### Comparing `aib_logging-1.0.7/LICENSE.txt` & `aib_logging-1.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aib_logging-1.0.7/PKG-INFO` & `aib_logging-1.0.8/src/aib_logging.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aib_logging
-Version: 1.0.7
+Name: aib-logging
+Version: 1.0.8
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aib_logging-1.0.7/pyproject.toml` & `aib_logging-1.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aib_logging"
-version = "1.0.7"
+version = "1.0.8"
 authors = [
   { name="akib Shaikh", email="shaikhakib.k@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `aib_logging-1.0.7/src/aib_logging/logger.py` & `aib_logging-1.0.8/src/aib_logging/logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
         OTHER="Other"
 
     class Actions(Enum):
         CREATE="Create"
         UPDATE="Update"
         DELETE="Delete"
         UPLOAD="Upload"
+        READ="Read"
         MODEL_SCORE="Model_Score"
         DATA_STAT="Data_statistics"
         OTHER="Other"
     
     class Severities(Enum):
         INFO="INFO"
         WARNING="WARNING"
```

### Comparing `aib_logging-1.0.7/src/aib_logging.egg-info/PKG-INFO` & `aib_logging-1.0.8/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: aib-logging
-Version: 1.0.7
+Name: aib_logging
+Version: 1.0.8
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


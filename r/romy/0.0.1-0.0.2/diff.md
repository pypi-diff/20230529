# Comparing `tmp/romy-0.0.1.tar.gz` & `tmp/romy-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romy-0.0.1.tar", last modified: Mon May 22 20:38:33 2023, max compression
+gzip compressed data, was "romy-0.0.2.tar", last modified: Mon May 29 16:44:47 2023, max compression
```

## Comparing `romy-0.0.1.tar` & `romy-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 nios      (1000) users      (985)        0 2023-05-22 20:38:33.292479 romy-0.0.1/
--rw-r--r--   0 nios      (1000) users      (985)    34523 2023-05-22 20:30:58.000000 romy-0.0.1/LICENSE
--rw-r--r--   0 nios      (1000) users      (985)     1506 2023-05-22 20:38:33.292479 romy-0.0.1/PKG-INFO
--rw-r--r--   0 nios      (1000) users      (985)      713 2023-05-22 20:30:58.000000 romy-0.0.1/README.md
--rw-r--r--   0 nios      (1000) users      (985)      926 2023-05-22 20:31:27.000000 romy-0.0.1/pyproject.toml
--rw-r--r--   0 nios      (1000) users      (985)       38 2023-05-22 20:38:33.292479 romy-0.0.1/setup.cfg
-drwxr-xr-x   0 nios      (1000) users      (985)        0 2023-05-22 20:38:33.292479 romy-0.0.1/src/
-drwxr-xr-x   0 nios      (1000) users      (985)        0 2023-05-22 20:38:33.292479 romy-0.0.1/src/romy/
--rw-r--r--   0 nios      (1000) users      (985)      143 2023-05-22 20:33:59.000000 romy-0.0.1/src/romy/__init__.py
--rw-r--r--   0 nios      (1000) users      (985)     7845 2023-05-22 20:33:09.000000 romy-0.0.1/src/romy/romy.py
--rw-r--r--   0 nios      (1000) users      (985)     1987 2023-05-22 20:33:09.000000 romy-0.0.1/src/romy/utils.py
-drwxr-xr-x   0 nios      (1000) users      (985)        0 2023-05-22 20:38:33.292479 romy-0.0.1/src/romy.egg-info/
--rw-r--r--   0 nios      (1000) users      (985)     1506 2023-05-22 20:38:33.000000 romy-0.0.1/src/romy.egg-info/PKG-INFO
--rw-r--r--   0 nios      (1000) users      (985)      237 2023-05-22 20:38:33.000000 romy-0.0.1/src/romy.egg-info/SOURCES.txt
--rw-r--r--   0 nios      (1000) users      (985)        1 2023-05-22 20:38:33.000000 romy-0.0.1/src/romy.egg-info/dependency_links.txt
--rw-r--r--   0 nios      (1000) users      (985)       19 2023-05-22 20:38:33.000000 romy-0.0.1/src/romy.egg-info/top_level.txt
--rw-r--r--   0 nios      (1000) users      (985)     1123 2023-05-22 20:36:29.000000 romy-0.0.1/src/usage_example.py
+drwxr-xr-x   0 nios      (1000) users      (985)        0 2023-05-29 16:44:47.182791 romy-0.0.2/
+-rw-r--r--   0 nios      (1000) users      (985)    34523 2023-05-22 20:30:58.000000 romy-0.0.2/LICENSE
+-rw-r--r--   0 nios      (1000) users      (985)     1506 2023-05-29 16:44:47.182791 romy-0.0.2/PKG-INFO
+-rw-r--r--   0 nios      (1000) users      (985)      713 2023-05-22 20:30:58.000000 romy-0.0.2/README.md
+-rw-r--r--   0 nios      (1000) users      (985)      926 2023-05-29 16:43:02.000000 romy-0.0.2/pyproject.toml
+-rw-r--r--   0 nios      (1000) users      (985)       38 2023-05-29 16:44:47.182791 romy-0.0.2/setup.cfg
+drwxr-xr-x   0 nios      (1000) users      (985)        0 2023-05-29 16:44:47.182791 romy-0.0.2/src/
+drwxr-xr-x   0 nios      (1000) users      (985)        0 2023-05-29 16:44:47.182791 romy-0.0.2/src/romy/
+-rw-r--r--   0 nios      (1000) users      (985)      143 2023-05-29 16:42:58.000000 romy-0.0.2/src/romy/__init__.py
+-rw-r--r--   0 nios      (1000) users      (985)        0 2023-05-29 16:41:33.000000 romy-0.0.2/src/romy/py.typed
+-rw-r--r--   0 nios      (1000) users      (985)    11419 2023-05-29 16:41:27.000000 romy-0.0.2/src/romy/romy.py
+-rw-r--r--   0 nios      (1000) users      (985)     1987 2023-05-22 20:33:09.000000 romy-0.0.2/src/romy/utils.py
+drwxr-xr-x   0 nios      (1000) users      (985)        0 2023-05-29 16:44:47.182791 romy-0.0.2/src/romy.egg-info/
+-rw-r--r--   0 nios      (1000) users      (985)     1506 2023-05-29 16:44:47.000000 romy-0.0.2/src/romy.egg-info/PKG-INFO
+-rw-r--r--   0 nios      (1000) users      (985)      255 2023-05-29 16:44:47.000000 romy-0.0.2/src/romy.egg-info/SOURCES.txt
+-rw-r--r--   0 nios      (1000) users      (985)        1 2023-05-29 16:44:47.000000 romy-0.0.2/src/romy.egg-info/dependency_links.txt
+-rw-r--r--   0 nios      (1000) users      (985)       19 2023-05-29 16:44:47.000000 romy-0.0.2/src/romy.egg-info/top_level.txt
+-rw-r--r--   0 nios      (1000) users      (985)     1123 2023-05-29 16:41:35.000000 romy-0.0.2/src/usage_example.py
```

### Comparing `romy-0.0.1/LICENSE` & `romy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `romy-0.0.1/PKG-INFO` & `romy-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python program and library to control Wi-Fi enabled ROMY vacuum cleaners
 Author-email: Manuel Dipolt <manuel.dipolt@robart.cc>
 Project-URL: Homepage, https://github.com/xeniter/romy
 Project-URL: Bug Tracker, https://github.com/xeniter/romy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `romy-0.0.1/README.md` & `romy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `romy-0.0.1/pyproject.toml` & `romy-0.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "romy"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Manuel Dipolt", email="manuel.dipolt@robart.cc" },
 ]
 description = "Python program and library to control Wi-Fi enabled ROMY vacuum cleaners"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.md"}
```

### Comparing `romy-0.0.1/src/romy/utils.py` & `romy-0.0.2/src/romy/utils.py`

 * *Files identical despite different names*

### Comparing `romy-0.0.1/src/romy.egg-info/PKG-INFO` & `romy-0.0.2/src/romy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romy
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python program and library to control Wi-Fi enabled ROMY vacuum cleaners
 Author-email: Manuel Dipolt <manuel.dipolt@robart.cc>
 Project-URL: Homepage, https://github.com/xeniter/romy
 Project-URL: Bug Tracker, https://github.com/xeniter/romy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `romy-0.0.1/src/usage_example.py` & `romy-0.0.2/src/usage_example.py`

 * *Files identical despite different names*


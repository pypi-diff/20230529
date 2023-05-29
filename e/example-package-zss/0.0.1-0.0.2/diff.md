# Comparing `tmp/example_package_zss-0.0.1.tar.gz` & `tmp/example_package_zss-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_package_zss-0.0.1.tar", last modified: Mon May 29 07:53:33 2023, max compression
+gzip compressed data, was "example_package_zss-0.0.2.tar", last modified: Mon May 29 14:03:36 2023, max compression
```

## Comparing `example_package_zss-0.0.1.tar` & `example_package_zss-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 07:53:33.446124 example_package_zss-0.0.1/
--rw-rw-r--   0 zss       (1000) zss       (1000)     1068 2023-05-29 07:50:18.000000 example_package_zss-0.0.1/LICENSE
--rw-rw-r--   0 zss       (1000) zss       (1000)      681 2023-05-29 07:53:33.446124 example_package_zss-0.0.1/PKG-INFO
--rw-rw-r--   0 zss       (1000) zss       (1000)      170 2023-05-29 07:49:05.000000 example_package_zss-0.0.1/README.md
--rw-rw-r--   0 zss       (1000) zss       (1000)      583 2023-05-29 07:53:07.000000 example_package_zss-0.0.1/pyproject.toml
--rw-rw-r--   0 zss       (1000) zss       (1000)       38 2023-05-29 07:53:33.446124 example_package_zss-0.0.1/setup.cfg
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 07:53:33.446124 example_package_zss-0.0.1/src/
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 07:53:33.446124 example_package_zss-0.0.1/src/example_package_zss/
--rw-rw-r--   0 zss       (1000) zss       (1000)        0 2023-05-29 07:44:05.000000 example_package_zss-0.0.1/src/example_package_zss/__init__.py
--rw-rw-r--   0 zss       (1000) zss       (1000)       42 2023-05-29 07:44:24.000000 example_package_zss-0.0.1/src/example_package_zss/example.py
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 07:53:33.446124 example_package_zss-0.0.1/src/example_package_zss.egg-info/
--rw-rw-r--   0 zss       (1000) zss       (1000)      681 2023-05-29 07:53:33.000000 example_package_zss-0.0.1/src/example_package_zss.egg-info/PKG-INFO
--rw-rw-r--   0 zss       (1000) zss       (1000)      291 2023-05-29 07:53:33.000000 example_package_zss-0.0.1/src/example_package_zss.egg-info/SOURCES.txt
--rw-rw-r--   0 zss       (1000) zss       (1000)        1 2023-05-29 07:53:33.000000 example_package_zss-0.0.1/src/example_package_zss.egg-info/dependency_links.txt
--rw-rw-r--   0 zss       (1000) zss       (1000)       20 2023-05-29 07:53:33.000000 example_package_zss-0.0.1/src/example_package_zss.egg-info/top_level.txt
+drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 14:03:36.782229 example_package_zss-0.0.2/
+-rw-rw-r--   0 zss       (1000) zss       (1000)     1068 2023-05-29 07:50:18.000000 example_package_zss-0.0.2/LICENSE
+-rw-rw-r--   0 zss       (1000) zss       (1000)      681 2023-05-29 14:03:36.782229 example_package_zss-0.0.2/PKG-INFO
+-rw-rw-r--   0 zss       (1000) zss       (1000)      170 2023-05-29 07:49:05.000000 example_package_zss-0.0.2/README.md
+-rw-rw-r--   0 zss       (1000) zss       (1000)      583 2023-05-29 14:03:05.000000 example_package_zss-0.0.2/pyproject.toml
+-rw-rw-r--   0 zss       (1000) zss       (1000)       38 2023-05-29 14:03:36.782229 example_package_zss-0.0.2/setup.cfg
+drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 14:03:36.782229 example_package_zss-0.0.2/src/
+drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 14:03:36.782229 example_package_zss-0.0.2/src/example_package_zss/
+-rw-rw-r--   0 zss       (1000) zss       (1000)        0 2023-05-29 07:44:05.000000 example_package_zss-0.0.2/src/example_package_zss/__init__.py
+-rw-rw-r--   0 zss       (1000) zss       (1000)       42 2023-05-29 07:44:24.000000 example_package_zss-0.0.2/src/example_package_zss/example.py
+drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 14:03:36.782229 example_package_zss-0.0.2/src/example_package_zss.egg-info/
+-rw-rw-r--   0 zss       (1000) zss       (1000)      681 2023-05-29 14:03:36.000000 example_package_zss-0.0.2/src/example_package_zss.egg-info/PKG-INFO
+-rw-rw-r--   0 zss       (1000) zss       (1000)      291 2023-05-29 14:03:36.000000 example_package_zss-0.0.2/src/example_package_zss.egg-info/SOURCES.txt
+-rw-rw-r--   0 zss       (1000) zss       (1000)        1 2023-05-29 14:03:36.000000 example_package_zss-0.0.2/src/example_package_zss.egg-info/dependency_links.txt
+-rw-rw-r--   0 zss       (1000) zss       (1000)       20 2023-05-29 14:03:36.000000 example_package_zss-0.0.2/src/example_package_zss.egg-info/top_level.txt
```

### Comparing `example_package_zss-0.0.1/LICENSE` & `example_package_zss-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `example_package_zss-0.0.1/PKG-INFO` & `example_package_zss-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_zss
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `example_package_zss-0.0.1/pyproject.toml` & `example_package_zss-0.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "example_package_zss"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Example Author", email="author@example.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `example_package_zss-0.0.1/src/example_package_zss.egg-info/PKG-INFO` & `example_package_zss-0.0.2/src/example_package_zss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example-package-zss
-Version: 0.0.1
+Version: 0.0.2
 Summary: A small example package
 Author-email: Example Author <author@example.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


# Comparing `tmp/random_math_rmaiaaaa-0.0.10.tar.gz` & `tmp/random_math_rmaiaaaa-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "random_math_rmaiaaaa-0.0.10.tar", last modified: Mon May 29 00:59:17 2023, max compression
+gzip compressed data, was "/home/runner/work/random-math/random-math/dist/.tmp-zixg_2eb/random_math_rmaiaaaa-0.0.13.tar", last modified: Mon May 29 20:47:49 2023, max compression
```

## Comparing `random_math_rmaiaaaa-0.0.10.tar` & `random_math_rmaiaaaa-0.0.13.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:59:17.264570 random_math_rmaiaaaa-0.0.10/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-29 00:59:02.000000 random_math_rmaiaaaa-0.0.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 00:59:17.264570 random_math_rmaiaaaa-0.0.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 00:59:02.000000 random_math_rmaiaaaa-0.0.10/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 00:59:02.000000 random_math_rmaiaaaa-0.0.10/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 00:59:17.264570 random_math_rmaiaaaa-0.0.10/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:59:17.260570 random_math_rmaiaaaa-0.0.10/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:59:17.264570 random_math_rmaiaaaa-0.0.10/src/RandomMath/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-29 00:59:02.000000 random_math_rmaiaaaa-0.0.10/src/RandomMath/RandomMathOperations.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 00:59:02.000000 random_math_rmaiaaaa-0.0.10/src/RandomMath/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:59:17.264570 random_math_rmaiaaaa-0.0.10/src/random_math_rmaiaaaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 00:59:17.000000 random_math_rmaiaaaa-0.0.10/src/random_math_rmaiaaaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-29 00:59:17.000000 random_math_rmaiaaaa-0.0.10/src/random_math_rmaiaaaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:59:17.000000 random_math_rmaiaaaa-0.0.10/src/random_math_rmaiaaaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 00:59:17.000000 random_math_rmaiaaaa-0.0.10/src/random_math_rmaiaaaa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:59:17.264570 random_math_rmaiaaaa-0.0.10/src/test/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-29 00:59:02.000000 random_math_rmaiaaaa-0.0.10/src/test/test_RandomMathOperations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/RandomMath/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/src/RandomMath/RandomMathOperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/src/RandomMath/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/apiRandomMath/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/src/apiRandomMath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-29 20:47:37.000000 random_math_rmaiaaaa-0.0.13/src/apiRandomMath/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 20:47:49.000000 random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `random_math_rmaiaaaa-0.0.10/LICENSE` & `random_math_rmaiaaaa-0.0.13/LICENSE`

 * *Files identical despite different names*

### Comparing `random_math_rmaiaaaa-0.0.10/PKG-INFO` & `random_math_rmaiaaaa-0.0.13/src/random_math_rmaiaaaa.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: random_math_rmaiaaaa
-Version: 0.0.10
+Name: random-math-rmaiaaaa
+Version: 0.0.13
 Summary: Random Math Package
 Author-email: Rafael Maia de Souza <rmaiadesouza@gmail.com>
 Project-URL: Homepage, https://github.com/rmaiaaaa/random-math
 Project-URL: Bug Tracker, https://github.com/rmaiaaaa/random-math/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # random_math
 Repositório para demonstração de um pipeline de Devops
```

### Comparing `random_math_rmaiaaaa-0.0.10/pyproject.toml` & `random_math_rmaiaaaa-0.0.13/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "random_math_rmaiaaaa"
-version = "v0.0.10"
+version = "v0.0.13"
 authors = [
   { name="Rafael Maia de Souza", email="rmaiadesouza@gmail.com" },
 ]
 description = "Random Math Package"
 readme = "README.md"
-requires-python = ">=3.8"
+requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [project.urls]
 "Homepage" = "https://github.com/rmaiaaaa/random-math"
```

### Comparing `random_math_rmaiaaaa-0.0.10/src/random_math_rmaiaaaa.egg-info/PKG-INFO` & `random_math_rmaiaaaa-0.0.13/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
-Name: random-math-rmaiaaaa
-Version: 0.0.10
+Name: random_math_rmaiaaaa
+Version: 0.0.13
 Summary: Random Math Package
 Author-email: Rafael Maia de Souza <rmaiadesouza@gmail.com>
 Project-URL: Homepage, https://github.com/rmaiaaaa/random-math
 Project-URL: Bug Tracker, https://github.com/rmaiaaaa/random-math/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # random_math
 Repositório para demonstração de um pipeline de Devops
```


# Comparing `tmp/matlab-tictoc-1.0.2.tar.gz` & `tmp/matlab-tictoc-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matlab-tictoc-1.0.2.tar", last modified: Wed May 24 16:39:49 2023, max compression
+gzip compressed data, was "matlab-tictoc-1.0.3.tar", last modified: Mon May 29 15:14:12 2023, max compression
```

## Comparing `matlab-tictoc-1.0.2.tar` & `matlab-tictoc-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:49.022887 matlab-tictoc-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 16:39:39.000000 matlab-tictoc-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-24 16:39:49.022887 matlab-tictoc-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-24 16:39:39.000000 matlab-tictoc-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-24 16:39:39.000000 matlab-tictoc-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 16:39:49.022887 matlab-tictoc-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:49.022887 matlab-tictoc-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:49.022887 matlab-tictoc-1.0.2/src/matlab_tictoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-24 16:39:49.000000 matlab-tictoc-1.0.2/src/matlab_tictoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-24 16:39:49.000000 matlab-tictoc-1.0.2/src/matlab_tictoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 16:39:49.000000 matlab-tictoc-1.0.2/src/matlab_tictoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-24 16:39:49.000000 matlab-tictoc-1.0.2/src/matlab_tictoc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 16:39:49.022887 matlab-tictoc-1.0.2/src/tictoc/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-24 16:39:39.000000 matlab-tictoc-1.0.2/src/tictoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2347 2023-05-24 16:39:39.000000 matlab-tictoc-1.0.2/src/tictoc/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:14:12.169743 matlab-tictoc-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 15:14:00.000000 matlab-tictoc-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-29 15:14:12.169743 matlab-tictoc-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-29 15:14:00.000000 matlab-tictoc-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-29 15:14:00.000000 matlab-tictoc-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:14:12.169743 matlab-tictoc-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:14:12.165743 matlab-tictoc-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:14:12.169743 matlab-tictoc-1.0.3/src/matlab_tictoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-29 15:14:12.000000 matlab-tictoc-1.0.3/src/matlab_tictoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 15:14:12.000000 matlab-tictoc-1.0.3/src/matlab_tictoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:14:12.000000 matlab-tictoc-1.0.3/src/matlab_tictoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 15:14:12.000000 matlab-tictoc-1.0.3/src/matlab_tictoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:14:12.169743 matlab-tictoc-1.0.3/src/tictoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 15:14:00.000000 matlab-tictoc-1.0.3/src/tictoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-05-29 15:14:00.000000 matlab-tictoc-1.0.3/src/tictoc/tictoc.py
```

### Comparing `matlab-tictoc-1.0.2/LICENSE` & `matlab-tictoc-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matlab-tictoc-1.0.2/PKG-INFO` & `matlab-tictoc-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-tictoc
-Version: 1.0.2
+Version: 1.0.3
 Summary: A timing package that mimics MATLAB's tic and toc functionality
 Author: Matthew Altberg
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MATLAB Tic Toc
```

### Comparing `matlab-tictoc-1.0.2/README.md` & `matlab-tictoc-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `matlab-tictoc-1.0.2/src/matlab_tictoc.egg-info/PKG-INFO` & `matlab-tictoc-1.0.3/src/matlab_tictoc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-tictoc
-Version: 1.0.2
+Version: 1.0.3
 Summary: A timing package that mimics MATLAB's tic and toc functionality
 Author: Matthew Altberg
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MATLAB Tic Toc
```

### Comparing `matlab-tictoc-1.0.2/src/tictoc/tictoc.py` & `matlab-tictoc-1.0.3/src/tictoc/tictoc.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,12 +83,12 @@
     if is_assigned_to_var:
         return timer.elapsed_time
 
     print(f'Elapsed time is {timer.elapsed_time} seconds.')
     return
 
 def func_timer(func):
-    def timer_wrapper():
+    def timer_wrapper(func):
         _func_timer = tic()
         func()
         print(f'Elapsed time for function {func.__name__} is {toc(_func_timer)} seconds.')
     return timer_wrapper
```


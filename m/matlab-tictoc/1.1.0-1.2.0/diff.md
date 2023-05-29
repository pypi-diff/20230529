# Comparing `tmp/matlab-tictoc-1.1.0.tar.gz` & `tmp/matlab-tictoc-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matlab-tictoc-1.1.0.tar", last modified: Mon May 29 15:23:10 2023, max compression
+gzip compressed data, was "matlab-tictoc-1.2.0.tar", last modified: Mon May 29 16:01:52 2023, max compression
```

## Comparing `matlab-tictoc-1.1.0.tar` & `matlab-tictoc-1.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:23:10.307181 matlab-tictoc-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 15:23:00.000000 matlab-tictoc-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-29 15:23:10.303181 matlab-tictoc-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-29 15:23:00.000000 matlab-tictoc-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-29 15:23:00.000000 matlab-tictoc-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:23:10.307181 matlab-tictoc-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:23:10.303181 matlab-tictoc-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:23:10.303181 matlab-tictoc-1.1.0/src/matlab_tictoc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-29 15:23:10.000000 matlab-tictoc-1.1.0/src/matlab_tictoc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 15:23:10.000000 matlab-tictoc-1.1.0/src/matlab_tictoc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:23:10.000000 matlab-tictoc-1.1.0/src/matlab_tictoc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 15:23:10.000000 matlab-tictoc-1.1.0/src/matlab_tictoc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:23:10.303181 matlab-tictoc-1.1.0/src/tictoc/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 15:23:00.000000 matlab-tictoc-1.1.0/src/tictoc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-29 15:23:00.000000 matlab-tictoc-1.1.0/src/tictoc/tictoc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:01:52.767171 matlab-tictoc-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 16:01:42.000000 matlab-tictoc-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-29 16:01:52.767171 matlab-tictoc-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-29 16:01:42.000000 matlab-tictoc-1.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-29 16:01:42.000000 matlab-tictoc-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:01:52.767171 matlab-tictoc-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:01:52.763171 matlab-tictoc-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:01:52.763171 matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-29 16:01:52.000000 matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 16:01:52.000000 matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:01:52.000000 matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 16:01:52.000000 matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:01:52.767171 matlab-tictoc-1.2.0/src/tictoc/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 16:01:42.000000 matlab-tictoc-1.2.0/src/tictoc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-29 16:01:42.000000 matlab-tictoc-1.2.0/src/tictoc/tictoc.py
```

### Comparing `matlab-tictoc-1.1.0/LICENSE` & `matlab-tictoc-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matlab-tictoc-1.1.0/PKG-INFO` & `matlab-tictoc-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-tictoc
-Version: 1.1.0
+Version: 1.2.0
 Summary: A timing package that mimics MATLAB's tic and toc functionality
 Author: Matthew Altberg
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MATLAB Tic Toc
```

### Comparing `matlab-tictoc-1.1.0/README.md` & `matlab-tictoc-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `matlab-tictoc-1.1.0/src/matlab_tictoc.egg-info/PKG-INFO` & `matlab-tictoc-1.2.0/src/matlab_tictoc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-tictoc
-Version: 1.1.0
+Version: 1.2.0
 Summary: A timing package that mimics MATLAB's tic and toc functionality
 Author: Matthew Altberg
 Requires-Python: <3.11,>=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # MATLAB Tic Toc
```

### Comparing `matlab-tictoc-1.1.0/src/tictoc/tictoc.py` & `matlab-tictoc-1.2.0/src/tictoc/tictoc.py`

 * *Files 5% similar despite different names*

```diff
@@ -85,10 +85,11 @@
 
     print(f'Elapsed time is {timer.elapsed_time} seconds.')
     return
 
 def func_timer(func):
     def timer_wrapper(*args, **kwargs):
         _func_timer = tic()
-        func(*args, **kwargs)
+        result = func(*args, **kwargs)
         print(f'Elapsed time for function {func.__name__} is {toc(_func_timer)} seconds.')
+        return result
     return timer_wrapper
```


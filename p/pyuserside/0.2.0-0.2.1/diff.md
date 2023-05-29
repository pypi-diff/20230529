# Comparing `tmp/pyuserside-0.2.0.tar.gz` & `tmp/pyuserside-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuserside-0.2.0.tar", last modified: Sat May 27 10:37:13 2023, max compression
+gzip compressed data, was "pyuserside-0.2.1.tar", last modified: Mon May 29 18:44:15 2023, max compression
```

## Comparing `pyuserside-0.2.0.tar` & `pyuserside-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:37:13.145438 pyuserside-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-27 10:36:59.000000 pyuserside-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-27 10:37:13.145438 pyuserside-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-27 10:36:59.000000 pyuserside-0.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-27 10:36:59.000000 pyuserside-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 10:37:13.145438 pyuserside-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:37:13.145438 pyuserside-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:37:13.145438 pyuserside-0.2.0/src/pyuserside/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-27 10:36:59.000000 pyuserside-0.2.0/src/pyuserside/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-27 10:36:59.000000 pyuserside-0.2.0/src/pyuserside/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:37:13.145438 pyuserside-0.2.0/src/pyuserside/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-27 10:36:59.000000 pyuserside-0.2.0/src/pyuserside/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-27 10:36:59.000000 pyuserside-0.2.0/src/pyuserside/asyncio/api.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-27 10:36:59.000000 pyuserside-0.2.0/src/pyuserside/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-27 10:36:59.000000 pyuserside-0.2.0/src/pyuserside/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 10:37:13.145438 pyuserside-0.2.0/src/pyuserside.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-27 10:37:13.000000 pyuserside-0.2.0/src/pyuserside.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-27 10:37:13.000000 pyuserside-0.2.0/src/pyuserside.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 10:37:13.000000 pyuserside-0.2.0/src/pyuserside.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-27 10:37:13.000000 pyuserside-0.2.0/src/pyuserside.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-27 10:37:13.000000 pyuserside-0.2.0/src/pyuserside.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:15.620773 pyuserside-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-29 18:44:03.000000 pyuserside-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-29 18:44:15.620773 pyuserside-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 18:44:03.000000 pyuserside-0.2.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-29 18:44:03.000000 pyuserside-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 18:44:15.624773 pyuserside-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:15.620773 pyuserside-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:15.620773 pyuserside-0.2.1/src/pyuserside/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 18:44:03.000000 pyuserside-0.2.1/src/pyuserside/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-29 18:44:03.000000 pyuserside-0.2.1/src/pyuserside/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:15.620773 pyuserside-0.2.1/src/pyuserside/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 18:44:03.000000 pyuserside-0.2.1/src/pyuserside/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-29 18:44:03.000000 pyuserside-0.2.1/src/pyuserside/asyncio/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-29 18:44:03.000000 pyuserside-0.2.1/src/pyuserside/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-29 18:44:03.000000 pyuserside-0.2.1/src/pyuserside/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:44:15.620773 pyuserside-0.2.1/src/pyuserside.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-05-29 18:44:15.000000 pyuserside-0.2.1/src/pyuserside.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-29 18:44:15.000000 pyuserside-0.2.1/src/pyuserside.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 18:44:15.000000 pyuserside-0.2.1/src/pyuserside.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 18:44:15.000000 pyuserside-0.2.1/src/pyuserside.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 18:44:15.000000 pyuserside-0.2.1/src/pyuserside.egg-info/top_level.txt
```

### Comparing `pyuserside-0.2.0/LICENSE` & `pyuserside-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuserside-0.2.0/PKG-INFO` & `pyuserside-0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuserside
-Version: 0.2.0
+Version: 0.2.1
 Summary: Userside API client implementation
 Author-email: Ivan Balakin <nekonekun@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Ivan Balakin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pyuserside-0.2.0/pyproject.toml` & `pyuserside-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "pyuserside"
 
-version = "0.2.0"
+version = "0.2.1"
 
 description = "Userside API client implementation"
 
 readme = "README.rst"
 
 requires-python = ">=3.10"
```

### Comparing `pyuserside-0.2.0/src/pyuserside/api.py` & `pyuserside-0.2.1/src/pyuserside/api.py`

 * *Files identical despite different names*

### Comparing `pyuserside-0.2.0/src/pyuserside/asyncio/api.py` & `pyuserside-0.2.1/src/pyuserside/asyncio/api.py`

 * *Files identical despite different names*

### Comparing `pyuserside-0.2.0/src/pyuserside.egg-info/PKG-INFO` & `pyuserside-0.2.1/src/pyuserside.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyuserside
-Version: 0.2.0
+Version: 0.2.1
 Summary: Userside API client implementation
 Author-email: Ivan Balakin <nekonekun@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Ivan Balakin
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


# Comparing `tmp/rudderclient-1.5.0.tar.gz` & `tmp/rudderclient-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rudderclient-1.5.0.tar", last modified: Mon May 29 14:30:57 2023, max compression
+gzip compressed data, was "rudderclient-1.6.0.tar", last modified: Mon May 29 14:51:43 2023, max compression
```

## Comparing `rudderclient-1.5.0.tar` & `rudderclient-1.6.0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.176339 rudderclient-1.5.0/
--rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-05-29 14:30:26.000000 rudderclient-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-29 14:30:57.176339 rudderclient-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-05-29 14:30:26.000000 rudderclient-1.5.0/README.md
--rw-r--r--   0 runner    (1001) runner    (1001)      940 2023-05-29 14:30:46.000000 rudderclient-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-05-29 14:30:57.176339 rudderclient-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.172338 rudderclient-1.5.0/src/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.172338 rudderclient-1.5.0/src/rudderclient/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/__init__.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.174338 rudderclient-1.5.0/src/rudderclient/aws/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/aws/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5274 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/aws/requests.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.174338 rudderclient-1.5.0/src/rudderclient/gcp/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/gcp/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     2747 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/gcp/auth.py
--rw-r--r--   0 runner    (1001) runner    (1001)     1087 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/gcp/http_requests.py
--rw-r--r--   0 runner    (1001) runner    (1001)      943 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/gcp/pubsub.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.175339 rudderclient-1.5.0/src/rudderclient/request/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/request/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/request/exceptions.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.175339 rudderclient-1.5.0/src/rudderclient/tools/
--rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/tools/__init__.py
--rw-r--r--   0 runner    (1001) runner    (1001)     5491 2023-05-29 14:30:26.000000 rudderclient-1.5.0/src/rudderclient/tools/send_account_email.py
-drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:30:57.173339 rudderclient-1.5.0/src/rudderclient.egg-info/
--rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-29 14:30:57.000000 rudderclient-1.5.0/src/rudderclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) runner    (1001)      629 2023-05-29 14:30:57.000000 rudderclient-1.5.0/src/rudderclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-05-29 14:30:57.000000 rudderclient-1.5.0/src/rudderclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-05-29 14:30:57.000000 rudderclient-1.5.0/src/rudderclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) runner    (1001)       22 2023-05-29 14:30:57.000000 rudderclient-1.5.0/src/rudderclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:43.626091 rudderclient-1.6.0/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1069 2023-05-29 14:51:15.000000 rudderclient-1.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-29 14:51:43.626091 rudderclient-1.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      224 2023-05-29 14:51:15.000000 rudderclient-1.6.0/README.md
+-rw-r--r--   0 runner    (1001) runner    (1001)      940 2023-05-29 14:51:33.000000 rudderclient-1.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) runner    (1001)       38 2023-05-29 14:51:43.626091 rudderclient-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:43.622090 rudderclient-1.6.0/src/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:43.622090 rudderclient-1.6.0/src/rudderclient/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/__init__.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:43.623090 rudderclient-1.6.0/src/rudderclient/aws/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/aws/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5274 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/aws/requests.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:43.624090 rudderclient-1.6.0/src/rudderclient/gcp/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     2747 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/gcp/auth.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1087 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/gcp/http_requests.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      943 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/gcp/pubsub.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:43.625090 rudderclient-1.6.0/src/rudderclient/request/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/request/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)      528 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/request/exceptions.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     1282 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/request/helpers.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:43.625090 rudderclient-1.6.0/src/rudderclient/tools/
+-rw-r--r--   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/tools/__init__.py
+-rw-r--r--   0 runner    (1001) runner    (1001)     5491 2023-05-29 14:51:15.000000 rudderclient-1.6.0/src/rudderclient/tools/send_account_email.py
+drwxr-xr-x   0 runner    (1001) runner    (1001)        0 2023-05-29 14:51:43.623090 rudderclient-1.6.0/src/rudderclient.egg-info/
+-rw-r--r--   0 runner    (1001) runner    (1001)     1968 2023-05-29 14:51:43.000000 rudderclient-1.6.0/src/rudderclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) runner    (1001)      665 2023-05-29 14:51:43.000000 rudderclient-1.6.0/src/rudderclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)        1 2023-05-29 14:51:43.000000 rudderclient-1.6.0/src/rudderclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       28 2023-05-29 14:51:43.000000 rudderclient-1.6.0/src/rudderclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) runner    (1001)       22 2023-05-29 14:51:43.000000 rudderclient-1.6.0/src/rudderclient.egg-info/top_level.txt
```

### Comparing `rudderclient-1.5.0/LICENSE` & `rudderclient-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rudderclient-1.5.0/PKG-INFO` & `rudderclient-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.5.0
+Version: 1.6.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.5.0/pyproject.toml` & `rudderclient-1.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0.0", "wheel",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "rudderclient"
-version = "1.5.0"
+version = "1.6.0"
 description = "Shared helpers for rudder application functions code"
 readme = "README.md"
 classifiers = [ "License :: OSI Approved :: MIT License", "Programming Language :: Python", "Programming Language :: Python :: 3.10",]
 keywords = [ "rudder", "client", "helper",]
 dependencies = [ "google-cloud-secret-manager",]
 requires-python = ">=3.10"
 [[project.authors]]
```

### Comparing `rudderclient-1.5.0/src/rudderclient/aws/requests.py` & `rudderclient-1.6.0/src/rudderclient/aws/requests.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.5.0/src/rudderclient/gcp/auth.py` & `rudderclient-1.6.0/src/rudderclient/gcp/auth.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.5.0/src/rudderclient/gcp/http_requests.py` & `rudderclient-1.6.0/src/rudderclient/gcp/http_requests.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.5.0/src/rudderclient/gcp/pubsub.py` & `rudderclient-1.6.0/src/rudderclient/gcp/pubsub.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.5.0/src/rudderclient/request/exceptions.py` & `rudderclient-1.6.0/src/rudderclient/request/exceptions.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.5.0/src/rudderclient/tools/send_account_email.py` & `rudderclient-1.6.0/src/rudderclient/tools/send_account_email.py`

 * *Files identical despite different names*

### Comparing `rudderclient-1.5.0/src/rudderclient.egg-info/PKG-INFO` & `rudderclient-1.6.0/src/rudderclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rudderclient
-Version: 1.5.0
+Version: 1.6.0
 Summary: Shared helpers for rudder application functions code
 Author-email: Rudder Team <rudder@realnaut.com>
 License: MIT License
         
         Copyright (c) 2023 RealNaut Ops
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `rudderclient-1.5.0/src/rudderclient.egg-info/SOURCES.txt` & `rudderclient-1.6.0/src/rudderclient.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -12,9 +12,10 @@
 src/rudderclient/aws/requests.py
 src/rudderclient/gcp/__init__.py
 src/rudderclient/gcp/auth.py
 src/rudderclient/gcp/http_requests.py
 src/rudderclient/gcp/pubsub.py
 src/rudderclient/request/__init__.py
 src/rudderclient/request/exceptions.py
+src/rudderclient/request/helpers.py
 src/rudderclient/tools/__init__.py
 src/rudderclient/tools/send_account_email.py
```


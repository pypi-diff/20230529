# Comparing `tmp/LumosWeb-0.0.1.tar.gz` & `tmp/LumosWeb-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LumosWeb-0.0.1.tar", last modified: Mon May 29 12:23:50 2023, max compression
+gzip compressed data, was "LumosWeb-0.0.2.tar", last modified: Mon May 29 12:59:23 2023, max compression
```

## Comparing `LumosWeb-0.0.1.tar` & `LumosWeb-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:23:50.595528 LumosWeb-0.0.1/
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:23:50.304784 LumosWeb-0.0.1/LumosWeb/
--rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.1/LumosWeb/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4085 2023-05-29 11:58:23.000000 LumosWeb-0.0.1/LumosWeb/api.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.1/LumosWeb/middleware.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.1/LumosWeb/response.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:23:50.539044 LumosWeb-0.0.1/LumosWeb.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      364 2023-05-29 12:23:49.000000 LumosWeb-0.0.1/LumosWeb.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      258 2023-05-29 12:23:49.000000 LumosWeb-0.0.1/LumosWeb.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-29 12:23:49.000000 LumosWeb-0.0.1/LumosWeb.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-29 12:23:49.000000 LumosWeb-0.0.1/LumosWeb.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-29 12:23:49.000000 LumosWeb-0.0.1/LumosWeb.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)      364 2023-05-29 12:23:50.589525 LumosWeb-0.0.1/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)       62 2023-05-26 09:16:40.000000 LumosWeb-0.0.1/README.md
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-29 12:23:50.598132 LumosWeb-0.0.1/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1740 2023-05-29 12:22:16.000000 LumosWeb-0.0.1/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:59:23.463206 LumosWeb-0.0.2/
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:59:23.159403 LumosWeb-0.0.2/LumosWeb/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:02:38.000000 LumosWeb-0.0.2/LumosWeb/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     4085 2023-05-29 11:58:23.000000 LumosWeb-0.0.2/LumosWeb/api.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1018 2023-05-26 18:17:43.000000 LumosWeb-0.0.2/LumosWeb/middleware.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      972 2023-05-29 08:01:54.000000 LumosWeb-0.0.2/LumosWeb/response.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-05-29 12:59:23.403240 LumosWeb-0.0.2/LumosWeb.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3836 2023-05-29 12:59:22.000000 LumosWeb-0.0.2/LumosWeb.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      258 2023-05-29 12:59:22.000000 LumosWeb-0.0.2/LumosWeb.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-05-29 12:59:22.000000 LumosWeb-0.0.2/LumosWeb.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      105 2023-05-29 12:59:22.000000 LumosWeb-0.0.2/LumosWeb.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        9 2023-05-29 12:59:22.000000 LumosWeb-0.0.2/LumosWeb.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3836 2023-05-29 12:59:23.456203 LumosWeb-0.0.2/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3653 2023-05-29 12:56:35.000000 LumosWeb-0.0.2/README.md
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-05-29 12:59:23.466218 LumosWeb-0.0.2/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1740 2023-05-29 12:59:06.000000 LumosWeb-0.0.2/setup.py
```

### Comparing `LumosWeb-0.0.1/LumosWeb/api.py` & `LumosWeb-0.0.2/LumosWeb/api.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.1/LumosWeb/middleware.py` & `LumosWeb-0.0.2/LumosWeb/middleware.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.1/LumosWeb/response.py` & `LumosWeb-0.0.2/LumosWeb/response.py`

 * *Files identical despite different names*

### Comparing `LumosWeb-0.0.1/setup.py` & `LumosWeb-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 # Package meta-data.
 NAME = "LumosWeb"
 DESCRIPTION = "LumosWeb is web framework, simple and effective usage"
 EMAIL = "sumeyyedilaradogan@gmail.com"
 AUTHOR = "Sddilora"
 REQUIRES_PYTHON = ">=3.6.0"
-VERSION = "0.0.1"
+VERSION = "0.0.2"
 
 # Which packages are required for this module to be executed?
 REQUIRED = [
     "Jinja2==3.1.2",
     "parse==1.19.0",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
```


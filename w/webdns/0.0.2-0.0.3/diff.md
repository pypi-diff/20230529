# Comparing `tmp/webdns-0.0.2.tar.gz` & `tmp/webdns-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webdns-0.0.2.tar", last modified: Thu May 25 18:23:35 2023, max compression
+gzip compressed data, was "webdns-0.0.3.tar", last modified: Mon May 29 13:10:35 2023, max compression
```

## Comparing `webdns-0.0.2.tar` & `webdns-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:23:35.962000 webdns-0.0.2/
--rw-r--r--   0 root         (0) root         (0)     1055 2023-05-25 14:04:05.000000 webdns-0.0.2/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      718 2023-05-25 18:23:35.961000 webdns-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 18:23:35.962000 webdns-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3975 2023-05-25 14:38:07.000000 webdns-0.0.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:23:35.955000 webdns-0.0.2/webdns/
--rw-r--r--   0 root         (0) root         (0)       75 2023-05-25 13:50:57.000000 webdns-0.0.2/webdns/__init__.py
--rw-r--r--   0 root         (0) root         (0)       98 2023-05-25 18:21:44.000000 webdns-0.0.2/webdns/__version__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:23:35.961000 webdns-0.0.2/webdns/api/
--rw-r--r--   0 root         (0) root         (0)       24 2023-05-25 13:50:59.000000 webdns-0.0.2/webdns/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2083 2023-05-24 14:43:52.000000 webdns-0.0.2/webdns/api/api.py
--rw-r--r--   0 root         (0) root         (0)      826 2023-05-24 14:43:52.000000 webdns-0.0.2/webdns/api/utils.py
--rw-r--r--   0 root         (0) root         (0)     2896 2023-05-24 14:43:52.000000 webdns-0.0.2/webdns/app.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-05-24 20:14:17.000000 webdns-0.0.2/webdns/methods.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 18:23:35.960000 webdns-0.0.2/webdns.egg-info/
--rw-r--r--   0 root         (0) root         (0)      718 2023-05-25 18:23:35.000000 webdns-0.0.2/webdns.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      303 2023-05-25 18:23:35.000000 webdns-0.0.2/webdns.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 18:23:35.000000 webdns-0.0.2/webdns.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-25 18:23:35.000000 webdns-0.0.2/webdns.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-25 18:23:35.000000 webdns-0.0.2/webdns.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:10:35.130000 webdns-0.0.3/
+-rwxrwxr-x   0 root         (0) root         (0)     1055 2023-05-25 14:04:05.000000 webdns-0.0.3/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      720 2023-05-29 13:10:35.129000 webdns-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 13:10:35.130000 webdns-0.0.3/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)     3976 2023-05-25 18:25:34.000000 webdns-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:10:34.964000 webdns-0.0.3/webdns/
+-rwxrwxr-x   0 root         (0) root         (0)       75 2023-05-25 13:50:57.000000 webdns-0.0.3/webdns/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)       98 2023-05-29 13:04:09.000000 webdns-0.0.3/webdns/__version__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:10:35.127000 webdns-0.0.3/webdns/api/
+-rwxrwxr-x   0 root         (0) root         (0)       24 2023-05-25 13:50:59.000000 webdns-0.0.3/webdns/api/__init__.py
+-rwxrwxr-x   0 root         (0) root         (0)     2083 2023-05-24 14:43:52.000000 webdns-0.0.3/webdns/api/api.py
+-rwxrwxr-x   0 root         (0) root         (0)      826 2023-05-24 14:43:52.000000 webdns-0.0.3/webdns/api/utils.py
+-rwxrwxr-x   0 root         (0) root         (0)     2896 2023-05-24 14:43:52.000000 webdns-0.0.3/webdns/app.py
+-rwxrwxr-x   0 root         (0) root         (0)     3394 2023-05-24 20:14:17.000000 webdns-0.0.3/webdns/methods.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 13:10:35.072000 webdns-0.0.3/webdns.egg-info/
+-rwxrwxr-x   0 root         (0) root         (0)      720 2023-05-29 13:10:34.000000 webdns-0.0.3/webdns.egg-info/PKG-INFO
+-rwxrwxr-x   0 root         (0) root         (0)      303 2023-05-29 13:10:34.000000 webdns-0.0.3/webdns.egg-info/SOURCES.txt
+-rwxrwxr-x   0 root         (0) root         (0)        1 2023-05-29 13:10:34.000000 webdns-0.0.3/webdns.egg-info/dependency_links.txt
+-rwxrwxr-x   0 root         (0) root         (0)       26 2023-05-29 13:10:34.000000 webdns-0.0.3/webdns.egg-info/requires.txt
+-rwxrwxr-x   0 root         (0) root         (0)        7 2023-05-29 13:10:34.000000 webdns-0.0.3/webdns.egg-info/top_level.txt
```

### Comparing `webdns-0.0.2/LICENSE.txt` & `webdns-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `webdns-0.0.2/setup.py` & `webdns-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import sys
 from shutil import rmtree
 
 from setuptools import find_packages, setup, Command
 
 # Package meta-data.
 NAME = 'webdns'
-DESCRIPTION = 'DnsMasq utiity to name IP addresses from Netbox NSOT.'
+DESCRIPTION = 'DnsMasq utility to name IP addresses from Netbox NSOT.'
 URL = 'https://git.rnp.br/pop-rj/dns-conectividade'
 EMAIL = 'infra@pop-rj.rnp.br'
 AUTHOR = 'PoP-RJ/RNP - BR'
 REQUIRES_PYTHON = '>=3.8.0'
 VERSION = None # Available at NAME.__version__.py
 
 # What packages are required for this module to be executed?
```

### Comparing `webdns-0.0.2/webdns/api/api.py` & `webdns-0.0.3/webdns/api/api.py`

 * *Files identical despite different names*

### Comparing `webdns-0.0.2/webdns/api/utils.py` & `webdns-0.0.3/webdns/api/utils.py`

 * *Files identical despite different names*

### Comparing `webdns-0.0.2/webdns/app.py` & `webdns-0.0.3/webdns/app.py`

 * *Files identical despite different names*

### Comparing `webdns-0.0.2/webdns/methods.py` & `webdns-0.0.3/webdns/methods.py`

 * *Files identical despite different names*


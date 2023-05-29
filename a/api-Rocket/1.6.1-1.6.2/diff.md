# Comparing `tmp/api-Rocket-1.6.1.tar.gz` & `tmp/api-Rocket-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-Rocket-1.6.1.tar", last modified: Sun May 28 19:09:09 2023, max compression
+gzip compressed data, was "dist\api-Rocket-1.6.2.tar", last modified: Sun May 28 19:14:43 2023, max compression
```

## Comparing `api-Rocket-1.6.1.tar` & `api-Rocket-1.6.2.tar`

### file list

```diff
@@ -1,18 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.403843 api-Rocket-1.6.1/
--rw-rw-rw-   0        0        0       20 2023-05-28 19:09:08.000000 api-Rocket-1.6.1/MANIFEST.in
--rw-rw-rw-   0        0        0      390 2023-05-28 19:09:09.404820 api-Rocket-1.6.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.365758 api-Rocket-1.6.1/api_Rocket/
--rw-rw-rw-   0        0        0      685 2023-05-28 18:53:58.000000 api-Rocket-1.6.1/api_Rocket/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.284703 api-Rocket-1.6.1/api_Rocket/lib/
-drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.389195 api-Rocket-1.6.1/api_Rocket/lib/clients/
--rw-rw-rw-   0        0        0      418 2023-03-20 11:34:29.000000 api-Rocket-1.6.1/api_Rocket/lib/clients/async_client.py
--rw-rw-rw-   0        0        0    10920 2023-05-26 14:58:16.000000 api-Rocket-1.6.1/api_Rocket/lib/clients/client.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.392125 api-Rocket-1.6.1/api_Rocket/lib/clients/exception/
--rw-rw-rw-   0        0        0     1718 2023-03-24 14:12:55.000000 api-Rocket-1.6.1/api_Rocket/lib/clients/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:09:09.381383 api-Rocket-1.6.1/api_Rocket.egg-info/
--rw-rw-rw-   0        0        0      390 2023-05-28 19:09:09.000000 api-Rocket-1.6.1/api_Rocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-05-28 19:09:09.000000 api-Rocket-1.6.1/api_Rocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 19:09:09.000000 api-Rocket-1.6.1/api_Rocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-28 19:09:09.000000 api-Rocket-1.6.1/api_Rocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 19:09:09.407750 api-Rocket-1.6.1/setup.cfg
--rw-rw-rw-   0        0        0      378 2023-05-28 19:09:08.000000 api-Rocket-1.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:14:43.815953 api-Rocket-1.6.2/
+-rw-rw-rw-   0        0        0       20 2023-05-28 19:14:42.000000 api-Rocket-1.6.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      390 2023-05-28 19:14:43.816929 api-Rocket-1.6.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 19:14:43.802281 api-Rocket-1.6.2/api_Rocket/
+-rw-rw-rw-   0        0        0      677 2023-05-28 19:13:01.000000 api-Rocket-1.6.2/api_Rocket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 19:14:43.814976 api-Rocket-1.6.2/api_Rocket.egg-info/
+-rw-rw-rw-   0        0        0      390 2023-05-28 19:14:43.000000 api-Rocket-1.6.2/api_Rocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-05-28 19:14:43.000000 api-Rocket-1.6.2/api_Rocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 19:14:43.000000 api-Rocket-1.6.2/api_Rocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-28 19:14:43.000000 api-Rocket-1.6.2/api_Rocket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 19:14:43.818883 api-Rocket-1.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-05-28 19:14:42.000000 api-Rocket-1.6.2/setup.py
```

### Comparing `api-Rocket-1.6.1/api_Rocket/__init__.py` & `api-Rocket-1.6.2/api_Rocket/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from .lib.clients.client import Client, Trade_Client
-from .lib.clients.async_client import async_Client
+from .clients.client import Client, Trade_Client
+from .clients.async_client import async_Client
 import requests
 import json
 
 
 #information
 __title__ = "api-Rocket"
```


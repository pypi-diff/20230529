# Comparing `tmp/api-Rocket-1.6.3.tar.gz` & `tmp/api-Rocket-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\api-Rocket-1.6.3.tar", last modified: Mon May 29 06:50:14 2023, max compression
+gzip compressed data, was "dist\api-Rocket-1.6.4.tar", last modified: Mon May 29 07:05:43 2023, max compression
```

## Comparing `api-Rocket-1.6.3.tar` & `api-Rocket-1.6.4.tar`

### file list

```diff
@@ -1,17 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 06:50:14.663445 api-Rocket-1.6.3/
--rw-rw-rw-   0        0        0       20 2023-05-29 06:50:11.000000 api-Rocket-1.6.3/MANIFEST.in
--rw-rw-rw-   0        0        0      390 2023-05-29 06:50:14.663445 api-Rocket-1.6.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 06:50:14.622429 api-Rocket-1.6.3/api_Rocket/
--rw-rw-rw-   0        0        0      677 2023-05-29 06:48:21.000000 api-Rocket-1.6.3/api_Rocket/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 06:50:14.636101 api-Rocket-1.6.3/api_Rocket/clients/
--rw-rw-rw-   0        0        0      418 2023-03-20 11:34:29.000000 api-Rocket-1.6.3/api_Rocket/clients/async_client.py
--rw-rw-rw-   0        0        0    10920 2023-05-26 14:58:16.000000 api-Rocket-1.6.3/api_Rocket/clients/client.py
-drwxrwxrwx   0        0        0        0 2023-05-29 06:50:14.654656 api-Rocket-1.6.3/api_Rocket/clients/exception/
--rw-rw-rw-   0        0        0     1718 2023-03-24 14:12:55.000000 api-Rocket-1.6.3/api_Rocket/clients/exception/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-29 06:50:14.631218 api-Rocket-1.6.3/api_Rocket.egg-info/
--rw-rw-rw-   0        0        0      390 2023-05-29 06:50:13.000000 api-Rocket-1.6.3/api_Rocket.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-05-29 06:50:13.000000 api-Rocket-1.6.3/api_Rocket.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 06:50:13.000000 api-Rocket-1.6.3/api_Rocket.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-29 06:50:13.000000 api-Rocket-1.6.3/api_Rocket.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 06:50:14.681023 api-Rocket-1.6.3/setup.cfg
--rw-rw-rw-   0        0        0      378 2023-05-29 06:50:11.000000 api-Rocket-1.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:05:43.224968 api-Rocket-1.6.4/
+-rw-rw-rw-   0        0        0       20 2023-05-29 07:05:42.000000 api-Rocket-1.6.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      390 2023-05-29 07:05:43.225945 api-Rocket-1.6.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-29 07:05:43.215203 api-Rocket-1.6.4/api_Rocket/
+-rw-rw-rw-   0        0        0      677 2023-05-29 06:57:31.000000 api-Rocket-1.6.4/api_Rocket/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:05:43.223992 api-Rocket-1.6.4/api_Rocket.egg-info/
+-rw-rw-rw-   0        0        0      390 2023-05-29 07:05:43.000000 api-Rocket-1.6.4/api_Rocket.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-05-29 07:05:43.000000 api-Rocket-1.6.4/api_Rocket.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 07:05:43.000000 api-Rocket-1.6.4/api_Rocket.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-29 07:05:43.000000 api-Rocket-1.6.4/api_Rocket.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 07:05:43.227898 api-Rocket-1.6.4/setup.cfg
+-rw-rw-rw-   0        0        0      378 2023-05-29 07:05:42.000000 api-Rocket-1.6.4/setup.py
```

### Comparing `api-Rocket-1.6.3/api_Rocket/__init__.py` & `api-Rocket-1.6.4/api_Rocket/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 __author__ = "Redpiar"
 
 __license__ = "MIT"
 
 __copyright__ = "Copyright 2023 Redpiar"
 
-__version__ = '1.6.3'
+__version__ = '1.6.4'
 
 __status__ = "(Beta)"
 
 __newest__ = json.loads(requests.get("https://pypi.org/pypi/api-Rocket/json").text)["info"]["version"]
 
 if __version__ != __newest__:
 	print(f"""
```


# Comparing `tmp/econuker-1.0.7.tar.gz` & `tmp/econuker-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "econuker-1.0.7.tar", last modified: Sat May 20 19:43:36 2023, max compression
+gzip compressed data, was "econuker-1.0.8.tar", last modified: Mon May 29 17:11:04 2023, max compression
```

## Comparing `econuker-1.0.7.tar` & `econuker-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 19:43:36.818910 econuker-1.0.7/
--rw-rw-rw-   0        0        0     3419 2023-05-20 19:43:36.816911 econuker-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2612 2023-05-20 01:22:57.000000 econuker-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 19:43:36.799909 econuker-1.0.7/econuker/
--rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.7/econuker/Exceptions.py
--rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.7/econuker/__init__.py
--rw-rw-rw-   0        0        0    14456 2023-05-20 15:46:49.000000 econuker-1.0.7/econuker/async_client.py
--rw-rw-rw-   0        0        0    13947 2023-05-20 15:45:37.000000 econuker-1.0.7/econuker/client.py
-drwxrwxrwx   0        0        0        0 2023-05-20 19:43:36.814909 econuker-1.0.7/econuker.egg-info/
--rw-rw-rw-   0        0        0     3419 2023-05-20 19:43:36.000000 econuker-1.0.7/econuker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-20 19:43:36.000000 econuker-1.0.7/econuker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 19:43:36.000000 econuker-1.0.7/econuker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-20 19:43:36.000000 econuker-1.0.7/econuker.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-20 19:43:36.000000 econuker-1.0.7/econuker.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 19:43:36.818910 econuker-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1165 2023-05-20 19:43:30.000000 econuker-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 17:11:04.588586 econuker-1.0.8/
+-rw-rw-rw-   0        0        0     5069 2023-05-29 17:11:04.586587 econuker-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     4262 2023-05-29 17:09:06.000000 econuker-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 17:11:04.549817 econuker-1.0.8/econuker/
+-rw-rw-rw-   0        0        0     1368 2023-05-19 23:47:34.000000 econuker-1.0.8/econuker/Exceptions.py
+-rw-rw-rw-   0        0        0      104 2023-05-20 00:09:50.000000 econuker-1.0.8/econuker/__init__.py
+-rw-rw-rw-   0        0        0    14456 2023-05-29 14:15:21.000000 econuker-1.0.8/econuker/async_client.py
+-rw-rw-rw-   0        0        0    13841 2023-05-29 14:15:03.000000 econuker-1.0.8/econuker/client.py
+drwxrwxrwx   0        0        0        0 2023-05-29 17:11:04.579605 econuker-1.0.8/econuker.egg-info/
+-rw-rw-rw-   0        0        0     5069 2023-05-29 17:11:03.000000 econuker-1.0.8/econuker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-29 17:11:04.000000 econuker-1.0.8/econuker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 17:11:03.000000 econuker-1.0.8/econuker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-29 17:11:03.000000 econuker-1.0.8/econuker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 17:11:03.000000 econuker-1.0.8/econuker.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 17:11:04.589583 econuker-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1165 2023-05-29 17:10:58.000000 econuker-1.0.8/setup.py
```

### Comparing `econuker-1.0.7/econuker/Exceptions.py` & `econuker-1.0.8/econuker/Exceptions.py`

 * *Files identical despite different names*

### Comparing `econuker-1.0.7/econuker/async_client.py` & `econuker-1.0.8/econuker/async_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         auth_token (str, optional): The authentication token. Can be None. Must be valid. Defaults to None.
         
         beta (bool, optional): Whether or not to use the BETA API. Defaults to False.
     """
 
     def __init__(self, auth_token: str = None, beta: bool = False):
         self.auth_token: str = auth_token
-        self.base_url: str = "https://beta.econuker.xyz/api" if beta else "https://api.econuker.xyz"
+        self.base_url: str = "https://beta.econuker.xyz/api" if beta else "https://econuker.xyz/api"
         self.auth_level: str = None
 
         if not beta:
             raise EconukerException("Main API is not available at this moment.")
 
         def __check_verify(self) -> Token:
             """
```

### Comparing `econuker-1.0.7/econuker/client.py` & `econuker-1.0.8/econuker/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,20 +99,17 @@
         auth_token (str, optional): The authentication token. Can be None. Must be valid. Defaults to None.
         
         beta (bool, optional): Whether or not to use the BETA API. Defaults to False.
     """
 
     def __init__(self, auth_token: str = None, beta: bool = False):
         self.auth_token: str = auth_token
-        self.base_url: str = "https://beta.econuker.xyz/api" if beta else "https://api.econuker.xyz"
+        self.base_url: str = "https://beta.econuker.xyz/api" if beta else "https://econuker.xyz/api"
         self.auth_level: str = None
 
-        if not beta:
-            raise EconukerException("Main API is not available at this moment.")
-
         def __check_verify(self) -> Token:
             """
             Verifies an authentication token.
 
             Args:
                 auth_token (str): The authentication token to verify.
```

### Comparing `econuker-1.0.7/setup.py` & `econuker-1.0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='econuker',
-    version='1.0.7',
+    version='1.0.8',
     author='YumYummity',
     author_email='034nop@gmail.com',
     description='API wrapper for https://api.econuker.xyz',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type
     url='https://github.com/EcoNuker/EcoNuker-API-Python/',
     packages=find_packages(),
```


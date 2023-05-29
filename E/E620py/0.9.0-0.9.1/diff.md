# Comparing `tmp/E620py-0.9.0.tar.gz` & `tmp/E620py-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "E620py-0.9.0.tar", last modified: Tue Mar  7 16:43:20 2023, max compression
+gzip compressed data, was "E620py-0.9.1.tar", last modified: Mon May 29 17:45:54 2023, max compression
```

## Comparing `E620py-0.9.0.tar` & `E620py-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:43:20.586746 E620py-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-07 16:43:10.000000 E620py-0.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-07 16:43:20.586746 E620py-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-03-07 16:43:10.000000 E620py-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-07 16:43:10.000000 E620py-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 16:43:20.586746 E620py-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:43:20.586746 E620py-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:43:20.586746 E620py-0.9.0/src/E620py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-03-07 16:43:20.000000 E620py-0.9.0/src/E620py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-07 16:43:20.000000 E620py-0.9.0/src/E620py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 16:43:20.000000 E620py-0.9.0/src/E620py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-07 16:43:20.000000 E620py-0.9.0/src/E620py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-07 16:43:20.000000 E620py-0.9.0/src/E620py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 16:43:20.586746 E620py-0.9.0/src/e620py/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-03-07 16:43:10.000000 E620py-0.9.0/src/e620py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20331 2023-03-07 16:43:10.000000 E620py-0.9.0/src/e620py/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8644 2023-03-07 16:43:10.000000 E620py-0.9.0/src/e620py/downloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-03-07 16:43:10.000000 E620py-0.9.0/src/e620py/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-03-07 16:43:10.000000 E620py-0.9.0/src/e620py/file_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-03-07 16:43:10.000000 E620py-0.9.0/src/e620py/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     5709 2023-03-07 16:43:10.000000 E620py-0.9.0/src/e620py/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-03-07 16:43:10.000000 E620py-0.9.0/src/e620py/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:45:54.638410 E620py-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 17:45:43.000000 E620py-0.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-29 17:45:54.638410 E620py-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-29 17:45:43.000000 E620py-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-29 17:45:43.000000 E620py-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:45:54.638410 E620py-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:45:54.638410 E620py-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:45:54.638410 E620py-0.9.1/src/E620py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-29 17:45:54.000000 E620py-0.9.1/src/E620py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-29 17:45:54.000000 E620py-0.9.1/src/E620py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:45:54.000000 E620py-0.9.1/src/E620py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 17:45:54.000000 E620py-0.9.1/src/E620py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 17:45:54.000000 E620py-0.9.1/src/E620py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:45:54.638410 E620py-0.9.1/src/e620py/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19928 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/downloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/file_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9590 2023-05-29 17:45:43.000000 E620py-0.9.1/src/e620py/objects.py
```

### Comparing `E620py-0.9.0/LICENSE` & `E620py-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `E620py-0.9.0/PKG-INFO` & `E620py-0.9.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: E620py
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python library for interacting with the e621 api
 Author: mrcrabs695
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # E620py
 
-E620py is a python library for interacting with the e621 api designed to be simple and easy to use.
+E620py is a python library for interacting with the e621 api.
 
 Here is an example of fetching a single post:
 ```python
 >>> import e620py
 >>> post = e620py.E6get().post_get("order:score", fetch_all=False, fetch_count=1)
 >>> print(post[0].m_id)
 2848682
 ```
 Most functions have doc strings so its easy to quickly see how a function works without having to understand the spaghetti code 💀.
-I will try and implement all of the main features of the e621 api and possibly implement some of the undocumented endpoints.
 
 ## Features
   Post:
   + Fetching
-  + Uploading (uploading a file directly does not work)
+  + Uploading
   + Editing
   + Voting
   + Favorite and unfavorite
   + Downloading
 
   Pool:
   + Fetching (only one page at a time for now)
```

### Comparing `E620py-0.9.0/pyproject.toml` & `E620py-0.9.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 authors = [
     {name="mrcrabs695"}
 ]
 description = "A python library for interacting with the e621 api"
 readme = "README.md"
 requires-python = ">=3.10"
 dependencies = [
-    "requests"
+    "httpx"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "License :: OSI Approved :: MIT License",
 ]
```

### Comparing `E620py-0.9.0/src/E620py.egg-info/PKG-INFO` & `E620py-0.9.1/src/E620py.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: E620py
-Version: 0.9.0
+Version: 0.9.1
 Summary: A python library for interacting with the e621 api
 Author: mrcrabs695
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # E620py
 
-E620py is a python library for interacting with the e621 api designed to be simple and easy to use.
+E620py is a python library for interacting with the e621 api.
 
 Here is an example of fetching a single post:
 ```python
 >>> import e620py
 >>> post = e620py.E6get().post_get("order:score", fetch_all=False, fetch_count=1)
 >>> print(post[0].m_id)
 2848682
 ```
 Most functions have doc strings so its easy to quickly see how a function works without having to understand the spaghetti code 💀.
-I will try and implement all of the main features of the e621 api and possibly implement some of the undocumented endpoints.
 
 ## Features
   Post:
   + Fetching
-  + Uploading (uploading a file directly does not work)
+  + Uploading
   + Editing
   + Voting
   + Favorite and unfavorite
   + Downloading
 
   Pool:
   + Fetching (only one page at a time for now)
```

### Comparing `E620py-0.9.0/src/e620py/api.py` & `E620py-0.9.1/src/e620py/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -202,15 +202,15 @@
         Returns:
             A list of PostObject instances representing the retrieved posts.
             
         Raises:
             - AuthError: If the session is not authenticated and username is not provided
             - NoResults: If there are no posts that match the given search query.
         """
-        #? im most likely going to replace this method with the old way i did it as there really aren't any benefits to doing it like this
+        self.e6get_log.warning('favorites_get is deprecated, if you want to fetch favorites, use the regular post_get and append "fav:[user here]" to the tags arg')
 
         endpoint = "/favorites.json"
         tags = "order:id"
         get_options = {'limit': fetch_count}
 
         if username == None and self.session.auth == False:
             self.e6get_log.error("No username provided and not logged in")
@@ -372,17 +372,14 @@
         description=None,
         file=None,
         direct_url=None,
         parent_id=None,
     ):
         """
         Uploads a post to e621.
-        
-        Note that the method currently does not support uploading files directly and will raise a warning if a file argument is provided.
-        Instead, the direct_url argument should be used.
 
         Args:
             - tags (str): The tags to apply to the post.
             - rating (str): The rating of the post.
             - source (str): The source of the post. Can be an empty string
             - description (str, optional): A description of the post. Defaults to None.
             - file (file, optional): A file object to upload. Defaults to None.
@@ -398,30 +395,24 @@
             'upload[rating]': rating,
             'upload[source]': source,
             'upload[description]': description,
             'upload[parent_id]': parent_id,
         }
 
         if file != None:
-            # file_md5 = file_handling.calculate_md5(file)
-            # post_data = {**post_data, 'upload[file]': (file.name, file)}
-
-            self.e6post_log.warning(
-                "Direct uploads dont work for now, use direct_url until its fixed"
-            )
-            return
+            post_file = {'upload[file]': file}
 
         elif direct_url != None:
             post_data = {**post_data, 'upload[direct_url]': direct_url}
 
         else:
             self.e6post_log.error("Uploading post failed, no file given or direct url")
             return
 
-        request = self.session.post_request("/uploads.json", files=post_data)
+        request = self.session.post_request("/uploads.json", data=post_data, files=post_file)
 
         self.e6post_log.info(f"Post uploaded successfully! Id: {request['post_id']}")
         return request
 
     def edit_post(
         self,
         post_id,
```

### Comparing `E620py-0.9.0/src/e620py/downloader.py` & `E620py-0.9.1/src/e620py/downloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """
 Provides functions for downloading posts and other data
 """
 #? the functions here will be made after the main api is done
+#* this whole module is honestly quite shit, im gonna rewrite it at some point. this actually hurts looking at :skull_emoguy:
 
-import requests
+import httpx
 import os
 import logging
 import json
 from . import objects as ob
 from . import exceptions
 from .logging import main_log
 
@@ -73,22 +74,24 @@
         self.download_log.info(f"Downloading post: {post.m_id}")
         
         if os.path.isfile(post.filename) and not skip_downloaded_check:
             self.download_log.info(f"Post {post.m_id} already saved")
             return False, "already saved"
 
         try:
-            download = requests.get(post.m_data['url'], stream=True)
-        except requests.exceptions.MissingSchema:
+            with httpx.stream("GET", post.m_data['url']) as download:
+                with open(post.filename, 'wb') as file:
+                    
+                    for chunk in download.iter_bytes():
+                        file.write(chunk)
+                        
+        except httpx.InvalidURL:
             self.download_log.warning(f"Post {post.m_id} has no valid url")
             return False, "invalid url"
         
-        with open(post.filename, 'wb') as file:
-            for chunk in download.iter_content(chunk_size=1024):
-                file.write(chunk)
         return True, ""
     
     def __single_pool_download(self, pool, skip_downloaded_check=False, save_old_posts=False):
     
         self.download_log.info(f"Downloading pool: {pool.m_id}")
         
         if os.path.isdir(pool.folder_name) and not skip_downloaded_check:
```

### Comparing `E620py-0.9.0/src/e620py/exceptions.py` & `E620py-0.9.1/src/e620py/exceptions.py`

 * *Files identical despite different names*

### Comparing `E620py-0.9.0/src/e620py/file_handling.py` & `E620py-0.9.1/src/e620py/file_handling.py`

 * *Files identical despite different names*

### Comparing `E620py-0.9.0/src/e620py/networking.py` & `E620py-0.9.1/src/e620py/networking.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 Handles the actual requests being made and checking the responses for errors
 """
 
-import requests
+import httpx
 import json
 from . import objects as ob
 from . import __user_agent__, base_url, exceptions
 from .logging import main_log
 
 
 class ConnectionHandler:
@@ -18,39 +18,39 @@
     def __init__(self, url=base_url):
 
         self.connection_handler_log = main_log.getChild("Connection_Handler")
 
         self.url = url
         self.user_agent = {'user-agent': __user_agent__}
         try:
-            requests.get(url=self.url, headers=self.user_agent)
-        except requests.ConnectionError as error:
+            httpx.get(url=self.url, headers=self.user_agent)
+        except httpx.ConnectError as error:
             self.connection_handler_log.error(
                 "Something went wrong while connecting to url, check your internet and try again"
             )
             raise exceptions.NetworkError(
                 "Something went wrong while connecting to url", error
             )
 
         self.auth = False
-        self.session = requests.Session()
+        self.session = httpx.Client()
         self.session.headers.update(self.user_agent)
 
     def update_auth(self, username, api_key) -> bool:
         """
         The update_auth function updates the session with a new username and api key.
             It does this by making a request to the favorites endpoint, which requires authentication.
             If the request is successful, it updates the session with the new auth.
 
         :param username: Used to Set the username for the session.
         :param api_key: Used to Authenticate the user.
         :return: True if auth is valid, otherwise False
         """
 
-        request = requests.get(
+        request = httpx.get(
             url=f"{self.url}/favorites.json",
             headers=self.user_agent,
             auth=(username, api_key),
         )
 
         if request.status_code == 401:
             self.connection_handler_log.error(
@@ -83,41 +83,41 @@
             This function returns a dict object containing all of the data returned by the API.
         """
 
         try:
             request = self.session.get(url=self.url + url_endpoint, params=options)
             request.raise_for_status()
 
-        except requests.HTTPError as error:
+        except httpx.HTTPError as error:
             self.raise_network_error(request, error, "Get")
 
         return json.loads(request.text)
 
     def post_request(self, url_endpoint, data=None, files=None):
 
         try:
             if files != None:
-                request = self.session.post(url=self.url + url_endpoint, files=files)
+                request = self.session.post(url=self.url + url_endpoint, files=files, data=data)
             else:
                 request = self.session.post(url=self.url + url_endpoint, data=data)
             request.raise_for_status()
 
-        except requests.HTTPError as error:
+        except httpx.HTTPError as error:
             self.raise_network_error(request, error, "Post")
 
         return json.loads(request.text)
 
     def delete_request(self, url_endpoint):
         # * this function does not come with an options parameter, but if need be i can add one later
 
         try:
             request = self.session.delete(url=self.url + url_endpoint)
             request.raise_for_status()
 
-        except requests.HTTPError as error:
+        except httpx.HTTPError as error:
             self.raise_network_error(request, error, "Delete")
 
         try:
             return json.loads(request.text)
 
         except json.JSONDecodeError:
             self.connection_handler_log.critical("Non json content")
@@ -125,15 +125,15 @@
 
     def patch_request(self, url_endpoint, options):
 
         try:
             request = self.session.patch(url=self.url + url_endpoint, params=options)
             request.raise_for_status()
 
-        except requests.HTTPError() as error:
+        except httpx.HTTPError() as error:
             self.raise_network_error(request, error, "Patch")
 
         try:
             return json.loads(request.text)
 
         except json.JSONDecodeError:
             self.connection_handler_log.critical("Non json content")
@@ -141,15 +141,15 @@
         
     def put_request(self, url_endpoint, options):
 
         try:
             request = self.session.put(url=self.url + url_endpoint, params=options)
             request.raise_for_status()
 
-        except requests.HTTPError() as error:
+        except httpx.HTTPError() as error:
             self.raise_network_error(request, error, "Put")
 
         try:
             return json.loads(request.text)
 
         except json.JSONDecodeError:
             self.connection_handler_log.debug("Non json content")
```

### Comparing `E620py-0.9.0/src/e620py/objects.py` & `E620py-0.9.1/src/e620py/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Contains objects and types commonly used in bingus lib modules
+Contains objects and types commonly used in e620py modules
 """
 
 from . import api
 
 class PostObject:
     def __init__(self):
         # metadata vars, most strings are None when first initialized since the values when fetched can be null if there was no data attached
```


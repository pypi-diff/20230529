# Comparing `tmp/wf_video_io-3.3.4.tar.gz` & `tmp/wf_video_io-3.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf_video_io-3.3.4.tar", max compression
+gzip compressed data, was "wf_video_io-3.3.5.tar", max compression
```

## Comparing `wf_video_io-3.3.4.tar` & `wf_video_io-3.3.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.3.4/LICENSE
--rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.3.4/README.md
--rw-r--r--   0        0        0     1162 2023-05-29 18:04:26.822155 wf_video_io-3.3.4/pyproject.toml
--rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.3.4/video_io/__init__.py
--rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.3.4/video_io/client/__init__.py
--rwxr-xr-x   0        0        0    17350 2023-05-29 18:04:06.027409 wf_video_io-3.3.4/video_io/client/core.py
--rw-r--r--   0        0        0      308 2023-05-25 17:31:09.138857 wf_video_io-3.3.4/video_io/client/errors.py
--rw-r--r--   0        0        0     3385 2023-05-25 18:28:00.924148 wf_video_io-3.3.4/video_io/client/utils.py
--rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.3.4/video_io/config.py
--rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.3.4/video_io/core.py
--rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.3.4/video_io/log_retry.py
--rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.3.4/video_io/utils.py
--rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.3.4/video_io/video_reader.py
--rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.3.4/setup.py
--rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.3.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1088 2022-07-13 02:25:51.284383 wf_video_io-3.3.5/LICENSE
+-rwxr-xr-x   0        0        0      278 2023-01-27 16:56:30.309581 wf_video_io-3.3.5/README.md
+-rw-r--r--   0        0        0     1162 2023-05-29 18:34:29.454143 wf_video_io-3.3.5/pyproject.toml
+-rwxr-xr-x   0        0        0       28 2022-07-13 02:25:51.323025 wf_video_io-3.3.5/video_io/__init__.py
+-rw-r--r--   0        0        0       37 2022-10-13 19:42:09.408938 wf_video_io-3.3.5/video_io/client/__init__.py
+-rwxr-xr-x   0        0        0    17319 2023-05-29 18:34:10.695630 wf_video_io-3.3.5/video_io/client/core.py
+-rw-r--r--   0        0        0      308 2023-05-25 17:31:09.138857 wf_video_io-3.3.5/video_io/client/errors.py
+-rw-r--r--   0        0        0     3385 2023-05-25 18:28:00.924148 wf_video_io-3.3.5/video_io/client/utils.py
+-rw-r--r--   0        0        0     1742 2023-05-15 17:34:04.821553 wf_video_io-3.3.5/video_io/config.py
+-rwxr-xr-x   0        0        0    47659 2023-05-15 17:34:04.959430 wf_video_io-3.3.5/video_io/core.py
+-rw-r--r--   0        0        0      382 2023-05-15 17:34:04.811182 wf_video_io-3.3.5/video_io/log_retry.py
+-rw-r--r--   0        0        0    10067 2023-05-15 17:34:04.860739 wf_video_io-3.3.5/video_io/utils.py
+-rw-r--r--   0        0        0      585 2023-01-27 16:56:30.326420 wf_video_io-3.3.5/video_io/video_reader.py
+-rw-r--r--   0        0        0     1261 1970-01-01 00:00:00.000000 wf_video_io-3.3.5/setup.py
+-rw-r--r--   0        0        0     1345 1970-01-01 00:00:00.000000 wf_video_io-3.3.5/PKG-INFO
```

### Comparing `wf_video_io-3.3.4/LICENSE` & `wf_video_io-3.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.4/pyproject.toml` & `wf_video_io-3.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "wf-video-io"
 dynamic = ["version"]
 
 [tool.poetry]
 name = "wf-video-io"
-version = "3.3.4"
+version = "3.3.5"
 description = "Library for working with video files and interacting with the wildflower video-service"
 authors = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>"]
 maintainers = ["Paul J DeCoursey <paul@decoursey.net>", "Theodore Quinn <ted.quinn@wildflowerschools.org>", "Benjamin Jaffe-Talberg <ben.talberg@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "video_io"}]
```

### Comparing `wf_video_io-3.3.4/video_io/client/core.py` & `wf_video_io-3.3.5/video_io/client/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,14 @@
         )
 
     async def _upload_videos(self, file_details: List[Dict]):
         request = {
             "method": "POST",
             "url": f"{self.URL}/videos",
             "headers": self.headers,
-            "timeout": 45,
         }
 
         files = []
         videos = []
         results = []
         for details in file_details:
             try:
@@ -338,15 +337,15 @@
             videos.append(meta)
 
         request["files"] = files
         request["data"] = {"videos": json.dumps(videos)}
         try:
             request = requests.Request(**request)
             r = request.prepare()
-            response = self.request_session.send(r)
+            response = self.request_session.send(r, timeout=45)
             response.raise_for_status()
 
             for ii, vr in enumerate(response.json()):
                 results.append(
                     {
                         "path": videos[ii]["meta"]["path"],
                         "uploaded": True,
@@ -380,20 +379,19 @@
             raise e
 
     async def video_existence_check(self, paths: List[str]):
         request = {
             "method": "POST",
             "url": f"{self.URL}/videos/check",
             "headers": self.headers,
-            "json": paths,
-            "timeout": 45,
+            "json": paths
         }
         try:
             r = requests.Request(**request).prepare()
-            response = self.request_session.send(r)
+            response = self.request_session.send(r, timeout=45)
             try:
                 return response.json()
             except Exception:
                 print(response.text)
                 return [
                     {"err": "response error", "path": p, "exists": False} for p in paths
                 ]
```

### Comparing `wf_video_io-3.3.4/video_io/client/utils.py` & `wf_video_io-3.3.5/video_io/client/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.4/video_io/config.py` & `wf_video_io-3.3.5/video_io/config.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.4/video_io/core.py` & `wf_video_io-3.3.5/video_io/core.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.4/video_io/utils.py` & `wf_video_io-3.3.5/video_io/utils.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.4/video_io/video_reader.py` & `wf_video_io-3.3.5/video_io/video_reader.py`

 * *Files identical despite different names*

### Comparing `wf_video_io-3.3.4/setup.py` & `wf_video_io-3.3.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'wf-cv-utils>=3.4.0',
  'wf-fastapi-auth0>=1.0',
  'wf-gqlpycgen>=0.7.4,<0.8.0',
  'wf-honeycomb-io>=2.0.0']
 
 setup_kwargs = {
     'name': 'wf-video-io',
-    'version': '3.3.4',
+    'version': '3.3.5',
     'description': 'Library for working with video files and interacting with the wildflower video-service',
     'long_description': '# video_io\n\nTools for accessing Wildflower video data\n\n## Test\n\nTests are written with *behave* and *pytest*. As of 11/10/2022, *behave* tests are not functional.\n\n__Run pytest tests__\n\n```pytest```\n\n## Task list\n* ~~Add ability to request concatenation of videos~~ (11/7/2022)\n',
     'author': 'Paul J DeCoursey',
     'author_email': 'paul@decoursey.net',
     'maintainer': 'Paul J DeCoursey',
     'maintainer_email': 'paul@decoursey.net',
     'url': 'None',
```

### Comparing `wf_video_io-3.3.4/PKG-INFO` & `wf_video_io-3.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wf-video-io
-Version: 3.3.4
+Version: 3.3.5
 Summary: Library for working with video files and interacting with the wildflower video-service
 License: MIT
 Author: Paul J DeCoursey
 Author-email: paul@decoursey.net
 Maintainer: Paul J DeCoursey
 Maintainer-email: paul@decoursey.net
 Requires-Python: >=3.8,<3.12
```


# Comparing `tmp/video_utils-2.3.1.tar.gz` & `tmp/video_utils-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "video_utils-2.3.1.tar", max compression
+gzip compressed data, was "video_utils-2.3.2.tar", max compression
```

## Comparing `video_utils-2.3.1.tar` & `video_utils-2.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1078 2023-05-23 11:07:11.915122 video_utils-2.3.1/LICENSE.md
--rw-r--r--   0        0        0     1368 2023-05-23 11:07:11.915122 video_utils-2.3.1/README.md
--rw-r--r--   0        0        0      744 2023-05-23 11:07:11.915122 video_utils-2.3.1/pyproject.toml
--rw-r--r--   0        0        0      166 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/__init__.py
--rw-r--r--   0        0        0     1802 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/codec.py
--rw-r--r--   0        0        0      274 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/colour.py
--rw-r--r--   0        0        0     5661 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/fileMap.py
--rw-r--r--   0        0        0      962 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/parse_episode.py
--rw-r--r--   0        0        0     1549 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/validators.py
--rw-r--r--   0        0        0     3811 2023-05-23 11:07:11.915122 video_utils-2.3.1/video_utils/video.py
--rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 video_utils-2.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-29 02:01:12.915944 video_utils-2.3.2/LICENSE.md
+-rw-r--r--   0        0        0     1368 2023-05-29 02:01:12.915944 video_utils-2.3.2/README.md
+-rw-r--r--   0        0        0      744 2023-05-29 02:01:12.915944 video_utils-2.3.2/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-05-29 02:01:12.915944 video_utils-2.3.2/video_utils/__init__.py
+-rw-r--r--   0        0        0     1802 2023-05-29 02:01:12.915944 video_utils-2.3.2/video_utils/codec.py
+-rw-r--r--   0        0        0      274 2023-05-29 02:01:12.915944 video_utils-2.3.2/video_utils/colour.py
+-rw-r--r--   0        0        0     5661 2023-05-29 02:01:12.915944 video_utils-2.3.2/video_utils/fileMap.py
+-rw-r--r--   0        0        0      962 2023-05-29 02:01:12.915944 video_utils-2.3.2/video_utils/parse_episode.py
+-rw-r--r--   0        0        0     1730 2023-05-29 02:01:12.915944 video_utils-2.3.2/video_utils/validators.py
+-rw-r--r--   0        0        0     3811 2023-05-29 02:01:12.915944 video_utils-2.3.2/video_utils/video.py
+-rw-r--r--   0        0        0     2265 1970-01-01 00:00:00.000000 video_utils-2.3.2/PKG-INFO
```

### Comparing `video_utils-2.3.1/LICENSE.md` & `video_utils-2.3.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `video_utils-2.3.1/README.md` & `video_utils-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `video_utils-2.3.1/pyproject.toml` & `video_utils-2.3.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "video_utils"
-version = "2.3.1"
+version = "2.3.2"
 description = "This library is used for lots of shared functionality around parsing TV shows and movies"
 authors = ["Justin Dray <justin@dray.be>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
```

### Comparing `video_utils-2.3.1/video_utils/codec.py` & `video_utils-2.3.2/video_utils/codec.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.3.1/video_utils/fileMap.py` & `video_utils-2.3.2/video_utils/fileMap.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.3.1/video_utils/parse_episode.py` & `video_utils-2.3.2/video_utils/parse_episode.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.3.1/video_utils/validators.py` & `video_utils-2.3.2/video_utils/validators.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,24 @@
+from os.path import basename
+
 VALID_EXTENSIONS = ("avi", "divx", "mkv", "mp4", "mpg",
                     "mpeg", "mov", "m4v", "flv", "ts", "wmv")
 
 # This can't be an enum because you can't have numbers at the start of the enums
 VALID_QUALITIES = ("2160p", "1080p", "720p", "SD", "Unknown")
 
 
 class Validator:
 
     def is_video(self, file_path):
         return file_path.lower().endswith(VALID_EXTENSIONS)
 
+    def is_temporary_file(self, file_path):
+        return basename(file_path).lower().startswith("._")
+
     def quality_similar_to(self, track):
         # TODO: Refactor this; it's not a validator
         if self.track_resolution_similar_to(track, 3840, 2160):
             return "2160p"
         if self.track_resolution_similar_to(track, 1920, 1080):
             return "1080p"
         if self.track_resolution_similar_to(track, 1280, 720):
@@ -36,11 +41,11 @@
 
 
 class Filter:
     def only_videos(self, file_list):
         validator = Validator()
         videos = []
         for filename in file_list:
-            if validator.is_video(filename):
+            if validator.is_video(filename) and not validator.is_temporary_file(filename):
                 videos.append(filename)
         videos.sort()
         return videos
```

### Comparing `video_utils-2.3.1/video_utils/video.py` & `video_utils-2.3.2/video_utils/video.py`

 * *Files identical despite different names*

### Comparing `video_utils-2.3.1/PKG-INFO` & `video_utils-2.3.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: video-utils
-Version: 2.3.1
+Version: 2.3.2
 Summary: This library is used for lots of shared functionality around parsing TV shows and movies
 License: MIT
 Author: Justin Dray
 Author-email: justin@dray.be
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


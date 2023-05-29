# Comparing `tmp/aij-1.2.8.tar.gz` & `tmp/aij-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.2.8.tar", last modified: Mon May 29 15:04:06 2023, max compression
+gzip compressed data, was "aij-1.2.9.tar", last modified: Mon May 29 15:12:37 2023, max compression
```

## Comparing `aij-1.2.8.tar` & `aij-1.2.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.489664 aij-1.2.8/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.8/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-29 15:04:06.487661 aij-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.8/README.md
--rw-rw-rw-   0        0        0     7696 2023-05-29 15:03:56.000000 aij-1.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 15:04:06.489664 aij-1.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.399408 aij-1.2.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.437789 aij-1.2.8/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      841 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      725 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      606 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      202 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.439786 aij-1.2.8/src/animation/
--rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.8/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.441779 aij-1.2.8/src/chat/
--rw-rw-rw-   0        0        0     4002 2023-05-29 14:13:33.000000 aij-1.2.8/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.443787 aij-1.2.8/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.8/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.446785 aij-1.2.8/src/emotion/
--rw-rw-rw-   0        0        0     2688 2023-05-29 14:18:56.000000 aij-1.2.8/src/emotion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.447781 aij-1.2.8/src/entity/
--rw-rw-rw-   0        0        0      651 2023-05-29 14:09:50.000000 aij-1.2.8/src/entity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.449777 aij-1.2.8/src/face/
--rw-rw-rw-   0        0        0     7945 2023-05-29 14:08:59.000000 aij-1.2.8/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.451164 aij-1.2.8/src/fake/
--rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.8/src/fake/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.452181 aij-1.2.8/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.8/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.454194 aij-1.2.8/src/keyboard/
--rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.8/src/keyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.456191 aij-1.2.8/src/knowledge/
--rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.8/src/knowledge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.458184 aij-1.2.8/src/language/
--rw-rw-rw-   0        0        0      673 2023-05-29 14:16:07.000000 aij-1.2.8/src/language/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.460579 aij-1.2.8/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.8/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.462589 aij-1.2.8/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.8/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.464593 aij-1.2.8/src/objectron/
--rw-rw-rw-   0        0        0     1992 2023-05-29 14:03:52.000000 aij-1.2.8/src/objectron/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.465589 aij-1.2.8/src/scrape/
--rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.8/src/scrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.467597 aij-1.2.8/src/selfie/
--rw-rw-rw-   0        0        0     3671 2023-05-29 14:00:41.000000 aij-1.2.8/src/selfie/__ini__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.468591 aij-1.2.8/src/sentiment/
--rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.8/src/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.470590 aij-1.2.8/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.8/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.471594 aij-1.2.8/src/stream/
--rw-rw-rw-   0        0        0     1976 2023-05-29 00:10:40.000000 aij-1.2.8/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.473592 aij-1.2.8/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.8/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.474661 aij-1.2.8/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.8/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.478686 aij-1.2.8/src/voice/
--rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.8/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.481678 aij-1.2.8/src/volume/
--rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.8/src/volume/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.482662 aij-1.2.8/src/webcam/
--rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.8/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.484661 aij-1.2.8/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.8/src/webcam2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.485665 aij-1.2.8/src/webcam3/
--rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.8/src/webcam3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.113572 aij-1.2.9/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.9/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-29 15:12:37.113572 aij-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.9/README.md
+-rw-rw-rw-   0        0        0     7696 2023-05-29 15:12:27.000000 aij-1.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 15:12:37.114599 aij-1.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.021978 aij-1.2.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.063309 aij-1.2.9/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-29 15:12:36.000000 aij-1.2.9/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2023-05-29 15:12:36.000000 aij-1.2.9/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 15:12:36.000000 aij-1.2.9/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      725 2023-05-29 15:12:36.000000 aij-1.2.9/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      606 2023-05-29 15:12:36.000000 aij-1.2.9/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      202 2023-05-29 15:12:36.000000 aij-1.2.9/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.066295 aij-1.2.9/src/animation/
+-rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.9/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.069293 aij-1.2.9/src/chat/
+-rw-rw-rw-   0        0        0     4002 2023-05-29 14:13:33.000000 aij-1.2.9/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.071302 aij-1.2.9/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.9/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.073299 aij-1.2.9/src/emotion/
+-rw-rw-rw-   0        0        0     2688 2023-05-29 14:18:56.000000 aij-1.2.9/src/emotion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.074295 aij-1.2.9/src/entity/
+-rw-rw-rw-   0        0        0      651 2023-05-29 14:09:50.000000 aij-1.2.9/src/entity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.076290 aij-1.2.9/src/face/
+-rw-rw-rw-   0        0        0     7945 2023-05-29 14:08:59.000000 aij-1.2.9/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.077296 aij-1.2.9/src/fake/
+-rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.9/src/fake/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.079294 aij-1.2.9/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.9/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.081289 aij-1.2.9/src/keyboard/
+-rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.9/src/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.082300 aij-1.2.9/src/knowledge/
+-rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.9/src/knowledge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.083298 aij-1.2.9/src/language/
+-rw-rw-rw-   0        0        0      673 2023-05-29 14:16:07.000000 aij-1.2.9/src/language/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.085291 aij-1.2.9/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.9/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.087297 aij-1.2.9/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.9/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.088295 aij-1.2.9/src/objectron/
+-rw-rw-rw-   0        0        0     1992 2023-05-29 14:03:52.000000 aij-1.2.9/src/objectron/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.090291 aij-1.2.9/src/scrape/
+-rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.9/src/scrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.092296 aij-1.2.9/src/selfie/
+-rw-rw-rw-   0        0        0     3671 2023-05-29 14:00:41.000000 aij-1.2.9/src/selfie/__ini__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.094289 aij-1.2.9/src/sentiment/
+-rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.9/src/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.096295 aij-1.2.9/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.9/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.097289 aij-1.2.9/src/stream/
+-rw-rw-rw-   0        0        0     1976 2023-05-29 00:10:40.000000 aij-1.2.9/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.098291 aij-1.2.9/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.9/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.100301 aij-1.2.9/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.9/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.103307 aij-1.2.9/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.9/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.105293 aij-1.2.9/src/volume/
+-rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.9/src/volume/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.107317 aij-1.2.9/src/webcam/
+-rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.9/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.109317 aij-1.2.9/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.9/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:12:37.110323 aij-1.2.9/src/webcam3/
+-rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.9/src/webcam3/__init__.py
```

### Comparing `aij-1.2.8/LICENSE.txt` & `aij-1.2.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/PKG-INFO` & `aij-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.8
+Version: 1.2.9
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.8/README.md` & `aij-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/pyproject.toml` & `aij-1.2.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.2.8"
+version = "1.2.9"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-1.2.8/src/aij.egg-info/PKG-INFO` & `aij-1.2.9/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.8
+Version: 1.2.9
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.8/src/aij.egg-info/SOURCES.txt` & `aij-1.2.9/src/aij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/aij.egg-info/entry_points.txt` & `aij-1.2.9/src/aij.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/aij.egg-info/requires.txt` & `aij-1.2.9/src/aij.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/animation/__init__.py` & `aij-1.2.9/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/chat/__init__.py` & `aij-1.2.9/src/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/download/__init__.py` & `aij-1.2.9/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/emotion/__init__.py` & `aij-1.2.9/src/emotion/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/entity/__init__.py` & `aij-1.2.9/src/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/face/__init__.py` & `aij-1.2.9/src/face/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/fake/__init__.py` & `aij-1.2.9/src/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/intro/__init__.py` & `aij-1.2.9/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/keyboard/__init__.py` & `aij-1.2.9/src/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/knowledge/__init__.py` & `aij-1.2.9/src/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/language/__init__.py` & `aij-1.2.9/src/language/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/messaging/__init__.py` & `aij-1.2.9/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/news/__init__.py` & `aij-1.2.9/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/objectron/__init__.py` & `aij-1.2.9/src/objectron/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/scrape/__init__.py` & `aij-1.2.9/src/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/selfie/__ini__.py` & `aij-1.2.9/src/selfie/__ini__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/sentiment/__init__.py` & `aij-1.2.9/src/sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/setup/__init__.py` & `aij-1.2.9/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/stream/__init__.py` & `aij-1.2.9/src/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/transcribe/__init__.py` & `aij-1.2.9/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/translate/__init__.py` & `aij-1.2.9/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/voice/__init__.py` & `aij-1.2.9/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/volume/__init__.py` & `aij-1.2.9/src/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/webcam/__init__.py` & `aij-1.2.9/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/webcam2/__init__.py` & `aij-1.2.9/src/webcam2/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.8/src/webcam3/__init__.py` & `aij-1.2.9/src/webcam3/__init__.py`

 * *Files identical despite different names*


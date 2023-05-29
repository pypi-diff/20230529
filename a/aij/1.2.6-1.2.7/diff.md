# Comparing `tmp/aij-1.2.6.tar.gz` & `tmp/aij-1.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.2.6.tar", last modified: Mon May 29 14:01:01 2023, max compression
+gzip compressed data, was "aij-1.2.7.tar", last modified: Mon May 29 14:04:07 2023, max compression
```

## Comparing `aij-1.2.6.tar` & `aij-1.2.7.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.806507 aij-1.2.6/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.6/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-29 14:01:01.805505 aij-1.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.6/README.md
--rw-rw-rw-   0        0        0     7696 2023-05-29 14:00:47.000000 aij-1.2.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 14:01:01.806507 aij-1.2.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.700782 aij-1.2.6/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.743841 aij-1.2.6/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      841 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      725 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      606 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      202 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.745844 aij-1.2.6/src/animation/
--rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.6/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.748844 aij-1.2.6/src/chat/
--rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.6/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.750354 aij-1.2.6/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.6/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.752370 aij-1.2.6/src/emotion/
--rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.6/src/emotion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.755375 aij-1.2.6/src/entity/
--rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.6/src/entity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.758378 aij-1.2.6/src/face/
--rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.6/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.760914 aij-1.2.6/src/fake/
--rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.6/src/fake/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.762940 aij-1.2.6/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.6/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.766937 aij-1.2.6/src/keyboard/
--rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.6/src/keyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.767935 aij-1.2.6/src/knowledge/
--rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.6/src/knowledge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.769938 aij-1.2.6/src/language/
--rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.6/src/language/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.771950 aij-1.2.6/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.6/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.773944 aij-1.2.6/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.6/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.775638 aij-1.2.6/src/objectron/
--rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.2.6/src/objectron/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.777165 aij-1.2.6/src/scrape/
--rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.6/src/scrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.779725 aij-1.2.6/src/selfie/
--rw-rw-rw-   0        0        0     3671 2023-05-29 14:00:41.000000 aij-1.2.6/src/selfie/__ini__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.781871 aij-1.2.6/src/sentiment/
--rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.6/src/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.783845 aij-1.2.6/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.6/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.784850 aij-1.2.6/src/stream/
--rw-rw-rw-   0        0        0     1976 2023-05-29 00:10:40.000000 aij-1.2.6/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.788397 aij-1.2.6/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.6/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.790938 aij-1.2.6/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.6/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.792939 aij-1.2.6/src/voice/
--rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.6/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.796481 aij-1.2.6/src/volume/
--rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.6/src/volume/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.799507 aij-1.2.6/src/webcam/
--rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.6/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.801506 aij-1.2.6/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.6/src/webcam2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.803505 aij-1.2.6/src/webcam3/
--rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.6/src/webcam3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.435872 aij-1.2.7/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.7/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-29 14:04:07.435872 aij-1.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.7/README.md
+-rw-rw-rw-   0        0        0     7696 2023-05-29 14:03:57.000000 aij-1.2.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 14:04:07.437287 aij-1.2.7/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.352763 aij-1.2.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.385212 aij-1.2.7/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      725 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      606 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      202 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.386209 aij-1.2.7/src/animation/
+-rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.7/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.388205 aij-1.2.7/src/chat/
+-rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.7/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.391201 aij-1.2.7/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.7/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.394210 aij-1.2.7/src/emotion/
+-rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.7/src/emotion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.395791 aij-1.2.7/src/entity/
+-rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.7/src/entity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.397754 aij-1.2.7/src/face/
+-rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.7/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.398745 aij-1.2.7/src/fake/
+-rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.7/src/fake/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.400741 aij-1.2.7/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.7/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.402743 aij-1.2.7/src/keyboard/
+-rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.7/src/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.404754 aij-1.2.7/src/knowledge/
+-rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.7/src/knowledge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.405751 aij-1.2.7/src/language/
+-rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.7/src/language/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.407214 aij-1.2.7/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.7/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.409219 aij-1.2.7/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.7/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.411216 aij-1.2.7/src/objectron/
+-rw-rw-rw-   0        0        0     1992 2023-05-29 14:03:52.000000 aij-1.2.7/src/objectron/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.412216 aij-1.2.7/src/scrape/
+-rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.7/src/scrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.414689 aij-1.2.7/src/selfie/
+-rw-rw-rw-   0        0        0     3671 2023-05-29 14:00:41.000000 aij-1.2.7/src/selfie/__ini__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.416697 aij-1.2.7/src/sentiment/
+-rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.7/src/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.420309 aij-1.2.7/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.7/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.421313 aij-1.2.7/src/stream/
+-rw-rw-rw-   0        0        0     1976 2023-05-29 00:10:40.000000 aij-1.2.7/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.423315 aij-1.2.7/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.7/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.424316 aij-1.2.7/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.7/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.426841 aij-1.2.7/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.7/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.428871 aij-1.2.7/src/volume/
+-rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.7/src/volume/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.430878 aij-1.2.7/src/webcam/
+-rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.7/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.431878 aij-1.2.7/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.7/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.433875 aij-1.2.7/src/webcam3/
+-rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.7/src/webcam3/__init__.py
```

### Comparing `aij-1.2.6/LICENSE.txt` & `aij-1.2.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/PKG-INFO` & `aij-1.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.6
+Version: 1.2.7
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.6/README.md` & `aij-1.2.7/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/pyproject.toml` & `aij-1.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.2.6"
+version = "1.2.7"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-1.2.6/src/aij.egg-info/PKG-INFO` & `aij-1.2.7/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.6
+Version: 1.2.7
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.6/src/aij.egg-info/SOURCES.txt` & `aij-1.2.7/src/aij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/aij.egg-info/entry_points.txt` & `aij-1.2.7/src/aij.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/aij.egg-info/requires.txt` & `aij-1.2.7/src/aij.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/animation/__init__.py` & `aij-1.2.7/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/chat/__init__.py` & `aij-1.2.7/src/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/download/__init__.py` & `aij-1.2.7/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/emotion/__init__.py` & `aij-1.2.7/src/emotion/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/entity/__init__.py` & `aij-1.2.7/src/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/face/__init__.py` & `aij-1.2.7/src/face/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/fake/__init__.py` & `aij-1.2.7/src/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/intro/__init__.py` & `aij-1.2.7/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/keyboard/__init__.py` & `aij-1.2.7/src/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/knowledge/__init__.py` & `aij-1.2.7/src/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/messaging/__init__.py` & `aij-1.2.7/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/news/__init__.py` & `aij-1.2.7/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/objectron/__init__.py` & `aij-1.2.7/src/objectron/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 import cv2
 import mediapipe as mp
 
 mp_drawing = mp.solutions.drawing_utils
 mp_objectron = mp.solutions.objectron
 
-# For webcam input:
-cap = cv2.VideoCapture(0)
+def main():
 
-with mp_objectron.Objectron(static_image_mode=False,
-                            max_num_objects=5,
-                            min_detection_confidence=0.5,
-                            min_tracking_confidence=0.75,
-                            model_name='Cup') as objectron:
-    while cap.isOpened():
-        success, image = cap.read()
-        if not success:
-            print("Ignoring empty camera frame.")
-            # If loading a video, use 'break' instead of 'continue'.
-            continue
-
-        # To improve performance, optionally mark the image as not writeable to
-        # pass by reference.
-        image.flags.writeable = False
-        image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-        results = objectron.process(image)
-
-        # Draw the box landmarks on the image.
-        image.flags.writeable = True
-        image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
-        if results.detected_objects:
-            for detected_object in results.detected_objects:
-                mp_drawing.draw_landmarks(
-                    image, detected_object.landmarks_2d, mp_objectron.BOX_CONNECTIONS)
-                mp_drawing.draw_axis(image, detected_object.rotation,
-                                    detected_object.translation)
-        # Flip the image horizontally for a selfie-view display.
-        cv2.imshow('Objectron', cv2.flip(image, 1))
+    # For webcam input:
+    cap = cv2.VideoCapture(0)
 
+    with mp_objectron.Objectron(static_image_mode=False,
+                                max_num_objects=5,
+                                min_detection_confidence=0.5,
+                                min_tracking_confidence=0.75,
+                                model_name='Cup') as objectron:
+        while cap.isOpened():
+            success, image = cap.read()
+            if not success:
+                print("Ignoring empty camera frame.")
+                # If loading a video, use 'break' instead of 'continue'.
+                continue
+
+            # To improve performance, optionally mark the image as not writeable to
+            # pass by reference.
+            image.flags.writeable = False
+            image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+            results = objectron.process(image)
+
+            # Draw the box landmarks on the image.
+            image.flags.writeable = True
+            image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
+            if results.detected_objects:
+                for detected_object in results.detected_objects:
+                    mp_drawing.draw_landmarks(
+                        image, detected_object.landmarks_2d, mp_objectron.BOX_CONNECTIONS)
+                    mp_drawing.draw_axis(image, detected_object.rotation,
+                                        detected_object.translation)
+            # Flip the image horizontally for a selfie-view display.
+            cv2.imshow('Objectron', cv2.flip(image, 1))
+
+            
+            # if escape or q is pressed, break the loop
+            if (cv2.waitKey(5) & 0xFF == 27) or (cv2.waitKey(5) & 0xFF == ord('q')):
+                break
         
-        # if escape or q is pressed, break the loop
-        if (cv2.waitKey(5) & 0xFF == 27) or (cv2.waitKey(5) & 0xFF == ord('q')):
-            break
-    
 
-cap.release()
-cv2.destroyAllWindows()
+    cap.release()
+    cv2.destroyAllWindows()
+    
+    
+if __name__ == '__main__':
+    main()
```

### Comparing `aij-1.2.6/src/scrape/__init__.py` & `aij-1.2.7/src/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/selfie/__ini__.py` & `aij-1.2.7/src/selfie/__ini__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/sentiment/__init__.py` & `aij-1.2.7/src/sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/setup/__init__.py` & `aij-1.2.7/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/stream/__init__.py` & `aij-1.2.7/src/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/transcribe/__init__.py` & `aij-1.2.7/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/translate/__init__.py` & `aij-1.2.7/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/voice/__init__.py` & `aij-1.2.7/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/volume/__init__.py` & `aij-1.2.7/src/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/webcam/__init__.py` & `aij-1.2.7/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/webcam2/__init__.py` & `aij-1.2.7/src/webcam2/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.6/src/webcam3/__init__.py` & `aij-1.2.7/src/webcam3/__init__.py`

 * *Files identical despite different names*


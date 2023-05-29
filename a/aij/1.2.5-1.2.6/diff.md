# Comparing `tmp/aij-1.2.5.tar.gz` & `tmp/aij-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.2.5.tar", last modified: Mon May 29 00:10:56 2023, max compression
+gzip compressed data, was "aij-1.2.6.tar", last modified: Mon May 29 14:01:01 2023, max compression
```

## Comparing `aij-1.2.5.tar` & `aij-1.2.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.312939 aij-1.2.5/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.5/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-29 00:10:56.311939 aij-1.2.5/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.5/README.md
--rw-rw-rw-   0        0        0     7696 2023-05-29 00:10:47.000000 aij-1.2.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 00:10:56.313940 aij-1.2.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.238120 aij-1.2.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.270501 aij-1.2.5/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      841 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      725 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      606 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      202 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.272235 aij-1.2.5/src/animation/
--rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.5/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.273304 aij-1.2.5/src/chat/
--rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.5/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.274918 aij-1.2.5/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.5/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.275990 aij-1.2.5/src/emotion/
--rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.5/src/emotion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.278234 aij-1.2.5/src/entity/
--rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.5/src/entity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.279955 aij-1.2.5/src/face/
--rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.5/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.281566 aij-1.2.5/src/fake/
--rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.5/src/fake/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.282666 aij-1.2.5/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.5/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.283674 aij-1.2.5/src/keyboard/
--rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.5/src/keyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.284677 aij-1.2.5/src/knowledge/
--rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.5/src/knowledge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.286186 aij-1.2.5/src/language/
--rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.5/src/language/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.288726 aij-1.2.5/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.5/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.289726 aij-1.2.5/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.5/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.291724 aij-1.2.5/src/objectron/
--rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.2.5/src/objectron/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.292723 aij-1.2.5/src/scrape/
--rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.5/src/scrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.295553 aij-1.2.5/src/selfie/
--rw-rw-rw-   0        0        0     3329 2023-05-27 23:20:20.000000 aij-1.2.5/src/selfie/__ini__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.297788 aij-1.2.5/src/sentiment/
--rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.5/src/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.299435 aij-1.2.5/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.5/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.300516 aij-1.2.5/src/stream/
--rw-rw-rw-   0        0        0     1976 2023-05-29 00:10:40.000000 aij-1.2.5/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.302119 aij-1.2.5/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.5/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.303187 aij-1.2.5/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.5/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.304791 aij-1.2.5/src/voice/
--rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.5/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.305858 aij-1.2.5/src/volume/
--rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.5/src/volume/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.306927 aij-1.2.5/src/webcam/
--rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.5/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.308937 aij-1.2.5/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.5/src/webcam2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.309938 aij-1.2.5/src/webcam3/
--rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.5/src/webcam3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.806507 aij-1.2.6/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.6/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-29 14:01:01.805505 aij-1.2.6/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.6/README.md
+-rw-rw-rw-   0        0        0     7696 2023-05-29 14:00:47.000000 aij-1.2.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 14:01:01.806507 aij-1.2.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.700782 aij-1.2.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.743841 aij-1.2.6/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      725 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      606 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      202 2023-05-29 14:01:01.000000 aij-1.2.6/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.745844 aij-1.2.6/src/animation/
+-rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.6/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.748844 aij-1.2.6/src/chat/
+-rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.6/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.750354 aij-1.2.6/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.6/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.752370 aij-1.2.6/src/emotion/
+-rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.6/src/emotion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.755375 aij-1.2.6/src/entity/
+-rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.6/src/entity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.758378 aij-1.2.6/src/face/
+-rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.6/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.760914 aij-1.2.6/src/fake/
+-rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.6/src/fake/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.762940 aij-1.2.6/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.6/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.766937 aij-1.2.6/src/keyboard/
+-rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.6/src/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.767935 aij-1.2.6/src/knowledge/
+-rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.6/src/knowledge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.769938 aij-1.2.6/src/language/
+-rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.6/src/language/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.771950 aij-1.2.6/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.6/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.773944 aij-1.2.6/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.6/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.775638 aij-1.2.6/src/objectron/
+-rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.2.6/src/objectron/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.777165 aij-1.2.6/src/scrape/
+-rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.6/src/scrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.779725 aij-1.2.6/src/selfie/
+-rw-rw-rw-   0        0        0     3671 2023-05-29 14:00:41.000000 aij-1.2.6/src/selfie/__ini__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.781871 aij-1.2.6/src/sentiment/
+-rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.6/src/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.783845 aij-1.2.6/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.6/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.784850 aij-1.2.6/src/stream/
+-rw-rw-rw-   0        0        0     1976 2023-05-29 00:10:40.000000 aij-1.2.6/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.788397 aij-1.2.6/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.6/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.790938 aij-1.2.6/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.6/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.792939 aij-1.2.6/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.6/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.796481 aij-1.2.6/src/volume/
+-rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.6/src/volume/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.799507 aij-1.2.6/src/webcam/
+-rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.6/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.801506 aij-1.2.6/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.6/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:01:01.803505 aij-1.2.6/src/webcam3/
+-rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.6/src/webcam3/__init__.py
```

### Comparing `aij-1.2.5/LICENSE.txt` & `aij-1.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/PKG-INFO` & `aij-1.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.5
+Version: 1.2.6
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.5/README.md` & `aij-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/pyproject.toml` & `aij-1.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.2.5"
+version = "1.2.6"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-1.2.5/src/aij.egg-info/PKG-INFO` & `aij-1.2.6/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.5
+Version: 1.2.6
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.5/src/aij.egg-info/SOURCES.txt` & `aij-1.2.6/src/aij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/aij.egg-info/entry_points.txt` & `aij-1.2.6/src/aij.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/aij.egg-info/requires.txt` & `aij-1.2.6/src/aij.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/animation/__init__.py` & `aij-1.2.6/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/chat/__init__.py` & `aij-1.2.6/src/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/download/__init__.py` & `aij-1.2.6/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/emotion/__init__.py` & `aij-1.2.6/src/emotion/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/entity/__init__.py` & `aij-1.2.6/src/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/face/__init__.py` & `aij-1.2.6/src/face/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/fake/__init__.py` & `aij-1.2.6/src/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/intro/__init__.py` & `aij-1.2.6/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/keyboard/__init__.py` & `aij-1.2.6/src/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/knowledge/__init__.py` & `aij-1.2.6/src/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/messaging/__init__.py` & `aij-1.2.6/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/news/__init__.py` & `aij-1.2.6/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/objectron/__init__.py` & `aij-1.2.6/src/objectron/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/scrape/__init__.py` & `aij-1.2.6/src/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/selfie/__ini__.py` & `aij-1.2.6/src/selfie/__ini__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,77 +1,83 @@
 import cv2
 import mediapipe as mp
 import numpy as np
 
 mp_drawing = mp.solutions.drawing_utils
 mp_selfie_segmentation = mp.solutions.selfie_segmentation
 
-# For static images:
-IMAGE_FILES = []
-BG_COLOR = (192, 192, 192)  # gray
-MASK_COLOR = (255, 255, 255)  # white
-with mp_selfie_segmentation.SelfieSegmentation(
-        model_selection=0) as selfie_segmentation:
-    for idx, file in enumerate(IMAGE_FILES):
-        image = cv2.imread(file)
-        image_height, image_width, _ = image.shape
-        # Convert the BGR image to RGB before processing.
-        results = selfie_segmentation.process(
-            cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
-
-        # Draw selfie segmentation on the background image.
-        # To improve segmentation around boundaries, consider applying a joint
-        # bilateral filter to "results.segmentation_mask" with "image".
-        condition = np.stack((results.segmentation_mask,) * 3, axis=-1) > 0.1
-        # Generate solid color images for showing the output selfie segmentation mask.
-        fg_image = np.zeros(image.shape, dtype=np.uint8)
-        fg_image[:] = MASK_COLOR
-        bg_image = np.zeros(image.shape, dtype=np.uint8)
-        bg_image[:] = BG_COLOR
-        output_image = np.where(condition, fg_image, bg_image)
-        cv2.imwrite('/tmp/selfie_segmentation_output' +
-                    str(idx) + '.png', output_image)
-
-# For webcam input:
-BG_COLOR = (192, 192, 192)  # gray
-cap = cv2.VideoCapture(0)
-with mp_selfie_segmentation.SelfieSegmentation(
-        model_selection=1) as selfie_segmentation:
-    bg_image = None
-    while cap.isOpened():
-        success, image = cap.read()
-        if not success:
-            print("Ignoring empty camera frame.")
-            # If loading a video, use 'break' instead of 'continue'.
-            continue
-
-        # Flip the image horizontally for a later selfie-view display, and convert
-        # the BGR image to RGB.
-        image = cv2.cvtColor(cv2.flip(image, 1), cv2.COLOR_BGR2RGB)
-        # To improve performance, optionally mark the image as not writeable to
-        # pass by reference.
-        image.flags.writeable = False
-        results = selfie_segmentation.process(image)
-
-        image.flags.writeable = True
-        image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
-
-        # Draw selfie segmentation on the background image.
-        # To improve segmentation around boundaries, consider applying a joint
-        # bilateral filter to "results.segmentation_mask" with "image".
-        condition = np.stack(
-            (results.segmentation_mask,) * 3, axis=-1) > 0.1
-        # The background can be customized.
-        #   a) Load an image (with the same width and height of the input image) to
-        #      be the background, e.g., bg_image = cv2.imread('/path/to/image/file')
-        #   b) Blur the input image by applying image filtering, e.g.,
-        #      bg_image = cv2.GaussianBlur(image,(55,55),0)
-        if bg_image is None:
+def main():
+
+    # For static images:
+    IMAGE_FILES = []
+    BG_COLOR = (192, 192, 192)  # gray
+    MASK_COLOR = (255, 255, 255)  # white
+    with mp_selfie_segmentation.SelfieSegmentation(
+            model_selection=0) as selfie_segmentation:
+        for idx, file in enumerate(IMAGE_FILES):
+            image = cv2.imread(file)
+            image_height, image_width, _ = image.shape
+            # Convert the BGR image to RGB before processing.
+            results = selfie_segmentation.process(
+                cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
+
+            # Draw selfie segmentation on the background image.
+            # To improve segmentation around boundaries, consider applying a joint
+            # bilateral filter to "results.segmentation_mask" with "image".
+            condition = np.stack((results.segmentation_mask,) * 3, axis=-1) > 0.1
+            # Generate solid color images for showing the output selfie segmentation mask.
+            fg_image = np.zeros(image.shape, dtype=np.uint8)
+            fg_image[:] = MASK_COLOR
             bg_image = np.zeros(image.shape, dtype=np.uint8)
             bg_image[:] = BG_COLOR
-        output_image = np.where(condition, image, bg_image)
-
-        cv2.imshow('MediaPipe Selfie Segmentation', output_image)
-        if cv2.waitKey(5) & 0xFF == 27:
-            break
-
-cap.release()
+            output_image = np.where(condition, fg_image, bg_image)
+            cv2.imwrite('/tmp/selfie_segmentation_output' +
+                        str(idx) + '.png', output_image)
+
+    # For webcam input:
+    BG_COLOR = (192, 192, 192)  # gray
+    cap = cv2.VideoCapture(0)
+    with mp_selfie_segmentation.SelfieSegmentation(
+            model_selection=1) as selfie_segmentation:
+        bg_image = None
+        while cap.isOpened():
+            success, image = cap.read()
+            if not success:
+                print("Ignoring empty camera frame.")
+                # If loading a video, use 'break' instead of 'continue'.
+                continue
+
+            # Flip the image horizontally for a later selfie-view display, and convert
+            # the BGR image to RGB.
+            image = cv2.cvtColor(cv2.flip(image, 1), cv2.COLOR_BGR2RGB)
+            # To improve performance, optionally mark the image as not writeable to
+            # pass by reference.
+            image.flags.writeable = False
+            results = selfie_segmentation.process(image)
+
+            image.flags.writeable = True
+            image = cv2.cvtColor(image, cv2.COLOR_RGB2BGR)
+
+            # Draw selfie segmentation on the background image.
+            # To improve segmentation around boundaries, consider applying a joint
+            # bilateral filter to "results.segmentation_mask" with "image".
+            condition = np.stack(
+                (results.segmentation_mask,) * 3, axis=-1) > 0.1
+            # The background can be customized.
+            #   a) Load an image (with the same width and height of the input image) to
+            #      be the background, e.g., bg_image = cv2.imread('/path/to/image/file')
+            #   b) Blur the input image by applying image filtering, e.g.,
+            #      bg_image = cv2.GaussianBlur(image,(55,55),0)
+            if bg_image is None:
+                bg_image = np.zeros(image.shape, dtype=np.uint8)
+                bg_image[:] = BG_COLOR
+            output_image = np.where(condition, image, bg_image)
+
+            cv2.imshow('MediaPipe Selfie Segmentation', output_image)
+            if cv2.waitKey(5) & 0xFF == 27:
+                break
+
+    cap.release()
+    cv2.destroyAllWindows()
+    
+if __name__ == '__main__':
+    main()
```

### Comparing `aij-1.2.5/src/sentiment/__init__.py` & `aij-1.2.6/src/sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/setup/__init__.py` & `aij-1.2.6/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/stream/__init__.py` & `aij-1.2.6/src/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/transcribe/__init__.py` & `aij-1.2.6/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/translate/__init__.py` & `aij-1.2.6/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/voice/__init__.py` & `aij-1.2.6/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/volume/__init__.py` & `aij-1.2.6/src/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/webcam/__init__.py` & `aij-1.2.6/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/webcam2/__init__.py` & `aij-1.2.6/src/webcam2/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.5/src/webcam3/__init__.py` & `aij-1.2.6/src/webcam3/__init__.py`

 * *Files identical despite different names*


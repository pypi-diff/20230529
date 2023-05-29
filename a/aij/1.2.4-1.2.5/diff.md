# Comparing `tmp/aij-1.2.4.tar.gz` & `tmp/aij-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.2.4.tar", last modified: Mon May 29 00:07:34 2023, max compression
+gzip compressed data, was "aij-1.2.5.tar", last modified: Mon May 29 00:10:56 2023, max compression
```

## Comparing `aij-1.2.4.tar` & `aij-1.2.5.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.791816 aij-1.2.4/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.4/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-29 00:07:34.791816 aij-1.2.4/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.4/README.md
--rw-rw-rw-   0        0        0     7696 2023-05-29 00:07:25.000000 aij-1.2.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 00:07:34.792816 aij-1.2.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.717716 aij-1.2.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.751424 aij-1.2.4/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      841 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      725 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      606 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      202 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.752932 aij-1.2.4/src/animation/
--rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.4/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.754948 aij-1.2.4/src/chat/
--rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.4/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.755954 aij-1.2.4/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.4/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.757477 aij-1.2.4/src/emotion/
--rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.4/src/emotion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.759006 aij-1.2.4/src/entity/
--rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.4/src/entity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.760186 aij-1.2.4/src/face/
--rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.4/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.761202 aij-1.2.4/src/fake/
--rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.4/src/fake/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.762203 aij-1.2.4/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.4/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.763718 aij-1.2.4/src/keyboard/
--rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.4/src/keyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.765735 aij-1.2.4/src/knowledge/
--rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.4/src/knowledge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.768403 aij-1.2.4/src/language/
--rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.4/src/language/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.769418 aij-1.2.4/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.4/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.771415 aij-1.2.4/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.4/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.772419 aij-1.2.4/src/objectron/
--rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.2.4/src/objectron/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.773415 aij-1.2.4/src/scrape/
--rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.4/src/scrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.775740 aij-1.2.4/src/selfie/
--rw-rw-rw-   0        0        0     3329 2023-05-27 23:20:20.000000 aij-1.2.4/src/selfie/__ini__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.776737 aij-1.2.4/src/sentiment/
--rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.4/src/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.777737 aij-1.2.4/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.4/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.778494 aij-1.2.4/src/stream/
--rw-rw-rw-   0        0        0     1265 2023-05-29 00:07:15.000000 aij-1.2.4/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.779675 aij-1.2.4/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.4/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.781694 aij-1.2.4/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.4/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.784207 aij-1.2.4/src/voice/
--rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.4/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.785227 aij-1.2.4/src/volume/
--rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.4/src/volume/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.786234 aij-1.2.4/src/webcam/
--rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.4/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.788763 aij-1.2.4/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.4/src/webcam2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.789820 aij-1.2.4/src/webcam3/
--rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.4/src/webcam3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.312939 aij-1.2.5/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.5/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-29 00:10:56.311939 aij-1.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.5/README.md
+-rw-rw-rw-   0        0        0     7696 2023-05-29 00:10:47.000000 aij-1.2.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 00:10:56.313940 aij-1.2.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.238120 aij-1.2.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.270501 aij-1.2.5/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      725 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      606 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      202 2023-05-29 00:10:56.000000 aij-1.2.5/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.272235 aij-1.2.5/src/animation/
+-rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.5/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.273304 aij-1.2.5/src/chat/
+-rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.5/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.274918 aij-1.2.5/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.5/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.275990 aij-1.2.5/src/emotion/
+-rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.5/src/emotion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.278234 aij-1.2.5/src/entity/
+-rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.5/src/entity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.279955 aij-1.2.5/src/face/
+-rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.5/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.281566 aij-1.2.5/src/fake/
+-rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.5/src/fake/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.282666 aij-1.2.5/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.5/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.283674 aij-1.2.5/src/keyboard/
+-rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.5/src/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.284677 aij-1.2.5/src/knowledge/
+-rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.5/src/knowledge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.286186 aij-1.2.5/src/language/
+-rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.5/src/language/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.288726 aij-1.2.5/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.5/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.289726 aij-1.2.5/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.5/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.291724 aij-1.2.5/src/objectron/
+-rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.2.5/src/objectron/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.292723 aij-1.2.5/src/scrape/
+-rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.5/src/scrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.295553 aij-1.2.5/src/selfie/
+-rw-rw-rw-   0        0        0     3329 2023-05-27 23:20:20.000000 aij-1.2.5/src/selfie/__ini__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.297788 aij-1.2.5/src/sentiment/
+-rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.5/src/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.299435 aij-1.2.5/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.5/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.300516 aij-1.2.5/src/stream/
+-rw-rw-rw-   0        0        0     1976 2023-05-29 00:10:40.000000 aij-1.2.5/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.302119 aij-1.2.5/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.5/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.303187 aij-1.2.5/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.5/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.304791 aij-1.2.5/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.5/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.305858 aij-1.2.5/src/volume/
+-rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.5/src/volume/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.306927 aij-1.2.5/src/webcam/
+-rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.5/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.308937 aij-1.2.5/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.5/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:10:56.309938 aij-1.2.5/src/webcam3/
+-rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.5/src/webcam3/__init__.py
```

### Comparing `aij-1.2.4/LICENSE.txt` & `aij-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/PKG-INFO` & `aij-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.4
+Version: 1.2.5
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.4/README.md` & `aij-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/pyproject.toml` & `aij-1.2.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.2.4"
+version = "1.2.5"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-1.2.4/src/aij.egg-info/PKG-INFO` & `aij-1.2.5/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.4
+Version: 1.2.5
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.4/src/aij.egg-info/SOURCES.txt` & `aij-1.2.5/src/aij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/aij.egg-info/entry_points.txt` & `aij-1.2.5/src/aij.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/aij.egg-info/requires.txt` & `aij-1.2.5/src/aij.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/animation/__init__.py` & `aij-1.2.5/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/chat/__init__.py` & `aij-1.2.5/src/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/download/__init__.py` & `aij-1.2.5/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/emotion/__init__.py` & `aij-1.2.5/src/emotion/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/entity/__init__.py` & `aij-1.2.5/src/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/face/__init__.py` & `aij-1.2.5/src/face/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/fake/__init__.py` & `aij-1.2.5/src/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/intro/__init__.py` & `aij-1.2.5/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/keyboard/__init__.py` & `aij-1.2.5/src/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/knowledge/__init__.py` & `aij-1.2.5/src/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/messaging/__init__.py` & `aij-1.2.5/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/news/__init__.py` & `aij-1.2.5/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/objectron/__init__.py` & `aij-1.2.5/src/objectron/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/scrape/__init__.py` & `aij-1.2.5/src/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/selfie/__ini__.py` & `aij-1.2.5/src/selfie/__ini__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/sentiment/__init__.py` & `aij-1.2.5/src/sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/setup/__init__.py` & `aij-1.2.5/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/transcribe/__init__.py` & `aij-1.2.5/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/translate/__init__.py` & `aij-1.2.5/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/voice/__init__.py` & `aij-1.2.5/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/volume/__init__.py` & `aij-1.2.5/src/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/webcam/__init__.py` & `aij-1.2.5/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/webcam2/__init__.py` & `aij-1.2.5/src/webcam2/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.4/src/webcam3/__init__.py` & `aij-1.2.5/src/webcam3/__init__.py`

 * *Files identical despite different names*


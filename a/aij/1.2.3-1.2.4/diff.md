# Comparing `tmp/aij-1.2.3.tar.gz` & `tmp/aij-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.2.3.tar", last modified: Mon May 29 00:04:49 2023, max compression
+gzip compressed data, was "aij-1.2.4.tar", last modified: Mon May 29 00:07:34 2023, max compression
```

## Comparing `aij-1.2.3.tar` & `aij-1.2.4.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.357831 aij-1.2.3/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.3/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-29 00:04:49.356318 aij-1.2.3/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.3/README.md
--rw-rw-rw-   0        0        0     7696 2023-05-29 00:04:40.000000 aij-1.2.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 00:04:49.358356 aij-1.2.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.278345 aij-1.2.3/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.317675 aij-1.2.3/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-29 00:04:49.000000 aij-1.2.3/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      841 2023-05-29 00:04:49.000000 aij-1.2.3/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 00:04:49.000000 aij-1.2.3/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      725 2023-05-29 00:04:49.000000 aij-1.2.3/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      606 2023-05-29 00:04:49.000000 aij-1.2.3/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      202 2023-05-29 00:04:49.000000 aij-1.2.3/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.319898 aij-1.2.3/src/animation/
--rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.3/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.321422 aij-1.2.3/src/chat/
--rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.3/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.322930 aij-1.2.3/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.3/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.323941 aij-1.2.3/src/emotion/
--rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.3/src/emotion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.324941 aij-1.2.3/src/entity/
--rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.3/src/entity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.325940 aij-1.2.3/src/face/
--rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.3/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.327449 aij-1.2.3/src/fake/
--rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.3/src/fake/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.328460 aij-1.2.3/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.3/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.330720 aij-1.2.3/src/keyboard/
--rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.3/src/keyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.331723 aij-1.2.3/src/knowledge/
--rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.3/src/knowledge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.334052 aij-1.2.3/src/language/
--rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.3/src/language/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.336048 aij-1.2.3/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.3/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.336048 aij-1.2.3/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.3/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.339082 aij-1.2.3/src/objectron/
--rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.2.3/src/objectron/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.340894 aij-1.2.3/src/scrape/
--rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.3/src/scrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.341401 aij-1.2.3/src/selfie/
--rw-rw-rw-   0        0        0     3329 2023-05-27 23:20:20.000000 aij-1.2.3/src/selfie/__ini__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.343241 aij-1.2.3/src/sentiment/
--rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.3/src/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.344265 aij-1.2.3/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.3/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.345266 aij-1.2.3/src/stream/
--rw-rw-rw-   0        0        0     1174 2023-05-29 00:04:34.000000 aij-1.2.3/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.346265 aij-1.2.3/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.3/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.347777 aij-1.2.3/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.3/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.349302 aij-1.2.3/src/voice/
--rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.3/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.351311 aij-1.2.3/src/volume/
--rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.3/src/volume/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.352318 aij-1.2.3/src/webcam/
--rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.3/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.353319 aij-1.2.3/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.3/src/webcam2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:04:49.355314 aij-1.2.3/src/webcam3/
--rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.3/src/webcam3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.791816 aij-1.2.4/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.4/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-29 00:07:34.791816 aij-1.2.4/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.4/README.md
+-rw-rw-rw-   0        0        0     7696 2023-05-29 00:07:25.000000 aij-1.2.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 00:07:34.792816 aij-1.2.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.717716 aij-1.2.4/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.751424 aij-1.2.4/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      725 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      606 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      202 2023-05-29 00:07:34.000000 aij-1.2.4/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.752932 aij-1.2.4/src/animation/
+-rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.4/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.754948 aij-1.2.4/src/chat/
+-rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.4/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.755954 aij-1.2.4/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.4/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.757477 aij-1.2.4/src/emotion/
+-rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.4/src/emotion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.759006 aij-1.2.4/src/entity/
+-rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.4/src/entity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.760186 aij-1.2.4/src/face/
+-rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.4/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.761202 aij-1.2.4/src/fake/
+-rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.4/src/fake/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.762203 aij-1.2.4/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.4/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.763718 aij-1.2.4/src/keyboard/
+-rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.4/src/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.765735 aij-1.2.4/src/knowledge/
+-rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.4/src/knowledge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.768403 aij-1.2.4/src/language/
+-rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.4/src/language/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.769418 aij-1.2.4/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.4/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.771415 aij-1.2.4/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.4/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.772419 aij-1.2.4/src/objectron/
+-rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.2.4/src/objectron/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.773415 aij-1.2.4/src/scrape/
+-rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.4/src/scrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.775740 aij-1.2.4/src/selfie/
+-rw-rw-rw-   0        0        0     3329 2023-05-27 23:20:20.000000 aij-1.2.4/src/selfie/__ini__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.776737 aij-1.2.4/src/sentiment/
+-rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.4/src/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.777737 aij-1.2.4/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.4/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.778494 aij-1.2.4/src/stream/
+-rw-rw-rw-   0        0        0     1265 2023-05-29 00:07:15.000000 aij-1.2.4/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.779675 aij-1.2.4/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.4/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.781694 aij-1.2.4/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.4/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.784207 aij-1.2.4/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.4/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.785227 aij-1.2.4/src/volume/
+-rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.4/src/volume/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.786234 aij-1.2.4/src/webcam/
+-rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.4/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.788763 aij-1.2.4/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.4/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:07:34.789820 aij-1.2.4/src/webcam3/
+-rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.4/src/webcam3/__init__.py
```

### Comparing `aij-1.2.3/LICENSE.txt` & `aij-1.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/PKG-INFO` & `aij-1.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.3
+Version: 1.2.4
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.3/README.md` & `aij-1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/pyproject.toml` & `aij-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.2.3"
+version = "1.2.4"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-1.2.3/src/aij.egg-info/PKG-INFO` & `aij-1.2.4/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.3
+Version: 1.2.4
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.3/src/aij.egg-info/SOURCES.txt` & `aij-1.2.4/src/aij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/aij.egg-info/entry_points.txt` & `aij-1.2.4/src/aij.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/aij.egg-info/requires.txt` & `aij-1.2.4/src/aij.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/animation/__init__.py` & `aij-1.2.4/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/chat/__init__.py` & `aij-1.2.4/src/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/download/__init__.py` & `aij-1.2.4/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/emotion/__init__.py` & `aij-1.2.4/src/emotion/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/entity/__init__.py` & `aij-1.2.4/src/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/face/__init__.py` & `aij-1.2.4/src/face/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/fake/__init__.py` & `aij-1.2.4/src/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/intro/__init__.py` & `aij-1.2.4/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/keyboard/__init__.py` & `aij-1.2.4/src/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/knowledge/__init__.py` & `aij-1.2.4/src/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/messaging/__init__.py` & `aij-1.2.4/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/news/__init__.py` & `aij-1.2.4/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/objectron/__init__.py` & `aij-1.2.4/src/objectron/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/scrape/__init__.py` & `aij-1.2.4/src/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/selfie/__ini__.py` & `aij-1.2.4/src/selfie/__ini__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/sentiment/__init__.py` & `aij-1.2.4/src/sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/setup/__init__.py` & `aij-1.2.4/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/stream/__init__.py` & `aij-1.2.4/src/stream/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -26,15 +26,17 @@
     # Video streaming route. Put this in the src attribute of an img tag
     return Response(gen_frames(), mimetype='multipart/x-mixed-replace; boundary=frame')
 
 
 @app.route('/')
 def index():
     """Video streaming home page."""
-    return render_template('index.html')
+    return render_template(
+        "https://raw.githubusercontent.com/codesapienbe/aij/main/src/stream/templates/index.html"
+    )
 
 def main():
     app.run(
         host='localhost', 
         port=8080,
         debug=True
     )
```

### Comparing `aij-1.2.3/src/transcribe/__init__.py` & `aij-1.2.4/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/translate/__init__.py` & `aij-1.2.4/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/voice/__init__.py` & `aij-1.2.4/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/volume/__init__.py` & `aij-1.2.4/src/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/webcam/__init__.py` & `aij-1.2.4/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/webcam2/__init__.py` & `aij-1.2.4/src/webcam2/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.3/src/webcam3/__init__.py` & `aij-1.2.4/src/webcam3/__init__.py`

 * *Files identical despite different names*


# Comparing `tmp/aij-1.1.5.tar.gz` & `tmp/aij-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.1.5.tar", last modified: Sat May 27 23:40:45 2023, max compression
+gzip compressed data, was "aij-1.2.0.tar", last modified: Sun May 28 23:35:44 2023, max compression
```

## Comparing `aij-1.1.5.tar` & `aij-1.2.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.445083 aij-1.1.5/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.1.5/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-27 23:40:45.444081 aij-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.1.5/README.md
--rw-rw-rw-   0        0        0     7185 2023-05-27 23:40:32.000000 aij-1.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 23:40:45.445083 aij-1.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.370756 aij-1.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.403757 aij-1.1.5/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      842 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      247 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      606 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      203 2023-05-27 23:40:45.000000 aij-1.1.5/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.404754 aij-1.1.5/src/animation/
--rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.1.5/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.406756 aij-1.1.5/src/category/
--rw-rw-rw-   0        0        0     6518 2023-05-27 23:18:50.000000 aij-1.1.5/src/category/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.407754 aij-1.1.5/src/chat/
--rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.1.5/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.408755 aij-1.1.5/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.1.5/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.410752 aij-1.1.5/src/emotion/
--rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.1.5/src/emotion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.411756 aij-1.1.5/src/entity/
--rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.1.5/src/entity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.413756 aij-1.1.5/src/face/
--rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.1.5/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.414757 aij-1.1.5/src/fake/
--rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.1.5/src/fake/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.415754 aij-1.1.5/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.1.5/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.417756 aij-1.1.5/src/keyboard/
--rw-rw-rw-   0        0        0     6518 2023-05-27 23:12:06.000000 aij-1.1.5/src/keyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.418754 aij-1.1.5/src/knowledge/
--rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.1.5/src/knowledge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.420754 aij-1.1.5/src/language/
--rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.1.5/src/language/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.421754 aij-1.1.5/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.1.5/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.423756 aij-1.1.5/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.1.5/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.424754 aij-1.1.5/src/objectron/
--rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.1.5/src/objectron/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.426751 aij-1.1.5/src/scrape/
--rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.1.5/src/scrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.428786 aij-1.1.5/src/selfie/
--rw-rw-rw-   0        0        0     3329 2023-05-27 23:20:20.000000 aij-1.1.5/src/selfie/__ini__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.430063 aij-1.1.5/src/sentiment/
--rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.1.5/src/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.431073 aij-1.1.5/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.1.5/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.433070 aij-1.1.5/src/stream/
--rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.1.5/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.434073 aij-1.1.5/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.1.5/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.435083 aij-1.1.5/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.1.5/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.437083 aij-1.1.5/src/voice/
--rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.1.5/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.438082 aij-1.1.5/src/volume/
--rw-rw-rw-   0        0        0     6737 2023-05-27 23:26:16.000000 aij-1.1.5/src/volume/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.440084 aij-1.1.5/src/webcam/
--rw-rw-rw-   0        0        0    18760 2023-05-26 11:58:38.000000 aij-1.1.5/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 23:40:45.441081 aij-1.1.5/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.1.5/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.365786 aij-1.2.0/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-28 23:35:44.364278 aij-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.0/README.md
+-rw-rw-rw-   0        0        0     6936 2023-05-28 23:35:31.000000 aij-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 23:35:44.365786 aij-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.286248 aij-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.318771 aij-1.2.0/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-28 23:35:44.000000 aij-1.2.0/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      832 2023-05-28 23:35:44.000000 aij-1.2.0/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:35:44.000000 aij-1.2.0/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      606 2023-05-28 23:35:44.000000 aij-1.2.0/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      211 2023-05-28 23:35:44.000000 aij-1.2.0/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.320778 aij-1.2.0/src/animation/
+-rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.0/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.321773 aij-1.2.0/src/category/
+-rw-rw-rw-   0        0        0     6518 2023-05-27 23:18:50.000000 aij-1.2.0/src/category/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.323778 aij-1.2.0/src/chat/
+-rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.0/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.325772 aij-1.2.0/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.0/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.328113 aij-1.2.0/src/emotion/
+-rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.0/src/emotion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.330323 aij-1.2.0/src/entity/
+-rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.0/src/entity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.332942 aij-1.2.0/src/face/
+-rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.0/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.333939 aij-1.2.0/src/fake/
+-rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.0/src/fake/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.335974 aij-1.2.0/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.0/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.337495 aij-1.2.0/src/keyboard/
+-rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.0/src/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.339515 aij-1.2.0/src/knowledge/
+-rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.0/src/knowledge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.341511 aij-1.2.0/src/language/
+-rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.0/src/language/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.342512 aij-1.2.0/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.0/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.344506 aij-1.2.0/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.0/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.345508 aij-1.2.0/src/objectron/
+-rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.2.0/src/objectron/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.347031 aij-1.2.0/src/scrape/
+-rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.0/src/scrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.349034 aij-1.2.0/src/selfie/
+-rw-rw-rw-   0        0        0     3329 2023-05-27 23:20:20.000000 aij-1.2.0/src/selfie/__ini__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.350030 aij-1.2.0/src/sentiment/
+-rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.0/src/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.351030 aij-1.2.0/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.0/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.352030 aij-1.2.0/src/stream/
+-rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.2.0/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.354031 aij-1.2.0/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.0/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.355544 aij-1.2.0/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.0/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.357284 aij-1.2.0/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.0/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.359284 aij-1.2.0/src/volume/
+-rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.0/src/volume/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.360279 aij-1.2.0/src/webcam/
+-rw-rw-rw-   0        0        0    18760 2023-05-26 11:58:38.000000 aij-1.2.0/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.361279 aij-1.2.0/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.0/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.363278 aij-1.2.0/src/webcam3/
+-rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.0/src/webcam3/__init__.py
```

### Comparing `aij-1.1.5/LICENSE.txt` & `aij-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/PKG-INFO` & `aij-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.1.5
+Version: 1.2.0
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.1.5/README.md` & `aij-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/pyproject.toml` & `aij-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.1.05"
+version = "1.2.0"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -184,24 +184,15 @@
 "Funding" = "https://donate.pypi.org"
 "Say Thanks!" = "http://saythanks.io/to/aij"
 "Source" = "https://github.com/codesapienbe/aij"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
-aij = "webcam:main"
-aij2 = "webcam2:main"
-aijnews = "news:main"
-aijintro = "intro:main"
-aijtranslate = "translate:main"
-aijtranscribe = "transcribe:main"
-aijchat = "chat:main"
-aijtube = "download:main"
-aijinit = "setup:main"
-aijvoice = "voice:main"
+
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = { "db" = ["*.dat"] }
```

### Comparing `aij-1.1.5/src/aij.egg-info/PKG-INFO` & `aij-1.2.0/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.1.5
+Version: 1.2.0
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.1.5/src/aij.egg-info/SOURCES.txt` & `aij-1.2.0/src/aij.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/aij.egg-info/PKG-INFO
 src/aij.egg-info/SOURCES.txt
 src/aij.egg-info/dependency_links.txt
-src/aij.egg-info/entry_points.txt
 src/aij.egg-info/requires.txt
 src/aij.egg-info/top_level.txt
 src/animation/__init__.py
 src/category/__init__.py
 src/chat/__init__.py
 src/download/__init__.py
 src/emotion/__init__.py
@@ -28,8 +27,9 @@
 src/setup/__init__.py
 src/stream/__init__.py
 src/transcribe/__init__.py
 src/translate/__init__.py
 src/voice/__init__.py
 src/volume/__init__.py
 src/webcam/__init__.py
-src/webcam2/__init__.py
+src/webcam2/__init__.py
+src/webcam3/__init__.py
```

### Comparing `aij-1.1.5/src/aij.egg-info/requires.txt` & `aij-1.2.0/src/aij.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/animation/__init__.py` & `aij-1.2.0/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/category/__init__.py` & `aij-1.2.0/src/category/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/chat/__init__.py` & `aij-1.2.0/src/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/download/__init__.py` & `aij-1.2.0/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/emotion/__init__.py` & `aij-1.2.0/src/emotion/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/entity/__init__.py` & `aij-1.2.0/src/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/face/__init__.py` & `aij-1.2.0/src/face/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/fake/__init__.py` & `aij-1.2.0/src/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/intro/__init__.py` & `aij-1.2.0/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/knowledge/__init__.py` & `aij-1.2.0/src/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/messaging/__init__.py` & `aij-1.2.0/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/news/__init__.py` & `aij-1.2.0/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/objectron/__init__.py` & `aij-1.2.0/src/objectron/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/scrape/__init__.py` & `aij-1.2.0/src/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/selfie/__ini__.py` & `aij-1.2.0/src/selfie/__ini__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/sentiment/__init__.py` & `aij-1.2.0/src/sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/setup/__init__.py` & `aij-1.2.0/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/stream/__init__.py` & `aij-1.2.0/src/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/transcribe/__init__.py` & `aij-1.2.0/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/translate/__init__.py` & `aij-1.2.0/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/voice/__init__.py` & `aij-1.2.0/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/webcam/__init__.py` & `aij-1.2.0/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.1.5/src/webcam2/__init__.py` & `aij-1.2.0/src/webcam2/__init__.py`

 * *Files identical despite different names*


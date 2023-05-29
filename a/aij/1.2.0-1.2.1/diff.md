# Comparing `tmp/aij-1.2.0.tar.gz` & `tmp/aij-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.2.0.tar", last modified: Sun May 28 23:35:44 2023, max compression
+gzip compressed data, was "aij-1.2.1.tar", last modified: Sun May 28 23:52:15 2023, max compression
```

## Comparing `aij-1.2.0.tar` & `aij-1.2.1.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.365786 aij-1.2.0/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.0/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-28 23:35:44.364278 aij-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.0/README.md
--rw-rw-rw-   0        0        0     6936 2023-05-28 23:35:31.000000 aij-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 23:35:44.365786 aij-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.286248 aij-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.318771 aij-1.2.0/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-28 23:35:44.000000 aij-1.2.0/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      832 2023-05-28 23:35:44.000000 aij-1.2.0/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 23:35:44.000000 aij-1.2.0/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      606 2023-05-28 23:35:44.000000 aij-1.2.0/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      211 2023-05-28 23:35:44.000000 aij-1.2.0/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.320778 aij-1.2.0/src/animation/
--rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.0/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.321773 aij-1.2.0/src/category/
--rw-rw-rw-   0        0        0     6518 2023-05-27 23:18:50.000000 aij-1.2.0/src/category/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.323778 aij-1.2.0/src/chat/
--rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.0/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.325772 aij-1.2.0/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.0/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.328113 aij-1.2.0/src/emotion/
--rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.0/src/emotion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.330323 aij-1.2.0/src/entity/
--rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.0/src/entity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.332942 aij-1.2.0/src/face/
--rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.0/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.333939 aij-1.2.0/src/fake/
--rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.0/src/fake/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.335974 aij-1.2.0/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.0/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.337495 aij-1.2.0/src/keyboard/
--rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.0/src/keyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.339515 aij-1.2.0/src/knowledge/
--rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.0/src/knowledge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.341511 aij-1.2.0/src/language/
--rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.0/src/language/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.342512 aij-1.2.0/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.0/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.344506 aij-1.2.0/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.0/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.345508 aij-1.2.0/src/objectron/
--rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.2.0/src/objectron/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.347031 aij-1.2.0/src/scrape/
--rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.0/src/scrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.349034 aij-1.2.0/src/selfie/
--rw-rw-rw-   0        0        0     3329 2023-05-27 23:20:20.000000 aij-1.2.0/src/selfie/__ini__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.350030 aij-1.2.0/src/sentiment/
--rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.0/src/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.351030 aij-1.2.0/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.0/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.352030 aij-1.2.0/src/stream/
--rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.2.0/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.354031 aij-1.2.0/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.0/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.355544 aij-1.2.0/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.0/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.357284 aij-1.2.0/src/voice/
--rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.0/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.359284 aij-1.2.0/src/volume/
--rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.0/src/volume/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.360279 aij-1.2.0/src/webcam/
--rw-rw-rw-   0        0        0    18760 2023-05-26 11:58:38.000000 aij-1.2.0/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.361279 aij-1.2.0/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.0/src/webcam2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:35:44.363278 aij-1.2.0/src/webcam3/
--rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.0/src/webcam3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.684040 aij-1.2.1/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.1/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-28 23:52:15.683044 aij-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.1/README.md
+-rw-rw-rw-   0        0        0     7696 2023-05-28 23:52:06.000000 aij-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-28 23:52:15.684040 aij-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.599652 aij-1.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.638184 aij-1.2.1/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-28 23:52:15.000000 aij-1.2.1/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2023-05-28 23:52:15.000000 aij-1.2.1/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:52:15.000000 aij-1.2.1/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      725 2023-05-28 23:52:15.000000 aij-1.2.1/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      606 2023-05-28 23:52:15.000000 aij-1.2.1/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      202 2023-05-28 23:52:15.000000 aij-1.2.1/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.640727 aij-1.2.1/src/animation/
+-rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.1/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.641733 aij-1.2.1/src/chat/
+-rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.1/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.643724 aij-1.2.1/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.1/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.645238 aij-1.2.1/src/emotion/
+-rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.1/src/emotion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.647250 aij-1.2.1/src/entity/
+-rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.1/src/entity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.649255 aij-1.2.1/src/face/
+-rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.1/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.651128 aij-1.2.1/src/fake/
+-rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.1/src/fake/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.651775 aij-1.2.1/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.1/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.653776 aij-1.2.1/src/keyboard/
+-rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.1/src/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.653776 aij-1.2.1/src/knowledge/
+-rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.1/src/knowledge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.656297 aij-1.2.1/src/language/
+-rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.1/src/language/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.658817 aij-1.2.1/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.1/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.660923 aij-1.2.1/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.1/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.661920 aij-1.2.1/src/objectron/
+-rw-rw-rw-   0        0        0     1781 2023-05-27 23:37:19.000000 aij-1.2.1/src/objectron/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.663925 aij-1.2.1/src/scrape/
+-rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.1/src/scrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.663925 aij-1.2.1/src/selfie/
+-rw-rw-rw-   0        0        0     3329 2023-05-27 23:20:20.000000 aij-1.2.1/src/selfie/__ini__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.666444 aij-1.2.1/src/sentiment/
+-rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.1/src/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.667443 aij-1.2.1/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.1/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.668952 aij-1.2.1/src/stream/
+-rw-rw-rw-   0        0        0     1093 2023-05-24 23:06:34.000000 aij-1.2.1/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.669962 aij-1.2.1/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.1/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.671045 aij-1.2.1/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.1/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.673572 aij-1.2.1/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.1/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.675897 aij-1.2.1/src/volume/
+-rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.1/src/volume/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.677476 aij-1.2.1/src/webcam/
+-rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.1/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.680005 aij-1.2.1/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.1/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:52:15.681041 aij-1.2.1/src/webcam3/
+-rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.1/src/webcam3/__init__.py
```

### Comparing `aij-1.2.0/LICENSE.txt` & `aij-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/PKG-INFO` & `aij-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.0
+Version: 1.2.1
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.0/README.md` & `aij-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/pyproject.toml` & `aij-1.2.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.2.0"
+version = "1.2.1"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
@@ -184,15 +184,41 @@
 "Funding" = "https://donate.pypi.org"
 "Say Thanks!" = "http://saythanks.io/to/aij"
 "Source" = "https://github.com/codesapienbe/aij"
 
 # The following would provide a command line executable called `sample`
 # which executes the function `main` from this package when invoked.
 [project.scripts]  # Optional
-
+aij = "webcam:main"
+aij-animation = "animation:main"
+aij-chat = "chat:main"
+aij-download = "download:main"
+aij-emotion = "emotion:main"
+aij-entity = "entity:main"
+aij-face = "face:main"
+aij-fake = "fake:main"
+aij-intro = "intro:main"
+aij-keyboard = "keyboard:main"
+aij-knowledge = "knowledge:main"
+aij-language = "language:main"
+aij-messaging = "messaging:main"
+aij-news = "news:main"
+aij-objectron = "objectron:main"
+aij-scrape = "scrape:main"
+aij-selfie = "selfie:main"
+aij-sentiment = "sentiment:main"
+aij-setup = "setup:main"
+aij-stream = "stream:main"
+aij-transcibe = "transcribe:main"
+aij-translate = "translate:main"
+aij-voice = "voice:main"
+aij-volume = "volume:main"
+aij-webcam = "webcam:main"
+aij-webcam2 = "webcam2:main"
+aij-webcam3 = "webcam3:main"
 
 # This is configuration specific to the `setuptools` build backend.
 # If you are using a different build backend, you will need to change this.
 [tool.setuptools]
 # If there are data files included in your packages that need to be
 # installed, specify them here.
 package-data = { "db" = ["*.dat"] }
```

### Comparing `aij-1.2.0/src/aij.egg-info/PKG-INFO` & `aij-1.2.1/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.0
+Version: 1.2.1
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.0/src/aij.egg-info/SOURCES.txt` & `aij-1.2.1/src/aij.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 LICENSE.txt
 README.md
 pyproject.toml
 src/aij.egg-info/PKG-INFO
 src/aij.egg-info/SOURCES.txt
 src/aij.egg-info/dependency_links.txt
+src/aij.egg-info/entry_points.txt
 src/aij.egg-info/requires.txt
 src/aij.egg-info/top_level.txt
 src/animation/__init__.py
-src/category/__init__.py
 src/chat/__init__.py
 src/download/__init__.py
 src/emotion/__init__.py
 src/entity/__init__.py
 src/face/__init__.py
 src/fake/__init__.py
 src/intro/__init__.py
```

### Comparing `aij-1.2.0/src/aij.egg-info/requires.txt` & `aij-1.2.1/src/aij.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/animation/__init__.py` & `aij-1.2.1/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/chat/__init__.py` & `aij-1.2.1/src/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/download/__init__.py` & `aij-1.2.1/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/emotion/__init__.py` & `aij-1.2.1/src/emotion/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/entity/__init__.py` & `aij-1.2.1/src/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/face/__init__.py` & `aij-1.2.1/src/face/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/fake/__init__.py` & `aij-1.2.1/src/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/intro/__init__.py` & `aij-1.2.1/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/keyboard/__init__.py` & `aij-1.2.1/src/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/knowledge/__init__.py` & `aij-1.2.1/src/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/messaging/__init__.py` & `aij-1.2.1/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/news/__init__.py` & `aij-1.2.1/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/objectron/__init__.py` & `aij-1.2.1/src/objectron/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/scrape/__init__.py` & `aij-1.2.1/src/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/selfie/__ini__.py` & `aij-1.2.1/src/selfie/__ini__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/sentiment/__init__.py` & `aij-1.2.1/src/sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/setup/__init__.py` & `aij-1.2.1/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/stream/__init__.py` & `aij-1.2.1/src/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/transcribe/__init__.py` & `aij-1.2.1/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/translate/__init__.py` & `aij-1.2.1/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/voice/__init__.py` & `aij-1.2.1/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/volume/__init__.py` & `aij-1.2.1/src/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/webcam/__init__.py` & `aij-1.2.1/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/webcam2/__init__.py` & `aij-1.2.1/src/webcam2/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.0/src/webcam3/__init__.py` & `aij-1.2.1/src/webcam3/__init__.py`

 * *Files identical despite different names*


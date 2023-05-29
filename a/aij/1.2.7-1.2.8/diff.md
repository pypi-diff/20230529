# Comparing `tmp/aij-1.2.7.tar.gz` & `tmp/aij-1.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aij-1.2.7.tar", last modified: Mon May 29 14:04:07 2023, max compression
+gzip compressed data, was "aij-1.2.8.tar", last modified: Mon May 29 15:04:06 2023, max compression
```

## Comparing `aij-1.2.7.tar` & `aij-1.2.8.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.435872 aij-1.2.7/
--rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.7/LICENSE.txt
--rw-rw-rw-   0        0        0    30052 2023-05-29 14:04:07.435872 aij-1.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.7/README.md
--rw-rw-rw-   0        0        0     7696 2023-05-29 14:03:57.000000 aij-1.2.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 14:04:07.437287 aij-1.2.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.352763 aij-1.2.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.385212 aij-1.2.7/src/aij.egg-info/
--rw-rw-rw-   0        0        0    30052 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      841 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      725 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      606 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/requires.txt
--rw-rw-rw-   0        0        0      202 2023-05-29 14:04:07.000000 aij-1.2.7/src/aij.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.386209 aij-1.2.7/src/animation/
--rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.7/src/animation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.388205 aij-1.2.7/src/chat/
--rw-rw-rw-   0        0        0     3861 2023-05-26 12:12:18.000000 aij-1.2.7/src/chat/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.391201 aij-1.2.7/src/download/
--rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.7/src/download/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.394210 aij-1.2.7/src/emotion/
--rw-rw-rw-   0        0        0     2537 2023-05-26 12:58:13.000000 aij-1.2.7/src/emotion/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.395791 aij-1.2.7/src/entity/
--rw-rw-rw-   0        0        0      651 2023-05-26 12:48:48.000000 aij-1.2.7/src/entity/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.397754 aij-1.2.7/src/face/
--rw-rw-rw-   0        0        0     7696 2023-05-26 11:57:56.000000 aij-1.2.7/src/face/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.398745 aij-1.2.7/src/fake/
--rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.7/src/fake/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.400741 aij-1.2.7/src/intro/
--rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.7/src/intro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.402743 aij-1.2.7/src/keyboard/
--rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.7/src/keyboard/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.404754 aij-1.2.7/src/knowledge/
--rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.7/src/knowledge/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.405751 aij-1.2.7/src/language/
--rw-rw-rw-   0        0        0      507 2023-05-26 12:36:22.000000 aij-1.2.7/src/language/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.407214 aij-1.2.7/src/messaging/
--rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.7/src/messaging/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.409219 aij-1.2.7/src/news/
--rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.7/src/news/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.411216 aij-1.2.7/src/objectron/
--rw-rw-rw-   0        0        0     1992 2023-05-29 14:03:52.000000 aij-1.2.7/src/objectron/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.412216 aij-1.2.7/src/scrape/
--rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.7/src/scrape/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.414689 aij-1.2.7/src/selfie/
--rw-rw-rw-   0        0        0     3671 2023-05-29 14:00:41.000000 aij-1.2.7/src/selfie/__ini__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.416697 aij-1.2.7/src/sentiment/
--rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.7/src/sentiment/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.420309 aij-1.2.7/src/setup/
--rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.7/src/setup/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.421313 aij-1.2.7/src/stream/
--rw-rw-rw-   0        0        0     1976 2023-05-29 00:10:40.000000 aij-1.2.7/src/stream/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.423315 aij-1.2.7/src/transcribe/
--rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.7/src/transcribe/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.424316 aij-1.2.7/src/translate/
--rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.7/src/translate/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.426841 aij-1.2.7/src/voice/
--rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.7/src/voice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.428871 aij-1.2.7/src/volume/
--rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.7/src/volume/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.430878 aij-1.2.7/src/webcam/
--rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.7/src/webcam/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.431878 aij-1.2.7/src/webcam2/
--rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.7/src/webcam2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 14:04:07.433875 aij-1.2.7/src/webcam3/
--rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.7/src/webcam3/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.489664 aij-1.2.8/
+-rw-rw-rw-   0        0        0     1100 2023-05-21 18:35:40.000000 aij-1.2.8/LICENSE.txt
+-rw-rw-rw-   0        0        0    30052 2023-05-29 15:04:06.487661 aij-1.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    27745 2023-05-21 18:35:40.000000 aij-1.2.8/README.md
+-rw-rw-rw-   0        0        0     7696 2023-05-29 15:03:56.000000 aij-1.2.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 15:04:06.489664 aij-1.2.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.399408 aij-1.2.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.437789 aij-1.2.8/src/aij.egg-info/
+-rw-rw-rw-   0        0        0    30052 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      841 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      725 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      606 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      202 2023-05-29 15:04:06.000000 aij-1.2.8/src/aij.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.439786 aij-1.2.8/src/animation/
+-rw-rw-rw-   0        0        0     5848 2023-05-26 21:14:59.000000 aij-1.2.8/src/animation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.441779 aij-1.2.8/src/chat/
+-rw-rw-rw-   0        0        0     4002 2023-05-29 14:13:33.000000 aij-1.2.8/src/chat/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.443787 aij-1.2.8/src/download/
+-rw-rw-rw-   0        0        0     8301 2023-05-24 21:25:22.000000 aij-1.2.8/src/download/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.446785 aij-1.2.8/src/emotion/
+-rw-rw-rw-   0        0        0     2688 2023-05-29 14:18:56.000000 aij-1.2.8/src/emotion/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.447781 aij-1.2.8/src/entity/
+-rw-rw-rw-   0        0        0      651 2023-05-29 14:09:50.000000 aij-1.2.8/src/entity/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.449777 aij-1.2.8/src/face/
+-rw-rw-rw-   0        0        0     7945 2023-05-29 14:08:59.000000 aij-1.2.8/src/face/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.451164 aij-1.2.8/src/fake/
+-rw-rw-rw-   0        0        0      765 2023-05-26 12:46:38.000000 aij-1.2.8/src/fake/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.452181 aij-1.2.8/src/intro/
+-rw-rw-rw-   0        0        0     4532 2023-05-24 21:19:40.000000 aij-1.2.8/src/intro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.454194 aij-1.2.8/src/keyboard/
+-rw-rw-rw-   0        0        0    19934 2023-05-28 23:01:31.000000 aij-1.2.8/src/keyboard/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.456191 aij-1.2.8/src/knowledge/
+-rw-rw-rw-   0        0        0      807 2023-05-26 12:39:25.000000 aij-1.2.8/src/knowledge/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.458184 aij-1.2.8/src/language/
+-rw-rw-rw-   0        0        0      673 2023-05-29 14:16:07.000000 aij-1.2.8/src/language/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.460579 aij-1.2.8/src/messaging/
+-rw-rw-rw-   0        0        0     5060 2023-05-23 19:12:37.000000 aij-1.2.8/src/messaging/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.462589 aij-1.2.8/src/news/
+-rw-rw-rw-   0        0        0    10270 2023-05-25 21:21:31.000000 aij-1.2.8/src/news/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.464593 aij-1.2.8/src/objectron/
+-rw-rw-rw-   0        0        0     1992 2023-05-29 14:03:52.000000 aij-1.2.8/src/objectron/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.465589 aij-1.2.8/src/scrape/
+-rw-rw-rw-   0        0        0     1875 2023-05-26 21:20:55.000000 aij-1.2.8/src/scrape/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.467597 aij-1.2.8/src/selfie/
+-rw-rw-rw-   0        0        0     3671 2023-05-29 14:00:41.000000 aij-1.2.8/src/selfie/__ini__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.468591 aij-1.2.8/src/sentiment/
+-rw-rw-rw-   0        0        0      549 2023-05-26 12:50:27.000000 aij-1.2.8/src/sentiment/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.470590 aij-1.2.8/src/setup/
+-rw-rw-rw-   0        0        0     3925 2023-05-24 22:31:30.000000 aij-1.2.8/src/setup/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.471594 aij-1.2.8/src/stream/
+-rw-rw-rw-   0        0        0     1976 2023-05-29 00:10:40.000000 aij-1.2.8/src/stream/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.473592 aij-1.2.8/src/transcribe/
+-rw-rw-rw-   0        0        0     2215 2023-05-25 21:10:13.000000 aij-1.2.8/src/transcribe/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.474661 aij-1.2.8/src/translate/
+-rw-rw-rw-   0        0        0     2393 2023-05-25 21:47:13.000000 aij-1.2.8/src/translate/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.478686 aij-1.2.8/src/voice/
+-rw-rw-rw-   0        0        0     2239 2023-05-25 23:23:39.000000 aij-1.2.8/src/voice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.481678 aij-1.2.8/src/volume/
+-rw-rw-rw-   0        0        0     4322 2023-05-28 20:58:13.000000 aij-1.2.8/src/volume/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.482662 aij-1.2.8/src/webcam/
+-rw-rw-rw-   0        0        0    18760 2023-05-28 23:46:12.000000 aij-1.2.8/src/webcam/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.484661 aij-1.2.8/src/webcam2/
+-rw-rw-rw-   0        0        0     3351 2023-05-25 22:17:56.000000 aij-1.2.8/src/webcam2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:04:06.485665 aij-1.2.8/src/webcam3/
+-rw-rw-rw-   0        0        0    20490 2023-05-28 23:32:49.000000 aij-1.2.8/src/webcam3/__init__.py
```

### Comparing `aij-1.2.7/LICENSE.txt` & `aij-1.2.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/PKG-INFO` & `aij-1.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.7
+Version: 1.2.8
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.7/README.md` & `aij-1.2.8/README.md`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/pyproject.toml` & `aij-1.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 name = "aij"  # Required
 
 # Versions should comply with PEP 440:
 # https://www.python.org/dev/peps/pep-0440/
 #
 # For a discussion on single-sourcing the version, see
 # https://packaging.python.org/guides/single-sourcing-package-version/
-version = "1.2.7"
+version = "1.2.8"
 
 # This is a one-line description or tagline of what your project does. This
 # corresponds to the "Summary" metadata field:
 # https://packaging.python.org/specifications/core-metadata/#summary
 description = "AI Journalist"  # Optional
 
 # This is an optional longer description of your project that represents
```

### Comparing `aij-1.2.7/src/aij.egg-info/PKG-INFO` & `aij-1.2.8/src/aij.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aij
-Version: 1.2.7
+Version: 1.2.8
 Summary: AI Journalist
 Author-email: Yilmaz Mustafa <dev@mail.be>
 License: Copyright (c) 2016 The Python Packaging Authority (PyPA)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
```

### Comparing `aij-1.2.7/src/aij.egg-info/SOURCES.txt` & `aij-1.2.8/src/aij.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/aij.egg-info/entry_points.txt` & `aij-1.2.8/src/aij.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/aij.egg-info/requires.txt` & `aij-1.2.8/src/aij.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/animation/__init__.py` & `aij-1.2.8/src/animation/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/chat/__init__.py` & `aij-1.2.8/src/chat/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -122,11 +122,18 @@
     ai_assistant = AIAssistant(api_key)
     consumer = NewsConsumer('localhost', ai_assistant)
 
     try:
         consumer.consume()
     except KeyboardInterrupt:
         consumer.close()
+        
+        
+    result = ai_assistant.generate_response("What do you think about blockchain?")
 
 
+    print(
+        result
+    )
+
 if __name__ == '__main__':
     main()
```

### Comparing `aij-1.2.7/src/download/__init__.py` & `aij-1.2.8/src/download/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/emotion/__init__.py` & `aij-1.2.8/src/emotion/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,30 +39,36 @@
     # Normalize the pixel values to be between 0 and 1
     face = face / 255.0
     # Predict the emotion label using the trained model
     predictions = model.predict(face)
     # Return the predicted emotion label
     return emotions[np.argmax(predictions)]
 
-# Open a video stream
-cap = cv2.VideoCapture(0)
+def main():
 
-while True:
-    # Read a frame from the video stream
-    ret, frame = cap.read()
-    # Detect the face in the frame
-    face, coords = detect_face(frame)
-    # If a face is detected, predict the emotion label and draw a rectangle around the face
-    if face is not None:
-        emotion = predict_emotion(face)
-        x, y, w, h = coords
-        cv2.rectangle(frame, (x, y), (x+w, y+h), (0, 255, 0), 2)
-        cv2.putText(frame, emotion, (x, y-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 255, 0), 2)
-    # Display the frame
-    cv2.imshow('Face Emotion Recognition', frame)
-    # Wait for a key press
-    if cv2.waitKey(1) & 0xFF == ord('q'):
-        break
+    # Open a video stream
+    cap = cv2.VideoCapture(0)
 
-# Release the video stream and close all windows
-cap.release()
-cv2.destroyAllWindows()
+    while True:
+        # Read a frame from the video stream
+        ret, frame = cap.read()
+        # Detect the face in the frame
+        face, coords = detect_face(frame)
+        # If a face is detected, predict the emotion label and draw a rectangle around the face
+        if face is not None:
+            emotion = predict_emotion(face)
+            x, y, w, h = coords
+            cv2.rectangle(frame, (x, y), (x+w, y+h), (0, 255, 0), 2)
+            cv2.putText(frame, emotion, (x, y-10), cv2.FONT_HERSHEY_SIMPLEX, 0.9, (0, 255, 0), 2)
+        # Display the frame
+        cv2.imshow('Face Emotion Recognition', frame)
+        # Wait for a key press
+        if cv2.waitKey(1) & 0xFF == ord('q'):
+            break
+
+    # Release the video stream and close all windows
+    cap.release()
+    cv2.destroyAllWindows()
+    
+    
+if __name__ == '__main__':
+    main()
```

### Comparing `aij-1.2.7/src/entity/__init__.py` & `aij-1.2.8/src/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/face/__init__.py` & `aij-1.2.8/src/face/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,70 +223,75 @@
     x = image_width - emj_width - 5
     y = image_height - emj_height - 5
     # draw the emj on the main image
     img[y:y + emj_height, x:x + emj_width] = emj_resized
     return img
 
 
-# do not wait for the directories to be created
-thread_download_logo = threading.Thread(target=download_logo)
-thread_download_logo.start()
-
-default_backend = "opencv"
-default_model = "VGG-Face"
-
-cam = cv2.VideoCapture(0)
-cam.set(cv2.CAP_PROP_FRAME_WIDTH, SCREEN_WIDTH)
-cam.set(cv2.CAP_PROP_FRAME_HEIGHT, SCREEN_HEIGHT)
-cam.set(cv2.CAP_PROP_FPS, SCREEN_FPS)
-
-# Define min window size to be recognized as a face
-MIN_FACE_FRAME_WIDTH = 50
-MIN_FACE_FRAME_HEIGHT = 50
-FRAME_COUNTER = 0
-current_emotion = "neutral"
-
-while cam.isOpened():
-
-    ret, img = cam.read()
-    img = cv2.flip(img, 1)  # Flip vertically
-    gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
-
-    # increase the frame counter
-    FRAME_COUNTER += 1
-
-    try:
-        # after each 5 seconds detect faces
-        if FRAME_COUNTER >= SCREEN_FPS:
-            # reset the frame counter
-            FRAME_COUNTER = 0
-            # predict the emotion
-            emotion = DeepFace.analyze(img_path=img, actions=[
-                'emotion'], detector_backend=default_backend, align=True, silent=True)
-
-            # get the emotion data from the dictionary
-            emotion_data = emotion[0]['emotion']
-            # convert to dataframe
-            emotion_df = pd.DataFrame(emotion_data, index=[0])
-            # get the dominant emotion
-            emotion_label = emotion_df.idxmax(axis=1)[0]
-            # add the emotion to the emotion history
-            current_emotion = emotion_label
-
-    except Exception as e:
-        # draw error message if no face detected
-        pass
+def main():
 
-    img = draw_emoji(current_emotion, img)
-    img = draw_logo(logo_abs, img)
+    # do not wait for the directories to be created
+    thread_download_logo = threading.Thread(target=download_logo)
+    thread_download_logo.start()
+
+    default_backend = "opencv"
+    default_model = "VGG-Face"
+
+    cam = cv2.VideoCapture(0)
+    cam.set(cv2.CAP_PROP_FRAME_WIDTH, SCREEN_WIDTH)
+    cam.set(cv2.CAP_PROP_FRAME_HEIGHT, SCREEN_HEIGHT)
+    cam.set(cv2.CAP_PROP_FPS, SCREEN_FPS)
+
+    # Define min window size to be recognized as a face
+    MIN_FACE_FRAME_WIDTH = 50
+    MIN_FACE_FRAME_HEIGHT = 50
+    FRAME_COUNTER = 0
+    current_emotion = "neutral"
+
+    while cam.isOpened():
+
+        ret, img = cam.read()
+        img = cv2.flip(img, 1)  # Flip vertically
+        gray = cv2.cvtColor(img, cv2.COLOR_BGR2GRAY)
+
+        # increase the frame counter
+        FRAME_COUNTER += 1
+
+        try:
+            # after each 5 seconds detect faces
+            if FRAME_COUNTER >= SCREEN_FPS:
+                # reset the frame counter
+                FRAME_COUNTER = 0
+                # predict the emotion
+                emotion = DeepFace.analyze(img_path=img, actions=[
+                    'emotion'], detector_backend=default_backend, align=True, silent=True)
+
+                # get the emotion data from the dictionary
+                emotion_data = emotion[0]['emotion']
+                # convert to dataframe
+                emotion_df = pd.DataFrame(emotion_data, index=[0])
+                # get the dominant emotion
+                emotion_label = emotion_df.idxmax(axis=1)[0]
+                # add the emotion to the emotion history
+                current_emotion = emotion_label
+
+        except Exception as e:
+            # draw error message if no face detected
+            pass
+
+        img = draw_emoji(current_emotion, img)
+        img = draw_logo(logo_abs, img)
+
+        cv2.imshow('Emotion Recognition', img)
+
+        if cv2.waitKey(1) & 0xFF == ord('q'):
+            cam.release()
+            break
 
-    cv2.imshow('Emotion Recognition', img)
-
-    if cv2.waitKey(1) & 0xFF == ord('q'):
+    if cam.isOpened():
         cam.release()
-        break
 
+    cv2.destroyAllWindows()
 
-if cam.isOpened():
-    cam.release()
 
-cv2.destroyAllWindows()
+if __name__ == '__main__':
+    main()
```

### Comparing `aij-1.2.7/src/fake/__init__.py` & `aij-1.2.8/src/fake/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/intro/__init__.py` & `aij-1.2.8/src/intro/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/keyboard/__init__.py` & `aij-1.2.8/src/keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/knowledge/__init__.py` & `aij-1.2.8/src/knowledge/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/messaging/__init__.py` & `aij-1.2.8/src/messaging/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/news/__init__.py` & `aij-1.2.8/src/news/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/objectron/__init__.py` & `aij-1.2.8/src/objectron/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/scrape/__init__.py` & `aij-1.2.8/src/scrape/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/selfie/__ini__.py` & `aij-1.2.8/src/selfie/__ini__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/sentiment/__init__.py` & `aij-1.2.8/src/sentiment/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/setup/__init__.py` & `aij-1.2.8/src/setup/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/stream/__init__.py` & `aij-1.2.8/src/stream/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/transcribe/__init__.py` & `aij-1.2.8/src/transcribe/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/translate/__init__.py` & `aij-1.2.8/src/translate/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/voice/__init__.py` & `aij-1.2.8/src/voice/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/volume/__init__.py` & `aij-1.2.8/src/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/webcam/__init__.py` & `aij-1.2.8/src/webcam/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/webcam2/__init__.py` & `aij-1.2.8/src/webcam2/__init__.py`

 * *Files identical despite different names*

### Comparing `aij-1.2.7/src/webcam3/__init__.py` & `aij-1.2.8/src/webcam3/__init__.py`

 * *Files identical despite different names*


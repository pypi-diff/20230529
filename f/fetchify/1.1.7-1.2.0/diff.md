# Comparing `tmp/fetchify-1.1.7.tar.gz` & `tmp/fetchify-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetchify-1.1.7.tar", last modified: Sat May 27 15:26:03 2023, max compression
+gzip compressed data, was "fetchify-1.2.0.tar", last modified: Mon May 29 10:10:01 2023, max compression
```

## Comparing `fetchify-1.1.7.tar` & `fetchify-1.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 15:26:03.226784 fetchify-1.1.7/
--rw-rw-rw-   0        0        0      594 2023-05-27 15:26:03.106735 fetchify-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 15:26:03.104733 fetchify-1.1.7/fetchify.egg-info/
--rw-rw-rw-   0        0        0      594 2023-05-27 15:26:02.000000 fetchify-1.1.7/fetchify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-27 15:26:02.000000 fetchify-1.1.7/fetchify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 15:26:02.000000 fetchify-1.1.7/fetchify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 15:26:02.000000 fetchify-1.1.7/fetchify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-27 15:26:02.000000 fetchify-1.1.7/fetchify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      899 2023-05-27 15:25:30.000000 fetchify-1.1.7/fetchify.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.1.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-27 15:26:03.226784 fetchify-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-05-27 15:25:44.000000 fetchify-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:10:01.468557 fetchify-1.2.0/
+-rw-rw-rw-   0        0        0      594 2023-05-29 10:10:01.467099 fetchify-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 10:10:01.466101 fetchify-1.2.0/fetchify.egg-info/
+-rw-rw-rw-   0        0        0      594 2023-05-29 10:10:00.000000 fetchify-1.2.0/fetchify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-29 10:10:01.000000 fetchify-1.2.0/fetchify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 10:10:00.000000 fetchify-1.2.0/fetchify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 10:10:00.000000 fetchify-1.2.0/fetchify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 10:10:00.000000 fetchify-1.2.0/fetchify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      736 2023-05-29 10:05:56.000000 fetchify-1.2.0/fetchify.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 10:10:01.468557 fetchify-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-05-29 10:09:39.000000 fetchify-1.2.0/setup.py
```

### Comparing `fetchify-1.1.7/PKG-INFO` & `fetchify-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.1.7
+Version: 1.2.0
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.1.7/fetchify.egg-info/PKG-INFO` & `fetchify-1.2.0/fetchify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.1.7
+Version: 1.2.0
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.1.7/setup.py` & `fetchify-1.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fetchify",
-    version="1.1.7",
+    version="1.2.0",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Library to access Code Files from Cloud",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://techinfoak.wixsite.com/tech-info",
     project_urls={
```


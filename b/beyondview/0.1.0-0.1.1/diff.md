# Comparing `tmp/beyondview-0.1.0.tar.gz` & `tmp/beyondview-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beyondview-0.1.0.tar", last modified: Mon May 29 10:24:08 2023, max compression
+gzip compressed data, was "beyondview-0.1.1.tar", last modified: Mon May 29 10:42:25 2023, max compression
```

## Comparing `beyondview-0.1.0.tar` & `beyondview-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 10:24:08.006734 beyondview-0.1.0/
--rw-rw-rw-   0        0        0    35823 2023-05-29 06:31:20.000000 beyondview-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      538 2023-05-29 10:24:08.005737 beyondview-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      112 2023-05-29 06:44:14.000000 beyondview-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 10:24:07.992781 beyondview-0.1.0/beyondview/
--rw-rw-rw-   0        0        0        0 2023-05-29 09:07:36.000000 beyondview-0.1.0/beyondview/__init__.py
--rw-rw-rw-   0        0        0       70 2023-05-29 06:59:11.000000 beyondview-0.1.0/beyondview/test.py
-drwxrwxrwx   0        0        0        0 2023-05-29 10:24:08.004741 beyondview-0.1.0/beyondview.egg-info/
--rw-rw-rw-   0        0        0      538 2023-05-29 10:24:07.000000 beyondview-0.1.0/beyondview.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-29 10:24:07.000000 beyondview-0.1.0/beyondview.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 10:24:07.000000 beyondview-0.1.0/beyondview.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-29 10:24:07.000000 beyondview-0.1.0/beyondview.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 10:24:08.006734 beyondview-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      640 2023-05-29 10:21:45.000000 beyondview-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:42:25.425075 beyondview-0.1.1/
+-rw-rw-rw-   0        0        0    35823 2023-05-29 06:31:20.000000 beyondview-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      538 2023-05-29 10:42:25.425075 beyondview-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      112 2023-05-29 06:44:14.000000 beyondview-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 10:42:25.417665 beyondview-0.1.1/beyondview/
+-rw-rw-rw-   0        0        0       66 2023-05-29 10:33:31.000000 beyondview-0.1.1/beyondview/Maths.py
+-rw-rw-rw-   0        0        0       70 2023-05-29 06:59:11.000000 beyondview-0.1.1/beyondview/Test.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 09:07:36.000000 beyondview-0.1.1/beyondview/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:42:25.423080 beyondview-0.1.1/beyondview.egg-info/
+-rw-rw-rw-   0        0        0      538 2023-05-29 10:42:25.000000 beyondview-0.1.1/beyondview.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      243 2023-05-29 10:42:25.000000 beyondview-0.1.1/beyondview.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 10:42:25.000000 beyondview-0.1.1/beyondview.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-29 10:42:25.000000 beyondview-0.1.1/beyondview.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 10:42:25.425075 beyondview-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      640 2023-05-29 10:41:39.000000 beyondview-0.1.1/setup.py
```

### Comparing `beyondview-0.1.0/LICENSE` & `beyondview-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beyondview-0.1.0/PKG-INFO` & `beyondview-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beyondview
-Version: 0.1.0
+Version: 0.1.1
 Summary: General python tools for beyondview
 Home-page: https://github.com/jgbv/beyondview
 Author: Jesson Go
 Author-email: jesson.go@beyondview.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `beyondview-0.1.0/beyondview.egg-info/PKG-INFO` & `beyondview-0.1.1/beyondview.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beyondview
-Version: 0.1.0
+Version: 0.1.1
 Summary: General python tools for beyondview
 Home-page: https://github.com/jgbv/beyondview
 Author: Jesson Go
 Author-email: jesson.go@beyondview.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `beyondview-0.1.0/setup.py` & `beyondview-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="beyondview",
-    version="0.1.0",
+    version="0.1.1",
     author="Jesson Go",
     author_email="jesson.go@beyondview.com",
     description="General python tools for beyondview",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jgbv/beyondview",
     packages=setuptools.find_packages(),
```


# Comparing `tmp/thsquant-0.1.2.tar.gz` & `tmp/thsquant-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thsquant-0.1.2.tar", last modified: Mon May 29 07:02:34 2023, max compression
+gzip compressed data, was "thsquant-0.1.3.tar", last modified: Mon May 29 07:19:01 2023, max compression
```

## Comparing `thsquant-0.1.2.tar` & `thsquant-0.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 07:02:34.413935 thsquant-0.1.2/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 thsquant-0.1.2/LICENSE.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 07:02:34.413935 thsquant-0.1.2/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       24 2023-05-29 07:02:12.000000 thsquant-0.1.2/README.md
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 07:02:34.413935 thsquant-0.1.2/setup.cfg
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      993 2023-05-29 07:02:06.000000 thsquant-0.1.2/setup.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 07:02:34.413935 thsquant-0.1.2/thsquant.egg-info/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 07:02:34.000000 thsquant-0.1.2/thsquant.egg-info/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      193 2023-05-29 07:02:34.000000 thsquant-0.1.2/thsquant.egg-info/SOURCES.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 07:02:34.000000 thsquant-0.1.2/thsquant.egg-info/dependency_links.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       44 2023-05-29 07:02:34.000000 thsquant-0.1.2/thsquant.egg-info/entry_points.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 07:02:34.000000 thsquant-0.1.2/thsquant.egg-info/top_level.txt
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 07:19:01.288931 thsquant-0.1.3/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 thsquant-0.1.3/LICENSE.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 07:19:01.288931 thsquant-0.1.3/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       24 2023-05-29 07:18:52.000000 thsquant-0.1.3/README.md
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 07:19:01.288931 thsquant-0.1.3/setup.cfg
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      996 2023-05-29 07:18:44.000000 thsquant-0.1.3/setup.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 07:19:01.288931 thsquant-0.1.3/thsquant.egg-info/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 07:19:00.000000 thsquant-0.1.3/thsquant.egg-info/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      193 2023-05-29 07:19:01.000000 thsquant-0.1.3/thsquant.egg-info/SOURCES.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 07:19:01.000000 thsquant-0.1.3/thsquant.egg-info/dependency_links.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       47 2023-05-29 07:19:01.000000 thsquant-0.1.3/thsquant.egg-info/entry_points.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 07:19:01.000000 thsquant-0.1.3/thsquant.egg-info/top_level.txt
```

### Comparing `thsquant-0.1.2/LICENSE.txt` & `thsquant-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thsquant-0.1.2/PKG-INFO` & `thsquant-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.1.2
+Version: 0.1.3
 Summary: A short description of your awesome package
 Home-page: https://github.com/qinbo23/ths-quant
 Author: qinbo
 Author-email: qinbo@myhexin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -16,10 +16,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ths-quant
-test 0.1.2 
+test 0.1.3
```

### Comparing `thsquant-0.1.2/setup.py` & `thsquant-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="thsquant",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
     ],
     entry_points={
         'console_scripts': [
-            'thsquant = quant:sayhello'
+            'thsquant = thsquant:sayhello'
         ]
     },
     author="qinbo",
     author_email="qinbo@myhexin.com",
     description="A short description of your awesome package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `thsquant-0.1.2/thsquant.egg-info/PKG-INFO` & `thsquant-0.1.3/thsquant.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.1.2
+Version: 0.1.3
 Summary: A short description of your awesome package
 Home-page: https://github.com/qinbo23/ths-quant
 Author: qinbo
 Author-email: qinbo@myhexin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -16,10 +16,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ths-quant
-test 0.1.2 
+test 0.1.3
```


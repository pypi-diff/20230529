# Comparing `tmp/thsquant-0.1.7.tar.gz` & `tmp/thsquant-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thsquant-0.1.7.tar", last modified: Mon May 29 11:28:51 2023, max compression
+gzip compressed data, was "thsquant-0.1.8.tar", last modified: Mon May 29 12:26:35 2023, max compression
```

## Comparing `thsquant-0.1.7.tar` & `thsquant-0.1.8.tar`

### file list

```diff
@@ -1,12 +1,16 @@
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 11:28:51.881046 thsquant-0.1.7/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 thsquant-0.1.7/LICENSE.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 11:28:51.881046 thsquant-0.1.7/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       24 2023-05-29 11:27:34.000000 thsquant-0.1.7/README.md
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 11:28:51.881046 thsquant-0.1.7/setup.cfg
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     1002 2023-05-29 11:27:24.000000 thsquant-0.1.7/setup.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 11:28:51.881046 thsquant-0.1.7/thsquant.egg-info/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 11:28:51.000000 thsquant-0.1.7/thsquant.egg-info/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      193 2023-05-29 11:28:51.000000 thsquant-0.1.7/thsquant.egg-info/SOURCES.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 11:28:51.000000 thsquant-0.1.7/thsquant.egg-info/dependency_links.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       53 2023-05-29 11:28:51.000000 thsquant-0.1.7/thsquant.egg-info/entry_points.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 11:28:51.000000 thsquant-0.1.7/thsquant.egg-info/top_level.txt
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 12:26:35.497076 thsquant-0.1.8/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 thsquant-0.1.8/LICENSE.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-29 12:26:35.497076 thsquant-0.1.8/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       18 2023-05-29 12:07:48.000000 thsquant-0.1.8/README.md
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 12:26:35.497076 thsquant-0.1.8/setup.cfg
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1008 2023-05-29 12:24:51.000000 thsquant-0.1.8/setup.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 12:26:35.497076 thsquant-0.1.8/thsquant/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 09:25:35.000000 thsquant-0.1.8/thsquant/__init__.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       16 2023-05-29 12:07:58.000000 thsquant-0.1.8/thsquant/config.py
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      352 2023-05-29 12:25:49.000000 thsquant-0.1.8/thsquant/quant.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 12:26:35.497076 thsquant-0.1.8/thsquant.egg-info/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      747 2023-05-29 12:26:35.000000 thsquant-0.1.8/thsquant.egg-info/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      251 2023-05-29 12:26:35.000000 thsquant-0.1.8/thsquant.egg-info/SOURCES.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 12:26:35.000000 thsquant-0.1.8/thsquant.egg-info/dependency_links.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       59 2023-05-29 12:26:35.000000 thsquant-0.1.8/thsquant.egg-info/entry_points.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        9 2023-05-29 12:26:35.000000 thsquant-0.1.8/thsquant.egg-info/top_level.txt
```

### Comparing `thsquant-0.1.7/LICENSE.txt` & `thsquant-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thsquant-0.1.7/PKG-INFO` & `thsquant-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.1.7
+Version: 0.1.8
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
-test 0.1.7 
+test
```

### Comparing `thsquant-0.1.7/setup.py` & `thsquant-0.1.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name="thsquant",
-    version="0.1.7",
+    version="0.1.8",
     packages=find_packages(),
     install_requires=[
     ],
     entry_points={
         'console_scripts': [
-            'thsquant-llama = thsquant:sayhello'
+            'thsquant-llama = thsquant.quant:sayhello'
         ]
     },
     author="qinbo",
     author_email="qinbo@myhexin.com",
     description="A short description of your awesome package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `thsquant-0.1.7/thsquant.egg-info/PKG-INFO` & `thsquant-0.1.8/thsquant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.1.7
+Version: 0.1.8
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
-test 0.1.7 
+test
```


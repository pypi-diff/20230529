# Comparing `tmp/thsquant-0.1.5.tar.gz` & `tmp/thsquant-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thsquant-0.1.5.tar", last modified: Mon May 29 09:26:40 2023, max compression
+gzip compressed data, was "thsquant-0.1.6.tar", last modified: Mon May 29 11:25:11 2023, max compression
```

## Comparing `thsquant-0.1.5.tar` & `thsquant-0.1.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 09:26:40.185001 thsquant-0.1.5/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 thsquant-0.1.5/LICENSE.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 09:26:40.185001 thsquant-0.1.5/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       24 2023-05-29 09:26:26.000000 thsquant-0.1.5/README.md
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 09:26:40.185001 thsquant-0.1.5/setup.cfg
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     1002 2023-05-29 09:26:35.000000 thsquant-0.1.5/setup.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 09:26:40.185001 thsquant-0.1.5/thsquant.egg-info/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 09:26:39.000000 thsquant-0.1.5/thsquant.egg-info/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      193 2023-05-29 09:26:40.000000 thsquant-0.1.5/thsquant.egg-info/SOURCES.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 09:26:39.000000 thsquant-0.1.5/thsquant.egg-info/dependency_links.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       53 2023-05-29 09:26:40.000000 thsquant-0.1.5/thsquant.egg-info/entry_points.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 09:26:40.000000 thsquant-0.1.5/thsquant.egg-info/top_level.txt
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 11:25:11.197288 thsquant-0.1.6/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 thsquant-0.1.6/LICENSE.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 11:25:11.197288 thsquant-0.1.6/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       24 2023-05-29 11:23:46.000000 thsquant-0.1.6/README.md
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 11:25:11.197288 thsquant-0.1.6/setup.cfg
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1002 2023-05-29 11:24:43.000000 thsquant-0.1.6/setup.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 11:25:11.197288 thsquant-0.1.6/thsquant.egg-info/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 11:25:10.000000 thsquant-0.1.6/thsquant.egg-info/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      193 2023-05-29 11:25:11.000000 thsquant-0.1.6/thsquant.egg-info/SOURCES.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 11:25:10.000000 thsquant-0.1.6/thsquant.egg-info/dependency_links.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       53 2023-05-29 11:25:11.000000 thsquant-0.1.6/thsquant.egg-info/entry_points.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 11:25:11.000000 thsquant-0.1.6/thsquant.egg-info/top_level.txt
```

### Comparing `thsquant-0.1.5/LICENSE.txt` & `thsquant-0.1.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thsquant-0.1.5/PKG-INFO` & `thsquant-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.1.5
+Version: 0.1.6
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
-test 0.1.5 
+test 0.1.6
```

### Comparing `thsquant-0.1.5/setup.py` & `thsquant-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="thsquant",
-    version="0.1.5",
+    version="0.1.6",
     packages=find_packages(),
     install_requires=[
     ],
     entry_points={
         'console_scripts': [
             'thsquant-llama = thsquant:sayhello'
         ]
```

### Comparing `thsquant-0.1.5/thsquant.egg-info/PKG-INFO` & `thsquant-0.1.6/thsquant.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.1.5
+Version: 0.1.6
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
-test 0.1.5 
+test 0.1.6
```


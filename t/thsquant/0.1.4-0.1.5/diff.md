# Comparing `tmp/thsquant-0.1.4.tar.gz` & `tmp/thsquant-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thsquant-0.1.4.tar", last modified: Mon May 29 09:08:35 2023, max compression
+gzip compressed data, was "thsquant-0.1.5.tar", last modified: Mon May 29 09:26:40 2023, max compression
```

## Comparing `thsquant-0.1.4.tar` & `thsquant-0.1.5.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 09:08:35.174193 thsquant-0.1.4/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 thsquant-0.1.4/LICENSE.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 09:08:35.174193 thsquant-0.1.4/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       24 2023-05-29 09:08:08.000000 thsquant-0.1.4/README.md
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 09:08:35.174193 thsquant-0.1.4/setup.cfg
--rw-r--r--   0 qinbo     (1014) nmt       (1300)     1002 2023-05-29 09:07:43.000000 thsquant-0.1.4/setup.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 09:08:35.174193 thsquant-0.1.4/thsquant.egg-info/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 09:08:34.000000 thsquant-0.1.4/thsquant.egg-info/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      193 2023-05-29 09:08:35.000000 thsquant-0.1.4/thsquant.egg-info/SOURCES.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 09:08:34.000000 thsquant-0.1.4/thsquant.egg-info/dependency_links.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       53 2023-05-29 09:08:35.000000 thsquant-0.1.4/thsquant.egg-info/entry_points.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 09:08:35.000000 thsquant-0.1.4/thsquant.egg-info/top_level.txt
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 09:26:40.185001 thsquant-0.1.5/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 thsquant-0.1.5/LICENSE.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 09:26:40.185001 thsquant-0.1.5/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       24 2023-05-29 09:26:26.000000 thsquant-0.1.5/README.md
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 09:26:40.185001 thsquant-0.1.5/setup.cfg
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)     1002 2023-05-29 09:26:35.000000 thsquant-0.1.5/setup.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 09:26:40.185001 thsquant-0.1.5/thsquant.egg-info/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      753 2023-05-29 09:26:39.000000 thsquant-0.1.5/thsquant.egg-info/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      193 2023-05-29 09:26:40.000000 thsquant-0.1.5/thsquant.egg-info/SOURCES.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 09:26:39.000000 thsquant-0.1.5/thsquant.egg-info/dependency_links.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       53 2023-05-29 09:26:40.000000 thsquant-0.1.5/thsquant.egg-info/entry_points.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 09:26:40.000000 thsquant-0.1.5/thsquant.egg-info/top_level.txt
```

### Comparing `thsquant-0.1.4/LICENSE.txt` & `thsquant-0.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `thsquant-0.1.4/PKG-INFO` & `thsquant-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.1.4
+Version: 0.1.5
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
-test 0.1.4 
+test 0.1.5
```

### Comparing `thsquant-0.1.4/setup.py` & `thsquant-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="thsquant",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
     ],
     entry_points={
         'console_scripts': [
             'thsquant-llama = thsquant:sayhello'
         ]
```

### Comparing `thsquant-0.1.4/thsquant.egg-info/PKG-INFO` & `thsquant-0.1.5/thsquant.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thsquant
-Version: 0.1.4
+Version: 0.1.5
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
-test 0.1.4 
+test 0.1.5
```


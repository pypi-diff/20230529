# Comparing `tmp/ths-quant-0.1.1.tar.gz` & `tmp/ths-quant-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ths-quant-0.1.1.tar", last modified: Thu May 25 12:57:59 2023, max compression
+gzip compressed data, was "ths-quant-0.1.2.tar", last modified: Mon May 29 06:37:43 2023, max compression
```

## Comparing `ths-quant-0.1.1.tar` & `ths-quant-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-25 12:57:59.000000 ths-quant-0.1.1/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       12 2023-05-25 12:56:30.000000 ths-quant-0.1.1/README.md
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      890 2023-05-25 12:57:28.000000 ths-quant-0.1.1/setup.py
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      742 2023-05-25 12:57:59.000000 ths-quant-0.1.1/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-25 12:57:59.000000 ths-quant-0.1.1/setup.cfg
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 ths-quant-0.1.1/LICENSE.txt
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-25 12:57:59.000000 ths-quant-0.1.1/ths_quant.egg-info/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-25 12:57:59.000000 ths-quant-0.1.1/ths_quant.egg-info/top_level.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      742 2023-05-25 12:57:59.000000 ths-quant-0.1.1/ths_quant.egg-info/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-25 12:57:59.000000 ths-quant-0.1.1/ths_quant.egg-info/dependency_links.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      162 2023-05-25 12:57:59.000000 ths-quant-0.1.1/ths_quant.egg-info/SOURCES.txt
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 06:37:43.259464 ths-quant-0.1.2/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 ths-quant-0.1.2/LICENSE.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      754 2023-05-29 06:37:43.259464 ths-quant-0.1.2/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       24 2023-05-29 05:50:50.000000 ths-quant-0.1.2/README.md
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 06:37:43.259464 ths-quant-0.1.2/setup.cfg
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      890 2023-05-29 05:50:43.000000 ths-quant-0.1.2/setup.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 06:37:43.259464 ths-quant-0.1.2/ths_quant.egg-info/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      754 2023-05-29 06:37:42.000000 ths-quant-0.1.2/ths_quant.egg-info/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      162 2023-05-29 06:37:43.000000 ths-quant-0.1.2/ths_quant.egg-info/SOURCES.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 06:37:42.000000 ths-quant-0.1.2/ths_quant.egg-info/dependency_links.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 06:37:43.000000 ths-quant-0.1.2/ths_quant.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `ths-quant-0.1.1/setup.py` & `ths-quant-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ths-quant",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     install_requires=[
     ],
 
     author="qinbo",
     author_email="qinbo@myhexin.com",
     description="A short description of your awesome package",
```

### Comparing `ths-quant-0.1.1/PKG-INFO` & `ths-quant-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ths-quant
-Version: 0.1.1
+Version: 0.1.2
 Summary: A short description of your awesome package
 Home-page: https://github.com/qinbo23/ths-quant
 Author: qinbo
 Author-email: qinbo@myhexin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -16,9 +16,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ths-quant
+test 0.1.2
```

### Comparing `ths-quant-0.1.1/LICENSE.txt` & `ths-quant-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ths-quant-0.1.1/ths_quant.egg-info/PKG-INFO` & `ths-quant-0.1.2/ths_quant.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ths-quant
-Version: 0.1.1
+Version: 0.1.2
 Summary: A short description of your awesome package
 Home-page: https://github.com/qinbo23/ths-quant
 Author: qinbo
 Author-email: qinbo@myhexin.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -16,9 +16,10 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # ths-quant
+test 0.1.2
```


# Comparing `tmp/ths-quant-0.1.2.tar.gz` & `tmp/ths-quant-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ths-quant-0.1.2.tar", last modified: Mon May 29 06:37:43 2023, max compression
+gzip compressed data, was "ths-quant-0.1.3.tar", last modified: Mon May 29 06:42:01 2023, max compression
```

## Comparing `ths-quant-0.1.2.tar` & `ths-quant-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 06:37:43.259464 ths-quant-0.1.2/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 ths-quant-0.1.2/LICENSE.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      754 2023-05-29 06:37:43.259464 ths-quant-0.1.2/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       24 2023-05-29 05:50:50.000000 ths-quant-0.1.2/README.md
--rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 06:37:43.259464 ths-quant-0.1.2/setup.cfg
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      890 2023-05-29 05:50:43.000000 ths-quant-0.1.2/setup.py
-drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 06:37:43.259464 ths-quant-0.1.2/ths_quant.egg-info/
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      754 2023-05-29 06:37:42.000000 ths-quant-0.1.2/ths_quant.egg-info/PKG-INFO
--rw-r--r--   0 qinbo     (1014) nmt       (1300)      162 2023-05-29 06:37:43.000000 ths-quant-0.1.2/ths_quant.egg-info/SOURCES.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 06:37:42.000000 ths-quant-0.1.2/ths_quant.egg-info/dependency_links.txt
--rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 06:37:43.000000 ths-quant-0.1.2/ths_quant.egg-info/top_level.txt
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 06:42:01.839197 ths-quant-0.1.3/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)    11357 2023-05-25 12:56:47.000000 ths-quant-0.1.3/LICENSE.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      754 2023-05-29 06:42:01.839197 ths-quant-0.1.3/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       24 2023-05-29 06:41:49.000000 ths-quant-0.1.3/README.md
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       38 2023-05-29 06:42:01.839197 ths-quant-0.1.3/setup.cfg
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      987 2023-05-29 06:41:19.000000 ths-quant-0.1.3/setup.py
+drwxr-xr-x   0 qinbo     (1014) nmt       (1300)        0 2023-05-29 06:42:01.839197 ths-quant-0.1.3/ths_quant.egg-info/
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      754 2023-05-29 06:42:01.000000 ths-quant-0.1.3/ths_quant.egg-info/PKG-INFO
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)      198 2023-05-29 06:42:01.000000 ths-quant-0.1.3/ths_quant.egg-info/SOURCES.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 06:42:01.000000 ths-quant-0.1.3/ths_quant.egg-info/dependency_links.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)       37 2023-05-29 06:42:01.000000 ths-quant-0.1.3/ths_quant.egg-info/entry_points.txt
+-rw-r--r--   0 qinbo     (1014) nmt       (1300)        1 2023-05-29 06:42:01.000000 ths-quant-0.1.3/ths_quant.egg-info/top_level.txt
```

### Comparing `ths-quant-0.1.2/LICENSE.txt` & `ths-quant-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ths-quant-0.1.2/setup.py` & `ths-quant-0.1.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ths-quant",
-    version="0.1.2",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
     ],
-
+    entry_points={
+        'console_scripts': [
+            'hello = hello:main'
+        ]
+    },
     author="qinbo",
     author_email="qinbo@myhexin.com",
     description="A short description of your awesome package",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/qinbo23/ths-quant",
```


# Comparing `tmp/superstes_ctf_tools-1.0.0.tar.gz` & `tmp/superstes_ctf_tools-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superstes_ctf_tools-1.0.0.tar", last modified: Mon May 29 18:48:39 2023, max compression
+gzip compressed data, was "superstes_ctf_tools-1.0.1.tar", last modified: Mon May 29 18:51:22 2023, max compression
```

## Comparing `superstes_ctf_tools-1.0.0.tar` & `superstes_ctf_tools-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-05-29 18:48:39.361071 superstes_ctf_tools-1.0.0/
--rw-rw-r--   0 superstes  (1000) superstes  (1000)    33230 2023-05-29 18:09:01.000000 superstes_ctf_tools-1.0.0/LICENSE.txt
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      739 2023-05-29 18:48:39.361071 superstes_ctf_tools-1.0.0/PKG-INFO
--rw-rw-r--   0 superstes  (1000) superstes  (1000)       92 2023-05-29 18:06:52.000000 superstes_ctf_tools-1.0.0/README.md
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      490 2023-05-29 18:04:29.000000 superstes_ctf_tools-1.0.0/convert.py
--rw-rw-r--   0 superstes  (1000) superstes  (1000)       85 2023-04-19 18:56:28.000000 superstes_ctf_tools-1.0.0/pyproject.toml
--rw-rw-r--   0 superstes  (1000) superstes  (1000)       38 2023-05-29 18:48:39.361071 superstes_ctf_tools-1.0.0/setup.cfg
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      865 2023-05-29 18:17:18.000000 superstes_ctf_tools-1.0.0/setup.py
-drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-05-29 18:48:39.361071 superstes_ctf_tools-1.0.0/superstes_ctf_tools.egg-info/
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      739 2023-05-29 18:48:39.000000 superstes_ctf_tools-1.0.0/superstes_ctf_tools.egg-info/PKG-INFO
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      228 2023-05-29 18:48:39.000000 superstes_ctf_tools-1.0.0/superstes_ctf_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 superstes  (1000) superstes  (1000)        1 2023-05-29 18:48:39.000000 superstes_ctf_tools-1.0.0/superstes_ctf_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 superstes  (1000) superstes  (1000)        8 2023-05-29 18:48:39.000000 superstes_ctf_tools-1.0.0/superstes_ctf_tools.egg-info/top_level.txt
+drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-05-29 18:51:22.118267 superstes_ctf_tools-1.0.1/
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)    33230 2023-05-29 18:09:01.000000 superstes_ctf_tools-1.0.1/LICENSE.txt
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      739 2023-05-29 18:51:22.118267 superstes_ctf_tools-1.0.1/PKG-INFO
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)       92 2023-05-29 18:06:52.000000 superstes_ctf_tools-1.0.1/README.md
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)       85 2023-04-19 18:56:28.000000 superstes_ctf_tools-1.0.1/pyproject.toml
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)       38 2023-05-29 18:51:22.118267 superstes_ctf_tools-1.0.1/setup.cfg
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      865 2023-05-29 18:51:17.000000 superstes_ctf_tools-1.0.1/setup.py
+drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-05-29 18:51:22.118267 superstes_ctf_tools-1.0.1/superstes_ctf_tools.egg-info/
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      739 2023-05-29 18:51:22.000000 superstes_ctf_tools-1.0.1/superstes_ctf_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      217 2023-05-29 18:51:22.000000 superstes_ctf_tools-1.0.1/superstes_ctf_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)        1 2023-05-29 18:51:22.000000 superstes_ctf_tools-1.0.1/superstes_ctf_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)        1 2023-05-29 18:51:22.000000 superstes_ctf_tools-1.0.1/superstes_ctf_tools.egg-info/top_level.txt
```

### Comparing `superstes_ctf_tools-1.0.0/LICENSE.txt` & `superstes_ctf_tools-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superstes_ctf_tools-1.0.0/PKG-INFO` & `superstes_ctf_tools-1.0.1/superstes_ctf_tools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: superstes_ctf_tools
-Version: 1.0.0
+Name: superstes-ctf-tools
+Version: 1.0.1
 Summary: Some python utils and scripts that I find useful for security challenges
 Home-page: https://github.com/superstes/ctf-tools
 Author: René Rath
 Author-email: contact@superstes.eu
 Project-URL: Repository, https://github.com/superstes/ctf-tools
 Project-URL: Bug Tracker, https://github.com/superstes/ctf-tools/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `superstes_ctf_tools-1.0.0/setup.py` & `superstes_ctf_tools-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as info:
     long_description = info.read()
 
 setuptools.setup(
     name='superstes_ctf_tools',
-    version='1.0.0',
+    version='1.0.1',
     author='René Rath',
     author_email='contact@superstes.eu',
     description='Some python utils and scripts that I find useful for security challenges',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/superstes/ctf-tools',
     project_urls={
```

### Comparing `superstes_ctf_tools-1.0.0/superstes_ctf_tools.egg-info/PKG-INFO` & `superstes_ctf_tools-1.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: superstes-ctf-tools
-Version: 1.0.0
+Name: superstes_ctf_tools
+Version: 1.0.1
 Summary: Some python utils and scripts that I find useful for security challenges
 Home-page: https://github.com/superstes/ctf-tools
 Author: René Rath
 Author-email: contact@superstes.eu
 Project-URL: Repository, https://github.com/superstes/ctf-tools
 Project-URL: Bug Tracker, https://github.com/superstes/ctf-tools/issues
 Classifier: Programming Language :: Python :: 3
```


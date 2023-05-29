# Comparing `tmp/superstes_ctf_tools-1.0.2.tar.gz` & `tmp/superstes_ctf_tools-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superstes_ctf_tools-1.0.2.tar", last modified: Mon May 29 18:53:33 2023, max compression
+gzip compressed data, was "superstes_ctf_tools-1.0.3.tar", last modified: Mon May 29 18:57:37 2023, max compression
```

## Comparing `superstes_ctf_tools-1.0.2.tar` & `superstes_ctf_tools-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-05-29 18:53:33.175413 superstes_ctf_tools-1.0.2/
--rw-rw-r--   0 superstes  (1000) superstes  (1000)    33230 2023-05-29 18:09:01.000000 superstes_ctf_tools-1.0.2/LICENSE.txt
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      739 2023-05-29 18:53:33.171413 superstes_ctf_tools-1.0.2/PKG-INFO
--rw-rw-r--   0 superstes  (1000) superstes  (1000)       92 2023-05-29 18:06:52.000000 superstes_ctf_tools-1.0.2/README.md
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      490 2023-05-29 18:04:29.000000 superstes_ctf_tools-1.0.2/ctf_utils.py
--rw-rw-r--   0 superstes  (1000) superstes  (1000)       85 2023-04-19 18:56:28.000000 superstes_ctf_tools-1.0.2/pyproject.toml
--rw-rw-r--   0 superstes  (1000) superstes  (1000)       38 2023-05-29 18:53:33.175413 superstes_ctf_tools-1.0.2/setup.cfg
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      865 2023-05-29 18:53:29.000000 superstes_ctf_tools-1.0.2/setup.py
-drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-05-29 18:53:33.171413 superstes_ctf_tools-1.0.2/superstes_ctf_tools.egg-info/
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      739 2023-05-29 18:53:33.000000 superstes_ctf_tools-1.0.2/superstes_ctf_tools.egg-info/PKG-INFO
--rw-rw-r--   0 superstes  (1000) superstes  (1000)      230 2023-05-29 18:53:33.000000 superstes_ctf_tools-1.0.2/superstes_ctf_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 superstes  (1000) superstes  (1000)        1 2023-05-29 18:53:33.000000 superstes_ctf_tools-1.0.2/superstes_ctf_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 superstes  (1000) superstes  (1000)       10 2023-05-29 18:53:33.000000 superstes_ctf_tools-1.0.2/superstes_ctf_tools.egg-info/top_level.txt
+drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-05-29 18:57:37.569861 superstes_ctf_tools-1.0.3/
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)    33230 2023-05-29 18:09:01.000000 superstes_ctf_tools-1.0.3/LICENSE.txt
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      739 2023-05-29 18:57:37.569861 superstes_ctf_tools-1.0.3/PKG-INFO
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)       92 2023-05-29 18:06:52.000000 superstes_ctf_tools-1.0.3/README.md
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      530 2023-05-29 18:57:33.000000 superstes_ctf_tools-1.0.3/ctf_utils.py
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)       85 2023-04-19 18:56:28.000000 superstes_ctf_tools-1.0.3/pyproject.toml
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)       38 2023-05-29 18:57:37.569861 superstes_ctf_tools-1.0.3/setup.cfg
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      865 2023-05-29 18:57:33.000000 superstes_ctf_tools-1.0.3/setup.py
+drwxrwxr-x   0 superstes  (1000) superstes  (1000)        0 2023-05-29 18:57:37.569861 superstes_ctf_tools-1.0.3/superstes_ctf_tools.egg-info/
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      739 2023-05-29 18:57:37.000000 superstes_ctf_tools-1.0.3/superstes_ctf_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)      230 2023-05-29 18:57:37.000000 superstes_ctf_tools-1.0.3/superstes_ctf_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)        1 2023-05-29 18:57:37.000000 superstes_ctf_tools-1.0.3/superstes_ctf_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 superstes  (1000) superstes  (1000)       10 2023-05-29 18:57:37.000000 superstes_ctf_tools-1.0.3/superstes_ctf_tools.egg-info/top_level.txt
```

### Comparing `superstes_ctf_tools-1.0.2/LICENSE.txt` & `superstes_ctf_tools-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `superstes_ctf_tools-1.0.2/PKG-INFO` & `superstes_ctf_tools-1.0.3/superstes_ctf_tools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: superstes_ctf_tools
-Version: 1.0.2
+Name: superstes-ctf-tools
+Version: 1.0.3
 Summary: Some python utils and scripts that I find useful for security challenges
 Home-page: https://github.com/superstes/ctf-tools
 Author: René Rath
 Author-email: contact@superstes.eu
 Project-URL: Repository, https://github.com/superstes/ctf-tools
 Project-URL: Bug Tracker, https://github.com/superstes/ctf-tools/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `superstes_ctf_tools-1.0.2/setup.py` & `superstes_ctf_tools-1.0.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r', encoding='utf-8') as info:
     long_description = info.read()
 
 setuptools.setup(
     name='superstes_ctf_tools',
-    version='1.0.2',
+    version='1.0.3',
     author='René Rath',
     author_email='contact@superstes.eu',
     description='Some python utils and scripts that I find useful for security challenges',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/superstes/ctf-tools',
     project_urls={
```

### Comparing `superstes_ctf_tools-1.0.2/superstes_ctf_tools.egg-info/PKG-INFO` & `superstes_ctf_tools-1.0.3/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: superstes-ctf-tools
-Version: 1.0.2
+Name: superstes_ctf_tools
+Version: 1.0.3
 Summary: Some python utils and scripts that I find useful for security challenges
 Home-page: https://github.com/superstes/ctf-tools
 Author: René Rath
 Author-email: contact@superstes.eu
 Project-URL: Repository, https://github.com/superstes/ctf-tools
 Project-URL: Bug Tracker, https://github.com/superstes/ctf-tools/issues
 Classifier: Programming Language :: Python :: 3
```


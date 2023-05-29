# Comparing `tmp/np_codeocean-0.1.3.tar.gz` & `tmp/np_codeocean-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_codeocean-0.1.3.tar", last modified: Wed May 24 20:16:14 2023, max compression
+gzip compressed data, was "np_codeocean-0.1.4.tar", last modified: Mon May 29 19:53:37 2023, max compression
```

## Comparing `np_codeocean-0.1.3.tar` & `np_codeocean-0.1.4.tar`

### file list

```diff
@@ -1,6 +1,8 @@
--rw-r--r--   0        0        0      107 2023-05-02 03:16:59.498618 np_codeocean-0.1.3/README.md
--rw-r--r--   0        0        0     1834 2023-05-24 20:16:14.825779 np_codeocean-0.1.3/pyproject.toml
--rw-r--r--   0        0        0       66 2023-05-24 20:01:38.495205 np_codeocean-0.1.3/src/np_codeocean/__init__.py
--rw-r--r--   0        0        0     5377 2023-05-10 23:18:08.279782 np_codeocean-0.1.3/src/np_codeocean/upload.py
--rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.1.3/src/np_codeocean/utils.py
--rw-r--r--   0        0        0     1239 1970-01-01 00:00:00.000000 np_codeocean-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      107 2023-05-02 03:16:59.498618 np_codeocean-0.1.4/README.md
+-rw-r--r--   0        0        0     1807 2023-05-29 19:53:37.437154 np_codeocean-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       74 2023-05-29 19:53:07.139299 np_codeocean-0.1.4/src/np_codeocean/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 20:31:03.116207 np_codeocean-0.1.4/src/np_codeocean/__main__.py
+-rw-r--r--   0        0        0     7410 2023-05-24 23:26:55.631538 np_codeocean-0.1.4/src/np_codeocean/upload_one.py
+-rw-r--r--   0        0        0     5377 2023-05-10 23:18:08.279782 np_codeocean-0.1.4/src/np_codeocean/upload_session.py
+-rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.1.4/src/np_codeocean/utils.py
+-rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 np_codeocean-0.1.4/PKG-INFO
```

### Comparing `np_codeocean-0.1.3/pyproject.toml` & `np_codeocean-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,26 +36,24 @@
 composite = [
     "bump",
     "pdm publish",
 ]
 
 [project]
 name = "np_codeocean"
-version = "0.1.3"
+version = "0.1.4"
 description = "Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean"
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "np_session>=0.6.4",
     "np_tools>=0.1.12",
-    "aind-data-transfer[ephys]>=0.15",
-    "cmake",
+    "aind-data-transfer[ephys]>=0.20",
     "setuptools>=36.2.0",
-    "awscli",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
```

### Comparing `np_codeocean-0.1.3/src/np_codeocean/upload.py` & `np_codeocean-0.1.4/src/np_codeocean/upload_session.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.3/src/np_codeocean/utils.py` & `np_codeocean-0.1.4/src/np_codeocean/utils.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.3/PKG-INFO` & `np_codeocean-0.1.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-codeocean
-Version: 0.1.3
+Version: 0.1.4
 Summary: Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,18 +13,16 @@
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Project-URL: Source, https://github.com/AllenInstitute/np_codeocean
 Project-URL: Issues, https://github.com/AllenInstitute/np_codeocean/issues
 Requires-Python: >=3.8
 Requires-Dist: np_session>=0.6.4
 Requires-Dist: np_tools>=0.1.12
-Requires-Dist: aind-data-transfer[ephys]>=0.15
-Requires-Dist: cmake
+Requires-Dist: aind-data-transfer[ephys]>=0.20
 Requires-Dist: setuptools>=36.2.0
-Requires-Dist: awscli
 Requires-Dist: bump>=1.3.2; extra == "dev"
 Requires-Dist: pdm>=2.4.9; extra == "dev"
 Provides-Extra: dev
 Description-Content-Type: text/markdown
 
 # np_codeocean
 Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean
```


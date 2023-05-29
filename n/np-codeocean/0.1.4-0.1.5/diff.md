# Comparing `tmp/np_codeocean-0.1.4.tar.gz` & `tmp/np_codeocean-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_codeocean-0.1.4.tar", last modified: Mon May 29 19:53:37 2023, max compression
+gzip compressed data, was "np_codeocean-0.1.5.tar", last modified: Mon May 29 21:03:24 2023, max compression
```

## Comparing `np_codeocean-0.1.4.tar` & `np_codeocean-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      107 2023-05-02 03:16:59.498618 np_codeocean-0.1.4/README.md
--rw-r--r--   0        0        0     1807 2023-05-29 19:53:37.437154 np_codeocean-0.1.4/pyproject.toml
--rw-r--r--   0        0        0       74 2023-05-29 19:53:07.139299 np_codeocean-0.1.4/src/np_codeocean/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 20:31:03.116207 np_codeocean-0.1.4/src/np_codeocean/__main__.py
--rw-r--r--   0        0        0     7410 2023-05-24 23:26:55.631538 np_codeocean-0.1.4/src/np_codeocean/upload_one.py
--rw-r--r--   0        0        0     5377 2023-05-10 23:18:08.279782 np_codeocean-0.1.4/src/np_codeocean/upload_session.py
--rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.1.4/src/np_codeocean/utils.py
--rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 np_codeocean-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      107 2023-05-02 03:16:59.498618 np_codeocean-0.1.5/README.md
+-rw-r--r--   0        0        0     1807 2023-05-29 21:03:24.143263 np_codeocean-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-05-29 21:03:14.073762 np_codeocean-0.1.5/src/np_codeocean/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 20:31:03.116207 np_codeocean-0.1.5/src/np_codeocean/__main__.py
+-rw-r--r--   0        0        0     5377 2023-05-10 23:18:08.279782 np_codeocean-0.1.5/src/np_codeocean/upload.py
+-rw-r--r--   0        0        0     7410 2023-05-24 23:26:55.631538 np_codeocean-0.1.5/src/np_codeocean/upload_one.py
+-rw-r--r--   0        0        0     3375 2023-05-10 23:12:49.826589 np_codeocean-0.1.5/src/np_codeocean/utils.py
+-rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 np_codeocean-0.1.5/PKG-INFO
```

### Comparing `np_codeocean-0.1.4/pyproject.toml` & `np_codeocean-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 composite = [
     "bump",
     "pdm publish",
 ]
 
 [project]
 name = "np_codeocean"
-version = "0.1.4"
+version = "0.1.5"
 description = "Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean"
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "np_session>=0.6.4",
     "np_tools>=0.1.12",
```

### Comparing `np_codeocean-0.1.4/src/np_codeocean/upload_one.py` & `np_codeocean-0.1.5/src/np_codeocean/upload_one.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.4/src/np_codeocean/upload_session.py` & `np_codeocean-0.1.5/src/np_codeocean/upload.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.4/src/np_codeocean/utils.py` & `np_codeocean-0.1.5/src/np_codeocean/utils.py`

 * *Files identical despite different names*

### Comparing `np_codeocean-0.1.4/PKG-INFO` & `np_codeocean-0.1.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-codeocean
-Version: 0.1.4
+Version: 0.1.5
 Summary: Tools for uploading and interacting with Mindscope Neuropixels experiments on Code Ocean
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


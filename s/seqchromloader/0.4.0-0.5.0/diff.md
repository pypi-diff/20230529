# Comparing `tmp/seqchromloader-0.4.0.tar.gz` & `tmp/seqchromloader-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seqchromloader-0.4.0.tar", last modified: Wed Apr 12 20:59:39 2023, max compression
+gzip compressed data, was "seqchromloader-0.5.0.tar", last modified: Mon May 29 19:06:59 2023, max compression
```

## Comparing `seqchromloader-0.4.0.tar` & `seqchromloader-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-04-12 20:59:39.821490 seqchromloader-0.4.0/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-04-12 20:59:39.820919 seqchromloader-0.4.0/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.4.0/README.md
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-04-12 20:59:39.812257 seqchromloader-0.4.0/seqchromloader/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      176 2023-04-12 20:00:32.000000 seqchromloader-0.4.0/seqchromloader/__init__.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12427 2023-04-12 19:57:21.000000 seqchromloader-0.4.0/seqchromloader/loader.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    14355 2022-10-21 21:55:06.000000 seqchromloader-0.4.0/seqchromloader/utils.py
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     6248 2023-04-12 20:33:18.000000 seqchromloader-0.4.0/seqchromloader/writer.py
-drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-04-12 20:59:39.819836 seqchromloader-0.4.0/seqchromloader.egg-info/
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-04-12 20:59:39.000000 seqchromloader-0.4.0/seqchromloader.egg-info/PKG-INFO
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      308 2023-04-12 20:59:39.000000 seqchromloader-0.4.0/seqchromloader.egg-info/SOURCES.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-04-12 20:59:39.000000 seqchromloader-0.4.0/seqchromloader.egg-info/dependency_links.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-04-12 20:59:39.000000 seqchromloader-0.4.0/seqchromloader.egg-info/requires.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-04-12 20:59:39.000000 seqchromloader-0.4.0/seqchromloader.egg-info/top_level.txt
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-04-12 20:59:39.821658 seqchromloader-0.4.0/setup.cfg
--rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-04-12 20:58:23.000000 seqchromloader-0.4.0/setup.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 19:06:59.043941 seqchromloader-0.5.0/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-05-29 19:06:59.043643 seqchromloader-0.5.0/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      649 2023-03-27 19:08:58.000000 seqchromloader-0.5.0/README.md
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 19:06:59.038916 seqchromloader-0.5.0/seqchromloader/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      280 2023-05-29 18:55:42.000000 seqchromloader-0.5.0/seqchromloader/__init__.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)    12427 2023-04-12 19:57:21.000000 seqchromloader-0.5.0/seqchromloader/loader.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     9899 2023-05-29 18:44:55.000000 seqchromloader-0.5.0/seqchromloader/utils.py
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     6248 2023-04-12 20:33:18.000000 seqchromloader-0.5.0/seqchromloader/writer.py
+drwxr-xr-x   0 jmy5455  (258298369) PSU\Domain Users (357253257)        0 2023-05-29 19:06:59.043132 seqchromloader-0.5.0/seqchromloader.egg-info/
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     1086 2023-05-29 19:06:58.000000 seqchromloader-0.5.0/seqchromloader.egg-info/PKG-INFO
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      308 2023-05-29 19:06:59.000000 seqchromloader-0.5.0/seqchromloader.egg-info/SOURCES.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)        1 2023-05-29 19:06:58.000000 seqchromloader-0.5.0/seqchromloader.egg-info/dependency_links.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)      126 2023-05-29 19:06:58.000000 seqchromloader-0.5.0/seqchromloader.egg-info/requires.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       15 2023-05-29 19:06:58.000000 seqchromloader-0.5.0/seqchromloader.egg-info/top_level.txt
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)       38 2023-05-29 19:06:59.044023 seqchromloader-0.5.0/setup.cfg
+-rw-r--r--   0 jmy5455  (258298369) PSU\Domain Users (357253257)     3368 2023-05-29 18:56:49.000000 seqchromloader-0.5.0/setup.py
```

### Comparing `seqchromloader-0.4.0/PKG-INFO` & `seqchromloader-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.4.0
+Version: 0.5.0
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.4.0/README.md` & `seqchromloader-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.4.0/seqchromloader/loader.py` & `seqchromloader-0.5.0/seqchromloader/loader.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.4.0/seqchromloader/writer.py` & `seqchromloader-0.5.0/seqchromloader/writer.py`

 * *Files identical despite different names*

### Comparing `seqchromloader-0.4.0/seqchromloader.egg-info/PKG-INFO` & `seqchromloader-0.5.0/seqchromloader.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seqchromloader
-Version: 0.4.0
+Version: 0.5.0
 Summary: Sequence and chromatin dataloader for deep learning
 Home-page: https://github.com/yztxwd/seqchromloader
 Author-email: yztxwd@gmail.com
 Keywords: dataloder,pytorch,webdataset
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `seqchromloader-0.4.0/setup.py` & `seqchromloader-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     # The version of your project.
     # Usually, it would be in the form of:
     # major.minor.patch
     # eg: 1.0.0, 1.0.1, 3.0.2, 5.0-beta, etc.
     # You CANNOT upload two versions of your package with the same version number
     # This field is REQUIRED
-    version="0.4.0",
+    version="0.5.0",
 
     # The packages that constitute your project.
     # For my project, I have only one - "pydash".
     # Either you could write the name of the package, or
     # alternatively use setuptools.findpackages()
     #
     # If you only have one file, instead of a package,
```


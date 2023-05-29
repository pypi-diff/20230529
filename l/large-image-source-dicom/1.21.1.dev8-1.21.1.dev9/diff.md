# Comparing `tmp/large-image-source-dicom-1.21.1.dev8.tar.gz` & `tmp/large-image-source-dicom-1.21.1.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "large-image-source-dicom-1.21.1.dev8.tar", last modified: Thu May 25 15:25:32 2023, max compression
+gzip compressed data, was "large-image-source-dicom-1.21.1.dev9.tar", last modified: Thu May 25 15:25:59 2023, max compression
```

## Comparing `large-image-source-dicom-1.21.1.dev8.tar` & `large-image-source-dicom-1.21.1.dev9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:25:32.714317 large-image-source-dicom-1.21.1.dev8/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-05-25 15:25:32.000000 large-image-source-dicom-1.21.1.dev8/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-25 15:25:32.710317 large-image-source-dicom-1.21.1.dev8/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-05-25 15:25:32.000000 large-image-source-dicom-1.21.1.dev8/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:25:32.710317 large-image-source-dicom-1.21.1.dev8/large_image_source_dicom/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-05-25 15:24:31.000000 large-image-source-dicom-1.21.1.dev8/large_image_source_dicom/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1163 2023-05-25 15:24:31.000000 large-image-source-dicom-1.21.1.dev8/large_image_source_dicom/girder_source.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:25:32.710317 large-image-source-dicom-1.21.1.dev8/large_image_source_dicom.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-25 15:25:32.000000 large-image-source-dicom-1.21.1.dev8/large_image_source_dicom.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-05-25 15:25:32.000000 large-image-source-dicom-1.21.1.dev8/large_image_source_dicom.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-25 15:25:32.000000 large-image-source-dicom-1.21.1.dev8/large_image_source_dicom.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-25 15:25:32.000000 large-image-source-dicom-1.21.1.dev8/large_image_source_dicom.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-25 15:25:32.000000 large-image-source-dicom-1.21.1.dev8/large_image_source_dicom.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-25 15:25:32.000000 large-image-source-dicom-1.21.1.dev8/large_image_source_dicom.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-25 15:25:32.714317 large-image-source-dicom-1.21.1.dev8/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2427 2023-05-25 15:24:31.000000 large-image-source-dicom-1.21.1.dev8/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:25:59.770553 large-image-source-dicom-1.21.1.dev9/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10173 2023-05-25 15:25:59.000000 large-image-source-dicom-1.21.1.dev9/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-25 15:25:59.770553 large-image-source-dicom-1.21.1.dev9/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8267 2023-05-25 15:25:59.000000 large-image-source-dicom-1.21.1.dev9/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:25:59.770553 large-image-source-dicom-1.21.1.dev9/large_image_source_dicom/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9934 2023-05-25 15:25:01.000000 large-image-source-dicom-1.21.1.dev9/large_image_source_dicom/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1163 2023-05-25 15:25:01.000000 large-image-source-dicom-1.21.1.dev9/large_image_source_dicom/girder_source.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-25 15:25:59.770553 large-image-source-dicom-1.21.1.dev9/large_image_source_dicom.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      816 2023-05-25 15:25:59.000000 large-image-source-dicom-1.21.1.dev9/large_image_source_dicom.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2023-05-25 15:25:59.000000 large-image-source-dicom-1.21.1.dev9/large_image_source_dicom.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-25 15:25:59.000000 large-image-source-dicom-1.21.1.dev9/large_image_source_dicom.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-25 15:25:59.000000 large-image-source-dicom-1.21.1.dev9/large_image_source_dicom.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-05-25 15:25:59.000000 large-image-source-dicom-1.21.1.dev9/large_image_source_dicom.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       25 2023-05-25 15:25:59.000000 large-image-source-dicom-1.21.1.dev9/large_image_source_dicom.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-25 15:25:59.770553 large-image-source-dicom-1.21.1.dev9/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2427 2023-05-25 15:25:01.000000 large-image-source-dicom-1.21.1.dev9/setup.py
```

### Comparing `large-image-source-dicom-1.21.1.dev8/LICENSE` & `large-image-source-dicom-1.21.1.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.21.1.dev8/PKG-INFO` & `large-image-source-dicom-1.21.1.dev9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.21.1.dev8
+Version: 1.21.1.dev9
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-dicom-1.21.1.dev8/README.rst` & `large-image-source-dicom-1.21.1.dev9/README.rst`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.21.1.dev8/large_image_source_dicom/__init__.py` & `large-image-source-dicom-1.21.1.dev9/large_image_source_dicom/__init__.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.21.1.dev8/large_image_source_dicom/girder_source.py` & `large-image-source-dicom-1.21.1.dev9/large_image_source_dicom/girder_source.py`

 * *Files identical despite different names*

### Comparing `large-image-source-dicom-1.21.1.dev8/large_image_source_dicom.egg-info/PKG-INFO` & `large-image-source-dicom-1.21.1.dev9/large_image_source_dicom.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: large-image-source-dicom
-Version: 1.21.1.dev8
+Version: 1.21.1.dev9
 Summary: A DICOM tilesource for large_image.
 Home-page: https://github.com/girder/large_image
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache Software License 2.0
 Keywords: large_image,tile source
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `large-image-source-dicom-1.21.1.dev8/setup.py` & `large-image-source-dicom-1.21.1.dev9/setup.py`

 * *Files identical despite different names*


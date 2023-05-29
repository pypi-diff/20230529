# Comparing `tmp/human-protocol-basemodels-1.1.3.tar.gz` & `tmp/human-protocol-basemodels-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "human-protocol-basemodels-1.1.3.tar", last modified: Mon May 29 14:33:50 2023, max compression
+gzip compressed data, was "human-protocol-basemodels-1.1.4.tar", last modified: Mon May 29 17:11:41 2023, max compression
```

## Comparing `human-protocol-basemodels-1.1.3.tar` & `human-protocol-basemodels-1.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.447311 human-protocol-basemodels-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 14:33:50.447311 human-protocol-basemodels-1.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.443311 human-protocol-basemodels-1.1.3/basemodels/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 14:33:47.000000 human-protocol-basemodels-1.1.3/basemodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.443311 human-protocol-basemodels-1.1.3/basemodels/manifest/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.443311 human-protocol-basemodels-1.1.3/basemodels/manifest/data/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/data/groundtruth.py
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/data/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/data/taskdata.py
--rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/manifest/restricted_audience.py
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/basemodels/via.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.443311 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 14:33:50.000000 human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 14:33:50.447311 human-protocol-basemodels-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 14:33:50.443311 human-protocol-basemodels-1.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31783 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/test/test_manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-29 14:31:49.000000 human-protocol-basemodels-1.1.3/test/test_preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:11:41.432062 human-protocol-basemodels-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 17:11:41.432062 human-protocol-basemodels-1.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:11:41.428062 human-protocol-basemodels-1.1.4/basemodels/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-29 17:11:38.000000 human-protocol-basemodels-1.1.4/basemodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/basemodels/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:11:41.428062 human-protocol-basemodels-1.1.4/basemodels/manifest/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/basemodels/manifest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:11:41.428062 human-protocol-basemodels-1.1.4/basemodels/manifest/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/basemodels/manifest/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/basemodels/manifest/data/groundtruth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/basemodels/manifest/data/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/basemodels/manifest/data/taskdata.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/basemodels/manifest/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/basemodels/manifest/restricted_audience.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/basemodels/via.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:11:41.432062 human-protocol-basemodels-1.1.4/human_protocol_basemodels.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 17:11:41.000000 human-protocol-basemodels-1.1.4/human_protocol_basemodels.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-29 17:11:41.000000 human-protocol-basemodels-1.1.4/human_protocol_basemodels.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:11:41.000000 human-protocol-basemodels-1.1.4/human_protocol_basemodels.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 17:11:41.000000 human-protocol-basemodels-1.1.4/human_protocol_basemodels.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 17:11:41.000000 human-protocol-basemodels-1.1.4/human_protocol_basemodels.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:11:41.000000 human-protocol-basemodels-1.1.4/human_protocol_basemodels.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:11:41.432062 human-protocol-basemodels-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:11:41.432062 human-protocol-basemodels-1.1.4/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31783 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/test/test_manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-29 17:11:28.000000 human-protocol-basemodels-1.1.4/test/test_preprocess.py
```

### Comparing `human-protocol-basemodels-1.1.3/basemodels/manifest/data/groundtruth.py` & `human-protocol-basemodels-1.1.4/basemodels/manifest/data/groundtruth.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.3/basemodels/manifest/data/taskdata.py` & `human-protocol-basemodels-1.1.4/basemodels/manifest/data/taskdata.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.3/basemodels/manifest/manifest.py` & `human-protocol-basemodels-1.1.4/basemodels/manifest/manifest.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.3/basemodels/manifest/restricted_audience.py` & `human-protocol-basemodels-1.1.4/basemodels/manifest/restricted_audience.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.3/basemodels/via.py` & `human-protocol-basemodels-1.1.4/basemodels/via.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.3/human_protocol_basemodels.egg-info/SOURCES.txt` & `human-protocol-basemodels-1.1.4/human_protocol_basemodels.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.3/setup.py` & `human-protocol-basemodels-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.3/test/test_manifest.py` & `human-protocol-basemodels-1.1.4/test/test_manifest.py`

 * *Files identical despite different names*

### Comparing `human-protocol-basemodels-1.1.3/test/test_preprocess.py` & `human-protocol-basemodels-1.1.4/test/test_preprocess.py`

 * *Files identical despite different names*


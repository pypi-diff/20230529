# Comparing `tmp/sagemaker_pytorch_inference-2.0.8.tar.gz` & `tmp/sagemaker_pytorch_inference-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sagemaker_pytorch_inference-2.0.8.tar", last modified: Thu Jan 13 14:27:03 2022, max compression
+gzip compressed data, was "dist/sagemaker_pytorch_inference-2.0.9.tar", last modified: Mon Apr  4 14:28:41 2022, max compression
```

## Comparing `sagemaker_pytorch_inference-2.0.8.tar` & `sagemaker_pytorch_inference-2.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/
--rw-rw-r--   0 root         (0) root         (0)     1536 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_inference.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_inference.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       74 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_inference.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      980 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_inference.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)      348 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_inference.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       36 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_inference.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2527 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_inference.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/
--rw-rw-r--   0 root         (0) root         (0)     7681 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/torchserve.py
--rw-rw-r--   0 root         (0) root         (0)     4243 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/ts_environment.py
--rw-rw-r--   0 root         (0) root         (0)     1320 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/serving.py
--rw-rw-r--   0 root         (0) root         (0)     1047 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/ts_parameters.py
--rw-rw-r--   0 root         (0) root         (0)     2161 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/handler_service.py
--rw-rw-r--   0 root         (0) root         (0)     6125 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/default_pytorch_inference_handler.py
--rw-rw-r--   0 root         (0) root         (0)      609 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/etc/
--rw-rw-r--   0 root         (0) root         (0)      161 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/etc/mme-ts.properties
--rw-rw-r--   0 root         (0) root         (0)     3522 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/etc/log4j2.xml
--rw-rw-r--   0 root         (0) root         (0)      148 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/etc/default-ts.properties
--rw-rw-r--   0 root         (0) root         (0)     2570 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/setup.py
--rw-rw-r--   0 root         (0) root         (0)        6 2022-01-13 14:19:36.000000 sagemaker_pytorch_inference-2.0.8/VERSION
--rw-rw-r--   0 root         (0) root         (0)    10142 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/LICENSE
--rw-rw-r--   0 root         (0) root         (0)      104 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      186 2022-01-13 01:44:50.000000 sagemaker_pytorch_inference-2.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2527 2022-01-13 14:27:03.000000 sagemaker_pytorch_inference-2.0.8/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/
+-rw-rw-r--   0 root         (0) root         (0)     1536 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_inference.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       74 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_inference.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      980 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)      348 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_inference.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       36 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_inference.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2527 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_inference.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/
+-rw-rw-r--   0 root         (0) root         (0)     7681 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/torchserve.py
+-rw-rw-r--   0 root         (0) root         (0)     4243 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/ts_environment.py
+-rw-rw-r--   0 root         (0) root         (0)     1320 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/serving.py
+-rw-rw-r--   0 root         (0) root         (0)     1047 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/ts_parameters.py
+-rw-rw-r--   0 root         (0) root         (0)     2161 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/handler_service.py
+-rw-rw-r--   0 root         (0) root         (0)     6125 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/default_pytorch_inference_handler.py
+-rw-rw-r--   0 root         (0) root         (0)      609 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/etc/
+-rw-rw-r--   0 root         (0) root         (0)      161 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/etc/mme-ts.properties
+-rw-rw-r--   0 root         (0) root         (0)     3522 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/etc/log4j2.xml
+-rw-rw-r--   0 root         (0) root         (0)      148 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/etc/default-ts.properties
+-rw-rw-r--   0 root         (0) root         (0)     2570 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/setup.py
+-rw-rw-r--   0 root         (0) root         (0)        6 2022-04-04 14:19:57.000000 sagemaker_pytorch_inference-2.0.9/VERSION
+-rw-rw-r--   0 root         (0) root         (0)    10142 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      104 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      186 2022-04-01 00:44:16.000000 sagemaker_pytorch_inference-2.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2527 2022-04-04 14:28:41.000000 sagemaker_pytorch_inference-2.0.9/PKG-INFO
```

### Comparing `sagemaker_pytorch_inference-2.0.8/README.rst` & `sagemaker_pytorch_inference-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_inference.egg-info/SOURCES.txt` & `sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_inference.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_inference.egg-info/PKG-INFO` & `sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_inference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker-pytorch-inference
-Version: 2.0.8
+Version: 2.0.9
 Summary: Open source library for creating PyTorch containers to run on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-pytorch-inference-toolkit
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: ===================================
         SageMaker PyTorch Inference Toolkit
         ===================================
```

### Comparing `sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/torchserve.py` & `sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/torchserve.py`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/ts_environment.py` & `sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/ts_environment.py`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/serving.py` & `sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/serving.py`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/ts_parameters.py` & `sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/ts_parameters.py`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/handler_service.py` & `sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/handler_service.py`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/default_pytorch_inference_handler.py` & `sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/default_pytorch_inference_handler.py`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/__init__.py` & `sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/__init__.py`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/src/sagemaker_pytorch_serving_container/etc/log4j2.xml` & `sagemaker_pytorch_inference-2.0.9/src/sagemaker_pytorch_serving_container/etc/log4j2.xml`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/setup.py` & `sagemaker_pytorch_inference-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/LICENSE` & `sagemaker_pytorch_inference-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sagemaker_pytorch_inference-2.0.8/PKG-INFO` & `sagemaker_pytorch_inference-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sagemaker_pytorch_inference
-Version: 2.0.8
+Version: 2.0.9
 Summary: Open source library for creating PyTorch containers to run on Amazon SageMaker.
 Home-page: https://github.com/aws/sagemaker-pytorch-inference-toolkit
 Author: Amazon Web Services
 License: Apache License 2.0
 Description: ===================================
         SageMaker PyTorch Inference Toolkit
         ===================================
```


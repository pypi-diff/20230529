# Comparing `tmp/cdk8s-plus-25-2.8.4.tar.gz` & `tmp/cdk8s-plus-25-2.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-25-2.8.4.tar", last modified: Sun May 28 02:39:00 2023, max compression
+gzip compressed data, was "cdk8s-plus-25-2.8.5.tar", last modified: Mon May 29 02:35:14 2023, max compression
```

## Comparing `cdk8s-plus-25-2.8.4.tar` & `cdk8s-plus-25-2.8.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:39:00.742215 cdk8s-plus-25-2.8.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-28 02:39:00.742215 cdk8s-plus-25-2.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 02:39:00.742215 cdk8s-plus-25-2.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:39:00.734215 cdk8s-plus-25-2.8.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:39:00.738215 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25/
--rw-r--r--   0 runner    (1001) docker     (123)  1161508 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:39:00.738215 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1254800 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25/_jsii/cdk8s-plus-25@2.8.4.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:39:00.738215 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)  2644402 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 02:38:48.000000 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 02:39:00.738215 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-28 02:39:00.000000 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-28 02:39:00.000000 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 02:39:00.000000 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-28 02:39:00.000000 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-28 02:39:00.000000 cdk8s-plus-25-2.8.4/src/cdk8s_plus_25.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:35:14.785934 cdk8s-plus-25-2.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-29 02:35:14.781934 cdk8s-plus-25-2.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:35:14.785934 cdk8s-plus-25-2.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:35:14.777934 cdk8s-plus-25-2.8.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:35:14.777934 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25/
+-rw-r--r--   0 runner    (1001) docker     (123)  1161508 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:35:14.781934 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1254800 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25/_jsii/cdk8s-plus-25@2.8.5.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:35:14.781934 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)  2644402 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:35:03.000000 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:35:14.777934 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-29 02:35:14.000000 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-29 02:35:14.000000 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:35:14.000000 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-29 02:35:14.000000 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 02:35:14.000000 cdk8s-plus-25-2.8.5/src/cdk8s_plus_25.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-25-2.8.4/LICENSE` & `cdk8s-plus-25-2.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-25-2.8.4/PKG-INFO` & `cdk8s-plus-25-2.8.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-25
-Version: 2.8.4
+Version: 2.8.5
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-25 synthesizes Kubernetes manifests for Kubernetes 1.25.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-25-2.8.4/README.md` & `cdk8s-plus-25-2.8.5/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-25-2.8.4/setup.py` & `cdk8s-plus-25-2.8.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-25",
-    "version": "2.8.4",
+    "version": "2.8.5",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-25 synthesizes Kubernetes manifests for Kubernetes 1.25.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,24 +23,24 @@
     "packages": [
         "cdk8s_plus_25",
         "cdk8s_plus_25._jsii",
         "cdk8s_plus_25.k8s"
     ],
     "package_data": {
         "cdk8s_plus_25._jsii": [
-            "cdk8s-plus-25@2.8.4.jsii.tgz"
+            "cdk8s-plus-25@2.8.5.jsii.tgz"
         ],
         "cdk8s_plus_25": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "cdk8s>=2.7.75, <3.0.0",
-        "constructs>=10.2.35, <11.0.0",
+        "constructs>=10.2.36, <11.0.0",
         "jsii>=1.82.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
```

### Comparing `cdk8s-plus-25-2.8.4/src/cdk8s_plus_25/__init__.py` & `cdk8s-plus-25-2.8.5/src/cdk8s_plus_25/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-25-2.8.4/src/cdk8s_plus_25/k8s/__init__.py` & `cdk8s-plus-25-2.8.5/src/cdk8s_plus_25/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-25-2.8.4/src/cdk8s_plus_25.egg-info/PKG-INFO` & `cdk8s-plus-25-2.8.5/src/cdk8s_plus_25.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-25
-Version: 2.8.4
+Version: 2.8.5
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-25 synthesizes Kubernetes manifests for Kubernetes 1.25.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


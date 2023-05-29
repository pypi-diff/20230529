# Comparing `tmp/semi-tensor-product-0.0.2.tar.gz` & `tmp/semi-tensor-product-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\ProgramData\STP\numpy\dist\.tmp-ytpxht46\semi-tensor-product-0.0.2.tar", last modified: Mon May 29 11:15:18 2023, max compression
+gzip compressed data, was "D:\ProgramData\STP\stp\dist\.tmp-qhrvf6t5\semi-tensor-product-0.0.3.tar", last modified: Mon May 29 11:20:25 2023, max compression
```

## Comparing `semi-tensor-product-0.0.2.tar` & `semi-tensor-product-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 11:15:18.238330 semi-tensor-product-0.0.2/
--rw-rw-rw-   0        0        0     1068 2023-05-29 08:03:33.000000 semi-tensor-product-0.0.2/LICENSES
--rw-rw-rw-   0        0        0      662 2023-05-29 11:15:18.238330 semi-tensor-product-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      126 2023-05-29 08:17:04.000000 semi-tensor-product-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 11:15:18.232373 semi-tensor-product-0.0.2/STP/
-drwxrwxrwx   0        0        0        0 2023-05-29 11:15:18.237333 semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/
--rw-rw-rw-   0        0        0      662 2023-05-29 11:15:18.000000 semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-29 11:15:18.000000 semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 11:15:18.000000 semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 11:15:18.000000 semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-29 08:04:17.000000 semi-tensor-product-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 11:15:18.238330 semi-tensor-product-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-05-29 11:14:44.000000 semi-tensor-product-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:20:25.031207 semi-tensor-product-0.0.3/
+-rw-rw-rw-   0        0        0     1068 2023-05-29 08:03:33.000000 semi-tensor-product-0.0.3/LICENSES
+-rw-rw-rw-   0        0        0      662 2023-05-29 11:20:25.030210 semi-tensor-product-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2023-05-29 08:17:04.000000 semi-tensor-product-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 11:20:25.025223 semi-tensor-product-0.0.3/STP/
+drwxrwxrwx   0        0        0        0 2023-05-29 11:20:25.030210 semi-tensor-product-0.0.3/STP/semi_tensor_product.egg-info/
+-rw-rw-rw-   0        0        0      662 2023-05-29 11:20:25.000000 semi-tensor-product-0.0.3/STP/semi_tensor_product.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-05-29 11:20:25.000000 semi-tensor-product-0.0.3/STP/semi_tensor_product.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 11:20:25.000000 semi-tensor-product-0.0.3/STP/semi_tensor_product.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 11:20:25.000000 semi-tensor-product-0.0.3/STP/semi_tensor_product.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-29 08:04:17.000000 semi-tensor-product-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 11:20:25.031207 semi-tensor-product-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-05-29 11:19:46.000000 semi-tensor-product-0.0.3/setup.py
```

### Comparing `semi-tensor-product-0.0.2/LICENSES` & `semi-tensor-product-0.0.3/LICENSES`

 * *Files identical despite different names*

### Comparing `semi-tensor-product-0.0.2/PKG-INFO` & `semi-tensor-product-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semi-tensor-product
-Version: 0.0.2
+Version: 0.0.3
 Summary: STP Toolbox for Python
 Home-page: https://github.com/huanianss/semi-tensor-product
 Author: Huanianss
 Author-email: huanianss@qq.com
 Project-URL: Bug Tracker, https://github.com/huanianss/semi-tensor-product/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/PKG-INFO` & `semi-tensor-product-0.0.3/STP/semi_tensor_product.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semi-tensor-product
-Version: 0.0.2
+Version: 0.0.3
 Summary: STP Toolbox for Python
 Home-page: https://github.com/huanianss/semi-tensor-product
 Author: Huanianss
 Author-email: huanianss@qq.com
 Project-URL: Bug Tracker, https://github.com/huanianss/semi-tensor-product/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `semi-tensor-product-0.0.2/setup.py` & `semi-tensor-product-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="semi-tensor-product",
-    version="0.0.2",
+    version="0.0.3",
     author="Huanianss",
     author_email="huanianss@qq.com",
     description="STP Toolbox for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanianss/semi-tensor-product",
     project_urls={
```


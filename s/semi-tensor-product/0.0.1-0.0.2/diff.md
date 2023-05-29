# Comparing `tmp/semi-tensor-product-0.0.1.tar.gz` & `tmp/semi-tensor-product-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\ProgramData\STP\semi-tensor-product\dist\.tmp-nl896_up\semi-tensor-product-0.0.1.tar", last modified: Mon May 29 09:48:36 2023, max compression
+gzip compressed data, was "D:\ProgramData\STP\numpy\dist\.tmp-ytpxht46\semi-tensor-product-0.0.2.tar", last modified: Mon May 29 11:15:18 2023, max compression
```

## Comparing `semi-tensor-product-0.0.1.tar` & `semi-tensor-product-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 09:48:36.657992 semi-tensor-product-0.0.1/
--rw-rw-rw-   0        0        0     1068 2023-05-29 08:03:33.000000 semi-tensor-product-0.0.1/LICENSES
--rw-rw-rw-   0        0        0      662 2023-05-29 09:48:36.656995 semi-tensor-product-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      126 2023-05-29 08:17:04.000000 semi-tensor-product-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 09:48:36.652009 semi-tensor-product-0.0.1/STP/
-drwxrwxrwx   0        0        0        0 2023-05-29 09:48:36.656995 semi-tensor-product-0.0.1/STP/semi_tensor_product.egg-info/
--rw-rw-rw-   0        0        0      662 2023-05-29 09:48:36.000000 semi-tensor-product-0.0.1/STP/semi_tensor_product.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-05-29 09:48:36.000000 semi-tensor-product-0.0.1/STP/semi_tensor_product.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 09:48:36.000000 semi-tensor-product-0.0.1/STP/semi_tensor_product.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 09:48:36.000000 semi-tensor-product-0.0.1/STP/semi_tensor_product.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-29 08:04:17.000000 semi-tensor-product-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 09:48:36.657992 semi-tensor-product-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      865 2023-05-29 09:45:44.000000 semi-tensor-product-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:15:18.238330 semi-tensor-product-0.0.2/
+-rw-rw-rw-   0        0        0     1068 2023-05-29 08:03:33.000000 semi-tensor-product-0.0.2/LICENSES
+-rw-rw-rw-   0        0        0      662 2023-05-29 11:15:18.238330 semi-tensor-product-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2023-05-29 08:17:04.000000 semi-tensor-product-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 11:15:18.232373 semi-tensor-product-0.0.2/STP/
+drwxrwxrwx   0        0        0        0 2023-05-29 11:15:18.237333 semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/
+-rw-rw-rw-   0        0        0      662 2023-05-29 11:15:18.000000 semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-05-29 11:15:18.000000 semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 11:15:18.000000 semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 11:15:18.000000 semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-05-29 08:04:17.000000 semi-tensor-product-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 11:15:18.238330 semi-tensor-product-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      865 2023-05-29 11:14:44.000000 semi-tensor-product-0.0.2/setup.py
```

### Comparing `semi-tensor-product-0.0.1/LICENSES` & `semi-tensor-product-0.0.2/LICENSES`

 * *Files identical despite different names*

### Comparing `semi-tensor-product-0.0.1/PKG-INFO` & `semi-tensor-product-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semi-tensor-product
-Version: 0.0.1
+Version: 0.0.2
 Summary: STP Toolbox for Python
 Home-page: https://github.com/huanianss/semi-tensor-product
 Author: Huanianss
 Author-email: huanianss@qq.com
 Project-URL: Bug Tracker, https://github.com/huanianss/semi-tensor-product/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `semi-tensor-product-0.0.1/STP/semi_tensor_product.egg-info/PKG-INFO` & `semi-tensor-product-0.0.2/STP/semi_tensor_product.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semi-tensor-product
-Version: 0.0.1
+Version: 0.0.2
 Summary: STP Toolbox for Python
 Home-page: https://github.com/huanianss/semi-tensor-product
 Author: Huanianss
 Author-email: huanianss@qq.com
 Project-URL: Bug Tracker, https://github.com/huanianss/semi-tensor-product/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `semi-tensor-product-0.0.1/setup.py` & `semi-tensor-product-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="semi-tensor-product",
-    version="0.0.1",
+    version="0.0.2",
     author="Huanianss",
     author_email="huanianss@qq.com",
     description="STP Toolbox for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanianss/semi-tensor-product",
     project_urls={
```


# Comparing `tmp/semiTensorProduct-0.0.1.tar.gz` & `tmp/semiTensorProduct-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\ProgramData\STP\stp\dist\.tmp-jqekjjdn\semiTensorProduct-0.0.1.tar", last modified: Mon May 29 11:29:47 2023, max compression
+gzip compressed data, was "D:\ProgramData\STP\stp\dist\.tmp-6bvuaiyl\semiTensorProduct-0.0.2.tar", last modified: Mon May 29 11:59:57 2023, max compression
```

## Comparing `semiTensorProduct-0.0.1.tar` & `semiTensorProduct-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 11:29:47.129765 semiTensorProduct-0.0.1/
--rw-rw-rw-   0        0        0     1068 2023-05-29 08:03:33.000000 semiTensorProduct-0.0.1/LICENSES
--rw-rw-rw-   0        0        0      660 2023-05-29 11:29:47.128797 semiTensorProduct-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      126 2023-05-29 08:17:04.000000 semiTensorProduct-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 11:29:47.119793 semiTensorProduct-0.0.1/STP/
-drwxrwxrwx   0        0        0        0 2023-05-29 11:29:47.127798 semiTensorProduct-0.0.1/STP/semiTensorProduct.egg-info/
--rw-rw-rw-   0        0        0      660 2023-05-29 11:29:47.000000 semiTensorProduct-0.0.1/STP/semiTensorProduct.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-29 11:29:47.000000 semiTensorProduct-0.0.1/STP/semiTensorProduct.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 11:29:47.000000 semiTensorProduct-0.0.1/STP/semiTensorProduct.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 11:29:47.000000 semiTensorProduct-0.0.1/STP/semiTensorProduct.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-05-29 08:04:17.000000 semiTensorProduct-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 11:29:47.129765 semiTensorProduct-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      863 2023-05-29 11:29:03.000000 semiTensorProduct-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:57.425059 semiTensorProduct-0.0.2/
+-rw-rw-rw-   0        0        0     1068 2023-05-29 08:03:33.000000 semiTensorProduct-0.0.2/LICENSES
+-rw-rw-rw-   0        0        0      660 2023-05-29 11:59:57.424062 semiTensorProduct-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      126 2023-05-29 08:17:04.000000 semiTensorProduct-0.0.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-05-29 08:04:17.000000 semiTensorProduct-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 11:59:57.425059 semiTensorProduct-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      863 2023-05-29 11:55:39.000000 semiTensorProduct-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:57.416084 semiTensorProduct-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:57.422068 semiTensorProduct-0.0.2/src/semiTensorProduct.egg-info/
+-rw-rw-rw-   0        0        0      660 2023-05-29 11:59:57.000000 semiTensorProduct-0.0.2/src/semiTensorProduct.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2023-05-29 11:59:57.000000 semiTensorProduct-0.0.2/src/semiTensorProduct.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 11:59:57.000000 semiTensorProduct-0.0.2/src/semiTensorProduct.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-29 11:59:57.000000 semiTensorProduct-0.0.2/src/semiTensorProduct.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 11:59:57.423065 semiTensorProduct-0.0.2/src/stp/
+-rw-rw-rw-   0        0        0       42 2023-05-29 07:54:11.000000 semiTensorProduct-0.0.2/src/stp/__init__.py
+-rw-rw-rw-   0        0        0     2720 2023-05-29 07:50:50.000000 semiTensorProduct-0.0.2/src/stp/stp.py
+-rw-rw-rw-   0        0        0     7994 2023-05-29 07:44:58.000000 semiTensorProduct-0.0.2/src/stp/utils.py
```

### Comparing `semiTensorProduct-0.0.1/LICENSES` & `semiTensorProduct-0.0.2/LICENSES`

 * *Files identical despite different names*

### Comparing `semiTensorProduct-0.0.1/PKG-INFO` & `semiTensorProduct-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semiTensorProduct
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

### Comparing `semiTensorProduct-0.0.1/STP/semiTensorProduct.egg-info/PKG-INFO` & `semiTensorProduct-0.0.2/src/semiTensorProduct.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semiTensorProduct
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

### Comparing `semiTensorProduct-0.0.1/setup.py` & `semiTensorProduct-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="semiTensorProduct",
-    version="0.0.1",
+    version="0.0.2",
     author="Huanianss",
     author_email="huanianss@qq.com",
     description="STP Toolbox for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/huanianss/semi-tensor-product",
     project_urls={
         "Bug Tracker": "https://github.com/huanianss/semi-tensor-product/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    package_dir={"": "STP"},
-    packages=setuptools.find_packages(where="STP"),
+    package_dir={"": "src"},
+    packages=setuptools.find_packages(where="src"),
     python_requires=">=3.6",
     )
```


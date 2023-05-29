# Comparing `tmp/tronapi-JCO-3.1.8.tar.gz` & `tmp/tronapi-JCO-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tronapi-JCO-3.1.8.tar", last modified: Tue Apr 25 11:06:52 2023, max compression
+gzip compressed data, was "tronapi-JCO-3.1.9.tar", last modified: Tue Apr 25 11:12:01 2023, max compression
```

## Comparing `tronapi-JCO-3.1.8.tar` & `tronapi-JCO-3.1.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.881456 tronapi-JCO-3.1.8/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1064 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/LICENSE
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5373 2023-04-25 11:06:52.881309 tronapi-JCO-3.1.8/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4590 2023-04-21 10:07:20.000000 tronapi-JCO-3.1.8/README.rst
--rw-r--r--   0 rustinsoraki   (501) staff       (20)       38 2023-04-25 11:06:52.881494 tronapi-JCO-3.1.8/setup.cfg
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3126 2023-04-25 11:06:50.000000 tronapi-JCO-3.1.8/setup.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.875629 tronapi-JCO-3.1.8/tronapi/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      716 2023-04-24 14:21:45.000000 tronapi-JCO-3.1.8/tronapi/__init__.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.879514 tronapi-JCO-3.1.8/tronapi/common/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    15063 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/abi.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3192 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/account.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1328 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/blocks.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4862 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/contracts.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     6408 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/datastructures.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1520 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/datatypes.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     7948 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/encoding.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1781 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/formatters.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1820 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/normalizers.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     3280 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/threads.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.879727 tronapi-JCO-3.1.8/tronapi/common/toolz/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1013 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/toolz/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/transactions.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     6614 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/common/validation.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      582 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/constants.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    12561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/contract.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     2329 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/exceptions.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    11311 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/main.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4231 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/manager.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1009 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/module.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.880192 tronapi-JCO-3.1.8/tronapi/providers/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/providers/__init__.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     1382 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/providers/base.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     4661 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.8/tronapi/providers/http.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    43709 2023-04-25 11:06:34.000000 tronapi-JCO-3.1.8/tronapi/transactionbuilder.py
--rw-r--r--   0 rustinsoraki   (501) staff       (20)    34240 2023-04-25 09:59:51.000000 tronapi-JCO-3.1.8/tronapi/trx.py
-drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:06:52.881133 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/
--rw-r--r--   0 rustinsoraki   (501) staff       (20)     5373 2023-04-25 11:06:52.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/PKG-INFO
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      892 2023-04-25 11:06:52.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/SOURCES.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-25 11:06:52.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/dependency_links.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/not-zip-safe
--rw-r--r--   0 rustinsoraki   (501) staff       (20)      974 2023-04-25 11:06:52.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/requires.txt
--rw-r--r--   0 rustinsoraki   (501) staff       (20)        8 2023-04-25 11:06:52.000000 tronapi-JCO-3.1.8/tronapi_JCO.egg-info/top_level.txt
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:12:01.188912 tronapi-JCO-3.1.9/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1064 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/LICENSE
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5373 2023-04-25 11:12:01.188770 tronapi-JCO-3.1.9/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4590 2023-04-21 10:07:20.000000 tronapi-JCO-3.1.9/README.rst
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)       38 2023-04-25 11:12:01.188954 tronapi-JCO-3.1.9/setup.cfg
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3126 2023-04-25 11:11:58.000000 tronapi-JCO-3.1.9/setup.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:12:01.184448 tronapi-JCO-3.1.9/tronapi/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      716 2023-04-24 14:21:45.000000 tronapi-JCO-3.1.9/tronapi/__init__.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:12:01.186878 tronapi-JCO-3.1.9/tronapi/common/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    15063 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/abi.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3192 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/account.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1328 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/blocks.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4862 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/contracts.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     6408 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/datastructures.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1520 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/datatypes.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     7948 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/encoding.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1781 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/formatters.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1820 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/normalizers.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     3280 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/threads.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:12:01.187031 tronapi-JCO-3.1.9/tronapi/common/toolz/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1013 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/toolz/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/transactions.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     6614 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/common/validation.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      582 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/constants.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    12561 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/contract.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     2329 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/exceptions.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    11311 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/main.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4231 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/manager.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1009 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/module.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:12:01.187553 tronapi-JCO-3.1.9/tronapi/providers/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        0 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/providers/__init__.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     1382 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/providers/base.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     4661 2023-04-18 11:45:17.000000 tronapi-JCO-3.1.9/tronapi/providers/http.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    43741 2023-04-25 11:11:46.000000 tronapi-JCO-3.1.9/tronapi/transactionbuilder.py
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)    34240 2023-04-25 09:59:51.000000 tronapi-JCO-3.1.9/tronapi/trx.py
+drwxr-xr-x   0 rustinsoraki   (501) staff       (20)        0 2023-04-25 11:12:01.188575 tronapi-JCO-3.1.9/tronapi_JCO.egg-info/
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)     5373 2023-04-25 11:12:01.000000 tronapi-JCO-3.1.9/tronapi_JCO.egg-info/PKG-INFO
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      892 2023-04-25 11:12:01.000000 tronapi-JCO-3.1.9/tronapi_JCO.egg-info/SOURCES.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-25 11:12:01.000000 tronapi-JCO-3.1.9/tronapi_JCO.egg-info/dependency_links.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        1 2023-04-21 10:05:40.000000 tronapi-JCO-3.1.9/tronapi_JCO.egg-info/not-zip-safe
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)      974 2023-04-25 11:12:01.000000 tronapi-JCO-3.1.9/tronapi_JCO.egg-info/requires.txt
+-rw-r--r--   0 rustinsoraki   (501) staff       (20)        8 2023-04-25 11:12:01.000000 tronapi-JCO-3.1.9/tronapi_JCO.egg-info/top_level.txt
```

### Comparing `tronapi-JCO-3.1.8/LICENSE` & `tronapi-JCO-3.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/PKG-INFO` & `tronapi-JCO-3.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tronapi-JCO
-Version: 3.1.8
+Version: 3.1.9
 Summary: A Python API for interacting with Tron (Forked from tronapi)
 Home-page: https://github.com/RastinS/tron-api-JCO
 Author: Rustin Soraki
 Author-email: rustin.souraki@gmail.com
 License: MIT License
 Keywords: tron tron-api tron-api-python iexbase
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tronapi-JCO-3.1.8/README.rst` & `tronapi-JCO-3.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/setup.py` & `tronapi-JCO-3.1.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from setuptools import (
     find_packages,
     setup,
 )
 
 py_version = platform.python_version()
 
-PACKAGE_VERSION = "3.1.8"
+PACKAGE_VERSION = "3.1.9"
 
 EXTRAS_REQUIRE = {
     "tester": ["coverage", "pep8", "pyflakes", "pylint", "pytest-cov"],
     "docs": [
         "mock",
         "sphinx-better-theme>=0.1.4",
         "click>=5.1",
```

### Comparing `tronapi-JCO-3.1.8/tronapi/__init__.py` & `tronapi-JCO-3.1.9/tronapi/__init__.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/abi.py` & `tronapi-JCO-3.1.9/tronapi/common/abi.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/account.py` & `tronapi-JCO-3.1.9/tronapi/common/account.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/blocks.py` & `tronapi-JCO-3.1.9/tronapi/common/blocks.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/contracts.py` & `tronapi-JCO-3.1.9/tronapi/common/contracts.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/datastructures.py` & `tronapi-JCO-3.1.9/tronapi/common/datastructures.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/datatypes.py` & `tronapi-JCO-3.1.9/tronapi/common/datatypes.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/encoding.py` & `tronapi-JCO-3.1.9/tronapi/common/encoding.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/formatters.py` & `tronapi-JCO-3.1.9/tronapi/common/formatters.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/normalizers.py` & `tronapi-JCO-3.1.9/tronapi/common/normalizers.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/threads.py` & `tronapi-JCO-3.1.9/tronapi/common/threads.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/toolz/__init__.py` & `tronapi-JCO-3.1.9/tronapi/common/toolz/__init__.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/transactions.py` & `tronapi-JCO-3.1.9/tronapi/common/transactions.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/common/validation.py` & `tronapi-JCO-3.1.9/tronapi/common/validation.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/constants.py` & `tronapi-JCO-3.1.9/tronapi/constants.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/contract.py` & `tronapi-JCO-3.1.9/tronapi/contract.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/exceptions.py` & `tronapi-JCO-3.1.9/tronapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/main.py` & `tronapi-JCO-3.1.9/tronapi/main.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/manager.py` & `tronapi-JCO-3.1.9/tronapi/manager.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/module.py` & `tronapi-JCO-3.1.9/tronapi/module.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/providers/base.py` & `tronapi-JCO-3.1.9/tronapi/providers/base.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/providers/http.py` & `tronapi-JCO-3.1.9/tronapi/providers/http.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi/transactionbuilder.py` & `tronapi-JCO-3.1.9/tronapi/transactionbuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,16 +38,17 @@
         # If the address of the sender is not specified, we prescribe the default
         if account is None:
             account = self.tron.default_address.hex
 
         if not self.tron.isAddress(to):
             raise InvalidTronError("Invalid recipient address provided")
 
-        if not isinstance(amount, float) or not isinstance(amount, int) or amount <= 0:
-            raise InvalidTronError("Invalid amount provided")
+        if not isinstance(amount, float) or amount <= 0:
+            if not isinstance(amount, int) or amount <= 0:
+                raise InvalidTronError("Invalid amount provided")
 
         _to = self.tron.address.to_hex(to)
         _from = self.tron.address.to_hex(account)
 
         if _to == _from:
             raise TronError("Cannot transfer TRX to the same account")
```

### Comparing `tronapi-JCO-3.1.8/tronapi/trx.py` & `tronapi-JCO-3.1.9/tronapi/trx.py`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi_JCO.egg-info/PKG-INFO` & `tronapi-JCO-3.1.9/tronapi_JCO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tronapi-JCO
-Version: 3.1.8
+Version: 3.1.9
 Summary: A Python API for interacting with Tron (Forked from tronapi)
 Home-page: https://github.com/RastinS/tron-api-JCO
 Author: Rustin Soraki
 Author-email: rustin.souraki@gmail.com
 License: MIT License
 Keywords: tron tron-api tron-api-python iexbase
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `tronapi-JCO-3.1.8/tronapi_JCO.egg-info/SOURCES.txt` & `tronapi-JCO-3.1.9/tronapi_JCO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tronapi-JCO-3.1.8/tronapi_JCO.egg-info/requires.txt` & `tronapi-JCO-3.1.9/tronapi_JCO.egg-info/requires.txt`

 * *Files identical despite different names*


# Comparing `tmp/cs-binance-c2c-sapi-0.0.1.tar.gz` & `tmp/cs-binance-c2c-sapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-binance-c2c-sapi-0.0.1.tar", last modified: Mon May 29 06:45:31 2023, max compression
+gzip compressed data, was "cs-binance-c2c-sapi-0.0.2.tar", last modified: Mon May 29 06:52:01 2023, max compression
```

## Comparing `cs-binance-c2c-sapi-0.0.1.tar` & `cs-binance-c2c-sapi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 06:45:31.573123 cs-binance-c2c-sapi-0.0.1/
--rw-rw-rw-   0        0        0      606 2023-05-29 06:45:31.562661 cs-binance-c2c-sapi-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 cs-binance-c2c-sapi-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 06:45:31.524706 cs-binance-c2c-sapi-0.0.1/binance_c2c/
--rw-rw-rw-   0        0        0       26 2023-05-28 18:32:30.000000 cs-binance-c2c-sapi-0.0.1/binance_c2c/__init__.py
--rw-rw-rw-   0        0        0     7386 2023-05-29 06:32:10.000000 cs-binance-c2c-sapi-0.0.1/binance_c2c/api.py
-drwxrwxrwx   0        0        0        0 2023-05-29 06:45:31.562661 cs-binance-c2c-sapi-0.0.1/cs_binance_c2c_sapi.egg-info/
--rw-rw-rw-   0        0        0      606 2023-05-29 06:45:31.000000 cs-binance-c2c-sapi-0.0.1/cs_binance_c2c_sapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      275 2023-05-29 06:45:31.000000 cs-binance-c2c-sapi-0.0.1/cs_binance_c2c_sapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 06:45:31.000000 cs-binance-c2c-sapi-0.0.1/cs_binance_c2c_sapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 06:45:31.000000 cs-binance-c2c-sapi-0.0.1/cs_binance_c2c_sapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 06:45:31.000000 cs-binance-c2c-sapi-0.0.1/cs_binance_c2c_sapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 06:45:31.573123 cs-binance-c2c-sapi-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1112 2023-05-29 06:45:18.000000 cs-binance-c2c-sapi-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 06:52:01.314126 cs-binance-c2c-sapi-0.0.2/
+-rw-rw-rw-   0        0        0      606 2023-05-29 06:52:01.307834 cs-binance-c2c-sapi-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1210 2023-05-28 18:45:08.000000 cs-binance-c2c-sapi-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 06:52:01.277746 cs-binance-c2c-sapi-0.0.2/binance_c2c/
+-rw-rw-rw-   0        0        0       27 2023-05-29 06:50:57.000000 cs-binance-c2c-sapi-0.0.2/binance_c2c/__init__.py
+-rw-rw-rw-   0        0        0     7386 2023-05-29 06:32:10.000000 cs-binance-c2c-sapi-0.0.2/binance_c2c/api.py
+drwxrwxrwx   0        0        0        0 2023-05-29 06:52:01.307834 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/
+-rw-rw-rw-   0        0        0      606 2023-05-29 06:52:01.000000 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      275 2023-05-29 06:52:01.000000 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 06:52:01.000000 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 06:52:01.000000 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-29 06:52:01.000000 cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 06:52:01.314126 cs-binance-c2c-sapi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1112 2023-05-29 06:51:57.000000 cs-binance-c2c-sapi-0.0.2/setup.py
```

### Comparing `cs-binance-c2c-sapi-0.0.1/PKG-INFO` & `cs-binance-c2c-sapi-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.1/README.md` & `cs-binance-c2c-sapi-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cs-binance-c2c-sapi-0.0.1/binance_c2c/api.py` & `cs-binance-c2c-sapi-0.0.2/binance_c2c/api.py`

 * *Files identical despite different names*

### Comparing `cs-binance-c2c-sapi-0.0.1/cs_binance_c2c_sapi.egg-info/PKG-INFO` & `cs-binance-c2c-sapi-0.0.2/cs_binance_c2c_sapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs-binance-c2c-sapi
-Version: 0.0.1
+Version: 0.0.2
 Summary: Binance C2C SAPI Wrapper
 Author: Richard
 Author-email: <rich_swainson@hotmail.co.uk>
 Keywords: binance,api,wrapper,c2c,sapi
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cs-binance-c2c-sapi-0.0.1/setup.py` & `cs-binance-c2c-sapi-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Binance C2C SAPI Wrapper'
 LONG_DESCRIPTION = 'A Python wrapper for the Binance C2C (Customer-to-Customer) SAPI.'
 
 # Setting up
 setup(
     name="cs-binance-c2c-sapi",
     version=VERSION,
```


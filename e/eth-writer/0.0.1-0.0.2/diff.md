# Comparing `tmp/eth-writer-0.0.1.tar.gz` & `tmp/eth-writer-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-writer-0.0.1.tar", last modified: Sat May 13 19:33:29 2023, max compression
+gzip compressed data, was "eth-writer-0.0.2.tar", last modified: Mon May 29 12:11:53 2023, max compression
```

## Comparing `eth-writer-0.0.1.tar` & `eth-writer-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-13 19:33:29.173323 eth-writer-0.0.1/
--rw-r--r--   0 lash      (1000) lash      (1000)     3216 2023-05-08 16:19:25.000000 eth-writer-0.0.1/LICENSE
--rw-r--r--   0 lash      (1000) lash      (1000)      722 2023-05-13 19:33:29.173323 eth-writer-0.0.1/PKG-INFO
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-13 19:33:29.173323 eth-writer-0.0.1/eth_writer/
--rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-05-10 17:28:14.000000 eth-writer-0.0.1/eth_writer/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-05-10 17:49:05.000000 eth-writer-0.0.1/eth_writer/interface.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-13 19:33:29.173323 eth-writer-0.0.1/eth_writer/unittest/
--rw-r--r--   0 lash      (1000) lash      (1000)       41 2023-05-10 07:06:19.000000 eth-writer-0.0.1/eth_writer/unittest/__init__.py
--rw-r--r--   0 lash      (1000) lash      (1000)     1650 2023-05-13 14:56:28.000000 eth-writer-0.0.1/eth_writer/unittest/base.py
-drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-13 19:33:29.173323 eth-writer-0.0.1/eth_writer.egg-info/
--rw-r--r--   0 lash      (1000) lash      (1000)      722 2023-05-13 19:33:29.000000 eth-writer-0.0.1/eth_writer.egg-info/PKG-INFO
--rw-r--r--   0 lash      (1000) lash      (1000)      302 2023-05-13 19:33:29.000000 eth-writer-0.0.1/eth_writer.egg-info/SOURCES.txt
--rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-13 19:33:29.000000 eth-writer-0.0.1/eth_writer.egg-info/dependency_links.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-05-13 19:33:29.000000 eth-writer-0.0.1/eth_writer.egg-info/requires.txt
--rw-r--r--   0 lash      (1000) lash      (1000)       11 2023-05-13 19:33:29.000000 eth-writer-0.0.1/eth_writer.egg-info/top_level.txt
--rw-r--r--   0 lash      (1000) lash      (1000)      779 2023-05-13 19:33:29.173323 eth-writer-0.0.1/setup.cfg
--rw-r--r--   0 lash      (1000) lash      (1000)      642 2023-05-08 16:19:19.000000 eth-writer-0.0.1/setup.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-29 12:11:53.396647 eth-writer-0.0.2/
+-rw-r--r--   0 lash      (1000) lash      (1000)     3216 2023-05-08 16:19:25.000000 eth-writer-0.0.2/LICENSE
+-rw-r--r--   0 lash      (1000) lash      (1000)       42 2023-05-29 12:11:06.000000 eth-writer-0.0.2/MANIFEST.in
+-rw-r--r--   0 lash      (1000) lash      (1000)      722 2023-05-29 12:11:53.396647 eth-writer-0.0.2/PKG-INFO
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-29 12:11:53.393314 eth-writer-0.0.2/eth_writer/
+-rw-r--r--   0 lash      (1000) lash      (1000)       25 2023-05-10 17:28:14.000000 eth-writer-0.0.2/eth_writer/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1753 2023-05-10 17:49:05.000000 eth-writer-0.0.2/eth_writer/interface.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-29 12:11:53.396647 eth-writer-0.0.2/eth_writer/unittest/
+-rw-r--r--   0 lash      (1000) lash      (1000)       41 2023-05-10 07:06:19.000000 eth-writer-0.0.2/eth_writer/unittest/__init__.py
+-rw-r--r--   0 lash      (1000) lash      (1000)     1650 2023-05-13 14:56:28.000000 eth-writer-0.0.2/eth_writer/unittest/base.py
+drwxr-xr-x   0 lash      (1000) lash      (1000)        0 2023-05-29 12:11:53.393314 eth-writer-0.0.2/eth_writer.egg-info/
+-rw-r--r--   0 lash      (1000) lash      (1000)      722 2023-05-29 12:11:53.000000 eth-writer-0.0.2/eth_writer.egg-info/PKG-INFO
+-rw-r--r--   0 lash      (1000) lash      (1000)      353 2023-05-29 12:11:53.000000 eth-writer-0.0.2/eth_writer.egg-info/SOURCES.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)        1 2023-05-29 12:11:53.000000 eth-writer-0.0.2/eth_writer.egg-info/dependency_links.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-05-29 12:11:53.000000 eth-writer-0.0.2/eth_writer.egg-info/requires.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       11 2023-05-29 12:11:53.000000 eth-writer-0.0.2/eth_writer.egg-info/top_level.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)       21 2023-05-13 14:51:46.000000 eth-writer-0.0.2/requirements.txt
+-rw-r--r--   0 lash      (1000) lash      (1000)      779 2023-05-29 12:11:53.396647 eth-writer-0.0.2/setup.cfg
+-rw-r--r--   0 lash      (1000) lash      (1000)      642 2023-05-08 16:19:19.000000 eth-writer-0.0.2/setup.py
+-rw-r--r--   0 lash      (1000) lash      (1000)       58 2023-05-10 06:58:28.000000 eth-writer-0.0.2/test_requirements.txt
```

### Comparing `eth-writer-0.0.1/LICENSE` & `eth-writer-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-writer-0.0.1/PKG-INFO` & `eth-writer-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-writer
-Version: 0.0.1
+Version: 0.0.2
 Summary: An interface for non-owner writer role to smart contract instance
 Home-page: https://holbrook.no/src/eth-writer/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-writer-0.0.1/eth_writer/interface.py` & `eth-writer-0.0.2/eth_writer/interface.py`

 * *Files identical despite different names*

### Comparing `eth-writer-0.0.1/eth_writer/unittest/base.py` & `eth-writer-0.0.2/eth_writer/unittest/base.py`

 * *Files identical despite different names*

### Comparing `eth-writer-0.0.1/eth_writer.egg-info/PKG-INFO` & `eth-writer-0.0.2/eth_writer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-writer
-Version: 0.0.1
+Version: 0.0.2
 Summary: An interface for non-owner writer role to smart contract instance
 Home-page: https://holbrook.no/src/eth-writer/log.html
 Author: Louis Holbrook
 Author-email: dev@holbrook.no
 License: GPL3
 Keywords: ethereum
 Classifier: Programming Language :: Python :: 3
```

### Comparing `eth-writer-0.0.1/setup.cfg` & `eth-writer-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = eth-writer
-version = 0.0.1
+version = 0.0.2
 description = An interface for non-owner writer role to smart contract instance
 author = Louis Holbrook
 author_email = dev@holbrook.no
 url = https://holbrook.no/src/eth-writer/log.html
 keywords = 
 	ethereum
 classifiers =
```

### Comparing `eth-writer-0.0.1/setup.py` & `eth-writer-0.0.2/setup.py`

 * *Files identical despite different names*


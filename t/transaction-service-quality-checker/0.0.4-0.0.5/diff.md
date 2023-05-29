# Comparing `tmp/transaction_service_quality_checker-0.0.4.tar.gz` & `tmp/transaction_service_quality_checker-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "transaction_service_quality_checker-0.0.4.tar", last modified: Mon May 29 15:40:55 2023, max compression
+gzip compressed data, was "transaction_service_quality_checker-0.0.5.tar", last modified: Mon May 29 16:44:46 2023, max compression
```

## Comparing `transaction_service_quality_checker-0.0.4.tar` & `transaction_service_quality_checker-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 15:40:55.705689 transaction_service_quality_checker-0.0.4/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      258 2023-05-29 15:40:55.705252 transaction_service_quality_checker-0.0.4/PKG-INFO
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1601 2023-05-10 16:34:46.000000 transaction_service_quality_checker-0.0.4/README.md
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)       38 2023-05-29 15:40:55.705864 transaction_service_quality_checker-0.0.4/setup.cfg
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      383 2023-05-29 12:59:03.000000 transaction_service_quality_checker-0.0.4/setup.py
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 15:40:55.692612 transaction_service_quality_checker-0.0.4/tests/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:26:08.000000 transaction_service_quality_checker-0.0.4/tests/__init__.py
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 15:40:55.693741 transaction_service_quality_checker-0.0.4/tests/api/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:26:10.000000 transaction_service_quality_checker-0.0.4/tests/api/__init__.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      960 2023-05-25 12:23:42.000000 transaction_service_quality_checker-0.0.4/tests/api/test_config_api_interface.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2317 2023-05-25 12:26:21.000000 transaction_service_quality_checker-0.0.4/tests/api/test_transaction_api_interface.py
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 15:40:55.698623 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-25 12:19:38.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/__init__.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      513 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/addresses_map.py
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 15:40:55.704438 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/api/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:25:46.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/api/__init__.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      425 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/api/api_interface.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      651 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/api/config_api_interface.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2395 2023-05-10 10:11:34.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/api/etherscan_api_interface.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1828 2023-05-03 11:00:35.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/api/transaction_api_interface.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1374 2023-05-23 18:18:38.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/app.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      525 2023-05-08 10:47:32.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/app_block_creation.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2494 2023-05-29 15:40:49.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/app_by_list.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1226 2023-05-29 13:33:48.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/block_creation.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)    13763 2023-05-29 13:21:40.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/comparer.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1948 2023-05-10 11:20:21.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/metrics.py
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     6320 2023-05-24 09:08:26.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/reindex_operator.py
-drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 15:40:55.701747 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker.egg-info/
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)      258 2023-05-29 15:40:55.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker.egg-info/PKG-INFO
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1144 2023-05-29 15:40:55.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker.egg-info/SOURCES.txt
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)        1 2023-05-29 15:40:55.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker.egg-info/dependency_links.txt
--rw-r--r--   0 joseramirezencinas   (501) staff       (20)       42 2023-05-29 15:40:55.000000 transaction_service_quality_checker-0.0.4/transaction_service_quality_checker.egg-info/top_level.txt
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 16:44:46.849212 transaction_service_quality_checker-0.0.5/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      258 2023-05-29 16:44:46.848655 transaction_service_quality_checker-0.0.5/PKG-INFO
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1601 2023-05-10 16:34:46.000000 transaction_service_quality_checker-0.0.5/README.md
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)       38 2023-05-29 16:44:46.849718 transaction_service_quality_checker-0.0.5/setup.cfg
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      383 2023-05-29 16:44:34.000000 transaction_service_quality_checker-0.0.5/setup.py
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 16:44:46.821570 transaction_service_quality_checker-0.0.5/tests/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:26:08.000000 transaction_service_quality_checker-0.0.5/tests/__init__.py
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 16:44:46.823682 transaction_service_quality_checker-0.0.5/tests/api/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:26:10.000000 transaction_service_quality_checker-0.0.5/tests/api/__init__.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      960 2023-05-25 12:23:42.000000 transaction_service_quality_checker-0.0.5/tests/api/test_config_api_interface.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2317 2023-05-25 12:26:21.000000 transaction_service_quality_checker-0.0.5/tests/api/test_transaction_api_interface.py
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 16:44:46.832286 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-25 12:19:38.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/__init__.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      513 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/addresses_map.py
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 16:44:46.847514 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/api/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)        0 2023-05-24 16:25:46.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/api/__init__.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      425 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/api/api_interface.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      651 2023-04-27 08:35:17.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/api/config_api_interface.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2395 2023-05-10 10:11:34.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/api/etherscan_api_interface.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1828 2023-05-03 11:00:35.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/api/transaction_api_interface.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1374 2023-05-23 18:18:38.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/app.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      525 2023-05-08 10:47:32.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/app_block_creation.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     2494 2023-05-29 15:40:49.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/app_by_list.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1226 2023-05-29 13:33:48.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/block_creation.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)    13766 2023-05-29 16:42:03.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/comparer.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1948 2023-05-10 11:20:21.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/metrics.py
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     6320 2023-05-24 09:08:26.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/reindex_operator.py
+drwxr-xr-x   0 joseramirezencinas   (501) staff       (20)        0 2023-05-29 16:44:46.836138 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker.egg-info/
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)      258 2023-05-29 16:44:46.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker.egg-info/PKG-INFO
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)     1144 2023-05-29 16:44:46.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker.egg-info/SOURCES.txt
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)        1 2023-05-29 16:44:46.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker.egg-info/dependency_links.txt
+-rw-r--r--   0 joseramirezencinas   (501) staff       (20)       42 2023-05-29 16:44:46.000000 transaction_service_quality_checker-0.0.5/transaction_service_quality_checker.egg-info/top_level.txt
```

### Comparing `transaction_service_quality_checker-0.0.4/README.md` & `transaction_service_quality_checker-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/tests/api/test_config_api_interface.py` & `transaction_service_quality_checker-0.0.5/tests/api/test_config_api_interface.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/tests/api/test_transaction_api_interface.py` & `transaction_service_quality_checker-0.0.5/tests/api/test_transaction_api_interface.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/addresses_map.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/addresses_map.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/api/config_api_interface.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/api/config_api_interface.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/api/etherscan_api_interface.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/api/etherscan_api_interface.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/api/transaction_api_interface.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/api/transaction_api_interface.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/app.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/app.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/app_block_creation.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/app_block_creation.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/app_by_list.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/app_by_list.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/block_creation.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/block_creation.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/comparer.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/comparer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import web3
 import logging
 import json
-from api.config_api_interface import ConfigAPIinterface
-from api.transaction_api_interface import TransactionAPIinterface
-from metrics import Metrics
+from .api.config_api_interface import ConfigAPIinterface
+from .api.transaction_api_interface import TransactionAPIinterface
+from .metrics import Metrics
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 
 class Comparer():
     def __init__(self, domain_a: str, domain_b: str, log: logging.Logger = logging,
                  balance_in_usd_percentage_threshold: float = 0.03):
         self.log = log
```

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/metrics.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/metrics.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker/reindex_operator.py` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker/reindex_operator.py`

 * *Files identical despite different names*

### Comparing `transaction_service_quality_checker-0.0.4/transaction_service_quality_checker.egg-info/SOURCES.txt` & `transaction_service_quality_checker-0.0.5/transaction_service_quality_checker.egg-info/SOURCES.txt`

 * *Files identical despite different names*


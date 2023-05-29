# Comparing `tmp/funcat3-1.1.2.tar.gz` & `tmp/funcat3-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcat3-1.1.2.tar", last modified: Mon May 29 11:10:28 2023, max compression
+gzip compressed data, was "funcat3-1.1.3.tar", last modified: Mon May 29 14:44:31 2023, max compression
```

## Comparing `funcat3-1.1.2.tar` & `funcat3-1.1.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.923602 funcat3-1.1.2/
--rw-r--r--   0 root         (0) root         (0)    11358 2022-08-29 11:25:09.000000 funcat3-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       43 2022-08-29 11:25:09.000000 funcat3-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-29 11:10:28.923602 funcat3-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8193 2023-05-29 10:59:29.000000 funcat3-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.918602 funcat3-1.1.2/funcat/
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-29 11:06:53.000000 funcat3-1.1.2/funcat/VERSION.txt
--rw-r--r--   0 root         (0) root         (0)      617 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1133 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/account.py
--rw-r--r--   0 root         (0) root         (0)     2358 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/api.py
--rw-r--r--   0 root         (0) root         (0)     3456 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.920602 funcat3-1.1.2/funcat/data/
--rw-r--r--   0 root         (0) root         (0)       73 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7323 2023-05-29 03:14:54.000000 funcat3-1.1.2/funcat/data/akshare_backend.py
--rw-r--r--   0 root         (0) root         (0)      916 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/backend.py
--rw-r--r--   0 root         (0) root         (0)     4379 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/crypto_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.922602 funcat3-1.1.2/funcat/data/okex/
--rw-r--r--   0 root         (0) root         (0)       98 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3333 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/account_api.py
--rw-r--r--   0 root         (0) root         (0)     2695 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/client.py
--rw-r--r--   0 root         (0) root         (0)     5096 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/consts.py
--rw-r--r--   0 root         (0) root         (0)     2115 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/ett_api.py
--rw-r--r--   0 root         (0) root         (0)     1308 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7812 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/futures_api.py
--rw-r--r--   0 root         (0) root         (0)     7016 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/lever_api.py
--rw-r--r--   0 root         (0) root         (0)     6192 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/spot_api.py
--rw-r--r--   0 root         (0) root         (0)     6537 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/swap_api.py
--rw-r--r--   0 root         (0) root         (0)     1349 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/utils.py
--rw-r--r--   0 root         (0) root         (0)      807 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/websocket.py
--rw-r--r--   0 root         (0) root         (0)    51938 2023-05-25 02:34:54.000000 funcat3-1.1.2/funcat/data/order_book_id_list.csv
--rw-r--r--   0 root         (0) root         (0)     2732 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/rqalpha_data_backend.py
--rw-r--r--   0 root         (0) root         (0)     2042 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/rqdata_data_backend.py
--rw-r--r--   0 root         (0) root         (0)     1276 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/rt_data.py
--rw-r--r--   0 root         (0) root         (0)     1101 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/rt_data_from_tencent.py
--rw-r--r--   0 root         (0) root         (0)   824029 2023-05-25 02:34:54.000000 funcat3-1.1.2/funcat/data/stock_basic.csv
--rw-r--r--   0 root         (0) root         (0)     5185 2022-09-05 10:53:19.000000 funcat3-1.1.2/funcat/data/tencent_backend.py
--rw-r--r--   0 root         (0) root         (0)     8468 2023-05-25 02:34:54.000000 funcat3-1.1.2/funcat/data/tushare_backend.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-05-29 10:38:39.000000 funcat3-1.1.2/funcat/func.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-24 06:09:32.000000 funcat3-1.1.2/funcat/helper.py
--rw-r--r--   0 root         (0) root         (0)     3273 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/indicators.py
--rw-r--r--   0 root         (0) root         (0)     8281 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/time_series.py
--rw-r--r--   0 root         (0) root         (0)     2603 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.922602 funcat3-1.1.2/funcat3.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1141 2023-05-29 11:10:28.000000 funcat3-1.1.2/funcat3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1251 2023-05-29 11:10:28.000000 funcat3-1.1.2/funcat3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 11:10:28.000000 funcat3-1.1.2/funcat3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 06:52:56.000000 funcat3-1.1.2/funcat3.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-29 11:10:28.000000 funcat3-1.1.2/funcat3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-29 11:10:28.000000 funcat3-1.1.2/funcat3.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-29 11:05:00.000000 funcat3-1.1.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 11:10:28.923602 funcat3-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1915 2023-05-29 11:10:21.000000 funcat3-1.1.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.923602 funcat3-1.1.2/tests/
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-29 03:02:56.000000 funcat3-1.1.2/tests/test_akshare_api.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-05-29 10:38:39.000000 funcat3-1.1.2/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)      307 2022-08-29 11:25:09.000000 funcat3-1.1.2/tests/test_api_cryto.py
--rw-r--r--   0 root         (0) root         (0)      665 2022-09-01 09:41:08.000000 funcat3-1.1.2/tests/test_tencent_api.py
--rw-r--r--   0 root         (0) root         (0)      488 2023-05-25 02:34:54.000000 funcat3-1.1.2/tests/test_tushare_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:44:31.806307 funcat3-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)    11358 2022-08-29 11:25:09.000000 funcat3-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       43 2022-08-29 11:25:09.000000 funcat3-1.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-29 14:44:31.806307 funcat3-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8373 2023-05-29 14:41:02.000000 funcat3-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:44:31.802307 funcat3-1.1.3/funcat/
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-29 14:44:16.000000 funcat3-1.1.3/funcat/VERSION.txt
+-rw-r--r--   0 root         (0) root         (0)      670 2023-05-29 14:42:32.000000 funcat3-1.1.3/funcat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/account.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/api.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:44:31.804307 funcat3-1.1.3/funcat/data/
+-rw-r--r--   0 root         (0) root         (0)       73 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-05-29 03:14:54.000000 funcat3-1.1.3/funcat/data/akshare_backend.py
+-rw-r--r--   0 root         (0) root         (0)      916 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/backend.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/crypto_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:44:31.805307 funcat3-1.1.3/funcat/data/okex/
+-rw-r--r--   0 root         (0) root         (0)       98 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/account_api.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/client.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/consts.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/ett_api.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7812 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/futures_api.py
+-rw-r--r--   0 root         (0) root         (0)     7016 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/lever_api.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/spot_api.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/swap_api.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/utils.py
+-rw-r--r--   0 root         (0) root         (0)      807 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/okex/websocket.py
+-rw-r--r--   0 root         (0) root         (0)    51938 2023-05-25 02:34:54.000000 funcat3-1.1.3/funcat/data/order_book_id_list.csv
+-rw-r--r--   0 root         (0) root         (0)     2732 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/rqalpha_data_backend.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/rqdata_data_backend.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/rt_data.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/data/rt_data_from_tencent.py
+-rw-r--r--   0 root         (0) root         (0)   824029 2023-05-25 02:34:54.000000 funcat3-1.1.3/funcat/data/stock_basic.csv
+-rw-r--r--   0 root         (0) root         (0)     5185 2022-09-05 10:53:19.000000 funcat3-1.1.3/funcat/data/tencent_backend.py
+-rw-r--r--   0 root         (0) root         (0)     8468 2023-05-25 02:34:54.000000 funcat3-1.1.3/funcat/data/tushare_backend.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-29 10:38:39.000000 funcat3-1.1.3/funcat/func.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-24 06:09:32.000000 funcat3-1.1.3/funcat/helper.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/indicators.py
+-rw-r--r--   0 root         (0) root         (0)     8281 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/time_series.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2022-08-29 11:25:09.000000 funcat3-1.1.3/funcat/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:44:31.806307 funcat3-1.1.3/funcat3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-29 14:44:31.000000 funcat3-1.1.3/funcat3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-29 14:44:31.000000 funcat3-1.1.3/funcat3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 14:44:31.000000 funcat3-1.1.3/funcat3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 06:52:56.000000 funcat3-1.1.3/funcat3.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-29 14:44:31.000000 funcat3-1.1.3/funcat3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-29 14:44:31.000000 funcat3-1.1.3/funcat3.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      178 2023-05-29 14:43:17.000000 funcat3-1.1.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 14:44:31.806307 funcat3-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-05-29 11:10:21.000000 funcat3-1.1.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 14:44:31.806307 funcat3-1.1.3/tests/
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-29 03:02:56.000000 funcat3-1.1.3/tests/test_akshare_api.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-05-29 10:38:39.000000 funcat3-1.1.3/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)      307 2022-08-29 11:25:09.000000 funcat3-1.1.3/tests/test_api_cryto.py
+-rw-r--r--   0 root         (0) root         (0)      665 2022-09-01 09:41:08.000000 funcat3-1.1.3/tests/test_tencent_api.py
+-rw-r--r--   0 root         (0) root         (0)      488 2023-05-25 02:34:54.000000 funcat3-1.1.3/tests/test_tushare_api.py
```

### Comparing `funcat3-1.1.2/LICENSE` & `funcat3-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/PKG-INFO` & `funcat3-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcat3
-Version: 1.1.2
+Version: 1.1.3
 Home-page: https://github.com/mapicccy/funcat
 Author: Guanjun
 Author-email: mapicccy@gmail.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
```

### Comparing `funcat3-1.1.2/README.md` & `funcat3-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -27,28 +27,28 @@
 
 激活虚拟环境：
 ```
 conda activate py39
 ```
 ### 安装funcat
 1. 安装科学计算库(必选，用于funcat计算指标)
-以下安装方式2选1
-- 虚拟环境安装
+- 虚拟环境安装(推荐)
 ```
 conda install -c conda-forge ta-lib
 ```
-- pip安装
+- pip安装(不推荐，需要前置安装libta_lib.so，在大多数操作系统不提供该库)
 ```
 pip install ta-lib
 ```
 
 2. 安装funcat:
 ```
 pip install funcat3 -i https://pypi.org/simple
 ```
+如果上述命令在安装ta-lib时出现报错，请重新pip install ta-lib后再执行funcat3安装命令
 
 如有其他安装问题，请提issue，并附上足够的环境信息。
 
 
 ## notebooks 教程
 - [quick-start](https://github.com/mapicccy/funcat/blob/master/notebooks/funcat-tutorial.ipynb)
```

### Comparing `funcat3-1.1.2/funcat/__init__.py` & `funcat3-1.1.3/funcat/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,12 +11,13 @@
 
 del pkgutil
 
 from .api import *
 from .indicators import *
 
 from .data.tushare_backend import TushareDataBackend
+from .data.akshare_backend import AkshareDataBackend
 from .context import ExecutionContext as funcat_execution_context
 
 funcat_execution_context(date=20170104,
                          order_book_id="000001.SH",
                          data_backend=TushareDataBackend())._push()
```

### Comparing `funcat3-1.1.2/funcat/account.py` & `funcat3-1.1.3/funcat/account.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/api.py` & `funcat3-1.1.3/funcat/api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/context.py` & `funcat3-1.1.3/funcat/context.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/akshare_backend.py` & `funcat3-1.1.3/funcat/data/akshare_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/backend.py` & `funcat3-1.1.3/funcat/data/backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/crypto_backend.py` & `funcat3-1.1.3/funcat/data/crypto_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/account_api.py` & `funcat3-1.1.3/funcat/data/okex/account_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/client.py` & `funcat3-1.1.3/funcat/data/okex/client.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/consts.py` & `funcat3-1.1.3/funcat/data/okex/consts.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/ett_api.py` & `funcat3-1.1.3/funcat/data/okex/ett_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/exceptions.py` & `funcat3-1.1.3/funcat/data/okex/exceptions.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/futures_api.py` & `funcat3-1.1.3/funcat/data/okex/futures_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/lever_api.py` & `funcat3-1.1.3/funcat/data/okex/lever_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/spot_api.py` & `funcat3-1.1.3/funcat/data/okex/spot_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/swap_api.py` & `funcat3-1.1.3/funcat/data/okex/swap_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/utils.py` & `funcat3-1.1.3/funcat/data/okex/utils.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/okex/websocket.py` & `funcat3-1.1.3/funcat/data/okex/websocket.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/order_book_id_list.csv` & `funcat3-1.1.3/funcat/data/order_book_id_list.csv`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/rqalpha_data_backend.py` & `funcat3-1.1.3/funcat/data/rqalpha_data_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/rqdata_data_backend.py` & `funcat3-1.1.3/funcat/data/rqdata_data_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/rt_data.py` & `funcat3-1.1.3/funcat/data/rt_data.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/rt_data_from_tencent.py` & `funcat3-1.1.3/funcat/data/rt_data_from_tencent.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/stock_basic.csv` & `funcat3-1.1.3/funcat/data/stock_basic.csv`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/tencent_backend.py` & `funcat3-1.1.3/funcat/data/tencent_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/data/tushare_backend.py` & `funcat3-1.1.3/funcat/data/tushare_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/func.py` & `funcat3-1.1.3/funcat/func.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/helper.py` & `funcat3-1.1.3/funcat/helper.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/indicators.py` & `funcat3-1.1.3/funcat/indicators.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/time_series.py` & `funcat3-1.1.3/funcat/time_series.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat/utils.py` & `funcat3-1.1.3/funcat/utils.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/funcat3.egg-info/PKG-INFO` & `funcat3-1.1.3/funcat3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcat3
-Version: 1.1.2
+Version: 1.1.3
 Home-page: https://github.com/mapicccy/funcat
 Author: Guanjun
 Author-email: mapicccy@gmail.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
```

### Comparing `funcat3-1.1.2/funcat3.egg-info/SOURCES.txt` & `funcat3-1.1.3/funcat3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/setup.py` & `funcat3-1.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/tests/test_akshare_api.py` & `funcat3-1.1.3/tests/test_akshare_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/tests/test_api.py` & `funcat3-1.1.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.2/tests/test_tencent_api.py` & `funcat3-1.1.3/tests/test_tencent_api.py`

 * *Files identical despite different names*


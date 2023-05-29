# Comparing `tmp/funcat3-1.1.1.tar.gz` & `tmp/funcat3-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcat3-1.1.1.tar", last modified: Mon May 29 10:46:17 2023, max compression
+gzip compressed data, was "funcat3-1.1.2.tar", last modified: Mon May 29 11:10:28 2023, max compression
```

## Comparing `funcat3-1.1.1.tar` & `funcat3-1.1.2.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.621368 funcat3-1.1.1/
--rw-r--r--   0 root         (0) root         (0)    11358 2022-08-29 11:25:09.000000 funcat3-1.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       43 2022-08-29 11:25:09.000000 funcat3-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      919 2023-05-29 10:46:17.621368 funcat3-1.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8087 2023-05-29 09:48:34.000000 funcat3-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.616368 funcat3-1.1.1/funcat/
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-29 10:45:37.000000 funcat3-1.1.1/funcat/VERSION.txt
--rw-r--r--   0 root         (0) root         (0)      617 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1133 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/account.py
--rw-r--r--   0 root         (0) root         (0)     2358 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/api.py
--rw-r--r--   0 root         (0) root         (0)     3456 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.618368 funcat3-1.1.1/funcat/data/
--rw-r--r--   0 root         (0) root         (0)       73 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7323 2023-05-29 03:14:54.000000 funcat3-1.1.1/funcat/data/akshare_backend.py
--rw-r--r--   0 root         (0) root         (0)      916 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/backend.py
--rw-r--r--   0 root         (0) root         (0)     4379 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/crypto_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.619368 funcat3-1.1.1/funcat/data/okex/
--rw-r--r--   0 root         (0) root         (0)       98 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3333 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/account_api.py
--rw-r--r--   0 root         (0) root         (0)     2695 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/client.py
--rw-r--r--   0 root         (0) root         (0)     5096 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/consts.py
--rw-r--r--   0 root         (0) root         (0)     2115 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/ett_api.py
--rw-r--r--   0 root         (0) root         (0)     1308 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7812 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/futures_api.py
--rw-r--r--   0 root         (0) root         (0)     7016 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/lever_api.py
--rw-r--r--   0 root         (0) root         (0)     6192 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/spot_api.py
--rw-r--r--   0 root         (0) root         (0)     6537 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/swap_api.py
--rw-r--r--   0 root         (0) root         (0)     1349 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/utils.py
--rw-r--r--   0 root         (0) root         (0)      807 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/websocket.py
--rw-r--r--   0 root         (0) root         (0)    51938 2023-05-25 02:34:54.000000 funcat3-1.1.1/funcat/data/order_book_id_list.csv
--rw-r--r--   0 root         (0) root         (0)     2732 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/rqalpha_data_backend.py
--rw-r--r--   0 root         (0) root         (0)     2042 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/rqdata_data_backend.py
--rw-r--r--   0 root         (0) root         (0)     1276 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/rt_data.py
--rw-r--r--   0 root         (0) root         (0)     1101 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/rt_data_from_tencent.py
--rw-r--r--   0 root         (0) root         (0)   824029 2023-05-25 02:34:54.000000 funcat3-1.1.1/funcat/data/stock_basic.csv
--rw-r--r--   0 root         (0) root         (0)     5185 2022-09-05 10:53:19.000000 funcat3-1.1.1/funcat/data/tencent_backend.py
--rw-r--r--   0 root         (0) root         (0)     8468 2023-05-25 02:34:54.000000 funcat3-1.1.1/funcat/data/tushare_backend.py
--rw-r--r--   0 root         (0) root         (0)     8315 2023-05-29 10:38:39.000000 funcat3-1.1.1/funcat/func.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-24 06:09:32.000000 funcat3-1.1.1/funcat/helper.py
--rw-r--r--   0 root         (0) root         (0)     3273 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/indicators.py
--rw-r--r--   0 root         (0) root         (0)     8281 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/time_series.py
--rw-r--r--   0 root         (0) root         (0)     2603 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.620368 funcat3-1.1.1/funcat3.egg-info/
--rw-r--r--   0 root         (0) root         (0)      919 2023-05-29 10:46:17.000000 funcat3-1.1.1/funcat3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1251 2023-05-29 10:46:17.000000 funcat3-1.1.1/funcat3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 10:46:17.000000 funcat3-1.1.1/funcat3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 06:52:56.000000 funcat3-1.1.1/funcat3.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-29 10:46:17.000000 funcat3-1.1.1/funcat3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-29 10:46:17.000000 funcat3-1.1.1/funcat3.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      185 2023-05-29 10:43:25.000000 funcat3-1.1.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 10:46:17.621368 funcat3-1.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-29 07:02:54.000000 funcat3-1.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.620368 funcat3-1.1.1/tests/
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-29 03:02:56.000000 funcat3-1.1.1/tests/test_akshare_api.py
--rw-r--r--   0 root         (0) root         (0)     1349 2023-05-29 10:38:39.000000 funcat3-1.1.1/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)      307 2022-08-29 11:25:09.000000 funcat3-1.1.1/tests/test_api_cryto.py
--rw-r--r--   0 root         (0) root         (0)      665 2022-09-01 09:41:08.000000 funcat3-1.1.1/tests/test_tencent_api.py
--rw-r--r--   0 root         (0) root         (0)      488 2023-05-25 02:34:54.000000 funcat3-1.1.1/tests/test_tushare_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.923602 funcat3-1.1.2/
+-rw-r--r--   0 root         (0) root         (0)    11358 2022-08-29 11:25:09.000000 funcat3-1.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       43 2022-08-29 11:25:09.000000 funcat3-1.1.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-29 11:10:28.923602 funcat3-1.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8193 2023-05-29 10:59:29.000000 funcat3-1.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.918602 funcat3-1.1.2/funcat/
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-29 11:06:53.000000 funcat3-1.1.2/funcat/VERSION.txt
+-rw-r--r--   0 root         (0) root         (0)      617 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/account.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/api.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.920602 funcat3-1.1.2/funcat/data/
+-rw-r--r--   0 root         (0) root         (0)       73 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-05-29 03:14:54.000000 funcat3-1.1.2/funcat/data/akshare_backend.py
+-rw-r--r--   0 root         (0) root         (0)      916 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/backend.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/crypto_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.922602 funcat3-1.1.2/funcat/data/okex/
+-rw-r--r--   0 root         (0) root         (0)       98 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/account_api.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/client.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/consts.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/ett_api.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7812 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/futures_api.py
+-rw-r--r--   0 root         (0) root         (0)     7016 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/lever_api.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/spot_api.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/swap_api.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/utils.py
+-rw-r--r--   0 root         (0) root         (0)      807 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/okex/websocket.py
+-rw-r--r--   0 root         (0) root         (0)    51938 2023-05-25 02:34:54.000000 funcat3-1.1.2/funcat/data/order_book_id_list.csv
+-rw-r--r--   0 root         (0) root         (0)     2732 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/rqalpha_data_backend.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/rqdata_data_backend.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/rt_data.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/data/rt_data_from_tencent.py
+-rw-r--r--   0 root         (0) root         (0)   824029 2023-05-25 02:34:54.000000 funcat3-1.1.2/funcat/data/stock_basic.csv
+-rw-r--r--   0 root         (0) root         (0)     5185 2022-09-05 10:53:19.000000 funcat3-1.1.2/funcat/data/tencent_backend.py
+-rw-r--r--   0 root         (0) root         (0)     8468 2023-05-25 02:34:54.000000 funcat3-1.1.2/funcat/data/tushare_backend.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-29 10:38:39.000000 funcat3-1.1.2/funcat/func.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-24 06:09:32.000000 funcat3-1.1.2/funcat/helper.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/indicators.py
+-rw-r--r--   0 root         (0) root         (0)     8281 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/time_series.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2022-08-29 11:25:09.000000 funcat3-1.1.2/funcat/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.922602 funcat3-1.1.2/funcat3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-05-29 11:10:28.000000 funcat3-1.1.2/funcat3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-29 11:10:28.000000 funcat3-1.1.2/funcat3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 11:10:28.000000 funcat3-1.1.2/funcat3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 06:52:56.000000 funcat3-1.1.2/funcat3.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-29 11:10:28.000000 funcat3-1.1.2/funcat3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-29 11:10:28.000000 funcat3-1.1.2/funcat3.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-29 11:05:00.000000 funcat3-1.1.2/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 11:10:28.923602 funcat3-1.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1915 2023-05-29 11:10:21.000000 funcat3-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:10:28.923602 funcat3-1.1.2/tests/
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-29 03:02:56.000000 funcat3-1.1.2/tests/test_akshare_api.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-05-29 10:38:39.000000 funcat3-1.1.2/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)      307 2022-08-29 11:25:09.000000 funcat3-1.1.2/tests/test_api_cryto.py
+-rw-r--r--   0 root         (0) root         (0)      665 2022-09-01 09:41:08.000000 funcat3-1.1.2/tests/test_tencent_api.py
+-rw-r--r--   0 root         (0) root         (0)      488 2023-05-25 02:34:54.000000 funcat3-1.1.2/tests/test_tushare_api.py
```

### Comparing `funcat3-1.1.1/LICENSE` & `funcat3-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/PKG-INFO` & `funcat3-1.1.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcat3
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/mapicccy/funcat
 Author: Guanjun
 Author-email: mapicccy@gmail.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
@@ -16,8 +16,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-Using very simple code to compute indicator of stock\crytocurrency. Make quantify easier to everyone
+Using very simple code to compute indicator of stock\crytocurrency. Make quantify easier to everyone.
+Funcat has transplanted the indicator formulas of THS, Tongdaxin, Wenhua Finance, and other platforms into Python. It is suitable for quantitative analysis and trading of stocks, futures, contracts, and cryptocurrencies.
```

### Comparing `funcat3-1.1.1/README.md` & `funcat3-1.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,35 +13,41 @@
 - akshare (只支持python >= 3.9)
 - okex加密数字货币
 - rqdata
 - tencent实时A股接口
 
 ## 安装
 
-### Python环境安装
-推荐python39，推荐通过[miniconda](https://docs.conda.io/en/latest/miniconda.html)管理环境。
+### Python环境安装(可选)
+推荐通过[miniconda](https://docs.conda.io/en/latest/miniconda.html)管理环境。
 
 创建python 3.9.12的虚拟环境：
 ```
 conda create -n py39 python==3.9.12
 ```
 
 激活虚拟环境：
 ```
 conda activate py39
 ```
 ### 安装funcat
-安装funcat:
+1. 安装科学计算库(必选，用于funcat计算指标)
+以下安装方式2选1
+- 虚拟环境安装
 ```
-pip install funcat3==1.1.0 -i https://pypi.org/simple
+conda install -c conda-forge ta-lib
+```
+- pip安装
+```
+pip install ta-lib
 ```
 
-安装科学计算库：
+2. 安装funcat:
 ```
-conda install -c conda-forge ta-lib
+pip install funcat3 -i https://pypi.org/simple
 ```
 
 如有其他安装问题，请提issue，并附上足够的环境信息。
 
 
 ## notebooks 教程
 - [quick-start](https://github.com/mapicccy/funcat/blob/master/notebooks/funcat-tutorial.ipynb)
```

### Comparing `funcat3-1.1.1/funcat/__init__.py` & `funcat3-1.1.2/funcat/__init__.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/account.py` & `funcat3-1.1.2/funcat/account.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/api.py` & `funcat3-1.1.2/funcat/api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/context.py` & `funcat3-1.1.2/funcat/context.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/akshare_backend.py` & `funcat3-1.1.2/funcat/data/akshare_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/backend.py` & `funcat3-1.1.2/funcat/data/backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/crypto_backend.py` & `funcat3-1.1.2/funcat/data/crypto_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/account_api.py` & `funcat3-1.1.2/funcat/data/okex/account_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/client.py` & `funcat3-1.1.2/funcat/data/okex/client.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/consts.py` & `funcat3-1.1.2/funcat/data/okex/consts.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/ett_api.py` & `funcat3-1.1.2/funcat/data/okex/ett_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/exceptions.py` & `funcat3-1.1.2/funcat/data/okex/exceptions.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/futures_api.py` & `funcat3-1.1.2/funcat/data/okex/futures_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/lever_api.py` & `funcat3-1.1.2/funcat/data/okex/lever_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/spot_api.py` & `funcat3-1.1.2/funcat/data/okex/spot_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/swap_api.py` & `funcat3-1.1.2/funcat/data/okex/swap_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/utils.py` & `funcat3-1.1.2/funcat/data/okex/utils.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/okex/websocket.py` & `funcat3-1.1.2/funcat/data/okex/websocket.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/order_book_id_list.csv` & `funcat3-1.1.2/funcat/data/order_book_id_list.csv`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/rqalpha_data_backend.py` & `funcat3-1.1.2/funcat/data/rqalpha_data_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/rqdata_data_backend.py` & `funcat3-1.1.2/funcat/data/rqdata_data_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/rt_data.py` & `funcat3-1.1.2/funcat/data/rt_data.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/rt_data_from_tencent.py` & `funcat3-1.1.2/funcat/data/rt_data_from_tencent.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/stock_basic.csv` & `funcat3-1.1.2/funcat/data/stock_basic.csv`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/tencent_backend.py` & `funcat3-1.1.2/funcat/data/tencent_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/data/tushare_backend.py` & `funcat3-1.1.2/funcat/data/tushare_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/func.py` & `funcat3-1.1.2/funcat/func.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/helper.py` & `funcat3-1.1.2/funcat/helper.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/indicators.py` & `funcat3-1.1.2/funcat/indicators.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/time_series.py` & `funcat3-1.1.2/funcat/time_series.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat/utils.py` & `funcat3-1.1.2/funcat/utils.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/funcat3.egg-info/PKG-INFO` & `funcat3-1.1.2/funcat3.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcat3
-Version: 1.1.1
+Version: 1.1.2
 Home-page: https://github.com/mapicccy/funcat
 Author: Guanjun
 Author-email: mapicccy@gmail.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
@@ -16,8 +16,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
-Using very simple code to compute indicator of stock\crytocurrency. Make quantify easier to everyone
+Using very simple code to compute indicator of stock\crytocurrency. Make quantify easier to everyone.
+Funcat has transplanted the indicator formulas of THS, Tongdaxin, Wenhua Finance, and other platforms into Python. It is suitable for quantitative analysis and trading of stocks, futures, contracts, and cryptocurrencies.
```

### Comparing `funcat3-1.1.1/funcat3.egg-info/SOURCES.txt` & `funcat3-1.1.2/funcat3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/setup.py` & `funcat3-1.1.2/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 with open(join(dirname(__file__), 'funcat/VERSION.txt'), 'rb') as f:
     version = f.read().decode('ascii').strip()
 
 setup(
     name='funcat3',
     version=version,
-    long_description='Using very simple code to compute indicator of stock\crytocurrency. Make quantify easier to everyone',
+    long_description='Using very simple code to compute indicator of stock\crytocurrency. Make quantify easier to everyone.\nFuncat has transplanted the indicator formulas of THS, Tongdaxin, Wenhua Finance, and other platforms into Python. It is suitable for quantitative analysis and trading of stocks, futures, contracts, and cryptocurrencies.',
     long_description_content_type="text/x-rst",
     packages=find_packages(exclude=[]),
     author='Guanjun',
     url='https://github.com/mapicccy/funcat',
     author_email='mapicccy@gmail.com',
     license='Apache License v2',
     package_data={'': ['*.*']},
```

### Comparing `funcat3-1.1.1/tests/test_akshare_api.py` & `funcat3-1.1.2/tests/test_akshare_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/tests/test_api.py` & `funcat3-1.1.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.1/tests/test_tencent_api.py` & `funcat3-1.1.2/tests/test_tencent_api.py`

 * *Files identical despite different names*


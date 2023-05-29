# Comparing `tmp/funcat3-1.1.0.tar.gz` & `tmp/funcat3-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funcat3-1.1.0.tar", last modified: Mon May 29 07:55:47 2023, max compression
+gzip compressed data, was "funcat3-1.1.1.tar", last modified: Mon May 29 10:46:17 2023, max compression
```

## Comparing `funcat3-1.1.0.tar` & `funcat3-1.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:55:47.386631 funcat3-1.1.0/
--rw-r--r--   0 root         (0) root         (0)    11358 2022-08-29 11:25:09.000000 funcat3-1.1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       43 2022-08-29 11:25:09.000000 funcat3-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      919 2023-05-29 07:55:47.385630 funcat3-1.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9224 2023-05-29 04:53:05.000000 funcat3-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:55:47.381631 funcat3-1.1.0/funcat/
--rw-r--r--   0 root         (0) root         (0)        6 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/VERSION.txt
--rw-r--r--   0 root         (0) root         (0)      617 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1133 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/account.py
--rw-r--r--   0 root         (0) root         (0)     2358 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/api.py
--rw-r--r--   0 root         (0) root         (0)     3456 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:55:47.383631 funcat3-1.1.0/funcat/data/
--rw-r--r--   0 root         (0) root         (0)       73 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7323 2023-05-29 03:14:54.000000 funcat3-1.1.0/funcat/data/akshare_backend.py
--rw-r--r--   0 root         (0) root         (0)      916 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/backend.py
--rw-r--r--   0 root         (0) root         (0)     4379 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/crypto_backend.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:55:47.384631 funcat3-1.1.0/funcat/data/okex/
--rw-r--r--   0 root         (0) root         (0)       98 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3333 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/account_api.py
--rw-r--r--   0 root         (0) root         (0)     2695 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/client.py
--rw-r--r--   0 root         (0) root         (0)     5096 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/consts.py
--rw-r--r--   0 root         (0) root         (0)     2115 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/ett_api.py
--rw-r--r--   0 root         (0) root         (0)     1308 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     7812 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/futures_api.py
--rw-r--r--   0 root         (0) root         (0)     7016 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/lever_api.py
--rw-r--r--   0 root         (0) root         (0)     6192 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/spot_api.py
--rw-r--r--   0 root         (0) root         (0)     6537 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/swap_api.py
--rw-r--r--   0 root         (0) root         (0)     1349 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/utils.py
--rw-r--r--   0 root         (0) root         (0)      807 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/okex/websocket.py
--rw-r--r--   0 root         (0) root         (0)    51938 2023-05-25 02:34:54.000000 funcat3-1.1.0/funcat/data/order_book_id_list.csv
--rw-r--r--   0 root         (0) root         (0)     2732 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/rqalpha_data_backend.py
--rw-r--r--   0 root         (0) root         (0)     2042 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/rqdata_data_backend.py
--rw-r--r--   0 root         (0) root         (0)     1276 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/rt_data.py
--rw-r--r--   0 root         (0) root         (0)     1101 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/data/rt_data_from_tencent.py
--rw-r--r--   0 root         (0) root         (0)   824029 2023-05-25 02:34:54.000000 funcat3-1.1.0/funcat/data/stock_basic.csv
--rw-r--r--   0 root         (0) root         (0)     5185 2022-09-05 10:53:19.000000 funcat3-1.1.0/funcat/data/tencent_backend.py
--rw-r--r--   0 root         (0) root         (0)     8468 2023-05-25 02:34:54.000000 funcat3-1.1.0/funcat/data/tushare_backend.py
--rw-r--r--   0 root         (0) root         (0)     8318 2022-09-02 07:29:03.000000 funcat3-1.1.0/funcat/func.py
--rw-r--r--   0 root         (0) root         (0)     5308 2023-05-24 06:09:32.000000 funcat3-1.1.0/funcat/helper.py
--rw-r--r--   0 root         (0) root         (0)     3273 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/indicators.py
--rw-r--r--   0 root         (0) root         (0)     8281 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/time_series.py
--rw-r--r--   0 root         (0) root         (0)     2603 2022-08-29 11:25:09.000000 funcat3-1.1.0/funcat/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:55:47.385630 funcat3-1.1.0/funcat3.egg-info/
--rw-r--r--   0 root         (0) root         (0)      919 2023-05-29 07:55:47.000000 funcat3-1.1.0/funcat3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1251 2023-05-29 07:55:47.000000 funcat3-1.1.0/funcat3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 07:55:47.000000 funcat3-1.1.0/funcat3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 06:52:56.000000 funcat3-1.1.0/funcat3.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-29 07:55:47.000000 funcat3-1.1.0/funcat3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-29 07:55:47.000000 funcat3-1.1.0/funcat3.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      178 2023-05-29 07:45:24.000000 funcat3-1.1.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 07:55:47.386631 funcat3-1.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-29 07:02:54.000000 funcat3-1.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 07:55:47.385630 funcat3-1.1.0/tests/
--rw-r--r--   0 root         (0) root         (0)      555 2023-05-29 03:02:56.000000 funcat3-1.1.0/tests/test_akshare_api.py
--rw-r--r--   0 root         (0) root         (0)     1355 2023-05-29 03:13:46.000000 funcat3-1.1.0/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)      307 2022-08-29 11:25:09.000000 funcat3-1.1.0/tests/test_api_cryto.py
--rw-r--r--   0 root         (0) root         (0)      665 2022-09-01 09:41:08.000000 funcat3-1.1.0/tests/test_tencent_api.py
--rw-r--r--   0 root         (0) root         (0)      488 2023-05-25 02:34:54.000000 funcat3-1.1.0/tests/test_tushare_api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.621368 funcat3-1.1.1/
+-rw-r--r--   0 root         (0) root         (0)    11358 2022-08-29 11:25:09.000000 funcat3-1.1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       43 2022-08-29 11:25:09.000000 funcat3-1.1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      919 2023-05-29 10:46:17.621368 funcat3-1.1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8087 2023-05-29 09:48:34.000000 funcat3-1.1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.616368 funcat3-1.1.1/funcat/
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-29 10:45:37.000000 funcat3-1.1.1/funcat/VERSION.txt
+-rw-r--r--   0 root         (0) root         (0)      617 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/account.py
+-rw-r--r--   0 root         (0) root         (0)     2358 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/api.py
+-rw-r--r--   0 root         (0) root         (0)     3456 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.618368 funcat3-1.1.1/funcat/data/
+-rw-r--r--   0 root         (0) root         (0)       73 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7323 2023-05-29 03:14:54.000000 funcat3-1.1.1/funcat/data/akshare_backend.py
+-rw-r--r--   0 root         (0) root         (0)      916 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/backend.py
+-rw-r--r--   0 root         (0) root         (0)     4379 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/crypto_backend.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.619368 funcat3-1.1.1/funcat/data/okex/
+-rw-r--r--   0 root         (0) root         (0)       98 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3333 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/account_api.py
+-rw-r--r--   0 root         (0) root         (0)     2695 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/client.py
+-rw-r--r--   0 root         (0) root         (0)     5096 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/consts.py
+-rw-r--r--   0 root         (0) root         (0)     2115 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/ett_api.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     7812 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/futures_api.py
+-rw-r--r--   0 root         (0) root         (0)     7016 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/lever_api.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/spot_api.py
+-rw-r--r--   0 root         (0) root         (0)     6537 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/swap_api.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/utils.py
+-rw-r--r--   0 root         (0) root         (0)      807 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/okex/websocket.py
+-rw-r--r--   0 root         (0) root         (0)    51938 2023-05-25 02:34:54.000000 funcat3-1.1.1/funcat/data/order_book_id_list.csv
+-rw-r--r--   0 root         (0) root         (0)     2732 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/rqalpha_data_backend.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/rqdata_data_backend.py
+-rw-r--r--   0 root         (0) root         (0)     1276 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/rt_data.py
+-rw-r--r--   0 root         (0) root         (0)     1101 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/data/rt_data_from_tencent.py
+-rw-r--r--   0 root         (0) root         (0)   824029 2023-05-25 02:34:54.000000 funcat3-1.1.1/funcat/data/stock_basic.csv
+-rw-r--r--   0 root         (0) root         (0)     5185 2022-09-05 10:53:19.000000 funcat3-1.1.1/funcat/data/tencent_backend.py
+-rw-r--r--   0 root         (0) root         (0)     8468 2023-05-25 02:34:54.000000 funcat3-1.1.1/funcat/data/tushare_backend.py
+-rw-r--r--   0 root         (0) root         (0)     8315 2023-05-29 10:38:39.000000 funcat3-1.1.1/funcat/func.py
+-rw-r--r--   0 root         (0) root         (0)     5308 2023-05-24 06:09:32.000000 funcat3-1.1.1/funcat/helper.py
+-rw-r--r--   0 root         (0) root         (0)     3273 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/indicators.py
+-rw-r--r--   0 root         (0) root         (0)     8281 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/time_series.py
+-rw-r--r--   0 root         (0) root         (0)     2603 2022-08-29 11:25:09.000000 funcat3-1.1.1/funcat/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.620368 funcat3-1.1.1/funcat3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      919 2023-05-29 10:46:17.000000 funcat3-1.1.1/funcat3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1251 2023-05-29 10:46:17.000000 funcat3-1.1.1/funcat3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 10:46:17.000000 funcat3-1.1.1/funcat3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 06:52:56.000000 funcat3-1.1.1/funcat3.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-29 10:46:17.000000 funcat3-1.1.1/funcat3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-29 10:46:17.000000 funcat3-1.1.1/funcat3.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      185 2023-05-29 10:43:25.000000 funcat3-1.1.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 10:46:17.621368 funcat3-1.1.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-05-29 07:02:54.000000 funcat3-1.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:46:17.620368 funcat3-1.1.1/tests/
+-rw-r--r--   0 root         (0) root         (0)      555 2023-05-29 03:02:56.000000 funcat3-1.1.1/tests/test_akshare_api.py
+-rw-r--r--   0 root         (0) root         (0)     1349 2023-05-29 10:38:39.000000 funcat3-1.1.1/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)      307 2022-08-29 11:25:09.000000 funcat3-1.1.1/tests/test_api_cryto.py
+-rw-r--r--   0 root         (0) root         (0)      665 2022-09-01 09:41:08.000000 funcat3-1.1.1/tests/test_tencent_api.py
+-rw-r--r--   0 root         (0) root         (0)      488 2023-05-25 02:34:54.000000 funcat3-1.1.1/tests/test_tushare_api.py
```

### Comparing `funcat3-1.1.0/LICENSE` & `funcat3-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/PKG-INFO` & `funcat3-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcat3
-Version: 1.1.0
+Version: 1.1.1
 Home-page: https://github.com/mapicccy/funcat
 Author: Guanjun
 Author-email: mapicccy@gmail.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
```

### Comparing `funcat3-1.1.0/README.md` & `funcat3-1.1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -4,52 +4,39 @@
 
 Funcat 适合做股票、期货、合约、加密数字货币的量化分析与量化交易。
 
 ## 策略
 
 基于funcat实现选股策略，在每个交易日14：00左右推送当日推荐股票。感兴趣可以关注本人[微信推送服务](https://wxpusher.zjiecode.com/api/qrcode/xW1JFRyDVn3pBtdFEHOk2MEemewESUicDSvxBUdmF3QX5AgAQxOJ4hNLlWkQHqSs.jpg)
 
-## 更新计划
-
-- 增加加密数字货币后端，创建实例时需要填入api_key\seceret_key\passphrase, [了解详情](https://www.okex.com/account/my-api)(已完成)
-- 增加对[tushare pro](https://tushare.pro/register?reg=379083)接口支持，使用需要注册[获取token](https://tushare.pro/register?reg=379083)(已完成)
-- 增加对[akshare](https://akshare.xyz/tutorial.html)接口支持
-- 优化tushare pro数据存储方式(已完成)
-- 优化DataFrame数据，降低内存占用(进行中...)
-- 增加实时数据获取(已完成，实时数据来自腾讯股票接口，http://qt.gtimg.cn/q=sh601360)
-- 更新个人选股策略，并使用回测系统回测（进行中...）
-	- **[MACD三次金叉线性拟合趋势](https://github.com/mapicccy/funcat#macd%E4%B8%89%E6%AC%A1%E9%87%91%E5%8F%89%E7%BA%BF%E6%80%A7%E6%8B%9F%E5%90%88%E8%B6%8B%E5%8A%BF)**
-	- ...
-- 由于tushare pro某些数据获取频次有特殊限制，所以计划将数据整体搬移至mysql（未开始）
-- 适配更高的python版本，并且提供docker容器部署方案（python3全版本适配完成，docker部署未开始）
-
 ## 数据源支持
 - tushare pro
-- akshare
+- akshare (只支持python >= 3.9)
 - okex加密数字货币
 - rqdata
 - tencent实时A股接口
 
 ## 安装
 
+### Python环境安装
 推荐python39，推荐通过[miniconda](https://docs.conda.io/en/latest/miniconda.html)管理环境。
 
 创建python 3.9.12的虚拟环境：
 ```
 conda create -n py39 python==3.9.12
 ```
 
 激活虚拟环境：
 ```
 conda activate py39
 ```
-
-安装funcat（因python版本问题可能会有一些依赖库安装不成功，通过pip install xxx手动安装）:
+### 安装funcat
+安装funcat:
 ```
-python setup.py install
+pip install funcat3==1.1.0 -i https://pypi.org/simple
 ```
 
 安装科学计算库：
 ```
 conda install -c conda-forge ta-lib
 ```
```

### Comparing `funcat3-1.1.0/funcat/__init__.py` & `funcat3-1.1.1/funcat/__init__.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/account.py` & `funcat3-1.1.1/funcat/account.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/api.py` & `funcat3-1.1.1/funcat/api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/context.py` & `funcat3-1.1.1/funcat/context.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/akshare_backend.py` & `funcat3-1.1.1/funcat/data/akshare_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/backend.py` & `funcat3-1.1.1/funcat/data/backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/crypto_backend.py` & `funcat3-1.1.1/funcat/data/crypto_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/account_api.py` & `funcat3-1.1.1/funcat/data/okex/account_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/client.py` & `funcat3-1.1.1/funcat/data/okex/client.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/consts.py` & `funcat3-1.1.1/funcat/data/okex/consts.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/ett_api.py` & `funcat3-1.1.1/funcat/data/okex/ett_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/exceptions.py` & `funcat3-1.1.1/funcat/data/okex/exceptions.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/futures_api.py` & `funcat3-1.1.1/funcat/data/okex/futures_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/lever_api.py` & `funcat3-1.1.1/funcat/data/okex/lever_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/spot_api.py` & `funcat3-1.1.1/funcat/data/okex/spot_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/swap_api.py` & `funcat3-1.1.1/funcat/data/okex/swap_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/utils.py` & `funcat3-1.1.1/funcat/data/okex/utils.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/okex/websocket.py` & `funcat3-1.1.1/funcat/data/okex/websocket.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/order_book_id_list.csv` & `funcat3-1.1.1/funcat/data/order_book_id_list.csv`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/rqalpha_data_backend.py` & `funcat3-1.1.1/funcat/data/rqalpha_data_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/rqdata_data_backend.py` & `funcat3-1.1.1/funcat/data/rqdata_data_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/rt_data.py` & `funcat3-1.1.1/funcat/data/rt_data.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/rt_data_from_tencent.py` & `funcat3-1.1.1/funcat/data/rt_data_from_tencent.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/stock_basic.csv` & `funcat3-1.1.1/funcat/data/stock_basic.csv`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/tencent_backend.py` & `funcat3-1.1.1/funcat/data/tencent_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/data/tushare_backend.py` & `funcat3-1.1.1/funcat/data/tushare_backend.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/func.py` & `funcat3-1.1.1/funcat/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
 
 @handle_numpy_warning
 def count(cond, n):
     # TODO lazy compute
     series = cond.series
     size = len(cond.series) - n
     try:
-        result = np.full(size, 0, dtype=np.int)
+        result = np.full(size, 0, dtype=int)
     except ValueError as e:
         raise FormulaException(e)
     for i in range(size - 1, 0, -1):
         s = series[-n:]
         result[i] = len(s[s == True])
         series = series[:-1]
     return NumericSeries(result)
```

### Comparing `funcat3-1.1.0/funcat/helper.py` & `funcat3-1.1.1/funcat/helper.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/indicators.py` & `funcat3-1.1.1/funcat/indicators.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/time_series.py` & `funcat3-1.1.1/funcat/time_series.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat/utils.py` & `funcat3-1.1.1/funcat/utils.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/funcat3.egg-info/PKG-INFO` & `funcat3-1.1.1/funcat3.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funcat3
-Version: 1.1.0
+Version: 1.1.1
 Home-page: https://github.com/mapicccy/funcat
 Author: Guanjun
 Author-email: mapicccy@gmail.com
 License: Apache License v2
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
```

### Comparing `funcat3-1.1.0/funcat3.egg-info/SOURCES.txt` & `funcat3-1.1.1/funcat3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/setup.py` & `funcat3-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/tests/test_akshare_api.py` & `funcat3-1.1.1/tests/test_akshare_api.py`

 * *Files identical despite different names*

### Comparing `funcat3-1.1.0/tests/test_api.py` & `funcat3-1.1.1/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
 def test_stock_basic():
     pro = ts.pro_api()
     df = pro.query("stock_basic", exchange='', list_status='L', field='ts_code')
     print(df)
     df.to_csv("stock_basic.csv", index=False)
 
 
-# test_000001()
-# test_bak_basic()
-# test_stock_basic()
+test_000001()
+test_bak_basic()
+test_stock_basic()
 
 
 def test_akshare():
     from funcat.data.akshare_backend import AkshareDataBackend
     set_data_backend(AkshareDataBackend())
```

### Comparing `funcat3-1.1.0/tests/test_tencent_api.py` & `funcat3-1.1.1/tests/test_tencent_api.py`

 * *Files identical despite different names*


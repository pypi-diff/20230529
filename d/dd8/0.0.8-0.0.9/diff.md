# Comparing `tmp/dd8-0.0.8.tar.gz` & `tmp/dd8-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dd8-0.0.8.tar", last modified: Sun Feb  5 09:34:47 2023, max compression
+gzip compressed data, was "dd8-0.0.9.tar", last modified: Tue Feb 14 01:29:53 2023, max compression
```

## Comparing `dd8-0.0.8.tar` & `dd8-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-02-05 09:34:47.121848 dd8-0.0.8/
--rw-rw-rw-   0        0        0     1086 2022-10-09 23:58:50.000000 dd8-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      252 2023-02-05 09:34:47.115891 dd8-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        5 2022-10-09 23:58:50.000000 dd8-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-02-05 09:34:47.023838 dd8-0.0.8/dd8/
--rw-rw-rw-   0        0        0        0 2022-10-10 03:46:26.000000 dd8-0.0.8/dd8/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-05 09:34:47.110865 dd8-0.0.8/dd8/connectivity/
--rw-rw-rw-   0        0        0        0 2022-10-10 03:46:03.000000 dd8-0.0.8/dd8/connectivity/__init__.py
--rw-rw-rw-   0        0        0     7742 2022-12-23 10:28:01.000000 dd8-0.0.8/dd8/connectivity/base.py
--rw-rw-rw-   0        0        0     9324 2023-02-05 09:29:30.000000 dd8-0.0.8/dd8/connectivity/binance_.py
--rw-rw-rw-   0        0        0        0 2022-12-23 10:44:24.000000 dd8-0.0.8/dd8/connectivity/bloomberg_.py
--rw-rw-rw-   0        0        0     1554 2023-02-05 09:29:40.000000 dd8-0.0.8/dd8/connectivity/coinbase_.py
--rw-rw-rw-   0        0        0    18177 2023-02-05 09:29:45.000000 dd8-0.0.8/dd8/connectivity/defillama_.py
--rw-rw-rw-   0        0        0    26009 2023-02-05 09:29:53.000000 dd8-0.0.8/dd8/connectivity/deribit_.py
--rw-rw-rw-   0        0        0     1340 2022-12-22 03:40:43.000000 dd8-0.0.8/dd8/connectivity/enums.py
--rw-rw-rw-   0        0        0      498 2023-02-05 09:30:00.000000 dd8-0.0.8/dd8/connectivity/flipside_.py
--rw-rw-rw-   0        0        0     3646 2023-02-05 09:30:07.000000 dd8-0.0.8/dd8/connectivity/ftx_.py
--rw-rw-rw-   0        0        0     5822 2023-01-17 04:47:15.000000 dd8-0.0.8/dd8/connectivity/paradigm_.py
--rw-rw-rw-   0        0        0    11162 2023-02-05 09:30:20.000000 dd8-0.0.8/dd8/connectivity/talos_.py
-drwxrwxrwx   0        0        0        0 2023-02-05 09:34:47.044840 dd8-0.0.8/dd8.egg-info/
--rw-rw-rw-   0        0        0      252 2023-02-05 09:34:46.000000 dd8-0.0.8/dd8.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2023-02-05 09:34:46.000000 dd8-0.0.8/dd8.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-05 09:34:46.000000 dd8-0.0.8/dd8.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-01-31 15:37:22.000000 dd8-0.0.8/dd8.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        4 2023-02-05 09:34:46.000000 dd8-0.0.8/dd8.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-05 09:34:47.122856 dd8-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      466 2023-02-05 09:34:23.000000 dd8-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-14 01:29:53.957183 dd8-0.0.9/
+-rw-rw-rw-   0        0        0     1086 2022-10-09 23:58:50.000000 dd8-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      252 2023-02-14 01:29:53.957183 dd8-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        5 2022-10-09 23:58:50.000000 dd8-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-14 01:29:53.358893 dd8-0.0.9/dd8/
+-rw-rw-rw-   0        0        0        0 2022-10-10 03:46:26.000000 dd8-0.0.9/dd8/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-14 01:29:53.524630 dd8-0.0.9/dd8/connectivity/
+-rw-rw-rw-   0        0        0        0 2022-10-10 03:46:03.000000 dd8-0.0.9/dd8/connectivity/__init__.py
+-rw-rw-rw-   0        0        0     7742 2022-12-23 10:28:01.000000 dd8-0.0.9/dd8/connectivity/base.py
+-rw-rw-rw-   0        0        0     9324 2023-02-05 09:29:30.000000 dd8-0.0.9/dd8/connectivity/binance_.py
+-rw-rw-rw-   0        0        0        0 2022-12-23 10:44:24.000000 dd8-0.0.9/dd8/connectivity/bloomberg_.py
+-rw-rw-rw-   0        0        0     1554 2023-02-05 09:29:40.000000 dd8-0.0.9/dd8/connectivity/coinbase_.py
+-rw-rw-rw-   0        0        0    18177 2023-02-05 09:29:45.000000 dd8-0.0.9/dd8/connectivity/defillama_.py
+-rw-rw-rw-   0        0        0    26009 2023-02-05 09:29:53.000000 dd8-0.0.9/dd8/connectivity/deribit_.py
+-rw-rw-rw-   0        0        0     1340 2022-12-22 03:40:43.000000 dd8-0.0.9/dd8/connectivity/enums.py
+-rw-rw-rw-   0        0        0      498 2023-02-05 09:30:00.000000 dd8-0.0.9/dd8/connectivity/flipside_.py
+-rw-rw-rw-   0        0        0     3646 2023-02-05 09:30:07.000000 dd8-0.0.9/dd8/connectivity/ftx_.py
+-rw-rw-rw-   0        0        0     5822 2023-01-17 04:47:15.000000 dd8-0.0.9/dd8/connectivity/paradigm_.py
+-rw-rw-rw-   0        0        0    11162 2023-02-05 09:30:20.000000 dd8-0.0.9/dd8/connectivity/talos_.py
+drwxrwxrwx   0        0        0        0 2023-02-14 01:29:53.639346 dd8-0.0.9/dd8/finance/
+-rw-rw-rw-   0        0        0        0 2022-10-10 03:46:26.000000 dd8-0.0.9/dd8/finance/__init__.py
+-rw-rw-rw-   0        0        0     1551 2022-10-25 11:52:38.000000 dd8-0.0.9/dd8/finance/algo.py
+-rw-rw-rw-   0        0        0      691 2023-01-20 06:46:32.000000 dd8-0.0.9/dd8/finance/base.py
+-rw-rw-rw-   0        0        0     7557 2022-10-19 07:06:26.000000 dd8-0.0.9/dd8/finance/data.py
+drwxrwxrwx   0        0        0        0 2023-02-14 01:29:53.654926 dd8-0.0.9/dd8/finance/derivatives/
+-rw-rw-rw-   0        0        0       88 2023-02-05 09:48:03.000000 dd8-0.0.9/dd8/finance/derivatives/__init__.py
+-rw-rw-rw-   0        0        0     4187 2023-01-17 08:29:42.000000 dd8-0.0.9/dd8/finance/derivatives/rfq.py
+drwxrwxrwx   0        0        0        0 2023-02-14 01:29:53.756383 dd8-0.0.9/dd8/finance/derivatives/vanilla/
+-rw-rw-rw-   0        0        0       88 2023-02-05 09:48:14.000000 dd8-0.0.9/dd8/finance/derivatives/vanilla/__init__.py
+-rw-rw-rw-   0        0        0     4846 2023-02-13 03:24:19.000000 dd8-0.0.9/dd8/finance/derivatives/vanilla/base.py
+-rw-rw-rw-   0        0        0      891 2023-02-13 03:32:53.000000 dd8-0.0.9/dd8/finance/derivatives/vanilla/black_scholes.py
+-rw-rw-rw-   0        0        0      390 2023-02-06 05:33:44.000000 dd8-0.0.9/dd8/finance/derivatives/vanilla/enums.py
+-rw-rw-rw-   0        0        0      336 2023-02-06 05:55:59.000000 dd8-0.0.9/dd8/finance/derivatives/vanilla/instruments.py
+-rw-rw-rw-   0        0        0      486 2022-10-24 14:06:25.000000 dd8-0.0.9/dd8/finance/enums.py
+drwxrwxrwx   0        0        0        0 2023-02-14 01:29:53.834131 dd8-0.0.9/dd8/finance/market_data/
+-rw-rw-rw-   0        0        0       88 2023-02-05 09:48:03.000000 dd8-0.0.9/dd8/finance/market_data/__init__.py
+-rw-rw-rw-   0        0        0     8216 2023-02-13 08:35:15.000000 dd8-0.0.9/dd8/finance/market_data/base.py
+-rw-rw-rw-   0        0        0      729 2023-02-13 08:08:21.000000 dd8-0.0.9/dd8/finance/market_data/enums.py
+-rw-rw-rw-   0        0        0     4398 2023-02-13 08:21:48.000000 dd8-0.0.9/dd8/finance/market_data/rates.py
+-rw-rw-rw-   0        0        0     1870 2023-02-13 03:37:44.000000 dd8-0.0.9/dd8/finance/market_data/volatility.py
+-rw-rw-rw-   0        0        0     4481 2022-12-24 05:31:54.000000 dd8-0.0.9/dd8/finance/meta_trader.py
+-rw-rw-rw-   0        0        0     8455 2022-11-16 07:01:08.000000 dd8-0.0.9/dd8/finance/technical_analysis.py
+drwxrwxrwx   0        0        0        0 2023-02-14 01:29:53.376852 dd8-0.0.9/dd8.egg-info/
+-rw-rw-rw-   0        0        0      252 2023-02-14 01:29:53.000000 dd8-0.0.9/dd8.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1321 2023-02-14 01:29:53.000000 dd8-0.0.9/dd8.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-14 01:29:53.000000 dd8-0.0.9/dd8.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-01-31 15:37:22.000000 dd8-0.0.9/dd8.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        4 2023-02-14 01:29:53.000000 dd8-0.0.9/dd8.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-02-14 01:29:53.957183 dd8-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      466 2023-02-14 01:29:00.000000 dd8-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-14 01:29:53.957183 dd8-0.0.9/tests/
+-rw-rw-rw-   0        0        0      348 2022-12-23 04:30:48.000000 dd8-0.0.9/tests/test_binance_.py
+-rw-rw-rw-   0        0        0     5530 2022-11-19 05:22:18.000000 dd8-0.0.9/tests/test_cnn.py
+-rw-rw-rw-   0        0        0      420 2022-12-20 14:06:33.000000 dd8-0.0.9/tests/test_coinbase_.py
+-rw-rw-rw-   0        0        0      301 2022-12-23 07:50:26.000000 dd8-0.0.9/tests/test_defillama_.py
+-rw-rw-rw-   0        0        0     1919 2022-12-20 13:47:15.000000 dd8-0.0.9/tests/test_deribit_.py
+-rw-rw-rw-   0        0        0      376 2022-12-28 05:57:21.000000 dd8-0.0.9/tests/test_flipside_.py
+-rw-rw-rw-   0        0        0     2746 2022-10-28 11:40:03.000000 dd8-0.0.9/tests/test_ftx_.py
+-rw-rw-rw-   0        0        0      277 2022-12-08 07:39:03.000000 dd8-0.0.9/tests/test_talos_.py
```

### Comparing `dd8-0.0.8/LICENSE` & `dd8-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dd8-0.0.8/dd8/connectivity/base.py` & `dd8-0.0.9/dd8/connectivity/base.py`

 * *Files identical despite different names*

### Comparing `dd8-0.0.8/dd8/connectivity/binance_.py` & `dd8-0.0.9/dd8/connectivity/binance_.py`

 * *Files identical despite different names*

### Comparing `dd8-0.0.8/dd8/connectivity/coinbase_.py` & `dd8-0.0.9/dd8/connectivity/coinbase_.py`

 * *Files identical despite different names*

### Comparing `dd8-0.0.8/dd8/connectivity/defillama_.py` & `dd8-0.0.9/dd8/connectivity/defillama_.py`

 * *Files identical despite different names*

### Comparing `dd8-0.0.8/dd8/connectivity/deribit_.py` & `dd8-0.0.9/dd8/connectivity/deribit_.py`

 * *Files identical despite different names*

### Comparing `dd8-0.0.8/dd8/connectivity/enums.py` & `dd8-0.0.9/dd8/connectivity/enums.py`

 * *Files identical despite different names*

### Comparing `dd8-0.0.8/dd8/connectivity/ftx_.py` & `dd8-0.0.9/dd8/connectivity/ftx_.py`

 * *Files identical despite different names*

### Comparing `dd8-0.0.8/dd8/connectivity/paradigm_.py` & `dd8-0.0.9/dd8/connectivity/paradigm_.py`

 * *Files identical despite different names*

### Comparing `dd8-0.0.8/dd8/connectivity/talos_.py` & `dd8-0.0.9/dd8/connectivity/talos_.py`

 * *Files identical despite different names*


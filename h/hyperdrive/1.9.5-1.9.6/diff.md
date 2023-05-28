# Comparing `tmp/hyperdrive-1.9.5.tar.gz` & `tmp/hyperdrive-1.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyperdrive-1.9.5.tar", last modified: Sat Jan 14 02:31:56 2023, max compression
+gzip compressed data, was "hyperdrive-1.9.6.tar", last modified: Sun Jan 15 00:12:51 2023, max compression
```

## Comparing `hyperdrive-1.9.5.tar` & `hyperdrive-1.9.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 02:31:56.322620 hyperdrive-1.9.5/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-01-14 02:31:56.318620 hyperdrive-1.9.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    10422 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 02:31:56.318620 hyperdrive-1.9.5/hyperdrive/
--rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/Algotrader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2767 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/Broker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5699 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/Calculus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5825 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/Constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37330 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/DataSource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9884 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/Exchange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5075 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/FileOps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8687 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/History.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/Precognition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3084 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/Storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2662 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/TimeMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/Utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1920 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/Workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/hyperdrive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 02:31:56.318620 hyperdrive-1.9.5/hyperdrive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-01-14 02:31:56.000000 hyperdrive-1.9.5/hyperdrive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-14 02:31:56.000000 hyperdrive-1.9.5/hyperdrive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-14 02:31:56.000000 hyperdrive-1.9.5/hyperdrive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-14 02:31:56.000000 hyperdrive-1.9.5/hyperdrive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-14 02:31:56.000000 hyperdrive-1.9.5/hyperdrive.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-14 02:31:56.322620 hyperdrive-1.9.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-14 02:31:56.318620 hyperdrive-1.9.5/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)      413 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_Algotrader.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2065 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_Broker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3877 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_Calculus.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2283 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_Constants.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17336 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_DataSource.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8039 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_Exchange.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4701 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_FileOps.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_History.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_Precognition.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2592 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_Storage.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2059 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_TimeMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_Utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-01-14 02:31:44.000000 hyperdrive-1.9.5/test/test_Workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 00:12:51.750895 hyperdrive-1.9.6/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1069 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-01-15 00:12:51.750895 hyperdrive-1.9.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10422 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 00:12:51.746895 hyperdrive-1.9.6/hyperdrive/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      308 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/Algotrader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2767 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/Broker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5699 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/Calculus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6062 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/Constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37330 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/DataSource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9884 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/Exchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5075 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/FileOps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8687 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/History.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/Precognition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3084 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/Storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2900 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/TimeMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/Utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1920 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/Workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      103 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/hyperdrive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 00:12:51.746895 hyperdrive-1.9.6/hyperdrive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10877 2023-01-15 00:12:51.000000 hyperdrive-1.9.6/hyperdrive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-01-15 00:12:51.000000 hyperdrive-1.9.6/hyperdrive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-15 00:12:51.000000 hyperdrive-1.9.6/hyperdrive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-15 00:12:51.000000 hyperdrive-1.9.6/hyperdrive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-15 00:12:51.000000 hyperdrive-1.9.6/hyperdrive.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-15 00:12:51.750895 hyperdrive-1.9.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-15 00:12:51.750895 hyperdrive-1.9.6/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      413 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_Algotrader.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2065 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_Broker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3877 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_Calculus.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2283 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_Constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17336 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_DataSource.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8039 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_Exchange.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4701 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_FileOps.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2387 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_History.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_Precognition.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2592 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_Storage.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2059 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_TimeMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_Utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      562 2023-01-15 00:12:33.000000 hyperdrive-1.9.6/test/test_Workflow.py
```

### Comparing `hyperdrive-1.9.5/LICENSE` & `hyperdrive-1.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/PKG-INFO` & `hyperdrive-1.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdrive
-Version: 1.9.5
+Version: 1.9.6
 Summary: An algorithmic trading platform
 Home-page: https://github.com/suchak1/hyperdrive
 Author: Krish Suchak
 Author-email: suchak.krish@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/suchak1/hyperdrive/issues
 Project-URL: Source, https://github.com/suchak1/hyperdrive
```

### Comparing `hyperdrive-1.9.5/README.md` & `hyperdrive-1.9.6/README.md`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive/Broker.py` & `hyperdrive-1.9.6/hyperdrive/Broker.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive/Calculus.py` & `hyperdrive-1.9.6/hyperdrive/Calculus.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive/Constants.py` & `hyperdrive-1.9.6/hyperdrive/Constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from dotenv import load_dotenv, find_dotenv
 from pytz import timezone
 import vectorbt as vbt
 
 load_dotenv(find_dotenv('config.env'))
 
 
+def get_env_int(var_name, default=None):
+    return int(os.environ[var_name]) if os.environ.get(var_name) and os.environ[var_name].isnumeric() else default
+
+
 def get_env_bool(var_name):
     return bool(os.environ.get(var_name)
                 and os.environ[var_name].lower() == 'true')
 
 
 # Environment
 DEV = get_env_bool('DEV')
@@ -95,14 +99,18 @@
 SELL = 'SELL'
 
 # API
 BAL = 'Bal'
 NAME = 'Name'
 ABS_TOL = vbt.utils.math_.abs_tol
 
+# Model
+MAX_MODEL_AGE_DAYS = 90  # 3 months
+MIN_MODEL_ACCURACY = 0.95
+
 # Misc
 POLY_CRYPTO_SYMBOLS = [
     'X%3ABTCUSD', 'X%3AETHUSD',
     'X%3ALTCUSD', 'X%3AXMRUSD', 'X%3AIOTUSD'
 ]
 
 SENTIMENT_SYMBOLS_IGNORE = {
```

### Comparing `hyperdrive-1.9.5/hyperdrive/DataSource.py` & `hyperdrive-1.9.6/hyperdrive/DataSource.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive/Exchange.py` & `hyperdrive-1.9.6/hyperdrive/Exchange.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive/FileOps.py` & `hyperdrive-1.9.6/hyperdrive/FileOps.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive/History.py` & `hyperdrive-1.9.6/hyperdrive/History.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive/Precognition.py` & `hyperdrive-1.9.6/hyperdrive/Precognition.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive/Storage.py` & `hyperdrive-1.9.6/hyperdrive/Storage.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive/TimeMachine.py` & `hyperdrive-1.9.6/hyperdrive/TimeMachine.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 from time import sleep
 from datetime import datetime, timedelta
 from Constants import TZ, DATE_FMT, TIME_FMT, PRECISE_TIME_FMT
 
 
 class TimeTraveller:
+    def get_delta(self, d1, d2, format=DATE_FMT):
+        if type(d1) == str:
+            d1 = datetime.strptime(d1, format)
+        if type(d2) == str:
+            d2 = datetime.strptime(d2, format)
+
+        return abs(d2 - d1)
+
     def convert_delta(self, timeframe):
         if timeframe == 'max':
             return timedelta(days=36500)
 
         periods = {'y': 365, 'm': 30, 'w': 7, 'd': 1}
         period = 'y'
         idx = -1
```

### Comparing `hyperdrive-1.9.5/hyperdrive/Utils.py` & `hyperdrive-1.9.6/hyperdrive/Utils.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive/Workflow.py` & `hyperdrive-1.9.6/hyperdrive/Workflow.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/hyperdrive.egg-info/PKG-INFO` & `hyperdrive-1.9.6/hyperdrive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyperdrive
-Version: 1.9.5
+Version: 1.9.6
 Summary: An algorithmic trading platform
 Home-page: https://github.com/suchak1/hyperdrive
 Author: Krish Suchak
 Author-email: suchak.krish@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/suchak1/hyperdrive/issues
 Project-URL: Source, https://github.com/suchak1/hyperdrive
```

### Comparing `hyperdrive-1.9.5/hyperdrive.egg-info/SOURCES.txt` & `hyperdrive-1.9.6/hyperdrive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/setup.py` & `hyperdrive-1.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_Broker.py` & `hyperdrive-1.9.6/test/test_Broker.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_Calculus.py` & `hyperdrive-1.9.6/test/test_Calculus.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_Constants.py` & `hyperdrive-1.9.6/test/test_Constants.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_DataSource.py` & `hyperdrive-1.9.6/test/test_DataSource.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_Exchange.py` & `hyperdrive-1.9.6/test/test_Exchange.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_FileOps.py` & `hyperdrive-1.9.6/test/test_FileOps.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_History.py` & `hyperdrive-1.9.6/test/test_History.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_Precognition.py` & `hyperdrive-1.9.6/test/test_Precognition.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_Storage.py` & `hyperdrive-1.9.6/test/test_Storage.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_TimeMachine.py` & `hyperdrive-1.9.6/test/test_TimeMachine.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_Utils.py` & `hyperdrive-1.9.6/test/test_Utils.py`

 * *Files identical despite different names*

### Comparing `hyperdrive-1.9.5/test/test_Workflow.py` & `hyperdrive-1.9.6/test/test_Workflow.py`

 * *Files identical despite different names*


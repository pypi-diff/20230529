# Comparing `tmp/spotON_sdk-0.0.5.1.tar.gz` & `tmp/spotON_sdk-0.0.5.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.5.1.tar", last modified: Mon May 29 06:08:03 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.5.11.tar", last modified: Mon May 29 06:36:59 2023, max compression
```

## Comparing `spotON_sdk-0.0.5.1.tar` & `spotON_sdk-0.0.5.11.tar`

### file list

```diff
@@ -1,34 +1,26 @@
--rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.1/.gitignore
--rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.1/.gitmodules
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.1/LICENSE
--rw-r--r--   0        0        0      405 2023-05-29 06:03:48.378147 spotON_sdk-0.0.5.1/pyproject.toml
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0      165 2023-05-28 20:03:24.891372 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/API_Call.py
--rw-r--r--   0        0        0     2303 2023-05-28 16:41:31.459722 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      263 2023-05-28 19:44:31.805887 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/customBaseModel.py
--rw-r--r--   0        0        0     2806 2023-05-28 17:11:51.233618 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     8210 2023-05-28 16:32:06.404713 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/timeframes.py
--rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.5.1/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      459 2023-05-29 06:05:35.172801 spotON_sdk-0.0.5.1/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.1/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.5.1/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.1/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0     1753 2023-05-23 14:27:13.601664 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/Sensor_Device_test.py
--rw-r--r--   0        0        0     8258 2023-05-28 15:42:11.428221 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/_test.py
--rw-r--r--   0        0        0      452 2023-05-28 20:00:58.125992 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/api_call.py
--rw-r--r--   0        0        0     7199 2023-05-28 15:39:01.607110 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/create_spotON_Areas.py
--rw-r--r--   0        0        0     2051 2023-05-28 09:52:03.472090 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/create_token.py
--rw-r--r--   0        0        0     1964 2023-05-28 14:25:22.033622 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/make_json.py
--rw-r--r--   0        0        0      798 2023-05-28 18:21:21.497039 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/pricelogic_Test.py
--rw-r--r--   0        0        0     2930 2023-05-23 16:32:56.748640 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/userstate_test.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.1/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.11/.gitignore
+-rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.11/.gitmodules
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.11/LICENSE
+-rw-r--r--   0        0        0      416 2023-05-29 06:36:38.819802 spotON_sdk-0.0.5.11/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0      165 2023-05-28 20:03:24.891372 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/API_Call.py
+-rw-r--r--   0        0        0     2303 2023-05-28 16:41:31.459722 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      263 2023-05-28 19:44:31.805887 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/customBaseModel.py
+-rw-r--r--   0        0        0     2806 2023-05-28 17:11:51.233618 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     8210 2023-05-28 16:32:06.404713 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/timeframes.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.5.11/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      460 2023-05-29 06:36:50.213017 spotON_sdk-0.0.5.11/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.11/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.5.11/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.11/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.11/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.11/PKG-INFO
```

### Comparing `spotON_sdk-0.0.5.1/.gitignore` & `spotON_sdk-0.0.5.11/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.1/LICENSE` & `spotON_sdk-0.0.5.11/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/markets.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/timeframes.py` & `spotON_sdk-0.0.5.11/spotON_sdk/Logic/Price/timeframes.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.1/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.5.11/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.1/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.5.11/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*


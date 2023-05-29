# Comparing `tmp/asconnect-3.0.0.tar.gz` & `tmp/asconnect-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asconnect-3.0.0.tar", max compression
+gzip compressed data, was "asconnect-3.0.1.tar", max compression
```

## Comparing `asconnect-3.0.0.tar` & `asconnect-3.0.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1141 2023-05-26 09:25:30.302768 asconnect-3.0.0/LICENSE
--rw-r--r--   0        0        0     4502 2023-05-26 09:25:30.306768 asconnect-3.0.0/README.md
--rwxr-xr-x   0        0        0      297 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/__init__.py
--rw-r--r--   0        0        0     3165 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/altool.py
--rwxr-xr-x   0        0        0     3406 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/app_client.py
--rwxr-xr-x   0        0        0     5930 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/app_info_client.py
--rwxr-xr-x   0        0        0    10487 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/beta_review_client.py
--rwxr-xr-x   0        0        0     6296 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/build_client.py
--rwxr-xr-x   0        0        0     2301 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/client.py
--rw-r--r--   0        0        0     1301 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/exceptions.py
--rwxr-xr-x   0        0        0    12747 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/httpclient.py
--rw-r--r--   0        0        0      537 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/__init__.py
--rw-r--r--   0        0        0     2166 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/app_info.py
--rw-r--r--   0        0        0     4313 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/app_store.py
--rw-r--r--   0        0        0      933 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/app_store_version_localizations.py
--rw-r--r--   0        0        0     2721 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/apps.py
--rw-r--r--   0        0        0     1178 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/beta_app_review.py
--rw-r--r--   0        0        0     1866 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/beta_detail.py
--rw-r--r--   0        0        0     1277 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/beta_groups.py
--rw-r--r--   0        0        0     1225 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/builds.py
--rw-r--r--   0        0        0     1221 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/common.py
--rw-r--r--   0        0        0      978 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/idfa.py
--rw-r--r--   0        0        0     1373 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/localization.py
--rw-r--r--   0        0        0     4440 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/screenshots.py
--rw-r--r--   0        0        0     1364 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/models/users.py
--rwxr-xr-x   0        0        0     9963 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/screenshot_client.py
--rw-r--r--   0        0        0      352 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/sorting.py
--rwxr-xr-x   0        0        0     1216 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/users_client.py
--rw-r--r--   0        0        0     2219 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/utilities.py
--rwxr-xr-x   0        0        0    16470 2023-05-26 09:25:30.306768 asconnect-3.0.0/asconnect/version_client.py
--rw-r--r--   0        0        0     1342 2023-05-26 09:25:30.306768 asconnect-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     5662 1970-01-01 00:00:00.000000 asconnect-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1141 2023-05-29 02:27:05.304589 asconnect-3.0.1/LICENSE
+-rw-r--r--   0        0        0     4502 2023-05-29 02:27:05.304589 asconnect-3.0.1/README.md
+-rwxr-xr-x   0        0        0      297 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/__init__.py
+-rw-r--r--   0        0        0     3165 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/altool.py
+-rwxr-xr-x   0        0        0     3406 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/app_client.py
+-rwxr-xr-x   0        0        0     5930 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/app_info_client.py
+-rwxr-xr-x   0        0        0    10487 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/beta_review_client.py
+-rwxr-xr-x   0        0        0     6296 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/build_client.py
+-rwxr-xr-x   0        0        0     2301 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/client.py
+-rw-r--r--   0        0        0     1301 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/exceptions.py
+-rwxr-xr-x   0        0        0    12747 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/httpclient.py
+-rw-r--r--   0        0        0      537 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/__init__.py
+-rw-r--r--   0        0        0     2166 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/app_info.py
+-rw-r--r--   0        0        0     4313 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/app_store.py
+-rw-r--r--   0        0        0      933 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/app_store_version_localizations.py
+-rw-r--r--   0        0        0     2721 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/apps.py
+-rw-r--r--   0        0        0     1178 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/beta_app_review.py
+-rw-r--r--   0        0        0     1866 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/beta_detail.py
+-rw-r--r--   0        0        0     1277 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/beta_groups.py
+-rw-r--r--   0        0        0     1225 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/builds.py
+-rw-r--r--   0        0        0     1221 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/common.py
+-rw-r--r--   0        0        0      978 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/idfa.py
+-rw-r--r--   0        0        0     1373 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/localization.py
+-rw-r--r--   0        0        0     4556 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/screenshots.py
+-rw-r--r--   0        0        0     1364 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/models/users.py
+-rwxr-xr-x   0        0        0     9963 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/screenshot_client.py
+-rw-r--r--   0        0        0      352 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/sorting.py
+-rwxr-xr-x   0        0        0     1216 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/users_client.py
+-rw-r--r--   0        0        0     2219 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/utilities.py
+-rwxr-xr-x   0        0        0    16470 2023-05-29 02:27:05.304589 asconnect-3.0.1/asconnect/version_client.py
+-rw-r--r--   0        0        0     1342 2023-05-29 02:27:05.304589 asconnect-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5662 1970-01-01 00:00:00.000000 asconnect-3.0.1/PKG-INFO
```

### Comparing `asconnect-3.0.0/LICENSE` & `asconnect-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/README.md` & `asconnect-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/altool.py` & `asconnect-3.0.1/asconnect/altool.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/app_client.py` & `asconnect-3.0.1/asconnect/app_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/app_info_client.py` & `asconnect-3.0.1/asconnect/app_info_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/beta_review_client.py` & `asconnect-3.0.1/asconnect/beta_review_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/build_client.py` & `asconnect-3.0.1/asconnect/build_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/client.py` & `asconnect-3.0.1/asconnect/client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/exceptions.py` & `asconnect-3.0.1/asconnect/exceptions.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/httpclient.py` & `asconnect-3.0.1/asconnect/httpclient.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/__init__.py` & `asconnect-3.0.1/asconnect/models/__init__.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/app_info.py` & `asconnect-3.0.1/asconnect/models/app_info.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/app_store.py` & `asconnect-3.0.1/asconnect/models/app_store.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/app_store_version_localizations.py` & `asconnect-3.0.1/asconnect/models/app_store_version_localizations.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/apps.py` & `asconnect-3.0.1/asconnect/models/apps.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/beta_app_review.py` & `asconnect-3.0.1/asconnect/models/beta_app_review.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/beta_detail.py` & `asconnect-3.0.1/asconnect/models/beta_detail.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/beta_groups.py` & `asconnect-3.0.1/asconnect/models/beta_groups.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/builds.py` & `asconnect-3.0.1/asconnect/models/builds.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/common.py` & `asconnect-3.0.1/asconnect/models/common.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/idfa.py` & `asconnect-3.0.1/asconnect/models/idfa.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/localization.py` & `asconnect-3.0.1/asconnect/models/localization.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/models/screenshots.py` & `asconnect-3.0.1/asconnect/models/screenshots.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,33 +7,36 @@
 
 from asconnect.models.common import BaseAttributes, Resource, Links, Relationship, Reprable
 
 
 class ScreenshotDisplayType(enum.Enum):
     """Screenshot display type."""
 
+    APP_IPHONE_67 = "APP_IPHONE_67"
     APP_IPHONE_65 = "APP_IPHONE_65"
+    APP_IPHONE_61 = "APP_IPHONE_61"
     APP_IPHONE_58 = "APP_IPHONE_58"
     APP_IPHONE_55 = "APP_IPHONE_55"
     APP_IPHONE_47 = "APP_IPHONE_47"
     APP_IPHONE_40 = "APP_IPHONE_40"
     APP_IPHONE_35 = "APP_IPHONE_35"
-    APP_IPAD_PRO_6GEN_129 = "APP_IPAD_PRO_6GEN_129"
     APP_IPAD_PRO_3GEN_129 = "APP_IPAD_PRO_3GEN_129"
-    APP_IPAD_PRO_2GEN_129 = "APP_IPAD_PRO_2GEN_129"
     APP_IPAD_PRO_3GEN_11 = "APP_IPAD_PRO_3GEN_11"
     APP_IPAD_PRO_129 = "APP_IPAD_PRO_129"
     APP_IPAD_105 = "APP_IPAD_105"
     APP_IPAD_97 = "APP_IPAD_97"
-    APP_DESKTOP = "APP_DESKTOP"
+    APP_WATCH_ULTRA = "APP_WATCH_ULTRA"
     APP_WATCH_SERIES_7 = "APP_WATCH_SERIES_7"
     APP_WATCH_SERIES_4 = "APP_WATCH_SERIES_4"
     APP_WATCH_SERIES_3 = "APP_WATCH_SERIES_3"
+    APP_DESKTOP = "APP_DESKTOP"
     APP_APPLE_TV = "APP_APPLE_TV"
+    IMESSAGE_APP_IPHONE_67 = "IMESSAGE_APP_IPHONE_67"
     IMESSAGE_APP_IPHONE_65 = "IMESSAGE_APP_IPHONE_65"
+    IMESSAGE_APP_IPHONE_61 = "IMESSAGE_APP_IPHONE_61"
     IMESSAGE_APP_IPHONE_58 = "IMESSAGE_APP_IPHONE_58"
     IMESSAGE_APP_IPHONE_55 = "IMESSAGE_APP_IPHONE_55"
     IMESSAGE_APP_IPHONE_47 = "IMESSAGE_APP_IPHONE_47"
     IMESSAGE_APP_IPHONE_40 = "IMESSAGE_APP_IPHONE_40"
     IMESSAGE_APP_IPAD_PRO_3GEN_129 = "IMESSAGE_APP_IPAD_PRO_3GEN_129"
     IMESSAGE_APP_IPAD_PRO_3GEN_11 = "IMESSAGE_APP_IPAD_PRO_3GEN_11"
     IMESSAGE_APP_IPAD_PRO_129 = "IMESSAGE_APP_IPAD_PRO_129"
```

### Comparing `asconnect-3.0.0/asconnect/models/users.py` & `asconnect-3.0.1/asconnect/models/users.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/screenshot_client.py` & `asconnect-3.0.1/asconnect/screenshot_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/users_client.py` & `asconnect-3.0.1/asconnect/users_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/utilities.py` & `asconnect-3.0.1/asconnect/utilities.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/asconnect/version_client.py` & `asconnect-3.0.1/asconnect/version_client.py`

 * *Files identical despite different names*

### Comparing `asconnect-3.0.0/pyproject.toml` & `asconnect-3.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asconnect"
-version = "3.0.0"
+version = "3.0.1"
 description = "A wrapper around the Apple App Store Connect APIs"
 
 license = "MIT"
 
 authors = [
     "Dale Myers <dalemy@microsoft.com>"
 ]
```

### Comparing `asconnect-3.0.0/PKG-INFO` & `asconnect-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asconnect
-Version: 3.0.0
+Version: 3.0.1
 Summary: A wrapper around the Apple App Store Connect APIs
 Home-page: https://github.com/microsoft/asconnect
 License: MIT
 Keywords: apple,app store,itunes,connect
 Author: Dale Myers
 Author-email: dalemy@microsoft.com
 Requires-Python: >=3.8,<4.0
```


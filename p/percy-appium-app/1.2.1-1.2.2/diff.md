# Comparing `tmp/percy-appium-app-1.2.1.tar.gz` & `tmp/percy-appium-app-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "percy-appium-app-1.2.1.tar", last modified: Thu May 25 11:53:48 2023, max compression
+gzip compressed data, was "percy-appium-app-1.2.2.tar", last modified: Mon May 29 07:43:16 2023, max compression
```

## Comparing `percy-appium-app-1.2.1.tar` & `percy-appium-app-1.2.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.358613 percy-appium-app-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-25 11:53:48.358613 percy-appium-app-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/common/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/configs/
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/configs/devices.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/errors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/lib/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/ignore_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/lib/tile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/metadata/android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/metadata/ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/metadata/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/metadata/metadata_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/providers/app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/providers/generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/providers/provider_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/percy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.354613 percy-appium-app-1.2.1/percy_appium_app.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 11:53:48.000000 percy-appium-app-1.2.1/percy_appium_app.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 11:53:48.358613 percy-appium-app-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 11:53:48.358613 percy-appium-app-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_android_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_app_automate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_app_percy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_cli_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_generic_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_ignore_region.py
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_ios_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_metadata_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_percy_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     8196 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_screenshot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-25 11:53:26.000000 percy-appium-app-1.2.1/tests/test_tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.764246 percy-appium-app-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-29 07:43:16.760246 percy-appium-app-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4577 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.752246 percy-appium-app-1.2.2/percy/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.752246 percy-appium-app-1.2.2/percy/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.752246 percy-appium-app-1.2.2/percy/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/configs/devices.json
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.756246 percy-appium-app-1.2.2/percy/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/errors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.756246 percy-appium-app-1.2.2/percy/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/ignore_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/lib/tile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.756246 percy-appium-app-1.2.2/percy/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/metadata/android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/metadata/ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/metadata/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/metadata/metadata_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.756246 percy-appium-app-1.2.2/percy/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5376 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/providers/app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/providers/generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/providers/provider_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/percy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.756246 percy-appium-app-1.2.2/percy_appium_app.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5334 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 07:43:16.000000 percy-appium-app-1.2.2/percy_appium_app.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 07:43:16.764246 percy-appium-app-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:43:16.760246 percy-appium-app-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_android_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_app_automate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8709 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_app_percy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1975 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_cli_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13581 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_generic_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_ignore_region.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_ios_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_metadata_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_percy_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8240 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-29 07:42:54.000000 percy-appium-app-1.2.2/tests/test_tile.py
```

### Comparing `percy-appium-app-1.2.1/LICENSE` & `percy-appium-app-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/PKG-INFO` & `percy-appium-app-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `percy-appium-app-1.2.1/README.md` & `percy-appium-app-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/__init__.py` & `percy-appium-app-1.2.2/percy/__init__.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/configs/devices.json` & `percy-appium-app-1.2.2/percy/configs/devices.json`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/lib/app_percy.py` & `percy-appium-app-1.2.2/percy/lib/app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/lib/cache.py` & `percy-appium-app-1.2.2/percy/lib/cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/lib/cli_wrapper.py` & `percy-appium-app-1.2.2/percy/lib/cli_wrapper.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 from functools import lru_cache
 import os
-import platform
-
-from appium.version import version as APPIUM_VERSION
 import requests
-from percy.errors import CLIException
 
-from percy.version import __version__ as SDK_VERSION
+from percy.errors import CLIException
 from percy.common import log
-
-
-# Collect client and environment information
-CLIENT_INFO = 'percy-appium-app/' + SDK_VERSION
-ENV_INFO = ['appium/' + APPIUM_VERSION, 'python/' + platform.python_version()]
+from percy.environment import Environment
 
 # Maybe get the CLI API address from the environment
 PERCY_CLI_API = os.environ.get('PERCY_CLI_API') or 'http://localhost:5338'
 
-
 class CLIWrapper:
     def __init__(self) -> None:
         pass
 
     # Check if Percy is enabled, caching the result so it is only checked once
     @staticmethod
     @lru_cache(maxsize=None)
     def is_percy_enabled():
         try:
             response = requests.get(f'{PERCY_CLI_API}/percy/healthcheck', timeout=10)
             response.raise_for_status()
             data = response.json()
 
             if not data['success']: raise CLIException(data['error'])
+            Environment.percy_build_id = data['build']['id']
+            Environment.percy_build_url = data['build']['url']
             version = response.headers.get('x-percy-core-version')
 
             if version.split('.')[0] != '1':
                 log(f'Unsupported Percy CLI version, {version}')
                 return False
 
             return True
@@ -43,16 +36,16 @@
             log('Percy is not running, disabling screenshots')
             log(e, on_debug=True)
             return False
 
     def post_screenshots(self, name, tag, tiles, external_debug_url=None, ignored_elements_data=None):
         body = self._request_body(name, tag, tiles, external_debug_url, ignored_elements_data)
 
-        body['client_info'] = CLIENT_INFO
-        body['environment_info'] = ENV_INFO
+        body['client_info'] = Environment._get_client_info()
+        body['environment_info'] = Environment._get_env_info()
 
         response = requests.post(f'{PERCY_CLI_API}/percy/comparison', json=body, timeout=30)
         # Handle errors
         response.raise_for_status()
         data = response.json()
 
         if response.status_code != 200:
```

### Comparing `percy-appium-app-1.2.1/percy/lib/ignore_region.py` & `percy-appium-app-1.2.2/percy/lib/ignore_region.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/lib/percy_options.py` & `percy-appium-app-1.2.2/percy/lib/percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/lib/tile.py` & `percy-appium-app-1.2.2/percy/lib/tile.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/metadata/android_metadata.py` & `percy-appium-app-1.2.2/percy/metadata/android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/metadata/ios_metadata.py` & `percy-appium-app-1.2.2/percy/metadata/ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/metadata/metadata.py` & `percy-appium-app-1.2.2/percy/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/providers/app_automate.py` & `percy-appium-app-1.2.2/percy/providers/app_automate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import os
 from percy.common import log
 from percy.lib.tile import Tile
 from percy.providers.generic_provider import GenericProvider
-
+from percy.environment import Environment
 
 class AppAutomate(GenericProvider):
     @staticmethod
     def supports(remote_url) -> bool:
         if isinstance(remote_url, str):
             if remote_url.rfind("browserstack" if os.getenv("AA_DOMAIN") is None else os.getenv("AA_DOMAIN")) > -1:
                 return True
@@ -63,16 +63,16 @@
 
     def execute_percy_screenshot_begin(self, name):
         try:
             request_body = {
                 'action': 'percyScreenshot',
                 'arguments': {
                     'state': 'begin',
-                    'percyBuildId':  os.getenv('PERCY_BUILD_ID', ''),
-                    'percyBuildUrl': os.getenv('PERCY_BUILD_URL', ''),
+                    'percyBuildId':  Environment.percy_build_id,
+                    'percyBuildUrl': Environment.percy_build_url,
                     'name': name
                 }
             }
             command = f'browserstack_executor: {json.dumps(request_body)}'
             response = self.metadata.execute_script(command)
             response = json.loads(response)
             return response
@@ -101,15 +101,15 @@
 
     def execute_percy_screenshot(self, device_height, screen_lengths, scrollable_xpath=None, scrollable_id=None, scale_factor=1):
         try:
             request_body = {
                 'action': 'percyScreenshot',
                 'arguments': {
                     'state': 'screenshot',
-                    'percyBuildId':  os.getenv('PERCY_BUILD_ID', ''),
+                    'percyBuildId':  Environment.percy_build_id,
                     'screenshotType': 'fullpage',
                     'scaleFactor': scale_factor,
                     'options': { 
                         "numOfTiles": screen_lengths,
                         "deviceHeight": device_height,
                         "scrollableXpath":  scrollable_xpath,
                         "scrollableId": scrollable_id
```

### Comparing `percy-appium-app-1.2.1/percy/providers/generic_provider.py` & `percy-appium-app-1.2.2/percy/providers/generic_provider.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/providers/provider_resolver.py` & `percy-appium-app-1.2.2/percy/providers/provider_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy/screenshot.py` & `percy-appium-app-1.2.2/percy/screenshot.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/percy_appium_app.egg-info/PKG-INFO` & `percy-appium-app-1.2.2/percy_appium_app.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: percy-appium-app
-Version: 1.2.1
+Version: 1.2.2
 Summary: Python client for visual testing with Percy for mobile apps
 Home-page: https://github.com/percy/percy-appium-python
 Author: Perceptual Inc.
 Author-email: team@percy.io
 License: MIT
 Keywords: appium percy visual testing
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `percy-appium-app-1.2.1/percy_appium_app.egg-info/SOURCES.txt` & `percy-appium-app-1.2.2/percy_appium_app.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 percy/__init__.py
+percy/environment.py
 percy/screenshot.py
 percy/version.py
 percy/common/__init__.py
 percy/configs/devices.json
 percy/errors/__init__.py
 percy/lib/__init__.py
 percy/lib/app_percy.py
```

### Comparing `percy-appium-app-1.2.1/setup.py` & `percy-appium-app-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_android_metadata.py` & `percy-appium-app-1.2.2/tests/test_android_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_app_automate.py` & `percy-appium-app-1.2.2/tests/test_app_automate.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_app_percy.py` & `percy-appium-app-1.2.2/tests/test_app_percy.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_cache.py` & `percy-appium-app-1.2.2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_cli_wrapper.py` & `percy-appium-app-1.2.2/tests/test_cli_wrapper.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_generic_provider.py` & `percy-appium-app-1.2.2/tests/test_generic_provider.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_ignore_region.py` & `percy-appium-app-1.2.2/tests/test_ignore_region.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_ios_metadata.py` & `percy-appium-app-1.2.2/tests/test_ios_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_metadata.py` & `percy-appium-app-1.2.2/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_metadata_resolver.py` & `percy-appium-app-1.2.2/tests/test_metadata_resolver.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_percy_options.py` & `percy-appium-app-1.2.2/tests/test_percy_options.py`

 * *Files identical despite different names*

### Comparing `percy-appium-app-1.2.1/tests/test_screenshot.py` & `percy-appium-app-1.2.2/tests/test_screenshot.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 mock_server_thread = Thread(target=mock_server.serve_forever)
 mock_server_thread.daemon = True
 mock_server_thread.start()
 
 
 # mock helpers
 def mock_healthcheck(fail=False, fail_how="error"):
-    health_body = '{ "success": true }'
+    health_body = '{ "success": true, "build": {"id": "123", "url": "dummy_url"} }'
     health_headers = {"X-Percy-Core-Version": "1.0.0"}
     health_status = 200
 
     if fail and fail_how == "error":
         health_body = '{ "success": false, "error": "test" }'
         health_status = 500
     elif fail and fail_how == "wrong-version":
```

### Comparing `percy-appium-app-1.2.1/tests/test_tile.py` & `percy-appium-app-1.2.2/tests/test_tile.py`

 * *Files identical despite different names*


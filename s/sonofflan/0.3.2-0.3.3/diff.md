# Comparing `tmp/sonofflan-0.3.2.tar.gz` & `tmp/sonofflan-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonofflan-0.3.2.tar", max compression
+gzip compressed data, was "sonofflan-0.3.3.tar", max compression
```

## Comparing `sonofflan-0.3.2.tar` & `sonofflan-0.3.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1458 2022-11-21 17:52:10.623161 sonofflan-0.3.2/LICENSE
--rw-r--r--   0        0        0      488 2023-05-12 15:14:40.556172 sonofflan-0.3.2/README.md
--rw-r--r--   0        0        0      902 2023-05-12 15:14:14.942222 sonofflan-0.3.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-28 12:04:41.616281 sonofflan-0.3.2/sonofflan/__init__.py
--rw-r--r--   0        0        0     6582 2023-02-27 10:28:28.454057 sonofflan-0.3.2/sonofflan/__main__.py
--rw-r--r--   0        0        0     5557 2023-05-12 15:10:55.961242 sonofflan-0.3.2/sonofflan/browser.py
--rw-r--r--   0        0        0     3643 2022-11-29 20:41:55.723131 sonofflan-0.3.2/sonofflan/config.py
--rw-r--r--   0        0        0     1718 2022-11-29 20:43:10.176848 sonofflan-0.3.2/sonofflan/crypto.py
--rw-r--r--   0        0        0     1075 2023-02-01 17:49:54.112559 sonofflan-0.3.2/sonofflan/devices/__init__.py
--rw-r--r--   0        0        0     6046 2023-03-03 17:28:39.151166 sonofflan-0.3.2/sonofflan/devices/device.py
--rw-r--r--   0        0        0     2957 2023-02-27 10:28:21.314009 sonofflan-0.3.2/sonofflan/devices/plug.py
--rw-r--r--   0        0        0     1939 2023-02-01 18:03:45.853996 sonofflan-0.3.2/sonofflan/devices/powerplug.py
--rw-r--r--   0        0        0     3216 2022-11-28 17:19:41.600376 sonofflan-0.3.2/sonofflan/devices/strip.py
--rw-r--r--   0        0        0     1719 2022-12-01 17:11:19.286906 sonofflan-0.3.2/sonofflan/devices/thermoplug.py
--rw-r--r--   0        0        0     1317 2023-02-01 17:40:10.765696 sonofflan-0.3.2/sonofflan/errors.py
--rw-r--r--   0        0        0      288 2022-11-24 18:38:28.778014 sonofflan-0.3.2/sonofflan/utils.py
--rw-r--r--   0        0        0     1444 1970-01-01 00:00:00.000000 sonofflan-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1458 2022-11-21 17:52:10.623161 sonofflan-0.3.3/LICENSE
+-rw-r--r--   0        0        0      488 2023-05-29 10:44:47.804529 sonofflan-0.3.3/README.md
+-rw-r--r--   0        0        0      902 2023-05-29 10:44:47.804529 sonofflan-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-28 12:04:41.616281 sonofflan-0.3.3/sonofflan/__init__.py
+-rw-r--r--   0        0        0     6582 2023-02-27 10:28:28.454057 sonofflan-0.3.3/sonofflan/__main__.py
+-rw-r--r--   0        0        0     5557 2023-05-12 15:10:55.961242 sonofflan-0.3.3/sonofflan/browser.py
+-rw-r--r--   0        0        0     3643 2022-11-29 20:41:55.723131 sonofflan-0.3.3/sonofflan/config.py
+-rw-r--r--   0        0        0     1718 2022-11-29 20:43:10.176848 sonofflan-0.3.3/sonofflan/crypto.py
+-rw-r--r--   0        0        0     1075 2023-02-01 17:49:54.112559 sonofflan-0.3.3/sonofflan/devices/__init__.py
+-rw-r--r--   0        0        0     6046 2023-03-03 17:28:39.151166 sonofflan-0.3.3/sonofflan/devices/device.py
+-rw-r--r--   0        0        0     2957 2023-02-27 10:28:21.314009 sonofflan-0.3.3/sonofflan/devices/plug.py
+-rw-r--r--   0        0        0     2096 2023-05-29 10:32:36.449103 sonofflan-0.3.3/sonofflan/devices/powerplug.py
+-rw-r--r--   0        0        0     3216 2022-11-28 17:19:41.600376 sonofflan-0.3.3/sonofflan/devices/strip.py
+-rw-r--r--   0        0        0     1719 2022-12-01 17:11:19.286906 sonofflan-0.3.3/sonofflan/devices/thermoplug.py
+-rw-r--r--   0        0        0     1317 2023-02-01 17:40:10.765696 sonofflan-0.3.3/sonofflan/errors.py
+-rw-r--r--   0        0        0      288 2022-11-24 18:38:28.778014 sonofflan-0.3.3/sonofflan/utils.py
+-rw-r--r--   0        0        0     1444 1970-01-01 00:00:00.000000 sonofflan-0.3.3/PKG-INFO
```

### Comparing `sonofflan-0.3.2/LICENSE` & `sonofflan-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/pyproject.toml` & `sonofflan-0.3.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sonofflan"
-version = "0.3.2"
+version = "0.3.3"
 description = "Library to interact with Sonoff devices through LAN mode (without eWeLink cloud)"
 authors = ["Danilo Treffiletti <urban82@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 keywords = ["sonoff", "ewelink", "itead"]
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `sonofflan-0.3.2/sonofflan/__main__.py` & `sonofflan-0.3.3/sonofflan/__main__.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/sonofflan/browser.py` & `sonofflan-0.3.3/sonofflan/browser.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/sonofflan/config.py` & `sonofflan-0.3.3/sonofflan/config.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/sonofflan/crypto.py` & `sonofflan-0.3.3/sonofflan/crypto.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/sonofflan/devices/__init__.py` & `sonofflan-0.3.3/sonofflan/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/sonofflan/devices/device.py` & `sonofflan-0.3.3/sonofflan/devices/device.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/sonofflan/devices/plug.py` & `sonofflan-0.3.3/sonofflan/devices/plug.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/sonofflan/devices/powerplug.py` & `sonofflan-0.3.3/sonofflan/devices/powerplug.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """Parse data from update"""
 
     if isinstance(value, str):
         return float(value)
     if isinstance(value, float):
         return value
     if isinstance(value, int):
-        return value / 100.0
+        return float(value)
 
     return 0
 
 
 class PowerPlug(Plug):
     """Sonoff plug with power meter
 
@@ -52,14 +52,18 @@
             Dictionary with data coming from Zeroconf
         """
 
         super()._update(data)
         self._voltage = _parse_data(data['data']['voltage'])
         self._current = _parse_data(data['data']['current'])
         self._power = _parse_data(data['data']['power'])
+        if "switches" in data['data']:  # New Power R3
+            self._voltage /= 100.0
+            self._current /= 100.0
+            self._power /= 100.0
 
     def _repr(self) -> str:
         """Internal representation method"""
 
         return super()._repr() + f" V:{self._voltage}V C:{self._current}A P:{self._power}W"
 
     @property
```

### Comparing `sonofflan-0.3.2/sonofflan/devices/strip.py` & `sonofflan-0.3.3/sonofflan/devices/strip.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/sonofflan/devices/thermoplug.py` & `sonofflan-0.3.3/sonofflan/devices/thermoplug.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/sonofflan/errors.py` & `sonofflan-0.3.3/sonofflan/errors.py`

 * *Files identical despite different names*

### Comparing `sonofflan-0.3.2/PKG-INFO` & `sonofflan-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonofflan
-Version: 0.3.2
+Version: 0.3.3
 Summary: Library to interact with Sonoff devices through LAN mode (without eWeLink cloud)
 License: BSD-3-Clause
 Keywords: sonoff,ewelink,itead
 Author: Danilo Treffiletti
 Author-email: urban82@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -28,15 +28,15 @@
 Library to interact with Sonoff devices through LAN mode (without eWeLink cloud) with firmware
 version 3+ (tested up to version 3.7.0).
 
 Author: Danilo Treffiletti <urban82@gmail.com>
 
 License: BSD-3
 
-Version: 0.3.2
+Version: 0.3.3
 
 ## Install
 
 ### Requirements
 * Python 3.9+
 
 ## Usage
```


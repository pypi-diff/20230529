# Comparing `tmp/tradernet_sdk-0.3.8.tar.gz` & `tmp/tradernet_sdk-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tradernet_sdk-0.3.8.tar", max compression
+gzip compressed data, was "tradernet_sdk-0.3.9.tar", max compression
```

## Comparing `tradernet_sdk-0.3.8.tar` & `tradernet_sdk-0.3.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1131 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/LICENSE
--rw-r--r--   0        0        0     4024 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/README.md
--rw-r--r--   0        0        0     1008 2023-05-15 11:16:42.031851 tradernet_sdk-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     1305 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/PublicApiClient.py
--rw-r--r--   0        0        0      583 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/__init__.py
--rw-r--r--   0        0        0    32923 2023-05-04 19:07:13.429662 tradernet_sdk-0.3.8/tradernet/client.py
--rw-r--r--   0        0        0      283 2023-05-04 19:07:13.429662 tradernet_sdk-0.3.8/tradernet/common/__init__.py
--rw-r--r--   0        0        0      565 2023-05-04 19:08:23.526279 tradernet_sdk-0.3.8/tradernet/common/file_utils.py
--rw-r--r--   0        0        0     2238 2023-05-04 19:02:07.994968 tradernet_sdk-0.3.8/tradernet/common/netutils.py
--rw-r--r--   0        0        0     7327 2023-05-04 19:07:13.429662 tradernet_sdk-0.3.8/tradernet/common/string_utils.py
--rw-r--r--   0        0        0     2858 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/common/ws_utils.py
--rw-r--r--   0        0        0    11653 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/core.py
--rw-r--r--   0        0        0        0 2023-05-15 11:16:15.403351 tradernet_sdk-0.3.8/tradernet/symbols/__init__.py
--rw-r--r--   0        0        0     6329 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/symbols/base_market_symbol.py
--rw-r--r--   0        0        0     4151 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/symbols/base_option_symbol.py
--rw-r--r--   0        0        0     2836 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/symbols/das_option.py
--rw-r--r--   0        0        0      290 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/symbols/option_properties.py
--rw-r--r--   0        0        0     2132 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/symbols/tradernet_option.py
--rw-r--r--   0        0        0     2336 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/symbols/tradernet_symbol.py
--rw-r--r--   0        0        0     3016 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/tradernet_wsapi.py
--rw-r--r--   0        0        0     6996 2023-05-04 18:16:09.806172 tradernet_sdk-0.3.8/tradernet/trading.py
--rw-r--r--   0        0        0     4915 1970-01-01 00:00:00.000000 tradernet_sdk-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-05-29 06:39:57.348645 tradernet_sdk-0.3.9/LICENSE
+-rw-r--r--   0        0        0     4024 2023-05-29 06:39:57.348645 tradernet_sdk-0.3.9/README.md
+-rw-r--r--   0        0        0     1008 2023-05-29 06:48:41.486559 tradernet_sdk-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0     1305 2023-05-29 06:39:57.348645 tradernet_sdk-0.3.9/tradernet/PublicApiClient.py
+-rw-r--r--   0        0        0      583 2023-05-29 06:39:57.348645 tradernet_sdk-0.3.9/tradernet/__init__.py
+-rw-r--r--   0        0        0    32923 2023-05-29 06:39:57.348645 tradernet_sdk-0.3.9/tradernet/client.py
+-rw-r--r--   0        0        0      283 2023-05-29 06:39:57.348645 tradernet_sdk-0.3.9/tradernet/common/__init__.py
+-rw-r--r--   0        0        0      565 2023-05-29 06:39:57.348645 tradernet_sdk-0.3.9/tradernet/common/file_utils.py
+-rw-r--r--   0        0        0     2238 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/common/netutils.py
+-rw-r--r--   0        0        0     7327 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/common/string_utils.py
+-rw-r--r--   0        0        0     2858 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/common/ws_utils.py
+-rw-r--r--   0        0        0    11786 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/core.py
+-rw-r--r--   0        0        0        0 2023-05-29 06:48:18.762129 tradernet_sdk-0.3.9/tradernet/symbols/__init__.py
+-rw-r--r--   0        0        0     6329 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/symbols/base_market_symbol.py
+-rw-r--r--   0        0        0     4151 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/symbols/base_option_symbol.py
+-rw-r--r--   0        0        0     2836 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/symbols/das_option.py
+-rw-r--r--   0        0        0      290 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/symbols/option_properties.py
+-rw-r--r--   0        0        0     2132 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/symbols/tradernet_option.py
+-rw-r--r--   0        0        0     2336 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/symbols/tradernet_symbol.py
+-rw-r--r--   0        0        0     3016 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/tradernet_wsapi.py
+-rw-r--r--   0        0        0     6996 2023-05-29 06:39:57.352645 tradernet_sdk-0.3.9/tradernet/trading.py
+-rw-r--r--   0        0        0     4915 1970-01-01 00:00:00.000000 tradernet_sdk-0.3.9/PKG-INFO
```

### Comparing `tradernet_sdk-0.3.8/LICENSE` & `tradernet_sdk-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/README.md` & `tradernet_sdk-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/pyproject.toml` & `tradernet_sdk-0.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tradernet-sdk"
-version = "0.3.8"
+version = "0.3.9"
 description = "Public API for TraderNet"
 authors = ["Anton Kudelin <a.kudelin@freedomfinance.eu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://tradernet.ru/tradernet-api/python-sdk"
 packages = [
     {include = "tradernet"}
```

### Comparing `tradernet_sdk-0.3.8/tradernet/PublicApiClient.py` & `tradernet_sdk-0.3.9/tradernet/PublicApiClient.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/__init__.py` & `tradernet_sdk-0.3.9/tradernet/__init__.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/client.py` & `tradernet_sdk-0.3.9/tradernet/client.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/common/file_utils.py` & `tradernet_sdk-0.3.9/tradernet/common/file_utils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/common/netutils.py` & `tradernet_sdk-0.3.9/tradernet/common/netutils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/common/string_utils.py` & `tradernet_sdk-0.3.9/tradernet/common/string_utils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/common/ws_utils.py` & `tradernet_sdk-0.3.9/tradernet/common/ws_utils.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/core.py` & `tradernet_sdk-0.3.9/tradernet/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,17 +124,19 @@
         # pylint: disable=protected-access
         core = cls(
             instance.public,
             instance._private,
             instance.login,
             instance._password
         )
+
         # Avoiding out of sync sessions
         if not instance._session_id:
             instance.get_authorized()
+
         core._session_id = instance._session_id
         core._session_time = instance._session_time
 
         return core
 
     @property
     def url(self) -> str:
@@ -182,18 +184,22 @@
         url = f'{self.url}/api/check-login-password'
         message = {
             'login': self.login, 'password': self._password, 'remember_me': 1
         }
         response = self.request('post', url, params=message)
         result = response.json()
         self.logger.debug('Authorization result: %s', result)
-        # Setting session key
-        self._session_id = result['SID']
-        # Setting timer
-        self._session_time = datetime.now()
+
+        if 'SID' in result:
+            # Setting session key
+            self._session_id = result['SID']
+            # Setting timer
+            self._session_time = datetime.now()
+        else:
+            self.logger.warning('Cannot obtain session ID: %s', result)
 
     def plain_request(
         self,
         cmd: str,
         params: dict[str, Any] | None = None
     ) -> Any:
         """
```

### Comparing `tradernet_sdk-0.3.8/tradernet/symbols/base_market_symbol.py` & `tradernet_sdk-0.3.9/tradernet/symbols/base_market_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/symbols/base_option_symbol.py` & `tradernet_sdk-0.3.9/tradernet/symbols/base_option_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/symbols/das_option.py` & `tradernet_sdk-0.3.9/tradernet/symbols/das_option.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/symbols/tradernet_option.py` & `tradernet_sdk-0.3.9/tradernet/symbols/tradernet_option.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/symbols/tradernet_symbol.py` & `tradernet_sdk-0.3.9/tradernet/symbols/tradernet_symbol.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/tradernet_wsapi.py` & `tradernet_sdk-0.3.9/tradernet/tradernet_wsapi.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/tradernet/trading.py` & `tradernet_sdk-0.3.9/tradernet/trading.py`

 * *Files identical despite different names*

### Comparing `tradernet_sdk-0.3.8/PKG-INFO` & `tradernet_sdk-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tradernet-sdk
-Version: 0.3.8
+Version: 0.3.9
 Summary: Public API for TraderNet
 Home-page: https://tradernet.ru/tradernet-api/python-sdk
 License: MIT
 Author: Anton Kudelin
 Author-email: a.kudelin@freedomfinance.eu
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


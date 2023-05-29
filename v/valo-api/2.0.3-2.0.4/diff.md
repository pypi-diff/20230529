# Comparing `tmp/valo_api-2.0.3.tar.gz` & `tmp/valo_api-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valo_api-2.0.3.tar", max compression
+gzip compressed data, was "valo_api-2.0.4.tar", max compression
```

## Comparing `valo_api-2.0.3.tar` & `valo_api-2.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1074 2023-05-07 18:57:50.442208 valo_api-2.0.3/LICENSE
--rw-r--r--   0        0        0     2451 2023-05-07 18:57:50.442208 valo_api-2.0.3/README.md
--rw-r--r--   0        0        0     3115 2023-05-07 18:57:50.442208 valo_api-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      388 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/__init__.py
--rw-r--r--   0        0        0      793 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/config.py
--rw-r--r--   0        0        0     5825 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/endpoint.py
--rw-r--r--   0        0        0      405 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/endpoints/__init__.py
--rw-r--r--   0        0        0    11908 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/endpoints_config.py
--rw-r--r--   0        0        0        0 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/exceptions/__init__.py
--rw-r--r--   0        0        0     1088 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/exceptions/rate_limit.py
--rw-r--r--   0        0        0     2069 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/exceptions/valo_api_exception.py
--rw-r--r--   0        0        0        0 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/__init__.py
--rw-r--r--   0        0        0      410 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/account_details.py
--rw-r--r--   0        0        0      541 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/competitive_updates_raw.py
--rw-r--r--   0        0        0      858 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/content.py
--rw-r--r--   0        0        0      371 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/error_response.py
--rw-r--r--   0        0        0      917 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/leaderboard.py
--rw-r--r--   0        0        0     1169 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/lifetime_match.py
--rw-r--r--   0        0        0     5550 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/match_details_raw.py
--rw-r--r--   0        0        0     5996 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/match_history.py
--rw-r--r--   0        0        0      299 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/match_history_raw.py
--rw-r--r--   0        0        0     1317 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/mmr_details.py
--rw-r--r--   0        0        0      628 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/mmr_history.py
--rw-r--r--   0        0        0     1306 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/mmr_raw.py
--rw-r--r--   0        0        0      817 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/status.py
--rw-r--r--   0        0        0     1093 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/store_featured.py
--rw-r--r--   0        0        0      853 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/store_offers.py
--rw-r--r--   0        0        0      157 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/version_info.py
--rw-r--r--   0        0        0      236 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/responses/website.py
--rw-r--r--   0        0        0        0 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/utils/__init__.py
--rw-r--r--   0        0        0      216 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/utils/dict_struct.py
--rw-r--r--   0        0        0     3821 2023-05-07 18:57:50.614219 valo_api-2.0.3/valo_api/utils/fetch_endpoint.py
--rw-r--r--   0        0        0     3838 1970-01-01 00:00:00.000000 valo_api-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-29 13:53:53.177282 valo_api-2.0.4/LICENSE
+-rw-r--r--   0        0        0     2451 2023-05-29 13:53:53.177282 valo_api-2.0.4/README.md
+-rw-r--r--   0        0        0     3115 2023-05-29 13:53:53.177282 valo_api-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/__init__.py
+-rw-r--r--   0        0        0      793 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/config.py
+-rw-r--r--   0        0        0     5952 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/endpoint.py
+-rw-r--r--   0        0        0      405 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/endpoints/__init__.py
+-rw-r--r--   0        0        0    11908 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/endpoints_config.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/exceptions/__init__.py
+-rw-r--r--   0        0        0     1088 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/exceptions/rate_limit.py
+-rw-r--r--   0        0        0     2069 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/exceptions/valo_api_exception.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/__init__.py
+-rw-r--r--   0        0        0      410 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/account_details.py
+-rw-r--r--   0        0        0      541 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/competitive_updates_raw.py
+-rw-r--r--   0        0        0      858 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/content.py
+-rw-r--r--   0        0        0      371 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/error_response.py
+-rw-r--r--   0        0        0      917 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/leaderboard.py
+-rw-r--r--   0        0        0     1169 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/lifetime_match.py
+-rw-r--r--   0        0        0     5550 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/match_details_raw.py
+-rw-r--r--   0        0        0     5996 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/match_history.py
+-rw-r--r--   0        0        0      299 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/match_history_raw.py
+-rw-r--r--   0        0        0     1317 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/mmr_details.py
+-rw-r--r--   0        0        0      628 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/mmr_history.py
+-rw-r--r--   0        0        0     1306 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/mmr_raw.py
+-rw-r--r--   0        0        0      817 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/status.py
+-rw-r--r--   0        0        0     1093 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/store_featured.py
+-rw-r--r--   0        0        0      853 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/store_offers.py
+-rw-r--r--   0        0        0      157 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/version_info.py
+-rw-r--r--   0        0        0      236 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/responses/website.py
+-rw-r--r--   0        0        0        0 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/utils/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/utils/dict_struct.py
+-rw-r--r--   0        0        0     4149 2023-05-29 13:53:53.329283 valo_api-2.0.4/valo_api/utils/fetch_endpoint.py
+-rw-r--r--   0        0        0     3639 1970-01-01 00:00:00.000000 valo_api-2.0.4/PKG-INFO
```

### Comparing `valo_api-2.0.3/LICENSE` & `valo_api-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/README.md` & `valo_api-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/pyproject.toml` & `valo_api-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "valo_api"
-version = "2.0.3"
+version = "2.0.4"
 description = "Valorant API Wrapper for https://github.com/Henrik-3/unofficial-valorant-api"
 readme = "README.md"
 authors = ["Manuel Raimann <raimannma@outlook.de>"]
 license = "MIT"
 repository = "https://github.com/raimannma/ValorantAPI"
 homepage = "https://github.com/raimannma/ValorantAPI"
 
@@ -27,23 +27,23 @@
 [tool.poetry.scripts]
 "valo_api" = "valo_api.__main__:app"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.1"
 Pillow = "^9.2.0"
-msgspec = ">=0.12,<0.15"
+msgspec = ">=0.12,<0.16"
 asyncio = {version = "^3.4.3", optional = true, extras = ["speedups"]}
 aiohttp = {version = "^3.8.3", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.5"
 black = {version = "^23.3.0", allow-prereleases = true}
 isort = "^5.12.0"
-mypy = ">=0.991,<1.3"
+mypy = ">=0.991,<1.4"
 mypy-extensions = ">=0.4.3,<1.1.0"
 pre-commit = "^3.2.2"
 pydocstyle = "^6.3.0"
 pylint = "^2.17.2"
 pytest = "^7.3.1"
 hypothesis = "^6.61.0"
 pyupgrade = "^3.3.1"
```

### Comparing `valo_api-2.0.3/valo_api/config.py` & `valo_api-2.0.4/valo_api/config.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/endpoint.py` & `valo_api-2.0.4/valo_api/endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     Type,
     TypeVar,
     Union,
     get_args,
 )
 
 import io
+import json
 from dataclasses import dataclass
 
 import msgspec
 from PIL import Image
 from requests import Response
 
 from valo_api.exceptions.valo_api_exception import ValoAPIException
@@ -129,14 +130,17 @@
         return filtered_query_args
 
     def _get_endpoint(self, *args, **kwargs) -> R:
         args_insert = [a for a in args]
         for k in self.kwargs.keys():
             if k not in kwargs or kwargs[k] is None or kwargs[k] == "":
                 kwargs[k] = args_insert.pop(0) if len(args_insert) > 0 else ""
+        kwargs = {
+            k: json.dumps(v) if isinstance(v, dict) else v for k, v in kwargs.items()
+        }
         response = fetch_endpoint(
             self.path,
             method=self.method,
             query_args=self.build_query_args(**kwargs),
             **kwargs,
         )
         return self.parse_response(response, response.content)
```

### Comparing `valo_api-2.0.3/valo_api/endpoints_config.py` & `valo_api-2.0.4/valo_api/endpoints_config.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/exceptions/rate_limit.py` & `valo_api-2.0.4/valo_api/exceptions/rate_limit.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/exceptions/valo_api_exception.py` & `valo_api-2.0.4/valo_api/exceptions/valo_api_exception.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/competitive_updates_raw.py` & `valo_api-2.0.4/valo_api/responses/competitive_updates_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/content.py` & `valo_api-2.0.4/valo_api/responses/content.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/leaderboard.py` & `valo_api-2.0.4/valo_api/responses/leaderboard.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/lifetime_match.py` & `valo_api-2.0.4/valo_api/responses/lifetime_match.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/match_details_raw.py` & `valo_api-2.0.4/valo_api/responses/match_details_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/match_history.py` & `valo_api-2.0.4/valo_api/responses/match_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/mmr_details.py` & `valo_api-2.0.4/valo_api/responses/mmr_details.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/mmr_history.py` & `valo_api-2.0.4/valo_api/responses/mmr_history.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/mmr_raw.py` & `valo_api-2.0.4/valo_api/responses/mmr_raw.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/status.py` & `valo_api-2.0.4/valo_api/responses/status.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/store_featured.py` & `valo_api-2.0.4/valo_api/responses/store_featured.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/responses/store_offers.py` & `valo_api-2.0.4/valo_api/responses/store_offers.py`

 * *Files identical despite different names*

### Comparing `valo_api-2.0.3/valo_api/utils/fetch_endpoint.py` & `valo_api-2.0.4/valo_api/utils/fetch_endpoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from typing import Any, Dict, Optional, Type, TypeVar
 
+import json
 import os
 import urllib.parse
 
 import requests
 from requests import Response
 
 from valo_api.config import Config
@@ -82,14 +83,17 @@
     fetch_endpoint.session = (
         fetch_endpoint.session
         if hasattr(fetch_endpoint, "session")
         else requests.Session()
     )
     url = parse_endpoint(endpoint_definition, **kwargs)
     headers = get_headers()
+    if "queries" in query_args and query_args["queries"] is not None:
+        queries = json.loads(query_args["queries"])
+        query_args["queries"] = f"?{urllib.parse.urlencode(queries)}"
     response = fetch_endpoint.session.request(
         method, url, params=query_args, json=query_args, headers=headers
     )
     set_rate_limit(response.headers)
     return response
 
 
@@ -116,14 +120,16 @@
         fetch_endpoint_async.session = (
             fetch_endpoint_async.session
             if hasattr(fetch_endpoint_async, "session")
             else aiohttp.ClientSession()
         )
         url = parse_endpoint(endpoint_definition, **kwargs)
         headers = get_headers()
+        if "queries" in query_args:
+            query_args["queries"] = f"?{urllib.parse.urlencode(query_args['queries'])}"
         async with fetch_endpoint_async.session.request(
             method, url, params=query_args, json=query_args, headers=headers
         ) as response:
             set_rate_limit(response.headers)
             return response, await response.read()
 
 except ImportError:
```

### Comparing `valo_api-2.0.3/PKG-INFO` & `valo_api-2.0.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valo-api
-Version: 2.0.3
+Version: 2.0.4
 Summary: Valorant API Wrapper for https://github.com/Henrik-3/unofficial-valorant-api
 Home-page: https://github.com/raimannma/ValorantAPI
 License: MIT
 Author: Manuel Raimann
 Author-email: raimannma@outlook.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,24 +12,20 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: async
 Requires-Dist: Pillow (>=9.2.0,<10.0.0)
 Requires-Dist: aiohttp (>=3.8.3,<4.0.0) ; extra == "async"
 Requires-Dist: asyncio[speedups] (>=3.4.3,<4.0.0) ; extra == "async"
-Requires-Dist: msgspec (>=0.12,<0.15)
+Requires-Dist: msgspec (>=0.12,<0.16)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Project-URL: Repository, https://github.com/raimannma/ValorantAPI
 Description-Content-Type: text/markdown
 
 # valo_api
 
 <div align="center">
```


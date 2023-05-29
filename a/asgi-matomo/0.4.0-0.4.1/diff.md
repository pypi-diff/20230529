# Comparing `tmp/asgi_matomo-0.4.0.tar.gz` & `tmp/asgi_matomo-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asgi_matomo-0.4.0.tar", max compression
+gzip compressed data, was "asgi_matomo-0.4.1.tar", max compression
```

## Comparing `asgi_matomo-0.4.0.tar` & `asgi_matomo-0.4.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/LICENSE
--rw-r--r--   0        0        0     5574 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/README.md
--rw-r--r--   0        0        0      186 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/asgi_matomo/__init__.py
--rw-r--r--   0        0        0    13164 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/asgi_matomo/middleware.py
--rw-r--r--   0        0        0        0 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/asgi_matomo/py.typed
--rw-r--r--   0        0        0     1024 2023-05-25 18:35:48.385600 asgi_matomo-0.4.0/asgi_matomo/trackers.py
--rw-r--r--   0        0        0     1072 2023-05-25 18:35:48.389600 asgi_matomo-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6463 1970-01-01 00:00:00.000000 asgi_matomo-0.4.0/setup.py
--rw-r--r--   0        0        0     6307 1970-01-01 00:00:00.000000 asgi_matomo-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-29 12:46:42.511300 asgi_matomo-0.4.1/LICENSE
+-rw-r--r--   0        0        0     5896 2023-05-29 12:46:42.511300 asgi_matomo-0.4.1/README.md
+-rw-r--r--   0        0        0      186 2023-05-29 12:46:42.511300 asgi_matomo-0.4.1/asgi_matomo/__init__.py
+-rw-r--r--   0        0        0    13453 2023-05-29 12:46:42.511300 asgi_matomo-0.4.1/asgi_matomo/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:46:42.511300 asgi_matomo-0.4.1/asgi_matomo/py.typed
+-rw-r--r--   0        0        0     1024 2023-05-29 12:46:42.511300 asgi_matomo-0.4.1/asgi_matomo/trackers.py
+-rw-r--r--   0        0        0     1072 2023-05-29 12:46:42.511300 asgi_matomo-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     6793 1970-01-01 00:00:00.000000 asgi_matomo-0.4.1/setup.py
+-rw-r--r--   0        0        0     6629 1970-01-01 00:00:00.000000 asgi_matomo-0.4.1/PKG-INFO
```

### Comparing `asgi_matomo-0.4.0/LICENSE` & `asgi_matomo-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.4.0/README.md` & `asgi_matomo-0.4.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -161,14 +161,22 @@
 
 This project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).
 
 # Releas Notes
 
 ## Latest Changes
 
+## [0.4.1] - 2023-05-29
+
+### Added
+- track urlref. PR [#21](https://github.com/spraakbanken/asgi-matomo/pull/21) by [@kod-kristoff](https://github.com/kod-kristoff).
+
+### Changed
+- respect x-forwarded-for. PR [#18](https://github.com/spraakbanken/asgi-matomo/pull/18) by [@kod-kristoff](https://github.com/kod-kristoff).
+
 ## [0.4.0] - 2023-05-25
 
 * Handle lifespan correctly. PR [#13](https://github.com/spraakbanken/asgi-matomo/pull/13) by [@kod-kristoff](https://github.com/kod-kristoff).
 * add docs. PR [#11](https://github.com/spraakbanken/asgi-matomo/pull/11) by [@kod-kristoff](https://github.com/kod-kristoff).
 ## [0.3.2] - 2023-05-23
 
 * feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).
```

### Comparing `asgi_matomo-0.4.0/asgi_matomo/middleware.py` & `asgi_matomo-0.4.1/asgi_matomo/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
     async def __call__(
         self, scope: HTTPScope, receive: ASGIReceiveCallable, send: ASGISendCallable
     ) -> Any:
         # locals inside the app function (send_wrapper) can't be assigned to,
         # as the interpreter detects the assignment and thus creates a new
         # local variable within that function, with that name.
-        instance = {"http_status_code": None}
+        instance = {"http_status_code": 500}
 
         def send_wrapper(response):
             if response["type"] == "http.response.start":
                 instance["http_status_code"] = response["status"]
             return send(response)
 
         if scope["type"] == "lifespan":
@@ -270,24 +270,29 @@
             except httpx.HTTPError:
                 logger.exception("Error tracking view")
 
     def _build_tracking_state(self, scope: HTTPScope) -> dict:
         server = None
         user_agent = None
         accept_lang = None
+        cip = None
         path = scope["path"]
+        urlref = None
 
         for header, value in scope["headers"]:
             if header == b"accept_lang":
                 accept_lang = value
-
             elif header == b"user-agent":
                 user_agent = value
             elif header == b"x-forwarded-server":
                 server = value.decode("utf-8")
+            elif header == b"x-forwarded-for":
+                cip = value.decode("utf-8")
+            elif header == b"referer":
+                urlref = value
         if server is None:
             if scope["server"] is None:
                 logger.error("'server' is not set in scope, skip tracking...")
                 raise RuntimeError("'server' is not set in scope")
             host, port = scope["server"]
             logger.debug(
                 "setting server from scope", extra={"host": host, "port": port}
@@ -321,15 +326,16 @@
                 server,
                 path,
                 "",
                 str(scope["query_string"]) if scope.get("query_string") else None,
             )
         )
 
-        cip = scope["client"][0] if scope["client"] else None
+        if not cip:
+            cip = scope["client"][0] if scope["client"] else None
 
         tracking_state = {
             "idsite": self.idsite,
             "action_name": scope["path"],
             "url": url,
             "rec": 1,
             "rand": random.getrandbits(32),
@@ -341,8 +347,10 @@
         if scope["path"] in self.route_details:
             tracking_state |= self.route_details[scope["path"]]
         if self.access_token and cip:
             tracking_state["token_auth"] = self.access_token
             tracking_state["cip"] = cip
         if accept_lang:
             tracking_state["lang"] = accept_lang
+        if urlref:
+            tracking_state["urlref"] = urlref
         return tracking_state
```

### Comparing `asgi_matomo-0.4.0/asgi_matomo/trackers.py` & `asgi_matomo-0.4.1/asgi_matomo/trackers.py`

 * *Files identical despite different names*

### Comparing `asgi_matomo-0.4.0/pyproject.toml` & `asgi_matomo-0.4.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asgi-matomo"
-version = "0.4.0"
+version = "0.4.1"
 description = "Middleware for tracking ASGI reqeusts with Matomo"
 authors = ["Kristoffer Andersson <kristoffer.andersson@gu.se>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://spraakbanken.gu.se"
 repository = "https://github.com/spraakbanken/asgi-matomo"
 packages = [{include = "asgi_matomo"}]
```

### Comparing `asgi_matomo-0.4.0/setup.py` & `asgi_matomo-0.4.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['asgiref>=3.6.0,<4.0.0', 'httpx>=0.24.0,<0.25.0']
 
 setup_kwargs = {
     'name': 'asgi-matomo',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Middleware for tracking ASGI reqeusts with Matomo',
-    'long_description': '# asgi-matomo\n[![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)\n[![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)\n[![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)\n\nTracking requests with Matomo from ASGI apps.\n\n`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.). The intended usage is for api tracking (backends).\n\n**Note** If you serve HTML (directly or by templates), it is suggested to track those parts through Matomo\'s javascript tracking.\n\n**Installation**\n\n```bash\npip install asgi-matomo\n```\n\n## What is tracked\n\nCurrently this middleware tracks:\n- `url`\n- `ua`: user_agent\n- `gt_ms`: mesaured as the time before and after this middleware call next in the asgi stack.\n- `send_image=0` for performance issues\n- `cvar` with at least `http_status_code` and `http_method` set.\n- `lang` if `accept-lang` is set\n- `cip` client ip, **requires** `access_token` to be given.\n- `action_name` that defaults to path, but can be specified.\n\nYou can also pass variable to track by adding an `asgi_matomo`  dict in the `state` dict of the ASGI `scope`:\n```python\nscope = {\n  "state": {\n    "asgi_matomo": {\n      "e_a": "Playing",\n      "cvar": {\n        "your": "custom",\n        "data": "here",\n      }\n    }\n  }\n}\n```\n\nThe keys of the `asgi_matomo` dict is expected to be valid parameter for the [Matomo HTTP Tracking API](https://developer.matomo.org/api-reference/tracking-api). `cvar` is serialized with the standard `json` lib.\n\nYou can also track time spent on different tasks with `trackers.PerfMsTracker`.\n```python\nimport asyncio\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\nfrom asgi_matomo.trackers import PerfMsTracker\n\nasync def homepage(request):\n    async with PerfMsTracker(scope=request.scope, key="pf_srv"):\n        # fetch/compute data\n        await asyncio.sleep(1)\n        data = {"data": "a"*4000}\n    return JSONResponse(data)\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n## Examples\n\n### Starlette\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\n\nasync def homepage(request):\n    return JSONResponse({"data": "a" * 4000})\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n### FastAPI\n\n```python\nfrom fastapi import FastAPI\nfrom asgi_matomo import MatomoMiddleware\n\napp = FastAPI()\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n)\n\n@app.get("/")\ndef home() -> dict:\n    return {"data": "a" * 4000}\n```\n\n## API Reference\n\n**Overview**\n\n```python\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n  access_token="SECRETTOKEN",\n  assume_https=True,\n  exclude_paths=["/health"],\n  exclude_patterns=[".*/old.*"],\n  route_details={\n    "route": {\n      "action_name": "Name",\n    }\n  }\n)\n```\n\n**Parameters**:\n\n- **(Required)** `matomo_url`: The URL to make your tracking calls to.\n- **(Required)** `idsite`: The tracking id for your service.\n- _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.\n- _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.\n- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`. Defaults to `None`.\n- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match. Defaults to `None`.\nThese are tried after `exclude_paths`.\n- _(Optional)_ `route_details`: A dict with custom route-specific tracking data. Defaults to `None`.\n\n\n**Notes**:\n\n- Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.\n\n## Ideas for further work:\n- [x] _filtering tracked of urls_\n- [x] _custom extraction of tracked data_\n\n\nThis project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).\n\n# Releas Notes\n\n## Latest Changes\n\n## [0.4.0] - 2023-05-25\n\n* Handle lifespan correctly. PR [#13](https://github.com/spraakbanken/asgi-matomo/pull/13) by [@kod-kristoff](https://github.com/kod-kristoff).\n* add docs. PR [#11](https://github.com/spraakbanken/asgi-matomo/pull/11) by [@kod-kristoff](https://github.com/kod-kristoff).\n## [0.3.2] - 2023-05-23\n\n* feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).\n\n## [0.3.0] - 2023-05-22\n### Added\n\n- Allow setting route-details\n\n',
+    'long_description': '# asgi-matomo\n[![Packaging status](https://img.shields.io/pypi/v/asgi-matomo?color=%2334D058&label=pypi%20package)](https://pypi.org/project/asgi-matomo)\n[![CI](https://github.com/spraakbanken/asgi-matomo/workflows/CI/badge.svg)](https://github.com/spraakbanken/asgi-matomo/actions?query=workflow%3ACI)\n[![codecov](https://codecov.io/gh/spraakbanken/asgi-matomo/branch/main/graph/badge.svg?token=MRJZVCJQF5)](https://codecov.io/gh/spraakbanken/asgi-matomo)\n\nTracking requests with Matomo from ASGI apps.\n\n`MatomoMiddleware` adds tracking of all requests to Matomo to ASGI applications (Starlette, FastAPI, Quart, etc.). The intended usage is for api tracking (backends).\n\n**Note** If you serve HTML (directly or by templates), it is suggested to track those parts through Matomo\'s javascript tracking.\n\n**Installation**\n\n```bash\npip install asgi-matomo\n```\n\n## What is tracked\n\nCurrently this middleware tracks:\n- `url`\n- `ua`: user_agent\n- `gt_ms`: mesaured as the time before and after this middleware call next in the asgi stack.\n- `send_image=0` for performance issues\n- `cvar` with at least `http_status_code` and `http_method` set.\n- `lang` if `accept-lang` is set\n- `cip` client ip, **requires** `access_token` to be given.\n- `action_name` that defaults to path, but can be specified.\n\nYou can also pass variable to track by adding an `asgi_matomo`  dict in the `state` dict of the ASGI `scope`:\n```python\nscope = {\n  "state": {\n    "asgi_matomo": {\n      "e_a": "Playing",\n      "cvar": {\n        "your": "custom",\n        "data": "here",\n      }\n    }\n  }\n}\n```\n\nThe keys of the `asgi_matomo` dict is expected to be valid parameter for the [Matomo HTTP Tracking API](https://developer.matomo.org/api-reference/tracking-api). `cvar` is serialized with the standard `json` lib.\n\nYou can also track time spent on different tasks with `trackers.PerfMsTracker`.\n```python\nimport asyncio\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\nfrom asgi_matomo.trackers import PerfMsTracker\n\nasync def homepage(request):\n    async with PerfMsTracker(scope=request.scope, key="pf_srv"):\n        # fetch/compute data\n        await asyncio.sleep(1)\n        data = {"data": "a"*4000}\n    return JSONResponse(data)\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n## Examples\n\n### Starlette\n\n```python\nfrom starlette.applications import Starlette\nfrom starlette.responses import JSONResponse\nfrom starlette.routing import Route\nfrom starlette.middleware import Middleware\n\nfrom asgi_matomo import MatomoMiddleware\n\nasync def homepage(request):\n    return JSONResponse({"data": "a" * 4000})\n\napp = Starlette(\n  routes=[Route("/", homepage)],\n  middleware=[\n    Middleware(\n      MatomoMiddleware,\n      matomo_url="YOUR MATOMO TRACKING URL",\n      idsite=12345, # your service tracking id\n  )],\n)\n```\n\n### FastAPI\n\n```python\nfrom fastapi import FastAPI\nfrom asgi_matomo import MatomoMiddleware\n\napp = FastAPI()\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n)\n\n@app.get("/")\ndef home() -> dict:\n    return {"data": "a" * 4000}\n```\n\n## API Reference\n\n**Overview**\n\n```python\napp.add_middleware(\n  MatomoMiddleware,\n  matomo_url="YOUR MATOMO TRACKING URL",\n  idsite=12345, # your service tracking id\n  access_token="SECRETTOKEN",\n  assume_https=True,\n  exclude_paths=["/health"],\n  exclude_patterns=[".*/old.*"],\n  route_details={\n    "route": {\n      "action_name": "Name",\n    }\n  }\n)\n```\n\n**Parameters**:\n\n- **(Required)** `matomo_url`: The URL to make your tracking calls to.\n- **(Required)** `idsite`: The tracking id for your service.\n- _(Optional)_ `access_token`: Access token for Matomo. If this is set `cip` is also tracked. Required for tracking some data.\n- _(Optional)_ `assume_https`: If `True`, set tracked url scheme to `https`, useful when running behind a proxy. Defaults to `True`.\n- _(Optional)_ `exclude_paths`: A list of paths to exclude, only excludes path that is equal to a path in this list. These are tried before `exclude_patterns`. Defaults to `None`.\n- _(Optional)_ `exclude_patterns`: A list of regex patterns that are compiled, and then exclude a path from tracking if any pattern match. Defaults to `None`.\nThese are tried after `exclude_paths`.\n- _(Optional)_ `route_details`: A dict with custom route-specific tracking data. Defaults to `None`.\n\n\n**Notes**:\n\n- Currently only some parts [Matomo Tracking HTTP API](https://developer.matomo.org/api-reference/tracking-api) is supported.\n\n## Ideas for further work:\n- [x] _filtering tracked of urls_\n- [x] _custom extraction of tracked data_\n\n\nThis project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).\n\n# Releas Notes\n\n## Latest Changes\n\n## [0.4.1] - 2023-05-29\n\n### Added\n- track urlref. PR [#21](https://github.com/spraakbanken/asgi-matomo/pull/21) by [@kod-kristoff](https://github.com/kod-kristoff).\n\n### Changed\n- respect x-forwarded-for. PR [#18](https://github.com/spraakbanken/asgi-matomo/pull/18) by [@kod-kristoff](https://github.com/kod-kristoff).\n\n## [0.4.0] - 2023-05-25\n\n* Handle lifespan correctly. PR [#13](https://github.com/spraakbanken/asgi-matomo/pull/13) by [@kod-kristoff](https://github.com/kod-kristoff).\n* add docs. PR [#11](https://github.com/spraakbanken/asgi-matomo/pull/11) by [@kod-kristoff](https://github.com/kod-kristoff).\n## [0.3.2] - 2023-05-23\n\n* feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).\n\n## [0.3.0] - 2023-05-22\n### Added\n\n- Allow setting route-details\n\n',
     'author': 'Kristoffer Andersson',
     'author_email': 'kristoffer.andersson@gu.se',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://spraakbanken.gu.se',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `asgi_matomo-0.4.0/PKG-INFO` & `asgi_matomo-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asgi-matomo
-Version: 0.4.0
+Version: 0.4.1
 Summary: Middleware for tracking ASGI reqeusts with Matomo
 Home-page: https://spraakbanken.gu.se
 License: MIT
 Author: Kristoffer Andersson
 Author-email: kristoffer.andersson@gu.se
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -180,14 +180,22 @@
 
 This project keeps a [changelog](https://github.com/spraakbanken/asgi-matomo/CHANGELOG.md).
 
 # Releas Notes
 
 ## Latest Changes
 
+## [0.4.1] - 2023-05-29
+
+### Added
+- track urlref. PR [#21](https://github.com/spraakbanken/asgi-matomo/pull/21) by [@kod-kristoff](https://github.com/kod-kristoff).
+
+### Changed
+- respect x-forwarded-for. PR [#18](https://github.com/spraakbanken/asgi-matomo/pull/18) by [@kod-kristoff](https://github.com/kod-kristoff).
+
 ## [0.4.0] - 2023-05-25
 
 * Handle lifespan correctly. PR [#13](https://github.com/spraakbanken/asgi-matomo/pull/13) by [@kod-kristoff](https://github.com/kod-kristoff).
 * add docs. PR [#11](https://github.com/spraakbanken/asgi-matomo/pull/11) by [@kod-kristoff](https://github.com/kod-kristoff).
 ## [0.3.2] - 2023-05-23
 
 * feat: add PerfMsTracker. PR [#10](https://github.com/spraakbanken/asgi-matomo/pull/10) by [@kod-kristoff](https://github.com/kod-kristoff).
```


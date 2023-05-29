# Comparing `tmp/loggate-1.8.0.tar.gz` & `tmp/loggate-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loggate-1.8.0.tar", max compression
+gzip compressed data, was "loggate-1.9.0.tar", max compression
```

## Comparing `loggate-1.8.0.tar` & `loggate-1.9.0.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1124 2023-01-24 12:27:55.649205 loggate-1.8.0/LICENSE
--rw-r--r--   0        0        0     8537 2023-01-24 12:27:55.649205 loggate-1.8.0/README.md
--rw-r--r--   0        0        0      603 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/__init__.py
--rw-r--r--   0        0        0      313 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/filters.py
--rw-r--r--   0        0        0     3845 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/formatters.py
--rw-r--r--   0        0        0      419 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/http/__init__.py
--rw-r--r--   0        0        0     1615 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/http/aio_api_call.py
--rw-r--r--   0        0        0     1753 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/http/simple_api_call.py
--rw-r--r--   0        0        0    13237 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/logger.py
--rw-r--r--   0        0        0      257 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/loki/__init__.py
--rw-r--r--   0        0        0     6314 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/loki/emitters.py
--rw-r--r--   0        0        0     1548 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/loki/formatters.py
--rw-r--r--   0        0        0     7539 2023-01-24 12:27:55.649205 loggate-1.8.0/loggate/loki/handlers.py
--rw-r--r--   0        0        0      969 2023-01-24 12:28:09.686189 loggate-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     9501 1970-01-01 00:00:00.000000 loggate-1.8.0/setup.py
--rw-r--r--   0        0        0     9547 1970-01-01 00:00:00.000000 loggate-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1124 2023-05-09 06:15:27.066926 loggate-1.9.0/LICENSE
+-rw-r--r--   0        0        0     8537 2023-05-09 06:15:27.066926 loggate-1.9.0/README.md
+-rw-r--r--   0        0        0      603 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/__init__.py
+-rw-r--r--   0        0        0      313 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/filters.py
+-rw-r--r--   0        0        0     3845 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/formatters.py
+-rw-r--r--   0        0        0      419 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/http/__init__.py
+-rw-r--r--   0        0        0     1764 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/http/aio_api_call.py
+-rw-r--r--   0        0        0     1753 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/http/simple_api_call.py
+-rw-r--r--   0        0        0    13483 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/logger.py
+-rw-r--r--   0        0        0      257 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/loki/__init__.py
+-rw-r--r--   0        0        0     6540 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/loki/emitters.py
+-rw-r--r--   0        0        0     1548 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/loki/formatters.py
+-rw-r--r--   0        0        0     7539 2023-05-09 06:15:27.070926 loggate-1.9.0/loggate/loki/handlers.py
+-rw-r--r--   0        0        0      880 2023-05-09 06:15:41.394899 loggate-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0     9497 1970-01-01 00:00:00.000000 loggate-1.9.0/PKG-INFO
```

### Comparing `loggate-1.8.0/LICENSE` & `loggate-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loggate-1.8.0/README.md` & `loggate-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `loggate-1.8.0/loggate/__init__.py` & `loggate-1.9.0/loggate/__init__.py`

 * *Files identical despite different names*

### Comparing `loggate-1.8.0/loggate/formatters.py` & `loggate-1.9.0/loggate/formatters.py`

 * *Files identical despite different names*

### Comparing `loggate-1.8.0/loggate/http/aio_api_call.py` & `loggate-1.9.0/loggate/http/aio_api_call.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import base64
 import ssl
 
 import aiohttp
+import aiohttp.client_exceptions
 
 from typing import Optional, Tuple
 
 from loggate.http import HttpApiCallInterface
 
 
 class AIOApiCall(HttpApiCallInterface):
     """
     This is the simplest way how we can do API call without any other
     dependencies.
     """
 
     def __init__(self, auth: Optional[Tuple[str, str]] = None,
                  timeout: int = None, ssl_verify=True):
-        self.__timeout = timeout = aiohttp.ClientTimeout(
+        self.__timeout = aiohttp.ClientTimeout(
             total=int(timeout) if timeout else 5
         )
 
         self.headers = {
             'Content-Type': 'application/json; charset=utf-8'
         }
         if auth:
@@ -42,9 +43,12 @@
                 headers=self.headers) as session:
             if method == 'POST':
                 fce = session.post
             elif method == 'GET':
                 fce = session.get
             else:
                 return 0, "The method is not supported"
-            async with fce(url, json=data, ssl=self.ctx) as resp:
-                return resp.status, await resp.text()
+            try:
+                async with fce(url, json=data, ssl=self.ctx) as resp:
+                    return resp.status, await resp.text()
+            except aiohttp.client_exceptions.ClientError as ex:
+                return 1000, str(ex)
```

### Comparing `loggate-1.8.0/loggate/http/simple_api_call.py` & `loggate-1.9.0/loggate/http/simple_api_call.py`

 * *Files identical despite different names*

### Comparing `loggate-1.8.0/loggate/logger.py` & `loggate-1.9.0/loggate/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,37 +210,46 @@
     def set_profiles(self, profiles: dict) -> None:
         """
         Setup profiles structure.
         :param profiles: dict
         """
         self.__profiles = profiles
 
+    def update_profiles(self, profile_patches: dict):
+        self.__profiles.update(profile_patches)
+
+    def get_profiles(self) -> dict:
+        return copy.deepcopy(self.__profiles)
+
     def __cleanup(self, disable_existing_loggers=False):
         logging._acquireLock()
         try:
             self.meta = {}
             self.__filters = {}
             self.__formatters = {}
             for handler in self.__handlers.values():
                 handler.flush()
                 handler.close()
             self.__handlers = {}
             if disable_existing_loggers:
                 self.loggerDict = {}
             else:
+                root = Logger.get_root()
+                root.setLevel(logging.NOTSET)
+                root.propagate = True
+                root.disabled = False
+                root.handlers = []
                 for logger in self.loggerDict.values():
                     if not isinstance(logger, logging.PlaceHolder):
                         logger.setLevel(logging.NOTSET)
                         logger.propagate = True
                         logger.disabled = False
                         logger.handlers = []
         finally:
             logging._releaseLock()
-        # self.loggerDict.clear()
-        # self.root = Logger.get_root(recreate=True)
 
     def __create_handler_from_schema(self, attrs: dict):
         _class = attrs.pop('class', 'logging.Handler')
         _class = dynamic_import(_class)
         attr_level = attrs.pop('level', None)
         attr_formatter = attrs.pop('formatter', None)
         attr_filters = attrs.pop('filters', [])
@@ -288,26 +297,25 @@
             else:
                 logger.addHandler(self.__handlers[handler])
 
     def activate_profile(self, profile_name: str) -> None:
         """
         Switch login profile
         :param profile_name: str - profile name
-        :param cleanup: bool - remove previous configuration
         """
         profile = self.__profiles.get(profile_name)
         if not profile:
             raise LoggingProfileDoesNotExist(
                 f'Profile "{profile_name}" does not exist.')
         profile = copy.deepcopy(profile)
         parent_profile_name = profile.get('inherited')
         if parent_profile_name:
-            self.activate_profile(parent_profile_name, False)
-
-        self.__cleanup(profile.get('disable_existing_loggers', False))
+            self.activate_profile(parent_profile_name)
+        else:
+            self.__cleanup(profile.get('disable_existing_loggers', False))
         # Filters
         for name, attrs in profile.get('filters', {}).items():
             _class = attrs.pop('class', 'logging.Filter')
             _class = dynamic_import(_class)
             self.__filters[name] = _class(**attrs)
 
         # Formatters
```

### Comparing `loggate-1.8.0/loggate/loki/emitters.py` & `loggate-1.9.0/loggate/loki/emitters.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,27 +46,31 @@
         if isinstance(urls, str):
             urls = [urls]
         if not strategy:
             strategy = LOKI_DEPLOY_STRATEGY_RANDOM
         strategy = strategy.lower()
         if strategy not in LOKI_DEPLOY_STRATEGIES:
             raise
-
         self.urls = urls
-        self.strategy = strategy
-        self._url_indexes = list(range(len(urls)))
         if strategy == LOKI_DEPLOY_STRATEGY_RANDOM:
-            random.shuffle(self._url_indexes)
-
+            random.shuffle(self.urls)
+        self.strategy = strategy
         self.handler = handler
         self.queue: SimpleQueue = queue
         self.api = api
         self.thread = None
         self.thread_stop = Event()
 
+    @property
+    def entrypoint(self):
+        return self.urls[0]
+
+    def rotate_entrypoints(self):
+        self.urls.append(self.urls.pop(0))
+
     def prepare_payload(self, records: [LogRecord]):
         data = []
         for record in records:
             data.append({
                 'stream': self.handler.build_tags(record),
                 'values': [(str(int(record.created * 1e9)),
                             self.handler.format(record))]
@@ -75,22 +79,24 @@
 
     def emit(self, records):
         """
         Send log records to Loki.
         :param records: List[LogRecord]
         """
         payload = self.prepare_payload(records)
-        for ix in self._url_indexes:
-            status_code, msg = self.api.send_json(self.urls[ix], payload)
+        status_code = ''
+        for _ in range(len(self.urls)):
+            status_code, msg = self.api.send_json(self.entrypoint, payload)
             if status_code == self.success_response_code:
                 if self.strategy != LOKI_DEPLOY_STRATEGY_ALL:
                     return
             elif status_code == self.timeout_response_code:
                 sys.stderr.write(f'loggate: The delivery logs to '
-                                 f'"{self.urls[ix]}" failed.\n')
+                                 f'"{self.entrypoint}" failed.\n')
+            self.rotate_entrypoints()
 
         if status_code in [self.success_response_code,
                            self.timeout_response_code]:
             return
         # TODO: make recovery strategy
         raise LokiServerError(
             f"Unexpected Loki API response status code: "
@@ -98,24 +104,26 @@
 
     async def emit_async(self, records):
         """
         Asyncio send log record to Loki.
         :param records: List[LogRecord]
         """
         payload = self.prepare_payload(records)
-        for ix in self._url_indexes:
+        status_code = ''
+        for _ in range(len(self.urls)):
             status_code, msg = await self.api.send_json(
-                self.urls[ix], payload
+                self.entrypoint, payload
             )
             if status_code == self.success_response_code:
                 if self.strategy != LOKI_DEPLOY_STRATEGY_ALL:
                     return
             elif status_code == self.timeout_response_code:
                 sys.stderr.write(f'loggate: The delivery logs to '
-                                 f'"{self.urls[ix]}" failed.\n')
+                                 f'"{self.entrypoint}" failed.\n')
+            self.rotate_entrypoints()
 
         if status_code in [self.success_response_code,
                            self.timeout_response_code]:
             return
         # TODO: make recovery strategy
         raise LokiServerError(
             f"Unexpected Loki API response status code: "
```

### Comparing `loggate-1.8.0/loggate/loki/formatters.py` & `loggate-1.9.0/loggate/loki/formatters.py`

 * *Files identical despite different names*

### Comparing `loggate-1.8.0/loggate/loki/handlers.py` & `loggate-1.9.0/loggate/loki/handlers.py`

 * *Files identical despite different names*

### Comparing `loggate-1.8.0/pyproject.toml` & `loggate-1.9.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "loggate"
-version = "1.8.0"
+version = "1.9.0"
 license = "MIT"
 readme = "README.md"
 description = "The complex logging system."
 authors = ["Martin Korbel <mkorbel@alps.cz>"]
 homepage = "https://github.com/calcite/loggate"
 repository = "https://github.com/calcite/loggate"
 documentation = "https://github.com/calcite/loggate"
@@ -12,22 +12,21 @@
 keywords = ["log", "logging", "logger", "loki"]
 classifiers = [
     "Topic :: System :: Networking",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6"
+python = "^3.7"
 aiohttp = { version = "*", optional = true}
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2.5"
+pytest = "^7.3.1"
 PyYAML = "^5.4.1 || ^6.0"
-pytest-asyncio = [{version = "^0.19.0", python = "^3.7"},
-                  {version = "^0.16.0", python = "^3.6"}]
+pytest-asyncio = "^0.21.0"
 
 [tool.poetry.extras]
 asyncio = ["aiohttp"]
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests"
```

### Comparing `loggate-1.8.0/setup.py` & `loggate-1.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,257 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: loggate
+Version: 1.9.0
+Summary: The complex logging system.
+Home-page: https://github.com/calcite/loggate
+License: MIT
+Keywords: log,logging,logger,loki
+Author: Martin Korbel
+Author-email: mkorbel@alps.cz
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Topic :: System :: Networking
+Provides-Extra: asyncio
+Requires-Dist: aiohttp ; extra == "asyncio"
+Project-URL: Documentation, https://github.com/calcite/loggate
+Project-URL: Repository, https://github.com/calcite/loggate
+Description-Content-Type: text/markdown
 
-packages = \
-['loggate', 'loggate.http', 'loggate.loki']
+# Loggate
+[![PyPI](https://img.shields.io/pypi/v/loggate?color=green&style=plastic)](https://pypi.org/project/loggate/)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loggate?style=plastic)
+![License](https://img.shields.io/github/license/calcite/loggate?style=plastic)
 
-package_data = \
-{'': ['*']}
+The complex logging system with support of log metadata and delivery to [Grafana Loki](https://grafana.com/oss/loki/). 
+This library supports threading & asyncio modules.  
 
-extras_require = \
-{'asyncio': ['aiohttp']}
-
-setup_kwargs = {
-    'name': 'loggate',
-    'version': '1.8.0',
-    'description': 'The complex logging system.',
-    'long_description': '# Loggate\n[![PyPI](https://img.shields.io/pypi/v/loggate?color=green&style=plastic)](https://pypi.org/project/loggate/)\n![PyPI - Python Version](https://img.shields.io/pypi/pyversions/loggate?style=plastic)\n![License](https://img.shields.io/github/license/calcite/loggate?style=plastic)\n\nThe complex logging system with support of log metadata and delivery to [Grafana Loki](https://grafana.com/oss/loki/). \nThis library supports threading & asyncio modules.  \n\n## Simple stdout/stderr colorized output\nOne example is more than a thousand words.\n\n```python\nfrom loggate import setup_logging, get_logger\n\nsetup_logging(level=\'DEBUG\')\nlogger = get_logger(\'component\', meta={\'version\': \'1.0.0\'})\n\nlogger.debug(\'Loading resources for the component\')\nlogger.info(\'Initialize of the component\')\nlogger.warning(\'The component is not ready\')\nlogger.error(\'The component failed.\',\n             meta={\'inputs\': {\'A\': 1, \'B\': 2}})\nlogger.critical(\'The component unexpected failed.\',\n                meta={\'attrs\': {\'A\': 1, \'B\': 2}})\n```\n*Console output:*\n\n![Console output](https://github.com/calcite/loggate/raw/master/img/console.png)\n\n\n### Exceptions\n\n```python\nfrom loggate import setup_logging, get_logger\n\nsetup_logging()\nlogger = get_logger(\'component\', meta={\'version\': \'1.0.0\'})\n\ntry:\n    raise Exception(\'Some error\')\nexcept Exception as ex:\n    logger.error(\'The component failed.\', exc_info=True)\n```\n*Console output:*\n\n![Console output](https://github.com/calcite/loggate/raw/master/img/exception.png)\n\n\n## Advanced configuration\nThe Loggate supports a declarative configuration alike as [logging.config](https://docs.python.org/3/library/logging.config.html).\nBut this support profiles as well. It\'s mean we can declare many logging profiles and switch between them. Default profile is called `default`.\n\nWe can use yaml file as configuration file (see next):\n```yaml\nprofiles:\n  default:                             \n    # Default profile\n    filters:\n      warning:                          \n        # This is a filter for stdout logger, that enable only logs with level lower than WARNING. \n        # For logs with WARNING and higher we use stderr logger. \n        class: loggate.LowerLogLevelFilter\n        level: WARNING\n\n    formatters:\n      colored:\n        # This is stdout/sterr formatter. \n        class: loggate.LogColorFormatter\n      loki:\n        # This is formatter of loki messages.\n        class: loggate.loki.LokiLogFormatter\n\n    handlers:\n      stdout:\n        # This is a stdout handler\n        class: logging.StreamHandler\n        stream: ext://sys.stdout\n        formatter: colored\n        filters:\n          - warning\n      stderr:\n        # This is a stderr handler\n        class: logging.StreamHandler\n        stream: ext://sys.stderr\n        formatter: colored\n        level: WARNING        \n      loki:\n        # This is a loki handler\n        class: loggate.loki.LokiThreadHandler  # for asyncio use loggate.loki.LokiHandler       \n        formatter: loki\n        urls:\n          - "http://loki1:3100/loki/api/v1/push"\n          - "http://loki2:3100/loki/api/v1/push"\n          - "http://loki3:3100/loki/api/v1/push"\n        meta:\n          # loggate handlers accept metadata as well. Standard logging handlers do not!\n          stage: dev\n          ip: 192.168.1.10                \n                  \n\n    loggers:\n        root:          \n          level: INFO\n          handlers:\n            - stdout\n            - stderr        \n            - loki\n        \'urllib3.connectionpool\': \n          level: WARNING\n\n```\n\n```python\nimport yaml\nfrom loggate import setup_logging, get_logger\n\n\ndef get_yaml(filename):\n    with open(filename, \'r+\') as fd:\n        return yaml.safe_load(fd)\n\n\nschema = get_yaml(\'test.yaml\')\nsetup_logging(profiles=schema.get(\'profiles\'))\n\nlogger = get_logger(\'component\')\n\nlogger.debug(\'Loading resources for the component\')\nlogger.info(\'Initialize of the component\')\nlogger.warning(\'The component is not ready\')\n```\nThe console output is the same as above, but now we send logs to Loki as well.\n\n*Loki output:*\n\n![loki output](https://github.com/calcite/loggate/raw/master/img/loki1.png)\n\n\n\n# Description\n## Methods\n- `get_logger`\n  - `name` - Return logger for this name. Empty name returns root logger.\n  - `meta` - Metadata (dict), which are sent only by this logger.\n\n- `getLogger` - only alias for `get_logger`\n- `setup_logging` - init setup of application logging.\n  - `profiles` - Profiles (dict) of logging profiles. When we do not set this parameter, application use predefined profile with log `INFO` level (this level can be set by parameter `level`). \n  - `default_profile` - name of the default profile (default: `default`)\n  - `level` - This is special parameter for situation when  application use predefined profile (default `INFO`).  \n\n## Filters\n### Class `loggate.LowerLogLevelFilter`\nThis filters out all logs which are higher than `level`.\n- `level` - log level\n\n## Formatters\n### Class `loggate.LogColorFormatter`\nColorized formatter for stdout/stderr.\n- `fmt` - message format (default: `%(LEVEL_COLOR)s%(asctime)s\\t [%(levelname)s] %(name)s:%(COLOR_RESET)s %(message)s`)\n- `datefmt` - datetime format (default: `%Y-%m-%d %H:%M:%S`)\n- `style` - style of templating (default: `%`). \n- `validate` - validate the input format (default: True)\n- `INDENTATION_TRACEBACK` - default: `\\t\\t\\t`\n- `INDENTATION_METADATA` - default: `\\t\\t\\t\\t`\n- `COLOR_DEBUG`, ..., `COLOR_CRITICAL` - set color of this levels (e.g. `\\x1b[1;31m`, see [more colors](https://dev.to/ifenna__/adding-colors-to-bash-scripts-48g4)).\n- `COLOR_METADATA` - set color metadata\n- `COLOR_TRACEBACK` - set color of tracebacks\n- `COLOR_...` - set custom color\n\n### Class `loggate.loki.LokiLogFormatter`\nThis is special loki formatter, this converts log records to jsons.\n\n\n## Handlers\n### Class `loggate.loki.LokiHandler`\nThis handler send log records to Loki server. This is blocking implementation of handler.\nIt means, when we call log method (`debug`, ... `critical`) the message is sent in the same thread. We should use\nthis only for tiny scripts where other ways have a big overhead.\n- `level` - This handler sends only log records with log level equal or higher than this (default: all = `logging.NOTSET`).\n- `urls` - List of loki entrypoints.\n- `strategy` - Deploy strategy (default: `random`).\n  - `random` - At the beginning the handler choose random Loki server and others are fallbacks.\n  - `fallbacks` - The handler uses the first Loki server and others are fallbacks.\n  - `all` - The handler send the log record to all loki servers.\n- `auth` - The Loki authentication, the list with two items (`username`, `password`).\n- `timeout` - Timeout for one delivery try (default: 5s).\n- `ssl_verify` - Enable ssl verify (default: True).\n- `loki_tags` - the list of metadata keys, which are sent to Loki server as label (defailt: [`logger`, `level`]).\n- `meta` - Metadata (dict), which are sent only by this handler.  \n\n### Class `loggate.loki.LokiAsyncioHandler`\nThis is non-bloking extending of LokiHandler. We register an extra asyncio task for sending messages to the Loki server.\nParameters are the same as `loggate.loki.LokiHandler`. This handler uses `urllib.requests` module in default ([aiohttp](https://pypi.org/project/aiohttp/) as optional). \nUnfortunately `urllib.requests` module does not support asyncio, it means the sending itself is blocking.\nThe `loggate.loki.Loki AsyncioHandler` can use the optional dependency [aiohttp](https://pypi.org/project/aiohttp/) for non-bloking sending.\n\n### Class `loggate.loki.LokiThreadHandler`\nThis is non-bloking extending of LokiHandler. We register and start an extra thread for sending messages to the Loki server.\nParameters are the same as `loggate.loki.LokiHandler`.\n\n## Profiles\nThe structure of profiles (parameter `profiles` of `setup_logging`).\n\n```yaml\n<profile_name>:\n  \n  filters:\n    <filter_name>:\n      class: <filter_class>\n      <filter_attribute_name>: <filter_attribute_value>\n  \n  formatters:\n    <formatter_name>:\n      class: <formatter_class>\n      <formatter_attribute_name>: <formatter_attribute_value>\n  \n  handlers:\n    <handler_name>:\n      class: <handler_class>\n      <handler_attribute_name>: <handler_attribute_value>\n\n  loggers:\n    <logger_name>|root:   # definition of root logger\n      level: <log_level>\n      handlers: \n        - <name_of_handler>|<definition_of_handler>\n      disabled: True|False    # default: False\n      propagate: True|False   # default: True\n      meta: <logger_metadata>  \n```\n',
-    'author': 'Martin Korbel',
-    'author_email': 'mkorbel@alps.cz',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/calcite/loggate',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
-}
+## Simple stdout/stderr colorized output
+One example is more than a thousand words.
 
+```python
+from loggate import setup_logging, get_logger
+
+setup_logging(level='DEBUG')
+logger = get_logger('component', meta={'version': '1.0.0'})
+
+logger.debug('Loading resources for the component')
+logger.info('Initialize of the component')
+logger.warning('The component is not ready')
+logger.error('The component failed.',
+             meta={'inputs': {'A': 1, 'B': 2}})
+logger.critical('The component unexpected failed.',
+                meta={'attrs': {'A': 1, 'B': 2}})
+```
+*Console output:*
+
+![Console output](https://github.com/calcite/loggate/raw/master/img/console.png)
+
+
+### Exceptions
+
+```python
+from loggate import setup_logging, get_logger
+
+setup_logging()
+logger = get_logger('component', meta={'version': '1.0.0'})
+
+try:
+    raise Exception('Some error')
+except Exception as ex:
+    logger.error('The component failed.', exc_info=True)
+```
+*Console output:*
+
+![Console output](https://github.com/calcite/loggate/raw/master/img/exception.png)
+
+
+## Advanced configuration
+The Loggate supports a declarative configuration alike as [logging.config](https://docs.python.org/3/library/logging.config.html).
+But this support profiles as well. It's mean we can declare many logging profiles and switch between them. Default profile is called `default`.
+
+We can use yaml file as configuration file (see next):
+```yaml
+profiles:
+  default:                             
+    # Default profile
+    filters:
+      warning:                          
+        # This is a filter for stdout logger, that enable only logs with level lower than WARNING. 
+        # For logs with WARNING and higher we use stderr logger. 
+        class: loggate.LowerLogLevelFilter
+        level: WARNING
+
+    formatters:
+      colored:
+        # This is stdout/sterr formatter. 
+        class: loggate.LogColorFormatter
+      loki:
+        # This is formatter of loki messages.
+        class: loggate.loki.LokiLogFormatter
+
+    handlers:
+      stdout:
+        # This is a stdout handler
+        class: logging.StreamHandler
+        stream: ext://sys.stdout
+        formatter: colored
+        filters:
+          - warning
+      stderr:
+        # This is a stderr handler
+        class: logging.StreamHandler
+        stream: ext://sys.stderr
+        formatter: colored
+        level: WARNING        
+      loki:
+        # This is a loki handler
+        class: loggate.loki.LokiThreadHandler  # for asyncio use loggate.loki.LokiHandler       
+        formatter: loki
+        urls:
+          - "http://loki1:3100/loki/api/v1/push"
+          - "http://loki2:3100/loki/api/v1/push"
+          - "http://loki3:3100/loki/api/v1/push"
+        meta:
+          # loggate handlers accept metadata as well. Standard logging handlers do not!
+          stage: dev
+          ip: 192.168.1.10                
+                  
+
+    loggers:
+        root:          
+          level: INFO
+          handlers:
+            - stdout
+            - stderr        
+            - loki
+        'urllib3.connectionpool': 
+          level: WARNING
+
+```
+
+```python
+import yaml
+from loggate import setup_logging, get_logger
+
+
+def get_yaml(filename):
+    with open(filename, 'r+') as fd:
+        return yaml.safe_load(fd)
+
+
+schema = get_yaml('test.yaml')
+setup_logging(profiles=schema.get('profiles'))
+
+logger = get_logger('component')
+
+logger.debug('Loading resources for the component')
+logger.info('Initialize of the component')
+logger.warning('The component is not ready')
+```
+The console output is the same as above, but now we send logs to Loki as well.
+
+*Loki output:*
+
+![loki output](https://github.com/calcite/loggate/raw/master/img/loki1.png)
+
+
+
+# Description
+## Methods
+- `get_logger`
+  - `name` - Return logger for this name. Empty name returns root logger.
+  - `meta` - Metadata (dict), which are sent only by this logger.
+
+- `getLogger` - only alias for `get_logger`
+- `setup_logging` - init setup of application logging.
+  - `profiles` - Profiles (dict) of logging profiles. When we do not set this parameter, application use predefined profile with log `INFO` level (this level can be set by parameter `level`). 
+  - `default_profile` - name of the default profile (default: `default`)
+  - `level` - This is special parameter for situation when  application use predefined profile (default `INFO`).  
+
+## Filters
+### Class `loggate.LowerLogLevelFilter`
+This filters out all logs which are higher than `level`.
+- `level` - log level
+
+## Formatters
+### Class `loggate.LogColorFormatter`
+Colorized formatter for stdout/stderr.
+- `fmt` - message format (default: `%(LEVEL_COLOR)s%(asctime)s\t [%(levelname)s] %(name)s:%(COLOR_RESET)s %(message)s`)
+- `datefmt` - datetime format (default: `%Y-%m-%d %H:%M:%S`)
+- `style` - style of templating (default: `%`). 
+- `validate` - validate the input format (default: True)
+- `INDENTATION_TRACEBACK` - default: `\t\t\t`
+- `INDENTATION_METADATA` - default: `\t\t\t\t`
+- `COLOR_DEBUG`, ..., `COLOR_CRITICAL` - set color of this levels (e.g. `\x1b[1;31m`, see [more colors](https://dev.to/ifenna__/adding-colors-to-bash-scripts-48g4)).
+- `COLOR_METADATA` - set color metadata
+- `COLOR_TRACEBACK` - set color of tracebacks
+- `COLOR_...` - set custom color
+
+### Class `loggate.loki.LokiLogFormatter`
+This is special loki formatter, this converts log records to jsons.
+
+
+## Handlers
+### Class `loggate.loki.LokiHandler`
+This handler send log records to Loki server. This is blocking implementation of handler.
+It means, when we call log method (`debug`, ... `critical`) the message is sent in the same thread. We should use
+this only for tiny scripts where other ways have a big overhead.
+- `level` - This handler sends only log records with log level equal or higher than this (default: all = `logging.NOTSET`).
+- `urls` - List of loki entrypoints.
+- `strategy` - Deploy strategy (default: `random`).
+  - `random` - At the beginning the handler choose random Loki server and others are fallbacks.
+  - `fallbacks` - The handler uses the first Loki server and others are fallbacks.
+  - `all` - The handler send the log record to all loki servers.
+- `auth` - The Loki authentication, the list with two items (`username`, `password`).
+- `timeout` - Timeout for one delivery try (default: 5s).
+- `ssl_verify` - Enable ssl verify (default: True).
+- `loki_tags` - the list of metadata keys, which are sent to Loki server as label (defailt: [`logger`, `level`]).
+- `meta` - Metadata (dict), which are sent only by this handler.  
+
+### Class `loggate.loki.LokiAsyncioHandler`
+This is non-bloking extending of LokiHandler. We register an extra asyncio task for sending messages to the Loki server.
+Parameters are the same as `loggate.loki.LokiHandler`. This handler uses `urllib.requests` module in default ([aiohttp](https://pypi.org/project/aiohttp/) as optional). 
+Unfortunately `urllib.requests` module does not support asyncio, it means the sending itself is blocking.
+The `loggate.loki.Loki AsyncioHandler` can use the optional dependency [aiohttp](https://pypi.org/project/aiohttp/) for non-bloking sending.
+
+### Class `loggate.loki.LokiThreadHandler`
+This is non-bloking extending of LokiHandler. We register and start an extra thread for sending messages to the Loki server.
+Parameters are the same as `loggate.loki.LokiHandler`.
+
+## Profiles
+The structure of profiles (parameter `profiles` of `setup_logging`).
+
+```yaml
+<profile_name>:
+  
+  filters:
+    <filter_name>:
+      class: <filter_class>
+      <filter_attribute_name>: <filter_attribute_value>
+  
+  formatters:
+    <formatter_name>:
+      class: <formatter_class>
+      <formatter_attribute_name>: <formatter_attribute_value>
+  
+  handlers:
+    <handler_name>:
+      class: <handler_class>
+      <handler_attribute_name>: <handler_attribute_value>
+
+  loggers:
+    <logger_name>|root:   # definition of root logger
+      level: <log_level>
+      handlers: 
+        - <name_of_handler>|<definition_of_handler>
+      disabled: True|False    # default: False
+      propagate: True|False   # default: True
+      meta: <logger_metadata>  
+```
 
-setup(**setup_kwargs)
```


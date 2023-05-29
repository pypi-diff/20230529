# Comparing `tmp/aiopvpc-4.2.0.tar.gz` & `tmp/aiopvpc-4.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopvpc-4.2.0.tar", max compression
+gzip compressed data, was "aiopvpc-4.2.1.tar", max compression
```

## Comparing `aiopvpc-4.2.0.tar` & `aiopvpc-4.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2023-05-29 08:06:38.025438 aiopvpc-4.2.0/LICENSE
--rw-r--r--   0        0        0     1714 2023-05-29 08:06:38.025438 aiopvpc-4.2.0/README.md
--rw-r--r--   0        0        0      382 2023-05-29 08:06:38.025438 aiopvpc-4.2.0/aiopvpc/__init__.py
--rw-r--r--   0        0        0     2612 2023-05-29 08:06:38.025438 aiopvpc-4.2.0/aiopvpc/const.py
--rw-r--r--   0        0        0     1360 2023-05-29 08:06:38.025438 aiopvpc-4.2.0/aiopvpc/ha_helpers.py
--rw-r--r--   0        0        0     4960 2023-05-29 08:06:38.025438 aiopvpc-4.2.0/aiopvpc/parser.py
--rw-r--r--   0        0        0     4370 2023-05-29 08:06:38.029438 aiopvpc-4.2.0/aiopvpc/prices.py
--rw-r--r--   0        0        0    15031 2023-05-29 08:06:38.029438 aiopvpc-4.2.0/aiopvpc/pvpc_data.py
--rw-r--r--   0        0        0     4803 2023-05-29 08:06:38.029438 aiopvpc-4.2.0/aiopvpc/pvpc_tariff.py
--rw-r--r--   0        0        0      401 2023-05-29 08:06:38.029438 aiopvpc-4.2.0/aiopvpc/utils.py
--rw-r--r--   0        0        0     1627 2023-05-29 08:06:38.029438 aiopvpc-4.2.0/pyproject.toml
--rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 aiopvpc-4.2.0/setup.py
--rw-r--r--   0        0        0     2411 1970-01-01 00:00:00.000000 aiopvpc-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/LICENSE
+-rw-r--r--   0        0        0     1714 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/README.md
+-rw-r--r--   0        0        0      382 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/__init__.py
+-rw-r--r--   0        0        0     2612 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/const.py
+-rw-r--r--   0        0        0     1360 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/ha_helpers.py
+-rw-r--r--   0        0        0     4960 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/parser.py
+-rw-r--r--   0        0        0     4380 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/prices.py
+-rw-r--r--   0        0        0    15031 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/pvpc_data.py
+-rw-r--r--   0        0        0     4803 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/pvpc_tariff.py
+-rw-r--r--   0        0        0      401 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/aiopvpc/utils.py
+-rw-r--r--   0        0        0     1627 2023-05-29 10:24:28.495344 aiopvpc-4.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2461 1970-01-01 00:00:00.000000 aiopvpc-4.2.1/setup.py
+-rw-r--r--   0        0        0     2411 1970-01-01 00:00:00.000000 aiopvpc-4.2.1/PKG-INFO
```

### Comparing `aiopvpc-4.2.0/LICENSE` & `aiopvpc-4.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.0/README.md` & `aiopvpc-4.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.0/aiopvpc/const.py` & `aiopvpc-4.2.1/aiopvpc/const.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.0/aiopvpc/ha_helpers.py` & `aiopvpc-4.2.1/aiopvpc/ha_helpers.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.0/aiopvpc/parser.py` & `aiopvpc-4.2.1/aiopvpc/parser.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.0/aiopvpc/prices.py` & `aiopvpc-4.2.1/aiopvpc/prices.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,19 +76,19 @@
     try:
         attributes["price_ratio"] = round(
             (current_price - min_price) / (max_price - min_price), 2
         )
     except ZeroDivisionError:  # pragma: no cover
         pass
     attributes["max_price"] = max_price
-    best_price_at = next(iter(prices_sorted)).astimezone(timezone).hour
-    worst_price_at = next(iter(reversed(prices_sorted))).astimezone(timezone).hour
-    attributes["max_price_at"] = worst_price_at if sign_is_best else best_price_at
+    first_price_at = next(iter(prices_sorted)).astimezone(timezone).hour
+    last_price_at = next(iter(reversed(prices_sorted))).astimezone(timezone).hour
+    attributes["max_price_at"] = last_price_at if sign_is_best == 1 else first_price_at
     attributes["min_price"] = min_price
-    attributes["min_price_at"] = best_price_at if sign_is_best else worst_price_at
+    attributes["min_price_at"] = first_price_at if sign_is_best == 1 else last_price_at
     attributes["next_best_at"] = [
         ts.astimezone(timezone).hour for ts in prices_sorted.keys() if ts >= utc_time
     ]
     return attributes
 
 
 def make_price_sensor_attributes(
```

### Comparing `aiopvpc-4.2.0/aiopvpc/pvpc_data.py` & `aiopvpc-4.2.1/aiopvpc/pvpc_data.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.0/aiopvpc/pvpc_tariff.py` & `aiopvpc-4.2.1/aiopvpc/pvpc_tariff.py`

 * *Files identical despite different names*

### Comparing `aiopvpc-4.2.0/pyproject.toml` & `aiopvpc-4.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 log_cli_date_format = "%H:%M:%S"
 markers = [
     "real_api_call: Tests making requests to api.esios.ree.es (deselected by default)",
 ]
 
 [tool.poetry]
 name = "aiopvpc"
-version = "4.2.0"
+version = "4.2.1"
 description = "Retrieval of Spanish Electricity hourly prices (PVPC)"
 authors = ["Eugenio Panadero <eugenio.panadero@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/azogue/aiopvpc"
 
 [tool.poetry.dependencies]
```

### Comparing `aiopvpc-4.2.0/setup.py` & `aiopvpc-4.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['aiohttp>=3.7.4.post0', 'async_timeout>=3.0.1']
 
 setup_kwargs = {
     'name': 'aiopvpc',
-    'version': '4.2.0',
+    'version': '4.2.1',
     'description': 'Retrieval of Spanish Electricity hourly prices (PVPC)',
     'long_description': '[![PyPI Version][pypi-image]][pypi-url]\n[![pre-commit.ci Status][pre-commit-ci-image]][pre-commit-ci-url]\n[![Build Status][build-image]][build-url]\n[![Code Coverage][coverage-image]][coverage-url]\n\n<!-- Badges -->\n\n[pypi-image]: https://img.shields.io/pypi/v/aiopvpc\n[pypi-url]: https://pypi.org/project/aiopvpc/\n[pre-commit-ci-image]: https://results.pre-commit.ci/badge/github/azogue/aiopvpc/master.svg\n[pre-commit-ci-url]: https://results.pre-commit.ci/latest/github/azogue/aiopvpc/master\n[build-image]: https://github.com/azogue/aiopvpc/actions/workflows/main.yml/badge.svg\n[build-url]: https://github.com/azogue/aiopvpc/actions/workflows/main.yml\n[coverage-image]: https://codecov.io/gh/azogue/aiopvpc/branch/master/graph/badge.svg\n[coverage-url]: https://codecov.io/gh/azogue/aiopvpc\n\n# aiopvpc\n\nSimple aio library to download Spanish electricity hourly prices.\n\nMade to support the [**`pvpc_hourly_pricing`** HomeAssistant integration](https://www.home-assistant.io/integrations/pvpc_hourly_pricing/).\n\n<span class="badge-buymeacoffee"><a href="https://www.buymeacoffee.com/azogue" title="Donate to this project using Buy Me A Coffee"><img src="https://img.shields.io/badge/buy%20me%20a%20coffee-donate-yellow.svg" alt="Buy Me A Coffee donate button" /></a></span>\n\n## Install\n\nInstall with `pip install aiopvpc` or clone it to run tests or anything else.\n\n## Usage\n\n```python\nimport aiohttp\nfrom datetime import datetime\nfrom aiopvpc import PVPCData\n\nasync with aiohttp.ClientSession() as session:\n    pvpc_handler = PVPCData(session=session, tariff="2.0TD")\n    esios_data = await pvpc_handler.async_update_all(\n        current_data=None, now=datetime.utcnow()\n    )\nprint(esios_data.sensors["PVPC"])\n```\n',
     'author': 'Eugenio Panadero',
     'author_email': 'eugenio.panadero@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/azogue/aiopvpc',
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['aiopvpc']
 package_data = \ {'': ['*']} install_requires = \ ['aiohttp>=3.7.4.post0',
-'async_timeout>=3.0.1'] setup_kwargs = { 'name': 'aiopvpc', 'version': '4.2.0',
+'async_timeout>=3.0.1'] setup_kwargs = { 'name': 'aiopvpc', 'version': '4.2.1',
 'description': 'Retrieval of Spanish Electricity hourly prices (PVPC)',
 'long_description': '[![PyPI Version][pypi-image]][pypi-url]\n[![pre-commit.ci
 Status][pre-commit-ci-image]][pre-commit-ci-url]\n[![Build Status][build-
 image]][build-url]\n[![Code Coverage][coverage-image]][coverage-url]\n\n\n\n
 [pypi-image]: https://img.shields.io/pypi/v/aiopvpc\n[pypi-url]: https://
 pypi.org/project/aiopvpc/\n[pre-commit-ci-image]: https://results.pre-
 commit.ci/badge/github/azogue/aiopvpc/master.svg\n[pre-commit-ci-url]: https://
```

### Comparing `aiopvpc-4.2.0/PKG-INFO` & `aiopvpc-4.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopvpc
-Version: 4.2.0
+Version: 4.2.1
 Summary: Retrieval of Spanish Electricity hourly prices (PVPC)
 Home-page: https://github.com/azogue/aiopvpc
 License: MIT
 Author: Eugenio Panadero
 Author-email: eugenio.panadero@gmail.com
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: aiopvpc Version: 4.2.0 Summary: Retrieval of
+Metadata-Version: 2.1 Name: aiopvpc Version: 4.2.1 Summary: Retrieval of
 Spanish Electricity hourly prices (PVPC) Home-page: https://github.com/azogue/
 aiopvpc License: MIT Author: Eugenio Panadero Author-email:
 eugenio.panadero@gmail.com Requires-Python: >=3.9,<3.12 Classifier: License ::
 OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: aiohttp (>=3.7.4.post0) Requires-Dist: async_timeout (>=3.0.1)
```


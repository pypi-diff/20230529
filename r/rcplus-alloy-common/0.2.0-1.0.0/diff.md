# Comparing `tmp/rcplus_alloy_common-0.2.0.tar.gz` & `tmp/rcplus_alloy_common-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcplus_alloy_common-0.2.0.tar", max compression
+gzip compressed data, was "rcplus_alloy_common-1.0.0.tar", max compression
```

## Comparing `rcplus_alloy_common-0.2.0.tar` & `rcplus_alloy_common-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,17 @@
--rw-r--r--   0        0        0       77 2023-02-24 10:40:56.135339 rcplus_alloy_common-0.2.0/LICENSE
--rw-r--r--   0        0        0      966 2023-02-24 10:40:56.135339 rcplus_alloy_common-0.2.0/README.md
--rw-r--r--   0        0        0     1089 2023-02-24 10:40:56.135339 rcplus_alloy_common-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    13880 2023-02-24 10:40:56.135339 rcplus_alloy_common-0.2.0/src/rcplus_alloy_common/__init__.py
--rw-r--r--   0        0        0     1921 2023-02-24 10:40:56.135339 rcplus_alloy_common-0.2.0/src/rcplus_alloy_common/constants.py
--rw-r--r--   0        0        0     1897 1970-01-01 00:00:00.000000 rcplus_alloy_common-0.2.0/setup.py
--rw-r--r--   0        0        0     2199 1970-01-01 00:00:00.000000 rcplus_alloy_common-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       77 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/LICENSE
+-rw-r--r--   0        0        0      571 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/README.md
+-rw-r--r--   0        0        0     1930 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2881 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/__init__.py
+-rw-r--r--   0        0        0      581 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/__init__.py
+-rw-r--r--   0        0        0     1182 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/dag.py
+-rw-r--r--   0        0        0     1655 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/decorators.py
+-rw-r--r--   0        0        0     7448 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/observability.py
+-rw-r--r--   0        0        0     9867 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/operators.py
+-rw-r--r--   0        0        0     2611 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/sensors.py
+-rw-r--r--   0        0        0     2009 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/airflow/utils.py
+-rw-r--r--   0        0        0     2279 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/constants.py
+-rw-r--r--   0        0        0     3866 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/logging.py
+-rw-r--r--   0        0        0     6388 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/metrics.py
+-rw-r--r--   0        0        0     3925 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/retry.py
+-rw-r--r--   0        0        0       19 2023-05-29 17:18:21.056573 rcplus_alloy_common-1.0.0/src/rcplus_alloy_common/version.py
+-rw-r--r--   0        0        0     1781 1970-01-01 00:00:00.000000 rcplus_alloy_common-1.0.0/PKG-INFO
```

### Comparing `rcplus_alloy_common-0.2.0/pyproject.toml` & `rcplus_alloy_common-1.0.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,77 @@
 [build-system]
-requires = ["setuptools", "wheel", "poetry-core>=1.0.0"]
+requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
+[tool.black]
+line-length = 120
+
 [tool.poetry]
 name = "rcplus_alloy_common"
-version = "0.2.0"
+version = "1.0.0"
 description = "RC+/Alloy helpers functions for Python"
 readme = "README.md"
 authors = [
     "Ringier AG <info@rcplus.io>",
 ]
 license = "Proprietary"
 repository = "https://github.com/ringier-data/rcplus-alloy-lib-py-common"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Natural Language :: English",
     "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Utilities",
     "Intended Audience :: Developers",
 ]
 keywords = ["rcplus", "alloy", "logging", "metrics", "utilities"]
 
 [tool.poetry.dependencies]
-python = ">= 3.8, < 4"
+python = ">= 3.10, < 4"
 requests = ">=2.6.1"
 jsonschema = ">=3.0.0"
 python-json-logger = ">=2.0.4"
-logzio-python-handler = {version = ">=4.0.0", optional = true}
+apache-airflow = {version = "^2.6.1", optional = true, extras=["amazon", "slack"]}
+pytz = {version = "^2023.3", optional = true}
 
 [tool.poetry.extras]
-logzio = ["logzio-python-handler"]
+airflow = ["apache-airflow", "pytz"]
 
 [tool.poetry.group.dev.dependencies]
+prospector = {version="*", extras=["with_mypy"]}
+black = ">=22.10.0"
 pytest = ">=7.2.0"
+pytest-asyncio = ">=0.10.0"
+pylint-quotes = ">=0.2.0"
+moto = "^4.1.10"
+coverage = "^7.2.6"
 bumpsemver = "*"
 
 [tool.pylint]
 max-line-length = 120
+
+[tool.pylint.main]
+string-quote = "double"
+triple-quote = "double"
+docstring-quote = "double"
+
+[tool.mypy]
+[[tool.mypy.overrides]]
+module = [
+    "pandas",
+    "scipy.*",
+    "rcplus_alloy_common",
+]
+ignore_missing_imports = true
+
+[tool.vulture]
+ignore_names = ["logger"]
+
+[tool.pytest.ini_options]
+addopts = "-rsxX -vv --capture=tee-sys"
+testpaths = ["tests"]
+python_files="tests/*.py"
+log_cli = "0"
+log_cli_level = "INFO"
+log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
```

### Comparing `rcplus_alloy_common-0.2.0/PKG-INFO` & `rcplus_alloy_common-1.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 Metadata-Version: 2.1
 Name: rcplus-alloy-common
-Version: 0.2.0
+Version: 1.0.0
 Summary: RC+/Alloy helpers functions for Python
 Home-page: https://github.com/ringier-data/rcplus-alloy-lib-py-common
 License: Proprietary
 Keywords: rcplus,alloy,logging,metrics,utilities
 Author: Ringier AG
 Author-email: info@rcplus.io
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.10,<4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Utilities
-Provides-Extra: logzio
+Provides-Extra: airflow
+Requires-Dist: apache-airflow[amazon,slack] (>=2.6.1,<3.0.0) ; extra == "airflow"
 Requires-Dist: jsonschema (>=3.0.0)
-Requires-Dist: logzio-python-handler (>=4.0.0) ; extra == "logzio"
 Requires-Dist: python-json-logger (>=2.0.4)
+Requires-Dist: pytz (>=2023.3,<2024.0) ; extra == "airflow"
 Requires-Dist: requests (>=2.6.1)
 Project-URL: Repository, https://github.com/ringier-data/rcplus-alloy-lib-py-common
 Description-Content-Type: text/markdown
 
 # rcplus-alloy-lib-py-common
 
 ![PyPI](https://img.shields.io/pypi/v/rcplus-alloy-common)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/rcplus-alloy-common)
-[![Codacy Badge](https://app.codacy.com/project/badge/Grade/c215bf6e2fbc4c9fb8230b7c7d237686)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ringier-data/rcplus-alloy-lib-py-common&amp;utm_campaign=Badge_Grade)
-[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/c215bf6e2fbc4c9fb8230b7c7d237686)](https://www.codacy.com?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ringier-data/rcplus-alloy-lib-py-common&amp;utm_campaign=Badge_Coverage)
+![Coverage badge](./coverage.svg)
 
-Current version: **v0.2.0**
+Current version: **v1.0.0**
 
 ---
 
-Python utilities for RC+/Alloy. _**NOTE**_: This Python package is published to PyPI.org as publicly available package.
+Python utilities for RC+/Alloy.
+
+_**NOTE**_: This Python package is published to PyPI.org as publicly available package.
 
 ## Install
 
 ```bash
 pip install -U rcplus-alloy-common
 ```
 
@@ -53,7 +53,15 @@
 
 TODO
 
 ### Application metrics
 
 TODO
 
+### Airflow
+
+```bash
+pip install -U rcplus-alloy-common[airflow]
+```
+
+TODO
+
```


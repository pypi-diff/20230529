# Comparing `tmp/prometheus-pve-sd-2.5.8.tar.gz` & `tmp/prometheus-pve-sd-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus-pve-sd-2.5.8.tar", max compression
+gzip compressed data, was "prometheus-pve-sd-2.5.9.tar", max compression
```

## Comparing `prometheus-pve-sd-2.5.8.tar` & `prometheus-pve-sd-2.5.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1123 2022-08-22 19:20:31.394032 prometheus-pve-sd-2.5.8/LICENSE
--rw-r--r--   0        0        0     2669 2022-08-22 19:20:31.394032 prometheus-pve-sd-2.5.8/README.md
--rw-r--r--   0        0        0       46 2022-08-22 19:20:41.241769 prometheus-pve-sd-2.5.8/prometheuspvesd/__init__.py
--rw-r--r--   0        0        0     6040 2022-08-22 19:20:31.394032 prometheus-pve-sd-2.5.8/prometheuspvesd/cli.py
--rw-r--r--   0        0        0     3439 2022-08-22 19:20:31.394032 prometheus-pve-sd-2.5.8/prometheuspvesd/client.py
--rw-r--r--   0        0        0     9606 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/config.py
--rw-r--r--   0        0        0     7842 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/discovery.py
--rw-r--r--   0        0        0      559 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/exception.py
--rw-r--r--   0        0        0     7770 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/logger.py
--rw-r--r--   0        0        0     1884 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/model.py
--rw-r--r--   0        0        0       30 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/test/__init__.py
--rw-r--r--   0        0        0      378 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/test/data/config.yml
--rw-r--r--   0        0        0       28 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/test/fixtures/__init__.py
--rw-r--r--   0        0        0    10533 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/test/fixtures/fixtures.py
--rw-r--r--   0        0        0      370 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/test/unit/conftest.py
--rw-r--r--   0        0        0     3030 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/test/unit/test_cli.py
--rw-r--r--   0        0        0     1003 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/test/unit/test_config.py
--rw-r--r--   0        0        0     3574 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/test/unit/test_discovery.py
--rw-r--r--   0        0        0     1333 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/test/unit/test_model.py
--rw-r--r--   0        0        0      440 2022-08-22 19:20:31.398032 prometheus-pve-sd-2.5.8/prometheuspvesd/utils.py
--rw-r--r--   0        0        0     2683 2022-08-22 19:20:41.237769 prometheus-pve-sd-2.5.8/pyproject.toml
--rw-r--r--   0        0        0     3869 2022-08-22 19:20:41.696845 prometheus-pve-sd-2.5.8/setup.py
--rw-r--r--   0        0        0     4240 2022-08-22 19:20:41.697210 prometheus-pve-sd-2.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1123 2022-09-06 07:46:46.381046 prometheus-pve-sd-2.5.9/LICENSE
+-rw-r--r--   0        0        0     2669 2022-09-06 07:46:46.381046 prometheus-pve-sd-2.5.9/README.md
+-rw-r--r--   0        0        0       46 2022-09-06 07:47:02.164971 prometheus-pve-sd-2.5.9/prometheuspvesd/__init__.py
+-rw-r--r--   0        0        0     6040 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/cli.py
+-rw-r--r--   0        0        0     3439 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/client.py
+-rw-r--r--   0        0        0     9606 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/config.py
+-rw-r--r--   0        0        0     7842 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/discovery.py
+-rw-r--r--   0        0        0      559 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/exception.py
+-rw-r--r--   0        0        0     7770 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/logger.py
+-rw-r--r--   0        0        0     1884 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/model.py
+-rw-r--r--   0        0        0       30 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/test/__init__.py
+-rw-r--r--   0        0        0      378 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/test/data/config.yml
+-rw-r--r--   0        0        0       28 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/test/fixtures/__init__.py
+-rw-r--r--   0        0        0    10533 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/test/fixtures/fixtures.py
+-rw-r--r--   0        0        0      370 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/test/unit/conftest.py
+-rw-r--r--   0        0        0     3030 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/test/unit/test_cli.py
+-rw-r--r--   0        0        0     1003 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/test/unit/test_config.py
+-rw-r--r--   0        0        0     3574 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/test/unit/test_discovery.py
+-rw-r--r--   0        0        0     1333 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/test/unit/test_model.py
+-rw-r--r--   0        0        0      440 2022-09-06 07:46:46.385046 prometheus-pve-sd-2.5.9/prometheuspvesd/utils.py
+-rw-r--r--   0        0        0     2682 2022-09-06 07:47:02.164971 prometheus-pve-sd-2.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 prometheus-pve-sd-2.5.9/setup.py
+-rw-r--r--   0        0        0     4489 1970-01-01 00:00:00.000000 prometheus-pve-sd-2.5.9/PKG-INFO
```

### Comparing `prometheus-pve-sd-2.5.8/LICENSE` & `prometheus-pve-sd-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/README.md` & `prometheus-pve-sd-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/cli.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/cli.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/client.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/client.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/config.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/config.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/discovery.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/discovery.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/exception.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/exception.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/logger.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/logger.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/model.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/model.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/test/fixtures/fixtures.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/test/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/test/unit/test_cli.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/test/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/test/unit/test_config.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/test/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/test/unit/test_discovery.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/test/unit/test_discovery.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/prometheuspvesd/test/unit/test_model.py` & `prometheus-pve-sd-2.5.9/prometheuspvesd/test/unit/test_model.py`

 * *Files identical despite different names*

### Comparing `prometheus-pve-sd-2.5.8/pyproject.toml` & `prometheus-pve-sd-2.5.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -22,22 +22,22 @@
 include = ["LICENSE"]
 keywords = ["prometheus", "sd", "pve", "metrics"]
 license = "MIT"
 name = "prometheus-pve-sd"
 packages = [{ include = "prometheuspvesd" }]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/prometheus-pve-sd/"
-version = "2.5.8"
+version = "2.5.9"
 
 [tool.poetry.dependencies]
 anyconfig = "0.13.0"
 appdirs = "1.4.4"
 colorama = "0.4.5"
 environs = "9.5.0"
-jsonschema = "4.14.0"
+jsonschema = "4.15.0"
 nested-lookup = "0.2.25"
 prometheus-client = "0.14.1"
 proxmoxer = "1.3.1"
 python = "^3.7.0"
 python-json-logger = "2.0.4"
 requests = "2.28.1"
 "ruamel.yaml" = "0.17.21"
@@ -52,25 +52,25 @@
 flake8-isort = "4.2.0"
 flake8-logging-format = "0.7.5"
 flake8-pep3101 = "1.3.0"
 flake8-polyfill = "1.0.2"
 flake8-quotes = "3.3.1"
 pep8-naming = "0.13.2"
 pydocstyle = "6.1.1"
-pytest = "7.1.2"
+pytest = "7.1.3"
 pytest-cov = "3.0.0"
 pytest-mock = "3.8.2"
 yapf = "0.32.0"
 toml = "0.10.2"
 
 [tool.poetry.scripts]
 prometheus-pve-sd = "prometheuspvesd.cli:main"
 
 [tool.poetry-dynamic-versioning]
-enable = false
+enable = true
 style = "semver"
 vcs = "git"
 
 [tool.isort]
 default_section = "THIRDPARTY"
 force_single_line = true
 line_length = 99
```

### Comparing `prometheus-pve-sd-2.5.8/setup.py` & `prometheus-pve-sd-2.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,34 +11,34 @@
 {'': ['*'], 'prometheuspvesd.test': ['data/*']}
 
 install_requires = \
 ['anyconfig==0.13.0',
  'appdirs==1.4.4',
  'colorama==0.4.5',
  'environs==9.5.0',
- 'jsonschema==4.14.0',
+ 'jsonschema==4.15.0',
  'nested-lookup==0.2.25',
  'prometheus-client==0.14.1',
  'proxmoxer==1.3.1',
  'python-json-logger==2.0.4',
  'requests==2.28.1',
  'ruamel.yaml==0.17.21']
 
 entry_points = \
 {'console_scripts': ['prometheus-pve-sd = prometheuspvesd.cli:main']}
 
 setup_kwargs = {
     'name': 'prometheus-pve-sd',
-    'version': '2.5.8',
+    'version': '2.5.9',
     'description': 'Prometheus Service Discovery for Proxmox VE.',
     'long_description': "# prometheus-pve-sd\n\nPrometheus Service Discovery for Proxmox VE\n\n[![Build Status](https://img.shields.io/drone/build/thegeeklab/prometheus-pve-sd?logo=drone&server=https%3A%2F%2Fdrone.thegeeklab.de)](https://drone.thegeeklab.de/thegeeklab/prometheus-pve-sd)\n[![Docker Hub](https://img.shields.io/badge/dockerhub-latest-blue.svg?logo=docker&logoColor=white)](https://hub.docker.com/r/thegeeklab/prometheus-pve-sd)\n[![Quay.io](https://img.shields.io/badge/quay-latest-blue.svg?logo=docker&logoColor=white)](https://quay.io/repository/thegeeklab/prometheus-pve-sd)\n[![Python Version](https://img.shields.io/pypi/pyversions/prometheus-pve-sd.svg)](https://pypi.org/project/prometheus-pve-sd/)\n[![PyPI Status](https://img.shields.io/pypi/status/prometheus-pve-sd.svg)](https://pypi.org/project/prometheus-pve-sd/)\n[![PyPI Release](https://img.shields.io/pypi/v/prometheus-pve-sd.svg)](https://pypi.org/project/prometheus-pve-sd/)\n[![Codecov](https://img.shields.io/codecov/c/github/thegeeklab/prometheus-pve-sd)](https://codecov.io/gh/thegeeklab/prometheus-pve-sd)\n[![GitHub contributors](https://img.shields.io/github/contributors/thegeeklab/prometheus-pve-sd)](https://github.com/thegeeklab/prometheus-pve-sd/graphs/contributors)\n[![Source: GitHub](https://img.shields.io/badge/source-github-blue.svg?logo=github&logoColor=white)](https://github.com/thegeeklab/prometheus-pve-sd)\n[![License: MIT](https://img.shields.io/github/license/thegeeklab/prometheus-pve-sd)](https://github.com/thegeeklab/prometheus-pve-sd/blob/main/LICENSE)\n\nThis project provides a simple custom service discovery for [Prometheus](https://prometheus.io/). It is using the [Proxmox VE](https://www.proxmox.com/de/proxmox-ve) (PVE) API to fetch Hosts and it's meta information to generate a Prometheus compatible [file based](https://prometheus.io/docs/guides/file-sd/) service discovery. Releases are available as Python Packages on [GitHub](https://github.com/thegeeklab/prometheus-pve-sd/releases) or [PyPI](https://pypi.org/project/prometheus-pve-sd/) and as Docker Image on [Docker Hub](https://hub.docker.com/r/thegeeklab/prometheus-pve-sd).\n\nYou can find the full documentation at [https://prometheus-pve-sd.geekdocs.de](https://prometheus-pve-sd.geekdocs.de).\n\n## Contributors\n\nSpecial thanks to all [contributors](https://github.com/thegeeklab/prometheus-pve-sd/graphs/contributors). If you would like to contribute,\nplease see the [instructions](https://github.com/thegeeklab/prometheus-pve-sd/blob/main/CONTRIBUTING.md).\n\n## License\n\nThis project is licensed under the MIT License - see the [LICENSE](https://github.com/thegeeklab/prometheus-pve-sd/blob/main/LICENSE) file for details.\n",
     'author': 'Robert Kaussow',
     'author_email': 'mail@thegeeklab.de',
-    'maintainer': None,
-    'maintainer_email': None,
+    'maintainer': 'None',
+    'maintainer_email': 'None',
     'url': 'https://github.com/thegeeklab/prometheus-pve-sd/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.7.0,<4.0.0',
 }
```

### Comparing `prometheus-pve-sd-2.5.8/PKG-INFO` & `prometheus-pve-sd-2.5.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-pve-sd
-Version: 2.5.8
+Version: 2.5.9
 Summary: Prometheus Service Discovery for Proxmox VE.
 Home-page: https://github.com/thegeeklab/prometheus-pve-sd/
 License: MIT
 Keywords: prometheus,sd,pve,metrics
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.7.0,<4.0.0
@@ -13,24 +13,29 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Utilities
 Requires-Dist: anyconfig (==0.13.0)
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: colorama (==0.4.5)
 Requires-Dist: environs (==9.5.0)
-Requires-Dist: jsonschema (==4.14.0)
+Requires-Dist: jsonschema (==4.15.0)
 Requires-Dist: nested-lookup (==0.2.25)
 Requires-Dist: prometheus-client (==0.14.1)
 Requires-Dist: proxmoxer (==1.3.1)
 Requires-Dist: python-json-logger (==2.0.4)
 Requires-Dist: requests (==2.28.1)
 Requires-Dist: ruamel.yaml (==0.17.21)
 Project-URL: Documentation, https://github.com/thegeeklab/prometheus-pve-sd/
```


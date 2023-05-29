# Comparing `tmp/docker-tidy-1.1.8.tar.gz` & `tmp/docker-tidy-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docker-tidy-1.1.8.tar", max compression
+gzip compressed data, was "docker-tidy-1.1.9.tar", max compression
```

## Comparing `docker-tidy-1.1.8.tar` & `docker-tidy-1.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11366 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/LICENSE
--rw-r--r--   0        0        0     1913 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/README.md
--rw-r--r--   0        0        0       46 2022-01-10 09:12:38.641222 docker-tidy-1.1.8/dockertidy/__init__.py
--rw-r--r--   0        0        0     3136 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/autostop.py
--rw-r--r--   0        0        0     4870 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/cli.py
--rw-r--r--   0        0        0     8493 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/config.py
--rw-r--r--   0        0        0      423 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/exception.py
--rw-r--r--   0        0        0    11981 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/garbage_collector.py
--rw-r--r--   0        0        0     5914 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/logger.py
--rw-r--r--   0        0        0     1231 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/parser.py
--rw-r--r--   0        0        0        0 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/test/__init__.py
--rw-r--r--   0        0        0        0 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/test/fixtures/__init__.py
--rw-r--r--   0        0        0     1942 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/test/fixtures/fixtures.py
--rw-r--r--   0        0        0     1244 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/test/unit/test_autostop.py
--rw-r--r--   0        0        0    12321 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/test/unit/test_garbagecollector.py
--rw-r--r--   0        0        0      614 2022-01-10 09:12:28.869451 docker-tidy-1.1.8/dockertidy/utils.py
--rw-r--r--   0        0        0     2823 2022-01-10 09:12:38.637222 docker-tidy-1.1.8/pyproject.toml
--rw-r--r--   0        0        0     3166 2022-01-10 09:12:38.988253 docker-tidy-1.1.8/setup.py
--rw-r--r--   0        0        0     3808 2022-01-10 09:12:38.988575 docker-tidy-1.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11366 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/LICENSE
+-rw-r--r--   0        0        0     1913 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/README.md
+-rw-r--r--   0        0        0       46 2022-02-01 11:25:46.105038 docker-tidy-1.1.9/dockertidy/__init__.py
+-rw-r--r--   0        0        0     3136 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/autostop.py
+-rw-r--r--   0        0        0     4870 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/cli.py
+-rw-r--r--   0        0        0     8493 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/config.py
+-rw-r--r--   0        0        0      423 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/exception.py
+-rw-r--r--   0        0        0    11981 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/garbage_collector.py
+-rw-r--r--   0        0        0     5914 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/logger.py
+-rw-r--r--   0        0        0     1231 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/parser.py
+-rw-r--r--   0        0        0        0 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/test/__init__.py
+-rw-r--r--   0        0        0        0 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/test/fixtures/__init__.py
+-rw-r--r--   0        0        0     1942 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/test/fixtures/fixtures.py
+-rw-r--r--   0        0        0     1244 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/test/unit/test_autostop.py
+-rw-r--r--   0        0        0    12321 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/test/unit/test_garbagecollector.py
+-rw-r--r--   0        0        0      614 2022-02-01 11:25:35.740732 docker-tidy-1.1.9/dockertidy/utils.py
+-rw-r--r--   0        0        0     2823 2022-02-01 11:25:46.105038 docker-tidy-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3166 2022-02-01 11:25:46.516761 docker-tidy-1.1.9/setup.py
+-rw-r--r--   0        0        0     3808 2022-02-01 11:25:46.517089 docker-tidy-1.1.9/PKG-INFO
```

### Comparing `docker-tidy-1.1.8/LICENSE` & `docker-tidy-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/README.md` & `docker-tidy-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/dockertidy/autostop.py` & `docker-tidy-1.1.9/dockertidy/autostop.py`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/dockertidy/cli.py` & `docker-tidy-1.1.9/dockertidy/cli.py`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/dockertidy/config.py` & `docker-tidy-1.1.9/dockertidy/config.py`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/dockertidy/garbage_collector.py` & `docker-tidy-1.1.9/dockertidy/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/dockertidy/logger.py` & `docker-tidy-1.1.9/dockertidy/logger.py`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/dockertidy/parser.py` & `docker-tidy-1.1.9/dockertidy/parser.py`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/dockertidy/test/fixtures/fixtures.py` & `docker-tidy-1.1.9/dockertidy/test/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/dockertidy/test/unit/test_autostop.py` & `docker-tidy-1.1.9/dockertidy/test/unit/test_autostop.py`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/dockertidy/test/unit/test_garbagecollector.py` & `docker-tidy-1.1.9/dockertidy/test/unit/test_garbagecollector.py`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/dockertidy/utils.py` & `docker-tidy-1.1.9/dockertidy/utils.py`

 * *Files identical despite different names*

### Comparing `docker-tidy-1.1.8/pyproject.toml` & `docker-tidy-1.1.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -28,55 +28,55 @@
 license = "Apache-2.0"
 name = "docker-tidy"
 packages = [
   {include = "dockertidy"},
 ]
 readme = "README.md"
 repository = "https://github.com/thegeeklab/docker-tidy/"
-version = "1.1.8"
+version = "1.1.9"
 
 [tool.poetry.dependencies]
 anyconfig = "0.12.0"
 appdirs = "1.4.4"
 certifi = "2021.10.8"
 colorama = "0.4.4"
 dateparser = "1.1.0"
 docker = "5.0.3"
 docker-pycreds = "0.4.0"
-environs = "9.4.0"
+environs = "9.5.0"
 idna = "3.3"
 ipaddress = "1.0.23"
-jsonschema = "4.3.3"
+jsonschema = "4.4.0"
 nested-lookup = "0.2.23"
 pathspec = "0.9.0"
 python = "^3.7.0"
 python-dateutil = "2.8.2"
 python-json-logger = "2.0.2"
 requests = "2.27.1"
 "ruamel.yaml" = "0.17.20"
 websocket_client = "1.2.3"
 zipp = "3.7.0"
 
 [tool.poetry.dev-dependencies]
-bandit = "1.7.1"
+bandit = "1.7.2"
 flake8 = "4.0.1"
 flake8-blind-except = "0.2.0"
 flake8-builtins = "1.5.3"
 flake8-docstrings = "1.6.0"
 flake8-eradicate = "1.2.0"
 flake8-isort = "4.1.1"
 flake8-logging-format = "0.6.0"
 flake8-pep3101 = "1.3.0"
 flake8-polyfill = "1.0.2"
 flake8-quotes = "3.3.1"
 pep8-naming = "0.12.1"
 pydocstyle = "6.1.1"
 pytest = "6.2.5"
 pytest-cov = "3.0.0"
-pytest-mock = "3.6.1"
+pytest-mock = "3.7.0"
 tomli = "2.0.0"
 yapf = "0.32.0"
 
 [tool.poetry.scripts]
 docker-tidy = "dockertidy.cli:main"
 
 [tool.poetry-dynamic-versioning]
```

### Comparing `docker-tidy-1.1.8/setup.py` & `docker-tidy-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,33 +14,33 @@
 ['anyconfig==0.12.0',
  'appdirs==1.4.4',
  'certifi==2021.10.8',
  'colorama==0.4.4',
  'dateparser==1.1.0',
  'docker-pycreds==0.4.0',
  'docker==5.0.3',
- 'environs==9.4.0',
+ 'environs==9.5.0',
  'idna==3.3',
  'ipaddress==1.0.23',
- 'jsonschema==4.3.3',
+ 'jsonschema==4.4.0',
  'nested-lookup==0.2.23',
  'pathspec==0.9.0',
  'python-dateutil==2.8.2',
  'python-json-logger==2.0.2',
  'requests==2.27.1',
  'ruamel.yaml==0.17.20',
  'websocket_client==1.2.3',
  'zipp==3.7.0']
 
 entry_points = \
 {'console_scripts': ['docker-tidy = dockertidy.cli:main']}
 
 setup_kwargs = {
     'name': 'docker-tidy',
-    'version': '1.1.8',
+    'version': '1.1.9',
     'description': 'Keep docker hosts tidy.',
     'long_description': '# docker-tidy\n\nKeep docker hosts tidy\n\n[![Build Status](https://img.shields.io/drone/build/thegeeklab/docker-tidy?logo=drone&server=https%3A%2F%2Fdrone.thegeeklab.de)](https://drone.thegeeklab.de/thegeeklab/docker-tidy)\n[![Docker Hub](https://img.shields.io/badge/docker-latest-blue.svg?logo=docker&logoColor=white)](https://hub.docker.com/r/thegeeklab/docker-tidy)\n[![Python Version](https://img.shields.io/pypi/pyversions/docker-tidy.svg)](https://pypi.org/project/docker-tidy/)\n[![PyPI Status](https://img.shields.io/pypi/status/docker-tidy.svg)](https://pypi.org/project/docker-tidy/)\n[![PyPI Release](https://img.shields.io/pypi/v/docker-tidy.svg)](https://pypi.org/project/docker-tidy/)\n[![Codecov](https://img.shields.io/codecov/c/github/thegeeklab/docker-tidy)](https://codecov.io/gh/thegeeklab/docker-tidy)\n[![GitHub contributors](https://img.shields.io/github/contributors/thegeeklab/docker-tidy)](https://github.com/thegeeklab/docker-tidy/graphs/contributors)\n[![Source: GitHub](https://img.shields.io/badge/source-github-blue.svg?logo=github&logoColor=white)](https://github.com/thegeeklab/docker-tidy)\n[![License: Apache-2.0](https://img.shields.io/github/license/thegeeklab/docker-tidy)](https://github.com/thegeeklab/docker-tidy/blob/main/LICENSE)\n\nThis project is a fork of [Yelp/docker-custodian](https://github.com/Yelp/docker-custodian). Keep docker hosts tidy.\n\nYou can find the full documentation at [https://docker-tidy.geekdocs.de](https://docker-tidy.geekdocs.de/).\n\n## Contributors\n\nSpecial thanks goes to all [contributors](https://github.com/thegeeklab/docker-tidy/graphs/contributors). If you would like to contribute,\nplease see the [instructions](https://github.com/thegeeklab/docker-tidy/blob/main/CONTRIBUTING.md).\n\n## License\n\nThis project is licensed under the Apache-2.0 License - see the [LICENSE](https://github.com/thegeeklab/docker-tidy/blob/main/LICENSE) file for details.\n',
     'author': 'Robert Kaussow',
     'author_email': 'mail@thegeeklab.de',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://docker-tidy.geekdocs.de/',
```

### Comparing `docker-tidy-1.1.8/PKG-INFO` & `docker-tidy-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docker-tidy
-Version: 1.1.8
+Version: 1.1.9
 Summary: Keep docker hosts tidy.
 Home-page: https://docker-tidy.geekdocs.de/
 License: Apache-2.0
 Keywords: docker,gc,prune,garbage
 Author: Robert Kaussow
 Author-email: mail@thegeeklab.de
 Requires-Python: >=3.7.0,<4.0.0
@@ -27,18 +27,18 @@
 Requires-Dist: anyconfig (==0.12.0)
 Requires-Dist: appdirs (==1.4.4)
 Requires-Dist: certifi (==2021.10.8)
 Requires-Dist: colorama (==0.4.4)
 Requires-Dist: dateparser (==1.1.0)
 Requires-Dist: docker (==5.0.3)
 Requires-Dist: docker-pycreds (==0.4.0)
-Requires-Dist: environs (==9.4.0)
+Requires-Dist: environs (==9.5.0)
 Requires-Dist: idna (==3.3)
 Requires-Dist: ipaddress (==1.0.23)
-Requires-Dist: jsonschema (==4.3.3)
+Requires-Dist: jsonschema (==4.4.0)
 Requires-Dist: nested-lookup (==0.2.23)
 Requires-Dist: pathspec (==0.9.0)
 Requires-Dist: python-dateutil (==2.8.2)
 Requires-Dist: python-json-logger (==2.0.2)
 Requires-Dist: requests (==2.27.1)
 Requires-Dist: ruamel.yaml (==0.17.20)
 Requires-Dist: websocket_client (==1.2.3)
```


# Comparing `tmp/pwdriver-0.26.9.tar.gz` & `tmp/pwdriver-0.27.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pwdriver-0.26.9.tar", last modified: Sun Jan 29 11:42:57 2023, max compression
+gzip compressed data, was "pwdriver-0.27.2.tar", max compression
```

## Comparing `pwdriver-0.26.9.tar` & `pwdriver-0.27.2.tar`

### file list

```diff
@@ -1,19 +1,10 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 11:42:57.658460 pwdriver-0.26.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-01-29 11:42:48.000000 pwdriver-0.26.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-01-29 11:42:57.658460 pwdriver-0.26.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-01-29 11:42:48.000000 pwdriver-0.26.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 11:42:57.654460 pwdriver-0.26.9/pwdriver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-29 11:42:48.000000 pwdriver-0.26.9/pwdriver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11601 2023-01-29 11:42:48.000000 pwdriver-0.26.9/pwdriver/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-01-29 11:42:48.000000 pwdriver-0.26.9/pwdriver/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-01-29 11:42:48.000000 pwdriver-0.26.9/pwdriver/page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-01-29 11:42:48.000000 pwdriver-0.26.9/pwdriver/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-01-29 11:42:48.000000 pwdriver-0.26.9/pwdriver/val.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-29 11:42:57.658460 pwdriver-0.26.9/pwdriver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-01-29 11:42:57.000000 pwdriver-0.26.9/pwdriver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-29 11:42:57.000000 pwdriver-0.26.9/pwdriver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-29 11:42:57.000000 pwdriver-0.26.9/pwdriver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-01-29 11:42:57.000000 pwdriver-0.26.9/pwdriver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-29 11:42:57.000000 pwdriver-0.26.9/pwdriver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-29 11:42:57.658460 pwdriver-0.26.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-01-29 11:42:48.000000 pwdriver-0.26.9/setup.py
+-rw-r--r--   0        0        0     1074 2023-05-29 16:32:27.591685 pwdriver-0.27.2/LICENSE
+-rw-r--r--   0        0        0     5485 2023-05-29 16:32:27.591685 pwdriver-0.27.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/__init__.py
+-rw-r--r--   0        0        0    11601 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/core.py
+-rw-r--r--   0        0        0     1358 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/listener.py
+-rw-r--r--   0        0        0     4199 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/page.py
+-rw-r--r--   0        0        0     1333 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/util.py
+-rw-r--r--   0        0        0     1024 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pwdriver/val.py
+-rw-r--r--   0        0        0     1352 2023-05-29 16:32:27.591685 pwdriver-0.27.2/pyproject.toml
+-rw-r--r--   0        0        0     6765 1970-01-01 00:00:00.000000 pwdriver-0.27.2/PKG-INFO
```

### Comparing `pwdriver-0.26.9/LICENSE` & `pwdriver-0.27.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pwdriver-0.26.9/PKG-INFO` & `pwdriver-0.27.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: pwdriver
-Version: 0.26.9
+Version: 0.27.2
 Summary: It will download a WebDriver, and then set basic configuration automatically.
 Home-page: https://github.com/jinmoo21/pwdriver
+License: MIT
+Keywords: python,testing,automation,webdriver,selenium,test-automation,selenium-webdriver,appium,appium-webdriver
 Author: Jinmoo Han
 Author-email: jinmoo21@naver.com
-License: MIT
-Classifier: Topic :: Software Development :: Quality Assurance
-Classifier: Topic :: Software Development :: Testing
+Maintainer: Jinmoo Han
+Maintainer-email: jinmoo21@naver.com
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Classifier: Topic :: Software Development :: Quality Assurance
+Classifier: Topic :: Software Development :: Testing
+Requires-Dist: Appium-Python-Client (>=2.10.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: selenium (>=4.9.1,<5.0.0)
+Project-URL: Bug Reports, https://github.com/jinmoo21/pwdriver/issues
+Project-URL: Repository, https://github.com/jinmoo21/pwdriver
 Description-Content-Type: text/markdown
-License-File: LICENSE
 
 # PWDriver (PyWebDriver)
 
 [![E2e test](https://github.com/jinmoo21/pwdriver/actions/workflows/python_test.yml/badge.svg)](https://github.com/jinmoo21/pwdriver/actions/workflows/python_test.yml)
 [![Code Coverage](https://codecov.io/gh/jinmoo21/pwdriver/branch/master/graph/badge.svg)](https://codecov.io/gh/jinmoo21/pwdriver)
 
 [![Release status](https://github.com/jinmoo21/pwdriver/actions/workflows/python_release.yml/badge.svg)](https://github.com/jinmoo21/pwdriver/actions/workflows/python_release.yml)
```

### Comparing `pwdriver-0.26.9/README.md` & `pwdriver-0.27.2/README.md`

 * *Files identical despite different names*

### Comparing `pwdriver-0.26.9/pwdriver/core.py` & `pwdriver-0.27.2/pwdriver/core.py`

 * *Files identical despite different names*

### Comparing `pwdriver-0.26.9/pwdriver/listener.py` & `pwdriver-0.27.2/pwdriver/listener.py`

 * *Files identical despite different names*

### Comparing `pwdriver-0.26.9/pwdriver/page.py` & `pwdriver-0.27.2/pwdriver/page.py`

 * *Files identical despite different names*

### Comparing `pwdriver-0.26.9/pwdriver/util.py` & `pwdriver-0.27.2/pwdriver/util.py`

 * *Files identical despite different names*

### Comparing `pwdriver-0.26.9/pwdriver/val.py` & `pwdriver-0.27.2/pwdriver/val.py`

 * *Files identical despite different names*


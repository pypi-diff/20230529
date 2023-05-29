# Comparing `tmp/aiodiskqueue-0.1.0a9.tar.gz` & `tmp/aiodiskqueue-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0a9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0b1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0a9.tar` & `aiodiskqueue-0.1.0b1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a9/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a9/.github/workflows/main.yml
--rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0a9/.github/workflows/release.yml
--rw-r--r--   0        0        0      113 2023-05-28 13:27:18.116278 aiodiskqueue-0.1.0a9/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a9/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a9/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a9/LICENSE
--rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0a9/Makefile
--rw-r--r--   0        0        0     2170 2023-05-28 14:06:56.935356 aiodiskqueue-0.1.0a9/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a9/docs/Makefile
--rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0a9/docs/_static/custom.css
--rw-r--r--   0        0        0      110 2023-05-28 18:07:59.394553 aiodiskqueue-0.1.0a9/docs/api.rst
--rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0a9/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a9/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a9/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a9/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0a9/examples/basic_usage.py
--rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0a9/examples/multiple_consumers.py
--rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0a9/examples/single_consumer.py
--rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a9/pyproject.toml
--rw-r--r--   0        0        0      211 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0a9/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0     7836 2023-05-28 18:28:49.530087 aiodiskqueue-0.1.0a9/src/aiodiskqueue/core.py
--rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0a9/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0a9/src/aiodiskqueue/utils.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a9/tests/__init__.py
--rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0a9/tests/factories.py
--rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0a9/tests/helpers.py
--rw-r--r--   0        0        0     3158 2023-05-28 14:06:56.951355 aiodiskqueue-0.1.0a9/tests/loadtest.py
--rw-r--r--   0        0        0     6476 2023-05-28 18:50:55.148916 aiodiskqueue-0.1.0a9/tests/test_core.py
--rw-r--r--   0        0        0     2493 2023-05-28 18:39:49.776986 aiodiskqueue-0.1.0a9/tests/test_integration.py
--rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0a9/tests/test_utils.py
--rw-r--r--   0        0        0      413 2023-05-26 21:16:13.559594 aiodiskqueue-0.1.0a9/tox.ini
--rw-r--r--   0        0        0     2974 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a9/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0b1/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0b1/.github/workflows/main.yml
+-rw-r--r--   0        0        0      798 2023-05-28 19:18:15.116717 aiodiskqueue-0.1.0b1/.github/workflows/release.yml
+-rw-r--r--   0        0        0      113 2023-05-28 13:27:18.116278 aiodiskqueue-0.1.0b1/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0b1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0b1/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0b1/LICENSE
+-rw-r--r--   0        0        0      121 2023-05-28 14:06:56.931356 aiodiskqueue-0.1.0b1/Makefile
+-rw-r--r--   0        0        0     2124 2023-05-29 15:23:28.059933 aiodiskqueue-0.1.0b1/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0b1/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0b1/docs/_static/custom.css
+-rw-r--r--   0        0        0      110 2023-05-28 18:07:59.394553 aiodiskqueue-0.1.0b1/docs/api.rst
+-rw-r--r--   0        0        0     1884 2023-05-28 18:08:22.925790 aiodiskqueue-0.1.0b1/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0b1/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0b1/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0b1/examples/__init__.py
+-rw-r--r--   0        0        0      210 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b1/examples/basic_usage.py
+-rw-r--r--   0        0        0      933 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b1/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      879 2023-05-28 14:06:56.943355 aiodiskqueue-0.1.0b1/examples/single_consumer.py
+-rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0      211 2023-05-29 15:25:04.099811 aiodiskqueue-0.1.0b1/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0     7836 2023-05-28 18:28:49.530087 aiodiskqueue-0.1.0b1/src/aiodiskqueue/core.py
+-rw-r--r--   0        0        0      268 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b1/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0      714 2023-05-28 18:34:37.954258 aiodiskqueue-0.1.0b1/src/aiodiskqueue/utils.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0b1/tests/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-28 14:06:56.947355 aiodiskqueue-0.1.0b1/tests/factories.py
+-rw-r--r--   0        0        0      356 2023-05-28 18:38:14.973455 aiodiskqueue-0.1.0b1/tests/helpers.py
+-rw-r--r--   0        0        0     3158 2023-05-28 14:06:56.951355 aiodiskqueue-0.1.0b1/tests/loadtest.py
+-rw-r--r--   0        0        0     6476 2023-05-28 18:50:55.148916 aiodiskqueue-0.1.0b1/tests/test_core.py
+-rw-r--r--   0        0        0     2493 2023-05-28 18:39:49.776986 aiodiskqueue-0.1.0b1/tests/test_integration.py
+-rw-r--r--   0        0        0      627 2023-05-28 17:55:30.938412 aiodiskqueue-0.1.0b1/tests/test_utils.py
+-rw-r--r--   0        0        0      413 2023-05-26 21:16:13.559594 aiodiskqueue-0.1.0b1/tox.ini
+-rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0b1/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0a9/.github/workflows/main.yml` & `aiodiskqueue-0.1.0b1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/.github/workflows/release.yml` & `aiodiskqueue-0.1.0b1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/LICENSE` & `aiodiskqueue-0.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/README.rst` & `aiodiskqueue-0.1.0b1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
 This library provides a persistent FIFO queue for Python AsyncIO:
 
-- Queue content is preserved after a by process restart
+- Queue content can persist a process restart
 - Feature parity with Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
 - Similar API to Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
-- Designed for durability and decent performance
 - Sane logging
+- Type hints
 - Fully tested
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
```

### Comparing `aiodiskqueue-0.1.0a9/docs/Makefile` & `aiodiskqueue-0.1.0b1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/docs/conf.py` & `aiodiskqueue-0.1.0b1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/docs/make.bat` & `aiodiskqueue-0.1.0b1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0b1/examples/multiple_consumers.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/examples/single_consumer.py` & `aiodiskqueue-0.1.0b1/examples/single_consumer.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/pyproject.toml` & `aiodiskqueue-0.1.0b1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/src/aiodiskqueue/core.py` & `aiodiskqueue-0.1.0b1/src/aiodiskqueue/core.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/src/aiodiskqueue/utils.py` & `aiodiskqueue-0.1.0b1/src/aiodiskqueue/utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/tests/factories.py` & `aiodiskqueue-0.1.0b1/tests/factories.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/tests/loadtest.py` & `aiodiskqueue-0.1.0b1/tests/loadtest.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/tests/test_core.py` & `aiodiskqueue-0.1.0b1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/tests/test_integration.py` & `aiodiskqueue-0.1.0b1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/tests/test_utils.py` & `aiodiskqueue-0.1.0b1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a9/PKG-INFO` & `aiodiskqueue-0.1.0b1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0a9
+Version: 0.1.0b1
 Summary: Persistent queue for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -25,19 +25,19 @@
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
 This library provides a persistent FIFO queue for Python AsyncIO:
 
-- Queue content is preserved after a by process restart
+- Queue content can persist a process restart
 - Feature parity with Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
 - Similar API to Python's `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_
-- Designed for durability and decent performance
 - Sane logging
+- Type hints
 - Fully tested
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
```


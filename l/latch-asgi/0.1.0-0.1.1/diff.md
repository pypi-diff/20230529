# Comparing `tmp/latch_asgi-0.1.0.tar.gz` & `tmp/latch_asgi-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "latch_asgi-0.1.0.tar", max compression
+gzip compressed data, was "latch_asgi-0.1.1.tar", max compression
```

## Comparing `latch_asgi-0.1.0.tar` & `latch_asgi-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0       14 2023-05-29 19:32:41.850558 latch_asgi-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-29 19:37:32.876999 latch_asgi-0.1.0/latch_asgi/__init__.py
--rw-r--r--   0        0        0     5002 2023-05-29 19:42:37.064349 latch_asgi-0.1.0/latch_asgi/asgi_iface.py
--rw-r--r--   0        0        0     4999 2023-05-29 20:11:30.512830 latch_asgi-0.1.0/latch_asgi/auth.py
--rw-r--r--   0        0        0      240 2023-05-29 20:11:37.739187 latch_asgi-0.1.0/latch_asgi/config.py
--rw-r--r--   0        0        0     2802 2023-05-29 20:13:46.441816 latch_asgi-0.1.0/latch_asgi/context.py
--rw-r--r--   0        0        0     3306 2023-05-29 20:18:25.688320 latch_asgi-0.1.0/latch_asgi/datadog_propagator.py
--rw-r--r--   0        0        0     5261 2023-05-29 20:03:21.571328 latch_asgi-0.1.0/latch_asgi/framework.py
--rw-r--r--   0        0        0     8364 2023-05-29 20:29:49.450448 latch_asgi-0.1.0/latch_asgi/server.py
--rw-r--r--   0        0        0     1388 2023-05-29 20:23:34.621655 latch_asgi-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 latch_asgi-0.1.0/setup.py
--rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 latch_asgi-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       14 2023-05-29 19:32:41.850558 latch_asgi-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 19:37:32.876999 latch_asgi-0.1.1/latch_asgi/__init__.py
+-rw-r--r--   0        0        0     5002 2023-05-29 19:42:37.064349 latch_asgi-0.1.1/latch_asgi/asgi_iface.py
+-rw-r--r--   0        0        0     4999 2023-05-29 20:11:30.512830 latch_asgi-0.1.1/latch_asgi/auth.py
+-rw-r--r--   0        0        0      240 2023-05-29 20:11:37.739187 latch_asgi-0.1.1/latch_asgi/config.py
+-rw-r--r--   0        0        0     2802 2023-05-29 20:13:46.441816 latch_asgi-0.1.1/latch_asgi/context.py
+-rw-r--r--   0        0        0     3306 2023-05-29 20:18:25.688320 latch_asgi-0.1.1/latch_asgi/datadog_propagator.py
+-rw-r--r--   0        0        0     5261 2023-05-29 20:03:21.571328 latch_asgi-0.1.1/latch_asgi/framework.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:46:30.864706 latch_asgi-0.1.1/latch_asgi/py.typed
+-rw-r--r--   0        0        0     8364 2023-05-29 20:29:49.450448 latch_asgi-0.1.1/latch_asgi/server.py
+-rw-r--r--   0        0        0     1388 2023-05-29 20:46:39.814788 latch_asgi-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      945 1970-01-01 00:00:00.000000 latch_asgi-0.1.1/setup.py
+-rw-r--r--   0        0        0      870 1970-01-01 00:00:00.000000 latch_asgi-0.1.1/PKG-INFO
```

### Comparing `latch_asgi-0.1.0/latch_asgi/asgi_iface.py` & `latch_asgi-0.1.1/latch_asgi/asgi_iface.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.0/latch_asgi/auth.py` & `latch_asgi-0.1.1/latch_asgi/auth.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.0/latch_asgi/context.py` & `latch_asgi-0.1.1/latch_asgi/context.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.0/latch_asgi/datadog_propagator.py` & `latch_asgi-0.1.1/latch_asgi/datadog_propagator.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.0/latch_asgi/framework.py` & `latch_asgi-0.1.1/latch_asgi/framework.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.0/latch_asgi/server.py` & `latch_asgi-0.1.1/latch_asgi/server.py`

 * *Files identical despite different names*

### Comparing `latch_asgi-0.1.0/pyproject.toml` & `latch_asgi-0.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "latch-asgi"
-version = "0.1.0"
+version = "0.1.1"
 description = "ASGI python server"
 authors = ["Max Smolin <max@latch.bio>"]
 license = "CC0 1.0"
 readme = "README.md"
 packages = [{include = "latch_asgi"}]
 
 [tool.poetry.dependencies]
```

### Comparing `latch_asgi-0.1.0/setup.py` & `latch_asgi-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
  'opentelemetry-instrumentation-asgi>=0.36b0,<0.37',
  'opentelemetry-sdk>=1.15.0,<2.0.0',
  'orjson>=3.8.5,<4.0.0',
  'pysimdjson>=5.0.2,<6.0.0']
 
 setup_kwargs = {
     'name': 'latch-asgi',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'ASGI python server',
     'long_description': '# python-asgi\n',
     'author': 'Max Smolin',
     'author_email': 'max@latch.bio',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `latch_asgi-0.1.0/PKG-INFO` & `latch_asgi-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: latch-asgi
-Version: 0.1.0
+Version: 0.1.1
 Summary: ASGI python server
 License: CC0 1.0
 Author: Max Smolin
 Author-email: max@latch.bio
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


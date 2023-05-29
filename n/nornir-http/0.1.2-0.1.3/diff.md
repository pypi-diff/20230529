# Comparing `tmp/nornir_http-0.1.2.tar.gz` & `tmp/nornir_http-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_http-0.1.2.tar", max compression
+gzip compressed data, was "nornir_http-0.1.3.tar", max compression
```

## Comparing `nornir_http-0.1.2.tar` & `nornir_http-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0      282 2022-09-30 18:41:56.344091 nornir_http-0.1.2/README.md
--rw-r--r--   0        0        0       39 2022-09-30 18:41:56.344091 nornir_http-0.1.2/nornir_http/__init__.py
--rw-r--r--   0        0        0     1180 2022-09-30 18:41:56.344091 nornir_http-0.1.2/nornir_http/result.py
--rw-r--r--   0        0        0     1606 2022-09-30 18:41:56.344091 nornir_http-0.1.2/nornir_http/tasks.py
--rw-r--r--   0        0        0      637 2022-09-30 18:41:56.344091 nornir_http-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      982 1970-01-01 00:00:00.000000 nornir_http-0.1.2/setup.py
--rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 nornir_http-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      286 2023-05-29 20:04:44.133241 nornir_http-0.1.3/README.md
+-rw-r--r--   0        0        0       39 2023-05-29 20:04:44.133241 nornir_http-0.1.3/nornir_http/__init__.py
+-rw-r--r--   0        0        0     1179 2023-05-29 20:04:44.133241 nornir_http-0.1.3/nornir_http/result.py
+-rw-r--r--   0        0        0     1606 2023-05-29 20:04:44.133241 nornir_http-0.1.3/nornir_http/tasks.py
+-rw-r--r--   0        0        0      629 2023-05-29 20:04:44.133241 nornir_http-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1078 1970-01-01 00:00:00.000000 nornir_http-0.1.3/PKG-INFO
```

### Comparing `nornir_http-0.1.2/nornir_http/result.py` & `nornir_http-0.1.3/nornir_http/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,10 +26,9 @@
         self,
         host: Union["Host", None],
         response: Response,
         result: Any = None,
         failed: bool = False,
         **kwargs: Any
     ):
-
         super().__init__(host=host, result=result, failed=failed, **kwargs)
         self.response = response
```

### Comparing `nornir_http-0.1.2/nornir_http/tasks.py` & `nornir_http-0.1.3/nornir_http/tasks.py`

 * *Files identical despite different names*

### Comparing `nornir_http-0.1.2/pyproject.toml` & `nornir_http-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "nornir_http"
-version = "0.1.2"
+version = "0.1.3"
 description = "http plugins for nornir"
 authors = ["ubaumann <github@m.ubaumann.ch>"]
 license = "Apache-2.0"
 keywords = ["nornir", "http", "nornir-plugin"]
 readme = "README.md"
 repository = "https://github.com/InfrastructureAsCode-ch/nornir_http"
 homepage = "https://github.com/InfrastructureAsCode-ch/nornir_http"
 
 [tool.poetry.dependencies]
 python = "^3.8"
-httpx = "^0.23.0"
+httpx = "^0.24"
 nornir = "^3"
 
 [tool.poetry.dev-dependencies]
-pytest = "^6.2"
+pytest = "^7"
 black = "*"
-mypy = "^0.981"
-pytest-httpx = "^0.21.0"
+mypy = "^1"
+pytest-httpx = "^0.22.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nornir_http-0.1.2/PKG-INFO` & `nornir_http-0.1.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 Metadata-Version: 2.1
 Name: nornir-http
-Version: 0.1.2
+Version: 0.1.3
 Summary: http plugins for nornir
 Home-page: https://github.com/InfrastructureAsCode-ch/nornir_http
 License: Apache-2.0
 Keywords: nornir,http,nornir-plugin
 Author: ubaumann
 Author-email: github@m.ubaumann.ch
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: httpx (>=0.24,<0.25)
 Requires-Dist: nornir (>=3,<4)
 Project-URL: Repository, https://github.com/InfrastructureAsCode-ch/nornir_http
 Description-Content-Type: text/markdown
 
 # nornir_http
 
-Collection of simple plugins for [nornir](github.com/nornir-automation/nornir/)
+Simple HTTP Task plugins for [nornir](https://github.com/nornir-automation/nornir/)
 
 
 ## Install
 
 ```bash
 pip install nornir_http
 ```
```


# Comparing `tmp/pyprotogen-0.0.5.tar.gz` & `tmp/pyprotogen-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprotogen-0.0.5.tar", max compression
+gzip compressed data, was "pyprotogen-0.0.6.tar", max compression
```

## Comparing `pyprotogen-0.0.5.tar` & `pyprotogen-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
--rw-r--r--   0        0        0     1063 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/LICENSE
--rw-r--r--   0        0        0     1378 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/README.md
--rw-r--r--   0        0        0      868 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/pyprotogen/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/pyprotogen/dependencies/__init__.py
--rw-r--r--   0        0        0     1039 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/pyprotogen/dependencies/client.py
--rw-r--r--   0        0        0        0 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/pyprotogen/dependencies/interceptors/__init__.py
--rw-r--r--   0        0        0     1796 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/pyprotogen/dependencies/interceptors/client_logging.py
--rw-r--r--   0        0        0      212 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/pyprotogen/dependencies/interceptors/dto.py
--rw-r--r--   0        0        0      506 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/pyprotogen/dependencies/interceptors/utils.py
--rw-r--r--   0        0        0      393 2023-03-29 12:18:59.755266 pyprotogen-0.0.5/pyprotogen/dependencies/server.py
--rw-r--r--   0        0        0      956 2023-03-29 12:18:59.759266 pyprotogen-0.0.5/pyprotogen/main.py
--rw-r--r--   0        0        0     2031 2023-03-29 12:18:59.759266 pyprotogen-0.0.5/pyprotogen/packager.py
--rw-r--r--   0        0        0     1531 2023-03-29 12:18:59.759266 pyprotogen-0.0.5/pyprotogen/renderer.py
--rw-r--r--   0        0        0      224 2023-03-29 12:18:59.759266 pyprotogen-0.0.5/pyprotogen/settings.py
--rw-r--r--   0        0        0       33 2023-03-29 12:18:59.759266 pyprotogen-0.0.5/pyprotogen/templates/init-py.j2
--rw-r--r--   0        0        0      348 2023-03-29 12:18:59.759266 pyprotogen-0.0.5/pyprotogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 pyprotogen-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 12:54:40.870321 pyprotogen-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1378 2023-05-29 12:54:40.870321 pyprotogen-0.0.6/README.md
+-rw-r--r--   0        0        0      868 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/__init__.py
+-rw-r--r--   0        0        0     1286 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/__init__.py
+-rw-r--r--   0        0        0     1796 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/client_logging.py
+-rw-r--r--   0        0        0      212 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/dto.py
+-rw-r--r--   0        0        0      779 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/metadata.py
+-rw-r--r--   0        0        0      506 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/utils.py
+-rw-r--r--   0        0        0      393 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/server.py
+-rw-r--r--   0        0        0      956 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/main.py
+-rw-r--r--   0        0        0     2031 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/packager.py
+-rw-r--r--   0        0        0     1535 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/renderer.py
+-rw-r--r--   0        0        0      224 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/settings.py
+-rw-r--r--   0        0        0       33 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/templates/init-py.j2
+-rw-r--r--   0        0        0      348 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/templates/pyproject-toml.j2
+-rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 pyprotogen-0.0.6/PKG-INFO
```

### Comparing `pyprotogen-0.0.5/LICENSE` & `pyprotogen-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.5/README.md` & `pyprotogen-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.5/pyproject.toml` & `pyprotogen-0.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprotogen"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 repository = "https://github.com/sollof/pyprotogen"
 authors = ["Sergio Soldatov <soldatovsr97@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyprotogen-0.0.5/pyprotogen/dependencies/client.py` & `pyprotogen-0.0.6/pyprotogen/dependencies/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 from grpc.aio import insecure_channel, secure_channel, Channel
 from grpc import ssl_channel_credentials
 from grpc_prometheus_metrics.aio.prometheus_aio_client_interceptor import PromAioClientInterceptor
-from .interceptors.client_logging import LoggingClientInterceptor
+
+from interceptors.client_logging import LoggingClientInterceptor
+from interceptors.metadata import MetadataClientInterceptor
 
 
 def get_channel(
-    host: str, cert: str | None = None, enable_metrics: bool = True, enable_logging: bool = True,
+    host: str,
+    client_name: str | None = None,
+    cert: str | None = None,
+    enable_metrics: bool = True,
+    enable_logging: bool = True
 ) -> Channel:
     interceptors = []
     if enable_logging:
         prom = PromAioClientInterceptor(
             enable_client_handling_time_histogram=True,
             enable_client_stream_receive_time_histogram=True,
             enable_client_stream_send_time_histogram=True,
         )
         interceptors.append(prom)
     if enable_metrics:
         log = LoggingClientInterceptor()
         interceptors.append(log)
+    if client_name is not None:
+        metadata = MetadataClientInterceptor(client_name=client_name)
+        interceptors.append(metadata)
     if cert:
         creds = ssl_channel_credentials(cert.encode())
         ch = secure_channel(host, credentials=creds, interceptors=interceptors)
     else:
         ch = insecure_channel(host, interceptors=interceptors)
     return ch
```

### Comparing `pyprotogen-0.0.5/pyprotogen/dependencies/interceptors/client_logging.py` & `pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/client_logging.py`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.5/pyprotogen/main.py` & `pyprotogen-0.0.6/pyprotogen/main.py`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.5/pyprotogen/packager.py` & `pyprotogen-0.0.6/pyprotogen/packager.py`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.5/pyprotogen/renderer.py` & `pyprotogen-0.0.6/pyprotogen/renderer.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,15 +35,15 @@
         f'--grpc_python_out={grpc_gen_path}',
         *proto_files,
     ]
     proto_include = resources.path('grpc_tools', '_proto')
     include = ['-I{}'.format(proto_include)]
     protoc.main(args + include)
 
-    for file in grpc_gen_path.iterdir():
+    for file in grpc_gen_path.rglob('*.py'):
         with open(file, "r") as sources:
             lines = sources.readlines()
         with open(file, "w") as sources:
             for line in lines:
                 if re.search(r'^import .*_pb2 as', line) is not None:
                     line = 'from . ' + line
                 sources.write(line)
```

### Comparing `pyprotogen-0.0.5/PKG-INFO` & `pyprotogen-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprotogen
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Home-page: https://github.com/sollof/pyprotogen
 Author: Sergio Soldatov
 Author-email: soldatovsr97@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


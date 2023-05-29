# Comparing `tmp/pyprotogen-0.0.8.tar.gz` & `tmp/pyprotogen-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprotogen-0.0.8.tar", max compression
+gzip compressed data, was "pyprotogen-0.0.9.tar", max compression
```

## Comparing `pyprotogen-0.0.8.tar` & `pyprotogen-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1063 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/LICENSE
--rw-r--r--   0        0        0     1378 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/README.md
--rw-r--r--   0        0        0      868 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/dependencies/__init__.py
--rw-r--r--   0        0        0     1286 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/dependencies/client.py
--rw-r--r--   0        0        0        0 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/dependencies/interceptors/__init__.py
--rw-r--r--   0        0        0     1796 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/dependencies/interceptors/client_logging.py
--rw-r--r--   0        0        0      212 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/dependencies/interceptors/dto.py
--rw-r--r--   0        0        0      779 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/dependencies/interceptors/metadata.py
--rw-r--r--   0        0        0      506 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/dependencies/interceptors/utils.py
--rw-r--r--   0        0        0      393 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/dependencies/server.py
--rw-r--r--   0        0        0      956 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/main.py
--rw-r--r--   0        0        0     2031 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/packager.py
--rw-r--r--   0        0        0     1936 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/renderer.py
--rw-r--r--   0        0        0      224 2023-05-29 15:26:45.731573 pyprotogen-0.0.8/pyprotogen/settings.py
--rw-r--r--   0        0        0       33 2023-05-29 15:26:45.735573 pyprotogen-0.0.8/pyprotogen/templates/init-py.j2
--rw-r--r--   0        0        0      348 2023-05-29 15:26:45.735573 pyprotogen-0.0.8/pyprotogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 pyprotogen-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1378 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/README.md
+-rw-r--r--   0        0        0      868 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/dependencies/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/dependencies/interceptors/__init__.py
+-rw-r--r--   0        0        0     1796 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/dependencies/interceptors/client_logging.py
+-rw-r--r--   0        0        0      212 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/dependencies/interceptors/dto.py
+-rw-r--r--   0        0        0      779 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/dependencies/interceptors/metadata.py
+-rw-r--r--   0        0        0      506 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/dependencies/interceptors/utils.py
+-rw-r--r--   0        0        0      393 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/dependencies/server.py
+-rw-r--r--   0        0        0     1067 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/main.py
+-rw-r--r--   0        0        0     2080 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/packager.py
+-rw-r--r--   0        0        0     2451 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/renderer.py
+-rw-r--r--   0        0        0      224 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/settings.py
+-rw-r--r--   0        0        0     1324 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/templates/client-py.j2
+-rw-r--r--   0        0        0       33 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/templates/init-py.j2
+-rw-r--r--   0        0        0      348 2023-05-29 16:57:46.154245 pyprotogen-0.0.9/pyprotogen/templates/pyproject-toml.j2
+-rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 pyprotogen-0.0.9/PKG-INFO
```

### Comparing `pyprotogen-0.0.8/LICENSE` & `pyprotogen-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.8/README.md` & `pyprotogen-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.8/pyproject.toml` & `pyprotogen-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprotogen"
-version = "0.0.8"
+version = "0.0.9"
 description = ""
 repository = "https://github.com/sollof/pyprotogen"
 authors = ["Sergio Soldatov <soldatovsr97@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyprotogen-0.0.8/pyprotogen/dependencies/client.py` & `pyprotogen-0.0.9/pyprotogen/templates/client-py.j2`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from grpc.aio import insecure_channel, secure_channel, Channel
 from grpc import ssl_channel_credentials
 from grpc_prometheus_metrics.aio.prometheus_aio_client_interceptor import PromAioClientInterceptor
 
-from interceptors.client_logging import LoggingClientInterceptor
-from interceptors.metadata import MetadataClientInterceptor
+from {{ package_name }}.interceptors.client_logging import LoggingClientInterceptor
+from {{ package_name }}.interceptors.metadata import MetadataClientInterceptor
 
 
 def get_channel(
     host: str,
     client_name: str | None = None,
     cert: str | None = None,
     enable_metrics: bool = True,
```

### Comparing `pyprotogen-0.0.8/pyprotogen/dependencies/interceptors/client_logging.py` & `pyprotogen-0.0.9/pyprotogen/dependencies/interceptors/client_logging.py`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.8/pyprotogen/dependencies/interceptors/metadata.py` & `pyprotogen-0.0.9/pyprotogen/dependencies/interceptors/metadata.py`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.8/pyprotogen/main.py` & `pyprotogen-0.0.9/pyprotogen/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,25 +13,27 @@
 def main(
     input: str = typer.Argument(..., help="input .proto file"),
     output: str = typer.Argument(..., help="client output file path"),
     name: str = typer.Option("Client", help="client class name"),
     package_version: Optional[str] = typer.Option(None, help="package version"),
     package_authors: Optional[str] = typer.Option(None, help="package authors"),
 ):
+    package_name = ''
     if package_version:
         resp = packager.init_package(
             output_path=output,
             client_class_name=name,
             package_version=package_version,
             package_authors=package_authors,
         )
         output = resp.client_output_path
+        package_name = resp.package_name
 
     renderer.gen_pb2_files(input, output)
-
+    renderer.create_client(output, package_name)
     renderer.copy_dependencies(output)
 
 
 def run() -> None:
     typer.run(main)
```

### Comparing `pyprotogen-0.0.8/pyprotogen/packager.py` & `pyprotogen-0.0.9/pyprotogen/packager.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from jinja2 import Environment
 from jinja2 import FileSystemLoader
 from pyprotogen import settings
 
 
 @dataclass
 class InitPackageResponse:
+    package_name: str
     client_output_path: str
 
 
 def init_package(
     *,
     output_path: str,
     client_class_name: str,
@@ -25,15 +26,15 @@
     pyproject_path.mkdir(parents=True, exist_ok=True)
     _create_pyproject_file(pyproject_path, package_name, package_version, package_authors)
 
     sources_path = pyproject_path.joinpath(package_name)
     sources_path.mkdir(parents=True, exist_ok=True)
     _create_init_file(sources_path, package_name)
 
-    return InitPackageResponse(client_output_path=str(sources_path))
+    return InitPackageResponse(client_output_path=str(sources_path), package_name=package_name)
 
 
 def _create_pyproject_file(
     output_dir: Path, package_name: str, version: str, authors: Optional[str] = None
 ) -> None:
     env = Environment(
         loader=FileSystemLoader(settings.TEMPLATES_DIR_PATH),
```

### Comparing `pyprotogen-0.0.8/pyprotogen/renderer.py` & `pyprotogen-0.0.9/pyprotogen/renderer.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,17 +2,35 @@
 import re
 import shutil
 
 from importlib import resources
 from pathlib import Path
 
 from grpc_tools import protoc
+from jinja2 import Environment, FileSystemLoader
+
 from pyprotogen import settings
 
 
+def create_client(
+    output_path: str, package_name: str
+) -> None:
+    output_dir = Path(output_path)
+    env = Environment(
+        loader=FileSystemLoader(settings.TEMPLATES_DIR_PATH),
+        extensions=['jinja2.ext.loopcontrols'],
+    )
+    template = env.get_template('client-py.j2')
+
+    client_path = output_dir.joinpath('client.py')
+
+    with open(client_path, 'w') as client_file:
+        client_file.write(template.render(package_name=package_name))
+
+
 def copy_dependencies(output_path: str) -> None:
     shutil.copytree(
         settings.DEPENDENCIES_DIR_PATH, Path(output_path).absolute(), dirs_exist_ok=True
     )
 
 
 def gen_pb2_files(proto_path: str, output_path: str) -> None:
```

### Comparing `pyprotogen-0.0.8/PKG-INFO` & `pyprotogen-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprotogen
-Version: 0.0.8
+Version: 0.0.9
 Summary: 
 Home-page: https://github.com/sollof/pyprotogen
 Author: Sergio Soldatov
 Author-email: soldatovsr97@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


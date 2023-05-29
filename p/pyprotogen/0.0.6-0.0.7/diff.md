# Comparing `tmp/pyprotogen-0.0.6.tar.gz` & `tmp/pyprotogen-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprotogen-0.0.6.tar", max compression
+gzip compressed data, was "pyprotogen-0.0.7.tar", max compression
```

## Comparing `pyprotogen-0.0.6.tar` & `pyprotogen-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1063 2023-05-29 12:54:40.870321 pyprotogen-0.0.6/LICENSE
--rw-r--r--   0        0        0     1378 2023-05-29 12:54:40.870321 pyprotogen-0.0.6/README.md
--rw-r--r--   0        0        0      868 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/__init__.py
--rw-r--r--   0        0        0     1286 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/client.py
--rw-r--r--   0        0        0        0 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/__init__.py
--rw-r--r--   0        0        0     1796 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/client_logging.py
--rw-r--r--   0        0        0      212 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/dto.py
--rw-r--r--   0        0        0      779 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/metadata.py
--rw-r--r--   0        0        0      506 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/utils.py
--rw-r--r--   0        0        0      393 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/dependencies/server.py
--rw-r--r--   0        0        0      956 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/main.py
--rw-r--r--   0        0        0     2031 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/packager.py
--rw-r--r--   0        0        0     1535 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/renderer.py
--rw-r--r--   0        0        0      224 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/settings.py
--rw-r--r--   0        0        0       33 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/templates/init-py.j2
--rw-r--r--   0        0        0      348 2023-05-29 12:54:40.874321 pyprotogen-0.0.6/pyprotogen/templates/pyproject-toml.j2
--rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 pyprotogen-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 15:18:19.579951 pyprotogen-0.0.7/LICENSE
+-rw-r--r--   0        0        0     1378 2023-05-29 15:18:19.579951 pyprotogen-0.0.7/README.md
+-rw-r--r--   0        0        0      868 2023-05-29 15:18:19.579951 pyprotogen-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:19.579951 pyprotogen-0.0.7/pyprotogen/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:19.579951 pyprotogen-0.0.7/pyprotogen/dependencies/__init__.py
+-rw-r--r--   0        0        0     1286 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/dependencies/client.py
+-rw-r--r--   0        0        0        0 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/dependencies/interceptors/__init__.py
+-rw-r--r--   0        0        0     1796 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/dependencies/interceptors/client_logging.py
+-rw-r--r--   0        0        0      212 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/dependencies/interceptors/dto.py
+-rw-r--r--   0        0        0      779 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/dependencies/interceptors/metadata.py
+-rw-r--r--   0        0        0      506 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/dependencies/interceptors/utils.py
+-rw-r--r--   0        0        0      393 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/dependencies/server.py
+-rw-r--r--   0        0        0      956 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/main.py
+-rw-r--r--   0        0        0     2031 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/packager.py
+-rw-r--r--   0        0        0     1891 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/renderer.py
+-rw-r--r--   0        0        0      224 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/settings.py
+-rw-r--r--   0        0        0       33 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/templates/init-py.j2
+-rw-r--r--   0        0        0      348 2023-05-29 15:18:19.583951 pyprotogen-0.0.7/pyprotogen/templates/pyproject-toml.j2
+-rw-r--r--   0        0        0     2208 1970-01-01 00:00:00.000000 pyprotogen-0.0.7/PKG-INFO
```

### Comparing `pyprotogen-0.0.6/LICENSE` & `pyprotogen-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.6/README.md` & `pyprotogen-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.6/pyproject.toml` & `pyprotogen-0.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyprotogen"
-version = "0.0.6"
+version = "0.0.7"
 description = ""
 repository = "https://github.com/sollof/pyprotogen"
 authors = ["Sergio Soldatov <soldatovsr97@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `pyprotogen-0.0.6/pyprotogen/dependencies/client.py` & `pyprotogen-0.0.7/pyprotogen/dependencies/client.py`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/client_logging.py` & `pyprotogen-0.0.7/pyprotogen/dependencies/interceptors/client_logging.py`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.6/pyprotogen/dependencies/interceptors/metadata.py` & `pyprotogen-0.0.7/pyprotogen/dependencies/interceptors/metadata.py`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.6/pyprotogen/main.py` & `pyprotogen-0.0.7/pyprotogen/main.py`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.6/pyprotogen/packager.py` & `pyprotogen-0.0.7/pyprotogen/packager.py`

 * *Files identical despite different names*

### Comparing `pyprotogen-0.0.6/pyprotogen/renderer.py` & `pyprotogen-0.0.7/pyprotogen/renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
 import re
+import shutil
+
 from importlib import resources
 from pathlib import Path
 
 from grpc_tools import protoc
 from pyprotogen import settings
-import shutil
 
 
 def copy_dependencies(output_path: str) -> None:
     shutil.copytree(
         settings.DEPENDENCIES_DIR_PATH, Path(output_path).absolute(), dirs_exist_ok=True
     )
 
@@ -36,14 +38,21 @@
         *proto_files,
     ]
     proto_include = resources.path('grpc_tools', '_proto')
     include = ['-I{}'.format(proto_include)]
     protoc.main(args + include)
 
     for file in grpc_gen_path.rglob('*.py'):
+        name, extension = os.path.splitext(file.name)
+        if '.' in name:
+            new_name = f'{name.replace(".", "/")}{extension}'
+            os.rename(file, f'{file.parent}/{new_name}')
+
         with open(file, "r") as sources:
             lines = sources.readlines()
         with open(file, "w") as sources:
             for line in lines:
                 if re.search(r'^import .*_pb2 as', line) is not None:
                     line = 'from . ' + line
+                if re.search(r'^from .* import .*_pb2 as', line) is not None:
+                    line = 'from . import' + line.split('import')[1]
                 sources.write(line)
```

### Comparing `pyprotogen-0.0.6/PKG-INFO` & `pyprotogen-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprotogen
-Version: 0.0.6
+Version: 0.0.7
 Summary: 
 Home-page: https://github.com/sollof/pyprotogen
 Author: Sergio Soldatov
 Author-email: soldatovsr97@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```


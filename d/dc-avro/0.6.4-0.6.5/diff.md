# Comparing `tmp/dc_avro-0.6.4.tar.gz` & `tmp/dc_avro-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dc_avro-0.6.4.tar", max compression
+gzip compressed data, was "dc_avro-0.6.5.tar", max compression
```

## Comparing `dc_avro-0.6.4.tar` & `dc_avro-0.6.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1081 2023-03-22 16:01:53.219397 dc_avro-0.6.4/LICENSE
--rw-r--r--   0        0        0     2209 2023-03-22 16:01:53.219397 dc_avro-0.6.4/README.md
--rw-r--r--   0        0        0       35 2023-03-22 16:01:53.219397 dc_avro-0.6.4/dc_avro/__init__.py
--rw-r--r--   0        0        0     1232 2023-03-22 16:01:53.219397 dc_avro-0.6.4/dc_avro/_schema_utils.py
--rw-r--r--   0        0        0      193 2023-03-22 16:01:53.219397 dc_avro-0.6.4/dc_avro/_types.py
--rw-r--r--   0        0        0       81 2023-03-22 16:01:53.219397 dc_avro-0.6.4/dc_avro/exceptions.py
--rw-r--r--   0        0        0     4138 2023-03-22 16:01:53.219397 dc_avro-0.6.4/dc_avro/main.py
--rw-r--r--   0        0        0     2139 2023-03-22 16:01:53.219397 dc_avro-0.6.4/pyproject.toml
--rw-r--r--   0        0        0     3592 1970-01-01 00:00:00.000000 dc_avro-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-29 11:39:01.439021 dc_avro-0.6.5/LICENSE
+-rw-r--r--   0        0        0     2209 2023-05-29 11:39:01.439021 dc_avro-0.6.5/README.md
+-rw-r--r--   0        0        0       35 2023-05-29 11:39:01.439021 dc_avro-0.6.5/dc_avro/__init__.py
+-rw-r--r--   0        0        0     1232 2023-05-29 11:39:01.439021 dc_avro-0.6.5/dc_avro/_schema_utils.py
+-rw-r--r--   0        0        0      193 2023-05-29 11:39:01.439021 dc_avro-0.6.5/dc_avro/_types.py
+-rw-r--r--   0        0        0       81 2023-05-29 11:39:01.439021 dc_avro-0.6.5/dc_avro/exceptions.py
+-rw-r--r--   0        0        0     4154 2023-05-29 11:39:01.439021 dc_avro-0.6.5/dc_avro/main.py
+-rw-r--r--   0        0        0     2118 2023-05-29 11:39:01.439021 dc_avro-0.6.5/pyproject.toml
+-rw-r--r--   0        0        0     3290 1970-01-01 00:00:00.000000 dc_avro-0.6.5/PKG-INFO
```

### Comparing `dc_avro-0.6.4/LICENSE` & `dc_avro-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dc_avro-0.6.4/README.md` & `dc_avro-0.6.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 # Dataclasses Avro Schema CLI
 
 Command line interface from [dataclasses-avroschema](https://github.com/marcosschroh/dataclasses-avroschema) to work with `avsc` resources
 
 [![Tests](https://github.com/marcosschroh/dc-avro/actions/workflows/tests.yaml/badge.svg)](https://github.com/marcosschroh/dc-avro/actions/workflows/tests.yaml)
 [![GitHub license](https://img.shields.io/github/license/marcosschroh/dc-avro.svg)](https://github.com/marcosschroh/dc-avro/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/marcosschroh/dc-avro/branch/master/graph/badge.svg)](https://codecov.io/gh/marcosschroh/dc-avro)
-![python version](https://img.shields.io/badge/python-3.7%2B-yellowgreen)
+![python version](https://img.shields.io/badge/python-3.8%2B-yellowgreen)
 
 ## Requirements
 
-`python 3.7+`
+`python 3.8+`
 
 ## Documentation
 
 https://marcosschroh.github.io/dc-avro/
 
 ## Usage
```

### Comparing `dc_avro-0.6.4/dc_avro/_schema_utils.py` & `dc_avro-0.6.5/dc_avro/_schema_utils.py`

 * *Files identical despite different names*

### Comparing `dc_avro-0.6.4/dc_avro/main.py` & `dc_avro-0.6.5/dc_avro/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         SerializationType.AVRO,
     ),
 ):
     resource = get_resource(path=path, url=url)
     _schema_utils.validate(schema=resource)
 
     output = serialization.serialize(
-        data, resource, serialization_type=serialization_type
+        data, resource, serialization_type=serialization_type  # type: ignore
     )
     console.print(output)
 
 
 @app.command()
 def deserialize(
     event: str,
```

### Comparing `dc_avro-0.6.4/pyproject.toml` & `dc_avro-0.6.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.poetry]
 name = "dc-avro"
-version = "0.6.4"
+version = "0.6.5"
 description = ""
 authors = ["Marcos Schroh <marcos.schroh@kpn.com>"]
 readme = "README.md"
 packages = [{include = "dc_avro"}]
 license = "MIT"
 keywords = ["avro", "avro schemas", "dataclasses", "dataclasses-avroschema", "pydantic"]
 classifiers = [
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Application Frameworks",
     "Topic :: System :: Networking",
     "Topic :: System :: Distributed Computing",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 aiofiles = "^22.1.0" # remove this
 httpx = "^0.23.3"
 dataclasses-avroschema = "^0"
 typer = {extras = ["all"], version = "^0.7.0"}
 deepdiff = "^6.2.3"
 
 [tool.poetry.group.dev.dependencies]
@@ -33,14 +32,15 @@
 ruff = "^0.0.238"
 black = "^22.12.0"
 mypy = "^0.991"
 mkdocs = "^1.4.2"
 pytest = "^7.2.0"
 pytest-cov = "^4.0.0"
 mkdocs-material = "^9.0.6"
+types-attrs = "^19.1.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 dc-avro = "dc_avro.main:app"
@@ -75,15 +75,15 @@
     ".venv",
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
 [tool.commitizen]
-version = "0.6.4"
+version = "0.6.5"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:version",
 ]
 update_changelog_on_bump = true
 major_version_zero = true
```

### Comparing `dc_avro-0.6.4/PKG-INFO` & `dc_avro-0.6.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,23 @@
 Metadata-Version: 2.1
 Name: dc-avro
-Version: 0.6.4
+Version: 0.6.5
 Summary: 
 License: MIT
 Keywords: avro,avro schemas,dataclasses,dataclasses-avroschema,pydantic
 Author: Marcos Schroh
 Author-email: marcos.schroh@kpn.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: System :: Distributed Computing
 Classifier: Topic :: System :: Networking
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0)
 Requires-Dist: dataclasses-avroschema (>=0,<1)
 Requires-Dist: deepdiff (>=6.2.3,<7.0.0)
@@ -34,19 +28,19 @@
 # Dataclasses Avro Schema CLI
 
 Command line interface from [dataclasses-avroschema](https://github.com/marcosschroh/dataclasses-avroschema) to work with `avsc` resources
 
 [![Tests](https://github.com/marcosschroh/dc-avro/actions/workflows/tests.yaml/badge.svg)](https://github.com/marcosschroh/dc-avro/actions/workflows/tests.yaml)
 [![GitHub license](https://img.shields.io/github/license/marcosschroh/dc-avro.svg)](https://github.com/marcosschroh/dc-avro/blob/master/LICENSE)
 [![codecov](https://codecov.io/gh/marcosschroh/dc-avro/branch/master/graph/badge.svg)](https://codecov.io/gh/marcosschroh/dc-avro)
-![python version](https://img.shields.io/badge/python-3.7%2B-yellowgreen)
+![python version](https://img.shields.io/badge/python-3.8%2B-yellowgreen)
 
 ## Requirements
 
-`python 3.7+`
+`python 3.8+`
 
 ## Documentation
 
 https://marcosschroh.github.io/dc-avro/
 
 ## Usage
```


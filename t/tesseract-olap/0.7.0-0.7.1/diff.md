# Comparing `tmp/tesseract_olap-0.7.0.tar.gz` & `tmp/tesseract_olap-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tesseract_olap-0.7.0.tar", max compression
+gzip compressed data, was "tesseract_olap-0.7.1.tar", max compression
```

## Comparing `tesseract_olap-0.7.0.tar` & `tesseract_olap-0.7.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
--rw-r--r--   0        0        0     2221 2023-05-19 01:51:12.794118 tesseract_olap-0.7.0/PACKAGE.md
--rw-r--r--   0        0        0      862 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/__init__.py
--rw-r--r--   0        0        0       92 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/__init__.py
--rw-r--r--   0        0        0       79 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/__init__.py
--rw-r--r--   0        0        0     5868 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/backend.py
--rw-r--r--   0        0        0     1762 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/dialect.py
--rw-r--r--   0        0        0     1221 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/enums.py
--rw-r--r--   0        0        0    19408 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/sqlbuild.py
--rw-r--r--   0        0        0     1734 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/exceptions.py
--rw-r--r--   0        0        0     3248 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/backend/models.py
--rw-r--r--   0        0        0      243 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/common/__init__.py
--rw-r--r--   0        0        0      219 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/common/exceptions.py
--rw-r--r--   0        0        0     1570 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/common/strings.py
--rw-r--r--   0        0        0      385 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/common/types.py
--rw-r--r--   0        0        0      380 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/exceptions.py
--rw-r--r--   0        0        0      511 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/logiclayer/__init__.py
--rw-r--r--   0        0        0     6665 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/logiclayer/dependencies.py
--rw-r--r--   0        0        0     5677 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/logiclayer/module.py
--rw-r--r--   0        0        0     1198 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/logiclayer/response.py
--rw-r--r--   0        0        0     1129 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/__init__.py
--rw-r--r--   0        0        0     2262 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/calculations.py
--rw-r--r--   0        0        0     2848 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/enums.py
--rw-r--r--   0        0        0     3104 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/exceptions.py
--rw-r--r--   0        0        0    10377 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/models.py
--rw-r--r--   0        0        0    11603 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/queries.py
--rw-r--r--   0        0        0     7990 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/requests.py
--rw-r--r--   0        0        0     1539 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/query/results.py
--rw-r--r--   0        0        0     1145 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/__init__.py
--rw-r--r--   0        0        0     5400 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/aggregators.py
--rw-r--r--   0        0        0     3391 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/csv.py
--rw-r--r--   0        0        0     2908 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/enums.py
--rw-r--r--   0        0        0     3323 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/exceptions.py
--rw-r--r--   0        0        0     2500 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/json.py
--rw-r--r--   0        0        0     8559 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/models.py
--rw-r--r--   0        0        0     4645 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/schema.xsd
--rw-r--r--   0        0        0    23574 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/traverse.py
--rw-r--r--   0        0        0    18440 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/schema/xml.py
--rw-r--r--   0        0        0       64 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/server/__init__.py
--rw-r--r--   0        0        0      898 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/server/exceptions.py
--rw-r--r--   0        0        0     4269 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/server/schema.py
--rw-r--r--   0        0        0     4260 2023-05-19 01:51:12.798118 tesseract_olap-0.7.0/tesseract_olap/server/server.py
--rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 tesseract_olap-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     2221 2023-05-29 21:46:22.858263 tesseract_olap-0.7.1/PACKAGE.md
+-rw-r--r--   0        0        0      862 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/__init__.py
+-rw-r--r--   0        0        0       92 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/__init__.py
+-rw-r--r--   0        0        0       79 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/__init__.py
+-rw-r--r--   0        0        0     5868 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/backend.py
+-rw-r--r--   0        0        0     1894 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/dialect.py
+-rw-r--r--   0        0        0     1221 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/enums.py
+-rw-r--r--   0        0        0    19408 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/sqlbuild.py
+-rw-r--r--   0        0        0     1734 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/exceptions.py
+-rw-r--r--   0        0        0     3248 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/backend/models.py
+-rw-r--r--   0        0        0      243 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/common/__init__.py
+-rw-r--r--   0        0        0      219 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/common/exceptions.py
+-rw-r--r--   0        0        0     1570 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/common/strings.py
+-rw-r--r--   0        0        0      385 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/common/types.py
+-rw-r--r--   0        0        0      380 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/exceptions.py
+-rw-r--r--   0        0        0      511 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/logiclayer/__init__.py
+-rw-r--r--   0        0        0     6665 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/logiclayer/dependencies.py
+-rw-r--r--   0        0        0     5677 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/logiclayer/module.py
+-rw-r--r--   0        0        0     1198 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/logiclayer/response.py
+-rw-r--r--   0        0        0     1129 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/__init__.py
+-rw-r--r--   0        0        0     2262 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/calculations.py
+-rw-r--r--   0        0        0     2848 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/enums.py
+-rw-r--r--   0        0        0     3104 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/exceptions.py
+-rw-r--r--   0        0        0    10377 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/models.py
+-rw-r--r--   0        0        0    11603 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/queries.py
+-rw-r--r--   0        0        0     7990 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/requests.py
+-rw-r--r--   0        0        0     1539 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/query/results.py
+-rw-r--r--   0        0        0     1145 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/__init__.py
+-rw-r--r--   0        0        0     5400 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/aggregators.py
+-rw-r--r--   0        0        0     3533 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/csv.py
+-rw-r--r--   0        0        0     3649 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/enums.py
+-rw-r--r--   0        0        0     3323 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/exceptions.py
+-rw-r--r--   0        0        0     2497 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/json.py
+-rw-r--r--   0        0        0     8559 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/models.py
+-rw-r--r--   0        0        0     4645 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/schema.xsd
+-rw-r--r--   0        0        0    23574 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/traverse.py
+-rw-r--r--   0        0        0    18440 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/schema/xml.py
+-rw-r--r--   0        0        0       64 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/server/__init__.py
+-rw-r--r--   0        0        0      898 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/server/exceptions.py
+-rw-r--r--   0        0        0     4532 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/server/schema.py
+-rw-r--r--   0        0        0     4260 2023-05-29 21:46:22.862263 tesseract_olap-0.7.1/tesseract_olap/server/server.py
+-rw-r--r--   0        0        0     3260 1970-01-01 00:00:00.000000 tesseract_olap-0.7.1/PKG-INFO
```

### Comparing `tesseract_olap-0.7.0/PACKAGE.md` & `tesseract_olap-0.7.1/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/pyproject.toml` & `tesseract_olap-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tesseract-olap"
-version = "0.7.0"
+version = "0.7.1"
 description = "A simple OLAP library."
 authors = ["Francisco Abarzua <francisco@datawheel.us>"]
 license = "MIT"
 readme = "PACKAGE.md"
 repository = "https://github.com/Datawheel/tesseract-python"
 
 [tool.poetry.dependencies]
```

### Comparing `tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/backend.py` & `tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/backend.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/dialect.py` & `tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/dialect.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,14 +15,20 @@
     TIMESTAMP = "UInt32"
     FLOAT32 = "Float32"
     FLOAT64 = "Float64"
     INT8 = "Int8"
     INT16 = "Int16"
     INT32 = "Int32"
     INT64 = "Int64"
+    INT128 = "Int128"
+    UINT8 = "UInt8"
+    UINT16 = "UInt16"
+    UINT32 = "UInt32"
+    UINT64 = "UInt64"
+    UINT128 = "UInt128"
     STRING = "String"
 
     @classmethod
     def from_membertype(cls, mt: MemberType):
         """Transforms a MemberType enum value into a ClickhouseDataType."""
         return next((item for item in cls if item.name == mt.name), cls.STRING)
```

### Comparing `tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/enums.py` & `tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/backend/clickhouse/sqlbuild.py` & `tesseract_olap-0.7.1/tesseract_olap/backend/clickhouse/sqlbuild.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/backend/exceptions.py` & `tesseract_olap-0.7.1/tesseract_olap/backend/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/backend/models.py` & `tesseract_olap-0.7.1/tesseract_olap/backend/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/common/strings.py` & `tesseract_olap-0.7.1/tesseract_olap/common/strings.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/logiclayer/dependencies.py` & `tesseract_olap-0.7.1/tesseract_olap/logiclayer/dependencies.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/logiclayer/module.py` & `tesseract_olap-0.7.1/tesseract_olap/logiclayer/module.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/logiclayer/response.py` & `tesseract_olap-0.7.1/tesseract_olap/logiclayer/response.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/query/__init__.py` & `tesseract_olap-0.7.1/tesseract_olap/query/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/query/calculations.py` & `tesseract_olap-0.7.1/tesseract_olap/query/calculations.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/query/enums.py` & `tesseract_olap-0.7.1/tesseract_olap/query/enums.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/query/exceptions.py` & `tesseract_olap-0.7.1/tesseract_olap/query/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/query/models.py` & `tesseract_olap-0.7.1/tesseract_olap/query/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/query/queries.py` & `tesseract_olap-0.7.1/tesseract_olap/query/queries.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/query/requests.py` & `tesseract_olap-0.7.1/tesseract_olap/query/requests.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/query/results.py` & `tesseract_olap-0.7.1/tesseract_olap/query/results.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/schema/__init__.py` & `tesseract_olap-0.7.1/tesseract_olap/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/schema/aggregators.py` & `tesseract_olap-0.7.1/tesseract_olap/schema/aggregators.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/schema/csv.py` & `tesseract_olap-0.7.1/tesseract_olap/schema/csv.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,30 +93,33 @@
         kwargs["delimiter"] = DELIMITER_TRANSLATE.get(delimiter, delimiter)
 
     content = ColumnTypeInferrer(content, kwargs)
     table = tuple(csv.reader(content, **kwargs))
     return list(content.cast(table))
 
 
-def parse_csv_schema(source: Union[str, Path, TextIO], name: str = "") -> "CSVSchema":
+def parse_csv_schema(source: Union[str, Path, TextIO], table_name: str = "") -> "CSVSchema":
     if isinstance(source, Path):
-        name = source.name.replace(source.suffix, "")
+        table_name = source.name.replace(source.suffix, "")
         with source.open("r") as io:
             headers, *rows = parse_csv(line for line in io)
 
-    elif isinstance(source, TextIO):
-        name = source.name
+    elif isinstance(source, str):
+        headers, *rows = parse_csv(source.splitlines())
+
+    else: # isinstance(a, TextIO) has runtime issues
+        try:
+            table_name = source.name
+        except AttributeError:
+            pass
         headers, *rows = parse_csv(source.readlines())
         source.close()
 
-    else:
-        headers, *rows = parse_csv(source)
-
     table = CSVInlineTable(
-        name=name,
+        name=table_name,
         headers=tuple(str(item) for item in headers),
         types=CSVInlineTable.infer_types(rows),
         rows=rows,
     )
 
     return CSVSchema(
         name="",
```

### Comparing `tesseract_olap-0.7.0/tesseract_olap/schema/exceptions.py` & `tesseract_olap-0.7.1/tesseract_olap/schema/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/schema/json.py` & `tesseract_olap-0.7.1/tesseract_olap/schema/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,18 @@
     """
     contents: Union[str, bytes]
 
     # if argument is pathlib.Path, resolve its contents
     if isinstance(source, Path):
         contents = source.read_bytes()
 
+    # if argument is str, parse its contents directly
+    elif isinstance(source, str):
+        contents = source
+
     # if argument is a file-like, attempt to read it
-    elif isinstance(source, TextIO):
+    else:
         contents = source.read()
         source.close()
 
-    # if argument is str, parse its contents directly
-    else:
-        contents = source
-
     root = orjson.loads(contents)
     return JSONSchema.parse(root)
```

### Comparing `tesseract_olap-0.7.0/tesseract_olap/schema/models.py` & `tesseract_olap-0.7.1/tesseract_olap/schema/models.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/schema/schema.xsd` & `tesseract_olap-0.7.1/tesseract_olap/schema/schema.xsd`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/schema/traverse.py` & `tesseract_olap-0.7.1/tesseract_olap/schema/traverse.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/schema/xml.py` & `tesseract_olap-0.7.1/tesseract_olap/schema/xml.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/server/exceptions.py` & `tesseract_olap-0.7.1/tesseract_olap/server/exceptions.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/tesseract_olap/server/schema.py` & `tesseract_olap-0.7.1/tesseract_olap/server/schema.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+from itertools import chain
 from pathlib import Path
 from typing import TextIO, Union
 
 import httpx
 
 from tesseract_olap.schema import (Schema, parse_csv_schema, parse_json_schema,
                                    parse_xml_schema)
@@ -47,15 +48,15 @@
         elif source.is_file():
             return _parse_path_file(source)
 
         elif source.is_dir():
             logger.debug("Looking for schemas in local directory: %s", source)
             schemas = (
                 _parse_path_file(item)
-                for item in source.glob("**/*.xml,**/*.json")
+                for item in chain(source.glob("**/*.csv"), source.glob("**/*.xml"))
                 if item.is_file()
             )
             return Schema.join(*schemas)
 
     raise UnknownSchemaError(
         "Schema source can't be recognized as URL, file or raw string: %s" % source
     )
@@ -65,25 +66,32 @@
     """Attempts to fetch a remote URL and parse its contents as a Schema."""
     response = httpx.get(source)
     if response.is_error:
         raise FileNotFoundError(
             "Remote file %s does not exist: %d" % (source, response.status_code)
         )
 
+    path = response.url.path
+    ctype = response.headers["Content-Type"].lower()
     text = response.text.strip()
 
-    if source.endswith(".xml") or text.startswith(("<Schema ", "<?xml ")):
+    if path.endswith(".xml") \
+    or ctype == "text/xml" \
+    or text.startswith(("<Schema ", "<?xml ")):
         logger.debug("Parsing XML schema from URL: %s", source)
         return parse_xml_schema(text)
 
-    if source.endswith(".json") or text.startswith(("{\"", "[{")):
+    if path.endswith(".json") \
+    or ctype == "application/json" \
+    or text.startswith(("{\"", "[{")):
         logger.debug("Parsing JSON schema from URL: %s", source)
         return parse_json_schema(text)
 
-    if source.endswith(".csv"):
+    if path.endswith(".csv") \
+    or ctype in ("text/csv", "application/vnd.ms-excel"):
         logger.debug("Parsing CSV table from URL: %s", source)
         return parse_csv_schema(text)
 
     raise UnknownSchemaError("Linked source couldn't be parsed: %s" % source)
 
 
 def _parse_source_raw_string(source: str) -> Union["Schema", None]:
```

### Comparing `tesseract_olap-0.7.0/tesseract_olap/server/server.py` & `tesseract_olap-0.7.1/tesseract_olap/server/server.py`

 * *Files identical despite different names*

### Comparing `tesseract_olap-0.7.0/PKG-INFO` & `tesseract_olap-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tesseract-olap
-Version: 0.7.0
+Version: 0.7.1
 Summary: A simple OLAP library.
 Home-page: https://github.com/Datawheel/tesseract-python
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


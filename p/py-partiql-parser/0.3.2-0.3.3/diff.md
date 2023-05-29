# Comparing `tmp/py-partiql-parser-0.3.2.tar.gz` & `tmp/py-partiql-parser-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-partiql-parser-0.3.2.tar", last modified: Sun May 28 11:34:21 2023, max compression
+gzip compressed data, was "py-partiql-parser-0.3.3.tar", last modified: Mon May 29 20:32:37 2023, max compression
```

## Comparing `py-partiql-parser-0.3.2.tar` & `py-partiql-parser-0.3.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:34:21.741792 py-partiql-parser-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-28 11:34:21.741792 py-partiql-parser-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:34:21.737792 py-partiql-parser-0.3.2/py_partiql_parser/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:34:21.737792 py-partiql-parser-0.3.2/py_partiql_parser/_internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/case_insensitive_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/clause_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8487 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/py_partiql_parser/_internal/where_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:34:21.737792 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-28 11:34:21.000000 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-28 11:34:21.000000 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:34:21.000000 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-28 11:34:21.000000 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-28 11:34:21.000000 py-partiql-parser-0.3.2/py_partiql_parser.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-28 11:34:14.000000 py-partiql-parser-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-28 11:34:21.741792 py-partiql-parser-0.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:34:21.741792 py-partiql-parser-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_csv_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_dynamodb_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_from_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_json_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_query_metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_s3_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_select_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_select_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-28 11:33:57.000000 py-partiql-parser-0.3.2/tests/test_where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:37.674716 py-partiql-parser-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-29 20:32:37.674716 py-partiql-parser-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:37.670716 py-partiql-parser-0.3.3/py_partiql_parser/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:37.674716 py-partiql-parser-0.3.3/py_partiql_parser/_internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/case_insensitive_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/clause_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2965 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3332 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/py_partiql_parser/_internal/where_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:37.670716 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-05-29 20:32:37.000000 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-29 20:32:37.000000 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:32:37.000000 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-29 20:32:37.000000 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 20:32:37.000000 py-partiql-parser-0.3.3/py_partiql_parser.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-29 20:32:31.000000 py-partiql-parser-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 20:32:37.674716 py-partiql-parser-0.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:32:37.674716 py-partiql-parser-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_csv_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_dynamodb_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_from_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_json_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_query_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6494 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_s3_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_select_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_select_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-05-29 20:32:20.000000 py-partiql-parser-0.3.3/tests/test_where_parser.py
```

### Comparing `py-partiql-parser-0.3.2/LICENSE` & `py-partiql-parser-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/PKG-INFO` & `py-partiql-parser-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.3.2
+Version: 0.3.3
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `py-partiql-parser-0.3.2/README.md` & `py-partiql-parser-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/py_partiql_parser/_internal/case_insensitive_dict.py` & `py-partiql-parser-0.3.3/py_partiql_parser/_internal/case_insensitive_dict.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,19 @@
         if isinstance(other, Mapping):
             other = CaseInsensitiveDict(other)
         else:
             return NotImplemented
         # Compare insensitively
         return dict(self.lower_items()) == dict(other.lower_items())
 
-    def get_original(self, key):
+    def get_original(self, key, get_default=None):
+        if key.lower() not in self._store:
+            return get_default
         original_key, original_value = self._store[key.lower()]
-        return {original_key: original_value}
+        return CaseInsensitiveDict({original_key: original_value})
 
     # Copy is required
     def copy(self):
         return CaseInsensitiveDict(self._store.values())
 
     def __repr__(self):
         return str(dict(self.items()))
```

### Comparing `py-partiql-parser-0.3.2/py_partiql_parser/_internal/clause_tokenizer.py` & `py-partiql-parser-0.3.3/py_partiql_parser/_internal/clause_tokenizer.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/py_partiql_parser/_internal/csv_converter.py` & `py-partiql-parser-0.3.3/py_partiql_parser/_internal/csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/py_partiql_parser/_internal/from_parser.py` & `py-partiql-parser-0.3.3/py_partiql_parser/_internal/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,93 +1,96 @@
-from typing import Dict, Any
+from .case_insensitive_dict import CaseInsensitiveDict
+from .json_parser import MissingVariable, Variable
+from typing import Any, Dict, List, Tuple, Union
+
+
+def is_dict(dct):
+    return isinstance(dct, dict) or isinstance(dct, CaseInsensitiveDict)
+
+
+def find_nested_data(
+    select_clause: str, data_source: List[Dict[str, Any]]
+) -> List[Dict[str, Any]]:
+    """
+    Iterate over a list of JSON objects, and return only the keys specified
+    :param select_clause: Key of the data source, in dot-notation: a.b
+    :param data_source: List of JSON documents as dictionary
+    :return: A list of JSON keys as dictionary
+    """
+
+    results: List[Dict[str, Any]] = []
+
+    for row in data_source:
+        # Run the select-clause over each row
+        result = find_nested_data_in_object(select_clause=select_clause, json_doc=row)
+        results.append(result)
+    return results
+
+
+def find_nested_data_in_object(
+    select_clause: Union[None, str, Variable], json_doc: Any
+) -> Any:
+    if isinstance(select_clause, str):
+        if select_clause == "*":
+            return json_doc
+        select_clause = Variable(select_clause)
+    if isinstance(select_clause, Variable):
+        if not select_clause.value:
+            return json_doc
+        current_key = select_clause.value.split(".")[0]
+        remaining_keys = ".".join(select_clause.value.split(".")[1:])
+        if isinstance(json_doc, list):
+            result = []
+            for row in json_doc:
+                if current_key not in row:
+                    result.append(MissingVariable())
+                else:
+                    result.append(
+                        find_nested_data_in_object(
+                            row[current_key], Variable(remaining_keys)
+                        )
+                    )
+            return result
+        elif isinstance(json_doc, CaseInsensitiveDict):
+            if current_key not in json_doc:
+                return MissingVariable()
+            if remaining_keys:
+                return find_nested_data_in_object(
+                    json_doc[current_key], Variable(remaining_keys)
+                )
+            return json_doc.get_original(current_key)
+    if isinstance(select_clause, CaseInsensitiveDict):
+        result = [
+            {k: v.apply(row) for k, v in select_clause.items()} for row in json_doc
+        ]
+        return [
+            {k: v for k, v in row.items() if not isinstance(v, MissingVariable)}
+            for row in result
+        ]
+    if isinstance(select_clause, list):
+        return [
+            [find_nested_data_in_object(data_row, x) for x in select_clause]
+            for data_row in json_doc
+        ]
+    return []
+
+
+def find_value_in_document(keys: List[str], json_doc):
+    if not is_dict(json_doc):
+        return None
+    if len(keys) == 1:
+        return json_doc.get(keys[0])
+    return find_value_in_document(keys[1:], json_doc.get(keys[0], {}))
+
+
+class QueryMetadata:
+    def __init__(
+        self, tables: Dict[str, str], where_clauses: List[Tuple[List[str], str]] = None
+    ):
+        self._tables = tables
+        self._where_clauses = where_clauses or []
 
-from .clause_tokenizer import ClauseTokenizer
-from .json_parser import JsonParser
+    def get_table_names(self) -> List[str]:
+        return list(self._tables.values())
 
-
-class FromParser:
-    def __init__(self):
-        self.clauses = None
-
-    def parse(self, from_clause) -> Dict[str, str]:
-        """
-        Parse a FROM-clause in a PARTIQL query
-        :param from_clause: a string of format `a AS b, x AS y` where `a` and `x` can contain commas
-        :return: a dictionary of format `[b:a, y:x]`
-        """
-        clauses: Dict[str, Any] = dict()
-        section = None  # NAME/AS/ALIAS
-        current_phrase = ""
-        name = alias = None
-        from_clause_parser = ClauseTokenizer(from_clause)
-        while True:
-            c = from_clause_parser.next()
-            if c is None:
-                break
-            if c == "[":
-                if section is None:
-                    # Beginning of the FROM-clause - probably a document in its own right, instead of a name
-                    current_phrase = "[" + from_clause_parser.next_until(["]"]) + "]"
-                    section = "NAME"
-                    continue
-            if c == " ":
-                if section == "AS" and current_phrase.upper() == "AS":
-                    current_phrase = ""
-                    section = "ALIAS"
-                elif section == "NAME":
-                    name = current_phrase
-                    current_phrase = ""
-                    section = "AS"
-                elif section == "ALIAS":
-                    alias = current_phrase  # noqa
-                    current_phrase = ""
-                    section = "NAME"
-                continue
-            if c == ",":
-                if section == "NAME":
-                    clauses[current_phrase] = current_phrase
-                elif section == "ALIAS":
-                    clauses[current_phrase] = name
-                    section = "NAME"
-                current_phrase = ""
-                from_clause_parser.skip_white_space()
-                # new phrase
-                section = None
-                continue
-
-            if section is None:
-                section = "NAME"
-
-            current_phrase += c
-        if section == "NAME":
-            clauses[current_phrase] = current_phrase
-        else:
-            clauses[current_phrase] = name
-        #
-        # One FROM clause may point to the alias of another
-        # {'s': 'sensors', 'r': 's.readings'} --> {'s': 'sensors', 'r': 'sensors.readings'}
-        aliases = [(f"{key}.", f"{value}.") for key, value in clauses.items()]
-        for key, value in clauses.items():
-            for short, long in aliases:
-                if value.startswith(short):
-                    clauses[key] = value.replace(short, long)
-
-        # {alias: full_name_of_table_or_file}
-        self.clauses = clauses
-        return clauses
-
-    def get_source_data(self, documents: Dict[str, str]):
-        source_data = documents
-        for key in list(self.clauses.values())[0].lower().split("."):
-            if key in source_data:
-                source_data = JsonParser().parse(source_data[key])
-            elif key.endswith("[*]"):
-                if isinstance(source_data, dict):
-                    source_data = JsonParser().parse(source_data[key[0:-3]])
-                elif isinstance(source_data, list):
-                    new_source = []
-                    for row in source_data:
-                        if isinstance(row[key[0:-3]], list):
-                            new_source.extend(row[key[0:-3]])
-                    source_data = new_source
-
-        return source_data
+    def get_filter_names(self) -> List[str]:
+        return [".".join(keys) for keys, _ in self._where_clauses]
```

### Comparing `py-partiql-parser-0.3.2/py_partiql_parser/_internal/json_parser.py` & `py-partiql-parser-0.3.3/py_partiql_parser/_internal/json_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,14 +144,15 @@
                     # That means it's either a variable, or a number
                     if c.isnumeric():
                         section = "INT_VALUE"
                     else:
                         section = "VAR_VALUE"
                 if section in ["DICT_KEY", "DICT_VAL", "INT_VALUE", "VAR_VALUE"]:
                     current_phrase += c
+
         return result
 
     def _parse_list(self, original, tokenizer) -> Any:
         result: List[Union[Any, Dict]] = list()
         section = None
         current_phrase = ""
         while True:
```

### Comparing `py-partiql-parser-0.3.2/py_partiql_parser/_internal/parser.py` & `py-partiql-parser-0.3.3/py_partiql_parser/_internal/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,67 +1,79 @@
 import re
 
 from typing import Dict, Any, Union, List, AnyStr, Optional
 
-from .from_parser import FromParser
+from .from_parser import DynamoDBFromParser, S3FromParser, FromParser
 from .select_parser import SelectParser
 from .where_parser import DynamoDBWhereParser, S3WhereParser, WhereParser
 from .utils import is_dict, QueryMetadata
 
 
 class Parser:
     RETURN_TYPE = Union[Dict[AnyStr, Any], List]
 
     def __init__(
         self,
         source_data: Dict[str, str],
         table_prefix: Optional[str],
-        where_parser,
+        from_parser: FromParser,
+        where_parser: WhereParser,
     ):
         # Source data is in the format: {source: json}
         # Where 'json' is one or more json documents separated by a newline
         self.documents = source_data
         self.table_prefix = table_prefix
+        self.from_parser = from_parser
         self.where_parser = where_parser
 
     def parse(self, query: str, parameters=None) -> List[Dict[str, Any]]:
         query = query.replace("\n", " ")
         clauses = re.split("SELECT | FROM | WHERE ", query, flags=re.IGNORECASE)
         # First clause is whatever comes in front of SELECT - which should be nothing
         _ = clauses[0]
         # FROM
-        from_parser = FromParser()
+        from_parser = self.from_parser()
         from_clauses = from_parser.parse(clauses[2])
         source_data = from_parser.get_source_data(self.documents)
         if is_dict(source_data):
             source_data = [source_data]  # type: ignore
 
         # WHERE
         if len(clauses) > 3:
             where_clause = clauses[3]
             source_data = self.where_parser(source_data).parse(where_clause, parameters)
 
         # SELECT
         select_clause = clauses[1]
-        return SelectParser(self.table_prefix).parse(
+        table_prefix = self.table_prefix
+        for alias_key, alias_value in from_clauses.items():
+            if table_prefix == alias_value:
+                table_prefix = alias_key
+        return SelectParser(table_prefix).parse(
             select_clause, from_clauses, source_data
         )
 
 
 class S3SelectParser(Parser):
     def __init__(self, source_data: Dict[str, str]):
         super().__init__(
-            source_data, table_prefix="s3object", where_parser=S3WhereParser
+            source_data,
+            table_prefix="s3object",
+            from_parser=S3FromParser,
+            where_parser=S3WhereParser,
         )
 
 
 class DynamoDBStatementParser(Parser):
     def __init__(self, source_data: Dict[str, str]):
         super().__init__(
-            source_data, table_prefix=None, where_parser=DynamoDBWhereParser
+            source_data,
+            table_prefix=None,
+            from_parser=DynamoDBFromParser,
+            where_parser=DynamoDBWhereParser,
         )
 
     @classmethod
     def get_query_metadata(cls, query: str):
         query = query.replace("\n", " ")
         clauses = re.split("SELECT | FROM | WHERE ", query, flags=re.IGNORECASE)
```

### Comparing `py-partiql-parser-0.3.2/py_partiql_parser/_internal/select_parser.py` & `py-partiql-parser-0.3.3/py_partiql_parser/_internal/select_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 from typing import Dict, Any, List, Optional
 
 from .clause_tokenizer import ClauseTokenizer
-from .utils import find_nested_data_in_object, MissingVariable
+from .utils import find_nested_data_in_object, MissingVariable, is_dict
 
 
 class SelectClause:
     def __init__(self, value: str, table_prefix: Optional[str] = None):
         self.table_prefix = table_prefix
         self.value = value.strip()
 
-    def select(self, aliases: Dict[str, str], document: Dict[str, Any]):
+    def select(self, document: Dict[str, Any]):
         if self.value == "*":
-            if self.table_prefix:
+            if self.table_prefix and self.table_prefix in document:
                 return document[self.table_prefix]
             else:
                 return document
         if "." in self.value:
             key, remaining = self.value.split(".", maxsplit=1)
             return find_nested_data_in_object(
-                select_clause=remaining, json_doc=document[aliases.get(key, key)]
+                select_clause=remaining, json_doc=document[key]
             )
         elif not self.table_prefix:
             return find_nested_data_in_object(
                 select_clause=self.value, json_doc=document
             )
         else:
-            return document[aliases.get(self.value, self.value)]
+            if is_dict(document[self.value]):
+                return document[self.value]
+            else:
+                return {self.value: document[self.value]}
 
     def __repr__(self):
         return f"<SelectClause({self.value})>"
 
     def __eq__(self, other):
         return isinstance(other, SelectClause) and other.value == self.value
 
@@ -68,21 +71,28 @@
         for clause in clauses:
             if isinstance(clause, FunctionClause):
                 return [clause.execute(aliases, documents)]
 
         result: List[Dict[str, Any]] = []
 
         for json_document in documents:
-            if self.table_prefix is not None:
-                json_document = {self.table_prefix: json_document}
             filtered_document = dict()
             for clause in clauses:
-                attr = clause.select(aliases, json_document)
+                attr = clause.select(json_document)
                 if attr is not None and not isinstance(attr, MissingVariable):
-                    filtered_document.update(attr)
+                    # Specific usecase:
+                    # select * from s3object[*].Name my_n
+                    if (
+                        "." in list(aliases.values())[0]
+                        and list(aliases.keys())[0] in attr
+                        and select_clause == "*"
+                    ):
+                        filtered_document.update({"_1": attr[list(aliases.keys())[0]]})
+                    else:
+                        filtered_document.update(attr)
             result.append(filtered_document)
         return result
 
     @classmethod
     def parse_clauses(
         cls, select_clause: str, prefix: Optional[str] = None
     ) -> List[SelectClause]:
```

### Comparing `py-partiql-parser-0.3.2/py_partiql_parser/_internal/where_parser.py` & `py-partiql-parser-0.3.3/py_partiql_parser/_internal/where_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,14 +96,11 @@
         _filters = WhereParser.parse_where_clause(where_clause)
 
         return self.filter_rows(_filters)
 
     def filter_rows(self, _filters):
         def _filter(row):
             return all(
-                [
-                    find_value_in_document(keys[1:], row) == value
-                    for keys, value in _filters
-                ]
+                [find_value_in_document(keys, row) == value for keys, value in _filters]
             )
 
         return [row for row in self.source_data if _filter(row)]
```

### Comparing `py-partiql-parser-0.3.2/py_partiql_parser.egg-info/PKG-INFO` & `py-partiql-parser-0.3.3/py_partiql_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-partiql-parser
-Version: 0.3.2
+Version: 0.3.3
 Summary: Pure Python PartiQL Parser
 Author-email: Bert Blommers <info@bertblommers.nl>
 License: MIT
 Keywords: pypartiql,parser
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
```

### Comparing `py-partiql-parser-0.3.2/py_partiql_parser.egg-info/SOURCES.txt` & `py-partiql-parser-0.3.3/py_partiql_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/tests/test_csv_converter.py` & `py-partiql-parser-0.3.3/tests/test_csv_converter.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/tests/test_dynamodb_examples.py` & `py-partiql-parser-0.3.3/tests/test_dynamodb_examples.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/tests/test_from_parser.py` & `py-partiql-parser-0.3.3/tests/test_from_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/tests/test_json_parser.py` & `py-partiql-parser-0.3.3/tests/test_json_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/tests/test_query_metadata.py` & `py-partiql-parser-0.3.3/tests/test_query_metadata.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/tests/test_s3_examples.py` & `py-partiql-parser-0.3.3/tests/test_s3_examples.py`

 * *Files 12% similar despite different names*

```diff
@@ -161,15 +161,61 @@
     )
     parser = S3SelectParser(source_data={"s3object": all_rows})
     assert parser.parse(query, parameters=None) == [
         {"Name": "Vinod", "City": "Los Angeles"}
     ]
 
 
-def test_select_root_objects():
-    query = "select * from s3object[*].staff[*] s"
+def test_select_doc_using_asterisk():
+    query = "select * from s3object[*]"
+    result = S3SelectParser(source_data={"s3object": json_as_lines}).parse(query)
+    assert len(result) == 7
+    assert {
+        "Name": "Sam",
+        "PhoneNumber": "(949) 555-6701",
+        "City": "Irvine",
+        "Occuption": "Solutions Architect",
+    } in result
+
+
+@pytest.mark.parametrize(
+    "query",
+    [
+        "select my_n from s3object[*].Name my_n",
+        "select my_n from s3object[*].Name as my_n",
+    ],
+)
+def test_select_specific_object_doc_using_named_asterisk(query):
+    result = S3SelectParser(source_data={"s3object": json_as_lines}).parse(query)
+    assert len(result) == 7
+    assert {"my_n": "Sam"} in result
+    assert {"my_n": "Jeff"} in result
+
+
+@pytest.mark.parametrize(
+    "query",
+    ["select * from s3object[*].Name my_n", "select * from s3object[*].Name as my_n"],
+)
+def test_select_nested_object_using_named_asterisk(query):
+    result = S3SelectParser(source_data={"s3object": json_as_lines}).parse(query)
+    assert len(result) == 7
+    assert {"_1": "Sam"} in result
+    assert {"_1": "Jeff"} in result
+
+
+def test_select_list_using_asterisk():
+    query = "select * from s3object[*] s"
+    result = S3SelectParser(
+        source_data={"s3object": json.dumps(input_with_lists)}
+    ).parse(query)
+    assert result == [{"_1": input_with_lists}]
+
+
+@pytest.mark.parametrize(
+    "query",
+    ["select * from s3object[*].staff s", "select * from s3object[*].staff[*] s"],
+)
+def test_select_nested_list_using_asterisk(query):
     result = S3SelectParser(
         source_data={"s3object": json.dumps(input_with_lists)}
     ).parse(query)
-    assert len(result) == 2
-    assert input_with_lists[0]["staff"][0] in result
-    assert input_with_lists[0]["staff"][1] in result
+    assert result == [{}]
```

### Comparing `py-partiql-parser-0.3.2/tests/test_select_functions.py` & `py-partiql-parser-0.3.3/tests/test_select_functions.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/tests/test_select_parser.py` & `py-partiql-parser-0.3.3/tests/test_select_parser.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/tests/test_utils.py` & `py-partiql-parser-0.3.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `py-partiql-parser-0.3.2/tests/test_where_parser.py` & `py-partiql-parser-0.3.3/tests/test_where_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,36 +69,36 @@
         {"Name": "Jane", "city": "Chicago"},
         {"Name": "Sean", "city": "Chicago"},
         {"Name": "Mary", "city": "Chicago", "notes": {"extra": "y"}},
         {"Name": "Kate", "city": "Chicago", "notes": {"extra": "n"}},
     ]
 
     def test_simple(self):
-        filter_keys = ["s3object", "city"]
+        filter_keys = ["city"]
         filter_value = "Los Angeles"
         assert S3WhereParser(TestFilter.all_rows).filter_rows(
             _filters=[(filter_keys, filter_value)]
         ) == [{"Name": "Vinod", "city": "Los Angeles"}]
 
     def test_without_prefix(self):
         filter_keys = ["city"]
         filter_value = "Los Angeles"
         assert DynamoDBWhereParser(TestFilter.all_rows).filter_rows(
             _filters=[(filter_keys, filter_value)]
         ) == [{"Name": "Vinod", "city": "Los Angeles"}]
 
     def test_alias(self):
-        filter_keys = ["s", "city"]
+        filter_keys = ["city"]
         filter_value = "Los Angeles"
         assert S3WhereParser(TestFilter.all_rows).filter_rows(
             _filters=[(filter_keys, filter_value)]
         ) == [{"Name": "Vinod", "city": "Los Angeles"}]
 
     def test_alias_nested_key(self):
-        filter_keys = ["s3object", "notes", "extra"]
+        filter_keys = ["notes", "extra"]
         filter_value = "y"
         assert S3WhereParser(TestFilter.all_rows).filter_rows(
             _filters=[(filter_keys, filter_value)]
         ) == [{"Name": "Mary", "city": "Chicago", "notes": {"extra": "y"}}]
 
 
 class TestDynamoDBParse:
```


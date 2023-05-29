# Comparing `tmp/kolo-2.9.2.tar.gz` & `tmp/kolo-2.9.3.tar.gz`

## Comparing `kolo-2.9.2.tar` & `kolo-2.9.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 kolo-2.9.2/rust/Cargo.toml
--rw-rw-r--   0     1000     1001       54 2023-05-23 17:47:16.000000 kolo-2.9.2/rust/build.rs
--rw-rw-r--   0     1000     1001    35207 2023-05-23 17:47:16.000000 kolo-2.9.2/rust/src/lib.rs
--rw-rw-r--   0     1000     1001     2176 2023-05-23 17:47:16.000000 kolo-2.9.2/pyproject.toml
--rw-rw-r--   0     1000     1001    11199 2023-05-23 17:48:14.000000 kolo-2.9.2/rust/Cargo.lock
--rw-rw-r--   0     1000     1001     2677 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/django_schema.py
--rw-rw-r--   0     1000     1001     3798 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/serialize.py
--rw-rw-r--   0     1000     1001     3400 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/requests.py
--rw-rw-r--   0     1000     1001      348 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/kolo.py
--rw-rw-r--   0     1000     1001     1322 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/unittest.py
--rw-rw-r--   0     1000     1001     4448 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/exception.py
--rw-rw-r--   0     1000     1001     1457 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/pytest.py
--rw-rw-r--   0     1000     1001     4345 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/sql.py
--rw-rw-r--   0     1000     1001     2262 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/celery.py
--rw-rw-r--   0     1000     1001     3157 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/urllib.py
--rw-rw-r--   0     1000     1001     4141 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/django.py
--rw-rw-r--   0     1000     1001     1778 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/logging.py
--rw-rw-r--   0     1000     1001     5180 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/core.py
--rw-rw-r--   0     1000     1001      809 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/attrs.py
--rw-rw-r--   0     1000     1001     3707 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/urllib3.py
--rw-rw-r--   0     1000     1001      141 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/pypy.py
--rw-rw-r--   0     1000     1001        0 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/__init__.py
--rw-rw-r--   0     1000     1001     2921 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/filters/huey.py
--rw-rw-r--   0     1000     1001     2640 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/middleware.py
--rw-rw-r--   0     1000     1001     2118 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/templates/django_request_test.py.j2
--rw-rw-r--   0     1000     1001    13710 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/profiler.py
--rw-rw-r--   0     1000     1001      169 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/version.py
--rw-rw-r--   0     1000     1001    29613 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/generate_tests.py
--rw-rw-r--   0     1000     1001      360 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/utils.py
--rw-rw-r--   0     1000     1001    11763 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/__main__.py
--rw-rw-r--   0     1000     1001     5431 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/db.py
--rw-rw-r--   0     1000     1001      473 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/git.py
--rw-rw-r--   0     1000     1001      228 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/pytest_plugin.py
--rw-rw-r--   0     1000     1001      108 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/__init__.py
--rw-rw-r--   0     1000     1001     2881 2023-05-23 17:47:16.000000 kolo-2.9.2/src/kolo/config.py
--rw-rw-r--   0     1000     1001      228 2023-05-23 17:47:16.000000 kolo-2.9.2/README.md
--rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 kolo-2.9.2/PKG-INFO
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 kolo-2.9.3/rust/Cargo.toml
+-rw-rw-r--   0     1000     1001       54 2023-05-29 08:14:53.000000 kolo-2.9.3/rust/build.rs
+-rw-rw-r--   0     1000     1001    35207 2023-05-29 08:14:53.000000 kolo-2.9.3/rust/src/lib.rs
+-rw-rw-r--   0     1000     1001     2176 2023-05-29 08:14:53.000000 kolo-2.9.3/pyproject.toml
+-rw-rw-r--   0     1000     1001    11199 2023-05-29 08:15:59.000000 kolo-2.9.3/rust/Cargo.lock
+-rw-rw-r--   0     1000     1001     2677 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/django_schema.py
+-rw-rw-r--   0     1000     1001     3798 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/serialize.py
+-rw-rw-r--   0     1000     1001     3400 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/requests.py
+-rw-rw-r--   0     1000     1001      348 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/kolo.py
+-rw-rw-r--   0     1000     1001     1322 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/unittest.py
+-rw-rw-r--   0     1000     1001     4448 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/exception.py
+-rw-rw-r--   0     1000     1001     1457 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/pytest.py
+-rw-rw-r--   0     1000     1001     4345 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/sql.py
+-rw-rw-r--   0     1000     1001     2262 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/celery.py
+-rw-rw-r--   0     1000     1001     3157 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/urllib.py
+-rw-rw-r--   0     1000     1001     4141 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/django.py
+-rw-rw-r--   0     1000     1001     1778 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/logging.py
+-rw-rw-r--   0     1000     1001     5180 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/core.py
+-rw-rw-r--   0     1000     1001      809 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/attrs.py
+-rw-rw-r--   0     1000     1001     3707 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/urllib3.py
+-rw-rw-r--   0     1000     1001      141 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/pypy.py
+-rw-rw-r--   0     1000     1001        0 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/__init__.py
+-rw-rw-r--   0     1000     1001     2921 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/filters/huey.py
+-rw-rw-r--   0     1000     1001     2640 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/middleware.py
+-rw-rw-r--   0     1000     1001     1936 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/templates/django_request_test.py.j2
+-rw-rw-r--   0     1000     1001    13710 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/profiler.py
+-rw-rw-r--   0     1000     1001      169 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/version.py
+-rw-rw-r--   0     1000     1001    32582 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/generate_tests.py
+-rw-rw-r--   0     1000     1001      360 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/utils.py
+-rw-rw-r--   0     1000     1001    11995 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/__main__.py
+-rw-rw-r--   0     1000     1001     5542 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/db.py
+-rw-rw-r--   0     1000     1001      473 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/git.py
+-rw-rw-r--   0     1000     1001      228 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/pytest_plugin.py
+-rw-rw-r--   0     1000     1001      108 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/__init__.py
+-rw-rw-r--   0     1000     1001     2881 2023-05-29 08:14:53.000000 kolo-2.9.3/src/kolo/config.py
+-rw-rw-r--   0     1000     1001      228 2023-05-29 08:14:53.000000 kolo-2.9.3/README.md
+-rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 kolo-2.9.3/PKG-INFO
```

### Comparing `kolo-2.9.2/rust/src/lib.rs` & `kolo-2.9.3/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/pyproject.toml` & `kolo-2.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "kolo"
-version = "2.9.2"
+version = "2.9.3"
 description = "See everything happening in your running Django app"
 readme = "README.md"
 authors = [
     {name = "Wilhelm Klopp", email = "team@kolo.app"},
     {name = "Lily Foote", email = "lily@kolo.app"},
 ]
 urls.Homepage = "https://kolo.app"
```

### Comparing `kolo-2.9.2/rust/Cargo.lock` & `kolo-2.9.3/rust/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -147,17 +147,17 @@
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.58"
+version = "1.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa1fb82fc0c281dd9671101b66b771ebbe1eaf967b96ac8740dcba4b70005ca8"
+checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -216,17 +216,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.27"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "rand"
 version = "0.8.5"
@@ -332,17 +332,17 @@
 checksum = "13a3aaa69b04e5b66cc27309710a569ea23593612387d67daaf102e73aa974fd"
 dependencies = [
  "rand",
 ]
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5464a87b239f13a63a501f2701565754bae92d243d4bb7eb12f6d57d2269bf4"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unindent"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1766d682d402817b5ac4490b3c3002d91dfa0d22812f341609f97b08757359c"
```

### Comparing `kolo-2.9.2/src/kolo/django_schema.py` & `kolo-2.9.3/src/kolo/django_schema.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/serialize.py` & `kolo-2.9.3/src/kolo/serialize.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/requests.py` & `kolo-2.9.3/src/kolo/filters/requests.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/unittest.py` & `kolo-2.9.3/src/kolo/filters/unittest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/exception.py` & `kolo-2.9.3/src/kolo/filters/exception.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/pytest.py` & `kolo-2.9.3/src/kolo/filters/pytest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/sql.py` & `kolo-2.9.3/src/kolo/filters/sql.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/celery.py` & `kolo-2.9.3/src/kolo/filters/celery.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/urllib.py` & `kolo-2.9.3/src/kolo/filters/urllib.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/django.py` & `kolo-2.9.3/src/kolo/filters/django.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/logging.py` & `kolo-2.9.3/src/kolo/filters/logging.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/core.py` & `kolo-2.9.3/src/kolo/filters/core.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/attrs.py` & `kolo-2.9.3/src/kolo/filters/attrs.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/urllib3.py` & `kolo-2.9.3/src/kolo/filters/urllib3.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/filters/huey.py` & `kolo-2.9.3/src/kolo/filters/huey.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/middleware.py` & `kolo-2.9.3/src/kolo/middleware.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/profiler.py` & `kolo-2.9.3/src/kolo/profiler.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/src/kolo/generate_tests.py` & `kolo-2.9.3/src/kolo/generate_tests.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,22 +40,23 @@
 
 
 def maybe_black(rendered):
     try:
         from black import format_file_contents
         from black.mode import Mode
         from black.parsing import InvalidInput
+        from black.report import NothingChanged
     except ImportError:  # pragma: no cover
         return rendered
 
     try:
         return format_file_contents(
             rendered, fast=True, mode=Mode(magic_trailing_comma=False)
         )
-    except InvalidInput:  # pragma: no cover
+    except (InvalidInput, NothingChanged):  # pragma: no cover
         return rendered
 
 
 env = Environment(loader=KoloPackageLoader("kolo"))
 
 
 def _format_header(header: str) -> str:
@@ -68,35 +69,45 @@
 UUID_REPR_REGEX = re.compile(
     r"UUID\(\'([0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12})\'\)"
 )
 DECIMAL_REPR_REGEX = re.compile(r"Decimal\('(\d+.?\d+?)'\)")
 TIMEDELTA_REPR_REGEX = re.compile(
     r"datetime.timedelta\((?:days=(\d+),? ?)?(?:seconds=(\d+),? ?)?(?:microseconds=(\d+))?\)"
 )
+TIMEDELTA_STR_REGEX = re.compile(r"(\d+) days (\d+)\.(\d+) seconds")
 
 
 def parse_value(value, column_schema):
     if column_schema["django_field"] == "django.db.models.fields.UUIDField":
         uuid_match = UUID_REPR_REGEX.match(str(value))
         if uuid_match:
             value = uuid_match[1]
     elif column_schema["django_field"] == "django.db.models.fields.json.JSONField":
-        value = json.loads(value)
+        if value is not None:
+            value = json.loads(value)
     elif column_schema["django_field"] == "django.db.models.fields.DecimalField":
         decimal_match = DECIMAL_REPR_REGEX.match(str(value))
         if decimal_match:
             value = Decimal(decimal_match[1])
     elif column_schema["django_field"] == "django.db.models.fields.DurationField":
         if isinstance(value, str):
             timedelta_match = TIMEDELTA_REPR_REGEX.match(value)
+            duration_match = TIMEDELTA_STR_REGEX.match(value)
             if timedelta_match:  # pragma: no branch
                 groups = [int(g) if g else 0 for g in timedelta_match.groups()]
                 value = timedelta(
                     days=groups[0], seconds=groups[1], microseconds=groups[2]
                 )
+            elif duration_match:
+                groups = duration_match.groups()
+                value = timedelta(
+                    days=int(groups[0]),
+                    seconds=int(groups[1]),
+                    microseconds=int(groups[2]),
+                )
         else:
             value = timedelta(microseconds=value)
     return value
 
 
 class TooComplicatedError(Exception):
     pass
@@ -123,14 +134,16 @@
         field_schema = table_schema["fields"][identifier.name]
         if isinstance(value, sqlglot.expressions.Null):
             value = None
         elif isinstance(value, sqlglot.expressions.Boolean):
             value = value.this
         elif isinstance(value, sqlglot.expressions.Cast):
             value = value.name
+        elif isinstance(value, sqlglot.expressions.Anonymous):
+            value = value.name
         elif value.is_string:
             value = value.name
         else:
             value = literal_eval(value.name)
         value = parse_value(value, field_schema)
         return cls(identifier.name, value, field_schema)
 
@@ -152,47 +165,51 @@
         return cls(name, value, {})
 
     def __eq__(self, other):
         return (self.name, self.value) == (other.name, other.value)
 
     def __lt__(self, other) -> bool:
         if self.name == other.name:
+            if self.value is None:
+                return False
+            if other.value is None:
+                return True
             return self.value < other.value
         return self.name < other.name
 
     def __hash__(self):
         return hash((self.name, self.value))
 
     def __repr__(self):
         return f'DjangoField("{self.name}", {self.value})'
 
     def assert_equal_template(self, variable_name):
-        return f"self.assertEqual({variable_name}.{self.name}, {self.value})"
+        return f"self.assertEqual({variable_name}.{self.name}, {self.value_repr})"
 
 
 def find_pk(fields):
     for field in fields:
         if field.schema["primary_key"]:
             return field
     return None  # pragma: no cover
 
 
 class VariableNames:
     def __init__(self):
         self.counts: Counter = Counter()
         self.names = {}
 
-    def next_variable_name(self, verbose_name, field):
-        full_key = verbose_name, field.name, field.value_repr
+    def next_variable_name(self, verbose_name, field_name, field_repr):
+        full_key = verbose_name, field_name, field_repr
         try:
             return self.names[full_key]
         except KeyError:
             pass
 
-        key = verbose_name, field.name
+        key = verbose_name, field_name
         self.counts[key] += 1
         suffix = self.counts[key]
         if suffix == 1:
             name = verbose_name
         else:
             name = f"{verbose_name}_{suffix}"
         self.names[full_key] = name
@@ -231,15 +248,17 @@
     @classmethod
     def from_raw(cls, table, values, query, schema_data, names):
         module = schema_data[table]["model_module"]
         model = schema_data[table]["model_name"]
         values = tuple(values)
         primary_key = find_pk(values)
         verbose_name = schema_data[table]["verbose_name"]
-        variable_name = names.next_variable_name(verbose_name, primary_key)
+        variable_name = names.next_variable_name(
+            verbose_name, primary_key.name, primary_key.value_repr
+        )
         return cls(
             table,
             f"{module}.{model}",
             primary_key,
             values,
             variable_name,
             f"import {module}",
@@ -278,14 +297,16 @@
                     ]
                 except KeyError:
                     field.name = field.schema["field_attname"]
             fields.append(field)
         self.values = tuple(fields)
 
     def __eq__(self, other):
+        if not isinstance(other, DjangoCreate):
+            return NotImplemented
         return (self.table, self.model, self.values, self.variable_name) == (
             other.table,
             other.model,
             other.values,
             other.variable_name,
         )
 
@@ -304,15 +325,15 @@
             )"""
         )
 
     @property
     def template_parts(self):
         yield f"{self.variable_name}, _created = {self.model}.objects.get_or_create("
         for field in self.values:
-            yield f"{field.name}={field.value},"
+            yield f"{field.name}={field.value_repr},"
         defaults = {self.primary_key.name: self.primary_key.raw_value}
         yield f"defaults={defaults},"
         yield ")"
 
 
 class AssertSelect:
     def __init__(self, model, fields, import_path=None, query=None):
@@ -364,15 +385,15 @@
             )"""
         )
 
     @property
     def template_parts(self):
         yield f"self.assertTrue({self.model}.objects.filter("
         for field in self.fields:
-            yield f"{field.name}={field.value},"
+            yield f"{field.name}={field.value_repr},"
         yield ").exists())"
 
 
 class AssertInsert:
     def __init__(self, variable_name, model, fields, import_path=None, query=None):
         self.variable_name = variable_name
         self.model = model
@@ -381,15 +402,17 @@
         self.import_path = import_path
 
     @classmethod
     def from_raw(cls, fields, query, table_schema, names, primary_key):
         module = table_schema["model_module"]
         model = table_schema["model_name"]
         verbose_name = table_schema["verbose_name"]
-        variable_name = names.next_variable_name(verbose_name, primary_key)
+        variable_name = names.next_variable_name(
+            verbose_name, primary_key.name, primary_key.value_repr
+        )
         return cls(
             variable_name, f"{module}.{model}", fields, f"import {module}", query
         )
 
     def update_fields(self, names, schema):
         fields = []
         for field in self.fields:
@@ -432,15 +455,15 @@
             )"""
         )
 
     @property
     def template_parts(self):
         yield f"{self.variable_name} = {self.model}.objects.get("
         for field in self.fields:
-            yield f"{field.name}={field.value},"
+            yield f"{field.name}={field.value_repr},"
         yield ")"
 
 
 class AssertUpdate:
     def __init__(self, variable_name, fields, query=None):
         self.variable_name = variable_name
         self.fields = fields
@@ -496,15 +519,17 @@
         related_tables = tables[table]
 
         if len(related_tables) == 0:
             return 0
         return max(table_depth(related) for related in related_tables) + 1
 
     def sort_key(create):
-        return (table_depth(create.table), create.table, create.values)
+        if isinstance(create, DjangoCreate):
+            return (table_depth(create.table), create.table, create.values)
+        return (table_depth(create.table), create.table)
 
     return sort_key
 
 
 def parse_columns(columns, row, schema_data):
     columns_by_table: Dict[str, List[DjangoField]] = {}
     for column, value in zip(columns, row):
@@ -548,25 +573,25 @@
     names = VariableNames()
     # each select needs to become an insert
     inserts = []
     imports = set()
     asserts = []
     seen_mutations: Dict[str, Set[str]] = {}
     for query in sql_queries:
-        if query["query_data"] is None:
+        if query["query_data"] is None or query["query"] is None:
             continue
 
         database = query["database"]
         database = DATABASES.get(database, database)
         try:
             parsed_query = sqlglot.parse_one(query["query"], read=database)
         except sqlglot.errors.ParseError as e:  # pragma: no cover
-            print("Error parsing query:")
-            print(query["query"])
-            print(e.errors)
+            print("# Error parsing query:")
+            print(f'# {query["query"]}')
+            print(f"# {e.errors}")
             continue
 
         if isinstance(parsed_query, sqlglot.exp.Select):
             columns = [column for (_key, column) in parsed_query.iter_expressions()]
             for batch in query["query_data"]:
                 # Skip queries with no columns, eg .count(), .exists()
                 if not any(
@@ -574,15 +599,17 @@
                 ):
                     continue
                 for row in batch:
                     columns_by_table = parse_columns(columns, row, schema_data)
 
                     for table, row in columns_by_table.items():
                         pk = find_pk(row)
-                        if pk.value_repr in seen_mutations.setdefault(table, set()):
+                        if pk is None:
+                            inserts.append(DjangoQuery(table, query))
+                        elif pk.value_repr in seen_mutations.setdefault(table, set()):
                             asserts.append(
                                 AssertSelect.from_raw(row, query, schema_data[table])
                             )
                         else:
                             create = DjangoCreate.from_raw(
                                 table, row, query, schema_data, names
                             )
@@ -598,24 +625,37 @@
             if isinstance(parsed_query, sqlglot.expressions.Update):
                 where = parsed_query.find(sqlglot.expressions.Where)
                 if where is None:
                     continue  # pragma: no cover
 
                 fields = build_update_assert_fields(columns, table_schema["fields"])
 
-                lookup_name = where.this.left.name
-                lookup_value = where.this.right.name
+                if isinstance(where.this, sqlglot.expressions.In):
+                    lookups = []
+                    lookup_name = where.this.this.name
+                    for literal in where.this.expressions:
+                        lookups.append((lookup_name, literal.name))
+                elif isinstance(where.this, sqlglot.expressions.Paren):
+                    asserts.append(DjangoQuery(table_name, query))
+                else:
+                    lookup_name = where.this.left.name
+                    lookup_value = where.this.right.name
+                    lookups = [(lookup_name, lookup_value)]
+
                 verbose_name = table_schema["verbose_name"]
-                variable_name = names.names[(verbose_name, lookup_name, lookup_value)]
-                assert_update = AssertUpdate(variable_name, fields, query)
-                asserts.append(assert_update)
-                if table_schema["fields"][lookup_name][  # pragma: no branch
-                    "primary_key"
-                ]:
-                    seen_mutations.setdefault(table_name, set()).add(lookup_value)
+                for lookup_name, lookup_value in lookups:
+                    variable_name = names.next_variable_name(
+                        verbose_name, lookup_name, lookup_value
+                    )
+                    assert_update = AssertUpdate(variable_name, fields, query)
+                    asserts.append(assert_update)
+                    if table_schema["fields"][lookup_name][  # pragma: no branch
+                        "primary_key"
+                    ]:
+                        seen_mutations.setdefault(table_name, set()).add(lookup_value)
             elif isinstance(  # pragma: no branch
                 parsed_query, sqlglot.expressions.Insert
             ):
                 sql_schema = parsed_query.find(sqlglot.expressions.Schema)
                 sql_values_tuple = parsed_query.find(sqlglot.expressions.Tuple)
                 if sql_schema is None or sql_values_tuple is None:
                     continue  # pragma: no cover
@@ -650,47 +690,73 @@
                 )
                 asserts.append(assert_insert)
                 imports.add(assert_insert.import_path)
 
     deduplicated = unique_everseen(inserts)
     sql_fixtures = sorted(deduplicated, key=make_table_sort_key(schema_data))
     for create in sql_fixtures:
-        create.update_fields(names, schema_data)
+        if isinstance(create, DjangoCreate):
+            create.update_fields(names, schema_data)
     for assert_ in asserts:
         if isinstance(assert_, (AssertInsert, AssertSelect)):
             assert_.update_fields(names, schema_data)
     return sql_fixtures, imports, asserts
 
 
 def get_request_headers(request):
+    if not request:
+        return {}
     request_headers = {
         _format_header(header): value for header, value in request["headers"].items()
     }
     if "HTTP_COOKIE" in request_headers and request_headers["HTTP_COOKIE"] == "":
         del request_headers["HTTP_COOKIE"]
-    if "CONTENT_LENGTH" in request_headers:
-        del request_headers["CONTENT_LENGTH"]
-    if "HTTP_HOST" in request_headers:
-        del request_headers["HTTP_HOST"]
-    if "HTTP_X_FORWARDED_FOR" in request_headers:
-        del request_headers["HTTP_X_FORWARDED_FOR"]
-    if "HTTP_X_FORWARDED_PROTO" in request_headers:
-        del request_headers["HTTP_X_FORWARDED_PROTO"]
+
+    request_headers_to_delete = [
+        "CONTENT_LENGTH",
+        "HTTP_HOST",
+        "HTTP_X_FORWARDED_FOR",
+        "HTTP_X_FORWARDED_PROTO",
+        "HTTP_CONNECTION",
+        "HTTP_CACHE_CONTROL",
+        "HTTP_DNT",
+        "HTTP_SEC_CH_UA",
+        "HTTP_USER_AGENT",
+        "HTTP_ACCEPT",
+        "HTTP_SEC_FETCH_DEST",
+        "HTTP_SEC_CH_UA_MOBILE",
+        "HTTP_REFERER",
+        "HTTP_ACCEPT_ENCODING",
+        "HTTP_ACCEPT_LANGUAGE",
+        "HTTP_SEC_FETCH_SITE",
+        "HTTP_SEC_FETCH_MODE",
+        "HTTP_SEC_FETCH_USER",
+        "HTTP_SEC_FETCH_DEST",
+        "HTTP_SEC_CH_UA_PLATFORM",
+        "HTTP_ORIGIN",
+        "HTTP_UPGRADE_INSECURE_REQUESTS"
+    ]
+
+    for request_header in request_headers_to_delete:
+        if request_header in request_headers:
+            del request_headers[request_header]
 
     if "CONTENT_TYPE" in request_headers:
         # This is a special header, which ends up influencing
         # how the django test client formats different parts of the
         # request. It's provided to the test client as a lowercased
         # argument
         request_headers["content_type"] = request_headers["CONTENT_TYPE"]
         del request_headers["CONTENT_TYPE"]
     return request_headers
 
 
 def get_request_body(request, request_headers):
+    if not request:
+        return ""
     request_body = request["body"]
     content_type = request_headers.get("content_type", "")
     if content_type == "application/x-www-form-urlencoded":
         # So: How can we now format the body so that it becomes more readable
         # We can totally cater to just this urlencoded version first...
 
         # TODO: Eventually need to be able to support multivaluedicts / query params
@@ -701,18 +767,20 @@
         return f"urlencode({urldecoded_body})"
     elif "multipart/form-data" in content_type:
         request_headers.pop("content_type")
         if request["method"] == "POST":
             return str(request["post_data"])
         return ""
     else:
-        return f'"{request_body}"'
+        return repr(request_body)
 
 
 def get_query_params(request):
+    if not request:
+        return ""
     query_params = request["query_params"]
     if query_params:
         return f"{query_params},"
     return ""
 
 
 def generate_from_trace_id(trace_id: str, test_class: str, test_name: str) -> str:
@@ -748,14 +816,16 @@
             assert current_outbound_request is None
             current_outbound_request = {"request": frame}
         elif frame["type"] == "outbound_http_response":
             if frame["subtype"] == "urllib3":
                 continue
             assert current_outbound_request is not None
             current_outbound_request["response"] = frame
+            if current_outbound_request["response"]["body"] and current_outbound_request["response"]["headers"].get("Content-Type") == "application/json":
+                current_outbound_request["response"]["json_body"] = json.loads(current_outbound_request["response"]["body"])
             outbound_request_frames.append(current_outbound_request)
 
             current_outbound_request = None
         elif frame["type"] == "end_sql_query":
             sql_queries.append(frame)
 
     if sql_queries:
@@ -782,42 +852,48 @@
 
     # This will be useful in the extension too to figure out
     # what were the rows that were created. What were the updates
     # that were actually made.
 
     # And then in the tests, we can make assertions around certain updates having happened
 
-    request = served_request_frames[0]["request"]
-    response = served_request_frames[0]["response"]
+    request = served_request_frames[0]["request"] if served_request_frames else None
+    response = served_request_frames[0]["response"] if served_request_frames else None
     request_headers = get_request_headers(request)
     prettified_request_body = get_request_body(request, request_headers)
     query_params = get_query_params(request)
-    request_timestamp = datetime.utcfromtimestamp(request["timestamp"]).isoformat(
-        timespec="seconds"
-    )
+    if request:
+        request_timestamp = datetime.utcfromtimestamp(request["timestamp"]).isoformat(
+            timespec="seconds"
+        )
+    else:
+        request_timestamp = ""
 
     try:
         from django import __version__ as django_version
     except ImportError:  # pragma: no cover
         django_version = ""
 
     template = env.get_template("django_request_test.py.j2")
+    template_names = (
+        served_request_frames[0]["templates"] if served_request_frames else []
+    )
     rendered = template.render(
         asserts=asserts,
         django_version=django_version,
         imports=sorted(imports),
         kolo_version=kolo_version,
         now=datetime.utcnow(),
         outbound_request_frames=outbound_request_frames,
         prettified_request_body=prettified_request_body,
         query_params=query_params,
         request=request,
         request_headers=request_headers,
         request_timestamp=request_timestamp,
         response=response,
         sql_fixtures=sql_fixtures,
-        template_names=served_request_frames[0]["templates"],
+        template_names=template_names,
         test_class=test_class,
         test_name=test_name,
         trace_id=trace_id,
     )
     return maybe_black(rendered)
```

### Comparing `kolo-2.9.2/src/kolo/__main__.py` & `kolo-2.9.3/src/kolo/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import click
 
 from . import django_schema
 from .config import load_config
 from .db import (
     SchemaNotFoundError,
+    TraceNotFoundError,
     create_schema_table,
     db_cursor,
     delete_traces_before,
     delete_traces_by_id,
     list_traces_from_db,
     load_trace_from_db,
     save_invocation_in_sqlite,
@@ -35,14 +36,31 @@
         "%Y-%m-%d %H:%M:%S",
         "%Y-%m-%dT%H:%M:%S.%f",
         "%Y-%m-%d %H:%M:%S.%f",
     )
 )
 
 
+DJANGO_SETTINGS_ERROR = """Django settings not found.
+Use `--settings` or set the `DJANGO_SETTINGS_MODULE` environment variable."""
+
+SCHEMA_NOT_FOUND_ERROR = """\
+Could not find a Django schema for commit: {}.
+
+Run `kolo store-django-model-schema` from that commit then retry this command."""
+
+TRACE_NOT_FOUND_ERROR = "Could not find trace_id: `{trace_id}`"
+
+TEST_GENERATION_ERROR = """\
+Test generation dependencies are not installed.
+
+Run `pip install kolo[test_generation]` to install them.
+"""
+
+
 def get_profiler(one_trace_per_test) -> KoloProfiler:
     config = load_config()
     db_path = setup_db(config)
     return KoloProfiler(db_path, config=config, one_trace_per_test=one_trace_per_test)
 
 
 def profile_module(profiler: KoloProfiler, module_name: str):
@@ -212,16 +230,16 @@
 def dump_trace_base(trace_id, file):
     config = load_config()
     wal_mode = config.get("wal_mode", True)
     db_path = setup_db(config)
 
     try:
         data = load_trace_from_db(db_path, trace_id, wal_mode=wal_mode)
-    except TypeError:
-        raise click.ClickException(f"Could not find trace_id: `{trace_id}`")
+    except TraceNotFoundError:
+        raise click.ClickException(TRACE_NOT_FOUND_ERROR.format(trace_id=trace_id))
 
     if file:
         with open(file, "w") as f:
             f.write(data)
     else:
         click.echo(data)
 
@@ -334,27 +352,14 @@
 
     if trace_ids and old:
         raise click.ClickException("Cannot specify TRACE_IDS and --old together")
 
     delete_traces_base(trace_ids, old, before, vacuum)
 
 
-TEST_GENERATION_ERROR = """\
-Test generation dependencies are not installed.
-
-Run `pip install kolo[test_generation]` to install them.
-"""
-
-
-SCHEMA_NOT_FOUND_ERROR = """\
-Could not find a Django schema for commit: {}.
-
-Run `kolo store-django-model-schema` from that commit then retry this command."""
-
-
 def manage_py_settings():
     import ast
 
     try:
         with open("manage.py") as f:
             data = f.read()
     except OSError:  # pragma: no cover
@@ -410,27 +415,25 @@
 
         load_django(settings)
 
         try:
             test_code = generate_from_trace_id(trace_id, test_class, test_name)
         except SchemaNotFoundError as e:
             raise click.ClickException(SCHEMA_NOT_FOUND_ERROR.format(e.args[0]))
+        except TraceNotFoundError as e:
+            raise click.ClickException(TRACE_NOT_FOUND_ERROR.format(trace_id=e.args[0]))
 
         if file:
             file.write(test_code)
         else:
             click.echo(test_code)
     finally:
         logging.disable(logging.NOTSET)
 
 
-DJANGO_SETTINGS_ERROR = """Django settings not found.
-Use `--settings` or set the `DJANGO_SETTINGS_MODULE` environment variable."""
-
-
 @cli.command()
 @click.option("--settings", default="")
 def store_django_model_schema(settings):
     from .git import COMMIT_SHA
 
     load_django(settings)
```

### Comparing `kolo-2.9.2/src/kolo/db.py` & `kolo-2.9.3/src/kolo/db.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from .config import create_kolo_directory
 
 
 class SchemaNotFoundError(Exception):
     pass
 
 
+class TraceNotFoundError(Exception):
+    pass
+
+
 @contextmanager
 def db_cursor(db_path, wal_mode=True):
     """
     Wrap sqlite's cursor for use as a context manager
 
     Commits all changes if no exception is raised.
     Always closes the cursor/connection after the context manager exits.
@@ -98,14 +102,16 @@
 
 def load_trace_from_db(db_path: Path, trace_id: str, wal_mode: bool = True) -> str:
     fetch_sql = "SELECT data FROM invocations WHERE id = ?"
 
     with db_cursor(db_path, wal_mode) as cursor:
         cursor.execute(fetch_sql, (trace_id,))
         row = cursor.fetchone()
+    if row is None:
+        raise TraceNotFoundError(trace_id)
     return row[0]
 
 
 def list_traces_from_db(db_path: Path, wal_mode: bool = True):
     list_sql = """
     SELECT id, created_at, LENGTH(CAST(data AS BLOB)) FROM invocations
     ORDER BY id DESC LIMIT 500
```

### Comparing `kolo-2.9.2/src/kolo/config.py` & `kolo-2.9.3/src/kolo/config.py`

 * *Files identical despite different names*

### Comparing `kolo-2.9.2/PKG-INFO` & `kolo-2.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolo
-Version: 2.9.2
+Version: 2.9.3
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```


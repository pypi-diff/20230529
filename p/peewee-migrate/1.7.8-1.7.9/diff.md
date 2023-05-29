# Comparing `tmp/peewee_migrate-1.7.8.tar.gz` & `tmp/peewee_migrate-1.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peewee_migrate-1.7.8.tar", max compression
+gzip compressed data, was "peewee_migrate-1.7.9.tar", max compression
```

## Comparing `peewee_migrate-1.7.8.tar` & `peewee_migrate-1.7.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     4456 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/README.rst
--rw-r--r--   0        0        0      146 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/__init__.py
--rw-r--r--   0        0        0       78 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/__main__.py
--rw-r--r--   0        0        0    11862 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/auto.py
--rw-r--r--   0        0        0     6597 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/cli.py
--rw-r--r--   0        0        0      146 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/logs.py
--rw-r--r--   0        0        0    16516 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/migrator.py
--rw-r--r--   0        0        0      461 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/models.py
--rw-r--r--   0        0        0        0 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/py.typed
--rw-r--r--   0        0        0    12235 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/router.py
--rw-r--r--   0        0        0     1701 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/template.py
--rw-r--r--   0        0        0      249 2023-05-22 21:38:45.433922 peewee_migrate-1.7.8/peewee_migrate/types.py
--rw-r--r--   0        0        0     1589 2023-05-22 21:38:45.437922 peewee_migrate-1.7.8/pyproject.toml
--rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.8/PKG-INFO
+-rw-r--r--   0        0        0     4456 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/README.rst
+-rw-r--r--   0        0        0      146 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/__init__.py
+-rw-r--r--   0        0        0       78 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/__main__.py
+-rw-r--r--   0        0        0    11862 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/auto.py
+-rw-r--r--   0        0        0     6597 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/cli.py
+-rw-r--r--   0        0        0      146 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/logs.py
+-rw-r--r--   0        0        0    17190 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/migrator.py
+-rw-r--r--   0        0        0      461 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/models.py
+-rw-r--r--   0        0        0        0 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/py.typed
+-rw-r--r--   0        0        0    12235 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/router.py
+-rw-r--r--   0        0        0     1802 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/template.py
+-rw-r--r--   0        0        0      249 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/peewee_migrate/types.py
+-rw-r--r--   0        0        0     1589 2023-05-22 22:05:32.906672 peewee_migrate-1.7.9/pyproject.toml
+-rw-r--r--   0        0        0     5440 1970-01-01 00:00:00.000000 peewee_migrate-1.7.9/PKG-INFO
```

### Comparing `peewee_migrate-1.7.8/README.rst` & `peewee_migrate-1.7.9/README.rst`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.8/peewee_migrate/auto.py` & `peewee_migrate-1.7.9/peewee_migrate/auto.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.8/peewee_migrate/cli.py` & `peewee_migrate-1.7.9/peewee_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.8/peewee_migrate/migrator.py` & `peewee_migrate-1.7.9/peewee_migrate/migrator.py`

 * *Files 8% similar despite different names*

```diff
@@ -462,7 +462,23 @@
         """Add default."""
         model = self.__get_model__(model)
         meta = model._meta  # type: ignore[]
         field = meta.fields[name]
         meta.defaults[field] = field.default = default
         self.__ops__.append(self.__migrator__.apply_default(meta.table_name, name, field))
         return model
+
+    def add_constraint(self, model: Union[str, TModelType], name, constraint):
+        """Add constraint."""
+        model = self.__get_model__(model)
+        meta = model._meta  # type: ignore[]
+        self.__ops__.append(self.__migrator__.add_constraint(meta.table_name, name, constraint))
+        return model
+
+    def drop_constraints(self, model: Union[str, TModelType], *names: str) -> TModelType:
+        """Drop constraints."""
+        model = self.__get_model__(model)
+        meta = model._meta  # type: ignore[]
+        self.__ops__.extend(
+            [self.__migrator__.drop_constraint(meta.table_name, name) for name in names]
+        )
+        return model
```

### Comparing `peewee_migrate-1.7.8/peewee_migrate/router.py` & `peewee_migrate-1.7.9/peewee_migrate/router.py`

 * *Files identical despite different names*

### Comparing `peewee_migrate-1.7.8/peewee_migrate/template.py` & `peewee_migrate-1.7.9/peewee_migrate/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,20 @@
     > migrator.remove_model(model, cascade=True)    # Remove a model
     > migrator.add_fields(model, **fields)          # Add fields to a model
     > migrator.change_fields(model, **fields)       # Change fields
     > migrator.remove_fields(model, *field_names, cascade=True)
     > migrator.rename_field(model, old_field_name, new_field_name)
     > migrator.rename_table(model, new_table_name)
     > migrator.add_index(model, *col_names, unique=False)
-    > migrator.drop_index(model, *col_names)
     > migrator.add_not_null(model, *field_names)
-    > migrator.drop_not_null(model, *field_names)
     > migrator.add_default(model, field_name, default)
+    > migrator.add_constraint(model, name, sql)
+    > migrator.drop_index(model, *col_names)
+    > migrator.drop_not_null(model, *field_names)
+    > migrator.drop_constraints(model, *constraints)
 
 \"\"\"
 
 from contextlib import suppress
 
 import peewee as pw
 from peewee_migrate import Migrator
```

### Comparing `peewee_migrate-1.7.8/pyproject.toml` & `peewee_migrate-1.7.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "peewee-migrate"
-version = "1.7.8"
+version = "1.7.9"
 homepage = "https://github.com/klen/peewee_migrate"
 repository = "https://github.com/klen/peewee_migrate"
 description = "Support for migrations in Peewee ORM"
 readme = "README.rst"
 authors = ["Kirill Klenov <horneds@gmail.com>"]
 license = "MIT"
 keywords = ["peewee", "migrations", "orm"]
```

### Comparing `peewee_migrate-1.7.8/PKG-INFO` & `peewee_migrate-1.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peewee-migrate
-Version: 1.7.8
+Version: 1.7.9
 Summary: Support for migrations in Peewee ORM
 Home-page: https://github.com/klen/peewee_migrate
 License: MIT
 Keywords: peewee,migrations,orm
 Author: Kirill Klenov
 Author-email: horneds@gmail.com
 Requires-Python: >=3.8,<4.0
```


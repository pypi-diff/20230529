# Comparing `tmp/ardilla-0.3.1b0.tar.gz` & `tmp/ardilla-0.3.2b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ardilla-0.3.1b0.tar", last modified: Sun May 28 13:49:38 2023, max compression
+gzip compressed data, was "ardilla-0.3.2b0.tar", last modified: Mon May 29 14:38:14 2023, max compression
```

## Comparing `ardilla-0.3.1b0.tar` & `ardilla-0.3.2b0.tar`

### file list

```diff
@@ -1,32 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 13:49:38.639693 ardilla-0.3.1b0/
--rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.3.1b0/LICENCE
--rw-rw-rw-   0        0        0     5203 2023-05-28 13:49:38.635694 ardilla-0.3.1b0/PKG-INFO
--rw-rw-rw-   0        0        0     4301 2023-05-28 05:57:28.000000 ardilla-0.3.1b0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 13:49:38.512148 ardilla-0.3.1b0/ardilla/
--rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.3.1b0/ardilla/__init__.py
--rw-rw-rw-   0        0        0     4877 2023-05-28 06:26:40.000000 ardilla-0.3.1b0/ardilla/abc.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:49:38.607691 ardilla-0.3.1b0/ardilla/asyncio/
--rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.3.1b0/ardilla/asyncio/__init__.py
--rw-rw-rw-   0        0        0     8730 2023-05-28 12:54:50.000000 ardilla-0.3.1b0/ardilla/asyncio/crud.py
--rw-rw-rw-   0        0        0     2074 2023-05-28 13:12:38.000000 ardilla-0.3.1b0/ardilla/asyncio/engine.py
--rw-rw-rw-   0        0        0     8762 2023-05-28 05:57:28.000000 ardilla-0.3.1b0/ardilla/crud.py
--rw-rw-rw-   0        0        0     2102 2023-05-28 06:30:14.000000 ardilla-0.3.1b0/ardilla/engine.py
--rw-rw-rw-   0        0        0      508 2023-05-28 05:57:28.000000 ardilla-0.3.1b0/ardilla/errors.py
--rw-rw-rw-   0        0        0     2586 2023-05-25 17:47:32.000000 ardilla-0.3.1b0/ardilla/fields.py
--rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.3.1b0/ardilla/logging.py
--rw-rw-rw-   0        0        0     2846 2023-05-28 13:16:48.000000 ardilla-0.3.1b0/ardilla/models.py
--rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.3.1b0/ardilla/ordering.py
--rw-rw-rw-   0        0        0     6460 2023-05-28 12:58:03.000000 ardilla-0.3.1b0/ardilla/queries.py
--rw-rw-rw-   0        0        0     5463 2023-05-28 13:44:47.000000 ardilla-0.3.1b0/ardilla/schemas.py
-drwxrwxrwx   0        0        0        0 2023-05-28 13:49:38.590145 ardilla-0.3.1b0/ardilla.egg-info/
--rw-rw-rw-   0        0        0     5203 2023-05-28 13:49:38.000000 ardilla-0.3.1b0/ardilla.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      524 2023-05-28 13:49:38.000000 ardilla-0.3.1b0/ardilla.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 13:49:38.000000 ardilla-0.3.1b0/ardilla.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      208 2023-05-28 13:49:38.000000 ardilla-0.3.1b0/ardilla.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 13:49:38.000000 ardilla-0.3.1b0/ardilla.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1216 2023-05-28 13:48:12.000000 ardilla-0.3.1b0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 13:49:38.640696 ardilla-0.3.1b0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 13:49:38.629691 ardilla-0.3.1b0/tests/
--rw-rw-rw-   0        0        0     6628 2023-05-28 05:57:28.000000 ardilla-0.3.1b0/tests/test_async.py
--rw-rw-rw-   0        0        0     2174 2023-05-28 13:21:08.000000 ardilla-0.3.1b0/tests/test_models.py
--rw-rw-rw-   0        0        0     5907 2023-05-28 05:57:28.000000 ardilla-0.3.1b0/tests/test_sync.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:38:14.898011 ardilla-0.3.2b0/
+-rw-rw-rw-   0        0        0     1084 2023-05-21 21:48:03.000000 ardilla-0.3.2b0/LICENCE
+-rw-rw-rw-   0        0        0      898 2023-05-29 14:38:14.889013 ardilla-0.3.2b0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-29 14:38:14.704012 ardilla-0.3.2b0/ardilla/
+-rw-rw-rw-   0        0        0      145 2023-05-22 03:22:06.000000 ardilla-0.3.2b0/ardilla/__init__.py
+-rw-rw-rw-   0        0        0     4877 2023-05-28 06:26:40.000000 ardilla-0.3.2b0/ardilla/abc.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:38:14.859013 ardilla-0.3.2b0/ardilla/asyncio/
+-rw-rw-rw-   0        0        0       78 2023-05-08 16:29:21.000000 ardilla-0.3.2b0/ardilla/asyncio/__init__.py
+-rw-rw-rw-   0        0        0     8771 2023-05-29 01:20:30.000000 ardilla-0.3.2b0/ardilla/asyncio/crud.py
+-rw-rw-rw-   0        0        0     2074 2023-05-28 13:12:38.000000 ardilla-0.3.2b0/ardilla/asyncio/engine.py
+-rw-rw-rw-   0        0        0     8808 2023-05-29 13:48:04.000000 ardilla-0.3.2b0/ardilla/crud.py
+-rw-rw-rw-   0        0        0     2232 2023-05-29 14:34:14.000000 ardilla-0.3.2b0/ardilla/engine.py
+-rw-rw-rw-   0        0        0      508 2023-05-28 05:57:28.000000 ardilla-0.3.2b0/ardilla/errors.py
+-rw-rw-rw-   0        0        0     2586 2023-05-25 17:47:32.000000 ardilla-0.3.2b0/ardilla/fields.py
+-rw-rw-rw-   0        0        0      222 2023-05-22 17:13:39.000000 ardilla-0.3.2b0/ardilla/logging.py
+-rw-rw-rw-   0        0        0     2846 2023-05-28 13:16:48.000000 ardilla-0.3.2b0/ardilla/models.py
+-rw-rw-rw-   0        0        0     1082 2023-05-18 22:33:35.000000 ardilla-0.3.2b0/ardilla/ordering.py
+-rw-rw-rw-   0        0        0     6518 2023-05-29 14:36:16.000000 ardilla-0.3.2b0/ardilla/queries.py
+-rw-rw-rw-   0        0        0     5680 2023-05-29 13:53:23.000000 ardilla-0.3.2b0/ardilla/schemas.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:38:14.841017 ardilla-0.3.2b0/ardilla.egg-info/
+-rw-rw-rw-   0        0        0      898 2023-05-29 14:38:14.000000 ardilla-0.3.2b0/ardilla.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      514 2023-05-29 14:38:14.000000 ardilla-0.3.2b0/ardilla.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 14:38:14.000000 ardilla-0.3.2b0/ardilla.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      208 2023-05-29 14:38:14.000000 ardilla-0.3.2b0/ardilla.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-29 14:38:14.000000 ardilla-0.3.2b0/ardilla.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1216 2023-05-29 13:53:31.000000 ardilla-0.3.2b0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 14:38:14.901023 ardilla-0.3.2b0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 14:38:14.885017 ardilla-0.3.2b0/tests/
+-rw-rw-rw-   0        0        0     6628 2023-05-28 05:57:28.000000 ardilla-0.3.2b0/tests/test_async.py
+-rw-rw-rw-   0        0        0     2174 2023-05-28 13:21:08.000000 ardilla-0.3.2b0/tests/test_models.py
+-rw-rw-rw-   0        0        0     5907 2023-05-28 05:57:28.000000 ardilla-0.3.2b0/tests/test_sync.py
```

### Comparing `ardilla-0.3.1b0/LICENCE` & `ardilla-0.3.2b0/LICENCE`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.1b0/ardilla/abc.py` & `ardilla-0.3.2b0/ardilla/abc.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.1b0/ardilla/asyncio/crud.py` & `ardilla-0.3.2b0/ardilla/asyncio/crud.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,18 +20,18 @@
     Args:
         connection (aiosqlite.Connection)
     """
     def __init__(self, connection: aiosqlite.Connection):
         self._connection = connection
     
     def __getattr__(self, __name: str) -> Any:
-        if self._connection._running and self._connection._connection:
-            return getattr(self._connection, __name)
-        else:
-            raise DisconnectedEngine('The engine is disconnected')
+        if __name in {'execute', 'commit'}:
+            if not self._connection._running or not self._connection._connection:
+                raise DisconnectedEngine('The engine is disconnected')
+        return getattr(self._connection, __name)
 
 
 class AsyncCrud(BaseCrud, Generic[M]):
     """Abstracts CRUD actions for model associated tables"""
     connection: aiosqlite.Connection
     
     def __init__(self, Model: type[M], connection: aiosqlite.Connection) -> None:
```

### Comparing `ardilla-0.3.1b0/ardilla/asyncio/engine.py` & `ardilla-0.3.2b0/ardilla/asyncio/engine.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.1b0/ardilla/crud.py` & `ardilla-0.3.2b0/ardilla/crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,40 +77,14 @@
             row = cur.fetchone()
             self.connection.commit()
             if returning and row:
                 return self._row2obj(row, cur.lastrowid)
 
         return None
 
-    def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
-        """Returns a row as an instance of the model if one is found or none
-
-        Args:
-            kws (SQLFieldType): The keyword arguments are passed as column names and values to
-                a select query
-
-        Example:
-            ```py
-            crud.get_or_none(id=42)
-
-            # returns an object with id of 42 or None if there isn't one in the database
-            ```
-
-        Returns:
-            The object found with the criteria if any
-        """
-        self.verify_kws(kws)
-        q, vals = queries.for_get_or_none(self.tablename, kws)
-        with contextcursor(self.connection) as cur:
-            cur.execute(q, vals)
-            row: Union[Row, None] = cur.fetchone()
-            if row:
-                return self._row2obj(row)
-        return None
-
     def insert(self, **kws: SQLFieldType) -> M:
         """Inserts a record into the database.
 
         Args:
             kws (SQLFieldType): The keyword arguments are passed as the column names and values
                 to the insert query
 
@@ -131,14 +105,40 @@
                 to the insert query
 
         Returns:
             The newly created row as an instance of the model if there was no conflicts
         """
         self.verify_kws(kws)
         return self._do_insert(True, True, **kws)
+    
+    def get_or_none(self, **kws: SQLFieldType) -> Optional[M]:
+        """Returns a row as an instance of the model if one is found or none
+
+        Args:
+            kws (SQLFieldType): The keyword arguments are passed as column names and values to
+                a select query
+
+        Example:
+            ```py
+            crud.get_or_none(id=42)
+
+            # returns an object with id of 42 or None if there isn't one in the database
+            ```
+
+        Returns:
+            The object found with the criteria if any
+        """
+        self.verify_kws(kws)
+        q, vals = queries.for_get_or_none(self.tablename, kws)
+        with contextcursor(self.connection) as cur:
+            cur.execute(q, vals)
+            row: Union[Row, None] = cur.fetchone()
+            if row:
+                return self._row2obj(row)
+        return None
 
     def get_or_create(self, **kws: SQLFieldType) -> tuple[M, bool]:
         """Returns an object from the database with the spefied matching data
         Args:
             kws (SQLFieldType): the key value pairs will be used to query for an existing row
                 if no record is found then a new row will be inserted
         Returns:
@@ -177,15 +177,18 @@
             kws (SQLFieldType): The column names and values for the select query
 
         Returns:
             a list of rows matching the criteria as intences of the model
         """
         self.verify_kws(kws)
         q, vals = queries.for_get_many(
-            self.Model, order_by=order_by, limit=limit, kws=kws
+            self.Model, 
+            order_by=order_by,
+            limit=limit, 
+            kws=kws,
         )
         with contextcursor(self.connection) as cur:
             cur.execute(q, vals)
             rows: list[Row] = cur.fetchall()
             return [self._row2obj(row) for row in rows]
 
     def save_one(self, obj: M) -> Literal[True]:
```

### Comparing `ardilla-0.3.1b0/ardilla/engine.py` & `ardilla-0.3.2b0/ardilla/engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,17 @@
     Attributes:
         path (str): the path to the db
         schemas (set[str]): a set of table schemas
         tables_created (set[str]): the tables that have been setup by the engine
         enable_foreing_keys (bool): if True, the engine enables the pragma on all connections
     """
     con: sqlite3.Connection
+    
+    def __init__(self, path: str, enable_foreing_keys: bool = False):
+        super().__init__(path, enable_foreing_keys)
         
     def __enter__(self):
         self.connect()
         return self
     
     def __exit__(self, *_):
         self.close()
```

### Comparing `ardilla-0.3.1b0/ardilla/fields.py` & `ardilla-0.3.2b0/ardilla/fields.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.1b0/ardilla/models.py` & `ardilla-0.3.2b0/ardilla/models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.1b0/ardilla/ordering.py` & `ardilla-0.3.2b0/ardilla/ordering.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.1b0/ardilla/queries.py` & `ardilla-0.3.2b0/ardilla/queries.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
     tablename = objs[0].__tablename__
     placeholders = ", ".join("?" * len(objs))
     if all(obj.__rowid__ for obj in objs):
         vals = tuple(obj.__rowid__ for obj in objs)
         q = f"DELETE FROM {tablename} WHERE rowid IN ({placeholders})"
 
-    elif pk := objs[0].__pk__:
+    elif (pk := objs[0].__pk__) and all(getattr(o, pk, None) is not None for o in objs):
         vals = tuple(getattr(obj, pk) for obj in objs)
         q = f"DELETE FROM {tablename} WHERE id IN ({placeholders})"
 
     else:
         raise BadQueryError(
             "Objects requiere either a primary key or the rowid set for mass deletion"
         )
```

### Comparing `ardilla-0.3.1b0/ardilla/schemas.py` & `ardilla-0.3.2b0/ardilla/schemas.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,15 +68,20 @@
         auto = extra.get('auto')
         unique = extra.get('unique')
         if default and unique:
             raise ModelIntegrityError("field {name} has both unique and default constrains which are incompatible")
         
         autoerror = ModelIntegrityError(f'field {name} has a type of "{T}" which does not support "auto"')
         schema = f'{name} {FIELD_MAPPING[T]}'
-        for k in {'pk', 'primary', 'primary_key'}:
+        
+        primary_field_keys = {'pk', 'primary', 'primary_key'}
+        if len(extra.keys() & primary_field_keys) >1:
+            raise ModelIntegrityError(f'Multiple keywords for a primary field in "{name}"')
+        
+        for k in primary_field_keys:
             if k in extra and extra[k]:
                 if pk is not None:
                     raise ModelIntegrityError('Only one primary key per model is allowed')
                 elif hasattr(Model, '__pk__') and Model.__pk__ != name:
                     raise ModelIntegrityError(f"field {name} is marked as pk, but __pk__ points to another field.")
                 
                 pk = name
```

### Comparing `ardilla-0.3.1b0/ardilla.egg-info/SOURCES.txt` & `ardilla-0.3.2b0/ardilla.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 LICENCE
-README.md
 pyproject.toml
 ardilla/__init__.py
 ardilla/abc.py
 ardilla/crud.py
 ardilla/engine.py
 ardilla/errors.py
 ardilla/fields.py
```

### Comparing `ardilla-0.3.1b0/pyproject.toml` & `ardilla-0.3.2b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ardilla"
-version = "0.3.1-beta"
+version = "0.3.2-beta"
 authors = [
   { name="ChrisDewa", email="chrisdewa@duck.com" },
 ]
 description = "Ardilla ORM. Easy to use, fast to implement, with sync and async flavors"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `ardilla-0.3.1b0/tests/test_async.py` & `ardilla-0.3.2b0/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.1b0/tests/test_models.py` & `ardilla-0.3.2b0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `ardilla-0.3.1b0/tests/test_sync.py` & `ardilla-0.3.2b0/tests/test_sync.py`

 * *Files identical despite different names*


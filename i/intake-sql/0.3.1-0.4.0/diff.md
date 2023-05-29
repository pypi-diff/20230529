# Comparing `tmp/intake-sql-0.3.1.tar.gz` & `tmp/intake-sql-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/intake-sql-0.3.1.tar", last modified: Fri Mar 26 15:52:35 2021, max compression
+gzip compressed data, was "intake-sql-0.4.0.tar", last modified: Mon May 29 20:08:57 2023, max compression
```

## Comparing `intake-sql-0.3.1.tar` & `intake-sql-0.4.0.tar`

### file list

```diff
@@ -1,39 +1,32 @@
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2021-03-26 15:52:35.982810 intake-sql-0.3.1/
--rw-r--r--   0 mdurant    (502) staff       (20)     1557 2020-12-11 15:38:24.000000 intake-sql-0.3.1/.travis.yml
--rw-r--r--   0 mdurant    (502) staff       (20)     1330 2020-12-11 15:38:24.000000 intake-sql-0.3.1/LICENSE
--rw-r--r--   0 mdurant    (502) staff       (20)      219 2020-12-11 15:38:24.000000 intake-sql-0.3.1/MANIFEST.in
--rw-r--r--   0 mdurant    (502) staff       (20)      852 2021-03-26 15:52:35.982942 intake-sql-0.3.1/PKG-INFO
--rw-r--r--   0 mdurant    (502) staff       (20)      452 2021-03-26 15:50:03.000000 intake-sql-0.3.1/README.md
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2021-03-26 15:52:35.974119 intake-sql-0.3.1/docs/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2021-03-26 15:52:35.969798 intake-sql-0.3.1/docs/build/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2021-03-26 15:52:35.976695 intake-sql-0.3.1/docs/build/html/
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2021-03-26 15:52:35.976997 intake-sql-0.3.1/docs/build/html/_modules/
--rwxrwxrwx   0 mdurant    (502) staff       (20)     4502 2020-04-14 14:08:53.000000 intake-sql-0.3.1/docs/build/html/_modules/index.html
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2021-03-26 15:52:35.977887 intake-sql-0.3.1/docs/build/html/_modules/intake_sql/
--rwxrwxrwx   0 mdurant    (502) staff       (20)    39271 2020-04-14 14:08:53.000000 intake-sql-0.3.1/docs/build/html/_modules/intake_sql/intake_sql.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)    11102 2020-04-14 14:08:53.000000 intake-sql-0.3.1/docs/build/html/_modules/intake_sql/sql_cat.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)    26420 2020-04-14 14:08:53.000000 intake-sql-0.3.1/docs/build/html/api.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)     6040 2020-04-14 14:08:53.000000 intake-sql-0.3.1/docs/build/html/genindex.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)     6125 2020-04-14 14:08:53.000000 intake-sql-0.3.1/docs/build/html/index.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)     7985 2020-04-14 14:08:53.000000 intake-sql-0.3.1/docs/build/html/quickstart.html
--rwxrwxrwx   0 mdurant    (502) staff       (20)     4678 2020-04-14 14:08:53.000000 intake-sql-0.3.1/docs/build/html/search.html
--rw-r--r--   0 mdurant    (502) staff       (20)      162 2020-12-11 15:38:24.000000 intake-sql-0.3.1/docs/environment.yml
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2021-03-26 15:52:35.983792 intake-sql-0.3.1/intake_sql/
--rw-r--r--   0 mdurant    (502) staff       (20)      251 2020-12-11 15:38:24.000000 intake-sql-0.3.1/intake_sql/__init__.py
--rw-r--r--   0 mdurant    (502) staff       (20)      497 2021-03-26 15:52:35.983900 intake-sql-0.3.1/intake_sql/_version.py
--rw-r--r--   0 mdurant    (502) staff       (20)    11641 2021-02-24 14:44:10.000000 intake-sql-0.3.1/intake_sql/intake_sql.py
--rw-r--r--   0 mdurant    (502) staff       (20)     2435 2020-12-11 15:38:24.000000 intake-sql-0.3.1/intake_sql/sql_cat.py
-drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2021-03-26 15:52:35.982541 intake-sql-0.3.1/intake_sql.egg-info/
--rwxrwxrwx   0 mdurant    (502) staff       (20)      852 2021-03-26 15:52:35.000000 intake-sql-0.3.1/intake_sql.egg-info/PKG-INFO
--rwxrwxrwx   0 mdurant    (502) staff       (20)      790 2021-03-26 15:52:35.000000 intake-sql-0.3.1/intake_sql.egg-info/SOURCES.txt
--rwxrwxrwx   0 mdurant    (502) staff       (20)        1 2021-03-26 15:52:35.000000 intake-sql-0.3.1/intake_sql.egg-info/dependency_links.txt
--rwxrwxrwx   0 mdurant    (502) staff       (20)      212 2021-03-26 15:52:35.000000 intake-sql-0.3.1/intake_sql.egg-info/entry_points.txt
--rwxrwxrwx   0 mdurant    (502) staff       (20)        1 2020-04-14 14:08:53.000000 intake-sql-0.3.1/intake_sql.egg-info/not-zip-safe
--rwxrwxrwx   0 mdurant    (502) staff       (20)       46 2020-04-14 14:08:53.000000 intake-sql-0.3.1/intake_sql.egg-info/pbr.json
--rwxrwxrwx   0 mdurant    (502) staff       (20)       25 2021-03-26 15:52:35.000000 intake-sql-0.3.1/intake_sql.egg-info/requires.txt
--rwxrwxrwx   0 mdurant    (502) staff       (20)       11 2021-03-26 15:52:35.000000 intake-sql-0.3.1/intake_sql.egg-info/top_level.txt
--rw-r--r--   0 mdurant    (502) staff       (20)       38 2020-12-11 15:38:24.000000 intake-sql-0.3.1/readthedocs.yml
--rw-r--r--   0 mdurant    (502) staff       (20)       24 2020-12-11 15:38:24.000000 intake-sql-0.3.1/requirements.txt
--rw-r--r--   0 mdurant    (502) staff       (20)      178 2021-03-26 15:52:35.983435 intake-sql-0.3.1/setup.cfg
--rw-r--r--   0 mdurant    (502) staff       (20)     1046 2021-03-26 15:51:12.000000 intake-sql-0.3.1/setup.py
--rw-r--r--   0 mdurant    (502) staff       (20)    68611 2020-12-11 15:38:24.000000 intake-sql-0.3.1/versioneer.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:08:57.791740 intake-sql-0.4.0/
+-rw-r--r--   0 mdurant    (502) staff       (20)     1330 2023-05-10 14:39:26.000000 intake-sql-0.4.0/LICENSE
+-rw-r--r--   0 mdurant    (502) staff       (20)      219 2023-05-10 14:39:26.000000 intake-sql-0.4.0/MANIFEST.in
+-rw-r--r--   0 mdurant    (502) staff       (20)      731 2023-05-29 20:08:57.791804 intake-sql-0.4.0/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      452 2023-05-10 14:39:26.000000 intake-sql-0.4.0/README.md
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:08:57.788987 intake-sql-0.4.0/ci/
+-rw-r--r--   0 mdurant    (502) staff       (20)      225 2023-05-10 17:08:09.000000 intake-sql-0.4.0/ci/environment-py310.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      205 2023-05-10 17:08:09.000000 intake-sql-0.4.0/ci/environment-py38.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)      205 2023-05-10 14:39:26.000000 intake-sql-0.4.0/ci/environment-py39.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:08:57.789263 intake-sql-0.4.0/docs/
+-rw-r--r--   0 mdurant    (502) staff       (20)      162 2023-05-10 14:39:26.000000 intake-sql-0.4.0/docs/environment.yml
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:08:57.792454 intake-sql-0.4.0/intake_sql/
+-rw-r--r--   0 mdurant    (502) staff       (20)      251 2023-05-10 14:39:26.000000 intake-sql-0.4.0/intake_sql/__init__.py
+-rw-r--r--   0 mdurant    (502) staff       (20)      497 2023-05-29 20:08:57.792515 intake-sql-0.4.0/intake_sql/_version.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    11749 2023-05-10 14:39:26.000000 intake-sql-0.4.0/intake_sql/intake_sql.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     3096 2023-05-10 17:08:09.000000 intake-sql-0.4.0/intake_sql/sql_cat.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:08:57.791272 intake-sql-0.4.0/intake_sql.egg-info/
+-rw-r--r--   0 mdurant    (502) staff       (20)      731 2023-05-29 20:08:57.000000 intake-sql-0.4.0/intake_sql.egg-info/PKG-INFO
+-rw-r--r--   0 mdurant    (502) staff       (20)      578 2023-05-29 20:08:57.000000 intake-sql-0.4.0/intake_sql.egg-info/SOURCES.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-29 20:08:57.000000 intake-sql-0.4.0/intake_sql.egg-info/dependency_links.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      211 2023-05-29 20:08:57.000000 intake-sql-0.4.0/intake_sql.egg-info/entry_points.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)        1 2023-05-10 14:54:23.000000 intake-sql-0.4.0/intake_sql.egg-info/not-zip-safe
+-rw-r--r--   0 mdurant    (502) staff       (20)       27 2023-05-29 20:08:57.000000 intake-sql-0.4.0/intake_sql.egg-info/requires.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       11 2023-05-29 20:08:57.000000 intake-sql-0.4.0/intake_sql.egg-info/top_level.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)       38 2023-05-10 14:39:26.000000 intake-sql-0.4.0/readthedocs.yml
+-rw-r--r--   0 mdurant    (502) staff       (20)       27 2023-05-10 17:08:09.000000 intake-sql-0.4.0/requirements.txt
+-rw-r--r--   0 mdurant    (502) staff       (20)      178 2023-05-29 20:08:57.792129 intake-sql-0.4.0/setup.cfg
+-rw-r--r--   0 mdurant    (502) staff       (20)     1046 2023-05-10 14:39:26.000000 intake-sql-0.4.0/setup.py
+drwxr-xr-x   0 mdurant    (502) staff       (20)        0 2023-05-29 20:08:57.791583 intake-sql-0.4.0/tests/
+-rw-r--r--   0 mdurant    (502) staff       (20)     2119 2023-05-10 17:08:09.000000 intake-sql-0.4.0/tests/test_intake_sql.py
+-rw-r--r--   0 mdurant    (502) staff       (20)     2063 2023-05-10 17:08:09.000000 intake-sql-0.4.0/tests/test_sql_cat.py
+-rw-r--r--   0 mdurant    (502) staff       (20)    68611 2023-05-10 14:39:26.000000 intake-sql-0.4.0/versioneer.py
```

### Comparing `intake-sql-0.3.1/LICENSE` & `intake-sql-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intake-sql-0.3.1/PKG-INFO` & `intake-sql-0.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: intake-sql
-Version: 0.3.1
+Version: 0.4.0
 Summary: SQL plugin for Intake
 Home-page: https://github.com/ContinuumIO/intake-sql
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
-Description: # Intake-SQL
-        [![Build Status](https://travis-ci.org/ContinuumIO/intake-sql.svg?branch=master)](https://travis-ci.org/ContinuumIO/intake-sql)
-        [![Documentation Status](https://readthedocs.org/projects/intake-sql/badge/?version=latest)](http://intake-sql.readthedocs.io/en/latest/?badge=latest)
-        
-        SQL Plugin for Intake
-        
-        
-        ## User Installation
-        
-        To install the intake-sql plugin, execute the following command
-        ```
-        conda install -c conda-forge intake-sql
-        ```
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Intake-SQL
+[![Build Status](https://travis-ci.org/ContinuumIO/intake-sql.svg?branch=master)](https://travis-ci.org/ContinuumIO/intake-sql)
+[![Documentation Status](https://readthedocs.org/projects/intake-sql/badge/?version=latest)](http://intake-sql.readthedocs.io/en/latest/?badge=latest)
+
+SQL Plugin for Intake
+
+
+## User Installation
+
+To install the intake-sql plugin, execute the following command
+```
+conda install -c conda-forge intake-sql
+```
+
```

### Comparing `intake-sql-0.3.1/intake_sql/intake_sql.py` & `intake-sql-0.4.0/intake_sql/intake_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     def _get_schema(self):
         if self._dataframe is None:
             # TODO: could do read_sql with chunksize to get likely schema from
             # first few records, rather than loading the whole thing
             self._load()
         return base.Schema(datashape=None,
-                           dtype=self._dataframe.dtypes,
+                           dtype={k: str(v) for k,v in self._dataframe.dtypes.items()},
                            shape=self._dataframe.shape,
                            npartitions=1,
                            extra_metadata={})
 
     def _get_partition(self, _):
         if self._dataframe is None:
             self._load_metadata()
@@ -132,15 +132,15 @@
         self._dataframe = dd.read_sql_table(self._sql_expr, self._uri,
                                             self._index, **self._sql_kwargs)
 
     def _get_schema(self):
         if self._dataframe is None:
             self._load()
         return base.Schema(datashape=None,
-                           dtype=self._dataframe,
+                           dtype={k: str(v) for k,v in self._dataframe.dtypes.items()},
                            shape=(None, len(self._dataframe.columns)),
                            npartitions=self._dataframe.npartitions,
                            extra_metadata={})
 
     def _get_partition(self, i):
         if self._dataframe is None:
             self._load_metadata()
@@ -241,15 +241,15 @@
                                          meta=self._meta,
                                          kwargs=self._sql_kwargs)
 
     def _get_schema(self):
         if self._dataframe is None:
             self._load()
         return base.Schema(datashape=None,
-                           dtype=self._dataframe,
+                           dtype={k: str(v) for k,v in self._dataframe.dtypes.items()},
                            shape=(None, len(self._dataframe.columns)),
                            npartitions=self._dataframe.npartitions,
                            extra_metadata={})
 
     def _get_partition(self, i):
         if self._dataframe is None:
             self._load_metadata()
@@ -304,15 +304,15 @@
     kwargs: dict
         Any further parameters to pass to pd.read_sql_query, see
         its documentation
     """
     import dask
     import dask.dataframe as dd
     if where_tmp is not None:
-        where = [where_tmp.format(values) for values in where]
+        where = [where_tmp.format(*values) for values in where]
     if kwargs is None:
         kwargs = {}
     dload = dask.delayed(load_part)
     parts = [dload(sql, uri, w, kwargs) for w in where]
     return dd.from_delayed(parts, meta=meta)
```

### Comparing `intake-sql-0.3.1/intake_sql/sql_cat.py` & `intake-sql-0.4.0/intake_sql/sql_cat.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-
 from . import __version__
+from collections.abc import Mapping
 from intake.catalog.base import Catalog
 from intake.catalog.local import LocalCatalogEntry
 
 
 class SQLCatalog(Catalog):
     """
     Makes data sources out of known tables in the given SQL service
@@ -19,40 +19,74 @@
         self.sql_kwargs = sql_kwargs or {}
         self.uri = uri
         self.views = views
         super(SQLCatalog, self).__init__(**kwargs)
 
     def _load(self):
         import sqlalchemy
-        from intake_sql import SQLSource, SQLSourceAutoPartition
         engine = sqlalchemy.create_engine(self.uri)
-        meta = sqlalchemy.MetaData(bind=engine)
-        meta.reflect(views=self.views, schema=self.sql_kwargs.get("schema"))
-        self._entries = {}
-        for name, table in meta.tables.items():
-            description = 'SQL table %s from %s' % (name, self.uri)
-            for c in table.columns:
-                # We use table.name instead of the metadata key here as it
-                # does not include the schema name, which is handled
-                # by the `sql_kwargs`.
-                if c.primary_key:
-
-                    description = 'SQL table %s from %s' % (name, self.uri)
-                    args = {'uri': self.uri, 'table': table.name, 'index': c.name,
-                            'sql_kwargs': self.sql_kwargs}
-                    e = LocalCatalogEntry(table.name, description, 'sql_auto', True,
-                                          args, {}, {}, {}, "", getenv=False,
-                                          getshell=False)
-                    e._plugin = [SQLSourceAutoPartition]
-                    self._entries[table.name] = e
-                    break
-            else:
-                args = {
-                    'uri': self.uri,
-                    'sql_expr': table.name,
-                    'sql_kwargs': self.sql_kwargs
-                }
-                e = LocalCatalogEntry(name,description, 'sql', True,
-                                      args, {}, {}, {}, "", getenv=False,
+        meta = sqlalchemy.MetaData()
+        meta.reflect(bind=engine, views=self.views,
+                     schema=self.sql_kwargs.get("schema"))
+        self._entries = SQLEntries(meta, self.uri, self.sql_kwargs)
+
+
+class SQLEntries(Mapping):
+
+    def __init__(self, meta, uri, sql_kwargs):
+        self.meta = meta
+        self.uri = uri
+        self.sql_kwargs = sql_kwargs
+        self.tables = None
+        self.cache = {}
+
+    def _get_tables(self):
+        if self.tables is None:
+            self.tables = list(self.meta.tables)
+
+    def _make_entry(self, name):
+        if name in self.cache:
+            return
+        from intake_sql import SQLSource, SQLSourceAutoPartition
+        description = 'SQL table %s from %s' % (name, self.uri)
+        table = self.meta.tables[name]
+        for c in table.columns:
+            # We use table.name instead of the metadata key here as it
+            # does not include the schema name, which is handled
+            # by the `sql_kwargs`.
+            if c.primary_key:
+
+                description = 'SQL table %s from %s' % (name, self.uri)
+                args = {'uri': self.uri, 'table': table.name, 'index': c.name,
+                        'sql_kwargs': self.sql_kwargs}
+                e = LocalCatalogEntry(table.name, description, 'sql_auto', True,
+                                      args, {}, [], {}, "", getenv=False,
                                       getshell=False)
-                e._plugin = [SQLSource]
-                self._entries[table.name] = e
+                e._plugin = [SQLSourceAutoPartition]
+                self.cache[name] = e
+                break
+        else:
+            args = {
+                'uri': self.uri,
+                'sql_expr': table.name,
+                'sql_kwargs': self.sql_kwargs
+            }
+            e = LocalCatalogEntry(name,description, 'sql', True,
+                                  args, {}, [], {}, "", getenv=False,
+                                  getshell=False)
+            e._plugin = [SQLSource]
+            self.cache[name] = e
+
+    def keys(self):
+        self._get_tables()
+        return self.tables
+
+    def __getitem__(self, item):
+        self._make_entry(item)
+        return self.cache[item]
+
+    def __len__(self):
+        return len(self.keys())
+
+    def __iter__(self):
+        return iter(self.keys())
+
```

### Comparing `intake-sql-0.3.1/intake_sql.egg-info/PKG-INFO` & `intake-sql-0.4.0/intake_sql.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: intake-sql
-Version: 0.3.1
+Version: 0.4.0
 Summary: SQL plugin for Intake
 Home-page: https://github.com/ContinuumIO/intake-sql
 Maintainer: Martin Durant
 Maintainer-email: mdurant@anaconda.com
 License: BSD
-Description: # Intake-SQL
-        [![Build Status](https://travis-ci.org/ContinuumIO/intake-sql.svg?branch=master)](https://travis-ci.org/ContinuumIO/intake-sql)
-        [![Documentation Status](https://readthedocs.org/projects/intake-sql/badge/?version=latest)](http://intake-sql.readthedocs.io/en/latest/?badge=latest)
-        
-        SQL Plugin for Intake
-        
-        
-        ## User Installation
-        
-        To install the intake-sql plugin, execute the following command
-        ```
-        conda install -c conda-forge intake-sql
-        ```
-        
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Intake-SQL
+[![Build Status](https://travis-ci.org/ContinuumIO/intake-sql.svg?branch=master)](https://travis-ci.org/ContinuumIO/intake-sql)
+[![Documentation Status](https://readthedocs.org/projects/intake-sql/badge/?version=latest)](http://intake-sql.readthedocs.io/en/latest/?badge=latest)
+
+SQL Plugin for Intake
+
+
+## User Installation
+
+To install the intake-sql plugin, execute the following command
+```
+conda install -c conda-forge intake-sql
+```
+
```

### Comparing `intake-sql-0.3.1/setup.py` & `intake-sql-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `intake-sql-0.3.1/versioneer.py` & `intake-sql-0.4.0/versioneer.py`

 * *Files identical despite different names*


# Comparing `tmp/red_postgres-0.0.1a0-py3-none-any.whl.zip` & `tmp/red_postgres-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10742 bytes, number of entries: 8
+Zip file size: 10719 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat       34 b- defN 23-May-29 15:32 __init__.py
 -rw-rw-rw-  2.0 fat     4126 b- defN 23-May-29 15:16 engine.py
 -rw-rw-rw-  2.0 fat       23 b- defN 23-May-29 15:15 version.py
--rw-rw-rw-  2.0 fat    18431 b- defN 23-May-29 16:31 red_postgres-0.0.1a0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1837 b- defN 23-May-29 16:31 red_postgres-0.0.1a0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 16:31 red_postgres-0.0.1a0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       24 b- defN 23-May-29 16:31 red_postgres-0.0.1a0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      619 b- defN 23-May-29 16:31 red_postgres-0.0.1a0.dist-info/RECORD
-8 files, 25186 bytes uncompressed, 9664 bytes compressed:  61.6%
+-rw-rw-rw-  2.0 fat    18431 b- defN 23-May-29 16:33 red_postgres-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1835 b- defN 23-May-29 16:33 red_postgres-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 16:33 red_postgres-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       24 b- defN 23-May-29 16:33 red_postgres-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      609 b- defN 23-May-29 16:33 red_postgres-0.0.2.dist-info/RECORD
+8 files, 25174 bytes uncompressed, 9661 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: engine.py
 Comment: 
 
 Filename: version.py
 Comment: 
 
-Filename: red_postgres-0.0.1a0.dist-info/LICENSE
+Filename: red_postgres-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: red_postgres-0.0.1a0.dist-info/METADATA
+Filename: red_postgres-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: red_postgres-0.0.1a0.dist-info/WHEEL
+Filename: red_postgres-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: red_postgres-0.0.1a0.dist-info/top_level.txt
+Filename: red_postgres-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: red_postgres-0.0.1a0.dist-info/RECORD
+Filename: red_postgres-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `red_postgres-0.0.1a0.dist-info/LICENSE` & `red_postgres-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `red_postgres-0.0.1a0.dist-info/METADATA` & `red_postgres-0.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: red-postgres
-Version: 0.0.1a0
+Version: 0.0.2
 Summary: Piccolo Postgres integration for Red
 Author: Vertyco
 Project-URL: Homepage, https://github.com/vertyco/red-postgres
 Project-URL: Bug Tracker, https://github.com/vertyco/red-postgres/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
@@ -23,15 +23,15 @@
     │   ├── migrations/
     │   ├── piccolo_conf.py
     │   ├── piccolo_app.py
     │   ├── tables.py
     ├── __init__.py
     ├── cog.py
 ```
-![SCHEMA](.github\ASSETS\schema.png)
+![SCHEMA](.github/ASSETS/schema.png)
 
 # piccolo_conf.py
 ```python
 import os
 
 from piccolo.conf.apps import AppRegistry
 from piccolo.engine.postgres import PostgresEngine
```


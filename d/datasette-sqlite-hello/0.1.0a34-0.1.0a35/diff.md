# Comparing `tmp/datasette_sqlite_hello-0.1.0a34-py3-none-any.whl.zip` & `tmp/datasette_sqlite_hello-0.1.0a35-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2205 bytes, number of entries: 7
--rw-r--r--  2.0 unx      269 b- defN 23-May-29 04:38 datasette_sqlite_hello/__init__.py
--rw-r--r--  2.0 unx       80 b- defN 23-May-29 04:38 datasette_sqlite_hello/version.py
--rw-r--r--  2.0 unx      570 b- defN 23-May-29 04:39 datasette_sqlite_hello-0.1.0a34.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 04:39 datasette_sqlite_hello-0.1.0a34.dist-info/WHEEL
--rw-r--r--  2.0 unx       50 b- defN 23-May-29 04:39 datasette_sqlite_hello-0.1.0a34.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       23 b- defN 23-May-29 04:39 datasette_sqlite_hello-0.1.0a34.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      660 b- defN 23-May-29 04:39 datasette_sqlite_hello-0.1.0a34.dist-info/RECORD
-7 files, 1744 bytes uncompressed, 1001 bytes compressed:  42.6%
+Zip file size: 2206 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      269 b- defN 23-May-29 04:50 datasette_sqlite_hello/__init__.py
+-rw-r--r--  2.0 unx       80 b- defN 23-May-29 04:50 datasette_sqlite_hello/version.py
+-rw-r--r--  2.0 unx      570 b- defN 23-May-29 04:50 datasette_sqlite_hello-0.1.0a35.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 04:50 datasette_sqlite_hello-0.1.0a35.dist-info/WHEEL
+-rw-r--r--  2.0 unx       50 b- defN 23-May-29 04:50 datasette_sqlite_hello-0.1.0a35.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       23 b- defN 23-May-29 04:50 datasette_sqlite_hello-0.1.0a35.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      660 b- defN 23-May-29 04:50 datasette_sqlite_hello-0.1.0a35.dist-info/RECORD
+7 files, 1744 bytes uncompressed, 1002 bytes compressed:  42.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: datasette_sqlite_hello/__init__.py
 Comment: 
 
 Filename: datasette_sqlite_hello/version.py
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a34.dist-info/METADATA
+Filename: datasette_sqlite_hello-0.1.0a35.dist-info/METADATA
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a34.dist-info/WHEEL
+Filename: datasette_sqlite_hello-0.1.0a35.dist-info/WHEEL
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a34.dist-info/entry_points.txt
+Filename: datasette_sqlite_hello-0.1.0a35.dist-info/entry_points.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a34.dist-info/top_level.txt
+Filename: datasette_sqlite_hello-0.1.0a35.dist-info/top_level.txt
 Comment: 
 
-Filename: datasette_sqlite_hello-0.1.0a34.dist-info/RECORD
+Filename: datasette_sqlite_hello-0.1.0a35.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## datasette_sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.34"
+__version__ = "0.1.0-alpha.35"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `datasette_sqlite_hello-0.1.0a34.dist-info/METADATA` & `datasette_sqlite_hello-0.1.0a35.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datasette-sqlite-hello
-Version: 0.1.0a34
+Version: 0.1.0a35
 Home-page: https://github.com/asg017/sqlite-hello
 Author: Alex Garcia
 License: MIT License, Apache License, Version 2.0
 Project-URL: Issues, https://github.com/asg017/sqlite-hello/issues
 Project-URL: CI, https://github.com/asg017/sqlite-hello/actions
 Project-URL: Changelog, https://github.com/asg017/sqlite-hello/releases
 Requires-Python: >=3.6
```


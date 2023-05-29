# Comparing `tmp/tablepy_lib-0.4.0.tar.gz` & `tmp/tablepy_lib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablepy_lib-0.4.0.tar", max compression
+gzip compressed data, was "tablepy_lib-0.5.0.tar", max compression
```

## Comparing `tablepy_lib-0.4.0.tar` & `tablepy_lib-0.5.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.4.0/LICENSE
--rw-r--r--   0        0        0      502 2023-05-29 14:01:31.354459 tablepy_lib-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1305 2023-05-29 14:01:08.849013 tablepy_lib-0.4.0/README.md
--rw-r--r--   0        0        0       49 2023-05-24 21:31:44.458131 tablepy_lib-0.4.0/tablepy_lib/__init__.py
--rw-r--r--   0        0        0     4471 2023-05-29 14:01:50.722503 tablepy_lib-0.4.0/tablepy_lib/consoleFormatter.py
--rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 tablepy_lib-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.5.0/LICENSE
+-rw-r--r--   0        0        0      504 2023-05-29 14:15:18.245163 tablepy_lib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1305 2023-05-29 14:01:08.849013 tablepy_lib-0.5.0/README.md
+-rw-r--r--   0        0        0      144 2023-05-29 14:13:45.843894 tablepy_lib-0.5.0/tablepy_lib/__init__.py
+-rw-r--r--   0        0        0     4493 2023-05-29 14:13:19.507295 tablepy_lib-0.5.0/tablepy_lib/consoleFormatter.py
+-rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 tablepy_lib-0.5.0/PKG-INFO
```

### Comparing `tablepy_lib-0.4.0/LICENSE` & `tablepy_lib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tablepy_lib-0.4.0/README.md` & `tablepy_lib-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `tablepy_lib-0.4.0/tablepy_lib/consoleFormatter.py` & `tablepy_lib-0.5.0/tablepy_lib/consoleFormatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #----------------------------------------------------------------------------
 # Created By  : Jordi Corbilla
 # Created Date: 2023
-# version ='0.4.0'
+# version ='0.5.0'
 # ---------------------------------------------------------------------------
 
 import pandas as pd
 
 class ConsoleFormatter:
     def __init__(self, data):
         if isinstance(data, dict):
@@ -130,9 +130,9 @@
         formatted_value = "'" + data.replace("'", "''") + "'"
         return formatted_value
 
     
 def markdown(data):
     return ConsoleFormatter(data).to_table()
 
-def sql_insert(data):
-    return ConsoleFormatter(data).to_sql()
+def sql_insert(data, table_name):
+    return ConsoleFormatter(data).to_sql(table_name)
```

### Comparing `tablepy_lib-0.4.0/PKG-INFO` & `tablepy_lib-0.5.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tablepy-lib
-Version: 0.4.0
-Summary: This is a versatile and user-friendly Python table library that can quickly render any Dictionary<TV, T> or DataFrame into a visually appealing markdown or sql insert
+Version: 0.5.0
+Summary: This is a versatile and user-friendly Python table library that can quickly render any Dictionary{key, []} or DataFrame into a visually appealing markdown or sql insert
 Author: Jordi Corbilla
 Author-email: jordi.coll.corbilla@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```


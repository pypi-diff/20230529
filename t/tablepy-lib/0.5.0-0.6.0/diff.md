# Comparing `tmp/tablepy_lib-0.5.0.tar.gz` & `tmp/tablepy_lib-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablepy_lib-0.5.0.tar", max compression
+gzip compressed data, was "tablepy_lib-0.6.0.tar", max compression
```

## Comparing `tablepy_lib-0.5.0.tar` & `tablepy_lib-0.6.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.5.0/LICENSE
--rw-r--r--   0        0        0      504 2023-05-29 14:15:18.245163 tablepy_lib-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1305 2023-05-29 14:01:08.849013 tablepy_lib-0.5.0/README.md
--rw-r--r--   0        0        0      144 2023-05-29 14:13:45.843894 tablepy_lib-0.5.0/tablepy_lib/__init__.py
--rw-r--r--   0        0        0     4493 2023-05-29 14:13:19.507295 tablepy_lib-0.5.0/tablepy_lib/consoleFormatter.py
--rw-r--r--   0        0        0     1825 1970-01-01 00:00:00.000000 tablepy_lib-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.6.0/LICENSE
+-rw-r--r--   0        0        0      504 2023-05-29 14:51:48.305727 tablepy_lib-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1497 2023-05-29 14:50:31.310092 tablepy_lib-0.6.0/README.md
+-rw-r--r--   0        0        0      144 2023-05-29 14:13:45.843894 tablepy_lib-0.6.0/tablepy_lib/__init__.py
+-rw-r--r--   0        0        0     4493 2023-05-29 14:51:55.275455 tablepy_lib-0.6.0/tablepy_lib/consoleFormatter.py
+-rw-r--r--   0        0        0     2014 1970-01-01 00:00:00.000000 tablepy_lib-0.6.0/PKG-INFO
```

### Comparing `tablepy_lib-0.5.0/LICENSE` & `tablepy_lib-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tablepy_lib-0.5.0/README.md` & `tablepy_lib-0.6.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # tablepy Lib
 
+This is a versatile and user-friendly Python table library that can quickly render any Dictionary{key, []} or DataFrame into a visually appealing markdown or sql insert
+
 ## Usage - Markdown
 
 ```python
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
     "Country": ["USA", "Canada", "UK", "DE"],
@@ -32,15 +34,16 @@
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
     "Country": ["USA", "Canada", "UK", "DE"],
     "Data": ["USA", "Canada", "UK", "3434243"]
 }
 
-table = consoleFormatter(data_frame).to_sql('dd')
+data_frame = pd.DataFrame(data)
+table = sql_insert(data_frame, 'dd')
 print(table)
 
 ```
 
 Sample output:
 
 ```
```

### Comparing `tablepy_lib-0.5.0/tablepy_lib/consoleFormatter.py` & `tablepy_lib-0.6.0/tablepy_lib/consoleFormatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #----------------------------------------------------------------------------
 # Created By  : Jordi Corbilla
 # Created Date: 2023
-# version ='0.5.0'
+# version ='0.6.0'
 # ---------------------------------------------------------------------------
 
 import pandas as pd
 
 class ConsoleFormatter:
     def __init__(self, data):
         if isinstance(data, dict):
```

### Comparing `tablepy_lib-0.5.0/PKG-INFO` & `tablepy_lib-0.6.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: tablepy-lib
-Version: 0.5.0
+Version: 0.6.0
 Summary: This is a versatile and user-friendly Python table library that can quickly render any Dictionary{key, []} or DataFrame into a visually appealing markdown or sql insert
 Author: Jordi Corbilla
 Author-email: jordi.coll.corbilla@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # tablepy Lib
 
+This is a versatile and user-friendly Python table library that can quickly render any Dictionary{key, []} or DataFrame into a visually appealing markdown or sql insert
+
 ## Usage - Markdown
 
 ```python
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
     "Country": ["USA", "Canada", "UK", "DE"],
@@ -45,15 +47,16 @@
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
     "Country": ["USA", "Canada", "UK", "DE"],
     "Data": ["USA", "Canada", "UK", "3434243"]
 }
 
-table = consoleFormatter(data_frame).to_sql('dd')
+data_frame = pd.DataFrame(data)
+table = sql_insert(data_frame, 'dd')
 print(table)
 
 ```
 
 Sample output:
 
 ```
```


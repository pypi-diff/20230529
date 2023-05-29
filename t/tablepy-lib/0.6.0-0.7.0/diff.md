# Comparing `tmp/tablepy_lib-0.6.0.tar.gz` & `tmp/tablepy_lib-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablepy_lib-0.6.0.tar", max compression
+gzip compressed data, was "tablepy_lib-0.7.0.tar", max compression
```

## Comparing `tablepy_lib-0.6.0.tar` & `tablepy_lib-0.7.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.6.0/LICENSE
--rw-r--r--   0        0        0      504 2023-05-29 14:51:48.305727 tablepy_lib-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     1497 2023-05-29 14:50:31.310092 tablepy_lib-0.6.0/README.md
--rw-r--r--   0        0        0      144 2023-05-29 14:13:45.843894 tablepy_lib-0.6.0/tablepy_lib/__init__.py
--rw-r--r--   0        0        0     4493 2023-05-29 14:51:55.275455 tablepy_lib-0.6.0/tablepy_lib/consoleFormatter.py
--rw-r--r--   0        0        0     2014 1970-01-01 00:00:00.000000 tablepy_lib-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.7.0/LICENSE
+-rw-r--r--   0        0        0      504 2023-05-29 19:12:21.590034 tablepy_lib-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     1830 2023-05-29 18:11:55.249238 tablepy_lib-0.7.0/README.md
+-rw-r--r--   0        0        0      496 2023-05-29 19:12:41.683383 tablepy_lib-0.7.0/tablepy_lib/__init__.py
+-rw-r--r--   0        0        0     4552 2023-05-29 19:12:26.039182 tablepy_lib-0.7.0/tablepy_lib/consoleFormatter.py
+-rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 tablepy_lib-0.7.0/PKG-INFO
```

### Comparing `tablepy_lib-0.6.0/LICENSE` & `tablepy_lib-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tablepy_lib-0.6.0/README.md` & `tablepy_lib-0.7.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,50 @@
 # tablepy Lib
 
 This is a versatile and user-friendly Python table library that can quickly render any Dictionary{key, []} or DataFrame into a visually appealing markdown or sql insert
 
 ## Usage - Markdown
 
 ```python
+from tablepy_lib import markdown
+
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
     "Country": ["USA", "Canada", "UK", "DE"],
     "Data": ["USA", "Canada", "UK", "3434243"]
 }
 
-formatter = consoleFormatter(data)
-table = formatter.to_table()
+table = markdown(data)
 print(table)    
 ```
 
 Sample output:
 
 ```
 | Name    | Age      | Country   | Data      | 
 | ------- | -------- | --------- | --------- | 
 | John    | -28.0    | USA       | USA       | 
 | Emily   | 3002.6   | Canada    | Canada    | 
 | Tom     | 25.0     | UK        | UK        | 
 | JC      | 2.0      | DE        | 3434243   | 
 ```
 
+| Name    | Age      | Country   | Data      | 
+| ------- | -------- | --------- | --------- | 
+| John    | -28.0    | USA       | USA       | 
+| Emily   | 3002.6   | Canada    | Canada    | 
+| Tom     | 25.0     | UK        | UK        | 
+| JC      | 2.0      | DE        | 3434243   | 
+
 ## Usage - SQL Insert
 
 ```python
+from tablepy_lib import sql_insert
+
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
     "Country": ["USA", "Canada", "UK", "DE"],
     "Data": ["USA", "Canada", "UK", "3434243"]
 }
 
@@ -42,13 +52,13 @@
 table = sql_insert(data_frame, 'dd')
 print(table)
 
 ```
 
 Sample output:
 
-```
+```sql
 INSERT INTO dd (Name, Age, Country, Data) VALUES ('John', -28.0, 'USA', 'USA');
 INSERT INTO dd (Name, Age, Country, Data) VALUES ('Emily', 3002.6, 'Canada', 'Canada');
 INSERT INTO dd (Name, Age, Country, Data) VALUES ('Tom', 25.0, 'UK', 'UK');
 INSERT INTO dd (Name, Age, Country, Data) VALUES ('JC', 2.0, 'DE', 3434243);
-```
+```
```

### Comparing `tablepy_lib-0.6.0/tablepy_lib/consoleFormatter.py` & `tablepy_lib-0.7.0/tablepy_lib/consoleFormatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #----------------------------------------------------------------------------
 # Created By  : Jordi Corbilla
 # Created Date: 2023
-# version ='0.6.0'
+# version ='0.7.0'
 # ---------------------------------------------------------------------------
 
 import pandas as pd
 
 class ConsoleFormatter:
     def __init__(self, data):
         if isinstance(data, dict):
@@ -127,12 +127,15 @@
         except:
             pass
         
         formatted_value = "'" + data.replace("'", "''") + "'"
         return formatted_value
 
     
+def formatter(data):
+    return ConsoleFormatter(data)
+
 def markdown(data):
     return ConsoleFormatter(data).to_table()
 
 def sql_insert(data, table_name):
     return ConsoleFormatter(data).to_sql(table_name)
```

### Comparing `tablepy_lib-0.6.0/PKG-INFO` & `tablepy_lib-0.7.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tablepy-lib
-Version: 0.6.0
+Version: 0.7.0
 Summary: This is a versatile and user-friendly Python table library that can quickly render any Dictionary{key, []} or DataFrame into a visually appealing markdown or sql insert
 Author: Jordi Corbilla
 Author-email: jordi.coll.corbilla@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -14,40 +14,50 @@
 # tablepy Lib
 
 This is a versatile and user-friendly Python table library that can quickly render any Dictionary{key, []} or DataFrame into a visually appealing markdown or sql insert
 
 ## Usage - Markdown
 
 ```python
+from tablepy_lib import markdown
+
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
     "Country": ["USA", "Canada", "UK", "DE"],
     "Data": ["USA", "Canada", "UK", "3434243"]
 }
 
-formatter = consoleFormatter(data)
-table = formatter.to_table()
+table = markdown(data)
 print(table)    
 ```
 
 Sample output:
 
 ```
 | Name    | Age      | Country   | Data      | 
 | ------- | -------- | --------- | --------- | 
 | John    | -28.0    | USA       | USA       | 
 | Emily   | 3002.6   | Canada    | Canada    | 
 | Tom     | 25.0     | UK        | UK        | 
 | JC      | 2.0      | DE        | 3434243   | 
 ```
 
+| Name    | Age      | Country   | Data      | 
+| ------- | -------- | --------- | --------- | 
+| John    | -28.0    | USA       | USA       | 
+| Emily   | 3002.6   | Canada    | Canada    | 
+| Tom     | 25.0     | UK        | UK        | 
+| JC      | 2.0      | DE        | 3434243   | 
+
 ## Usage - SQL Insert
 
 ```python
+from tablepy_lib import sql_insert
+
 data = {
     "Name": ["John", "Emily", "Tom", "JC"],
     "Age": [-28, 3002.6, 25, 2],
     "Country": ["USA", "Canada", "UK", "DE"],
     "Data": ["USA", "Canada", "UK", "3434243"]
 }
 
@@ -55,13 +65,14 @@
 table = sql_insert(data_frame, 'dd')
 print(table)
 
 ```
 
 Sample output:
 
-```
+```sql
 INSERT INTO dd (Name, Age, Country, Data) VALUES ('John', -28.0, 'USA', 'USA');
 INSERT INTO dd (Name, Age, Country, Data) VALUES ('Emily', 3002.6, 'Canada', 'Canada');
 INSERT INTO dd (Name, Age, Country, Data) VALUES ('Tom', 25.0, 'UK', 'UK');
 INSERT INTO dd (Name, Age, Country, Data) VALUES ('JC', 2.0, 'DE', 3434243);
 ```
+
```


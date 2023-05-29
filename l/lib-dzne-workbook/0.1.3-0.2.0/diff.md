# Comparing `tmp/lib-dzne-workbook-0.1.3.tar.gz` & `tmp/lib-dzne-workbook-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-workbook-0.1.3.tar", last modified: Wed Mar  1 23:18:56 2023, max compression
+gzip compressed data, was "lib-dzne-workbook-0.2.0.tar", last modified: Mon May 29 12:36:57 2023, max compression
```

## Comparing `lib-dzne-workbook-0.1.3.tar` & `lib-dzne-workbook-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-01 23:18:56.469203 lib-dzne-workbook-0.1.3/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-workbook-0.1.3/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1493 2023-03-01 23:18:56.469203 lib-dzne-workbook-0.1.3/PKG-INFO
--rw-r--r--   0 base      (1001) base      (1001)      558 2023-03-01 23:17:08.000000 lib-dzne-workbook-0.1.3/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-03-01 23:18:56.473204 lib-dzne-workbook-0.1.3/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-01 23:18:56.469203 lib-dzne-workbook-0.1.3/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-01 23:18:56.469203 lib-dzne-workbook-0.1.3/src/lib_dzne_workbook/
--rw-r--r--   0 base      (1001) base      (1001)     1699 2023-03-01 20:40:33.000000 lib-dzne-workbook-0.1.3/src/lib_dzne_workbook/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-01 23:18:56.469203 lib-dzne-workbook-0.1.3/src/lib_dzne_workbook.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1493 2023-03-01 23:18:56.000000 lib-dzne-workbook-0.1.3/src/lib_dzne_workbook.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      290 2023-03-01 23:18:56.000000 lib-dzne-workbook-0.1.3/src/lib_dzne_workbook.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-03-01 23:18:56.000000 lib-dzne-workbook-0.1.3/src/lib_dzne_workbook.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       31 2023-03-01 23:18:56.000000 lib-dzne-workbook-0.1.3/src/lib_dzne_workbook.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-03-01 23:18:56.000000 lib-dzne-workbook-0.1.3/src/lib_dzne_workbook.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:36:57.315720 lib-dzne-workbook-0.2.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-workbook-0.2.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1493 2023-05-29 12:36:57.315720 lib-dzne-workbook-0.2.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 12:22:38.000000 lib-dzne-workbook-0.2.0/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      583 2023-05-29 12:30:50.000000 lib-dzne-workbook-0.2.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 12:36:57.315720 lib-dzne-workbook-0.2.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:36:57.315720 lib-dzne-workbook-0.2.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:36:57.315720 lib-dzne-workbook-0.2.0/src/lib_dzne_workbook/
+-rw-rw-r--   0 base      (1001) base      (1001)     2405 2023-05-29 12:36:31.000000 lib-dzne-workbook-0.2.0/src/lib_dzne_workbook/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:36:57.315720 lib-dzne-workbook-0.2.0/src/lib_dzne_workbook.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1493 2023-05-29 12:36:57.000000 lib-dzne-workbook-0.2.0/src/lib_dzne_workbook.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 12:36:57.000000 lib-dzne-workbook-0.2.0/src/lib_dzne_workbook.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 12:36:57.000000 lib-dzne-workbook-0.2.0/src/lib_dzne_workbook.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       49 2023-05-29 12:36:57.000000 lib-dzne-workbook-0.2.0/src/lib_dzne_workbook.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 12:36:57.000000 lib-dzne-workbook-0.2.0/src/lib_dzne_workbook.egg-info/top_level.txt
```

### Comparing `lib-dzne-workbook-0.1.3/LICENSE` & `lib-dzne-workbook-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-workbook-0.1.3/PKG-INFO` & `lib-dzne-workbook-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-workbook
-Version: 0.1.3
+Version: 0.2.0
 Summary: Libary for handling workbooks. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-workbook-0.1.3/pyproject.toml` & `lib-dzne-workbook-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-workbook"
-version = "0.1.3"
+version = "0.2.0"
 description = "Libary for handling workbooks. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ['dzne']
 dependencies = [
     'pandas>=1.4.2',
     'openpyxl>=3.0.10',
+    'lib-dzne-filedata',
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-workbook-0.1.3/src/lib_dzne_workbook/__init__.py` & `lib-dzne-workbook-0.2.0/src/lib_dzne_workbook/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,56 +1,71 @@
-import openpyxl
-from openpyxl.styles import Alignment
+import math as _math
+import os as _os
 
-import math
-import pandas as pd
-import sys
-
-def default():
-    return openpyxl.Workbook()
-
-def from_file(file):
-    return openpyxl.load_workbook(file)
-
-def from_DataFrames(dataFrames):
-    dataFrames = dict(dataFrames)
-    if len(dataFrames) == 0:
-        return None
-    workbook = openpyxl.Workbook()
-    default_sheet = workbook.active
-    for table, df in dataFrames.items():
-        if default_sheet is None:
-            workbook.create_sheet(table)
+import lib_dzne_filedata as _fd
+import openpyxl as _xl
+import pandas as _pd
+
+
+class WorkbookData(_fd.FileData):
+    _ext = '.xlsx'
+    def __init__(self, workbook):
+        self.workbook = workbook
+    @classmethod
+    def _load(cls, /, file):
+        return _xl.load_workbook(file)
+    def _save(self, /, file):
+        self._workbook.save(filename=file)
+    @staticmethod
+    def _default():
+        return _xl.Workbook()
+    @classmethod
+    def clone_data(workbook):
+        with _tmp.TemporaryDirectory() as directory:
+            file = _os.path.join(directory, "a" + cls.ext())
+            workbook.save(file)
+            return _xl.load_workbook(file)
+    @staticmethod
+    def workbook_from_DataFrames(dataFrames):
+        dataFrames = dict(dataFrames)
+        if len(dataFrames) == 0:
+            return None
+        workbook = _xl.Workbook()
+        default_sheet = workbook.active
+        for table, df in dataFrames.items():
+            if default_sheet is None:
+                workbook.create_sheet(table)
+            else:
+                default_sheet.title = table
+                default_sheet = None
+        for table, df in dataFrames.items():
+            columns = list(df.columns)
+            for x, column in enumerate(columns):
+                workbook[table].cell(row=1, column=x+1).value = column
+                for y, v in enumerate(df[column].tolist()):
+                    if _pd.isna(v):
+                        continue
+                    elif (type(v) is float) and (_math.isinf(v)):# is this really needed?
+                        value = str(v)
+                    else:
+                        value = v
+                    workbook[table].cell(row=y+2, column=x+1).value = value
+        return workbook
+    @staticmethod
+    def set_cell(*, cell, value):
+        """Setting value of cell. """
+        if _pd.isna(value):
+            value = 'N/A'
         else:
-            default_sheet.title = table
-            default_sheet = None
-    for table, df in dataFrames.items():
-        columns = list(df.columns)
-        for x, column in enumerate(columns):
-            workbook[table].cell(row=1, column=x+1).value = column
-            for y, v in enumerate(df[column].tolist()):
-                if pd.isna(v):
-                    continue
-                elif (type(v) is float) and (math.isinf(v)):# is this really needed?
-                    value = str(v)
-                else:
-                    value = v
-                workbook[table].cell(row=y+2, column=x+1).value = value
-    return workbook
-
-def set_cell(*, cell, value):
-    """Setting value of cell. """
-    if pd.isna(value):
-        value = 'N/A'
-    else:
-        if type(value) is float:
-            if math.isinf(value):
-                if value < 0:
-                    value = '-inf'
-                else:
-                    value = '+inf'
-        if type(value) not in {str, int, float, bool}:
-            raise TypeError(f"The value {value} is of the invalid type {type(value)}! ")
-    cell.value = value
-    cell.alignment = Alignment()#horizontal='general')
+            if type(value) is float:
+                if _math.isinf(value):
+                    if value < 0:
+                        value = '-inf'
+                    else:
+                        value = '+inf'
+            if type(value) not in {str, int, float, bool}:
+                raise TypeError(f"The value {value} is of the invalid type {type(value)}! ")
+        cell.value = value
+        cell.alignment = _xl.styles.Alignment()#horizontal='general')
+
```

### Comparing `lib-dzne-workbook-0.1.3/src/lib_dzne_workbook.egg-info/PKG-INFO` & `lib-dzne-workbook-0.2.0/src/lib_dzne_workbook.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-workbook
-Version: 0.1.3
+Version: 0.2.0
 Summary: Libary for handling workbooks. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


# Comparing `tmp/lib-dzne-filedata-0.1.0.tar.gz` & `tmp/lib-dzne-filedata-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-filedata-0.1.0.tar", last modified: Mon May 29 08:51:40 2023, max compression
+gzip compressed data, was "lib-dzne-filedata-0.1.1.tar", last modified: Mon May 29 09:34:45 2023, max compression
```

## Comparing `lib-dzne-filedata-0.1.0.tar` & `lib-dzne-filedata-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.1.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      554 2023-05-29 08:50:54.000000 lib-dzne-filedata-0.1.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata/
--rw-r--r--   0 base      (1001) base      (1001)     9928 2023-05-29 08:50:04.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 08:51:40.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      290 2023-05-29 08:51:40.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 08:51:40.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       34 2023-05-29 08:51:40.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 08:51:40.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:34:45.579394 lib-dzne-filedata-0.1.1/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.1.1/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 09:34:45.579394 lib-dzne-filedata-0.1.1/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.1.1/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      661 2023-05-29 09:34:06.000000 lib-dzne-filedata-0.1.1/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 09:34:45.579394 lib-dzne-filedata-0.1.1/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:34:45.575394 lib-dzne-filedata-0.1.1/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:34:45.575394 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata/
+-rw-r--r--   0 base      (1001) base      (1001)     9909 2023-05-29 09:33:15.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:34:45.579394 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 09:34:45.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 09:34:45.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 09:34:45.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)      113 2023-05-29 09:34:45.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 09:34:45.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/top_level.txt
```

### Comparing `lib-dzne-filedata-0.1.0/LICENSE` & `lib-dzne-filedata-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-filedata-0.1.0/PKG-INFO` & `lib-dzne-filedata-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.1.0
+Version: 0.1.1
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-filedata-0.1.0/pyproject.toml` & `lib-dzne-filedata-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-filedata"
-version = "0.1.0"
+version = "0.1.1"
 description = "Libary for filedata handling. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
 dependencies = [
+    "Bio>=1.5.3",
     "pandas>=1.5.3",
-    "lib_dzne_seq>=0.2.0",
+    "lib-dzne-seq>=0.2.0",
+    "lib-dzne-basetables>=0.1.1",
+    "lib-dzne-tsv>=0.1.6",
+    "lib-dzne-math>=0.2.0",
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-filedata-0.1.0/src/lib_dzne_filedata/__init__.py` & `lib-dzne-filedata-0.1.1/src/lib_dzne_filedata/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import math as _math
 import os as _os
 import tempfile as _tmp
 import tomllib as _tomllib
 
 import Bio.Seq as _Seq
-import Bio.SeqIO as _SeqIO
-import Bio.SeqRecord as _SeqRecord
 import lib_dzne_basetables as _bt
+import lib_dzne_math.na as _na
+import lib_dzne_seq as _seq
 import lib_dzne_tsv as _tsv
 import lib_dzne_workbook as _wb
 import openpyxl as _xl
 import pandas as _pd
 import tomli_w as _tomli_w
-import lib_dzne_seq as _seq
 
 
 class _File:
     def __init__(self, *, fileDataType, string):
         fileDataType.check_ext(string)
         if not issubclass(fileDataType, FileData):
             raise TypeError()
@@ -215,15 +214,15 @@
                 target[k] = value
             else:
                 target = target[k]
     def items(self):
         return self.data.items()
     @classmethod
     def clone_data(cls, data):
-        if data is None:
+        if _na.isna(data):
             return float('nan')
         if type(data) in (str, int, bool, float):
             return data
         try:
             data = dict(data)
         except:
             pass
@@ -308,15 +307,15 @@
                         value = '+inf'
             if type(value) not in {str, int, float, bool}:
                 raise TypeError(f"The value {value} is of the invalid type {type(value)}! ")
         cell.value = value
         cell.alignment = _xl.styles.Alignment()#horizontal='general')
 
 
-class SeqReadData:
+class SeqReadData(FileData):
     @staticmethod
     def clone_data(data):
         return _seq.SeqRead(read=data)
     @classmethod
     def _load(cls, /, file):
         return _seq.SeqRead(file=file, format=cls._format)
     def _save(self, /, file):
```

### Comparing `lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/PKG-INFO` & `lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.1.0
+Version: 0.1.1
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


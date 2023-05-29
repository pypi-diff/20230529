# Comparing `tmp/lib-dzne-basetables-0.1.1.tar.gz` & `tmp/lib-dzne-basetables-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-basetables-0.1.1.tar", last modified: Sun Feb 19 01:26:41 2023, max compression
+gzip compressed data, was "lib-dzne-basetables-0.2.0.tar", last modified: Mon May 29 12:56:27 2023, max compression
```

## Comparing `lib-dzne-basetables-0.1.1.tar` & `lib-dzne-basetables-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 01:26:41.210360 lib-dzne-basetables-0.1.1/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.1.1/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-02-19 01:26:41.210360 lib-dzne-basetables-0.1.1/PKG-INFO
--rw-r--r--   0 base      (1001) base      (1001)      528 2023-02-19 01:25:13.000000 lib-dzne-basetables-0.1.1/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-02-19 01:26:41.210360 lib-dzne-basetables-0.1.1/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 01:26:41.206360 lib-dzne-basetables-0.1.1/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 01:26:41.206360 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables/
--rw-r--r--   0 base      (1001) base      (1001)       78 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables/__init__.py
--rw-r--r--   0 base      (1001) base      (1001)     2372 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables/baseconv.py
--rw-r--r--   0 base      (1001) base      (1001)      676 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables/common.py
--rw-r--r--   0 base      (1001) base      (1001)     1524 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables/pattern.py
--rw-r--r--   0 base      (1001) base      (1001)     7735 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables/table.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 01:26:41.210360 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-02-19 01:26:41.000000 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      440 2023-02-19 01:26:41.000000 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-02-19 01:26:41.000000 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       14 2023-02-19 01:26:41.000000 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-02-19 01:26:41.000000 lib-dzne-basetables-0.1.1/src/lib_dzne_basetables.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:56:27.476574 lib-dzne-basetables-0.2.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.2.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-05-29 12:56:27.476574 lib-dzne-basetables-0.2.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       22 2023-05-29 09:10:54.000000 lib-dzne-basetables-0.2.0/README.md
+-rw-r--r--   0 base      (1001) base      (1001)      528 2023-05-29 12:56:17.000000 lib-dzne-basetables-0.2.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 12:56:27.476574 lib-dzne-basetables-0.2.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:56:27.472574 lib-dzne-basetables-0.2.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:56:27.472574 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/
+-rw-r--r--   0 base      (1001) base      (1001)       54 2023-05-29 12:54:38.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/__init__.py
+-rw-r--r--   0 base      (1001) base      (1001)     2363 2023-05-29 12:47:17.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/baseconv.py
+-rw-r--r--   0 base      (1001) base      (1001)      675 2023-05-29 12:47:17.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/common.py
+-rw-rw-r--   0 base      (1001) base      (1001)     1241 2023-05-29 12:47:17.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/data.py
+-rw-r--r--   0 base      (1001) base      (1001)     1524 2023-02-19 00:26:57.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/pattern.py
+-rw-r--r--   0 base      (1001) base      (1001)     7732 2023-05-29 12:54:58.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/table.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:56:27.476574 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1487 2023-05-29 12:56:27.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      482 2023-05-29 12:56:27.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 12:56:27.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       14 2023-05-29 12:56:27.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 12:56:27.000000 lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/top_level.txt
```

### Comparing `lib-dzne-basetables-0.1.1/LICENSE` & `lib-dzne-basetables-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-basetables-0.1.1/PKG-INFO` & `lib-dzne-basetables-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-basetables
-Version: 0.1.1
+Version: 0.2.0
 Summary: Libary for basetables. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-basetables-0.1.1/pyproject.toml` & `lib-dzne-basetables-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-basetables"
-version = "0.1.1"
+version = "0.2.0"
 description = "Libary for basetables. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `lib-dzne-basetables-0.1.1/src/lib_dzne_basetables/baseconv.py` & `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/baseconv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 
-from collections import defaultdict
 import sys
+from collections import defaultdict
 
 from lib_dzne_basetables import common as _comm
 from lib_dzne_basetables import pattern as _pat
 from lib_dzne_basetables import table as _tbl
-        
 
 
 def a2d(table):
     """convert aTable to dTable"""
     table = _deconstruct_by_number(
         table, 
         purge=False,
```

### Comparing `lib-dzne-basetables-0.1.1/src/lib_dzne_basetables/common.py` & `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import sys
 
 
-
 def fuse(*dicts, reduce=False):
     assert reduce in (False, True)
     valuess = dict()
     for dB in dicts:
         for k, v in dB.items():
             if k not in valuess.keys():
                 valuess[k] = list()
```

### Comparing `lib-dzne-basetables-0.1.1/src/lib_dzne_basetables/pattern.py` & `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/pattern.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-basetables-0.1.1/src/lib_dzne_basetables/table.py` & `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables/table.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 # importing
-from collections import defaultdict
-import pandas as pd
 import string
 import sys
+from collections import defaultdict
 
+import pandas as pd
 
 import lib_dzne_basetables.common as _comm
 import lib_dzne_basetables.pattern as _pat
 
 
-
-
-
 def identify_columns(table, *, patterns):
     assert type(table) is pd.DataFrame
     return _pat.select(list(table.columns), patterns)
```

### Comparing `lib-dzne-basetables-0.1.1/src/lib_dzne_basetables.egg-info/PKG-INFO` & `lib-dzne-basetables-0.2.0/src/lib_dzne_basetables.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-basetables
-Version: 0.1.1
+Version: 0.2.0
 Summary: Libary for basetables. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


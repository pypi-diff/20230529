# Comparing `tmp/lib-dzne-tsv-0.1.6.tar.gz` & `tmp/lib-dzne-tsv-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-tsv-0.1.6.tar", last modified: Sun Apr 23 18:22:45 2023, max compression
+gzip compressed data, was "lib-dzne-tsv-0.2.0.tar", last modified: Mon May 29 12:42:13 2023, max compression
```

## Comparing `lib-dzne-tsv-0.1.6.tar` & `lib-dzne-tsv-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-tsv-0.1.6/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1472 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      522 2023-04-23 18:21:46.000000 lib-dzne-tsv-0.1.6/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv/
--rw-rw-r--   0 base      (1001) base      (1001)     5570 2023-04-23 18:17:57.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-04-23 18:22:45.518881 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1472 2023-04-23 18:22:45.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      260 2023-04-23 18:22:45.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-04-23 18:22:45.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       14 2023-04-23 18:22:45.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       13 2023-04-23 18:22:45.000000 lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:42:13.861493 lib-dzne-tsv-0.2.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-tsv-0.2.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1472 2023-05-29 12:42:13.861493 lib-dzne-tsv-0.2.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       15 2023-05-29 09:02:48.000000 lib-dzne-tsv-0.2.0/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      554 2023-05-29 12:40:01.000000 lib-dzne-tsv-0.2.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 12:42:13.861493 lib-dzne-tsv-0.2.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:42:13.861493 lib-dzne-tsv-0.2.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:42:13.861493 lib-dzne-tsv-0.2.0/src/lib_dzne_tsv/
+-rw-rw-r--   0 base      (1001) base      (1001)     6273 2023-05-29 12:11:29.000000 lib-dzne-tsv-0.2.0/src/lib_dzne_tsv/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:42:13.861493 lib-dzne-tsv-0.2.0/src/lib_dzne_tsv.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1472 2023-05-29 12:42:13.000000 lib-dzne-tsv-0.2.0/src/lib_dzne_tsv.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      270 2023-05-29 12:42:13.000000 lib-dzne-tsv-0.2.0/src/lib_dzne_tsv.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 12:42:13.000000 lib-dzne-tsv-0.2.0/src/lib_dzne_tsv.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       39 2023-05-29 12:42:13.000000 lib-dzne-tsv-0.2.0/src/lib_dzne_tsv.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       13 2023-05-29 12:42:13.000000 lib-dzne-tsv-0.2.0/src/lib_dzne_tsv.egg-info/top_level.txt
```

### Comparing `lib-dzne-tsv-0.1.6/LICENSE` & `lib-dzne-tsv-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-tsv-0.1.6/PKG-INFO` & `lib-dzne-tsv-0.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-tsv
-Version: 0.1.6
+Version: 0.2.0
 Summary: Libary for handling tsv-data. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-tsv-0.1.6/pyproject.toml` & `lib-dzne-tsv-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-tsv"
-version = "0.1.6"
+version = "0.2.0"
 description = "Libary for handling tsv-data. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
 dependencies = [
     'pandas>=1.4.2',
+    'lib-dzne-filedata>=0.4.0',
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-tsv-0.1.6/src/lib_dzne_tsv/__init__.py` & `lib-dzne-tsv-0.2.0/src/lib_dzne_tsv/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import csv as _csv
 import collections as _collections
-import pandas as _pd
 import contextlib as _contextlib
+import csv as _csv
+
+import lib_dzne_filedata as _fd
+import pandas as _pd
 
 
 def reader(target):
     return _csv.reader(target, dialect=Dialect)
 
 def writer(target):
     return _csv.writer(target, dialect=Dialect)
@@ -169,7 +171,29 @@
                     )
             if len(errors):
                 raise ExceptionGroup("Improper row! ", errors)
         values = [row[x] for x in self.fieldnames]
         self.use_handler(values)
 
 
+class TSVData(_fd.FileData):
+    _ext = '.tsv'
+    @classmethod
+    def _load(cls, /, file, *, strip=False, **kwargs):
+        ans = _tsv.read_DataFrame(file, **kwargs)
+        if strip:
+            ans = ans.applymap(lambda x: x.strip())
+        return cls(ans)
+    def _save(self, /, file, *, strip=False):
+        ans = self._dataFrame
+        if strip:
+            ans = ans.applymap(lambda x: x.strip())
+        _tsv.write_DataFrame(file, data)
+    @staticmethod
+    def _default():
+        return dict()
+    @staticmethod
+    def clone_data(data):
+        data = _pd.DataFrame(data)
+        data = data.copy()
+        data = data.applymap(str)
+        return data
```

### Comparing `lib-dzne-tsv-0.1.6/src/lib_dzne_tsv.egg-info/PKG-INFO` & `lib-dzne-tsv-0.2.0/src/lib_dzne_tsv.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-tsv
-Version: 0.1.6
+Version: 0.2.0
 Summary: Libary for handling tsv-data. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


# Comparing `tmp/lib-dzne-filedata-0.1.2.tar.gz` & `tmp/lib-dzne-filedata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-filedata-0.1.2.tar", last modified: Mon May 29 09:56:11 2023, max compression
+gzip compressed data, was "lib-dzne-filedata-0.2.0.tar", last modified: Mon May 29 10:34:06 2023, max compression
```

## Comparing `lib-dzne-filedata-0.1.2.tar` & `lib-dzne-filedata-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:56:11.992475 lib-dzne-filedata-0.1.2/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.1.2/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 09:56:11.992475 lib-dzne-filedata-0.1.2/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.1.2/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      661 2023-05-29 09:46:05.000000 lib-dzne-filedata-0.1.2/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 09:56:11.992475 lib-dzne-filedata-0.1.2/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:56:11.988475 lib-dzne-filedata-0.1.2/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:56:11.988475 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata/
--rw-r--r--   0 base      (1001) base      (1001)     9968 2023-05-29 09:50:20.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:56:11.992475 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 09:56:11.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 09:56:11.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 09:56:11.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)      113 2023-05-29 09:56:11.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 09:56:11.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.2.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.2.0/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      688 2023-05-29 10:29:47.000000 lib-dzne-filedata-0.2.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata/
+-rw-r--r--   0 base      (1001) base      (1001)    10217 2023-05-29 10:31:42.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 10:34:06.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 10:34:06.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 10:34:06.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)      133 2023-05-29 10:34:06.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 10:34:06.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/top_level.txt
```

### Comparing `lib-dzne-filedata-0.1.2/LICENSE` & `lib-dzne-filedata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-filedata-0.1.2/PKG-INFO` & `lib-dzne-filedata-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.1.2
+Version: 0.2.0
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-filedata-0.1.2/pyproject.toml` & `lib-dzne-filedata-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-filedata"
-version = "0.1.2"
+version = "0.2.0"
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
-    "Bio>=1.5.3",
+    "openpyxl>=3.1.1",
     "pandas>=1.5.3",
+    "tomli_w>=1.0.0",
     "lib-dzne-seq>=0.2.0",
     "lib-dzne-basetables>=0.1.1",
     "lib-dzne-tsv>=0.1.6",
     "lib-dzne-math>=0.2.0",
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-filedata-0.1.2/src/lib_dzne_filedata/__init__.py` & `lib-dzne-filedata-0.2.0/src/lib_dzne_filedata/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import math as _math
 import os as _os
 import tempfile as _tmp
 import tomllib as _tomllib
 
-import Bio.Seq as _Seq
 import lib_dzne_basetables as _bt
 import lib_dzne_math.na as _na
 import lib_dzne_seq as _seq
 import lib_dzne_tsv as _tsv
-import lib_dzne_workbook as _wb
 import openpyxl as _xl
 import pandas as _pd
 import tomli_w as _tomli_w
 
 
 class _File:
     def __init__(self, *, fileDataType, string):
@@ -50,50 +48,45 @@
     @classmethod
     def check_ext(cls, /, file):
         if cls._ext is None:
             return
         if cls._ext == _os.path.splitext(file):
             return
         raise ValueError()
-
     @classmethod
     def load(cls, /, file, **kwargs):
         if file == "":
             ans = cls._default()
         else:
             cls.check_ext(file)
             ans = cls._load(file=file, **kwargs)
         return cls(ans)
-
     def save(self, /, file, *, overwrite=False, **kwargs):
         cls = type(self)
         if file == "":
             ans = type(self).drop()
         elif _os.path.exists(file) and not overwrite:
             raise FileExistsError(file)
         else:
             cls.check_ext(file)
             ans = self._save(file=file, **kwargs)
         if ans is not None:
             raise TypeError()
-
     @classmethod
     def from_file(cls, file, /, *types):
         ext = _os.path.splitext(file)
         for t in types:
             if not issubclass(t, cls):
                 raise ValueError()
             if t._ext == ext:
                 return t.load(file)
         raise ValueError()
-
     @classmethod
     def default(cls):
         return cls.load("")
-
     @property
     def data(self):
         return type(self).clone_data(self._data)
     @data.setter
     def data(self, value):
         self._data = type(self).clone_data(self._data)
 
@@ -186,40 +179,50 @@
     _ext = ".ybase"
 
 class TOMLData(FileData):
     _ext = ".toml"
     def __init__(self, data):
         self.data = data
     def __getitem__(self, key):
-        if type(key) is tuple:
-            keys = key
-        else:
-            keys = key,
-        keytypes = {list:int, dict:str}
-        target = self._data
-        for i, key in enumerate(keys):
-            k = keytypes[type(target)](key)
-            target = target[k]
-        return self.clone_data(target)
+        keys = self._getkeys(key)
+        ans = self._getitem(*keys)
+        ans = self.clone_data(ans)
+        return ans
     def __setitem__(self, key, value):
+        value = self.clone_data(value)
+        keys = self._getkeys(key)
+        target = self._getitem(*(keys[:-1]))
+        if (type(target) is dict) and (type(keys[-1]) is not str):
+            raise TypeError()
+        target[keys[-1]] = value
+    def __delitem__(self, key):
+        keys = self._getkeys(key)
+        target = self._getitem(*(keys[:-1]))
+        del target[keys[-1]]
+    @staticmethod
+    def _getkeys(key):
         if type(key) is tuple:
-            keys = key
+            return key
         else:
-            keys = key,
-        value = self.clone_data(value)
-        keytypes = {list:int, dict:str}
+            return key,
+    def _getitem(self, *keys):
         target = self._data
-        for i, key in enumerate(keys):
-            k = keytypes[type(target)](key)
-            if i == len(keys) - 1:
-                target[k] = value
-            else:
-                target = target[k]
-    def items(self):
-        return self.data.items()
+        for key in keys:
+            target = target[key]
+        return target
+    def items(self, *keys):
+        return self[keys].items()
+    def append(self, *args):
+        *keys, value = args
+        self._getitem(*keys).append(value)
+    def get(self, *keys, default=None):
+        try:
+            return self[keys]
+        except KeyError:
+            return default
     @classmethod
     def clone_data(cls, data):
         if _na.isna(data):
             return float('nan')
         if type(data) in (str, int, bool, float):
             return data
         if data == str(data):
```

### Comparing `lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/PKG-INFO` & `lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.1.2
+Version: 0.2.0
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


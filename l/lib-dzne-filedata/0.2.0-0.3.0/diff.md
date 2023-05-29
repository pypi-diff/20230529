# Comparing `tmp/lib-dzne-filedata-0.2.0.tar.gz` & `tmp/lib-dzne-filedata-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-filedata-0.2.0.tar", last modified: Mon May 29 10:34:06 2023, max compression
+gzip compressed data, was "lib-dzne-filedata-0.3.0.tar", last modified: Mon May 29 11:45:23 2023, max compression
```

## Comparing `lib-dzne-filedata-0.2.0.tar` & `lib-dzne-filedata-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.2.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.2.0/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      688 2023-05-29 10:29:47.000000 lib-dzne-filedata-0.2.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata/
--rw-r--r--   0 base      (1001) base      (1001)    10217 2023-05-29 10:31:42.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:34:06.437254 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 10:34:06.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 10:34:06.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 10:34:06.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)      133 2023-05-29 10:34:06.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 10:34:06.000000 lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 11:45:23.321675 lib-dzne-filedata-0.3.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.3.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 11:45:23.321675 lib-dzne-filedata-0.3.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.3.0/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      688 2023-05-29 11:44:26.000000 lib-dzne-filedata-0.3.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 11:45:23.321675 lib-dzne-filedata-0.3.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 11:45:23.317675 lib-dzne-filedata-0.3.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 11:45:23.317675 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata/
+-rw-r--r--   0 base      (1001) base      (1001)    11182 2023-05-29 11:38:03.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 11:45:23.321675 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 11:45:23.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 11:45:23.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 11:45:23.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)      133 2023-05-29 11:45:23.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 11:45:23.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/top_level.txt
```

### Comparing `lib-dzne-filedata-0.2.0/LICENSE` & `lib-dzne-filedata-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-filedata-0.2.0/PKG-INFO` & `lib-dzne-filedata-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.2.0
+Version: 0.3.0
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-filedata-0.2.0/pyproject.toml` & `lib-dzne-filedata-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-filedata"
-version = "0.2.0"
+version = "0.3.0"
 description = "Libary for filedata handling. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `lib-dzne-filedata-0.2.0/src/lib_dzne_filedata/__init__.py` & `lib-dzne-filedata-0.3.0/src/lib_dzne_filedata/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -176,16 +176,14 @@
 class MBASEData(BASEData):
     _ext = ".mbase"
 class YBASEData(BASEData):
     _ext = ".ybase"
 
 class TOMLData(FileData):
     _ext = ".toml"
-    def __init__(self, data):
-        self.data = data
     def __getitem__(self, key):
         keys = self._getkeys(key)
         ans = self._getitem(*keys)
         ans = self.clone_data(ans)
         return ans
     def __setitem__(self, key, value):
         value = self.clone_data(value)
@@ -194,14 +192,31 @@
         if (type(target) is dict) and (type(keys[-1]) is not str):
             raise TypeError()
         target[keys[-1]] = value
     def __delitem__(self, key):
         keys = self._getkeys(key)
         target = self._getitem(*(keys[:-1]))
         del target[keys[-1]]
+    def __add__(self, other):
+        if type(self) is not type(other):
+            other = type(self)(other)
+        return self._add(self, other)
+    def __radd__(self, other):
+        return self.__add__(other)
+
+    @classmethod
+    def _add(cls, *objs):
+        ans = cls.default()
+        for obj in objs:
+            for k, v in obj.iteritems():
+                if ans.get(*k) is None:
+                    ans[k] = v
+                else:
+                    raise KeyError()
+        return ans
     @staticmethod
     def _getkeys(key):
         if type(key) is tuple:
             return key
         else:
             return key,
     def _getitem(self, *keys):
@@ -215,16 +230,34 @@
         *keys, value = args
         self._getitem(*keys).append(value)
     def get(self, *keys, default=None):
         try:
             return self[keys]
         except KeyError:
             return default
+    def iteritems(self):
+        return self._iteritems(self.data)
+    @classmethod
+    def _iteritems(cls, data):
+        gen = None
+        if type(data) is list:
+            gen = enumerate(data)
+        elif type(data) is dict:
+            gen = data.items()
+        else:
+            yield (tuple(), data)
+            return
+        for k, v in gen:
+            for keys, value in cls._iteritems(v):
+                yield ((k,) + keys), value
+
     @classmethod
     def clone_data(cls, data):
+        if issubclass(type(data), cls):
+            data = data._data
         if _na.isna(data):
             return float('nan')
         if type(data) in (str, int, bool, float):
             return data
         if data == str(data):
             return str(data)
         try:
```

### Comparing `lib-dzne-filedata-0.2.0/src/lib_dzne_filedata.egg-info/PKG-INFO` & `lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.2.0
+Version: 0.3.0
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


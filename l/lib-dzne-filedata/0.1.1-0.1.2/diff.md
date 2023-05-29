# Comparing `tmp/lib-dzne-filedata-0.1.1.tar.gz` & `tmp/lib-dzne-filedata-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-filedata-0.1.1.tar", last modified: Mon May 29 09:34:45 2023, max compression
+gzip compressed data, was "lib-dzne-filedata-0.1.2.tar", last modified: Mon May 29 09:56:11 2023, max compression
```

## Comparing `lib-dzne-filedata-0.1.1.tar` & `lib-dzne-filedata-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:34:45.579394 lib-dzne-filedata-0.1.1/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.1.1/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 09:34:45.579394 lib-dzne-filedata-0.1.1/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.1.1/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      661 2023-05-29 09:34:06.000000 lib-dzne-filedata-0.1.1/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 09:34:45.579394 lib-dzne-filedata-0.1.1/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:34:45.575394 lib-dzne-filedata-0.1.1/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:34:45.575394 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata/
--rw-r--r--   0 base      (1001) base      (1001)     9909 2023-05-29 09:33:15.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:34:45.579394 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 09:34:45.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 09:34:45.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 09:34:45.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)      113 2023-05-29 09:34:45.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 09:34:45.000000 lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:56:11.992475 lib-dzne-filedata-0.1.2/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.1.2/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 09:56:11.992475 lib-dzne-filedata-0.1.2/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.1.2/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      661 2023-05-29 09:46:05.000000 lib-dzne-filedata-0.1.2/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 09:56:11.992475 lib-dzne-filedata-0.1.2/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:56:11.988475 lib-dzne-filedata-0.1.2/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:56:11.988475 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata/
+-rw-r--r--   0 base      (1001) base      (1001)     9968 2023-05-29 09:50:20.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:56:11.992475 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 09:56:11.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 09:56:11.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 09:56:11.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)      113 2023-05-29 09:56:11.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 09:56:11.000000 lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/top_level.txt
```

### Comparing `lib-dzne-filedata-0.1.1/LICENSE` & `lib-dzne-filedata-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-filedata-0.1.1/PKG-INFO` & `lib-dzne-filedata-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-filedata-0.1.1/pyproject.toml` & `lib-dzne-filedata-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-filedata"
-version = "0.1.1"
+version = "0.1.2"
 description = "Libary for filedata handling. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `lib-dzne-filedata-0.1.1/src/lib_dzne_filedata/__init__.py` & `lib-dzne-filedata-0.1.2/src/lib_dzne_filedata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,14 +218,16 @@
         return self.data.items()
     @classmethod
     def clone_data(cls, data):
         if _na.isna(data):
             return float('nan')
         if type(data) in (str, int, bool, float):
             return data
+        if data == str(data):
+            return str(data)
         try:
             data = dict(data)
         except:
             pass
         else:
             keys = list(data.keys())
             for k in keys:
```

### Comparing `lib-dzne-filedata-0.1.1/src/lib_dzne_filedata.egg-info/PKG-INFO` & `lib-dzne-filedata-0.1.2/src/lib_dzne_filedata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.1.1
+Version: 0.1.2
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


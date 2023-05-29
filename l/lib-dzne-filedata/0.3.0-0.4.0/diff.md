# Comparing `tmp/lib-dzne-filedata-0.3.0.tar.gz` & `tmp/lib-dzne-filedata-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-filedata-0.3.0.tar", last modified: Mon May 29 11:45:23 2023, max compression
+gzip compressed data, was "lib-dzne-filedata-0.4.0.tar", last modified: Mon May 29 12:33:02 2023, max compression
```

## Comparing `lib-dzne-filedata-0.3.0.tar` & `lib-dzne-filedata-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 11:45:23.321675 lib-dzne-filedata-0.3.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.3.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 11:45:23.321675 lib-dzne-filedata-0.3.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.3.0/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      688 2023-05-29 11:44:26.000000 lib-dzne-filedata-0.3.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 11:45:23.321675 lib-dzne-filedata-0.3.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 11:45:23.317675 lib-dzne-filedata-0.3.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 11:45:23.317675 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata/
--rw-r--r--   0 base      (1001) base      (1001)    11182 2023-05-29 11:38:03.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 11:45:23.321675 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 11:45:23.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 11:45:23.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 11:45:23.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)      133 2023-05-29 11:45:23.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 11:45:23.000000 lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:33:02.670066 lib-dzne-filedata-0.4.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.4.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 12:33:02.670066 lib-dzne-filedata-0.4.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 09:06:58.000000 lib-dzne-filedata-0.4.0/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      556 2023-05-29 12:32:04.000000 lib-dzne-filedata-0.4.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 12:33:02.670066 lib-dzne-filedata-0.4.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:33:02.666066 lib-dzne-filedata-0.4.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:33:02.666066 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata/
+-rw-r--r--   0 base      (1001) base      (1001)     7233 2023-05-29 12:30:10.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:33:02.670066 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 12:33:02.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      300 2023-05-29 12:33:02.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 12:33:02.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       36 2023-05-29 12:33:02.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 12:33:02.000000 lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/top_level.txt
```

### Comparing `lib-dzne-filedata-0.3.0/LICENSE` & `lib-dzne-filedata-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-filedata-0.3.0/PKG-INFO` & `lib-dzne-filedata-0.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.3.0
+Version: 0.4.0
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-filedata-0.3.0/pyproject.toml` & `lib-dzne-filedata-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-filedata"
-version = "0.3.0"
+version = "0.4.0"
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
-    "openpyxl>=3.1.1",
-    "pandas>=1.5.3",
     "tomli_w>=1.0.0",
-    "lib-dzne-seq>=0.2.0",
-    "lib-dzne-basetables>=0.1.1",
-    "lib-dzne-tsv>=0.1.6",
     "lib-dzne-math>=0.2.0",
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-filedata-0.3.0/src/lib_dzne_filedata.egg-info/PKG-INFO` & `lib-dzne-filedata-0.4.0/src/lib_dzne_filedata.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.3.0
+Version: 0.4.0
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


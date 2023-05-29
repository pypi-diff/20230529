# Comparing `tmp/lib-dzne-filedata-0.0.0.tar.gz` & `tmp/lib-dzne-filedata-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-filedata-0.0.0.tar", last modified: Sun May 28 21:19:42 2023, max compression
+gzip compressed data, was "lib-dzne-filedata-0.1.0.tar", last modified: Mon May 29 08:51:40 2023, max compression
```

## Comparing `lib-dzne-filedata-0.0.0.tar` & `lib-dzne-filedata-0.1.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-28 21:19:42.243499 lib-dzne-filedata-0.0.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.0.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-28 21:19:42.243499 lib-dzne-filedata-0.0.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      506 2023-05-28 21:08:41.000000 lib-dzne-filedata-0.0.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-28 21:19:42.243499 lib-dzne-filedata-0.0.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-28 21:19:42.243499 lib-dzne-filedata-0.0.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-28 21:19:42.243499 lib-dzne-filedata-0.0.0/src/lib_dzne_filedata/
--rw-r--r--   0 base      (1001) base      (1001)      475 2023-05-28 21:18:39.000000 lib-dzne-filedata-0.0.0/src/lib_dzne_filedata/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-28 21:19:42.243499 lib-dzne-filedata-0.0.0/src/lib_dzne_filedata.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-28 21:19:42.000000 lib-dzne-filedata-0.0.0/src/lib_dzne_filedata.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      246 2023-05-28 21:19:42.000000 lib-dzne-filedata-0.0.0/src/lib_dzne_filedata.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-28 21:19:42.000000 lib-dzne-filedata-0.0.0/src/lib_dzne_filedata.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-28 21:19:42.000000 lib-dzne-filedata-0.0.0/src/lib_dzne_filedata.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-filedata-0.1.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      554 2023-05-29 08:50:54.000000 lib-dzne-filedata-0.1.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata/
+-rw-r--r--   0 base      (1001) base      (1001)     9928 2023-05-29 08:50:04.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 08:51:40.274705 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1477 2023-05-29 08:51:40.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      290 2023-05-29 08:51:40.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 08:51:40.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       34 2023-05-29 08:51:40.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 08:51:40.000000 lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/top_level.txt
```

### Comparing `lib-dzne-filedata-0.0.0/LICENSE` & `lib-dzne-filedata-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-filedata-0.0.0/PKG-INFO` & `lib-dzne-filedata-0.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.0.0
+Version: 0.1.0
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-filedata-0.0.0/src/lib_dzne_filedata.egg-info/PKG-INFO` & `lib-dzne-filedata-0.1.0/src/lib_dzne_filedata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-filedata
-Version: 0.0.0
+Version: 0.1.0
 Summary: Libary for filedata handling. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


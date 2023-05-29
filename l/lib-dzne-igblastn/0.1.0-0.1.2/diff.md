# Comparing `tmp/lib-dzne-igblastn-0.1.0.tar.gz` & `tmp/lib-dzne-igblastn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-igblastn-0.1.0.tar", last modified: Wed Mar  1 22:59:18 2023, max compression
+gzip compressed data, was "lib-dzne-igblastn-0.1.2.tar", last modified: Mon May 29 10:41:24 2023, max compression
```

## Comparing `lib-dzne-igblastn-0.1.0.tar` & `lib-dzne-igblastn-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-01 22:59:18.069672 lib-dzne-igblastn-0.1.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-igblastn-0.1.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-03-01 22:59:18.069672 lib-dzne-igblastn-0.1.0/PKG-INFO
--rw-r--r--   0 base      (1001) base      (1001)      530 2023-03-01 20:28:52.000000 lib-dzne-igblastn-0.1.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-03-01 22:59:18.069672 lib-dzne-igblastn-0.1.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-01 22:59:18.065671 lib-dzne-igblastn-0.1.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-01 22:59:18.069672 lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn/
--rw-r--r--   0 base      (1001) base      (1001)     9285 2023-03-01 20:28:52.000000 lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn/Parser.py
--rw-r--r--   0 base      (1001) base      (1001)      849 2023-03-01 20:28:52.000000 lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-03-01 22:59:18.069672 lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-03-01 22:59:18.000000 lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      322 2023-03-01 22:59:18.000000 lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-03-01 22:59:18.000000 lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-03-01 22:59:18.000000 lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-03-01 22:59:18.000000 lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-igblastn-0.1.2/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 10:37:39.000000 lib-dzne-igblastn-0.1.2/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      530 2023-05-29 10:38:31.000000 lib-dzne-igblastn-0.1.2/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/
+-rw-rw-r--   0 base      (1001) base      (1001)     9305 2023-05-29 10:40:18.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/Parser.py
+-rw-rw-r--   0 base      (1001) base      (1001)       87 2023-03-18 23:05:52.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/__init__.py
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-05-01 18:48:23.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/functions.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-05-29 10:41:24.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      367 2023-05-29 10:41:24.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 10:41:24.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 10:41:24.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 10:41:24.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/top_level.txt
```

### Comparing `lib-dzne-igblastn-0.1.0/LICENSE` & `lib-dzne-igblastn-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-igblastn-0.1.0/PKG-INFO` & `lib-dzne-igblastn-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-igblastn
-Version: 0.1.0
+Version: 0.1.2
 Summary: Libary for using igblastn. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-igblastn-0.1.0/pyproject.toml` & `lib-dzne-igblastn-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-igblastn"
-version = "0.1.0"
+version = "0.1.2"
 description = "Libary for using igblastn. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
 dependencies = [
-    'lib_dzne_tsv>=0.1.1',
+    'lib-dzne-tsv>=0.1.4',
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn/Parser.py` & `lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/Parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 
-import string
-import os
-import shutil
-import lib_dzne_tsv
+import string as _string
+import os as _os
+import lib_dzne_tsv as _tsv
  
 
 
 class Parser:
     class Error(ValueError):
         pass
     def parse_text(text):
@@ -38,15 +37,15 @@
         if sharp:
             line = line.strip()
             #if line == "#":
             #    return ""
             #Parser.check(line.startswith("# ")
             return line[1:]
         if tab:
-            ans, = (x for x in lib_dzne_tsv.reader([line.strip()]))
+            ans, = (x for x in _tsv.reader([line.strip()]))
             return ans
         Parser.check(line.startswith("Total"), "Lines that do not start with '#' or contain tabs start with 'Total'!")
         k, v = [x.strip() for x in line.split('=')]# and contain exactly one '='! 
         return (k, int(v))
     def get_chunks_from_lines(lines):
         chunk = None
         for line in lines:
@@ -65,38 +64,35 @@
         if phrase is None:
             return None
         phrase = phrase.strip()
         phrase = phrase.lower()
         phrase = phrase.replace('%', 'percent')
         ans = ""
         for ch in phrase:
-            if ch in (string.ascii_lowercase + string.digits):
+            if ch in (_string.ascii_lowercase + _string.digits):
                 ans += ch
             else:
                 ans += '-'
         return ans.strip('-')
     def get_header_from_description(description, *, width):
-        Parser.check(2 <= width, "A table must have at least to columns! ")
+        Parser.check(2 <= width, "A table must have at least two columns! ")
         for ch in [':', '(', ')']:
             description = description.replace(ch, '\n')
         headers = list()
         for splinter in description.split('\n'):
             part = splinter.strip(" ,")
-            prose = False
             for phrase in ['i.e', ', or', ', and']:
                 if phrase in part:
-                    prose = True
                     break
-            if prose:
-                continue
-            header = part.split(',')
-            if (width == len(header) + 1):
-                header = [None] + header
-            if (width == len(header)):
-                headers.append(header)
+            else:
+                header = part.split(',')
+                if (width == len(header) + 1):
+                    header = [None] + header
+                if (width == len(header)):
+                    headers.append(header)
         header, = headers
         header = [Parser.parse_key(col) for col in header]
         Parser.check(len(set(header)) == width, "The name of each column must be unique! ")
         return header
     def parse_blocks(blocks):
         ans = {
             'texts': list(),
@@ -219,22 +215,23 @@
                 'sub-region sequence details',
                 'alignment summary',
                 'hit table',
             ]
             sign, = [s for s in signs if (s in _description)]
             self._name = sign.split(' ')[0]
             header = Parser.get_header_from_description(description, width=width)
+            dictReader = _tsv.DictReader(iter(rows), fieldnames=header)
             if None in header:
                 body = dict()
             else:
                 body = list()
             dtss = Parser.TabBlock._get_datatypess()
-            for row in rows:
+            for dictrow in dictReader:
                 tablerow = dict()
-                for col, elem in zip(header, row):
+                for col, elem in dictrow.items():
                     dt = dtss[self._name][col]
                     tablerow[col] = Parser.parse_value(elem, dt)
                 if None in header:
                     index = Parser.parse_key(tablerow.pop(None))
                     if index not in body.keys():
                         body[index] = list()
                     body[index].append(tablerow)
```

### Comparing `lib-dzne-igblastn-0.1.0/src/lib_dzne_igblastn.egg-info/PKG-INFO` & `lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-igblastn
-Version: 0.1.0
+Version: 0.1.2
 Summary: Libary for using igblastn. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


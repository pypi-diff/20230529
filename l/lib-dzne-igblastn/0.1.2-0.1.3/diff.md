# Comparing `tmp/lib-dzne-igblastn-0.1.2.tar.gz` & `tmp/lib-dzne-igblastn-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-igblastn-0.1.2.tar", last modified: Mon May 29 10:41:24 2023, max compression
+gzip compressed data, was "lib-dzne-igblastn-0.1.3.tar", last modified: Mon May 29 13:36:59 2023, max compression
```

## Comparing `lib-dzne-igblastn-0.1.2.tar` & `lib-dzne-igblastn-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-igblastn-0.1.2/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 10:37:39.000000 lib-dzne-igblastn-0.1.2/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      530 2023-05-29 10:38:31.000000 lib-dzne-igblastn-0.1.2/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/
--rw-rw-r--   0 base      (1001) base      (1001)     9305 2023-05-29 10:40:18.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/Parser.py
--rw-rw-r--   0 base      (1001) base      (1001)       87 2023-03-18 23:05:52.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/__init__.py
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-05-01 18:48:23.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/functions.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 10:41:24.713622 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-05-29 10:41:24.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      367 2023-05-29 10:41:24.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 10:41:24.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 10:41:24.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 10:41:24.000000 lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:36:59.278564 lib-dzne-igblastn-0.1.3/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-igblastn-0.1.3/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-05-29 13:36:59.278564 lib-dzne-igblastn-0.1.3/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 10:37:39.000000 lib-dzne-igblastn-0.1.3/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      530 2023-05-29 13:36:39.000000 lib-dzne-igblastn-0.1.3/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 13:36:59.278564 lib-dzne-igblastn-0.1.3/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:36:59.274564 lib-dzne-igblastn-0.1.3/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:36:59.274564 lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn/
+-rw-rw-r--   0 base      (1001) base      (1001)     9304 2023-05-29 12:47:17.000000 lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn/Parser.py
+-rw-rw-r--   0 base      (1001) base      (1001)       86 2023-05-29 12:47:17.000000 lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn/__init__.py
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-05-29 12:47:17.000000 lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn/functions.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:36:59.278564 lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-05-29 13:36:59.000000 lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      367 2023-05-29 13:36:59.000000 lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 13:36:59.000000 lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 13:36:59.000000 lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 13:36:59.000000 lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn.egg-info/top_level.txt
```

### Comparing `lib-dzne-igblastn-0.1.2/LICENSE` & `lib-dzne-igblastn-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-igblastn-0.1.2/PKG-INFO` & `lib-dzne-igblastn-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-igblastn
-Version: 0.1.2
+Version: 0.1.3
 Summary: Libary for using igblastn. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-igblastn-0.1.2/pyproject.toml` & `lib-dzne-igblastn-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-igblastn"
-version = "0.1.2"
+version = "0.1.3"
 description = "Libary for using igblastn. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/Parser.py` & `lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn/Parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
-import string as _string
 import os as _os
+import string as _string
+
 import lib_dzne_tsv as _tsv
- 
 
 
 class Parser:
     class Error(ValueError):
         pass
     def parse_text(text):
         lines = [Parser.parse_line(line) for line in text.split('\n')]
```

### Comparing `lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn/functions.py` & `lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn/functions.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 
+import contextlib as _contextlib
 import os as _os
 import shutil as _shutil
-import contextlib as _contextlib
 import tempfile as _tempfile
 
 
 def get_cline(
     prog,
     *, 
     query,
```

### Comparing `lib-dzne-igblastn-0.1.2/src/lib_dzne_igblastn.egg-info/PKG-INFO` & `lib-dzne-igblastn-0.1.3/src/lib_dzne_igblastn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-igblastn
-Version: 0.1.2
+Version: 0.1.3
 Summary: Libary for using igblastn. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


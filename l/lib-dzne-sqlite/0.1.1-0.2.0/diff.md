# Comparing `tmp/lib-dzne-sqlite-0.1.1.tar.gz` & `tmp/lib-dzne-sqlite-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-sqlite-0.1.1.tar", last modified: Sun Feb 19 09:24:24 2023, max compression
+gzip compressed data, was "lib-dzne-sqlite-0.2.0.tar", last modified: Mon May 29 14:14:35 2023, max compression
```

## Comparing `lib-dzne-sqlite-0.1.1.tar` & `lib-dzne-sqlite-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:24:24.211216 lib-dzne-sqlite-0.1.1/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-19 00:26:57.000000 lib-dzne-sqlite-0.1.1/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1473 2023-02-19 09:24:24.211216 lib-dzne-sqlite-0.1.1/PKG-INFO
--rw-r--r--   0 base      (1001) base      (1001)      523 2023-02-19 09:09:38.000000 lib-dzne-sqlite-0.1.1/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-02-19 09:24:24.211216 lib-dzne-sqlite-0.1.1/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:24:24.207213 lib-dzne-sqlite-0.1.1/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:24:24.211216 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite/
--rw-r--r--   0 base      (1001) base      (1001)     1442 2023-02-19 00:26:57.000000 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite/Where.py
--rw-r--r--   0 base      (1001) base      (1001)        2 2023-02-19 00:26:57.000000 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite/__init__.py
--rw-r--r--   0 base      (1001) base      (1001)      450 2023-02-19 00:26:57.000000 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite/cmd.py
--rw-r--r--   0 base      (1001) base      (1001)     3063 2023-02-19 00:26:57.000000 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite/exec.py
--rw-r--r--   0 base      (1001) base      (1001)      464 2023-02-19 00:26:57.000000 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite/fmt.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:24:24.211216 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1473 2023-02-19 09:24:24.000000 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      389 2023-02-19 09:24:24.000000 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-02-19 09:24:24.000000 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       14 2023-02-19 09:24:24.000000 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       16 2023-02-19 09:24:24.000000 lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:14:35.736520 lib-dzne-sqlite-0.2.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-sqlite-0.2.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1473 2023-05-29 14:14:35.736520 lib-dzne-sqlite-0.2.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-05-29 14:13:11.000000 lib-dzne-sqlite-0.2.0/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      523 2023-05-29 14:13:29.000000 lib-dzne-sqlite-0.2.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 14:14:35.736520 lib-dzne-sqlite-0.2.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:14:35.732520 lib-dzne-sqlite-0.2.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:14:35.736520 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite/
+-rw-r--r--   0 base      (1001) base      (1001)     1444 2023-05-29 12:47:17.000000 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite/Where.py
+-rw-rw-r--   0 base      (1001) base      (1001)        2 2023-03-18 23:05:52.000000 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite/__init__.py
+-rw-r--r--   0 base      (1001) base      (1001)      451 2023-05-29 12:47:17.000000 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite/cmd.py
+-rw-r--r--   0 base      (1001) base      (1001)     3050 2023-05-29 12:47:17.000000 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite/exec.py
+-rw-r--r--   0 base      (1001) base      (1001)      465 2023-05-29 12:47:17.000000 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite/fmt.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:14:35.736520 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1473 2023-05-29 14:14:35.000000 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      399 2023-05-29 14:14:35.000000 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 14:14:35.000000 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       14 2023-05-29 14:14:35.000000 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       16 2023-05-29 14:14:35.000000 lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite.egg-info/top_level.txt
```

### Comparing `lib-dzne-sqlite-0.1.1/LICENSE` & `lib-dzne-sqlite-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-sqlite-0.1.1/PKG-INFO` & `lib-dzne-sqlite-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-sqlite
-Version: 0.1.1
+Version: 0.2.0
 Summary: Libary for handling sqlite. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-sqlite-0.1.1/pyproject.toml` & `lib-dzne-sqlite-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-sqlite"
-version = "0.1.1"
+version = "0.2.0"
 description = "Libary for handling sqlite. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite/Where.py` & `lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite/Where.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import pandas as pd
+
 from . import fmt
 
+
 class Where:
     def __str__(self):
         return self.command
     @property
     def command(self):
         return self._command
     @property
```

### Comparing `lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite/exec.py` & `lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite/exec.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import sys
-import pandas as pd
-from . import fmt
-from . import cmd
-from .Where import Where
 
+import pandas as pd
 
+from . import cmd, fmt
+from .Where import Where
 
 
 def _cursor_decorator(oldfunc):
     def newfunc(*, cursor, **kwargs):
         command, values = oldfunc(**kwargs)
         _main(
             cursor=cursor,
```

### Comparing `lib-dzne-sqlite-0.1.1/src/lib_dzne_sqlite.egg-info/PKG-INFO` & `lib-dzne-sqlite-0.2.0/src/lib_dzne_sqlite.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-sqlite
-Version: 0.1.1
+Version: 0.2.0
 Summary: Libary for handling sqlite. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


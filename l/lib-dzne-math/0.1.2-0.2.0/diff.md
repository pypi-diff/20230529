# Comparing `tmp/lib-dzne-math-0.1.2.tar.gz` & `tmp/lib-dzne-math-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-math-0.1.2.tar", last modified: Sun Feb 19 09:35:40 2023, max compression
+gzip compressed data, was "lib-dzne-math-0.2.0.tar", last modified: Mon May 29 09:26:55 2023, max compression
```

## Comparing `lib-dzne-math-0.1.2.tar` & `lib-dzne-math-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,26 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:35:40.550443 lib-dzne-math-0.1.2/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-02-19 00:26:57.000000 lib-dzne-math-0.1.2/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1460 2023-02-19 09:35:40.550443 lib-dzne-math-0.1.2/PKG-INFO
--rw-r--r--   0 base      (1001) base      (1001)      538 2023-02-19 09:33:13.000000 lib-dzne-math-0.1.2/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-02-19 09:35:40.550443 lib-dzne-math-0.1.2/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:35:40.546443 lib-dzne-math-0.1.2/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:35:40.546443 lib-dzne-math-0.1.2/src/lib_dzne_math/
--rw-r--r--   0 base      (1001) base      (1001)        1 2023-02-19 00:26:57.000000 lib-dzne-math-0.1.2/src/lib_dzne_math/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:35:40.550443 lib-dzne-math-0.1.2/src/lib_dzne_math/functions/
--rw-r--r--   0 base      (1001) base      (1001)       71 2023-02-19 00:26:57.000000 lib-dzne-math-0.1.2/src/lib_dzne_math/functions/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:35:40.550443 lib-dzne-math-0.1.2/src/lib_dzne_math/numerals/
--rw-r--r--   0 base      (1001) base      (1001)      873 2023-02-19 00:26:57.000000 lib-dzne-math-0.1.2/src/lib_dzne_math/numerals/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:35:40.550443 lib-dzne-math-0.1.2/src/lib_dzne_math/statistics/
--rw-r--r--   0 base      (1001) base      (1001)     1568 2023-02-19 00:26:57.000000 lib-dzne-math-0.1.2/src/lib_dzne_math/statistics/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-02-19 09:35:40.546443 lib-dzne-math-0.1.2/src/lib_dzne_math.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1460 2023-02-19 09:35:40.000000 lib-dzne-math-0.1.2/src/lib_dzne_math.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      346 2023-02-19 09:35:40.000000 lib-dzne-math-0.1.2/src/lib_dzne_math.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-02-19 09:35:40.000000 lib-dzne-math-0.1.2/src/lib_dzne_math.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       14 2023-02-19 09:35:40.000000 lib-dzne-math-0.1.2/src/lib_dzne_math.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:26:55.777012 lib-dzne-math-0.2.0/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-math-0.2.0/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1460 2023-05-29 09:26:55.777012 lib-dzne-math-0.2.0/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       16 2023-05-29 09:25:31.000000 lib-dzne-math-0.2.0/README.md
+-rw-r--r--   0 base      (1001) base      (1001)      560 2023-05-29 09:23:36.000000 lib-dzne-math-0.2.0/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 09:26:55.777012 lib-dzne-math-0.2.0/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:26:55.773012 lib-dzne-math-0.2.0/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:26:55.773012 lib-dzne-math-0.2.0/src/lib_dzne_math/
+-rw-r--r--   0 base      (1001) base      (1001)        1 2023-03-01 22:48:44.000000 lib-dzne-math-0.2.0/src/lib_dzne_math/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:26:55.773012 lib-dzne-math-0.2.0/src/lib_dzne_math/functions/
+-rw-r--r--   0 base      (1001) base      (1001)       73 2023-04-25 21:16:09.000000 lib-dzne-math-0.2.0/src/lib_dzne_math/functions/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:26:55.773012 lib-dzne-math-0.2.0/src/lib_dzne_math/na/
+-rw-rw-r--   0 base      (1001) base      (1001)      455 2023-05-29 09:22:45.000000 lib-dzne-math-0.2.0/src/lib_dzne_math/na/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:26:55.777012 lib-dzne-math-0.2.0/src/lib_dzne_math/numerals/
+-rw-r--r--   0 base      (1001) base      (1001)      873 2023-03-01 20:28:52.000000 lib-dzne-math-0.2.0/src/lib_dzne_math/numerals/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:26:55.777012 lib-dzne-math-0.2.0/src/lib_dzne_math/statistics/
+-rw-r--r--   0 base      (1001) base      (1001)     1568 2023-03-01 20:28:52.000000 lib-dzne-math-0.2.0/src/lib_dzne_math/statistics/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:26:55.777012 lib-dzne-math-0.2.0/src/lib_dzne_math/statistics/plots/
+-rw-rw-r--   0 base      (1001) base      (1001)       28 2023-03-03 21:33:18.000000 lib-dzne-math-0.2.0/src/lib_dzne_math/statistics/plots/DataEntry.py
+-rw-rw-r--   0 base      (1001) base      (1001)       35 2023-03-03 21:33:54.000000 lib-dzne-math-0.2.0/src/lib_dzne_math/statistics/plots/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 09:26:55.773012 lib-dzne-math-0.2.0/src/lib_dzne_math.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1460 2023-05-29 09:26:55.000000 lib-dzne-math-0.2.0/src/lib_dzne_math.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      524 2023-05-29 09:26:55.000000 lib-dzne-math-0.2.0/src/lib_dzne_math.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 09:26:55.000000 lib-dzne-math-0.2.0/src/lib_dzne_math.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       14 2023-05-29 09:26:55.000000 lib-dzne-math-0.2.0/src/lib_dzne_math.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       14 2023-05-29 09:26:55.000000 lib-dzne-math-0.2.0/src/lib_dzne_math.egg-info/top_level.txt
```

### Comparing `lib-dzne-math-0.1.2/LICENSE` & `lib-dzne-math-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-math-0.1.2/PKG-INFO` & `lib-dzne-math-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-math
-Version: 0.1.2
+Version: 0.2.0
 Summary: Libary for math. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-math-0.1.2/pyproject.toml` & `lib-dzne-math-0.2.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-math" # The package-name for "pip install package-name"
-version = "0.1.2"
+version = "0.2.0"
 description = "Libary for math. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
-dependencies = []
+dependencies = [
+    "pandas>=1.5.3",
+]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-math-0.1.2/src/lib_dzne_math/numerals/__init__.py` & `lib-dzne-math-0.2.0/src/lib_dzne_math/numerals/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-math-0.1.2/src/lib_dzne_math/statistics/__init__.py` & `lib-dzne-math-0.2.0/src/lib_dzne_math/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-math-0.1.2/src/lib_dzne_math.egg-info/PKG-INFO` & `lib-dzne-math-0.2.0/src/lib_dzne_math.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-math
-Version: 0.1.2
+Version: 0.2.0
 Summary: Libary for math. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


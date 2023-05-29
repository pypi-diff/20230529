# Comparing `tmp/tab-aaron-alphabet-0.0.1.tar.gz` & `tmp/tab-aaron-alphabet-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tab-aaron-alphabet-0.0.1.tar", last modified: Thu May 18 12:36:17 2023, max compression
+gzip compressed data, was "tab-aaron-alphabet-0.0.2.tar", last modified: Mon May 29 13:14:36 2023, max compression
```

## Comparing `tab-aaron-alphabet-0.0.1.tar` & `tab-aaron-alphabet-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/
--rwxrwxrwx   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 tab-aaron-alphabet-0.0.1/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1470 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/PKG-INFO
--rwxrwxrwx   0 base      (1001) base      (1001)      530 2023-05-18 12:34:01.000000 tab-aaron-alphabet-0.0.1/pyproject.toml
--rwxrwxrwx   0 base      (1001) base      (1001)       38 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet/
--rwxrwxrwx   0 base      (1001) base      (1001)      560 2023-05-18 12:20:33.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet/__init__.py
--rwxrwxrwx   0 base      (1001) base      (1001)       75 2023-04-08 07:54:57.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet/__main__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 12:36:17.035159 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1470 2023-05-18 12:36:17.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      331 2023-05-18 12:36:17.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-18 12:36:17.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       25 2023-05-18 12:36:17.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       19 2023-05-18 12:36:17.000000 tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:14:36.535231 tab-aaron-alphabet-0.0.2/
+-rwxrwxrwx   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 tab-aaron-alphabet-0.0.2/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1470 2023-05-29 13:14:36.535231 tab-aaron-alphabet-0.0.2/PKG-INFO
+-rwxrwxrwx   0 base      (1001) base      (1001)      530 2023-05-29 13:14:22.000000 tab-aaron-alphabet-0.0.2/pyproject.toml
+-rwxrwxrwx   0 base      (1001) base      (1001)       38 2023-05-29 13:14:36.539231 tab-aaron-alphabet-0.0.2/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:14:36.535231 tab-aaron-alphabet-0.0.2/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:14:36.535231 tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet/
+-rwxrwxrwx   0 base      (1001) base      (1001)      634 2023-05-29 13:14:02.000000 tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet/__init__.py
+-rwxrwxrwx   0 base      (1001) base      (1001)       76 2023-05-29 12:47:17.000000 tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet/__main__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:14:36.535231 tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1470 2023-05-29 13:14:36.000000 tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      331 2023-05-29 13:14:36.000000 tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 13:14:36.000000 tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       25 2023-05-29 13:14:36.000000 tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       19 2023-05-29 13:14:36.000000 tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet.egg-info/top_level.txt
```

### Comparing `tab-aaron-alphabet-0.0.1/LICENSE` & `tab-aaron-alphabet-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tab-aaron-alphabet-0.0.1/PKG-INFO` & `tab-aaron-alphabet-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tab-aaron-alphabet
-Version: 0.0.1
+Version: 0.0.2
 Summary: Convert tab to 4 spaces. 
 Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `tab-aaron-alphabet-0.0.1/pyproject.toml` & `tab-aaron-alphabet-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "tab-aaron-alphabet"
-version = "0.0.1"
+version = "0.0.2"
 description = "Convert tab to 4 spaces. "
 license = { file = "LICENSE" }
 authors = [{ name = "Aaron Alphabet", email = "aaron.alphabet@gmx.ch" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet/__init__.py` & `tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import argparse as _argparse
+
 import os_aaron_alphabet as _os
 
 parser = _argparse.ArgumentParser(
     fromfile_prefix_chars='@',
     allow_abbrev=False,
 )
 parser.add_argument('targets', nargs='*')
 
 def main(args=None):
     ns = parser.parse_args(args)
     if len(ns.targets):
         targets = ns.targets
     else:
         targets = ['.']
-    files = _os.walk(targets)
+    files = _os.walk(*targets)
     for file in targets:
+        if _os.os.path.splitext(file)[1] != ".py":
+            continue
         with open(file, 'r') as s:
             text = s.read()
         text = text.replace('\t', "    ")
         with open(file, 'w') as s:
             s.write(text)
```

### Comparing `tab-aaron-alphabet-0.0.1/src/tab_aaron_alphabet.egg-info/PKG-INFO` & `tab-aaron-alphabet-0.0.2/src/tab_aaron_alphabet.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tab-aaron-alphabet
-Version: 0.0.1
+Version: 0.0.2
 Summary: Convert tab to 4 spaces. 
 Author-email: Aaron Alphabet <aaron.alphabet@gmx.ch>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


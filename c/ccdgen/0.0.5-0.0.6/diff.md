# Comparing `tmp/ccdgen-0.0.5-py3-none-any.whl.zip` & `tmp/ccdgen-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 8721 bytes, number of entries: 7
+Zip file size: 8936 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 22-Nov-06 21:28 ccdgen/__init__.py
--rw-r--r--  2.0 unx     5638 b- defN 23-Mar-04 22:09 ccdgen/__main__.py
--rw-r--r--  2.0 unx    11344 b- defN 23-Mar-04 22:12 ccdgen-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3823 b- defN 23-Mar-04 22:12 ccdgen-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-04 22:12 ccdgen-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Mar-04 22:12 ccdgen-0.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      528 b- defN 23-Mar-04 22:12 ccdgen-0.0.5.dist-info/RECORD
-7 files, 21432 bytes uncompressed, 7787 bytes compressed:  63.7%
+-rw-r--r--  2.0 unx     6297 b- defN 23-May-29 10:54 ccdgen/__main__.py
+-rw-r--r--  2.0 unx    11344 b- defN 23-May-29 10:55 ccdgen-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3838 b- defN 23-May-29 10:55 ccdgen-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 10:55 ccdgen-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-29 10:55 ccdgen-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      528 b- defN 23-May-29 10:55 ccdgen-0.0.6.dist-info/RECORD
+7 files, 22106 bytes uncompressed, 8002 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: ccdgen/__init__.py
 Comment: 
 
 Filename: ccdgen/__main__.py
 Comment: 
 
-Filename: ccdgen-0.0.5.dist-info/LICENSE
+Filename: ccdgen-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: ccdgen-0.0.5.dist-info/METADATA
+Filename: ccdgen-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: ccdgen-0.0.5.dist-info/WHEEL
+Filename: ccdgen-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: ccdgen-0.0.5.dist-info/top_level.txt
+Filename: ccdgen-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: ccdgen-0.0.5.dist-info/RECORD
+Filename: ccdgen-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ccdgen/__main__.py

```diff
@@ -1,10 +1,11 @@
 import argparse
 import json
 import os
+import re
 import subprocess
 import sys
 
 
 def create_parser() -> argparse.ArgumentParser:
     """Creates argument parser
 
@@ -133,29 +134,51 @@
                 file = os.path.abspath(file)
                 break
 
         if file is None:
             continue
 
         tokens[-1] = file # use abs path for file in compiler command
+        command = ' '.join(tokens)
+        command = replace_relative_paths(command)
 
         db_entry = {
             "directory": os.path.dirname(file),
-            "command": ' '.join(tokens),
+            "command": command,
             "file": os.path.basename(file)
         }
         
         compile_db.append(db_entry)
 
     if compiler is None:
         print('Could not detect compiler')
         sys.exit(1)
 
     return compile_db
 
+def replace_relative_paths(command: str) -> str:
+    """Replaces any relative paths with absolute paths
+
+    Currently only checks for include paths starting with -I
+
+    Args:
+        command:    Compiler command from `make` output
+
+    Returns:
+        Command with relative paths replaced
+    """
+
+    matches = re.findall(r'-I(?:\.\.\/)+[^-\s]+', command)
+
+    for m in matches:
+        relative_path = m[2:]  # remove '-I' prefix
+        absolute_path = os.path.abspath(relative_path)
+        command = command.replace(m, '-I' + absolute_path)
+    
+    return command
 
 def detect_compiler(line: str) -> str | None:
     """Tries to detect the name of a compiler in a line of text
 
     Currently checks for:
         gcc, g++, clang, clang++, cc
```

## Comparing `ccdgen-0.0.5.dist-info/LICENSE` & `ccdgen-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ccdgen-0.0.5.dist-info/METADATA` & `ccdgen-0.0.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccdgen
-Version: 0.0.5
+Version: 0.0.6
 Summary: Generates compilation databases by capturing standard output from Make
 Author: Tim Brewis
 Author-email: timbrewis27@gmail.com
 License: Apache-2.0
 Project-URL: Source, https://github.com/t-bre/ccdgen
 Project-URL: Tracker, https://github.com/t-bre/ccdgen
 Keywords: make
@@ -88,15 +88,15 @@
 - The script relies on the Python standard library modules `argparse`, `json`, 
   `os`, `subprocess` and `sys`.
 - This script relies on `make` echoing the compiler commands it runs to 
   stdout. If compiler commands are prefixed in the Makefile with `@` or 
   `make` is run in silent mode, the output cannot be captured.
 - The build must succeed to generate a full compilation database, though 
   warnings are not a problem.
-- Currently only tested with Python 3.10 on macOS Ventura.
+- Currently only tested with Python 3.10 on macOS Ventura and Windows 10.
 
 ## Other Tools
 
 - [CMake](https://cmake.org) (since version 2.8.5) can be used as is to generate 
   `compile_commands.json` by adding `-DCMAKE_EXPORT_COMPILE_COMMANDS=ON` when 
   calling it. This only works for Unix Makefile builds.
 - [Bear](https://github.com/rizsotto/Bear) is much more advanced tool for
```


# Comparing `tmp/c_formatter_42-0.2.1.tar.gz` & `tmp/c_formatter_42-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "c_formatter_42-0.2.1.tar", last modified: Tue Jan 10 12:39:52 2023, max compression
+gzip compressed data, was "c_formatter_42-0.2.2.tar", last modified: Mon May 29 00:26:46 2023, max compression
```

## Comparing `c_formatter_42-0.2.1.tar` & `c_formatter_42-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:39:52.636960 c_formatter_42-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-01-10 12:39:52.636960 c_formatter_42-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:39:52.628960 c_formatter_42-0.2.1/c_formatter_42/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:39:52.632960 c_formatter_42-0.2.1/c_formatter_42/data/
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/data/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/data/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)  2457768 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/data/clang-format-darwin
--rwxr-xr-x   0 runner    (1001) docker     (123)  2332096 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/data/clang-format-linux
--rw-r--r--   0 runner    (1001) docker     (123)  1890816 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/data/clang-format-win32.exe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:39:52.636960 c_formatter_42-0.2.1/c_formatter_42/formatters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/formatters/align.py
--rw-r--r--   0 runner    (1001) docker     (123)     3038 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/formatters/clang_format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/formatters/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/formatters/hoist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/formatters/line_breaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/formatters/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/formatters/preprocessor_directive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/formatters/return_type_single_tab.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/c_formatter_42/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-10 12:39:52.628960 c_formatter_42-0.2.1/c_formatter_42.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-01-10 12:39:52.000000 c_formatter_42-0.2.1/c_formatter_42.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-01-10 12:39:52.000000 c_formatter_42-0.2.1/c_formatter_42.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-10 12:39:52.000000 c_formatter_42-0.2.1/c_formatter_42.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-01-10 12:39:52.000000 c_formatter_42-0.2.1/c_formatter_42.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-10 12:39:52.000000 c_formatter_42-0.2.1/c_formatter_42.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-01-10 12:39:52.636960 c_formatter_42-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-10 12:39:43.000000 c_formatter_42-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:26:46.925277 c_formatter_42-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-29 00:26:46.925277 c_formatter_42-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:26:46.913277 c_formatter_42-0.2.2/c_formatter_42/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:26:46.921277 c_formatter_42-0.2.2/c_formatter_42/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     5764 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/data/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/data/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2457768 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/data/clang-format-darwin
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2332096 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/data/clang-format-linux
+-rw-r--r--   0 runner    (1001) docker     (123)  1890816 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/data/clang-format-win32.exe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:26:46.925277 c_formatter_42-0.2.2/c_formatter_42/formatters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/formatters/align.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/formatters/clang_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/formatters/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/formatters/hoist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/formatters/line_breaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/formatters/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/formatters/preprocessor_directive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/formatters/return_type_single_tab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/c_formatter_42/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:26:46.913277 c_formatter_42-0.2.2/c_formatter_42.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3288 2023-05-29 00:26:46.000000 c_formatter_42-0.2.2/c_formatter_42.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-29 00:26:46.000000 c_formatter_42-0.2.2/c_formatter_42.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:26:46.000000 c_formatter_42-0.2.2/c_formatter_42.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-29 00:26:46.000000 c_formatter_42-0.2.2/c_formatter_42.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 00:26:46.000000 c_formatter_42-0.2.2/c_formatter_42.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-29 00:26:46.925277 c_formatter_42-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:26:46.925277 c_formatter_42-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-05-29 00:26:36.000000 c_formatter_42-0.2.2/tests/test_run.py
```

### Comparing `c_formatter_42-0.2.1/LICENSE` & `c_formatter_42-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `c_formatter_42-0.2.1/PKG-INFO` & `c_formatter_42-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c_formatter_42
-Version: 0.2.1
+Version: 0.2.2
 Summary: formatting tool complient with 42 school's norm
 Home-page: https://github.com/dawnbeen/c_formatter_42
 Project-URL: Tracker, https://github.com/dawnbeen/c_formatter_42/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `c_formatter_42-0.2.1/README.md` & `c_formatter_42-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `c_formatter_42-0.2.1/c_formatter_42/__main__.py` & `c_formatter_42-0.2.2/c_formatter_42/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #    By: cacharle <me@cacharle.xyz>                 +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2020/10/04 09:53:21 by cacharle          #+#    #+#              #
 #    Updated: 2020/10/04 09:53:21 by cacharle         ###   ########.fr        #
 #                                                                              #
 # ############################################################################ #
 
-import sys
 import argparse
+import sys
 
 from c_formatter_42.run import run_all
 
 
 def main():
     arg_parser = argparse.ArgumentParser(
         prog="c_formatter_42",
@@ -44,20 +44,20 @@
     else:
         for filepath in args.filepaths:
             try:
                 with open(filepath, "r") as file:
                     content = file.read()
                 if args.confirm:
                     result = input(
-                        "Are you sure you want to overwrite {}?[y/N]".format(filepath)
+                        f"Are you sure you want to overwrite {filepath}?[y/N]"
                     )
                     if result != "y":
                         continue
-                print("Writing to {}".format(filepath))
+                print(f"Writing to {filepath}")
                 with open(filepath, "w") as file:
                     file.write(run_all(content))
             except OSError as e:
-                print("Error: {}: {}".format(e.filename, e.strerror))
+                print(f"Error: {e.filename}: {e.strerror}")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `c_formatter_42-0.2.1/c_formatter_42/data/.clang-format` & `c_formatter_42-0.2.2/c_formatter_42/data/.clang-format`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
 # BreakBeforeTernaryOperators (bool)
 # If true, ternary operators will be placed after line breaks.
 BreakBeforeTernaryOperators: true
 
 
 # ColumnLimit (unsigned)
 # The column limit.
-ColumnLimit: 0
+ColumnLimit: 1024
 
 
 # FixNamespaceComments (bool)
 # If true, clang-format adds missing namespace end comments and fixes invalid existing ones.
 # FixNamespaceComments: false
```

### Comparing `c_formatter_42-0.2.1/c_formatter_42/data/clang-format-darwin` & `c_formatter_42-0.2.2/c_formatter_42/data/clang-format-darwin`

 * *Files identical despite different names*

### Comparing `c_formatter_42-0.2.1/c_formatter_42/data/clang-format-linux` & `c_formatter_42-0.2.2/c_formatter_42/data/clang-format-linux`

 * *Files identical despite different names*

### Comparing `c_formatter_42-0.2.1/c_formatter_42/data/clang-format-win32.exe` & `c_formatter_42-0.2.2/c_formatter_42/data/clang-format-win32.exe`

 * *Files identical despite different names*

### Comparing `c_formatter_42-0.2.1/c_formatter_42/formatters/align.py` & `c_formatter_42-0.2.2/c_formatter_42/formatters/align.py`

 * *Files identical despite different names*

### Comparing `c_formatter_42-0.2.1/c_formatter_42/formatters/clang_format.py` & `c_formatter_42-0.2.2/c_formatter_42/formatters/clang_format.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,58 +6,55 @@
 #    By: cacharle <me@cacharle.xyz>                 +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2020/10/04 10:40:07 by cacharle          #+#    #+#              #
 #    Updated: 2021/02/25 20:46:18 by cacharle         ###   ########.fr        #
 #                                                                              #
 # ############################################################################ #
 
-import os
-import sys
-import inspect
 import subprocess
+import sys
 from contextlib import contextmanager
+from pathlib import Path
 
 import c_formatter_42.data
 
-CONFIG_FILENAME = ".clang-format"
+CONFIG_FILENAME = Path(".clang-format")
 
-DATA_DIR = os.path.dirname(inspect.getfile(c_formatter_42.data))
+DATA_DIR = Path(c_formatter_42.data.__file__).parent
 
 
 @contextmanager
 def _config_context():
     """Temporarly place .clang-format config file in the current directory
     If there already is a config in the current directory, it's backed up
     then put back in place after clang-format is done running
     """
-    config_path = os.path.join(DATA_DIR, CONFIG_FILENAME)
+    config_path = DATA_DIR / CONFIG_FILENAME
     previous_config = None
     try:
-        os.symlink(config_path, CONFIG_FILENAME)
+        CONFIG_FILENAME.symlink_to(config_path)
     except FileExistsError:
-        if not os.path.islink(CONFIG_FILENAME):
-            with open(CONFIG_FILENAME) as f:
-                previous_config = f.read()
-        os.unlink(CONFIG_FILENAME)
-        os.symlink(config_path, CONFIG_FILENAME)
+        if not CONFIG_FILENAME.is_symlink():
+            previous_config = CONFIG_FILENAME.read_text()
+        CONFIG_FILENAME.unlink()
+        CONFIG_FILENAME.symlink_to(config_path)
     try:
         yield
     finally:
-        os.unlink(CONFIG_FILENAME)
+        CONFIG_FILENAME.unlink()
         if previous_config is not None:
-            with open(CONFIG_FILENAME, "w") as f:
-                f.write(previous_config)
+            CONFIG_FILENAME.write_text(previous_config)
 
 
 if sys.platform == "linux":
-    CLANG_FORMAT_EXEC = os.path.join(DATA_DIR, "clang-format-linux")
+    CLANG_FORMAT_EXEC = DATA_DIR / "clang-format-linux"
 elif sys.platform == "darwin":
-    CLANG_FORMAT_EXEC = os.path.join(DATA_DIR, "clang-format-darwin")
+    CLANG_FORMAT_EXEC = DATA_DIR / "clang-format-darwin"
 elif sys.platform == "win32":
-    CLANG_FORMAT_EXEC = os.path.join(DATA_DIR, "clang-format-win32.exe")
+    CLANG_FORMAT_EXEC = DATA_DIR / "clang-format-win32.exe"
 else:
     raise NotImplementedError("Your platform is not supported")
 
 
 def clang_format(content: str) -> str:
     """Wrapper around clang-format
 
@@ -69,10 +66,10 @@
         process = subprocess.Popen(
             [CLANG_FORMAT_EXEC, "-style=file"],
             stdin=subprocess.PIPE,
             stdout=subprocess.PIPE,
             stderr=subprocess.PIPE,
         )
         out, err = process.communicate(input=content.encode())
-        if process.returncode != 0:
+        if process.returncode != 0:  # pragma: no cover
             raise RuntimeError(f"clang-format error: {err.decode()}")
         return out.decode()
```

### Comparing `c_formatter_42-0.2.1/c_formatter_42/formatters/helper.py` & `c_formatter_42-0.2.2/c_formatter_42/formatters/helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 #    Created: 2020/10/04 11:38:00 by cacharle          #+#    #+#              #
 #    Updated: 2021/02/08 18:22:06 by charles          ###   ########.fr        #
 #                                                                              #
 # ############################################################################ #
 
 import re
 
-
 # regex for a type
 REGEX_TYPE = r"(?!return)([a-z]+\s+)*[a-zA-Z_]\w*"
 # regex for a c variable/function name
 REGEX_NAME = r"\**[a-zA-Z_*()]\w*"
 # regex for a name in a declaration context (with array and function ptr)
 REGEX_DECL_NAME = r"\(?{name}(\[.*\])*(\)\(.*\))?".format(name=REGEX_NAME)
```

### Comparing `c_formatter_42-0.2.1/c_formatter_42/formatters/hoist.py` & `c_formatter_42-0.2.2/c_formatter_42/formatters/hoist.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,15 +51,15 @@
             r"^(?P<indent>\s+)"
             r"(?P<type>{t})\s+"
             r"(?P<name>{d})\s+=\s+"
             r"(?P<value>.+);$".format(t=helper.REGEX_TYPE, d=helper.REGEX_DECL_NAME),
             line,
         )
         if m is not None:
-            lines.append("\t{}\t{};".format(m.group("type"), m.group("name")))
+            lines.append(f"\t{m.group('type')}\t{m.group('name')};")
             lines.append(
                 "{}{} = {};".format(
                     m.group("indent"),
                     m.group("name").replace("*", ""),
                     m.group("value"),
                 )
             )
```

### Comparing `c_formatter_42-0.2.1/c_formatter_42/formatters/line_breaker.py` & `c_formatter_42-0.2.2/c_formatter_42/formatters/line_breaker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,99 +1,90 @@
 import re
+
 from c_formatter_42.formatters import helper
 
 
 def line_breaker(content: str, column_limit: int = 80) -> str:
     lines = content.split("\n")
     lines = [insert_break(line, column_limit) for line in lines]
-
     return "\n".join(lines)
 
 
 def insert_break(line: str, column_limit: int) -> str:
     if line_length(line) <= column_limit:
         return line
 
-    # break at all breakable spaces (space after comma or space before binary
+    # Break at all breakable spaces (space after comma or space before binary
     # operators or logical AND or OR)
     breakable_space_pattern = r"((?<=,) | (?=[+\-*/%]|\|\||&&)(?!\*+\S|\+\+|\-\-))"
     line = re.sub(breakable_space_pattern, "\n", line)
     segments = line.split("\n")
 
     line_indent_level = indent_level(line)
 
-    # join as many segments as it doesn't exceed line length limit
+    # Join as many segments as it doesn't exceed line length limit
     line = segments[0]
     current_line_length = line_length(segments[0])
     for segment in segments[1:]:
         current_line_length += line_length(segment) + 1
         if current_line_length > column_limit:
             tabulation = "\t" * (line_indent_level + additional_indent_level(line))
             line = ("\n" + tabulation).join([line, segment])
             current_line_length = line_length(tabulation + segment)
         else:
             line = " ".join([line, segment])
 
     return line
 
 
+# The additional indent level increases in proportion to the corresponding parentheses depth
 #
-# additional indent level increases in proportion to corresponds paren depth
-#
-# (examples)
-# foo() * bar() * baz()
-# ~~~~~~~~~~~~~^~~~~~~~ when line breaks here,
-# foo() * bar()
-# >   * baz()           next line should be indented with 1 tab
-# ===
-# (foo(bar() * baz()))
-# ~~~~~~~~~~^~~~~~~~~    when line breaks here,
-# (foo(bar()
-# >   >   >   * baz()))  next line should be indented with 3 tabs
-#
-# function declaration, user defined type (?), and control statement needs one less tab (discount)
-#
+# Examples:
+#   -----------------------------------------------------------------------------------
+#   foo() * bar() * baz()
+#   ~~~~~~~~~~~~~^~~~~~~~   When line breaks here,
+#   foo() * bar()
+#   >   * baz()             Next line should be indented with 1 tab (default)
+#   -----------------------------------------------------------------------------------
+#   foo(bar() * baz())
+#   ~~~~~~~~~^~~~~~~~~      When line breaks here,
+#   foo(bar()
+#   >   * baz())            Next line should be indented with 1 tab (paren depth is 1)
+#   -----------------------------------------------------------------------------------
+#   (foo(bar() * baz()))
+#   ~~~~~~~~~~^~~~~~~~~~    When line breaks here,
+#   (foo(bar()
+#   >   >   * baz()))       Next line should be indented with 2 tabs (paren depth is 2)
+#   -----------------------------------------------------------------------------------
 def additional_indent_level(s: str) -> int:
-    additional_indent_level = 1
-
-    discount_pattern = (
-        r"(^\t*{type}\t+.*?[a-zA-Z0-9_]\((?!.*?;))|(^\t*typedef)"
-        "|(^\t*(if|while|return))"
-    )
-    discount_pattern = discount_pattern.format(
-        type=helper.REGEX_TYPE,
-    )
-    if re.match(discount_pattern, s):
-        additional_indent_level = 0
-
+    paren_depth = 0
     is_surrounded_sq = False
     is_surrounded_dq = False
-
     for c in s:
         if c == "'":
             is_surrounded_sq = not is_surrounded_sq
         elif c == '"':
             is_surrounded_dq = not is_surrounded_dq
         elif c == "(" and not is_surrounded_sq and not is_surrounded_dq:
-            additional_indent_level += 1
+            paren_depth += 1
         elif c == ")" and not is_surrounded_sq and not is_surrounded_dq:
-            additional_indent_level -= 1
+            paren_depth -= 1
 
-    return additional_indent_level
+    return max(1, paren_depth)  # 1 is the default additional indent level
 
 
 def line_length(line: str) -> int:
     line = line.expandtabs(4)
     return len(line)
 
 
 def indent_level(line: str) -> int:
-    # an exeptional rule for function declaration
+    # An exceptional rule for function declaration
     align_pattern = r"^(static\s+)?{type}\s+{name}\((.|\s)*?\);"
     align_pattern = align_pattern.format(type=helper.REGEX_TYPE, name=helper.REGEX_NAME)
     if re.match(align_pattern, line):
         last_tab_index = line.rfind("\t")
         if last_tab_index == -1:
             return 0
-        return int(len(line[: last_tab_index + 1].expandtabs(4)) / 4)
+        return line_length(line[: last_tab_index + 1]) // 4
 
     return line.count("\t")
```

### Comparing `c_formatter_42-0.2.1/c_formatter_42/formatters/preprocessor_directive.py` & `c_formatter_42-0.2.2/c_formatter_42/formatters/preprocessor_directive.py`

 * *Files identical despite different names*

### Comparing `c_formatter_42-0.2.1/c_formatter_42/formatters/return_type_single_tab.py` & `c_formatter_42-0.2.2/c_formatter_42/formatters/return_type_single_tab.py`

 * *Files identical despite different names*

### Comparing `c_formatter_42-0.2.1/c_formatter_42/run.py` & `c_formatter_42-0.2.2/c_formatter_42/run.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 #    By: cacharle <me@cacharle.xyz>                 +#+  +:+       +#+         #
 #                                                 +#+#+#+#+#+   +#+            #
 #    Created: 2020/10/09 18:15:09 by cacharle          #+#    #+#              #
 #    Updated: 2021/02/11 20:12:15 by charles          ###   ########.fr        #
 #                                                                              #
 # ############################################################################ #
 
+from c_formatter_42.formatters.align import align
 from c_formatter_42.formatters.clang_format import clang_format
 from c_formatter_42.formatters.hoist import hoist
-from c_formatter_42.formatters.align import align
-from c_formatter_42.formatters.preprocessor_directive import preprocessor_directive
-from c_formatter_42.formatters.return_type_single_tab import return_type_single_tab
+from c_formatter_42.formatters.line_breaker import line_breaker
 from c_formatter_42.formatters.misc import (
+    insert_void,
     parenthesize_return,
-    space_before_semi_colon,
     remove_multiline_condition_space,
-    insert_void,
+    space_before_semi_colon,
 )
-from c_formatter_42.formatters.line_breaker import line_breaker
+from c_formatter_42.formatters.preprocessor_directive import preprocessor_directive
+from c_formatter_42.formatters.return_type_single_tab import return_type_single_tab
 
 
 def run_all(content: str) -> str:
     """Run all formatters"""
     content = clang_format(content)
     content = preprocessor_directive(content)
     content = remove_multiline_condition_space(content)
```

### Comparing `c_formatter_42-0.2.1/c_formatter_42.egg-info/PKG-INFO` & `c_formatter_42-0.2.2/c_formatter_42.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: c-formatter-42
-Version: 0.2.1
+Version: 0.2.2
 Summary: formatting tool complient with 42 school's norm
 Home-page: https://github.com/dawnbeen/c_formatter_42
 Project-URL: Tracker, https://github.com/dawnbeen/c_formatter_42/issues
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `c_formatter_42-0.2.1/c_formatter_42.egg-info/SOURCES.txt` & `c_formatter_42-0.2.2/c_formatter_42.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 c_formatter_42/formatters/align.py
 c_formatter_42/formatters/clang_format.py
 c_formatter_42/formatters/helper.py
 c_formatter_42/formatters/hoist.py
 c_formatter_42/formatters/line_breaker.py
 c_formatter_42/formatters/misc.py
 c_formatter_42/formatters/preprocessor_directive.py
-c_formatter_42/formatters/return_type_single_tab.py
+c_formatter_42/formatters/return_type_single_tab.py
+tests/test_run.py
```

### Comparing `c_formatter_42-0.2.1/setup.cfg` & `c_formatter_42-0.2.2/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = c_formatter_42
-version = 0.2.1
+version = 0.2.2
 description = formatting tool complient with 42 school's norm
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/dawnbeen/c_formatter_42
 project_urls = 
 	Tracker = https://github.com/dawnbeen/c_formatter_42/issues
 classifiers = 
@@ -43,12 +43,25 @@
 
 [mypy]
 check_untyped_defs = true
 disallow_incomplete_defs = true
 
 [tool:pytest]
 testpaths = tests
+addopts = --cov=c_formatter_42 --cov-report=term-missing
+
+[coverage:run]
+source = c_formatter_42
+
+[coverage:report]
+exclude_lines = 
+	pragma: no cover
+	sys.platform
+	NotImplementedError
+
+[tool:isort]
+profile = black
 
 [egg_info]
 tag_build = 
 tag_date = 0
```


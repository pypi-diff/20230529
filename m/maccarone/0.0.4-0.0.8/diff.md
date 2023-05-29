# Comparing `tmp/maccarone-0.0.4.tar.gz` & `tmp/maccarone-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maccarone-0.0.4.tar", last modified: Mon May 29 02:56:59 2023, max compression
+gzip compressed data, was "maccarone-0.0.8.tar", last modified: Mon May 29 18:45:24 2023, max compression
```

## Comparing `maccarone-0.0.4.tar` & `maccarone-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.589148 maccarone-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.577148 maccarone-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.581148 maccarone-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 02:56:46.000000 maccarone-0.0.4/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-29 02:56:46.000000 maccarone-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 02:56:46.000000 maccarone-0.0.4/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-29 02:56:46.000000 maccarone-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 02:56:46.000000 maccarone-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 02:56:59.589148 maccarone-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 02:56:46.000000 maccarone-0.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.585148 maccarone-0.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 02:56:46.000000 maccarone-0.0.4/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 02:56:46.000000 maccarone-0.0.4/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 02:56:46.000000 maccarone-0.0.4/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-29 02:56:46.000000 maccarone-0.0.4/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 02:56:46.000000 maccarone-0.0.4/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-29 02:56:46.000000 maccarone-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:56:59.589148 maccarone-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.581148 maccarone-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.585148 maccarone-0.0.4/src/maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.589148 maccarone-0.0.4/src/maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.589148 maccarone-0.0.4/src/maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.589148 maccarone-0.0.4/src/maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.589148 maccarone-0.0.4/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-05-29 02:56:46.000000 maccarone-0.0.4/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:24.610774 maccarone-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:24.606774 maccarone-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:24.606774 maccarone-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-29 18:44:49.000000 maccarone-0.0.8/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-29 18:44:49.000000 maccarone-0.0.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 18:44:49.000000 maccarone-0.0.8/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-29 18:44:49.000000 maccarone-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 18:44:49.000000 maccarone-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 18:45:24.610774 maccarone-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 18:44:49.000000 maccarone-0.0.8/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:24.606774 maccarone-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 18:44:49.000000 maccarone-0.0.8/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 18:44:49.000000 maccarone-0.0.8/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 18:44:49.000000 maccarone-0.0.8/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-29 18:44:49.000000 maccarone-0.0.8/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 18:44:49.000000 maccarone-0.0.8/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-29 18:44:49.000000 maccarone-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 18:45:24.610774 maccarone-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:24.606774 maccarone-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:24.610774 maccarone-0.0.8/src/maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-29 18:44:49.000000 maccarone-0.0.8/src/maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-29 18:44:49.000000 maccarone-0.0.8/src/maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-05-29 18:44:49.000000 maccarone-0.0.8/src/maccarone/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-29 18:44:49.000000 maccarone-0.0.8/src/maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-05-29 18:44:49.000000 maccarone-0.0.8/src/maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:24.610774 maccarone-0.0.8/src/maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-29 18:44:49.000000 maccarone-0.0.8/src/maccarone/scripts/preprocess.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-29 18:45:12.000000 maccarone-0.0.8/src/maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:24.610774 maccarone-0.0.8/src/maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-29 18:44:49.000000 maccarone-0.0.8/src/maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-05-29 18:44:49.000000 maccarone-0.0.8/src/maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:24.610774 maccarone-0.0.8/src/maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 18:45:24.000000 maccarone-0.0.8/src/maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-29 18:45:24.000000 maccarone-0.0.8/src/maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 18:45:24.000000 maccarone-0.0.8/src/maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 18:45:24.000000 maccarone-0.0.8/src/maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 18:45:24.000000 maccarone-0.0.8/src/maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-29 18:45:24.000000 maccarone-0.0.8/src/maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:24.610774 maccarone-0.0.8/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-29 18:44:49.000000 maccarone-0.0.8/support/rename_to_stale.sh
```

### Comparing `maccarone-0.0.4/.gitignore` & `maccarone-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.4/LICENSE` & `maccarone-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.4/dev-requirements.txt` & `maccarone-0.0.8/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.4/pyproject.toml` & `maccarone-0.0.8/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -18,13 +18,14 @@
 "Homepage" = "https://github.com/bsilverthorn/maccarone"
 "Repository" = "https://github.com/bsilverthorn/maccarone"
 
 [project.optional-dependencies]
 dev = [
     "ipython",
     "pip-tools",
+    "stale_maccarone==0.0.4",
 ]
 
 [project.scripts]
 maccarone = "maccarone.scripts.preprocess:script_main"
 
 [tool.setuptools_scm]
```

### Comparing `maccarone-0.0.4/src/maccarone/caching.py` & `maccarone-0.0.8/src/maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.4/src/maccarone/enable.py` & `maccarone-0.0.8/src/maccarone/enable.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import re
 import sys
 import logging
 import importlib.abc
 import importlib.machinery
 
 from enum import Enum
 from importlib.abc import (
@@ -10,17 +11,24 @@
     SourceLoader,
 )
 from importlib.machinery import ModuleSpec
 
 from maccarone.preprocessor import preprocess_maccarone
 
 enable_py_string_matching = True
+fullname_pattern: str | None = None
 
 class ImportFinder(MetaPathFinder):
     def find_spec(self, fullname, path, target=None):
+        # check against module name pattern, if configured
+        if fullname_pattern is not None:
+            if re.match(fullname_pattern, fullname) is None:
+                return None
+
+        # module name looks ok; check for maccarone snippets
         def make_modulespec(filename):
             return ModuleSpec(
                 fullname,
                 ImportLoader(fullname, filename),
                 origin=filename,
                 is_package=False
             )
@@ -34,15 +42,15 @@
             package_path = parts[1:-1]
             base_filename = os.path.join(entry, *package_path, basename)
             py_filename = base_filename + '.py'
             mn_filename = base_filename + '.mn.py'
 
             if os.path.exists(mn_filename):
                 return make_modulespec(mn_filename)
-            elif os.path.exists(py_filename):
+            elif enable_py_string_matching and os.path.exists(py_filename):
                 with open(py_filename, "rt") as file:
                     if "#<<" in file.read():
                         return make_modulespec(py_filename)
 
         return None  # we don't know how to import this
 
 class ImportLoader(SourceLoader):
```

### Comparing `maccarone-0.0.4/src/maccarone/openai.py` & `maccarone-0.0.8/src/maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.4/src/maccarone/preprocessor.py` & `maccarone-0.0.8/src/maccarone/preprocessor.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,22 +37,14 @@
 
         position = piece.end("rm")
 
     pieces += [PresentPiece(text=input[position:])]
 
     return pieces
 
-def get_last_line(text: str):
-    index = text.rfind('\n')
-
-    if index == -1:
-        return text
-    else:
-        return text[index+1:]
-
 def raw_pieces_to_tagged_input(raw_pieces: list[Piece]) -> str:
     tag_source = ""
     id = 0
 
     for piece in raw_pieces:
         match piece:
             case PresentPiece(text):
```

### Comparing `maccarone-0.0.4/src/maccarone/scripts/preprocess.py` & `maccarone-0.0.8/src/maccarone/scripts/preprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,22 +29,19 @@
 def main(root_path: str):
     """Preprocess maccarone files into Python."""
 
     for path in glob.glob(root_path + "/**/*.mn.py", recursive=True):
         preprocess(path)
 
 def parse_args() -> Namespace:
-    parser = ArgumentParser()
+    parser = ArgumentParser(description="Preprocess maccarone files into Python.")
+    parser.add_argument("root_path", help="Root path to search for .mn.py files.")
+    args = parser.parse_args()
+    return args
 
-    parser.add_argument(
-        "root_path",
-        type=str,
-    )
-
-    return parser.parse_args()
 
 def script_main():
     logging.basicConfig(level=logging.INFO)
 
     return main(**vars(parse_args()))
 
 if __name__ == "__main__":
```

### Comparing `maccarone-0.0.4/src/maccarone/test/test_caching.py` & `maccarone-0.0.8/src/maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.4/src/maccarone/test/test_preprocessor.py` & `maccarone-0.0.8/src/maccarone/test/test_preprocessor.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from textwrap import dedent
 
 from maccarone.preprocessor import (
     PresentPiece,
     MissingPiece,
     raw_source_to_pieces,
-    get_last_line,
     raw_pieces_to_tagged_input,
     tagged_output_to_completed_pieces,
 )
 
 @pytest.mark.parametrize("input, expected", [
     (
         "",
@@ -38,24 +37,14 @@
             PresentPiece(" missing pieces"),
         ],
     ),
 ])
 def test_raw_source_to_pieces(input, expected):
     assert list(raw_source_to_pieces(input)) == expected
 
-@pytest.mark.parametrize("text,expected", [
-    ("\nThis is line 1.\nThis is line 2.\nThis is line 3.", "This is line 3."),
-    ("This is a single line with no newline", "This is a single line with no newline"),
-    ("", ""),
-    ("Line 1\nLine 2\nLine 3\n", ""),
-    ("Line 1\nLine 2\nLine 3\n    ", "    "),
-])
-def test_get_last_line(text, expected):
-    assert get_last_line(text) == expected
-
 @pytest.mark.parametrize("raw_pieces, expected", [
     (
         [
             PresentPiece("\ndef add_two_numbers(x, y):\n    "),
             MissingPiece("    ", "add the args"),
             PresentPiece("\n\n"),
             MissingPiece("", "add two numbers from command line args, using argparse"),
```

### Comparing `maccarone-0.0.4/src/maccarone.egg-info/SOURCES.txt` & `maccarone-0.0.8/src/maccarone.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -17,11 +17,12 @@
 src/maccarone/preprocessor.py
 src/maccarone.egg-info/PKG-INFO
 src/maccarone.egg-info/SOURCES.txt
 src/maccarone.egg-info/dependency_links.txt
 src/maccarone.egg-info/entry_points.txt
 src/maccarone.egg-info/requires.txt
 src/maccarone.egg-info/top_level.txt
+src/maccarone/scripts/preprocess.mn.py
 src/maccarone/scripts/preprocess.py
 src/maccarone/test/test_caching.py
 src/maccarone/test/test_preprocessor.py
 support/rename_to_stale.sh
```


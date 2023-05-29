# Comparing `tmp/stale_maccarone-0.0.4.dev0.tar.gz` & `tmp/stale_maccarone-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stale_maccarone-0.0.4.dev0.tar", last modified: Mon May 29 00:54:26 2023, max compression
+gzip compressed data, was "stale_maccarone-0.0.8.tar", last modified: Mon May 29 18:45:15 2023, max compression
```

## Comparing `stale_maccarone-0.0.4.dev0.tar` & `stale_maccarone-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.061977 stale_maccarone-0.0.4.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.053977 stale_maccarone-0.0.4.dev0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.057977 stale_maccarone-0.0.4.dev0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 00:54:26.061977 stale_maccarone-0.0.4.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.057977 stale_maccarone-0.0.4.dev0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 00:54:26.061977 stale_maccarone-0.0.4.dev0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.053977 stale_maccarone-0.0.4.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.057977 stale_maccarone-0.0.4.dev0/src/maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.057977 stale_maccarone-0.0.4.dev0/src/maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.057977 stale_maccarone-0.0.4.dev0/src/maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.061977 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.061977 stale_maccarone-0.0.4.dev0/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.576184 stale_maccarone-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-29 18:45:15.576184 stale_maccarone-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 18:45:15.576184 stale_maccarone-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/src/stale_maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/src/stale_maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/scripts/preprocess.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.576184 stale_maccarone-0.0.8/src/stale_maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-05-29 18:45:07.000000 stale_maccarone-0.0.8/src/stale_maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.572184 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 18:45:15.000000 stale_maccarone-0.0.8/src/stale_maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 18:45:15.576184 stale_maccarone-0.0.8/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-29 18:44:49.000000 stale_maccarone-0.0.8/support/rename_to_stale.sh
```

### Comparing `stale_maccarone-0.0.4.dev0/.github/workflows/publish-to-pypi-stale.yml` & `stale_maccarone-0.0.8/.github/workflows/publish-to-pypi.yml`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: PyPI
+name: PyPI (`maccarone`)
 on:
   release:
     types: [published]
 jobs:
   publish-to-pypi:
     runs-on: ubuntu-latest
     strategy:
@@ -10,21 +10,25 @@
         python-version: ["3.10"]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - run: python -m pip install --upgrade pip
-      - name: Rename to `stale_maccarone`
+      - name: Preprocess with stale_maccarone
         run: |
-          support/rename_to_stale.sh
+          pip install stale_maccarone
+          python -m stale_maccarone.scripts.preprocess src/maccarone
+          pip uninstall -y stale_maccarone
+        env:
+          OPENAI_API_KEY: ${{ secrets.OPENAI_API_KEY }}
       - name: Build package
         run: |
           pip install build
           python -m build
       - name: Publish package
         run: |
           pip install twine
           twine upload dist/*
         env:
           TWINE_USERNAME: __token__
-          TWINE_PASSWORD: ${{ secrets.PYPI_API_TOKEN_STALE_MACCARONE }}
+          TWINE_PASSWORD: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `stale_maccarone-0.0.4.dev0/.gitignore` & `stale_maccarone-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4.dev0/LICENSE` & `stale_maccarone-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4.dev0/dev-requirements.txt` & `stale_maccarone-0.0.8/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4.dev0/pyproject.toml` & `stale_maccarone-0.0.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -18,14 +18,14 @@
 "Homepage" = "https://github.com/bsilverthorn/maccarone"
 "Repository" = "https://github.com/bsilverthorn/maccarone"
 
 [project.optional-dependencies]
 dev = [
     "ipython",
     "pip-tools",
+    "stale_maccarone==0.0.4",
 ]
 
 [project.scripts]
-maccarone = "maccarone.scripts.preprocess:script_main"
+stale_maccarone = "stale_maccarone.scripts.preprocess:script_main"
 
 [tool.setuptools_scm]
-local_scheme = "no-local-version"
```

### Comparing `stale_maccarone-0.0.4.dev0/src/maccarone/caching.py` & `stale_maccarone-0.0.8/src/stale_maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4.dev0/src/maccarone/enable.py` & `stale_maccarone-0.0.8/src/stale_maccarone/enable.py`

 * *Files 26% similar despite different names*

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
 
 from stale_maccarone.preprocessor import preprocess_maccarone
 
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

### Comparing `stale_maccarone-0.0.4.dev0/src/maccarone/openai.py` & `stale_maccarone-0.0.8/src/stale_maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4.dev0/src/maccarone/preprocessor.py` & `stale_maccarone-0.0.8/src/stale_maccarone/preprocessor.py`

 * *Files 12% similar despite different names*

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

### Comparing `stale_maccarone-0.0.4.dev0/src/maccarone/test/test_caching.py` & `stale_maccarone-0.0.8/src/stale_maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4.dev0/src/maccarone/test/test_preprocessor.py` & `stale_maccarone-0.0.8/src/stale_maccarone/test/test_preprocessor.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from textwrap import dedent
 
 from stale_maccarone.preprocessor import (
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


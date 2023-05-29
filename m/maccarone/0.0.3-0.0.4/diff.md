# Comparing `tmp/maccarone-0.0.3.tar.gz` & `tmp/maccarone-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maccarone-0.0.3.tar", last modified: Mon May 29 00:54:25 2023, max compression
+gzip compressed data, was "maccarone-0.0.4.tar", last modified: Mon May 29 02:56:59 2023, max compression
```

## Comparing `maccarone-0.0.3.tar` & `maccarone-0.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:25.361644 maccarone-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:25.353644 maccarone-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:25.357644 maccarone-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 00:54:10.000000 maccarone-0.0.3/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-29 00:54:10.000000 maccarone-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 00:54:10.000000 maccarone-0.0.3/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-29 00:54:10.000000 maccarone-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 00:54:10.000000 maccarone-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 00:54:25.357644 maccarone-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 00:54:10.000000 maccarone-0.0.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:25.357644 maccarone-0.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 00:54:10.000000 maccarone-0.0.3/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 00:54:10.000000 maccarone-0.0.3/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 00:54:10.000000 maccarone-0.0.3/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-29 00:54:10.000000 maccarone-0.0.3/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 00:54:10.000000 maccarone-0.0.3/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-29 00:54:10.000000 maccarone-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 00:54:25.361644 maccarone-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:25.353644 maccarone-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:25.357644 maccarone-0.0.3/src/maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:10.000000 maccarone-0.0.3/src/maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-29 00:54:10.000000 maccarone-0.0.3/src/maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-29 00:54:10.000000 maccarone-0.0.3/src/maccarone/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-29 00:54:10.000000 maccarone-0.0.3/src/maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-29 00:54:10.000000 maccarone-0.0.3/src/maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:25.357644 maccarone-0.0.3/src/maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-29 00:54:10.000000 maccarone-0.0.3/src/maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:25.357644 maccarone-0.0.3/src/maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-29 00:54:10.000000 maccarone-0.0.3/src/maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-29 00:54:10.000000 maccarone-0.0.3/src/maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:25.357644 maccarone-0.0.3/src/maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 00:54:25.000000 maccarone-0.0.3/src/maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-29 00:54:25.000000 maccarone-0.0.3/src/maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:54:25.000000 maccarone-0.0.3/src/maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 00:54:25.000000 maccarone-0.0.3/src/maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 00:54:25.000000 maccarone-0.0.3/src/maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-29 00:54:25.000000 maccarone-0.0.3/src/maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:25.357644 maccarone-0.0.3/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-05-29 00:54:10.000000 maccarone-0.0.3/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.589148 maccarone-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.577148 maccarone-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.581148 maccarone-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 02:56:46.000000 maccarone-0.0.4/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-29 02:56:46.000000 maccarone-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 02:56:46.000000 maccarone-0.0.4/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-29 02:56:46.000000 maccarone-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 02:56:46.000000 maccarone-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 02:56:59.589148 maccarone-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 02:56:46.000000 maccarone-0.0.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.585148 maccarone-0.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 02:56:46.000000 maccarone-0.0.4/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 02:56:46.000000 maccarone-0.0.4/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 02:56:46.000000 maccarone-0.0.4/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-29 02:56:46.000000 maccarone-0.0.4/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 02:56:46.000000 maccarone-0.0.4/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-29 02:56:46.000000 maccarone-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:56:59.589148 maccarone-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.581148 maccarone-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.585148 maccarone-0.0.4/src/maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.589148 maccarone-0.0.4/src/maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.589148 maccarone-0.0.4/src/maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-29 02:56:46.000000 maccarone-0.0.4/src/maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.589148 maccarone-0.0.4/src/maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      771 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-29 02:56:59.000000 maccarone-0.0.4/src/maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.589148 maccarone-0.0.4/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-05-29 02:56:46.000000 maccarone-0.0.4/support/rename_to_stale.sh
```

### Comparing `maccarone-0.0.3/.github/workflows/publish-to-pypi-stale.yml` & `maccarone-0.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files 16% similar despite different names*

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
@@ -10,21 +10,18 @@
         python-version: ["3.10"]
     steps:
       - uses: actions/checkout@v3
       - uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
       - run: python -m pip install --upgrade pip
-      - name: Rename to `stale_maccarone`
-        run: |
-          support/rename_to_stale.sh
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

### Comparing `maccarone-0.0.3/.gitignore` & `maccarone-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.3/LICENSE` & `maccarone-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.3/dev-requirements.txt` & `maccarone-0.0.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.3/pyproject.toml` & `maccarone-0.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -24,8 +24,7 @@
     "pip-tools",
 ]
 
 [project.scripts]
 maccarone = "maccarone.scripts.preprocess:script_main"
 
 [tool.setuptools_scm]
-local_scheme = "node-and-date"
```

### Comparing `maccarone-0.0.3/src/maccarone/caching.py` & `maccarone-0.0.4/src/maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.3/src/maccarone/enable.py` & `maccarone-0.0.4/src/maccarone/enable.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.3/src/maccarone/openai.py` & `maccarone-0.0.4/src/maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.3/src/maccarone/preprocessor.py` & `maccarone-0.0.4/src/maccarone/preprocessor.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.3/src/maccarone/scripts/preprocess.py` & `maccarone-0.0.4/src/maccarone/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.3/src/maccarone/test/test_caching.py` & `maccarone-0.0.4/src/maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.3/src/maccarone/test/test_preprocessor.py` & `maccarone-0.0.4/src/maccarone/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.3/src/maccarone.egg-info/SOURCES.txt` & `maccarone-0.0.4/src/maccarone.egg-info/SOURCES.txt`

 * *Files identical despite different names*


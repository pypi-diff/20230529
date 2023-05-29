# Comparing `tmp/stale_maccarone-0.0.4.tar.gz` & `tmp/stale_maccarone-0.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stale_maccarone-0.0.4.tar", last modified: Mon May 29 02:56:59 2023, max compression
+gzip compressed data, was "stale_maccarone-0.0.4.dev0.tar", last modified: Mon May 29 00:54:26 2023, max compression
```

## Comparing `stale_maccarone-0.0.4.tar` & `stale_maccarone-0.0.4.dev0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.873284 stale_maccarone-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.865284 stale_maccarone-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.869284 stale_maccarone-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/.github/workflows/publish-to-pypi-stale.yml
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-29 02:56:59.869284 stale_maccarone-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.869284 stale_maccarone-0.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/examples/add.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/examples/fizzbuzz.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/examples/todo.mn.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/local-dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-29 02:56:50.000000 stale_maccarone-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 02:56:59.873284 stale_maccarone-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.865284 stale_maccarone-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.869284 stale_maccarone-0.0.4/src/stale_maccarone/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:50.000000 stale_maccarone-0.0.4/src/stale_maccarone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-29 02:56:50.000000 stale_maccarone-0.0.4/src/stale_maccarone/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-29 02:56:50.000000 stale_maccarone-0.0.4/src/stale_maccarone/enable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-29 02:56:50.000000 stale_maccarone-0.0.4/src/stale_maccarone/openai.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-29 02:56:50.000000 stale_maccarone-0.0.4/src/stale_maccarone/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.869284 stale_maccarone-0.0.4/src/stale_maccarone/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-29 02:56:50.000000 stale_maccarone-0.0.4/src/stale_maccarone/scripts/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.869284 stale_maccarone-0.0.4/src/stale_maccarone/test/
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 02:56:50.000000 stale_maccarone-0.0.4/src/stale_maccarone/test/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-29 02:56:50.000000 stale_maccarone-0.0.4/src/stale_maccarone/test/test_preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.869284 stale_maccarone-0.0.4/src/stale_maccarone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-29 02:56:59.000000 stale_maccarone-0.0.4/src/stale_maccarone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-05-29 02:56:59.000000 stale_maccarone-0.0.4/src/stale_maccarone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:56:59.000000 stale_maccarone-0.0.4/src/stale_maccarone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 02:56:59.000000 stale_maccarone-0.0.4/src/stale_maccarone.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 02:56:59.000000 stale_maccarone-0.0.4/src/stale_maccarone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 02:56:59.000000 stale_maccarone-0.0.4/src/stale_maccarone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:56:59.869284 stale_maccarone-0.0.4/support/
--rwxr-xr-x   0 runner    (1001) docker     (123)      424 2023-05-29 02:56:46.000000 stale_maccarone-0.0.4/support/rename_to_stale.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.061977 stale_maccarone-0.0.4.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.053977 stale_maccarone-0.0.4.dev0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.057977 stale_maccarone-0.0.4.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/.github/workflows/publish-to-pypi-stale.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 00:54:26.061977 stale_maccarone-0.0.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.057977 stale_maccarone-0.0.4.dev0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 00:54:26.061977 stale_maccarone-0.0.4.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.053977 stale_maccarone-0.0.4.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.057977 stale_maccarone-0.0.4.dev0/src/maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.057977 stale_maccarone-0.0.4.dev0/src/maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.057977 stale_maccarone-0.0.4.dev0/src/maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-29 00:54:16.000000 stale_maccarone-0.0.4.dev0/src/maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.061977 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-29 00:54:26.000000 stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:26.061977 stale_maccarone-0.0.4.dev0/support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      480 2023-05-29 00:54:13.000000 stale_maccarone-0.0.4.dev0/support/rename_to_stale.sh
```

### Comparing `stale_maccarone-0.0.4/.github/workflows/publish-to-pypi.yml` & `stale_maccarone-0.0.4.dev0/.github/workflows/publish-to-pypi.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: PyPI (`maccarone`)
+name: PyPI
 on:
   release:
     types: [published]
 jobs:
   publish-to-pypi:
     runs-on: ubuntu-latest
     strategy:
```

### Comparing `stale_maccarone-0.0.4/.gitignore` & `stale_maccarone-0.0.4.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4/LICENSE` & `stale_maccarone-0.0.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4/dev-requirements.txt` & `stale_maccarone-0.0.4.dev0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4/pyproject.toml` & `stale_maccarone-0.0.4.dev0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,7 +24,8 @@
     "pip-tools",
 ]
 
 [project.scripts]
 maccarone = "maccarone.scripts.preprocess:script_main"
 
 [tool.setuptools_scm]
+local_scheme = "no-local-version"
```

### Comparing `stale_maccarone-0.0.4/src/stale_maccarone/caching.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4/src/stale_maccarone/enable.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/enable.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4/src/stale_maccarone/openai.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4/src/stale_maccarone/preprocessor.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/preprocessor.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4/src/stale_maccarone/scripts/preprocess.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4/src/stale_maccarone/test/test_caching.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.4/src/stale_maccarone/test/test_preprocessor.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/test/test_preprocessor.py`

 * *Files identical despite different names*


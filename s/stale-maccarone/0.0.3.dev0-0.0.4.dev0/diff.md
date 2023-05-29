# Comparing `tmp/stale_maccarone-0.0.3.dev0.tar.gz` & `tmp/stale_maccarone-0.0.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stale_maccarone-0.0.3.dev0.tar", last modified: Sun May 28 23:46:12 2023, max compression
+gzip compressed data, was "stale_maccarone-0.0.4.dev0.tar", last modified: Mon May 29 00:54:26 2023, max compression
```

## Comparing `stale_maccarone-0.0.3.dev0.tar` & `stale_maccarone-0.0.4.dev0.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/.github/
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/.github/workflows/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      668 2023-05-19 23:46:06.000000 stale_maccarone-0.0.3.dev0/.github/workflows/publish-to-pypi.yml
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      462 2023-05-19 23:46:06.000000 stale_maccarone-0.0.3.dev0/.github/workflows/run-pytest.yml
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     3125 2023-05-20 00:42:00.000000 stale_maccarone-0.0.3.dev0/.gitignore
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1074 2023-05-19 23:43:32.000000 stale_maccarone-0.0.3.dev0/LICENSE
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      354 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2117 2023-05-20 00:38:51.000000 stale_maccarone-0.0.3.dev0/dev-requirements.txt
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/examples/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       24 2023-05-28 23:06:55.000000 stale_maccarone-0.0.3.dev0/examples/__init__.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      105 2023-05-28 23:00:28.000000 stale_maccarone-0.0.3.dev0/examples/add.mn.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      123 2023-05-28 23:00:28.000000 stale_maccarone-0.0.3.dev0/examples/fizzbuzz.mn.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      413 2023-05-28 23:00:28.000000 stale_maccarone-0.0.3.dev0/examples/todo.mn.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       34 2023-05-20 00:40:18.000000 stale_maccarone-0.0.3.dev0/local-dev-requirements.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      671 2023-05-28 23:45:59.000000 stale_maccarone-0.0.3.dev0/pyproject.toml
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       38 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/setup.cfg
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/src/
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/src/maccarone/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-28 23:41:14.000000 stale_maccarone-0.0.3.dev0/src/maccarone/__init__.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1015 2023-05-28 23:41:14.000000 stale_maccarone-0.0.3.dev0/src/maccarone/caching.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1890 2023-05-28 23:41:14.000000 stale_maccarone-0.0.3.dev0/src/maccarone/enable.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1350 2023-05-28 23:41:14.000000 stale_maccarone-0.0.3.dev0/src/maccarone/openai.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     3841 2023-05-28 23:41:14.000000 stale_maccarone-0.0.3.dev0/src/maccarone/preprocessor.py
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/src/maccarone/scripts/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1135 2023-05-28 23:41:14.000000 stale_maccarone-0.0.3.dev0/src/maccarone/scripts/preprocess.py
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/src/maccarone/test/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      538 2023-05-28 23:41:14.000000 stale_maccarone-0.0.3.dev0/src/maccarone/test/test_caching.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2945 2023-05-28 23:41:14.000000 stale_maccarone-0.0.3.dev0/src/maccarone/test/test_preprocessor.py
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-28 23:46:12.697716 stale_maccarone-0.0.3.dev0/src/stale_maccarone.egg-info/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      354 2023-05-28 23:46:12.000000 stale_maccarone-0.0.3.dev0/src/stale_maccarone.egg-info/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      736 2023-05-28 23:46:12.000000 stale_maccarone-0.0.3.dev0/src/stale_maccarone.egg-info/SOURCES.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        1 2023-05-28 23:46:12.000000 stale_maccarone-0.0.3.dev0/src/stale_maccarone.egg-info/dependency_links.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       71 2023-05-28 23:46:12.000000 stale_maccarone-0.0.3.dev0/src/stale_maccarone.egg-info/entry_points.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       54 2023-05-28 23:46:12.000000 stale_maccarone-0.0.3.dev0/src/stale_maccarone.egg-info/requires.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       10 2023-05-28 23:46:12.000000 stale_maccarone-0.0.3.dev0/src/stale_maccarone.egg-info/top_level.txt
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

### Comparing `stale_maccarone-0.0.3.dev0/.github/workflows/publish-to-pypi.yml` & `stale_maccarone-0.0.4.dev0/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/.gitignore` & `stale_maccarone-0.0.4.dev0/.gitignore`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/LICENSE` & `stale_maccarone-0.0.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/dev-requirements.txt` & `stale_maccarone-0.0.4.dev0/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/pyproject.toml` & `stale_maccarone-0.0.4.dev0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/src/maccarone/caching.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/src/maccarone/enable.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/enable.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/src/maccarone/openai.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/openai.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/src/maccarone/preprocessor.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/preprocessor.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/src/maccarone/scripts/preprocess.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/scripts/preprocess.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/src/maccarone/test/test_caching.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/src/maccarone/test/test_preprocessor.py` & `stale_maccarone-0.0.4.dev0/src/maccarone/test/test_preprocessor.py`

 * *Files identical despite different names*

### Comparing `stale_maccarone-0.0.3.dev0/src/stale_maccarone.egg-info/SOURCES.txt` & `stale_maccarone-0.0.4.dev0/src/stale_maccarone.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 LICENSE
 dev-requirements.txt
 local-dev-requirements.txt
 pyproject.toml
+.github/workflows/publish-to-pypi-stale.yml
 .github/workflows/publish-to-pypi.yml
 .github/workflows/run-pytest.yml
 examples/__init__.py
 examples/add.mn.py
 examples/fizzbuzz.mn.py
 examples/todo.mn.py
 src/maccarone/__init__.py
@@ -18,8 +19,9 @@
 src/maccarone/test/test_caching.py
 src/maccarone/test/test_preprocessor.py
 src/stale_maccarone.egg-info/PKG-INFO
 src/stale_maccarone.egg-info/SOURCES.txt
 src/stale_maccarone.egg-info/dependency_links.txt
 src/stale_maccarone.egg-info/entry_points.txt
 src/stale_maccarone.egg-info/requires.txt
-src/stale_maccarone.egg-info/top_level.txt
+src/stale_maccarone.egg-info/top_level.txt
+support/rename_to_stale.sh
```


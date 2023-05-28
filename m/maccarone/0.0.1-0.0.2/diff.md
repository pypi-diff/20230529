# Comparing `tmp/maccarone-0.0.1.tar.gz` & `tmp/maccarone-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maccarone-0.0.1.tar", last modified: Fri May 19 23:59:19 2023, max compression
+gzip compressed data, was "maccarone-0.0.2.tar", last modified: Sun May 28 23:40:38 2023, max compression
```

## Comparing `maccarone-0.0.1.tar` & `maccarone-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,36 @@
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-19 23:59:19.643233 maccarone-0.0.1/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     3078 2023-05-19 23:43:32.000000 maccarone-0.0.1/.gitignore
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     1074 2023-05-19 23:43:32.000000 maccarone-0.0.1/LICENSE
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      343 2023-05-19 23:59:19.643233 maccarone-0.0.1/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      576 2023-05-19 23:45:42.000000 maccarone-0.0.1/pyproject.toml
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       38 2023-05-19 23:59:19.643233 maccarone-0.0.1/setup.cfg
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-19 23:59:19.643233 maccarone-0.0.1/src/
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-19 23:59:19.643233 maccarone-0.0.1/src/maccarone/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-19 23:44:20.000000 maccarone-0.0.1/src/maccarone/__init__.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      743 2023-05-19 23:50:21.000000 maccarone-0.0.1/src/maccarone/caching.py
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)     2861 2023-05-19 23:44:20.000000 maccarone-0.0.1/src/maccarone/enable.py
-drwxrwxr-x   0 bsilverthorn  (1000) bsilverthorn  (1000)        0 2023-05-19 23:59:19.643233 maccarone-0.0.1/src/maccarone.egg-info/
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      343 2023-05-19 23:59:19.000000 maccarone-0.0.1/src/maccarone.egg-info/PKG-INFO
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)      292 2023-05-19 23:59:19.000000 maccarone-0.0.1/src/maccarone.egg-info/SOURCES.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)        1 2023-05-19 23:59:19.000000 maccarone-0.0.1/src/maccarone.egg-info/dependency_links.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       54 2023-05-19 23:59:19.000000 maccarone-0.0.1/src/maccarone.egg-info/requires.txt
--rw-rw-r--   0 bsilverthorn  (1000) bsilverthorn  (1000)       10 2023-05-19 23:59:19.000000 maccarone-0.0.1/src/maccarone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:40:38.202677 maccarone-0.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:40:38.190677 maccarone-0.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:40:38.194677 maccarone-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-28 23:40:25.000000 maccarone-0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-28 23:40:25.000000 maccarone-0.0.2/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-05-28 23:40:25.000000 maccarone-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-28 23:40:25.000000 maccarone-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-28 23:40:38.202677 maccarone-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-28 23:40:25.000000 maccarone-0.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:40:38.194677 maccarone-0.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 23:40:25.000000 maccarone-0.0.2/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-28 23:40:25.000000 maccarone-0.0.2/examples/add.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-28 23:40:25.000000 maccarone-0.0.2/examples/fizzbuzz.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-28 23:40:25.000000 maccarone-0.0.2/examples/todo.mn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-28 23:40:25.000000 maccarone-0.0.2/local-dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-28 23:40:25.000000 maccarone-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 23:40:38.202677 maccarone-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:40:38.190677 maccarone-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:40:38.198677 maccarone-0.0.2/src/maccarone/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 23:40:25.000000 maccarone-0.0.2/src/maccarone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-28 23:40:25.000000 maccarone-0.0.2/src/maccarone/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-28 23:40:25.000000 maccarone-0.0.2/src/maccarone/enable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-28 23:40:25.000000 maccarone-0.0.2/src/maccarone/openai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-05-28 23:40:25.000000 maccarone-0.0.2/src/maccarone/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:40:38.198677 maccarone-0.0.2/src/maccarone/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-05-28 23:40:25.000000 maccarone-0.0.2/src/maccarone/scripts/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:40:38.202677 maccarone-0.0.2/src/maccarone/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-28 23:40:25.000000 maccarone-0.0.2/src/maccarone/test/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-05-28 23:40:25.000000 maccarone-0.0.2/src/maccarone/test/test_preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:40:38.198677 maccarone-0.0.2/src/maccarone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-28 23:40:38.000000 maccarone-0.0.2/src/maccarone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-28 23:40:38.000000 maccarone-0.0.2/src/maccarone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 23:40:38.000000 maccarone-0.0.2/src/maccarone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-28 23:40:38.000000 maccarone-0.0.2/src/maccarone.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-28 23:40:38.000000 maccarone-0.0.2/src/maccarone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-28 23:40:38.000000 maccarone-0.0.2/src/maccarone.egg-info/top_level.txt
```

### Comparing `maccarone-0.0.1/.gitignore` & `maccarone-0.0.2/.gitignore`

 * *Files 5% similar despite different names*

```diff
@@ -154,7 +154,10 @@
 
 # PyCharm
 #  JetBrains specific template is maintained in a separate JetBrains.gitignore that can
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
+
+# direnv files (often contain secrets)
+.envrc
```

### Comparing `maccarone-0.0.1/LICENSE` & `maccarone-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maccarone-0.0.1/pyproject.toml` & `maccarone-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -21,9 +21,10 @@
 [project.optional-dependencies]
 dev = [
     "ipython",
     "pip-tools",
 ]
 
 [project.scripts]
+maccarone = "maccarone.scripts.preprocess:script_main"
 
 [tool.setuptools_scm]
```


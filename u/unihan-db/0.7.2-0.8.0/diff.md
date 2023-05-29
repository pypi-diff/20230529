# Comparing `tmp/unihan_db-0.7.2.tar.gz` & `tmp/unihan_db-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unihan_db-0.7.2.tar", max compression
+gzip compressed data, was "unihan_db-0.8.0.tar", max compression
```

## Comparing `unihan_db-0.7.2.tar` & `unihan_db-0.8.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1094 2023-05-13 12:53:28.019219 unihan_db-0.7.2/LICENSE
--rw-r--r--   0        0        0     3283 2023-05-13 12:53:28.019219 unihan_db-0.7.2/README.md
--rw-r--r--   0        0        0     3228 2023-05-13 12:53:28.023219 unihan_db-0.7.2/pyproject.toml
--rw-r--r--   0        0        0      496 2023-05-13 12:53:28.023219 unihan_db-0.7.2/src/unihan_db/__about__.py
--rw-r--r--   0        0        0      219 2023-05-13 12:53:28.023219 unihan_db-0.7.2/src/unihan_db/__init__.py
--rw-r--r--   0        0        0     6394 2023-05-13 12:53:28.023219 unihan_db-0.7.2/src/unihan_db/bootstrap.py
--rw-r--r--   0        0        0     8418 2023-05-13 12:53:28.023219 unihan_db-0.7.2/src/unihan_db/importer.py
--rw-r--r--   0        0        0    13498 2023-05-13 12:53:28.023219 unihan_db-0.7.2/src/unihan_db/tables.py
--rw-r--r--   0        0        0     1752 2023-05-13 12:53:28.023219 unihan_db-0.7.2/tests/conftest.py
--rw-r--r--   0        0        0    13881 2023-05-13 12:53:28.023219 unihan_db-0.7.2/tests/fixtures/Unihan_DictionaryIndices.txt
--rw-r--r--   0        0        0    11472 2023-05-13 12:53:28.023219 unihan_db-0.7.2/tests/fixtures/Unihan_DictionaryLikeData.txt
--rw-r--r--   0        0        0    13661 2023-05-13 12:53:28.023219 unihan_db-0.7.2/tests/fixtures/Unihan_IRGSources.txt
--rw-r--r--   0        0        0     2419 2023-05-13 12:53:28.023219 unihan_db-0.7.2/tests/fixtures/Unihan_NumericValues.txt
--rw-r--r--   0        0        0     9456 2023-05-13 12:53:28.023219 unihan_db-0.7.2/tests/fixtures/Unihan_OtherMappings.txt
--rw-r--r--   0        0        0    17767 2023-05-13 12:53:28.023219 unihan_db-0.7.2/tests/fixtures/Unihan_RadicalStrokeCounts.txt
--rw-r--r--   0        0        0    21631 2023-05-13 12:53:28.023219 unihan_db-0.7.2/tests/fixtures/Unihan_Readings.txt
--rw-r--r--   0        0        0    19028 2023-05-13 12:53:28.023219 unihan_db-0.7.2/tests/fixtures/Unihan_Variants.txt
--rw-r--r--   0        0        0      820 2023-05-13 12:53:28.023219 unihan_db-0.7.2/tests/test_bootstrap.py
--rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 unihan_db-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-05-29 17:46:49.608802 unihan_db-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3337 2023-05-29 17:46:49.608802 unihan_db-0.8.0/README.md
+-rw-r--r--   0        0        0     3045 2023-05-29 17:46:49.608802 unihan_db-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      496 2023-05-29 17:46:49.608802 unihan_db-0.8.0/src/unihan_db/__about__.py
+-rw-r--r--   0        0        0      219 2023-05-29 17:46:49.608802 unihan_db-0.8.0/src/unihan_db/__init__.py
+-rw-r--r--   0        0        0     6394 2023-05-29 17:46:49.608802 unihan_db-0.8.0/src/unihan_db/bootstrap.py
+-rw-r--r--   0        0        0     8418 2023-05-29 17:46:49.608802 unihan_db-0.8.0/src/unihan_db/importer.py
+-rw-r--r--   0        0        0    13498 2023-05-29 17:46:49.608802 unihan_db-0.8.0/src/unihan_db/tables.py
+-rw-r--r--   0        0        0     1752 2023-05-29 17:46:49.608802 unihan_db-0.8.0/tests/conftest.py
+-rw-r--r--   0        0        0    13881 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_DictionaryIndices.txt
+-rw-r--r--   0        0        0    11472 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_DictionaryLikeData.txt
+-rw-r--r--   0        0        0    13661 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_IRGSources.txt
+-rw-r--r--   0        0        0     2419 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_NumericValues.txt
+-rw-r--r--   0        0        0     9456 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_OtherMappings.txt
+-rw-r--r--   0        0        0    17767 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_RadicalStrokeCounts.txt
+-rw-r--r--   0        0        0    21631 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_Readings.txt
+-rw-r--r--   0        0        0    19028 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/fixtures/Unihan_Variants.txt
+-rw-r--r--   0        0        0      820 2023-05-29 17:46:49.612802 unihan_db-0.8.0/tests/test_bootstrap.py
+-rw-r--r--   0        0        0     4916 1970-01-01 00:00:00.000000 unihan_db-0.8.0/PKG-INFO
```

### Comparing `unihan_db-0.7.2/LICENSE` & `unihan_db-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/README.md` & `unihan_db-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -79,11 +79,15 @@
 
 ```console
 $ cd unihan-etl
 ```
 
 [Bootstrap your environment and learn more about contributing](https://cihai.git-pull.com/contributing/). We use the same conventions / tools across all cihai projects: `pytest`, `sphinx`, `flake8`, `mypy`, `black`, `isort`, `tmuxp`, and file watcher helpers (e.g. `entr(1)`).
 
+## Python versions
+
+- 0.8.0: Last Python 3.7 release
+
 ## More information
 
 [![Docs](https://github.com/cihai/unihan-db/workflows/docs/badge.svg)](https://unihan-db.git-pull.com/)
 [![Build Status](https://github.com/cihai/unihan-db/workflows/tests/badge.svg)](https://github.com/cihai/unihan-db/actions?query=workflow%3A%22tests%22)
```

### Comparing `unihan_db-0.7.2/pyproject.toml` & `unihan_db-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "unihan_db"
-version = "0.7.2"
+version = "0.8.0"
 description = "SQLAlchemy models for UNIHAN CJK database"
 license = "MIT"
 authors = ["Tony Narlock <tony@git-pull.com>"]
 classifiers = [
   "Development Status :: 4 - Beta",
   "License :: OSI Approved :: MIT License",
   "Environment :: Web Environment",
@@ -47,17 +47,17 @@
 Repository = "https://github.com/cihai/unihan-db"
 "Release notes" = "https://github.com/cihai/unihan-db/blob/master/CHANGES"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 appdirs = "*"
 SQLAlchemy = "<2"
-unihan-etl = "~=0.18.2"
+unihan-etl = "~=0.19.1"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 ### Docs ###
 sphinx = "*"
 furo = "*"
 gp-libs = "*"
 sphinx-autobuild = "*"
 sphinx-autodoc-typehints = "*"
 sphinx-inline-tabs = "<2023.4.21"  # For Python 3.7 support
@@ -73,25 +73,17 @@
 pytest-watcher = "*"
 
 ### Coverage ###
 codecov = "*"
 coverage = "*"
 pytest-cov = "*"
 
-### Format ###
-black = "*"
-isort = "*"
-
 ### Lint ###
-flake8 = [
-  { version = "*", python = "^3.7" },
-  { version = ">=5", python = "^3.8" },
-]
-flake8-bugbear = "*"
-flake8-comprehensions = "*"
+black = "*"
+ruff = "*"
 mypy = "*"
 sqlalchemy-stubs = "*"
 types-appdirs = "*"
 
 [tool.poetry.extras]
 docs = [
   "docutils",
@@ -104,28 +96,30 @@
   "sphinxext-rediraffe",
   "myst_parser",
   "furo",
   "gp-libs",
 ]
 test = ["pytest", "pytest-rerunfailures", "pytest-watcher"]
 coverage = ["codecov", "coverage", "pytest-cov"]
-format = ["black", "isort"]
 lint = [
-  "flake8",
-  "flake8-bugbear",
-  "flake8-comprehensions",
+  "black",
+  "ruff",
   "mypy",
   "sqlalchemy-stubs",
   "types-appdirs",
 ]
 
 [tool.mypy]
 plugins = [
   "sqlmypy",
 ]
+files = [
+  "src/",
+  "tests/",
+]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 omit = [
   "*/_compat.py",
   "docs/conf.py",
```

### Comparing `unihan_db-0.7.2/src/unihan_db/bootstrap.py` & `unihan_db-0.8.0/src/unihan_db/bootstrap.py`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/src/unihan_db/importer.py` & `unihan_db-0.8.0/src/unihan_db/importer.py`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/src/unihan_db/tables.py` & `unihan_db-0.8.0/src/unihan_db/tables.py`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/tests/conftest.py` & `unihan_db-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/tests/fixtures/Unihan_DictionaryIndices.txt` & `unihan_db-0.8.0/tests/fixtures/Unihan_DictionaryIndices.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/tests/fixtures/Unihan_DictionaryLikeData.txt` & `unihan_db-0.8.0/tests/fixtures/Unihan_DictionaryLikeData.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/tests/fixtures/Unihan_IRGSources.txt` & `unihan_db-0.8.0/tests/fixtures/Unihan_IRGSources.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/tests/fixtures/Unihan_NumericValues.txt` & `unihan_db-0.8.0/tests/fixtures/Unihan_NumericValues.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/tests/fixtures/Unihan_OtherMappings.txt` & `unihan_db-0.8.0/tests/fixtures/Unihan_OtherMappings.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/tests/fixtures/Unihan_RadicalStrokeCounts.txt` & `unihan_db-0.8.0/tests/fixtures/Unihan_RadicalStrokeCounts.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/tests/fixtures/Unihan_Readings.txt` & `unihan_db-0.8.0/tests/fixtures/Unihan_Readings.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/tests/fixtures/Unihan_Variants.txt` & `unihan_db-0.8.0/tests/fixtures/Unihan_Variants.txt`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/tests/test_bootstrap.py` & `unihan_db-0.8.0/tests/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `unihan_db-0.7.2/PKG-INFO` & `unihan_db-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unihan-db
-Version: 0.7.2
+Version: 0.8.0
 Summary: SQLAlchemy models for UNIHAN CJK database
 Home-page: https://unihan-db.git-pull.com
 License: MIT
 Keywords: unihan,sqlalchemy,cjk,chinese,japanese,sql,database
 Author: Tony Narlock
 Author-email: tony@git-pull.com
 Requires-Python: >=3.7,<4.0
@@ -15,32 +15,26 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Internationalization
 Classifier: Topic :: Software Development :: Localization
 Classifier: Topic :: Utilities
 Provides-Extra: coverage
 Provides-Extra: docs
-Provides-Extra: format
 Provides-Extra: lint
 Provides-Extra: test
 Requires-Dist: SQLAlchemy (<2)
 Requires-Dist: appdirs
-Requires-Dist: unihan-etl (>=0.18.2,<0.19.0)
+Requires-Dist: unihan-etl (>=0.19.1,<0.20.0)
 Project-URL: Bug Tracker, https://github.com/cihai/unihan-db/issues
 Project-URL: Documentation, https://unihan-db.git-pull.com
 Project-URL: Repository, https://github.com/cihai/unihan-db
 Project-URL: Release notes, https://github.com/cihai/unihan-db/blob/master/CHANGES
 Description-Content-Type: text/markdown
 
 # unihan-db &middot; [![Python Package](https://img.shields.io/pypi/v/unihan-db.svg)](https://pypi.org/project/unihan-db/) [![License](https://img.shields.io/github/license/cihai/unihan-db.svg)](https://github.com/cihai/unihan-db/blob/master/LICENSE) [![Code Coverage](https://codecov.io/gh/cihai/unihan-db/branch/master/graph/badge.svg)](https://codecov.io/gh/cihai/unihan-db)
@@ -124,12 +118,16 @@
 
 ```console
 $ cd unihan-etl
 ```
 
 [Bootstrap your environment and learn more about contributing](https://cihai.git-pull.com/contributing/). We use the same conventions / tools across all cihai projects: `pytest`, `sphinx`, `flake8`, `mypy`, `black`, `isort`, `tmuxp`, and file watcher helpers (e.g. `entr(1)`).
 
+## Python versions
+
+- 0.8.0: Last Python 3.7 release
+
 ## More information
 
 [![Docs](https://github.com/cihai/unihan-db/workflows/docs/badge.svg)](https://unihan-db.git-pull.com/)
 [![Build Status](https://github.com/cihai/unihan-db/workflows/tests/badge.svg)](https://github.com/cihai/unihan-db/actions?query=workflow%3A%22tests%22)
```


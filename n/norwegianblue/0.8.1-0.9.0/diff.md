# Comparing `tmp/norwegianblue-0.8.1.tar.gz` & `tmp/norwegianblue-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "norwegianblue-0.8.1.tar", last modified: Tue Jun  7 11:15:43 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `norwegianblue-0.8.1.tar` & `norwegianblue-0.9.0.tar`

### file list

```diff
@@ -1,51 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:43.091397 norwegianblue-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      368 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:43.087397 norwegianblue-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      574 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1765 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (121)      797 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:43.087397 norwegianblue-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (121)      352 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.github/workflows/labels.yml
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.github/workflows/lint.yml
--rw-r--r--   0 runner    (1001) docker     (121)      456 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1356 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6596 2022-06-07 11:15:43.091397 norwegianblue-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5448 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      839 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/RELEASING.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:43.087397 norwegianblue-0.8.1/img/
--rw-r--r--   0 runner    (1001) docker     (121)    13371 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/img/eol-python.png
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:43.087397 norwegianblue-0.8.1/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      478 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/scripts/run_command.py
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-06-07 11:15:43.091397 norwegianblue-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:43.083397 norwegianblue-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:43.087397 norwegianblue-0.8.1/src/norwegianblue/
--rw-r--r--   0 runner    (1001) docker     (121)     6537 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/src/norwegianblue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       73 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/src/norwegianblue/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1299 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/src/norwegianblue/_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     1673 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/src/norwegianblue/_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-07 11:15:41.000000 norwegianblue-0.8.1/src/norwegianblue/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     2211 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/src/norwegianblue/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:43.091397 norwegianblue-0.8.1/src/norwegianblue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6596 2022-06-07 11:15:42.000000 norwegianblue-0.8.1/src/norwegianblue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-06-07 11:15:43.000000 norwegianblue-0.8.1/src/norwegianblue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 11:15:42.000000 norwegianblue-0.8.1/src/norwegianblue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-06-07 11:15:42.000000 norwegianblue-0.8.1/src/norwegianblue.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      160 2022-06-07 11:15:42.000000 norwegianblue-0.8.1/src/norwegianblue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-07 11:15:42.000000 norwegianblue-0.8.1/src/norwegianblue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 11:15:42.000000 norwegianblue-0.8.1/src/norwegianblue.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:43.091397 norwegianblue-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:43.091397 norwegianblue-0.8.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9653 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/tests/data/expected_output.py
--rw-r--r--   0 runner    (1001) docker     (121)     2877 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/tests/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    13327 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/tests/test_norwegianblue.py
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-06-07 11:15:09.000000 norwegianblue-0.8.1/tox.ini
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.coveragerc
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.editorconfig
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.flake8
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/RELEASING.md
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/requirements.txt
+-rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/tox.ini
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.github/labels.yml
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.github/renovate.json
+-rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0      456 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      452 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0    13371 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/img/eol-python.png
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/scripts/run_command.py
+-rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/src/norwegianblue/__init__.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/src/norwegianblue/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/src/norwegianblue/_cache.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/src/norwegianblue/_data.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/src/norwegianblue/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     2913 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/tests/test_cache.py
+-rw-r--r--   0        0        0    12584 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/tests/test_norwegianblue.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/tests/data/__init__.py
+-rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/tests/data/expected_output.py
+-rw-r--r--   0        0        0     4068 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/tests/data/sample_response.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     6990 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/README.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8615 2020-02-02 00:00:00.000000 norwegianblue-0.9.0/PKG-INFO
```

### Comparing `norwegianblue-0.8.1/.github/labels.yml` & `norwegianblue-0.9.0/.github/labels.yml`

 * *Files 8% similar despite different names*

```diff
@@ -45,22 +45,22 @@
   description: "In case of vulnerabilities"
   name: "changelog: Security"
 - color: fbca04
   description: "Exclude PR from release draft"
   name: "changelog: skip"
 
 # Other labels
-- color: 28a745
-  description: "To automatically merge PRs that are ready"
-  name: automerge
 - color: 0366d6
-  description: "For dependencies and dependabot"
+  description: "For dependencies"
   name: dependencies
 - color: f4660e
   description: ""
   name: Hacktoberfest
 - color: f4660e
   description: "To credit accepted Hacktoberfest PRs"
   name: hacktoberfest-accepted
+- color: d65e88
+  description: "Deploy and release"
+  name: release
 - color: fbca04
   description: "Unit tests, linting, CI, etc."
   name: testing
```

### Comparing `norwegianblue-0.8.1/.github/release-drafter.yml` & `norwegianblue-0.9.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `norwegianblue-0.8.1/.github/workflows/deploy.yml` & `norwegianblue-0.9.0/.github/workflows/deploy.yml`

 * *Files 14% similar despite different names*

```diff
@@ -8,45 +8,44 @@
     types:
       - published
   workflow_dispatch:
 
 jobs:
   deploy:
     if: github.repository_owner == 'hugovk'
-    runs-on: ubuntu-20.04
+    runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
 
       - name: Set up Python
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.x"
           cache: pip
-          cache-dependency-path: setup.cfg
+          cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U build twine wheel
 
       - name: Build package
         run: |
-          python setup.py --version
           python -m build
           twine check --strict dist/*
 
       - name: Publish package to PyPI
         if: github.event.action == 'published'
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.PYPI_API_TOKEN }}
 
       - name: Publish package to TestPyPI
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: ${{ secrets.TEST_PYPI_API_TOKEN }}
           repository_url: https://test.pypi.org/legacy/
```

### Comparing `norwegianblue-0.8.1/.github/workflows/test.yml` & `norwegianblue-0.9.0/.github/workflows/test.yml`

 * *Files 14% similar despite different names*

```diff
@@ -7,41 +7,49 @@
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["3.11-dev", "pypy-3.7", "3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.11-dev", "pypy-3.8", "3.7", "3.8", "3.9", "3.10"]
         os: [windows-latest, macos-latest, ubuntu-latest]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v3
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
           cache: pip
-          cache-dependency-path: setup.cfg
+          cache-dependency-path: pyproject.toml
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
           python -m pip install -U wheel
           python -m pip install -U tox
 
       - name: Tox tests
         run: |
           tox -e py
 
       - name: Tox tests (pins)
-        if: matrix.python-version == '3.9' && matrix.os == 'ubuntu-latest'
+        if: matrix.python-version == '3.10' && matrix.os == 'ubuntu-latest'
         shell: bash
         run: |
           tox -e pins
 
       - name: Upload coverage
         uses: codecov/codecov-action@v3
         with:
           flags: ${{ matrix.os }}
           name: ${{ matrix.os }} Python ${{ matrix.python-version }}
+
+  success:
+    needs: test
+    runs-on: ubuntu-latest
+    name: Test successful
+    steps:
+      - name: Success
+        run: echo Test successful
```

### Comparing `norwegianblue-0.8.1/.gitignore` & `norwegianblue-0.9.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -106,10 +106,7 @@
 # mkdocs documentation
 /site
 
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
-
-# Version number generated by setuptools_scm
-_version.py
```

### Comparing `norwegianblue-0.8.1/.pre-commit-config.yaml` & `norwegianblue-0.9.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,56 +1,62 @@
 repos:
   - repo: https://github.com/asottile/pyupgrade
-    rev: v2.32.0
+    rev: v2.37.3
     hooks:
       - id: pyupgrade
         args: [--py37-plus]
 
   - repo: https://github.com/psf/black
-    rev: 22.3.0
+    rev: 22.8.0
     hooks:
       - id: black
         args: [--target-version=py37]
 
   - repo: https://github.com/PyCQA/isort
     rev: 5.10.1
     hooks:
       - id: isort
+        args: [--add-import=from __future__ import annotations]
 
   - repo: https://github.com/PyCQA/flake8
-    rev: 4.0.1
+    rev: 5.0.4
     hooks:
       - id: flake8
         additional_dependencies: [flake8-2020, flake8-implicit-str-concat]
 
   - repo: https://github.com/pre-commit/pygrep-hooks
     rev: v1.9.0
     hooks:
       - id: python-check-blanket-noqa
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.3.0
     hooks:
+      - id: check-json
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: requirements-txt-fixer
 
-  - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v1.20.1
+  - repo: https://github.com/tox-dev/pyproject-fmt
+    rev: 0.3.5
     hooks:
-      - id: setup-cfg-fmt
-        args: [--max-py-version=3.11]
+      - id: pyproject-fmt
+
+  - repo: https://github.com/abravalheri/validate-pyproject
+    rev: v0.10.1
+    hooks:
+      - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: 0.5.2
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.6.2
+    rev: v3.0.0-alpha.0
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `norwegianblue-0.8.1/LICENSE.txt` & `norwegianblue-0.9.0/LICENSE.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2018-2021 Hugo van Kemenade
+Copyright (c) 2018-2022 Hugo van Kemenade
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `norwegianblue-0.8.1/PKG-INFO` & `norwegianblue-0.9.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 Metadata-Version: 2.1
 Name: norwegianblue
-Version: 0.8.1
-Summary: CLI to show end-of-life dates for a number of products.
-Home-page: https://github.com/hugovk/norwegianblue
-Author: hugovk
-License: MIT
-Project-URL: Source, https://github.com/hugovk/norwegianblue
+Version: 0.9.0
+Summary: CLI to show end-of-life dates for a number of products
 Project-URL: Changelog, https://github.com/hugovk/norwegianblue/releases
+Project-URL: Homepage, https://github.com/hugovk/norwegianblue
+Project-URL: Source, https://github.com/hugovk/norwegianblue
+Author: Hugo van Kemenade
+License: MIT
+License-File: LICENSE.txt
 Keywords: end-of-life,endoflife,eol
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+Requires-Dist: httpx>=0.19
+Requires-Dist: platformdirs
+Requires-Dist: prettytable>=2.4
+Requires-Dist: pytablewriter[html]>=0.63
+Requires-Dist: python-dateutil
+Requires-Dist: python-slugify
+Requires-Dist: termcolor
 Provides-Extra: tests
-License-File: LICENSE.txt
+Requires-Dist: freezegun; extra == 'tests'
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-cov; extra == 'tests'
+Requires-Dist: respx>=0.11; extra == 'tests'
+Description-Content-Type: text/markdown
 
 # norwegianblue
 
 [![PyPI version](https://img.shields.io/pypi/v/norwegianblue.svg?logo=pypi&logoColor=FFE873)](https://pypi.org/project/norwegianblue/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/norwegianblue.svg?logo=python&logoColor=FFE873)](https://pypi.org/project/norwegianblue/)
 [![PyPI downloads](https://img.shields.io/pypi/dm/norwegianblue.svg)](https://pypistats.org/packages/norwegianblue)
 [![Test](https://github.com/hugovk/norwegianblue/actions/workflows/test.yml/badge.svg)](https://github.com/hugovk/norwegianblue/actions)
 [![codecov](https://codecov.io/gh/hugovk/norwegianblue/branch/main/graph/badge.svg)](https://codecov.io/gh/hugovk/norwegianblue)
-[![GitHub](https://img.shields.io/github/license/hugovk/norwegianblue.svg)](LICENSE.txt)
+[![Licence](https://img.shields.io/github/license/hugovk/norwegianblue.svg)](LICENSE.txt)
 [![Code style: Black](https://img.shields.io/badge/code%20style-Black-000000.svg)](https://github.com/psf/black)
 
 <p align="center"><img src="https://raw.githubusercontent.com/hugovk/norwegianblue/main/img/eol-python.png" width="319" height="197"></p>
 
 Python interface to [endoflife.date](https://endoflife.date/docs/api/) to show
 end-of-life dates for a number of products.
 
@@ -92,15 +104,15 @@
 options:
   -h, --help            show this help message and exit
   -f {html,json,markdown,rst,tsv}, --format {html,json,markdown,rst,tsv}
                         The format of output (default: markdown)
   -c {yes,no,auto}, --color {yes,no,auto}
                         color terminal output (default: auto)
   --clear-cache         Clear cache before running (default: False)
-  -v, --verbose         Print debug messages to stderr (default: False)
+  -v, --verbose         Print extra messages to stderr (default: 30)
   -V, --version         show program's version number and exit
 ```
 
 <!-- [[[end]]] -->
 
 List all available products with end-of-life dates:
 
@@ -129,69 +141,81 @@
 
 <!-- [[[cog
 run("norwegianblue python")
 ]]] -->
 
 ```console
 $ norwegianblue python
-| cycle | latest |  release   |    eol     |
-|:------|:-------|:----------:|:----------:|
-| 3.10  | 3.10.4 | 2021-10-04 | 2026-10-04 |
-| 3.9   | 3.9.12 | 2020-10-05 | 2025-10-05 |
-| 3.8   | 3.8.13 | 2019-10-14 | 2024-10-14 |
-| 3.7   | 3.7.13 | 2018-06-27 | 2023-06-27 |
-| 3.6   | 3.6.15 | 2016-12-23 | 2021-12-23 |
-| 3.5   | 3.5.10 | 2015-09-13 | 2020-09-13 |
-| 3.4   | 3.4.10 | 2014-03-16 | 2019-03-18 |
-| 3.3   | 3.3.7  | 2012-09-29 | 2017-09-29 |
-| 2.7   | 2.7.18 | 2010-07-03 | 2020-01-01 |
+| cycle |  release   | latest | latest release |    eol     |
+|:------|:----------:|:-------|:--------------:|:----------:|
+| 3.10  | 2021-10-04 | 3.10.5 |   2022-06-06   | 2026-10-04 |
+| 3.9   | 2020-10-05 | 3.9.13 |   2022-05-17   | 2025-10-05 |
+| 3.8   | 2019-10-14 | 3.8.13 |   2022-03-16   | 2024-10-14 |
+| 3.7   | 2018-06-26 | 3.7.13 |   2022-03-16   | 2023-06-27 |
+| 3.6   | 2016-12-22 | 3.6.15 |   2021-09-03   | 2021-12-23 |
+| 3.5   | 2015-09-12 | 3.5.10 |   2020-09-05   | 2020-09-13 |
+| 3.4   | 2014-03-15 | 3.4.10 |   2019-03-18   | 2019-03-18 |
+| 3.3   | 2012-09-29 | 3.3.7  |   2017-09-19   | 2017-09-29 |
+| 2.7   | 2010-07-03 | 2.7.18 |   2020-04-19   | 2020-01-01 |
 ```
 
 <!-- [[[end]]] -->
 
 The table is Markdown, ready for pasting in GitHub issues and PRs:
 
 <!-- [[[cog
 run("norwegianblue python", with_console=False)
 ]]] -->
 
-| cycle | latest |  release   |    eol     |
-| :---- | :----- | :--------: | :--------: |
-| 3.10  | 3.10.4 | 2021-10-04 | 2026-10-04 |
-| 3.9   | 3.9.12 | 2020-10-05 | 2025-10-05 |
-| 3.8   | 3.8.13 | 2019-10-14 | 2024-10-14 |
-| 3.7   | 3.7.13 | 2018-06-27 | 2023-06-27 |
-| 3.6   | 3.6.15 | 2016-12-23 | 2021-12-23 |
-| 3.5   | 3.5.10 | 2015-09-13 | 2020-09-13 |
-| 3.4   | 3.4.10 | 2014-03-16 | 2019-03-18 |
-| 3.3   | 3.3.7  | 2012-09-29 | 2017-09-29 |
-| 2.7   | 2.7.18 | 2010-07-03 | 2020-01-01 |
+| cycle |  release   | latest | latest release |    eol     |
+| :---- | :--------: | :----- | :------------: | :--------: |
+| 3.10  | 2021-10-04 | 3.10.5 |   2022-06-06   | 2026-10-04 |
+| 3.9   | 2020-10-05 | 3.9.13 |   2022-05-17   | 2025-10-05 |
+| 3.8   | 2019-10-14 | 3.8.13 |   2022-03-16   | 2024-10-14 |
+| 3.7   | 2018-06-26 | 3.7.13 |   2022-03-16   | 2023-06-27 |
+| 3.6   | 2016-12-22 | 3.6.15 |   2021-09-03   | 2021-12-23 |
+| 3.5   | 2015-09-12 | 3.5.10 |   2020-09-05   | 2020-09-13 |
+| 3.4   | 2014-03-15 | 3.4.10 |   2019-03-18   | 2019-03-18 |
+| 3.3   | 2012-09-29 | 3.3.7  |   2017-09-19   | 2017-09-29 |
+| 2.7   | 2010-07-03 | 2.7.18 |   2020-04-19   | 2020-01-01 |
 
 <!-- [[[end]]] -->
 
 With options:
 
 <!-- [[[cog
 run("eol nodejs --format rst")
 ]]] -->
 
 ```console
 $ eol nodejs --format rst
 .. table::
 
-    ========  ==========  ============  ============  ============
-     cycle      latest      release       support         eol
-    ========  ==========  ============  ============  ============
-     17        17.8.0      2021-10-19    2022-04-01    2022-06-01
-     16 LTS    16.14.2     2021-04-20    2022-10-18    2024-04-30
-     15        15.14.0     2020-10-20    2021-04-01    2021-06-01
-     14 LTS    14.19.1     2020-04-21    2021-10-19    2023-04-30
-     12 LTS    12.22.11    2019-04-23    2020-10-20    2022-04-30
-     10 LTS    10.24.1     2018-04-24    2020-05-19    2021-04-30
-    ========  ==========  ============  ============  ============
+    ========  ============  ==========  ================  ============  ============
+     cycle      release       latest     latest release     support         eol
+    ========  ============  ==========  ================  ============  ============
+     18 LTS    2022-04-19    18.3.0      2022-06-01        2023-10-18    2025-04-30
+     17        2021-10-19    17.9.1      2022-06-01        2022-04-01    2022-06-01
+     16 LTS    2021-04-20    16.15.1     2022-06-01        2022-10-18    2024-04-30
+     15        2020-10-20    15.14.0     2021-04-06        2021-04-01    2021-06-01
+     14 LTS    2020-04-21    14.19.3     2022-05-17        2021-10-19    2023-04-30
+     13        2019-10-22    13.14.0     2020-04-29        2020-04-01    2020-06-01
+     12 LTS    2019-04-23    12.22.12    2022-04-05        2020-10-20    2022-04-30
+     11        2018-10-23    11.15.0     2019-04-30        2019-04-01    2019-06-30
+     10 LTS    2018-04-24    10.24.1     2021-04-06        2020-05-19    2021-04-30
+     9         2017-10-31    9.11.2      2018-06-12        2018-06-30    2018-06-30
+     8 LTS     2017-05-30    8.17.0      2019-12-17        2019-01-01    2019-12-31
+     7         2016-10-25    7.10.1      2017-07-11        2017-06-30    2017-06-30
+     6 LTS     2016-04-26    6.17.1      2019-04-03        2018-04-30    2019-04-30
+     5         2015-10-30    5.12.0      2016-06-23        2016-06-30    2016-06-30
+     4 LTS     2015-09-09    4.9.1       2018-03-29        2017-04-01    2018-04-30
+     3         2015-08-04    3.3.1       2015-09-15        False         True
+     2         2015-05-04    2.5.0       2015-07-28        False         True
+     1         2015-01-20    1.8.4       2015-07-09        False         True
+    ========  ============  ==========  ================  ============  ============
 ```
 
 <!-- [[[end]]] -->
 
 ## Example programmatic use
 
 Return values are from the JSON responses documented in the API:
```

### Comparing `norwegianblue-0.8.1/RELEASING.md` & `norwegianblue-0.9.0/RELEASING.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,9 +15,9 @@
 - [ ] Check the tagged
       [GitHub Actions build](https://github.com/hugovk/norwegianblue/actions/workflows/deploy.yml)
       has deployed to [PyPI](https://pypi.org/project/norwegianblue/#history)
 
 - [ ] Check installation:
 
 ```bash
-pip3 uninstall -y norwegianblue && pip3 install -U norwegianblue
+pip3 uninstall -y norwegianblue && pip3 install -U norwegianblue && norwegianblue --version
 ```
```

### Comparing `norwegianblue-0.8.1/img/eol-python.png` & `norwegianblue-0.9.0/img/eol-python.png`

 * *Files identical despite different names*

### Comparing `norwegianblue-0.8.1/src/norwegianblue/__init__.py` & `norwegianblue-0.9.0/src/norwegianblue/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-#!/usr/bin/env python3
 """
 Python interface to endoflife.date API
 https://endoflife.date/docs/api/
 """
 from __future__ import annotations
 
 import datetime as dt
@@ -12,15 +11,25 @@
 import sys
 
 from dateutil.relativedelta import relativedelta
 from termcolor import colored
 
 from norwegianblue import _cache
 
-from ._version import version as __version__
+try:
+    # Python 3.8+
+    import importlib.metadata as importlib_metadata
+except ImportError:
+    # Python 3.7
+    import importlib_metadata  # type: ignore
+
+__version__ = importlib_metadata.version(__name__)
+
+
+__all__ = ["__version__"]
 
 BASE_URL = "https://endoflife.date/api/"
 USER_AGENT = f"norwegianblue/{__version__}"
 ERROR_404_TEXT = "Product not found, run 'eol all' for list"
 
 
 def norwegianblue(
@@ -143,28 +152,35 @@
                 cycle[property_] = colored(date_str, "green")
     return data
 
 
 def _tabulate(data: list[dict], format: str = "markdown") -> str:
     """Return data in specified format"""
 
+    # Rename some headers
+    for row in data:
+        if "releaseDate" in row:
+            row["release"] = row.pop("releaseDate")
+        if "latestReleaseDate" in row:
+            row["latest release"] = row.pop("latestReleaseDate")
+
     headers = sorted(set().union(*(d.keys() for d in data)))
 
     # Skip some headers, only used internally at https://endoflife.date
-    for header in ("cycleShortHand", "latestShortHand"):
+    for header in ("cycleShortHand", "latestShortHand", "releaseLabel"):
         if header in headers:
             headers.remove(header)
 
     # Put headers in preferred order, with the rest at the end
     new_headers = []
     for preferred in (
         "cycle",
-        "releaseDate",
+        "release",
         "latest",
-        "latestReleaseDate",
+        "latest release",
         "support",
         "discontinued",
         "eol",
     ):
         if preferred in headers:
             new_headers.append(preferred)
             headers.remove(preferred)
```

### Comparing `norwegianblue-0.8.1/src/norwegianblue/_cache.py` & `norwegianblue-0.9.0/src/norwegianblue/_cache.py`

 * *Files identical despite different names*

### Comparing `norwegianblue-0.8.1/src/norwegianblue/_data.py` & `norwegianblue-0.9.0/src/norwegianblue/_data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 import random
 
 d = {}
 for c in (32, 126):
     for i in range(94):
         d[chr(i + c)] = chr((i + 47) % 94 + c)
```

### Comparing `norwegianblue-0.8.1/src/norwegianblue/cli.py` & `norwegianblue-0.9.0/src/norwegianblue/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,17 +7,20 @@
 * `eol python` to see Python EOLs
 * `eol ubuntu` to see Ubuntu EOLs
 * `eol centos fedora` to see CentOS and Fedora EOLs
 * `eol all` to list all available products
 
 Something missing? Please contribute! https://endoflife.date/contribute
 """
+from __future__ import annotations
+
 import argparse
 import atexit
 import logging
+import platform
 import sys
 
 import norwegianblue
 from norwegianblue import _cache
 
 
 class Formatter(
@@ -46,15 +49,15 @@
         help="The format of output",
     )
     parser.add_argument(
         "-c",
         "--color",
         default="auto",
         choices=("yes", "no", "auto"),
-        help="color terminal output",
+        help="Color the terminal output",
     )
     parser.add_argument(
         "--clear-cache", action="store_true", help="Clear cache before running"
     )
     parser.add_argument(
         "-v",
         "--verbose",
@@ -64,15 +67,16 @@
         default=logging.WARNING,
         help="Print extra messages to stderr",
     )
     parser.add_argument(
         "-V",
         "--version",
         action="version",
-        version=f"%(prog)s {norwegianblue.__version__}",
+        version=f"%(prog)s {norwegianblue.__version__} "
+        f"(Python {platform.python_version()})",
     )
     args = parser.parse_args()
 
     logging.basicConfig(level=args.loglevel, format="%(message)s")
     if args.clear_cache:
         _cache.clear(clear_all=True)
```

### Comparing `norwegianblue-0.8.1/tests/data/expected_output.py` & `norwegianblue-0.9.0/tests/data/expected_output.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,604 +1,666 @@
-00000000: 4558 5045 4354 4544 5f48 544d 4c20 3d20  EXPECTED_HTML = 
-00000010: 2222 220a 3c74 6162 6c65 3e0a 2020 2020  """.<table>.    
-00000020: 3c74 6865 6164 3e0a 2020 2020 2020 2020  <thead>.        
-00000030: 3c74 723e 0a20 2020 2020 2020 2020 2020  <tr>.           
-00000040: 203c 7468 3e63 7963 6c65 3c2f 7468 3e0a   <th>cycle</th>.
-00000050: 2020 2020 2020 2020 2020 2020 3c74 683e              <th>
-00000060: 7265 6c65 6173 6544 6174 653c 2f74 683e  releaseDate</th>
-00000070: 0a20 2020 2020 2020 2020 2020 203c 7468  .            <th
-00000080: 3e6c 6174 6573 743c 2f74 683e 0a20 2020  >latest</th>.   
-00000090: 2020 2020 2020 2020 203c 7468 3e73 7570           <th>sup
-000000a0: 706f 7274 3c2f 7468 3e0a 2020 2020 2020  port</th>.      
-000000b0: 2020 2020 2020 3c74 683e 656f 6c3c 2f74        <th>eol</t
-000000c0: 683e 0a20 2020 2020 2020 2020 2020 203c  h>.            <
-000000d0: 7468 3e63 6f64 656e 616d 653c 2f74 683e  th>codename</th>
-000000e0: 0a20 2020 2020 2020 2020 2020 203c 7468  .            <th
-000000f0: 3e6c 696e 6b3c 2f74 683e 0a20 2020 2020  >link</th>.     
-00000100: 2020 203c 2f74 723e 0a20 2020 203c 2f74     </tr>.    </t
-00000110: 6865 6164 3e0a 2020 2020 3c74 626f 6479  head>.    <tbody
-00000120: 3e0a 2020 2020 2020 2020 3c74 723e 0a20  >.        <tr>. 
-00000130: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
-00000140: 6c69 676e 3d22 6c65 6674 223e 3232 2e30  lign="left">22.0
-00000150: 3420 4c54 533c 2f74 643e 0a20 2020 2020  4 LTS</td>.     
-00000160: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
-00000170: 3d22 6c65 6674 223e 3230 3232 2d30 342d  ="left">2022-04-
-00000180: 3231 3c2f 7464 3e0a 2020 2020 2020 2020  21</td>.        
-00000190: 2020 2020 3c74 6420 616c 6967 6e3d 226c      <td align="l
-000001a0: 6566 7422 3e32 322e 3034 3c2f 7464 3e0a  eft">22.04</td>.
-000001b0: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
-000001c0: 616c 6967 6e3d 226c 6566 7422 3e32 3032  align="left">202
-000001d0: 372d 3034 2d30 323c 2f74 643e 0a20 2020  7-04-02</td>.   
-000001e0: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
-000001f0: 676e 3d22 6c65 6674 223e 3230 3332 2d30  gn="left">2032-0
-00000200: 342d 3031 3c2f 7464 3e0a 2020 2020 2020  4-01</td>.      
-00000210: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
-00000220: 226c 6566 7422 3e4a 616d 6d79 204a 656c  "left">Jammy Jel
-00000230: 6c79 6669 7368 3c2f 7464 3e0a 2020 2020  lyfish</td>.    
-00000240: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
-00000250: 6e3d 226c 6566 7422 3e68 7474 7073 3a2f  n="left">https:/
-00000260: 2f77 696b 692e 7562 756e 7475 2e63 6f6d  /wiki.ubuntu.com
-00000270: 2f4a 616d 6d79 4a65 6c6c 7966 6973 682f  /JammyJellyfish/
-00000280: 5265 6c65 6173 654e 6f74 6573 2f3c 2f74  ReleaseNotes/</t
-00000290: 643e 0a20 2020 2020 2020 203c 2f74 723e  d>.        </tr>
-000002a0: 0a20 2020 2020 2020 203c 7472 3e0a 2020  .        <tr>.  
-000002b0: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
-000002c0: 6967 6e3d 226c 6566 7422 3e32 312e 3130  ign="left">21.10
-000002d0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-000002e0: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
-000002f0: 7422 3e32 3032 312d 3130 2d31 343c 2f74  t">2021-10-14</t
-00000300: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
-00000310: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
-00000320: 3231 2e31 303c 2f74 643e 0a20 2020 2020  21.10</td>.     
-00000330: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
-00000340: 3d22 6c65 6674 223e 3230 3232 2d30 372d  ="left">2022-07-
-00000350: 3331 3c2f 7464 3e0a 2020 2020 2020 2020  31</td>.        
-00000360: 2020 2020 3c74 6420 616c 6967 6e3d 226c      <td align="l
-00000370: 6566 7422 3e32 3032 322d 3037 2d33 313c  eft">2022-07-31<
-00000380: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
-00000390: 203c 7464 2061 6c69 676e 3d22 6c65 6674   <td align="left
-000003a0: 223e 496d 7069 7368 2049 6e64 7269 3c2f  ">Impish Indri</
-000003b0: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
-000003c0: 3c74 6420 616c 6967 6e3d 226c 6566 7422  <td align="left"
-000003d0: 3e68 7474 7073 3a2f 2f77 696b 692e 7562  >https://wiki.ub
-000003e0: 756e 7475 2e63 6f6d 2f49 6d70 6973 6849  untu.com/ImpishI
-000003f0: 6e64 7269 2f52 656c 6561 7365 4e6f 7465  ndri/ReleaseNote
-00000400: 732f 3c2f 7464 3e0a 2020 2020 2020 2020  s/</td>.        
-00000410: 3c2f 7472 3e0a 2020 2020 2020 2020 3c74  </tr>.        <t
-00000420: 723e 0a20 2020 2020 2020 2020 2020 203c  r>.            <
-00000430: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
-00000440: 3231 2e30 343c 2f74 643e 0a20 2020 2020  21.04</td>.     
-00000450: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
-00000460: 3d22 6c65 6674 223e 3230 3231 2d30 342d  ="left">2021-04-
-00000470: 3232 3c2f 7464 3e0a 2020 2020 2020 2020  22</td>.        
-00000480: 2020 2020 3c74 6420 616c 6967 6e3d 226c      <td align="l
-00000490: 6566 7422 3e32 312e 3034 3c2f 7464 3e0a  eft">21.04</td>.
-000004a0: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
-000004b0: 616c 6967 6e3d 226c 6566 7422 3e32 3032  align="left">202
-000004c0: 322d 3031 2d32 303c 2f74 643e 0a20 2020  2-01-20</td>.   
-000004d0: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
-000004e0: 676e 3d22 6c65 6674 223e 3230 3232 2d30  gn="left">2022-0
-000004f0: 312d 3230 3c2f 7464 3e0a 2020 2020 2020  1-20</td>.      
-00000500: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
-00000510: 226c 6566 7422 3e48 6972 7375 7465 2048  "left">Hirsute H
-00000520: 6970 706f 3c2f 7464 3e0a 2020 2020 2020  ippo</td>.      
-00000530: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
-00000540: 226c 6566 7422 3e68 7474 7073 3a2f 2f77  "left">https://w
-00000550: 696b 692e 7562 756e 7475 2e63 6f6d 2f48  iki.ubuntu.com/H
-00000560: 6972 7375 7465 4869 7070 6f2f 5265 6c65  irsuteHippo/Rele
-00000570: 6173 654e 6f74 6573 2f3c 2f74 643e 0a20  aseNotes/</td>. 
-00000580: 2020 2020 2020 203c 2f74 723e 0a20 2020         </tr>.   
-00000590: 2020 2020 203c 7472 3e0a 2020 2020 2020       <tr>.      
-000005a0: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
-000005b0: 226c 6566 7422 3e32 302e 3130 3c2f 7464  "left">20.10</td
-000005c0: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
-000005d0: 6420 616c 6967 6e3d 226c 6566 7422 3e32  d align="left">2
-000005e0: 3032 302d 3130 2d32 323c 2f74 643e 0a20  020-10-22</td>. 
-000005f0: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
-00000600: 6c69 676e 3d22 6c65 6674 223e 3230 2e31  lign="left">20.1
-00000610: 303c 2f74 643e 0a20 2020 2020 2020 2020  0</td>.         
-00000620: 2020 203c 7464 2061 6c69 676e 3d22 6c65     <td align="le
-00000630: 6674 223e 3230 3231 2d30 372d 3232 3c2f  ft">2021-07-22</
-00000640: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
-00000650: 3c74 6420 616c 6967 6e3d 226c 6566 7422  <td align="left"
-00000660: 3e32 3032 312d 3037 2d32 323c 2f74 643e  >2021-07-22</td>
-00000670: 0a20 2020 2020 2020 2020 2020 203c 7464  .            <td
-00000680: 2061 6c69 676e 3d22 6c65 6674 223e 4772   align="left">Gr
-00000690: 6f6f 7679 2047 6f72 696c 6c61 3c2f 7464  oovy Gorilla</td
-000006a0: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
-000006b0: 6420 616c 6967 6e3d 226c 6566 7422 3e3c  d align="left"><
-000006c0: 2f74 643e 0a20 2020 2020 2020 203c 2f74  /td>.        </t
-000006d0: 723e 0a20 2020 2020 2020 203c 7472 3e0a  r>.        <tr>.
-000006e0: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
-000006f0: 616c 6967 6e3d 226c 6566 7422 3e32 302e  align="left">20.
-00000700: 3034 204c 5453 3c2f 7464 3e0a 2020 2020  04 LTS</td>.    
-00000710: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
-00000720: 6e3d 226c 6566 7422 3e32 3032 302d 3034  n="left">2020-04
-00000730: 2d32 333c 2f74 643e 0a20 2020 2020 2020  -23</td>.       
-00000740: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
-00000750: 6c65 6674 223e 3230 2e30 342e 343c 2f74  left">20.04.4</t
-00000760: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
-00000770: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
-00000780: 3230 3235 2d30 342d 3032 3c2f 7464 3e0a  2025-04-02</td>.
-00000790: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
-000007a0: 616c 6967 6e3d 226c 6566 7422 3e32 3033  align="left">203
-000007b0: 302d 3034 2d30 313c 2f74 643e 0a20 2020  0-04-01</td>.   
-000007c0: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
-000007d0: 676e 3d22 6c65 6674 223e 466f 6361 6c20  gn="left">Focal 
-000007e0: 466f 7373 613c 2f74 643e 0a20 2020 2020  Fossa</td>.     
-000007f0: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
-00000800: 3d22 6c65 6674 223e 3c2f 7464 3e0a 2020  ="left"></td>.  
-00000810: 2020 2020 2020 3c2f 7472 3e0a 2020 2020        </tr>.    
-00000820: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
-00000830: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
-00000840: 6c65 6674 223e 3139 2e31 303c 2f74 643e  left">19.10</td>
-00000850: 0a20 2020 2020 2020 2020 2020 203c 7464  .            <td
-00000860: 2061 6c69 676e 3d22 6c65 6674 223e 3230   align="left">20
-00000870: 3139 2d31 302d 3137 3c2f 7464 3e0a 2020  19-10-17</td>.  
-00000880: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
-00000890: 6967 6e3d 226c 6566 7422 3e31 392e 3130  ign="left">19.10
-000008a0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-000008b0: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
-000008c0: 7422 3e32 3032 302d 3037 2d30 363c 2f74  t">2020-07-06</t
-000008d0: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
-000008e0: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
-000008f0: 3230 3230 2d30 372d 3036 3c2f 7464 3e0a  2020-07-06</td>.
-00000900: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
-00000910: 616c 6967 6e3d 226c 6566 7422 3e4b 6172  align="left">Kar
-00000920: 6d69 6320 4b6f 616c 613c 2f74 643e 0a20  mic Koala</td>. 
-00000930: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
-00000940: 6c69 676e 3d22 6c65 6674 223e 3c2f 7464  lign="left"></td
-00000950: 3e0a 2020 2020 2020 2020 3c2f 7472 3e0a  >.        </tr>.
-00000960: 2020 2020 2020 2020 3c74 723e 0a20 2020          <tr>.   
-00000970: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
-00000980: 676e 3d22 6c65 6674 223e 3138 2e30 3420  gn="left">18.04 
-00000990: 4c54 533c 2f74 643e 0a20 2020 2020 2020  LTS</td>.       
-000009a0: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
-000009b0: 6c65 6674 223e 3230 3138 2d30 342d 3236  left">2018-04-26
-000009c0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-000009d0: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
-000009e0: 7422 3e31 382e 3034 2e36 3c2f 7464 3e0a  t">18.04.6</td>.
-000009f0: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
-00000a00: 616c 6967 6e3d 226c 6566 7422 3e32 3032  align="left">202
-00000a10: 332d 3034 2d30 323c 2f74 643e 0a20 2020  3-04-02</td>.   
-00000a20: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
-00000a30: 676e 3d22 6c65 6674 223e 3230 3238 2d30  gn="left">2028-0
-00000a40: 342d 3031 3c2f 7464 3e0a 2020 2020 2020  4-01</td>.      
-00000a50: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
-00000a60: 226c 6566 7422 3e42 696f 6e69 6320 4265  "left">Bionic Be
-00000a70: 6176 6572 3c2f 7464 3e0a 2020 2020 2020  aver</td>.      
-00000a80: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
-00000a90: 226c 6566 7422 3e68 7474 7073 3a2f 2f77  "left">https://w
-00000aa0: 696b 692e 7562 756e 7475 2e63 6f6d 2f42  iki.ubuntu.com/B
-00000ab0: 696f 6e69 6342 6561 7665 722f 5265 6c65  ionicBeaver/Rele
-00000ac0: 6173 654e 6f74 6573 3c2f 7464 3e0a 2020  aseNotes</td>.  
-00000ad0: 2020 2020 2020 3c2f 7472 3e0a 2020 2020        </tr>.    
-00000ae0: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
-00000af0: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
-00000b00: 6c65 6674 223e 3136 2e30 3420 4c54 533c  left">16.04 LTS<
-00000b10: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
-00000b20: 203c 7464 2061 6c69 676e 3d22 6c65 6674   <td align="left
-00000b30: 223e 3230 3136 2d30 342d 3231 3c2f 7464  ">2016-04-21</td
-00000b40: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
-00000b50: 6420 616c 6967 6e3d 226c 6566 7422 3e31  d align="left">1
-00000b60: 362e 3034 2e37 3c2f 7464 3e0a 2020 2020  6.04.7</td>.    
-00000b70: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
-00000b80: 6e3d 226c 6566 7422 3e32 3032 312d 3034  n="left">2021-04
-00000b90: 2d30 323c 2f74 643e 0a20 2020 2020 2020  -02</td>.       
-00000ba0: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
-00000bb0: 6c65 6674 223e 3230 3236 2d30 342d 3031  left">2026-04-01
-00000bc0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-00000bd0: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
-00000be0: 7422 3e58 656e 6961 6c20 5865 7275 733c  t">Xenial Xerus<
-00000bf0: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
-00000c00: 203c 7464 2061 6c69 676e 3d22 6c65 6674   <td align="left
-00000c10: 223e 3c2f 7464 3e0a 2020 2020 2020 2020  "></td>.        
-00000c20: 3c2f 7472 3e0a 2020 2020 2020 2020 3c74  </tr>.        <t
-00000c30: 723e 0a20 2020 2020 2020 2020 2020 203c  r>.            <
-00000c40: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
-00000c50: 3134 2e30 3420 4c54 533c 2f74 643e 0a20  14.04 LTS</td>. 
-00000c60: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
-00000c70: 6c69 676e 3d22 6c65 6674 223e 3230 3134  lign="left">2014
-00000c80: 2d30 342d 3137 3c2f 7464 3e0a 2020 2020  -04-17</td>.    
-00000c90: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
-00000ca0: 6e3d 226c 6566 7422 3e31 342e 3034 2e36  n="left">14.04.6
-00000cb0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
-00000cc0: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
-00000cd0: 7422 3e32 3031 392d 3034 2d30 323c 2f74  t">2019-04-02</t
-00000ce0: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
-00000cf0: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
-00000d00: 3230 3234 2d30 342d 3031 3c2f 7464 3e0a  2024-04-01</td>.
-00000d10: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
-00000d20: 616c 6967 6e3d 226c 6566 7422 3e54 7275  align="left">Tru
-00000d30: 7374 7920 5461 6872 3c2f 7464 3e0a 2020  sty Tahr</td>.  
-00000d40: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
-00000d50: 6967 6e3d 226c 6566 7422 3e3c 2f74 643e  ign="left"></td>
-00000d60: 0a20 2020 2020 2020 203c 2f74 723e 0a20  .        </tr>. 
-00000d70: 2020 203c 2f74 626f 6479 3e0a 3c2f 7461     </tbody>.</ta
-00000d80: 626c 653e 0a22 2222 0a0a 4558 5045 4354  ble>."""..EXPECT
-00000d90: 4544 5f4d 4420 3d20 2222 220a 7c20 6379  ED_MD = """.| cy
-00000da0: 636c 6520 2020 2020 7c20 7265 6c65 6173  cle     | releas
-00000db0: 6544 6174 6520 7c20 6c61 7465 7374 2020  eDate | latest  
-00000dc0: 7c20 2073 7570 706f 7274 2020 207c 2020  |  support   |  
-00000dd0: 2020 656f 6c20 2020 2020 7c20 2020 2020    eol     |     
-00000de0: 636f 6465 6e61 6d65 2020 2020 7c20 6c69  codename    | li
-00000df0: 6e6b 2020 2020 2020 2020 2020 2020 2020  nk              
-00000e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e20: 2020 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d     |.|:---------
-00000e30: 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  -|:-----------:|
-00000e40: 3a2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d  :--------|:-----
-00000e50: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-00000e60: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
-00000e70: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
-00000e80: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000e90: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-00000ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20  ------------|.| 
-00000eb0: 3232 2e30 3420 4c54 5320 7c20 2032 3032  22.04 LTS |  202
-00000ec0: 322d 3034 2d32 3120 7c20 3232 2e30 3420  2-04-21 | 22.04 
-00000ed0: 2020 7c20 3230 3237 2d30 342d 3032 207c    | 2027-04-02 |
-00000ee0: 2032 3033 322d 3034 2d30 3120 7c20 4a61   2032-04-01 | Ja
-00000ef0: 6d6d 7920 4a65 6c6c 7966 6973 6820 7c20  mmy Jellyfish | 
-00000f00: 6874 7470 733a 2f2f 7769 6b69 2e75 6275  https://wiki.ubu
-00000f10: 6e74 752e 636f 6d2f 4a61 6d6d 794a 656c  ntu.com/JammyJel
-00000f20: 6c79 6669 7368 2f52 656c 6561 7365 4e6f  lyfish/ReleaseNo
-00000f30: 7465 732f 207c 0a7c 2032 312e 3130 2020  tes/ |.| 21.10  
-00000f40: 2020 207c 2020 3230 3231 2d31 302d 3134     |  2021-10-14
-00000f50: 207c 2032 312e 3130 2020 207c 2032 3032   | 21.10   | 202
-00000f60: 322d 3037 2d33 3120 7c20 3230 3232 2d30  2-07-31 | 2022-0
-00000f70: 372d 3331 207c 2020 2049 6d70 6973 6820  7-31 |   Impish 
-00000f80: 496e 6472 6920 207c 2068 7474 7073 3a2f  Indri  | https:/
-00000f90: 2f77 696b 692e 7562 756e 7475 2e63 6f6d  /wiki.ubuntu.com
-00000fa0: 2f49 6d70 6973 6849 6e64 7269 2f52 656c  /ImpishIndri/Rel
-00000fb0: 6561 7365 4e6f 7465 732f 2020 2020 7c0a  easeNotes/    |.
-00000fc0: 7c20 3231 2e30 3420 2020 2020 7c20 2032  | 21.04     |  2
-00000fd0: 3032 312d 3034 2d32 3220 7c20 3231 2e30  021-04-22 | 21.0
-00000fe0: 3420 2020 7c20 3230 3232 2d30 312d 3230  4   | 2022-01-20
-00000ff0: 207c 2032 3032 322d 3031 2d32 3020 7c20   | 2022-01-20 | 
-00001000: 2048 6972 7375 7465 2048 6970 706f 2020   Hirsute Hippo  
-00001010: 7c20 6874 7470 733a 2f2f 7769 6b69 2e75  | https://wiki.u
-00001020: 6275 6e74 752e 636f 6d2f 4869 7273 7574  buntu.com/Hirsut
-00001030: 6548 6970 706f 2f52 656c 6561 7365 4e6f  eHippo/ReleaseNo
-00001040: 7465 732f 2020 207c 0a7c 2032 302e 3130  tes/   |.| 20.10
-00001050: 2020 2020 207c 2020 3230 3230 2d31 302d       |  2020-10-
-00001060: 3232 207c 2032 302e 3130 2020 207c 2032  22 | 20.10   | 2
-00001070: 3032 312d 3037 2d32 3220 7c20 3230 3231  021-07-22 | 2021
-00001080: 2d30 372d 3232 207c 2020 4772 6f6f 7679  -07-22 |  Groovy
-00001090: 2047 6f72 696c 6c61 207c 2020 2020 2020   Gorilla |      
-000010a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000000: 6672 6f6d 205f 5f66 7574 7572 655f 5f20  from __future__ 
+00000010: 696d 706f 7274 2061 6e6e 6f74 6174 696f  import annotatio
+00000020: 6e73 0a0a 4558 5045 4354 4544 5f48 544d  ns..EXPECTED_HTM
+00000030: 4c20 3d20 2222 220a 3c74 6162 6c65 3e0a  L = """.<table>.
+00000040: 2020 2020 3c74 6865 6164 3e0a 2020 2020      <thead>.    
+00000050: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+00000060: 2020 2020 203c 7468 3e63 7963 6c65 3c2f       <th>cycle</
+00000070: 7468 3e0a 2020 2020 2020 2020 2020 2020  th>.            
+00000080: 3c74 683e 7265 6c65 6173 653c 2f74 683e  <th>release</th>
+00000090: 0a20 2020 2020 2020 2020 2020 203c 7468  .            <th
+000000a0: 3e6c 6174 6573 743c 2f74 683e 0a20 2020  >latest</th>.   
+000000b0: 2020 2020 2020 2020 203c 7468 3e73 7570           <th>sup
+000000c0: 706f 7274 3c2f 7468 3e0a 2020 2020 2020  port</th>.      
+000000d0: 2020 2020 2020 3c74 683e 656f 6c3c 2f74        <th>eol</t
+000000e0: 683e 0a20 2020 2020 2020 2020 2020 203c  h>.            <
+000000f0: 7468 3e63 6f64 656e 616d 653c 2f74 683e  th>codename</th>
+00000100: 0a20 2020 2020 2020 2020 2020 203c 7468  .            <th
+00000110: 3e6c 696e 6b3c 2f74 683e 0a20 2020 2020  >link</th>.     
+00000120: 2020 203c 2f74 723e 0a20 2020 203c 2f74     </tr>.    </t
+00000130: 6865 6164 3e0a 2020 2020 3c74 626f 6479  head>.    <tbody
+00000140: 3e0a 2020 2020 2020 2020 3c74 723e 0a20  >.        <tr>. 
+00000150: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
+00000160: 6c69 676e 3d22 6c65 6674 223e 3232 2e30  lign="left">22.0
+00000170: 3420 4c54 533c 2f74 643e 0a20 2020 2020  4 LTS</td>.     
+00000180: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
+00000190: 3d22 6c65 6674 223e 3230 3232 2d30 342d  ="left">2022-04-
+000001a0: 3231 3c2f 7464 3e0a 2020 2020 2020 2020  21</td>.        
+000001b0: 2020 2020 3c74 6420 616c 6967 6e3d 226c      <td align="l
+000001c0: 6566 7422 3e32 322e 3034 3c2f 7464 3e0a  eft">22.04</td>.
+000001d0: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+000001e0: 616c 6967 6e3d 226c 6566 7422 3e32 3032  align="left">202
+000001f0: 372d 3034 2d30 323c 2f74 643e 0a20 2020  7-04-02</td>.   
+00000200: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
+00000210: 676e 3d22 6c65 6674 223e 3230 3332 2d30  gn="left">2032-0
+00000220: 342d 3031 3c2f 7464 3e0a 2020 2020 2020  4-01</td>.      
+00000230: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
+00000240: 226c 6566 7422 3e4a 616d 6d79 204a 656c  "left">Jammy Jel
+00000250: 6c79 6669 7368 3c2f 7464 3e0a 2020 2020  lyfish</td>.    
+00000260: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
+00000270: 6e3d 226c 6566 7422 3e68 7474 7073 3a2f  n="left">https:/
+00000280: 2f77 696b 692e 7562 756e 7475 2e63 6f6d  /wiki.ubuntu.com
+00000290: 2f4a 616d 6d79 4a65 6c6c 7966 6973 682f  /JammyJellyfish/
+000002a0: 5265 6c65 6173 654e 6f74 6573 2f3c 2f74  ReleaseNotes/</t
+000002b0: 643e 0a20 2020 2020 2020 203c 2f74 723e  d>.        </tr>
+000002c0: 0a20 2020 2020 2020 203c 7472 3e0a 2020  .        <tr>.  
+000002d0: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
+000002e0: 6967 6e3d 226c 6566 7422 3e32 312e 3130  ign="left">21.10
+000002f0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+00000300: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
+00000310: 7422 3e32 3032 312d 3130 2d31 343c 2f74  t">2021-10-14</t
+00000320: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
+00000330: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
+00000340: 3231 2e31 303c 2f74 643e 0a20 2020 2020  21.10</td>.     
+00000350: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
+00000360: 3d22 6c65 6674 223e 3230 3232 2d30 372d  ="left">2022-07-
+00000370: 3331 3c2f 7464 3e0a 2020 2020 2020 2020  31</td>.        
+00000380: 2020 2020 3c74 6420 616c 6967 6e3d 226c      <td align="l
+00000390: 6566 7422 3e32 3032 322d 3037 2d33 313c  eft">2022-07-31<
+000003a0: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
+000003b0: 203c 7464 2061 6c69 676e 3d22 6c65 6674   <td align="left
+000003c0: 223e 496d 7069 7368 2049 6e64 7269 3c2f  ">Impish Indri</
+000003d0: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
+000003e0: 3c74 6420 616c 6967 6e3d 226c 6566 7422  <td align="left"
+000003f0: 3e68 7474 7073 3a2f 2f77 696b 692e 7562  >https://wiki.ub
+00000400: 756e 7475 2e63 6f6d 2f49 6d70 6973 6849  untu.com/ImpishI
+00000410: 6e64 7269 2f52 656c 6561 7365 4e6f 7465  ndri/ReleaseNote
+00000420: 732f 3c2f 7464 3e0a 2020 2020 2020 2020  s/</td>.        
+00000430: 3c2f 7472 3e0a 2020 2020 2020 2020 3c74  </tr>.        <t
+00000440: 723e 0a20 2020 2020 2020 2020 2020 203c  r>.            <
+00000450: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
+00000460: 3231 2e30 343c 2f74 643e 0a20 2020 2020  21.04</td>.     
+00000470: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
+00000480: 3d22 6c65 6674 223e 3230 3231 2d30 342d  ="left">2021-04-
+00000490: 3232 3c2f 7464 3e0a 2020 2020 2020 2020  22</td>.        
+000004a0: 2020 2020 3c74 6420 616c 6967 6e3d 226c      <td align="l
+000004b0: 6566 7422 3e32 312e 3034 3c2f 7464 3e0a  eft">21.04</td>.
+000004c0: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+000004d0: 616c 6967 6e3d 226c 6566 7422 3e32 3032  align="left">202
+000004e0: 322d 3031 2d32 303c 2f74 643e 0a20 2020  2-01-20</td>.   
+000004f0: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
+00000500: 676e 3d22 6c65 6674 223e 3230 3232 2d30  gn="left">2022-0
+00000510: 312d 3230 3c2f 7464 3e0a 2020 2020 2020  1-20</td>.      
+00000520: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
+00000530: 226c 6566 7422 3e48 6972 7375 7465 2048  "left">Hirsute H
+00000540: 6970 706f 3c2f 7464 3e0a 2020 2020 2020  ippo</td>.      
+00000550: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
+00000560: 226c 6566 7422 3e68 7474 7073 3a2f 2f77  "left">https://w
+00000570: 696b 692e 7562 756e 7475 2e63 6f6d 2f48  iki.ubuntu.com/H
+00000580: 6972 7375 7465 4869 7070 6f2f 5265 6c65  irsuteHippo/Rele
+00000590: 6173 654e 6f74 6573 2f3c 2f74 643e 0a20  aseNotes/</td>. 
+000005a0: 2020 2020 2020 203c 2f74 723e 0a20 2020         </tr>.   
+000005b0: 2020 2020 203c 7472 3e0a 2020 2020 2020       <tr>.      
+000005c0: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
+000005d0: 226c 6566 7422 3e32 302e 3130 3c2f 7464  "left">20.10</td
+000005e0: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
+000005f0: 6420 616c 6967 6e3d 226c 6566 7422 3e32  d align="left">2
+00000600: 3032 302d 3130 2d32 323c 2f74 643e 0a20  020-10-22</td>. 
+00000610: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
+00000620: 6c69 676e 3d22 6c65 6674 223e 3230 2e31  lign="left">20.1
+00000630: 303c 2f74 643e 0a20 2020 2020 2020 2020  0</td>.         
+00000640: 2020 203c 7464 2061 6c69 676e 3d22 6c65     <td align="le
+00000650: 6674 223e 3230 3231 2d30 372d 3232 3c2f  ft">2021-07-22</
+00000660: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
+00000670: 3c74 6420 616c 6967 6e3d 226c 6566 7422  <td align="left"
+00000680: 3e32 3032 312d 3037 2d32 323c 2f74 643e  >2021-07-22</td>
+00000690: 0a20 2020 2020 2020 2020 2020 203c 7464  .            <td
+000006a0: 2061 6c69 676e 3d22 6c65 6674 223e 4772   align="left">Gr
+000006b0: 6f6f 7679 2047 6f72 696c 6c61 3c2f 7464  oovy Gorilla</td
+000006c0: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
+000006d0: 6420 616c 6967 6e3d 226c 6566 7422 3e3c  d align="left"><
+000006e0: 2f74 643e 0a20 2020 2020 2020 203c 2f74  /td>.        </t
+000006f0: 723e 0a20 2020 2020 2020 203c 7472 3e0a  r>.        <tr>.
+00000700: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+00000710: 616c 6967 6e3d 226c 6566 7422 3e32 302e  align="left">20.
+00000720: 3034 204c 5453 3c2f 7464 3e0a 2020 2020  04 LTS</td>.    
+00000730: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
+00000740: 6e3d 226c 6566 7422 3e32 3032 302d 3034  n="left">2020-04
+00000750: 2d32 333c 2f74 643e 0a20 2020 2020 2020  -23</td>.       
+00000760: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
+00000770: 6c65 6674 223e 3230 2e30 342e 343c 2f74  left">20.04.4</t
+00000780: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
+00000790: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
+000007a0: 3230 3235 2d30 342d 3032 3c2f 7464 3e0a  2025-04-02</td>.
+000007b0: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+000007c0: 616c 6967 6e3d 226c 6566 7422 3e32 3033  align="left">203
+000007d0: 302d 3034 2d30 313c 2f74 643e 0a20 2020  0-04-01</td>.   
+000007e0: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
+000007f0: 676e 3d22 6c65 6674 223e 466f 6361 6c20  gn="left">Focal 
+00000800: 466f 7373 613c 2f74 643e 0a20 2020 2020  Fossa</td>.     
+00000810: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
+00000820: 3d22 6c65 6674 223e 3c2f 7464 3e0a 2020  ="left"></td>.  
+00000830: 2020 2020 2020 3c2f 7472 3e0a 2020 2020        </tr>.    
+00000840: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+00000850: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
+00000860: 6c65 6674 223e 3139 2e31 303c 2f74 643e  left">19.10</td>
+00000870: 0a20 2020 2020 2020 2020 2020 203c 7464  .            <td
+00000880: 2061 6c69 676e 3d22 6c65 6674 223e 3230   align="left">20
+00000890: 3139 2d31 302d 3137 3c2f 7464 3e0a 2020  19-10-17</td>.  
+000008a0: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
+000008b0: 6967 6e3d 226c 6566 7422 3e31 392e 3130  ign="left">19.10
+000008c0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+000008d0: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
+000008e0: 7422 3e32 3032 302d 3037 2d30 363c 2f74  t">2020-07-06</t
+000008f0: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
+00000900: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
+00000910: 3230 3230 2d30 372d 3036 3c2f 7464 3e0a  2020-07-06</td>.
+00000920: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+00000930: 616c 6967 6e3d 226c 6566 7422 3e4b 6172  align="left">Kar
+00000940: 6d69 6320 4b6f 616c 613c 2f74 643e 0a20  mic Koala</td>. 
+00000950: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
+00000960: 6c69 676e 3d22 6c65 6674 223e 3c2f 7464  lign="left"></td
+00000970: 3e0a 2020 2020 2020 2020 3c2f 7472 3e0a  >.        </tr>.
+00000980: 2020 2020 2020 2020 3c74 723e 0a20 2020          <tr>.   
+00000990: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
+000009a0: 676e 3d22 6c65 6674 223e 3138 2e30 3420  gn="left">18.04 
+000009b0: 4c54 533c 2f74 643e 0a20 2020 2020 2020  LTS</td>.       
+000009c0: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
+000009d0: 6c65 6674 223e 3230 3138 2d30 342d 3236  left">2018-04-26
+000009e0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+000009f0: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
+00000a00: 7422 3e31 382e 3034 2e36 3c2f 7464 3e0a  t">18.04.6</td>.
+00000a10: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+00000a20: 616c 6967 6e3d 226c 6566 7422 3e32 3032  align="left">202
+00000a30: 332d 3034 2d30 323c 2f74 643e 0a20 2020  3-04-02</td>.   
+00000a40: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
+00000a50: 676e 3d22 6c65 6674 223e 3230 3238 2d30  gn="left">2028-0
+00000a60: 342d 3031 3c2f 7464 3e0a 2020 2020 2020  4-01</td>.      
+00000a70: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
+00000a80: 226c 6566 7422 3e42 696f 6e69 6320 4265  "left">Bionic Be
+00000a90: 6176 6572 3c2f 7464 3e0a 2020 2020 2020  aver</td>.      
+00000aa0: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
+00000ab0: 226c 6566 7422 3e68 7474 7073 3a2f 2f77  "left">https://w
+00000ac0: 696b 692e 7562 756e 7475 2e63 6f6d 2f42  iki.ubuntu.com/B
+00000ad0: 696f 6e69 6342 6561 7665 722f 5265 6c65  ionicBeaver/Rele
+00000ae0: 6173 654e 6f74 6573 3c2f 7464 3e0a 2020  aseNotes</td>.  
+00000af0: 2020 2020 2020 3c2f 7472 3e0a 2020 2020        </tr>.    
+00000b00: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
+00000b10: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
+00000b20: 6c65 6674 223e 3136 2e30 3420 4c54 533c  left">16.04 LTS<
+00000b30: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
+00000b40: 203c 7464 2061 6c69 676e 3d22 6c65 6674   <td align="left
+00000b50: 223e 3230 3136 2d30 342d 3231 3c2f 7464  ">2016-04-21</td
+00000b60: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
+00000b70: 6420 616c 6967 6e3d 226c 6566 7422 3e31  d align="left">1
+00000b80: 362e 3034 2e37 3c2f 7464 3e0a 2020 2020  6.04.7</td>.    
+00000b90: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
+00000ba0: 6e3d 226c 6566 7422 3e32 3032 312d 3034  n="left">2021-04
+00000bb0: 2d30 323c 2f74 643e 0a20 2020 2020 2020  -02</td>.       
+00000bc0: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
+00000bd0: 6c65 6674 223e 3230 3236 2d30 342d 3031  left">2026-04-01
+00000be0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+00000bf0: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
+00000c00: 7422 3e58 656e 6961 6c20 5865 7275 733c  t">Xenial Xerus<
+00000c10: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
+00000c20: 203c 7464 2061 6c69 676e 3d22 6c65 6674   <td align="left
+00000c30: 223e 3c2f 7464 3e0a 2020 2020 2020 2020  "></td>.        
+00000c40: 3c2f 7472 3e0a 2020 2020 2020 2020 3c74  </tr>.        <t
+00000c50: 723e 0a20 2020 2020 2020 2020 2020 203c  r>.            <
+00000c60: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
+00000c70: 3134 2e30 3420 4c54 533c 2f74 643e 0a20  14.04 LTS</td>. 
+00000c80: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
+00000c90: 6c69 676e 3d22 6c65 6674 223e 3230 3134  lign="left">2014
+00000ca0: 2d30 342d 3137 3c2f 7464 3e0a 2020 2020  -04-17</td>.    
+00000cb0: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
+00000cc0: 6e3d 226c 6566 7422 3e31 342e 3034 2e36  n="left">14.04.6
+00000cd0: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+00000ce0: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
+00000cf0: 7422 3e32 3031 392d 3034 2d30 323c 2f74  t">2019-04-02</t
+00000d00: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
+00000d10: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
+00000d20: 3230 3234 2d30 342d 3031 3c2f 7464 3e0a  2024-04-01</td>.
+00000d30: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+00000d40: 616c 6967 6e3d 226c 6566 7422 3e54 7275  align="left">Tru
+00000d50: 7374 7920 5461 6872 3c2f 7464 3e0a 2020  sty Tahr</td>.  
+00000d60: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
+00000d70: 6967 6e3d 226c 6566 7422 3e3c 2f74 643e  ign="left"></td>
+00000d80: 0a20 2020 2020 2020 203c 2f74 723e 0a20  .        </tr>. 
+00000d90: 2020 203c 2f74 626f 6479 3e0a 3c2f 7461     </tbody>.</ta
+00000da0: 626c 653e 0a22 2222 0a0a 4558 5045 4354  ble>."""..EXPECT
+00000db0: 4544 5f4d 4420 3d20 2222 220a 7c20 6379  ED_MD = """.| cy
+00000dc0: 636c 6520 2020 2020 7c20 2072 656c 6561  cle     |  relea
+00000dd0: 7365 2020 207c 206c 6174 6573 7420 207c  se   | latest  |
+00000de0: 2020 7375 7070 6f72 7420 2020 7c20 2020    support   |   
+00000df0: 2065 6f6c 2020 2020 207c 2020 2020 2063   eol     |     c
+00000e00: 6f64 656e 616d 6520 2020 207c 206c 696e  odename    | lin
+00000e10: 6b20 2020 2020 2020 2020 2020 2020 2020  k               
+00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e40: 2020 7c0a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d    |.|:----------
+00000e50: 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d  |:----------:|:-
+00000e60: 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d  -------|:-------
+00000e70: 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 2d2d  ---:|:----------
+00000e80: 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  :|:-------------
+00000e90: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
+00000ea0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000eb0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00000ec0: 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20 3232  ----------|.| 22
+00000ed0: 2e30 3420 4c54 5320 7c20 3230 3232 2d30  .04 LTS | 2022-0
+00000ee0: 342d 3231 207c 2032 322e 3034 2020 207c  4-21 | 22.04   |
+00000ef0: 2032 3032 372d 3034 2d30 3220 7c20 3230   2027-04-02 | 20
+00000f00: 3332 2d30 342d 3031 207c 204a 616d 6d79  32-04-01 | Jammy
+00000f10: 204a 656c 6c79 6669 7368 207c 2068 7474   Jellyfish | htt
+00000f20: 7073 3a2f 2f77 696b 692e 7562 756e 7475  ps://wiki.ubuntu
+00000f30: 2e63 6f6d 2f4a 616d 6d79 4a65 6c6c 7966  .com/JammyJellyf
+00000f40: 6973 682f 5265 6c65 6173 654e 6f74 6573  ish/ReleaseNotes
+00000f50: 2f20 7c0a 7c20 3231 2e31 3020 2020 2020  / |.| 21.10     
+00000f60: 7c20 3230 3231 2d31 302d 3134 207c 2032  | 2021-10-14 | 2
+00000f70: 312e 3130 2020 207c 2032 3032 322d 3037  1.10   | 2022-07
+00000f80: 2d33 3120 7c20 3230 3232 2d30 372d 3331  -31 | 2022-07-31
+00000f90: 207c 2020 2049 6d70 6973 6820 496e 6472   |   Impish Indr
+00000fa0: 6920 207c 2068 7474 7073 3a2f 2f77 696b  i  | https://wik
+00000fb0: 692e 7562 756e 7475 2e63 6f6d 2f49 6d70  i.ubuntu.com/Imp
+00000fc0: 6973 6849 6e64 7269 2f52 656c 6561 7365  ishIndri/Release
+00000fd0: 4e6f 7465 732f 2020 2020 7c0a 7c20 3231  Notes/    |.| 21
+00000fe0: 2e30 3420 2020 2020 7c20 3230 3231 2d30  .04     | 2021-0
+00000ff0: 342d 3232 207c 2032 312e 3034 2020 207c  4-22 | 21.04   |
+00001000: 2032 3032 322d 3031 2d32 3020 7c20 3230   2022-01-20 | 20
+00001010: 3232 2d30 312d 3230 207c 2020 4869 7273  22-01-20 |  Hirs
+00001020: 7574 6520 4869 7070 6f20 207c 2068 7474  ute Hippo  | htt
+00001030: 7073 3a2f 2f77 696b 692e 7562 756e 7475  ps://wiki.ubuntu
+00001040: 2e63 6f6d 2f48 6972 7375 7465 4869 7070  .com/HirsuteHipp
+00001050: 6f2f 5265 6c65 6173 654e 6f74 6573 2f20  o/ReleaseNotes/ 
+00001060: 2020 7c0a 7c20 3230 2e31 3020 2020 2020    |.| 20.10     
+00001070: 7c20 3230 3230 2d31 302d 3232 207c 2032  | 2020-10-22 | 2
+00001080: 302e 3130 2020 207c 2032 3032 312d 3037  0.10   | 2021-07
+00001090: 2d32 3220 7c20 3230 3231 2d30 372d 3232  -22 | 2021-07-22
+000010a0: 207c 2020 4772 6f6f 7679 2047 6f72 696c   |  Groovy Goril
+000010b0: 6c61 207c 2020 2020 2020 2020 2020 2020  la |            
 000010c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000010d0: 7c0a 7c20 3230 2e30 3420 4c54 5320 7c20  |.| 20.04 LTS | 
-000010e0: 2032 3032 302d 3034 2d32 3320 7c20 3230   2020-04-23 | 20
-000010f0: 2e30 342e 3420 7c20 3230 3235 2d30 342d  .04.4 | 2025-04-
-00001100: 3032 207c 2032 3033 302d 3034 2d30 3120  02 | 2030-04-01 
-00001110: 7c20 2020 466f 6361 6c20 466f 7373 6120  |   Focal Fossa 
-00001120: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
-00001130: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000010e0: 2020 2020 2020 2020 2020 7c0a 7c20 3230            |.| 20
+000010f0: 2e30 3420 4c54 5320 7c20 3230 3230 2d30  .04 LTS | 2020-0
+00001100: 342d 3233 207c 2032 302e 3034 2e34 207c  4-23 | 20.04.4 |
+00001110: 2032 3032 352d 3034 2d30 3220 7c20 3230   2025-04-02 | 20
+00001120: 3330 2d30 342d 3031 207c 2020 2046 6f63  30-04-01 |   Foc
+00001130: 616c 2046 6f73 7361 2020 207c 2020 2020  al Fossa   |    
 00001140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001150: 2020 2020 2020 2020 207c 0a7c 2031 392e           |.| 19.
-00001160: 3130 2020 2020 207c 2020 3230 3139 2d31  10     |  2019-1
-00001170: 302d 3137 207c 2031 392e 3130 2020 207c  0-17 | 19.10   |
-00001180: 2032 3032 302d 3037 2d30 3620 7c20 3230   2020-07-06 | 20
-00001190: 3230 2d30 372d 3036 207c 2020 204b 6172  20-07-06 |   Kar
-000011a0: 6d69 6320 4b6f 616c 6120 207c 2020 2020  mic Koala  |    
-000011b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001150: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001170: 2020 7c0a 7c20 3139 2e31 3020 2020 2020    |.| 19.10     
+00001180: 7c20 3230 3139 2d31 302d 3137 207c 2031  | 2019-10-17 | 1
+00001190: 392e 3130 2020 207c 2032 3032 302d 3037  9.10   | 2020-07
+000011a0: 2d30 3620 7c20 3230 3230 2d30 372d 3036  -06 | 2020-07-06
+000011b0: 207c 2020 204b 6172 6d69 6320 4b6f 616c   |   Karmic Koal
+000011c0: 6120 207c 2020 2020 2020 2020 2020 2020  a  |            
 000011d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011e0: 2020 7c0a 7c20 3138 2e30 3420 4c54 5320    |.| 18.04 LTS 
-000011f0: 7c20 2032 3031 382d 3034 2d32 3620 7c20  |  2018-04-26 | 
-00001200: 3138 2e30 342e 3620 7c20 3230 3233 2d30  18.04.6 | 2023-0
-00001210: 342d 3032 207c 2032 3032 382d 3034 2d30  4-02 | 2028-04-0
-00001220: 3120 7c20 2042 696f 6e69 6320 4265 6176  1 |  Bionic Beav
-00001230: 6572 2020 7c20 6874 7470 733a 2f2f 7769  er  | https://wi
-00001240: 6b69 2e75 6275 6e74 752e 636f 6d2f 4269  ki.ubuntu.com/Bi
-00001250: 6f6e 6963 4265 6176 6572 2f52 656c 6561  onicBeaver/Relea
-00001260: 7365 4e6f 7465 7320 2020 207c 0a7c 2031  seNotes    |.| 1
-00001270: 362e 3034 204c 5453 207c 2020 3230 3136  6.04 LTS |  2016
-00001280: 2d30 342d 3231 207c 2031 362e 3034 2e37  -04-21 | 16.04.7
-00001290: 207c 2032 3032 312d 3034 2d30 3220 7c20   | 2021-04-02 | 
-000012a0: 3230 3236 2d30 342d 3031 207c 2020 2058  2026-04-01 |   X
-000012b0: 656e 6961 6c20 5865 7275 7320 207c 2020  enial Xerus  |  
-000012c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000011f0: 2020 2020 2020 2020 2020 7c0a 7c20 3138            |.| 18
+00001200: 2e30 3420 4c54 5320 7c20 3230 3138 2d30  .04 LTS | 2018-0
+00001210: 342d 3236 207c 2031 382e 3034 2e36 207c  4-26 | 18.04.6 |
+00001220: 2032 3032 332d 3034 2d30 3220 7c20 3230   2023-04-02 | 20
+00001230: 3238 2d30 342d 3031 207c 2020 4269 6f6e  28-04-01 |  Bion
+00001240: 6963 2042 6561 7665 7220 207c 2068 7474  ic Beaver  | htt
+00001250: 7073 3a2f 2f77 696b 692e 7562 756e 7475  ps://wiki.ubuntu
+00001260: 2e63 6f6d 2f42 696f 6e69 6342 6561 7665  .com/BionicBeave
+00001270: 722f 5265 6c65 6173 654e 6f74 6573 2020  r/ReleaseNotes  
+00001280: 2020 7c0a 7c20 3136 2e30 3420 4c54 5320    |.| 16.04 LTS 
+00001290: 7c20 3230 3136 2d30 342d 3231 207c 2031  | 2016-04-21 | 1
+000012a0: 362e 3034 2e37 207c 2032 3032 312d 3034  6.04.7 | 2021-04
+000012b0: 2d30 3220 7c20 3230 3236 2d30 342d 3031  -02 | 2026-04-01
+000012c0: 207c 2020 2058 656e 6961 6c20 5865 7275   |   Xenial Xeru
+000012d0: 7320 207c 2020 2020 2020 2020 2020 2020  s  |            
 000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 2020 2020 7c0a 7c20 3134 2e30 3420 4c54      |.| 14.04 LT
-00001300: 5320 7c20 2032 3031 342d 3034 2d31 3720  S |  2014-04-17 
-00001310: 7c20 3134 2e30 342e 3620 7c20 3230 3139  | 14.04.6 | 2019
-00001320: 2d30 342d 3032 207c 2032 3032 342d 3034  -04-02 | 2024-04
-00001330: 2d30 3120 7c20 2020 5472 7573 7479 2054  -01 |   Trusty T
-00001340: 6168 7220 2020 7c20 2020 2020 2020 2020  ahr   |         
-00001350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000012f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001300: 2020 2020 2020 2020 2020 7c0a 7c20 3134            |.| 14
+00001310: 2e30 3420 4c54 5320 7c20 3230 3134 2d30  .04 LTS | 2014-0
+00001320: 342d 3137 207c 2031 342e 3034 2e36 207c  4-17 | 14.04.6 |
+00001330: 2032 3031 392d 3034 2d30 3220 7c20 3230   2019-04-02 | 20
+00001340: 3234 2d30 342d 3031 207c 2020 2054 7275  24-04-01 |   Tru
+00001350: 7374 7920 5461 6872 2020 207c 2020 2020  sty Tahr   |    
 00001360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001370: 2020 2020 2020 2020 2020 2020 207c 0a22               |."
-00001380: 2222 2020 2320 6e6f 7161 3a20 4535 3031  ""  # noqa: E501
-00001390: 0a0a 0a45 5850 4543 5445 445f 4d44 5f43  ...EXPECTED_MD_C
-000013a0: 4f4c 4f55 5220 3d20 2222 220a 7c20 6379  OLOUR = """.| cy
-000013b0: 636c 6520 2020 2020 7c20 7265 6c65 6173  cle     | releas
-000013c0: 6544 6174 6520 7c20 6c61 7465 7374 2020  eDate | latest  
-000013d0: 7c20 2073 7570 706f 7274 2020 207c 2020  |  support   |  
-000013e0: 2020 656f 6c20 2020 2020 7c20 2020 2020    eol     |     
-000013f0: 636f 6465 6e61 6d65 2020 2020 7c20 6c69  codename    | li
-00001400: 6e6b 2020 2020 2020 2020 2020 2020 2020  nk              
-00001410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001370: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001380: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001390: 2020 7c0a 2222 2220 2023 206e 6f71 613a    |."""  # noqa:
+000013a0: 2045 3530 310a 0a0a 4558 5045 4354 4544   E501...EXPECTED
+000013b0: 5f4d 445f 434f 4c4f 5552 203d 2022 2222  _MD_COLOUR = """
+000013c0: 0a7c 2063 7963 6c65 2020 2020 207c 2020  .| cycle     |  
+000013d0: 7265 6c65 6173 6520 2020 7c20 6c61 7465  release   | late
+000013e0: 7374 2020 7c20 2073 7570 706f 7274 2020  st  |  support  
+000013f0: 207c 2020 2020 656f 6c20 2020 2020 7c20   |    eol     | 
+00001400: 2020 2020 636f 6465 6e61 6d65 2020 2020      codename    
+00001410: 7c20 6c69 6e6b 2020 2020 2020 2020 2020  | link          
 00001420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001430: 2020 207c 0a7c 3a2d 2d2d 2d2d 2d2d 2d2d     |.|:---------
-00001440: 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  -|:-----------:|
-00001450: 3a2d 2d2d 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d  :--------|:-----
-00001460: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
-00001470: 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d2d  --:|:-----------
-00001480: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 2d2d  ----:|:---------
-00001490: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001440: 2020 2020 2020 207c 0a7c 3a2d 2d2d 2d2d         |.|:-----
+00001450: 2d2d 2d2d 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d  -----|:---------
+00001460: 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d  -:|:--------|:--
+00001470: 2d2d 2d2d 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d  --------:|:-----
+00001480: 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d 2d2d  -----:|:--------
+00001490: 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d  -------:|:------
 000014a0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
-000014b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 7c0a 7c20  ------------|.| 
-000014c0: 3232 2e30 3420 4c54 5320 7c20 2032 3032  22.04 LTS |  202
-000014d0: 322d 3034 2d32 3120 7c20 3232 2e30 3420  2-04-21 | 22.04 
-000014e0: 2020 7c20 1b5b 3332 6d32 3032 372d 3034    | .[32m2027-04
-000014f0: 2d30 321b 5b30 6d20 7c20 1b5b 3332 6d32  -02.[0m | .[32m2
-00001500: 3033 322d 3034 2d30 311b 5b30 6d20 7c20  032-04-01.[0m | 
-00001510: 4a61 6d6d 7920 4a65 6c6c 7966 6973 6820  Jammy Jellyfish 
-00001520: 7c20 6874 7470 733a 2f2f 7769 6b69 2e75  | https://wiki.u
-00001530: 6275 6e74 752e 636f 6d2f 4a61 6d6d 794a  buntu.com/JammyJ
-00001540: 656c 6c79 6669 7368 2f52 656c 6561 7365  ellyfish/Release
-00001550: 4e6f 7465 732f 207c 0a7c 2032 312e 3130  Notes/ |.| 21.10
-00001560: 2020 2020 207c 2020 3230 3231 2d31 302d       |  2021-10-
-00001570: 3134 207c 2032 312e 3130 2020 207c 201b  14 | 21.10   | .
-00001580: 5b33 326d 3230 3232 2d30 372d 3331 1b5b  [32m2022-07-31.[
-00001590: 306d 207c 201b 5b33 326d 3230 3232 2d30  0m | .[32m2022-0
-000015a0: 372d 3331 1b5b 306d 207c 2020 2049 6d70  7-31.[0m |   Imp
-000015b0: 6973 6820 496e 6472 6920 207c 2068 7474  ish Indri  | htt
-000015c0: 7073 3a2f 2f77 696b 692e 7562 756e 7475  ps://wiki.ubuntu
-000015d0: 2e63 6f6d 2f49 6d70 6973 6849 6e64 7269  .com/ImpishIndri
-000015e0: 2f52 656c 6561 7365 4e6f 7465 732f 2020  /ReleaseNotes/  
-000015f0: 2020 7c0a 7c20 3231 2e30 3420 2020 2020    |.| 21.04     
-00001600: 7c20 2032 3032 312d 3034 2d32 3220 7c20  |  2021-04-22 | 
-00001610: 3231 2e30 3420 2020 7c20 1b5b 3333 6d32  21.04   | .[33m2
-00001620: 3032 322d 3031 2d32 301b 5b30 6d20 7c20  022-01-20.[0m | 
-00001630: 1b5b 3333 6d32 3032 322d 3031 2d32 301b  .[33m2022-01-20.
-00001640: 5b30 6d20 7c20 2048 6972 7375 7465 2048  [0m |  Hirsute H
-00001650: 6970 706f 2020 7c20 6874 7470 733a 2f2f  ippo  | https://
-00001660: 7769 6b69 2e75 6275 6e74 752e 636f 6d2f  wiki.ubuntu.com/
-00001670: 4869 7273 7574 6548 6970 706f 2f52 656c  HirsuteHippo/Rel
-00001680: 6561 7365 4e6f 7465 732f 2020 207c 0a7c  easeNotes/   |.|
-00001690: 2032 302e 3130 2020 2020 207c 2020 3230   20.10     |  20
-000016a0: 3230 2d31 302d 3232 207c 2032 302e 3130  20-10-22 | 20.10
-000016b0: 2020 207c 201b 5b33 316d 3230 3231 2d30     | .[31m2021-0
-000016c0: 372d 3232 1b5b 306d 207c 201b 5b33 316d  7-22.[0m | .[31m
-000016d0: 3230 3231 2d30 372d 3232 1b5b 306d 207c  2021-07-22.[0m |
-000016e0: 2020 4772 6f6f 7679 2047 6f72 696c 6c61    Groovy Gorilla
-000016f0: 207c 2020 2020 2020 2020 2020 2020 2020   |              
-00001700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000014b0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000014c0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d7c  ---------------|
+000014d0: 0a7c 2032 322e 3034 204c 5453 207c 2032  .| 22.04 LTS | 2
+000014e0: 3032 322d 3034 2d32 3120 7c20 3232 2e30  022-04-21 | 22.0
+000014f0: 3420 2020 7c20 1b5b 3332 6d32 3032 372d  4   | .[32m2027-
+00001500: 3034 2d30 321b 5b30 6d20 7c20 1b5b 3332  04-02.[0m | .[32
+00001510: 6d32 3033 322d 3034 2d30 311b 5b30 6d20  m2032-04-01.[0m 
+00001520: 7c20 4a61 6d6d 7920 4a65 6c6c 7966 6973  | Jammy Jellyfis
+00001530: 6820 7c20 6874 7470 733a 2f2f 7769 6b69  h | https://wiki
+00001540: 2e75 6275 6e74 752e 636f 6d2f 4a61 6d6d  .ubuntu.com/Jamm
+00001550: 794a 656c 6c79 6669 7368 2f52 656c 6561  yJellyfish/Relea
+00001560: 7365 4e6f 7465 732f 207c 0a7c 2032 312e  seNotes/ |.| 21.
+00001570: 3130 2020 2020 207c 2032 3032 312d 3130  10     | 2021-10
+00001580: 2d31 3420 7c20 3231 2e31 3020 2020 7c20  -14 | 21.10   | 
+00001590: 1b5b 3332 6d32 3032 322d 3037 2d33 311b  .[32m2022-07-31.
+000015a0: 5b30 6d20 7c20 1b5b 3332 6d32 3032 322d  [0m | .[32m2022-
+000015b0: 3037 2d33 311b 5b30 6d20 7c20 2020 496d  07-31.[0m |   Im
+000015c0: 7069 7368 2049 6e64 7269 2020 7c20 6874  pish Indri  | ht
+000015d0: 7470 733a 2f2f 7769 6b69 2e75 6275 6e74  tps://wiki.ubunt
+000015e0: 752e 636f 6d2f 496d 7069 7368 496e 6472  u.com/ImpishIndr
+000015f0: 692f 5265 6c65 6173 654e 6f74 6573 2f20  i/ReleaseNotes/ 
+00001600: 2020 207c 0a7c 2032 312e 3034 2020 2020     |.| 21.04    
+00001610: 207c 2032 3032 312d 3034 2d32 3220 7c20   | 2021-04-22 | 
+00001620: 3231 2e30 3420 2020 7c20 1b5b 3333 6d32  21.04   | .[33m2
+00001630: 3032 322d 3031 2d32 301b 5b30 6d20 7c20  022-01-20.[0m | 
+00001640: 1b5b 3333 6d32 3032 322d 3031 2d32 301b  .[33m2022-01-20.
+00001650: 5b30 6d20 7c20 2048 6972 7375 7465 2048  [0m |  Hirsute H
+00001660: 6970 706f 2020 7c20 6874 7470 733a 2f2f  ippo  | https://
+00001670: 7769 6b69 2e75 6275 6e74 752e 636f 6d2f  wiki.ubuntu.com/
+00001680: 4869 7273 7574 6548 6970 706f 2f52 656c  HirsuteHippo/Rel
+00001690: 6561 7365 4e6f 7465 732f 2020 207c 0a7c  easeNotes/   |.|
+000016a0: 2032 302e 3130 2020 2020 207c 2032 3032   20.10     | 202
+000016b0: 302d 3130 2d32 3220 7c20 3230 2e31 3020  0-10-22 | 20.10 
+000016c0: 2020 7c20 1b5b 3331 6d32 3032 312d 3037    | .[31m2021-07
+000016d0: 2d32 321b 5b30 6d20 7c20 1b5b 3331 6d32  -22.[0m | .[31m2
+000016e0: 3032 312d 3037 2d32 321b 5b30 6d20 7c20  021-07-22.[0m | 
+000016f0: 2047 726f 6f76 7920 476f 7269 6c6c 6120   Groovy Gorilla 
+00001700: 7c20 2020 2020 2020 2020 2020 2020 2020  |               
 00001710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001720: 2020 2020 2020 2020 7c0a 7c20 3230 2e30          |.| 20.0
-00001730: 3420 4c54 5320 7c20 2032 3032 302d 3034  4 LTS |  2020-04
-00001740: 2d32 3320 7c20 3230 2e30 342e 3420 7c20  -23 | 20.04.4 | 
-00001750: 1b5b 3332 6d32 3032 352d 3034 2d30 321b  .[32m2025-04-02.
-00001760: 5b30 6d20 7c20 1b5b 3332 6d32 3033 302d  [0m | .[32m2030-
-00001770: 3034 2d30 311b 5b30 6d20 7c20 2020 466f  04-01.[0m |   Fo
-00001780: 6361 6c20 466f 7373 6120 2020 7c20 2020  cal Fossa   |   
-00001790: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001730: 2020 2020 2020 207c 0a7c 2032 302e 3034         |.| 20.04
+00001740: 204c 5453 207c 2032 3032 302d 3034 2d32   LTS | 2020-04-2
+00001750: 3320 7c20 3230 2e30 342e 3420 7c20 1b5b  3 | 20.04.4 | .[
+00001760: 3332 6d32 3032 352d 3034 2d30 321b 5b30  32m2025-04-02.[0
+00001770: 6d20 7c20 1b5b 3332 6d32 3033 302d 3034  m | .[32m2030-04
+00001780: 2d30 311b 5b30 6d20 7c20 2020 466f 6361  -01.[0m |   Foca
+00001790: 6c20 466f 7373 6120 2020 7c20 2020 2020  l Fossa   |     
 000017a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000017b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000017c0: 2020 207c 0a7c 2031 392e 3130 2020 2020     |.| 19.10    
-000017d0: 207c 2020 3230 3139 2d31 302d 3137 207c   |  2019-10-17 |
-000017e0: 2031 392e 3130 2020 207c 201b 5b33 316d   19.10   | .[31m
-000017f0: 3230 3230 2d30 372d 3036 1b5b 306d 207c  2020-07-06.[0m |
-00001800: 201b 5b33 316d 3230 3230 2d30 372d 3036   .[31m2020-07-06
-00001810: 1b5b 306d 207c 2020 204b 6172 6d69 6320  .[0m |   Karmic 
-00001820: 4b6f 616c 6120 207c 2020 2020 2020 2020  Koala  |        
-00001830: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000017d0: 207c 0a7c 2031 392e 3130 2020 2020 207c   |.| 19.10     |
+000017e0: 2032 3031 392d 3130 2d31 3720 7c20 3139   2019-10-17 | 19
+000017f0: 2e31 3020 2020 7c20 1b5b 3331 6d32 3032  .10   | .[31m202
+00001800: 302d 3037 2d30 361b 5b30 6d20 7c20 1b5b  0-07-06.[0m | .[
+00001810: 3331 6d32 3032 302d 3037 2d30 361b 5b30  31m2020-07-06.[0
+00001820: 6d20 7c20 2020 4b61 726d 6963 204b 6f61  m |   Karmic Koa
+00001830: 6c61 2020 7c20 2020 2020 2020 2020 2020  la  |           
 00001840: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001850: 2020 2020 2020 2020 2020 2020 2020 7c0a                |.
-00001860: 7c20 3138 2e30 3420 4c54 5320 7c20 2032  | 18.04 LTS |  2
-00001870: 3031 382d 3034 2d32 3620 7c20 3138 2e30  018-04-26 | 18.0
-00001880: 342e 3620 7c20 1b5b 3332 6d32 3032 332d  4.6 | .[32m2023-
-00001890: 3034 2d30 321b 5b30 6d20 7c20 1b5b 3332  04-02.[0m | .[32
-000018a0: 6d32 3032 382d 3034 2d30 311b 5b30 6d20  m2028-04-01.[0m 
-000018b0: 7c20 2042 696f 6e69 6320 4265 6176 6572  |  Bionic Beaver
-000018c0: 2020 7c20 6874 7470 733a 2f2f 7769 6b69    | https://wiki
-000018d0: 2e75 6275 6e74 752e 636f 6d2f 4269 6f6e  .ubuntu.com/Bion
-000018e0: 6963 4265 6176 6572 2f52 656c 6561 7365  icBeaver/Release
-000018f0: 4e6f 7465 7320 2020 207c 0a7c 2031 362e  Notes    |.| 16.
-00001900: 3034 204c 5453 207c 2020 3230 3136 2d30  04 LTS |  2016-0
-00001910: 342d 3231 207c 2031 362e 3034 2e37 207c  4-21 | 16.04.7 |
-00001920: 201b 5b33 316d 3230 3231 2d30 342d 3032   .[31m2021-04-02
-00001930: 1b5b 306d 207c 201b 5b33 326d 3230 3236  .[0m | .[32m2026
-00001940: 2d30 342d 3031 1b5b 306d 207c 2020 2058  -04-01.[0m |   X
-00001950: 656e 6961 6c20 5865 7275 7320 207c 2020  enial Xerus  |  
-00001960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001860: 2020 2020 2020 2020 2020 207c 0a7c 2031             |.| 1
+00001870: 382e 3034 204c 5453 207c 2032 3031 382d  8.04 LTS | 2018-
+00001880: 3034 2d32 3620 7c20 3138 2e30 342e 3620  04-26 | 18.04.6 
+00001890: 7c20 1b5b 3332 6d32 3032 332d 3034 2d30  | .[32m2023-04-0
+000018a0: 321b 5b30 6d20 7c20 1b5b 3332 6d32 3032  2.[0m | .[32m202
+000018b0: 382d 3034 2d30 311b 5b30 6d20 7c20 2042  8-04-01.[0m |  B
+000018c0: 696f 6e69 6320 4265 6176 6572 2020 7c20  ionic Beaver  | 
+000018d0: 6874 7470 733a 2f2f 7769 6b69 2e75 6275  https://wiki.ubu
+000018e0: 6e74 752e 636f 6d2f 4269 6f6e 6963 4265  ntu.com/BionicBe
+000018f0: 6176 6572 2f52 656c 6561 7365 4e6f 7465  aver/ReleaseNote
+00001900: 7320 2020 207c 0a7c 2031 362e 3034 204c  s    |.| 16.04 L
+00001910: 5453 207c 2032 3031 362d 3034 2d32 3120  TS | 2016-04-21 
+00001920: 7c20 3136 2e30 342e 3720 7c20 1b5b 3331  | 16.04.7 | .[31
+00001930: 6d32 3032 312d 3034 2d30 321b 5b30 6d20  m2021-04-02.[0m 
+00001940: 7c20 1b5b 3332 6d32 3032 362d 3034 2d30  | .[32m2026-04-0
+00001950: 311b 5b30 6d20 7c20 2020 5865 6e69 616c  1.[0m |   Xenial
+00001960: 2058 6572 7573 2020 7c20 2020 2020 2020   Xerus  |       
 00001970: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001990: 2020 2020 7c0a 7c20 3134 2e30 3420 4c54      |.| 14.04 LT
-000019a0: 5320 7c20 2032 3031 342d 3034 2d31 3720  S |  2014-04-17 
-000019b0: 7c20 3134 2e30 342e 3620 7c20 1b5b 3331  | 14.04.6 | .[31
-000019c0: 6d32 3031 392d 3034 2d30 321b 5b30 6d20  m2019-04-02.[0m 
-000019d0: 7c20 1b5b 3332 6d32 3032 342d 3034 2d30  | .[32m2024-04-0
-000019e0: 311b 5b30 6d20 7c20 2020 5472 7573 7479  1.[0m |   Trusty
-000019f0: 2054 6168 7220 2020 7c20 2020 2020 2020   Tahr   |       
-00001a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001990: 2020 2020 2020 2020 2020 2020 2020 207c                 |
+000019a0: 0a7c 2031 342e 3034 204c 5453 207c 2032  .| 14.04 LTS | 2
+000019b0: 3031 342d 3034 2d31 3720 7c20 3134 2e30  014-04-17 | 14.0
+000019c0: 342e 3620 7c20 1b5b 3331 6d32 3031 392d  4.6 | .[31m2019-
+000019d0: 3034 2d30 321b 5b30 6d20 7c20 1b5b 3332  04-02.[0m | .[32
+000019e0: 6d32 3032 342d 3034 2d30 311b 5b30 6d20  m2024-04-01.[0m 
+000019f0: 7c20 2020 5472 7573 7479 2054 6168 7220  |   Trusty Tahr 
+00001a00: 2020 7c20 2020 2020 2020 2020 2020 2020    |             
 00001a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001a20: 2020 2020 2020 2020 2020 2020 2020 207c                 |
-00001a30: 0a0a 2222 2220 2023 206e 6f71 613a 2045  .."""  # noqa: E
-00001a40: 3530 310a 0a0a 4558 5045 4354 4544 5f52  501...EXPECTED_R
-00001a50: 5354 203d 2022 2222 0a2e 2e20 7461 626c  ST = """... tabl
-00001a60: 653a 3a0a 0a20 2020 203d 3d3d 3d3d 3d3d  e::..    =======
-00001a70: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
-00001a80: 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d 2020  ===  =========  
-00001a90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d  ============  ==
-00001aa0: 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d  ==========  ====
-00001ab0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 203d  =============  =
-00001ac0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00001a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001a30: 2020 2020 2020 2020 207c 0a22 2222 2020           |."""  
+00001a40: 2320 6e6f 7161 3a20 4535 3031 0a0a 0a45  # noqa: E501...E
+00001a50: 5850 4543 5445 445f 5253 5420 3d20 2222  XPECTED_RST = ""
+00001a60: 220a 2e2e 2074 6162 6c65 3a3a 0a0a 2020  "... table::..  
+00001a70: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 203d    ===========  =
+00001a80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 203d 3d3d  ===========  ===
+00001a90: 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d  ======  ========
+00001aa0: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
+00001ab0: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
+00001ac0: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
 00001ad0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00001ae0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001af0: 3d3d 3d3d 3d0a 2020 2020 2020 2063 7963  =====.       cyc
-00001b00: 6c65 2020 2020 2020 7265 6c65 6173 6544  le      releaseD
-00001b10: 6174 6520 2020 206c 6174 6573 7420 2020  ate    latest   
-00001b20: 2020 2073 7570 706f 7274 2020 2020 2020     support      
-00001b30: 2020 2065 6f6c 2020 2020 2020 2020 2020     eol          
-00001b40: 2063 6f64 656e 616d 6520 2020 2020 2020   codename       
+00001af0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
+00001b00: 2020 2020 2063 7963 6c65 2020 2020 2020       cycle      
+00001b10: 2072 656c 6561 7365 2020 2020 2020 6c61   release      la
+00001b20: 7465 7374 2020 2020 2020 7375 7070 6f72  test      suppor
+00001b30: 7420 2020 2020 2020 2020 656f 6c20 2020  t         eol   
+00001b40: 2020 2020 2020 2020 636f 6465 6e61 6d65          codename
 00001b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b60: 2020 2020 2020 2020 206c 696e 6b20 2020           link   
-00001b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001b80: 2020 2020 2020 0a20 2020 203d 3d3d 3d3d        .    =====
-00001b90: 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d  ======  ========
-00001ba0: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
-00001bb0: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020    ============  
-00001bc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d  ============  ==
-00001bd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d20  =============== 
-00001be0: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+00001b60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00001b70: 6c69 6e6b 2020 2020 2020 2020 2020 2020  link            
+00001b80: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00001b90: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 203d    ===========  =
+00001ba0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 203d 3d3d  ===========  ===
+00001bb0: 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d  ======  ========
+00001bc0: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
+00001bd0: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
+00001be0: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
 00001bf0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00001c00: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00001c10: 3d3d 3d3d 3d3d 3d0a 2020 2020 2032 322e  =======.     22.
-00001c20: 3034 204c 5453 2020 2020 3230 3232 2d30  04 LTS    2022-0
-00001c30: 342d 3231 2020 2020 2032 322e 3034 2020  4-21     22.04  
-00001c40: 2020 2020 3230 3237 2d30 342d 3032 2020      2027-04-02  
-00001c50: 2020 3230 3332 2d30 342d 3031 2020 2020    2032-04-01    
-00001c60: 4a61 6d6d 7920 4a65 6c6c 7966 6973 6820  Jammy Jellyfish 
-00001c70: 2020 2068 7474 7073 3a2f 2f77 696b 692e     https://wiki.
-00001c80: 7562 756e 7475 2e63 6f6d 2f4a 616d 6d79  ubuntu.com/Jammy
-00001c90: 4a65 6c6c 7966 6973 682f 5265 6c65 6173  Jellyfish/Releas
-00001ca0: 654e 6f74 6573 2f20 0a20 2020 2020 3231  eNotes/ .     21
-00001cb0: 2e31 3020 2020 2020 2020 2032 3032 312d  .10        2021-
-00001cc0: 3130 2d31 3420 2020 2020 3231 2e31 3020  10-14     21.10 
-00001cd0: 2020 2020 2032 3032 322d 3037 2d33 3120       2022-07-31 
-00001ce0: 2020 2032 3032 322d 3037 2d33 3120 2020     2022-07-31   
-00001cf0: 2049 6d70 6973 6820 496e 6472 6920 2020   Impish Indri   
-00001d00: 2020 2020 6874 7470 733a 2f2f 7769 6b69      https://wiki
-00001d10: 2e75 6275 6e74 752e 636f 6d2f 496d 7069  .ubuntu.com/Impi
-00001d20: 7368 496e 6472 692f 5265 6c65 6173 654e  shIndri/ReleaseN
-00001d30: 6f74 6573 2f20 2020 200a 2020 2020 2032  otes/    .     2
-00001d40: 312e 3034 2020 2020 2020 2020 3230 3231  1.04        2021
-00001d50: 2d30 342d 3232 2020 2020 2032 312e 3034  -04-22     21.04
-00001d60: 2020 2020 2020 3230 3232 2d30 312d 3230        2022-01-20
-00001d70: 2020 2020 3230 3232 2d30 312d 3230 2020      2022-01-20  
-00001d80: 2020 4869 7273 7574 6520 4869 7070 6f20    Hirsute Hippo 
-00001d90: 2020 2020 2068 7474 7073 3a2f 2f77 696b       https://wik
-00001da0: 692e 7562 756e 7475 2e63 6f6d 2f48 6972  i.ubuntu.com/Hir
-00001db0: 7375 7465 4869 7070 6f2f 5265 6c65 6173  suteHippo/Releas
-00001dc0: 654e 6f74 6573 2f20 2020 0a20 2020 2020  eNotes/   .     
-00001dd0: 3230 2e31 3020 2020 2020 2020 2032 3032  20.10        202
-00001de0: 302d 3130 2d32 3220 2020 2020 3230 2e31  0-10-22     20.1
-00001df0: 3020 2020 2020 2032 3032 312d 3037 2d32  0      2021-07-2
-00001e00: 3220 2020 2032 3032 312d 3037 2d32 3220  2    2021-07-22 
-00001e10: 2020 2047 726f 6f76 7920 476f 7269 6c6c     Groovy Gorill
-00001e20: 6120 2020 2020 2020 2020 2020 2020 2020  a               
+00001c10: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020  =============.  
+00001c20: 2020 2032 322e 3034 204c 5453 2020 2020     22.04 LTS    
+00001c30: 3230 3232 2d30 342d 3231 2020 2020 3232  2022-04-21    22
+00001c40: 2e30 3420 2020 2020 2032 3032 372d 3034  .04      2027-04
+00001c50: 2d30 3220 2020 2032 3033 322d 3034 2d30  -02    2032-04-0
+00001c60: 3120 2020 204a 616d 6d79 204a 656c 6c79  1    Jammy Jelly
+00001c70: 6669 7368 2020 2020 6874 7470 733a 2f2f  fish    https://
+00001c80: 7769 6b69 2e75 6275 6e74 752e 636f 6d2f  wiki.ubuntu.com/
+00001c90: 4a61 6d6d 794a 656c 6c79 6669 7368 2f52  JammyJellyfish/R
+00001ca0: 656c 6561 7365 4e6f 7465 732f 200a 2020  eleaseNotes/ .  
+00001cb0: 2020 2032 312e 3130 2020 2020 2020 2020     21.10        
+00001cc0: 3230 3231 2d31 302d 3134 2020 2020 3231  2021-10-14    21
+00001cd0: 2e31 3020 2020 2020 2032 3032 322d 3037  .10      2022-07
+00001ce0: 2d33 3120 2020 2032 3032 322d 3037 2d33  -31    2022-07-3
+00001cf0: 3120 2020 2049 6d70 6973 6820 496e 6472  1    Impish Indr
+00001d00: 6920 2020 2020 2020 6874 7470 733a 2f2f  i       https://
+00001d10: 7769 6b69 2e75 6275 6e74 752e 636f 6d2f  wiki.ubuntu.com/
+00001d20: 496d 7069 7368 496e 6472 692f 5265 6c65  ImpishIndri/Rele
+00001d30: 6173 654e 6f74 6573 2f20 2020 200a 2020  aseNotes/    .  
+00001d40: 2020 2032 312e 3034 2020 2020 2020 2020     21.04        
+00001d50: 3230 3231 2d30 342d 3232 2020 2020 3231  2021-04-22    21
+00001d60: 2e30 3420 2020 2020 2032 3032 322d 3031  .04      2022-01
+00001d70: 2d32 3020 2020 2032 3032 322d 3031 2d32  -20    2022-01-2
+00001d80: 3020 2020 2048 6972 7375 7465 2048 6970  0    Hirsute Hip
+00001d90: 706f 2020 2020 2020 6874 7470 733a 2f2f  po      https://
+00001da0: 7769 6b69 2e75 6275 6e74 752e 636f 6d2f  wiki.ubuntu.com/
+00001db0: 4869 7273 7574 6548 6970 706f 2f52 656c  HirsuteHippo/Rel
+00001dc0: 6561 7365 4e6f 7465 732f 2020 200a 2020  easeNotes/   .  
+00001dd0: 2020 2032 302e 3130 2020 2020 2020 2020     20.10        
+00001de0: 3230 3230 2d31 302d 3232 2020 2020 3230  2020-10-22    20
+00001df0: 2e31 3020 2020 2020 2032 3032 312d 3037  .10      2021-07
+00001e00: 2d32 3220 2020 2032 3032 312d 3037 2d32  -22    2021-07-2
+00001e10: 3220 2020 2047 726f 6f76 7920 476f 7269  2    Groovy Gori
+00001e20: 6c6c 6120 2020 2020 2020 2020 2020 2020  lla             
 00001e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001e50: 2020 2020 2020 2020 2020 200a 2020 2020             .    
-00001e60: 2032 302e 3034 204c 5453 2020 2020 3230   20.04 LTS    20
-00001e70: 3230 2d30 342d 3233 2020 2020 2032 302e  20-04-23     20.
-00001e80: 3034 2e34 2020 2020 3230 3235 2d30 342d  04.4    2025-04-
-00001e90: 3032 2020 2020 3230 3330 2d30 342d 3031  02    2030-04-01
-00001ea0: 2020 2020 466f 6361 6c20 466f 7373 6120      Focal Fossa 
+00001e50: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00001e60: 2020 2032 302e 3034 204c 5453 2020 2020     20.04 LTS    
+00001e70: 3230 3230 2d30 342d 3233 2020 2020 3230  2020-04-23    20
+00001e80: 2e30 342e 3420 2020 2032 3032 352d 3034  .04.4    2025-04
+00001e90: 2d30 3220 2020 2032 3033 302d 3034 2d30  -02    2030-04-0
+00001ea0: 3120 2020 2046 6f63 616c 2046 6f73 7361  1    Focal Fossa
 00001eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001ee0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-00001ef0: 2020 3139 2e31 3020 2020 2020 2020 2032    19.10        2
-00001f00: 3031 392d 3130 2d31 3720 2020 2020 3139  019-10-17     19
+00001ee0: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00001ef0: 2020 2031 392e 3130 2020 2020 2020 2020     19.10        
+00001f00: 3230 3139 2d31 302d 3137 2020 2020 3139  2019-10-17    19
 00001f10: 2e31 3020 2020 2020 2032 3032 302d 3037  .10      2020-07
 00001f20: 2d30 3620 2020 2032 3032 302d 3037 2d30  -06    2020-07-0
 00001f30: 3620 2020 204b 6172 6d69 6320 4b6f 616c  6    Karmic Koal
 00001f40: 6120 2020 2020 2020 2020 2020 2020 2020  a               
 00001f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00001f70: 2020 2020 2020 2020 2020 2020 200a 2020               .  
 00001f80: 2020 2031 382e 3034 204c 5453 2020 2020     18.04 LTS    
-00001f90: 3230 3138 2d30 342d 3236 2020 2020 2031  2018-04-26     1
-00001fa0: 382e 3034 2e36 2020 2020 3230 3233 2d30  8.04.6    2023-0
-00001fb0: 342d 3032 2020 2020 3230 3238 2d30 342d  4-02    2028-04-
-00001fc0: 3031 2020 2020 4269 6f6e 6963 2042 6561  01    Bionic Bea
-00001fd0: 7665 7220 2020 2020 2068 7474 7073 3a2f  ver      https:/
-00001fe0: 2f77 696b 692e 7562 756e 7475 2e63 6f6d  /wiki.ubuntu.com
-00001ff0: 2f42 696f 6e69 6342 6561 7665 722f 5265  /BionicBeaver/Re
-00002000: 6c65 6173 654e 6f74 6573 2020 2020 0a20  leaseNotes    . 
-00002010: 2020 2020 3136 2e30 3420 4c54 5320 2020      16.04 LTS   
-00002020: 2032 3031 362d 3034 2d32 3120 2020 2020   2016-04-21     
-00002030: 3136 2e30 342e 3720 2020 2032 3032 312d  16.04.7    2021-
-00002040: 3034 2d30 3220 2020 2032 3032 362d 3034  04-02    2026-04
-00002050: 2d30 3120 2020 2058 656e 6961 6c20 5865  -01    Xenial Xe
-00002060: 7275 7320 2020 2020 2020 2020 2020 2020  rus             
+00001f90: 3230 3138 2d30 342d 3236 2020 2020 3138  2018-04-26    18
+00001fa0: 2e30 342e 3620 2020 2032 3032 332d 3034  .04.6    2023-04
+00001fb0: 2d30 3220 2020 2032 3032 382d 3034 2d30  -02    2028-04-0
+00001fc0: 3120 2020 2042 696f 6e69 6320 4265 6176  1    Bionic Beav
+00001fd0: 6572 2020 2020 2020 6874 7470 733a 2f2f  er      https://
+00001fe0: 7769 6b69 2e75 6275 6e74 752e 636f 6d2f  wiki.ubuntu.com/
+00001ff0: 4269 6f6e 6963 4265 6176 6572 2f52 656c  BionicBeaver/Rel
+00002000: 6561 7365 4e6f 7465 7320 2020 200a 2020  easeNotes    .  
+00002010: 2020 2031 362e 3034 204c 5453 2020 2020     16.04 LTS    
+00002020: 3230 3136 2d30 342d 3231 2020 2020 3136  2016-04-21    16
+00002030: 2e30 342e 3720 2020 2032 3032 312d 3034  .04.7    2021-04
+00002040: 2d30 3220 2020 2032 3032 362d 3034 2d30  -02    2026-04-0
+00002050: 3120 2020 2058 656e 6961 6c20 5865 7275  1    Xenial Xeru
+00002060: 7320 2020 2020 2020 2020 2020 2020 2020  s               
 00002070: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002090: 2020 2020 2020 2020 2020 2020 2020 200a                 .
-000020a0: 2020 2020 2031 342e 3034 204c 5453 2020       14.04 LTS  
-000020b0: 2020 3230 3134 2d30 342d 3137 2020 2020    2014-04-17    
-000020c0: 2031 342e 3034 2e36 2020 2020 3230 3139   14.04.6    2019
-000020d0: 2d30 342d 3032 2020 2020 3230 3234 2d30  -04-02    2024-0
-000020e0: 342d 3031 2020 2020 5472 7573 7479 2054  4-01    Trusty T
-000020f0: 6168 7220 2020 2020 2020 2020 2020 2020  ahr             
+00002090: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+000020a0: 2020 2031 342e 3034 204c 5453 2020 2020     14.04 LTS    
+000020b0: 3230 3134 2d30 342d 3137 2020 2020 3134  2014-04-17    14
+000020c0: 2e30 342e 3620 2020 2032 3031 392d 3034  .04.6    2019-04
+000020d0: 2d30 3220 2020 2032 3032 342d 3034 2d30  -02    2024-04-0
+000020e0: 3120 2020 2054 7275 7374 7920 5461 6872  1    Trusty Tahr
+000020f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002100: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00002110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002130: 0a20 2020 203d 3d3d 3d3d 3d3d 3d3d 3d3d  .    ===========
-00002140: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d20    ============= 
-00002150: 203d 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d   =========  ====
-00002160: 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d  ========  ======
-00002170: 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d  ======  ========
-00002180: 3d3d 3d3d 3d3d 3d3d 3d20 203d 3d3d 3d3d  =========  =====
+00002120: 2020 2020 2020 2020 2020 2020 200a 2020               .  
+00002130: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 203d    ===========  =
+00002140: 3d3d 3d3d 3d3d 3d3d 3d3d 3d20 203d 3d3d  ===========  ===
+00002150: 3d3d 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d  ======  ========
+00002160: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
+00002170: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
+00002180: 3d3d 3d3d 3d20 203d 3d3d 3d3d 3d3d 3d3d  =====  =========
 00002190: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 000021a0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000021b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-000021c0: 3d0a 2222 2220 2023 206e 6f71 613a 2045  =."""  # noqa: E
-000021d0: 3530 3120 5732 3931 0a0a 4558 5045 4354  501 W291..EXPECT
-000021e0: 4544 5f54 5356 203d 2022 2222 0a22 6379  ED_TSV = """."cy
-000021f0: 636c 6522 0922 7265 6c65 6173 6544 6174  cle"."releaseDat
-00002200: 6522 0922 6c61 7465 7374 2209 2273 7570  e"."latest"."sup
-00002210: 706f 7274 2209 2265 6f6c 2209 2263 6f64  port"."eol"."cod
-00002220: 656e 616d 6522 0922 6c69 6e6b 220a 2232  ename"."link"."2
-00002230: 322e 3034 204c 5453 2209 2232 3032 322d  2.04 LTS"."2022-
-00002240: 3034 2d32 3122 0922 3232 2e30 3422 0922  04-21"."22.04"."
-00002250: 3230 3237 2d30 342d 3032 2209 2232 3033  2027-04-02"."203
-00002260: 322d 3034 2d30 3122 0922 4a61 6d6d 7920  2-04-01"."Jammy 
-00002270: 4a65 6c6c 7966 6973 6822 0922 6874 7470  Jellyfish"."http
-00002280: 733a 2f2f 7769 6b69 2e75 6275 6e74 752e  s://wiki.ubuntu.
-00002290: 636f 6d2f 4a61 6d6d 794a 656c 6c79 6669  com/JammyJellyfi
-000022a0: 7368 2f52 656c 6561 7365 4e6f 7465 732f  sh/ReleaseNotes/
-000022b0: 220a 2232 312e 3130 2209 2232 3032 312d  "."21.10"."2021-
-000022c0: 3130 2d31 3422 0922 3231 2e31 3022 0922  10-14"."21.10"."
-000022d0: 3230 3232 2d30 372d 3331 2209 2232 3032  2022-07-31"."202
-000022e0: 322d 3037 2d33 3122 0922 496d 7069 7368  2-07-31"."Impish
-000022f0: 2049 6e64 7269 2209 2268 7474 7073 3a2f   Indri"."https:/
-00002300: 2f77 696b 692e 7562 756e 7475 2e63 6f6d  /wiki.ubuntu.com
-00002310: 2f49 6d70 6973 6849 6e64 7269 2f52 656c  /ImpishIndri/Rel
-00002320: 6561 7365 4e6f 7465 732f 220a 2232 312e  easeNotes/"."21.
-00002330: 3034 2209 2232 3032 312d 3034 2d32 3222  04"."2021-04-22"
-00002340: 0922 3231 2e30 3422 0922 3230 3232 2d30  ."21.04"."2022-0
-00002350: 312d 3230 2209 2232 3032 322d 3031 2d32  1-20"."2022-01-2
-00002360: 3022 0922 4869 7273 7574 6520 4869 7070  0"."Hirsute Hipp
-00002370: 6f22 0922 6874 7470 733a 2f2f 7769 6b69  o"."https://wiki
-00002380: 2e75 6275 6e74 752e 636f 6d2f 4869 7273  .ubuntu.com/Hirs
-00002390: 7574 6548 6970 706f 2f52 656c 6561 7365  uteHippo/Release
-000023a0: 4e6f 7465 732f 220a 2232 302e 3130 2209  Notes/"."20.10".
-000023b0: 2232 3032 302d 3130 2d32 3222 0922 3230  "2020-10-22"."20
-000023c0: 2e31 3022 0922 3230 3231 2d30 372d 3232  .10"."2021-07-22
-000023d0: 2209 2232 3032 312d 3037 2d32 3222 0922  "."2021-07-22"."
-000023e0: 4772 6f6f 7679 2047 6f72 696c 6c61 2209  Groovy Gorilla".
-000023f0: 0a22 3230 2e30 3420 4c54 5322 0922 3230  ."20.04 LTS"."20
-00002400: 3230 2d30 342d 3233 2209 2232 302e 3034  20-04-23"."20.04
-00002410: 2e34 2209 2232 3032 352d 3034 2d30 3222  .4"."2025-04-02"
-00002420: 0922 3230 3330 2d30 342d 3031 2209 2246  ."2030-04-01"."F
-00002430: 6f63 616c 2046 6f73 7361 2209 0a22 3139  ocal Fossa".."19
-00002440: 2e31 3022 0922 3230 3139 2d31 302d 3137  .10"."2019-10-17
-00002450: 2209 2231 392e 3130 2209 2232 3032 302d  "."19.10"."2020-
-00002460: 3037 2d30 3622 0922 3230 3230 2d30 372d  07-06"."2020-07-
-00002470: 3036 2209 224b 6172 6d69 6320 4b6f 616c  06"."Karmic Koal
-00002480: 6122 090a 2231 382e 3034 204c 5453 2209  a".."18.04 LTS".
-00002490: 2232 3031 382d 3034 2d32 3622 0922 3138  "2018-04-26"."18
-000024a0: 2e30 342e 3622 0922 3230 3233 2d30 342d  .04.6"."2023-04-
-000024b0: 3032 2209 2232 3032 382d 3034 2d30 3122  02"."2028-04-01"
-000024c0: 0922 4269 6f6e 6963 2042 6561 7665 7222  ."Bionic Beaver"
-000024d0: 0922 6874 7470 733a 2f2f 7769 6b69 2e75  ."https://wiki.u
-000024e0: 6275 6e74 752e 636f 6d2f 4269 6f6e 6963  buntu.com/Bionic
-000024f0: 4265 6176 6572 2f52 656c 6561 7365 4e6f  Beaver/ReleaseNo
-00002500: 7465 7322 0a22 3136 2e30 3420 4c54 5322  tes"."16.04 LTS"
-00002510: 0922 3230 3136 2d30 342d 3231 2209 2231  ."2016-04-21"."1
-00002520: 362e 3034 2e37 2209 2232 3032 312d 3034  6.04.7"."2021-04
-00002530: 2d30 3222 0922 3230 3236 2d30 342d 3031  -02"."2026-04-01
-00002540: 2209 2258 656e 6961 6c20 5865 7275 7322  "."Xenial Xerus"
-00002550: 090a 2231 342e 3034 204c 5453 2209 2232  .."14.04 LTS"."2
-00002560: 3031 342d 3034 2d31 3722 0922 3134 2e30  014-04-17"."14.0
-00002570: 342e 3622 0922 3230 3139 2d30 342d 3032  4.6"."2019-04-02
-00002580: 2209 2232 3032 342d 3034 2d30 3122 0922  "."2024-04-01"."
-00002590: 5472 7573 7479 2054 6168 7222 090a 2222  Trusty Tahr"..""
-000025a0: 2220 2023 206e 6f71 613a 2045 3530 3120  "  # noqa: E501 
-000025b0: 5732 3931 0a                             W291.
+000021b0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2222  =============.""
+000021c0: 2220 2023 206e 6f71 613a 2045 3530 3120  "  # noqa: E501 
+000021d0: 5732 3931 0a0a 4558 5045 4354 4544 5f54  W291..EXPECTED_T
+000021e0: 5356 203d 2022 2222 0a22 6379 636c 6522  SV = """."cycle"
+000021f0: 0922 7265 6c65 6173 6522 0922 6c61 7465  ."release"."late
+00002200: 7374 2209 2273 7570 706f 7274 2209 2265  st"."support"."e
+00002210: 6f6c 2209 2263 6f64 656e 616d 6522 0922  ol"."codename"."
+00002220: 6c69 6e6b 220a 2232 322e 3034 204c 5453  link"."22.04 LTS
+00002230: 2209 2232 3032 322d 3034 2d32 3122 0922  "."2022-04-21"."
+00002240: 3232 2e30 3422 0922 3230 3237 2d30 342d  22.04"."2027-04-
+00002250: 3032 2209 2232 3033 322d 3034 2d30 3122  02"."2032-04-01"
+00002260: 0922 4a61 6d6d 7920 4a65 6c6c 7966 6973  ."Jammy Jellyfis
+00002270: 6822 0922 6874 7470 733a 2f2f 7769 6b69  h"."https://wiki
+00002280: 2e75 6275 6e74 752e 636f 6d2f 4a61 6d6d  .ubuntu.com/Jamm
+00002290: 794a 656c 6c79 6669 7368 2f52 656c 6561  yJellyfish/Relea
+000022a0: 7365 4e6f 7465 732f 220a 2232 312e 3130  seNotes/"."21.10
+000022b0: 2209 2232 3032 312d 3130 2d31 3422 0922  "."2021-10-14"."
+000022c0: 3231 2e31 3022 0922 3230 3232 2d30 372d  21.10"."2022-07-
+000022d0: 3331 2209 2232 3032 322d 3037 2d33 3122  31"."2022-07-31"
+000022e0: 0922 496d 7069 7368 2049 6e64 7269 2209  ."Impish Indri".
+000022f0: 2268 7474 7073 3a2f 2f77 696b 692e 7562  "https://wiki.ub
+00002300: 756e 7475 2e63 6f6d 2f49 6d70 6973 6849  untu.com/ImpishI
+00002310: 6e64 7269 2f52 656c 6561 7365 4e6f 7465  ndri/ReleaseNote
+00002320: 732f 220a 2232 312e 3034 2209 2232 3032  s/"."21.04"."202
+00002330: 312d 3034 2d32 3222 0922 3231 2e30 3422  1-04-22"."21.04"
+00002340: 0922 3230 3232 2d30 312d 3230 2209 2232  ."2022-01-20"."2
+00002350: 3032 322d 3031 2d32 3022 0922 4869 7273  022-01-20"."Hirs
+00002360: 7574 6520 4869 7070 6f22 0922 6874 7470  ute Hippo"."http
+00002370: 733a 2f2f 7769 6b69 2e75 6275 6e74 752e  s://wiki.ubuntu.
+00002380: 636f 6d2f 4869 7273 7574 6548 6970 706f  com/HirsuteHippo
+00002390: 2f52 656c 6561 7365 4e6f 7465 732f 220a  /ReleaseNotes/".
+000023a0: 2232 302e 3130 2209 2232 3032 302d 3130  "20.10"."2020-10
+000023b0: 2d32 3222 0922 3230 2e31 3022 0922 3230  -22"."20.10"."20
+000023c0: 3231 2d30 372d 3232 2209 2232 3032 312d  21-07-22"."2021-
+000023d0: 3037 2d32 3222 0922 4772 6f6f 7679 2047  07-22"."Groovy G
+000023e0: 6f72 696c 6c61 2209 0a22 3230 2e30 3420  orilla".."20.04 
+000023f0: 4c54 5322 0922 3230 3230 2d30 342d 3233  LTS"."2020-04-23
+00002400: 2209 2232 302e 3034 2e34 2209 2232 3032  "."20.04.4"."202
+00002410: 352d 3034 2d30 3222 0922 3230 3330 2d30  5-04-02"."2030-0
+00002420: 342d 3031 2209 2246 6f63 616c 2046 6f73  4-01"."Focal Fos
+00002430: 7361 2209 0a22 3139 2e31 3022 0922 3230  sa".."19.10"."20
+00002440: 3139 2d31 302d 3137 2209 2231 392e 3130  19-10-17"."19.10
+00002450: 2209 2232 3032 302d 3037 2d30 3622 0922  "."2020-07-06"."
+00002460: 3230 3230 2d30 372d 3036 2209 224b 6172  2020-07-06"."Kar
+00002470: 6d69 6320 4b6f 616c 6122 090a 2231 382e  mic Koala".."18.
+00002480: 3034 204c 5453 2209 2232 3031 382d 3034  04 LTS"."2018-04
+00002490: 2d32 3622 0922 3138 2e30 342e 3622 0922  -26"."18.04.6"."
+000024a0: 3230 3233 2d30 342d 3032 2209 2232 3032  2023-04-02"."202
+000024b0: 382d 3034 2d30 3122 0922 4269 6f6e 6963  8-04-01"."Bionic
+000024c0: 2042 6561 7665 7222 0922 6874 7470 733a   Beaver"."https:
+000024d0: 2f2f 7769 6b69 2e75 6275 6e74 752e 636f  //wiki.ubuntu.co
+000024e0: 6d2f 4269 6f6e 6963 4265 6176 6572 2f52  m/BionicBeaver/R
+000024f0: 656c 6561 7365 4e6f 7465 7322 0a22 3136  eleaseNotes"."16
+00002500: 2e30 3420 4c54 5322 0922 3230 3136 2d30  .04 LTS"."2016-0
+00002510: 342d 3231 2209 2231 362e 3034 2e37 2209  4-21"."16.04.7".
+00002520: 2232 3032 312d 3034 2d30 3222 0922 3230  "2021-04-02"."20
+00002530: 3236 2d30 342d 3031 2209 2258 656e 6961  26-04-01"."Xenia
+00002540: 6c20 5865 7275 7322 090a 2231 342e 3034  l Xerus".."14.04
+00002550: 204c 5453 2209 2232 3031 342d 3034 2d31   LTS"."2014-04-1
+00002560: 3722 0922 3134 2e30 342e 3622 0922 3230  7"."14.04.6"."20
+00002570: 3139 2d30 342d 3032 2209 2232 3032 342d  19-04-02"."2024-
+00002580: 3034 2d30 3122 0922 5472 7573 7479 2054  04-01"."Trusty T
+00002590: 6168 7222 090a 2222 2220 2023 206e 6f71  ahr".."""  # noq
+000025a0: 613a 2045 3530 3120 5732 3931 0a0a 4558  a: E501 W291..EX
+000025b0: 5045 4354 4544 5f4d 445f 4c4f 4734 4a20  PECTED_MD_LOG4J 
+000025c0: 3d20 2222 220a 7c20 6379 636c 6520 7c20  = """.| cycle | 
+000025d0: 2072 656c 6561 7365 2020 207c 206c 6174   release   | lat
+000025e0: 6573 7420 7c20 2020 2065 6f6c 2020 2020  est |    eol    
+000025f0: 207c 0a7c 3a2d 2d2d 2d2d 2d7c 3a2d 2d2d   |.|:------|:---
+00002600: 2d2d 2d2d 2d2d 2d3a 7c3a 2d2d 2d2d 2d2d  -------:|:------
+00002610: 2d7c 3a2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a  -|:----------:|.
+00002620: 7c20 3220 2020 2020 7c20 3230 3134 2d30  | 2     | 2014-0
+00002630: 372d 3132 207c 2032 2e31 372e 3220 7c20  7-12 | 2.17.2 | 
+00002640: 2020 4661 6c73 6520 2020 207c 0a7c 2032    False    |.| 2
+00002650: 2e31 3220 207c 2032 3031 392d 3036 2d32  .12  | 2019-06-2
+00002660: 3320 7c20 322e 3132 2e34 207c 2032 3032  3 | 2.12.4 | 202
+00002670: 312d 3132 2d31 3420 7c0a 7c20 322e 3320  1-12-14 |.| 2.3 
+00002680: 2020 7c20 3230 3135 2d30 352d 3039 207c    | 2015-05-09 |
+00002690: 2032 2e33 2e32 2020 7c20 3230 3135 2d30   2.3.2  | 2015-0
+000026a0: 392d 3230 207c 0a7c 2031 2020 2020 207c  9-20 |.| 1     |
+000026b0: 2032 3030 312d 3031 2d30 3820 7c20 312e   2001-01-08 | 1.
+000026c0: 322e 3137 207c 2032 3031 352d 3130 2d31  2.17 | 2015-10-1
+000026d0: 3520 7c0a 2222 220a 0a45 5850 4543 5445  5 |."""..EXPECTE
+000026e0: 445f 4d44 5f50 5954 484f 4e20 3d20 2222  D_MD_PYTHON = ""
+000026f0: 220a 7c20 6379 636c 6520 7c20 2072 656c  ".| cycle |  rel
+00002700: 6561 7365 2020 207c 206c 6174 6573 7420  ease   | latest 
+00002710: 7c20 6c61 7465 7374 2072 656c 6561 7365  | latest release
+00002720: 207c 2020 2020 656f 6c20 2020 2020 7c0a   |    eol     |.
+00002730: 7c3a 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d  |:------|:------
+00002740: 2d2d 2d2d 3a7c 3a2d 2d2d 2d2d 2d2d 7c3a  ----:|:-------|:
+00002750: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 3a7c  --------------:|
+00002760: 3a2d 2d2d 2d2d 2d2d 2d2d 2d3a 7c0a 7c20  :----------:|.| 
+00002770: 332e 3130 2020 7c20 3230 3231 2d31 302d  3.10  | 2021-10-
+00002780: 3034 207c 2033 2e31 302e 3520 7c20 2020  04 | 3.10.5 |   
+00002790: 3230 3232 2d30 362d 3036 2020 207c 2032  2022-06-06   | 2
+000027a0: 3032 362d 3130 2d30 3420 7c0a 7c20 332e  026-10-04 |.| 3.
+000027b0: 3920 2020 7c20 3230 3230 2d31 302d 3035  9   | 2020-10-05
+000027c0: 207c 2033 2e39 2e31 3320 7c20 2020 3230   | 3.9.13 |   20
+000027d0: 3232 2d30 352d 3137 2020 207c 2032 3032  22-05-17   | 202
+000027e0: 352d 3130 2d30 3520 7c0a 7c20 332e 3820  5-10-05 |.| 3.8 
+000027f0: 2020 7c20 3230 3139 2d31 302d 3134 207c    | 2019-10-14 |
+00002800: 2033 2e38 2e31 3320 7c20 2020 3230 3232   3.8.13 |   2022
+00002810: 2d30 332d 3136 2020 207c 2032 3032 342d  -03-16   | 2024-
+00002820: 3130 2d31 3420 7c0a 7c20 332e 3720 2020  10-14 |.| 3.7   
+00002830: 7c20 3230 3138 2d30 362d 3236 207c 2033  | 2018-06-26 | 3
+00002840: 2e37 2e31 3320 7c20 2020 3230 3232 2d30  .7.13 |   2022-0
+00002850: 332d 3136 2020 207c 2032 3032 332d 3036  3-16   | 2023-06
+00002860: 2d32 3720 7c0a 7c20 332e 3620 2020 7c20  -27 |.| 3.6   | 
+00002870: 3230 3136 2d31 322d 3232 207c 2033 2e36  2016-12-22 | 3.6
+00002880: 2e31 3520 7c20 2020 3230 3231 2d30 392d  .15 |   2021-09-
+00002890: 3033 2020 207c 2032 3032 312d 3132 2d32  03   | 2021-12-2
+000028a0: 3320 7c0a 7c20 332e 3520 2020 7c20 3230  3 |.| 3.5   | 20
+000028b0: 3135 2d30 392d 3132 207c 2033 2e35 2e31  15-09-12 | 3.5.1
+000028c0: 3020 7c20 2020 3230 3230 2d30 392d 3035  0 |   2020-09-05
+000028d0: 2020 207c 2032 3032 302d 3039 2d31 3320     | 2020-09-13 
+000028e0: 7c0a 7c20 332e 3420 2020 7c20 3230 3134  |.| 3.4   | 2014
+000028f0: 2d30 332d 3135 207c 2033 2e34 2e31 3020  -03-15 | 3.4.10 
+00002900: 7c20 2020 3230 3139 2d30 332d 3138 2020  |   2019-03-18  
+00002910: 207c 2032 3031 392d 3033 2d31 3820 7c0a   | 2019-03-18 |.
+00002920: 7c20 332e 3320 2020 7c20 3230 3132 2d30  | 3.3   | 2012-0
+00002930: 392d 3239 207c 2033 2e33 2e37 2020 7c20  9-29 | 3.3.7  | 
+00002940: 2020 3230 3137 2d30 392d 3139 2020 207c    2017-09-19   |
+00002950: 2032 3031 372d 3039 2d32 3920 7c0a 7c20   2017-09-29 |.| 
+00002960: 322e 3720 2020 7c20 3230 3130 2d30 372d  2.7   | 2010-07-
+00002970: 3033 207c 2032 2e37 2e31 3820 7c20 2020  03 | 2.7.18 |   
+00002980: 3230 3230 2d30 342d 3139 2020 207c 2032  2020-04-19   | 2
+00002990: 3032 302d 3031 2d30 3120 7c0a 2222 220a  020-01-01 |.""".
```

### Comparing `norwegianblue-0.8.1/tests/test_cache.py` & `norwegianblue-0.9.0/tests/test_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Unit tests for norwegianblue cache
 """
+from __future__ import annotations
+
 import tempfile
 from pathlib import Path
 
 from freezegun import freeze_time
 
 from norwegianblue import _cache
```

### Comparing `norwegianblue-0.8.1/tests/test_norwegianblue.py` & `norwegianblue-0.9.0/tests/test_norwegianblue.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """
 Unit tests for norwegianblue
 """
+from __future__ import annotations
+
 import json
 import os
 from pathlib import Path
 from unittest import mock
 
 import pytest
 import respx
@@ -13,113 +15,25 @@
 import norwegianblue
 from norwegianblue import _cache
 
 from .data.expected_output import (
     EXPECTED_HTML,
     EXPECTED_MD,
     EXPECTED_MD_COLOUR,
+    EXPECTED_MD_LOG4J,
+    EXPECTED_MD_PYTHON,
     EXPECTED_RST,
     EXPECTED_TSV,
 )
-
-SAMPLE_RESPONSE_JSON = """
-[
-  {
-    "cycle": "22.04",
-    "codename": "Jammy Jellyfish",
-    "support": "2027-04-02",
-    "eol": "2032-04-01",
-    "lts": true,
-    "latest": "22.04",
-    "link": "https://wiki.ubuntu.com/JammyJellyfish/ReleaseNotes/",
-    "releaseDate": "2022-04-21"
-  },
-  {
-    "cycle": "21.10",
-    "codename": "Impish Indri",
-    "support": "2022-07-31",
-    "eol": "2022-07-31",
-    "latest": "21.10",
-    "link": "https://wiki.ubuntu.com/ImpishIndri/ReleaseNotes/",
-    "releaseDate": "2021-10-14"
-  },
-  {
-    "cycle": "21.04",
-    "codename": "Hirsute Hippo",
-    "support": "2022-01-20",
-    "eol": "2022-01-20",
-    "latest": "21.04",
-    "link": "https://wiki.ubuntu.com/HirsuteHippo/ReleaseNotes/",
-    "releaseDate": "2021-04-22"
-  },
-  {
-    "cycle": "20.10",
-    "codename": "Groovy Gorilla",
-    "support": "2021-07-22",
-    "eol": "2021-07-22",
-    "latest": "20.10",
-    "releaseDate": "2020-10-22"
-  },
-  {
-    "cycle": "20.04",
-    "codename": "Focal Fossa",
-    "lts": true,
-    "support": "2025-04-02",
-    "eol": "2030-04-01",
-    "latest": "20.04.4",
-    "releaseDate": "2020-04-23"
-  },
-  {
-    "cycle": "19.10",
-    "codename": "Karmic Koala",
-    "support": "2020-07-06",
-    "eol": "2020-07-06",
-    "latest": "19.10",
-    "releaseDate": "2019-10-17"
-  },
-  {
-    "cycle": "18.04",
-    "codename": "Bionic Beaver",
-    "lts": true,
-    "support": "2023-04-02",
-    "eol": "2028-04-01",
-    "latest": "18.04.6",
-    "link": "https://wiki.ubuntu.com/BionicBeaver/ReleaseNotes",
-    "releaseDate": "2018-04-26"
-  },
-  {
-    "cycle": "16.04",
-    "codename": "Xenial Xerus",
-    "lts": true,
-    "support": "2021-04-02",
-    "eol": "2026-04-01",
-    "latest": "16.04.7",
-    "releaseDate": "2016-04-21"
-  },
-  {
-    "cycle": "14.04",
-    "codename": "Trusty Tahr",
-    "lts": true,
-    "support": "2019-04-02",
-    "eol": "2024-04-01",
-    "latest": "14.04.6",
-    "releaseDate": "2014-04-17"
-  }
-]
-"""
-
-SAMPLE_RESPONSE_ALL_JSON = """
-[
-    "alpine",
-    "amazon-linux",
-    "android",
-    "bootstrap",
-    "centos"
-]
-"""
+from .data.sample_response import (
+    SAMPLE_RESPONSE_ALL_JSON,
+    SAMPLE_RESPONSE_JSON_LOG4J,
+    SAMPLE_RESPONSE_JSON_PYTHON,
+    SAMPLE_RESPONSE_JSON_UBUNTU,
+)
 
 
 def stub__cache_filename(*args):
     return Path("/this/does/not/exist")
 
 
 def stub__save_cache(*args) -> None:
@@ -145,32 +59,61 @@
         [
             pytest.param("html", EXPECTED_HTML, id="html"),
             pytest.param("markdown", EXPECTED_MD, id="markdown"),
             pytest.param("rst", EXPECTED_RST, id="rst"),
             pytest.param("tsv", EXPECTED_TSV, id="tsv"),
         ],
     )
-    def test_norwegianblue(self, test_format: str, expected: str) -> None:
+    def test_norwegianblue_formats(self, test_format: str, expected: str) -> None:
         # Arrange
         mocked_url = "https://endoflife.date/api/ubuntu.json"
-        mocked_response = SAMPLE_RESPONSE_JSON
+        mocked_response = SAMPLE_RESPONSE_JSON_UBUNTU
 
         # Act
         respx.get(mocked_url).respond(content=mocked_response)
         output = norwegianblue.norwegianblue(product="ubuntu", format=test_format)
 
         # Assert
         assert output.strip() == expected.strip()
 
+    @respx.mock
+    @pytest.mark.parametrize(
+        "test_product, sample_response, expected",
+        [
+            pytest.param(
+                "log4j", SAMPLE_RESPONSE_JSON_LOG4J, EXPECTED_MD_LOG4J, id="log4j"
+            ),
+            pytest.param(
+                "python", SAMPLE_RESPONSE_JSON_PYTHON, EXPECTED_MD_PYTHON, id="python"
+            ),
+        ],
+    )
+    def test_norwegianblue_products(
+        self, test_product: str, sample_response: str, expected: str
+    ) -> None:
+        """Test other headers not present in Ubuntu:
+        * rename of releaseDate and latestReleaseDate headers (Python)
+        * skip of cycleShortHand (Log4j)"""
+        # Arrange
+        mocked_url = f"https://endoflife.date/api/{test_product}.json"
+        mocked_response = sample_response
+
+        # Act
+        respx.get(mocked_url).respond(content=mocked_response)
+        output = norwegianblue.norwegianblue(product=test_product, format="markdown")
+
+        # Assert
+        assert output.strip() == expected.strip()
+
     @mock.patch.dict(os.environ, {"NO_COLOR": "TRUE"})
     @respx.mock
     def test_norwegianblue_no_color(self) -> None:
         # Arrange
         mocked_url = "https://endoflife.date/api/ubuntu.json"
-        mocked_response = SAMPLE_RESPONSE_JSON
+        mocked_response = SAMPLE_RESPONSE_JSON_UBUNTU
         expected = EXPECTED_MD
 
         # Act
         respx.get(mocked_url).respond(content=mocked_response)
         output = norwegianblue.norwegianblue(product="ubuntu")
 
         # Assert
@@ -178,36 +121,36 @@
 
     @freeze_time("2021-09-13")
     @mock.patch.dict(os.environ, {"FORCE_COLOR": "TRUE"})
     @respx.mock
     def test_norwegianblue_force_color(self) -> None:
         # Arrange
         mocked_url = "https://endoflife.date/api/ubuntu.json"
-        mocked_response = SAMPLE_RESPONSE_JSON
+        mocked_response = SAMPLE_RESPONSE_JSON_UBUNTU
         expected = EXPECTED_MD_COLOUR
 
         # Act
         respx.get(mocked_url).respond(content=mocked_response)
         output = norwegianblue.norwegianblue(product="ubuntu")
 
         # Assert
         assert output.strip() == expected.strip()
 
     @respx.mock
     def test_norwegianblue_json(self) -> None:
         # Arrange
         mocked_url = "https://endoflife.date/api/ubuntu.json"
-        mocked_response = SAMPLE_RESPONSE_JSON
+        mocked_response = SAMPLE_RESPONSE_JSON_UBUNTU
 
         # Act
         respx.get(mocked_url).respond(content=mocked_response)
         output = norwegianblue.norwegianblue(product="ubuntu", format="json")
 
         # Assert
-        assert json.loads(output) == json.loads(SAMPLE_RESPONSE_JSON)
+        assert json.loads(output) == json.loads(SAMPLE_RESPONSE_JSON_UBUNTU)
 
     @freeze_time("2021-06-15")
     def test__colourify(self) -> None:
         # Arrange
         data = [
             {
                 "cycle": "21.04 LTS",
```

### Comparing `norwegianblue-0.8.1/tox.ini` & `norwegianblue-0.9.0/tox.ini`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tox]
 envlist =
     cog
     lint
     pins
-    py{311, 310, 39, 38, 37}
+    py{py3, 311, 310, 39, 38, 37}
+isolated_build = true
 
 [testenv]
 extras =
     tests
 commands =
-    {envpython} -m pytest --cov norwegianblue --cov tests --cov-report xml {posargs}
+    {envpython} -m pytest --cov norwegianblue --cov tests --cov-report html --cov-report term --cov-report xml {posargs}
     norwegianblue --version
     norwegianblue --help
     eol --version
     eol --help
 
 [testenv:cog]
 skip_install = true
@@ -25,14 +26,14 @@
 [testenv:lint]
 passenv =
     PRE_COMMIT_COLOR
 skip_install = true
 deps =
     pre-commit
 commands =
-    pre-commit run --all-files
+    pre-commit run --all-files --show-diff-on-failure
 
 [testenv:pins]
 extras =
     None
 commands_pre =
     {envpython} -m pip install -r requirements.txt
```


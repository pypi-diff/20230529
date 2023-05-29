# Comparing `tmp/srecli-0.0.4.tar.gz` & `tmp/srecli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srecli-0.0.4.tar", last modified: Sun May 28 14:21:28 2023, max compression
+gzip compressed data, was "srecli-0.0.5.tar", last modified: Mon May 29 15:02:08 2023, max compression
```

## Comparing `srecli-0.0.4.tar` & `srecli-0.0.5.tar`

### file list

```diff
@@ -1,31 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:28.207370 srecli-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:28.203370 srecli-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:28.203370 srecli-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-28 14:21:12.000000 srecli-0.0.4/.github/workflows/build_and_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-28 14:21:12.000000 srecli-0.0.4/.github/workflows/pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-28 14:21:12.000000 srecli-0.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-28 14:21:12.000000 srecli-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-28 14:21:28.207370 srecli-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-28 14:21:12.000000 srecli-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2285 2023-05-28 14:21:12.000000 srecli-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-28 14:21:12.000000 srecli-0.0.4/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-28 14:21:12.000000 srecli-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 14:21:28.207370 srecli-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-28 14:21:12.000000 srecli-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:28.203370 srecli-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:28.203370 srecli-0.0.4/src/srecli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:12.000000 srecli-0.0.4/src/srecli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-28 14:21:12.000000 srecli-0.0.4/src/srecli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:28.203370 srecli-0.0.4/src/srecli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:12.000000 srecli-0.0.4/src/srecli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-28 14:21:12.000000 srecli-0.0.4/src/srecli/commands/cmd_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:28.203370 srecli-0.0.4/src/srecli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-28 14:21:28.000000 srecli-0.0.4/src/srecli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-28 14:21:28.000000 srecli-0.0.4/src/srecli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:21:28.000000 srecli-0.0.4/src/srecli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-28 14:21:28.000000 srecli-0.0.4/src/srecli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-28 14:21:28.000000 srecli-0.0.4/src/srecli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-28 14:21:28.000000 srecli-0.0.4/src/srecli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:28.203370 srecli-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 14:21:12.000000 srecli-0.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-28 14:21:12.000000 srecli-0.0.4/tests/test_status_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.708823 srecli-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.704823 srecli-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.704823 srecli-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-29 15:01:57.000000 srecli-0.0.5/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 15:01:57.000000 srecli-0.0.5/.github/workflows/pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-29 15:01:57.000000 srecli-0.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-29 15:01:57.000000 srecli-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 15:02:08.708823 srecli-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 15:01:57.000000 srecli-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 15:01:57.000000 srecli-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 15:01:57.000000 srecli-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:02:08.708823 srecli-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 15:01:57.000000 srecli-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.704823 srecli-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.708823 srecli-0.0.5/src/srecli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:01:57.000000 srecli-0.0.5/src/srecli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-29 15:01:57.000000 srecli-0.0.5/src/srecli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.708823 srecli-0.0.5/src/srecli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:01:57.000000 srecli-0.0.5/src/srecli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-29 15:01:57.000000 srecli-0.0.5/src/srecli/commands/cmd_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.708823 srecli-0.0.5/src/srecli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.708823 srecli-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:01:57.000000 srecli-0.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-29 15:01:57.000000 srecli-0.0.5/tests/test_status_show.py
```

### Comparing `srecli-0.0.4/.github/workflows/build_and_publish.yaml` & `srecli-0.0.5/.github/workflows/build.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Build and Publish to PyPI
+name: Build Python package
 
 on:
   push:
     branches: [ "main" ]
   pull_request:
     branches: [ "main" ]
 
@@ -18,15 +18,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4.0.0
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install tox
+        python -m pip install -r requirements.txt
     - name: Formatting code with black
       run: |
         tox -e format
   lint:
     name: Code linting
     runs-on: ubuntu-latest
     strategy:
@@ -37,15 +37,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4.0.0
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install tox
+        python -m pip install -r requirements.txt
     - name: Linting code with flake8
       run: |
         tox -e lint
   typecheck:
     name: Code type checking
     runs-on: ubuntu-latest
     strategy:
@@ -56,15 +56,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4.0.0
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install tox
+        python -m pip install -r requirements.txt
     - name: Type checking code with flake8
       run: |
         tox -e typecheck
   test:
     name: Code testing
     runs-on: ubuntu-latest
     strategy:
@@ -81,15 +81,15 @@
     - name: Set up Python ${{ matrix.python.version }}
       uses: actions/setup-python@v4.0.0
       with:
         python-version: ${{ matrix.python.version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        pip install tox
+        python -m pip install -r requirements.txt
     - name: Testing code with pytest
       run: |
         tox -e ${{ matrix.python.toxenv }}
   build_source_dist:
     name: Build source distribution
     runs-on: ubuntu-latest
     strategy:
@@ -100,15 +100,15 @@
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4.0.0
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install build
+        python -m pip install -r requirements.txt
     - name: Building source distribution package
       run: |
         python -m build --sdist
     - uses: actions/upload-artifact@v3
       with:
         path: ./dist/*.tar.gz
   build_wheels:
@@ -124,14 +124,14 @@
     - name: Set up Python ${{ matrix.target.python-version }}
       uses: actions/setup-python@v4.0.0
       with:
         python-version: ${{ matrix.target.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install build
+        python -m pip install -r requirements.txt
     - name: Building wheels for ${{ matrix.target.os }}
       run: |
         python -m build --wheel
     - uses: actions/upload-artifact@v3
       with:
         path: ./dist/*.whl
```

### Comparing `srecli-0.0.4/.github/workflows/pypi_publish.yaml` & `srecli-0.0.5/.github/workflows/pypi_publish.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Publish package to PyPI
+name: Publish Python package to PyPI
 
 on:
   release:
     types: [published]
 
 permissions:
   contents: read
@@ -16,15 +16,15 @@
     - name: Set up Python 3.10
       uses: actions/setup-python@v3
       with:
         python-version: '3.10'
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
-        python -m pip install build
+        python -m pip install -r requirements.txt
     - name: Build package
       run: python -m build
     - name: Publish package
       uses: pypa/gh-action-pypi-publish@v1.5.0
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `srecli-0.0.4/.gitignore` & `srecli-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `srecli-0.0.4/LICENSE` & `srecli-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `srecli-0.0.4/PKG-INFO` & `srecli-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srecli
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI tool for common SRE related work
 Author-email: Shibhikkiran D <shibhikkiran@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `srecli-0.0.4/pyproject.toml` & `srecli-0.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 [project]
 name = "srecli"
-version = "0.0.4"
+version = "0.0.5"
 description = "CLI tool for common SRE related work"
 authors = [
     {name = "Shibhikkiran D", email = "shibhikkiran@example.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "click ~=8.1.3",
     "loguru ~=0.7.0",
-    "readchar ~=4.0.5",
-    "tox ~=4.5.2",
 ]
 
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = [
     "setuptools ~=63.2.0",
     "wheel ~=0.37.1",
@@ -35,20 +33,18 @@
 
 [project.optional-dependencies]
 dev = [
     "pylint ~=2.14.0",
     "toml ~=0.10.2",
     "yapf ~=0.32.0",
     "black ~=23.3.0",
-    "tox ~=4.5.2",
 ]
 test = [
     "pytest-cov ~=4.1.0",
     "pytest ~=7.3.1",
-    "tox ~=4.5.2",
 ]
 ci = [
     "pylint ~=2.14.0",
     "toml ~=0.10.2",
     "yapf ~=0.32.0",
     "black ~=23.3.0",
     "pytest-cov[all] ~=3.0.0",
```

### Comparing `srecli-0.0.4/src/srecli/cli.py` & `srecli-0.0.5/src/srecli/cli.py`

 * *Files identical despite different names*

### Comparing `srecli-0.0.4/src/srecli/commands/cmd_status.py` & `srecli-0.0.5/src/srecli/commands/cmd_status.py`

 * *Files identical despite different names*

### Comparing `srecli-0.0.4/src/srecli.egg-info/PKG-INFO` & `srecli-0.0.5/src/srecli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srecli
-Version: 0.0.4
+Version: 0.0.5
 Summary: CLI tool for common SRE related work
 Author-email: Shibhikkiran D <shibhikkiran@example.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `srecli-0.0.4/tests/test_status_show.py` & `srecli-0.0.5/tests/test_status_show.py`

 * *Files identical despite different names*


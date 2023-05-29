# Comparing `tmp/clementine-0.0.2.dev0.tar.gz` & `tmp/clementine-0.0.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clementine-0.0.2.dev0.tar", last modified: Sun May 28 02:37:37 2023, max compression
+gzip compressed data, was "clementine-0.0.3.dev0.tar", last modified: Mon May 29 01:26:52 2023, max compression
```

## Comparing `clementine-0.0.2.dev0.tar` & `clementine-0.0.3.dev0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 02:37:37.514394 clementine-0.0.2.dev0/
--rw-r--r--   0 sue        (501) staff       (20)     1163 2023-05-28 02:37:37.514266 clementine-0.0.2.dev0/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)      715 2023-05-28 02:24:32.000000 clementine-0.0.2.dev0/README.md
--rw-r--r--   0 sue        (501) staff       (20)      696 2023-05-28 02:26:45.000000 clementine-0.0.2.dev0/pyproject.toml
--rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-28 02:37:37.514435 clementine-0.0.2.dev0/setup.cfg
--rw-r--r--   0 sue        (501) staff       (20)       38 2023-02-27 16:19:17.000000 clementine-0.0.2.dev0/setup.py
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 02:37:37.512303 clementine-0.0.2.dev0/src/
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 02:37:37.513123 clementine-0.0.2.dev0/src/clementine/
--rw-r--r--   0 sue        (501) staff       (20)       94 2023-05-28 02:10:59.000000 clementine-0.0.2.dev0/src/clementine/__init__.py
--rw-r--r--   0 sue        (501) staff       (20)      137 2023-05-28 02:04:08.000000 clementine-0.0.2.dev0/src/clementine/cli.py
--rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-28 02:27:14.000000 clementine-0.0.2.dev0/src/clementine/version.py
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 02:37:37.513906 clementine-0.0.2.dev0/src/clementine.egg-info/
--rw-r--r--   0 sue        (501) staff       (20)     1163 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/PKG-INFO
--rw-r--r--   0 sue        (501) staff       (20)      363 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/SOURCES.txt
--rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/dependency_links.txt
--rw-r--r--   0 sue        (501) staff       (20)       51 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/entry_points.txt
--rw-r--r--   0 sue        (501) staff       (20)       88 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/requires.txt
--rw-r--r--   0 sue        (501) staff       (20)       11 2023-05-28 02:37:37.000000 clementine-0.0.2.dev0/src/clementine.egg-info/top_level.txt
-drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-28 02:37:37.514058 clementine-0.0.2.dev0/tests/
--rw-r--r--   0 sue        (501) staff       (20)      101 2023-05-28 02:27:19.000000 clementine-0.0.2.dev0/tests/test_clementine.py
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-29 01:26:52.210205 clementine-0.0.3.dev0/
+-rw-r--r--   0 sue        (501) staff       (20)     1394 2023-05-29 01:26:52.210060 clementine-0.0.3.dev0/PKG-INFO
+-rw-r--r--   0 sue        (501) staff       (20)      855 2023-05-29 01:24:23.000000 clementine-0.0.3.dev0/README.md
+-rw-r--r--   0 sue        (501) staff       (20)      994 2023-05-29 01:04:28.000000 clementine-0.0.3.dev0/pyproject.toml
+-rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-29 01:26:52.210240 clementine-0.0.3.dev0/setup.cfg
+-rw-r--r--   0 sue        (501) staff       (20)       38 2023-05-29 01:07:57.000000 clementine-0.0.3.dev0/setup.py
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-29 01:26:52.207232 clementine-0.0.3.dev0/src/
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-29 01:26:52.208299 clementine-0.0.3.dev0/src/clementine/
+-rw-r--r--   0 sue        (501) staff       (20)      108 2023-05-29 00:46:48.000000 clementine-0.0.3.dev0/src/clementine/__init__.py
+-rw-r--r--   0 sue        (501) staff       (20)      443 2023-05-29 00:34:22.000000 clementine-0.0.3.dev0/src/clementine/cli.py
+-rw-r--r--   0 sue        (501) staff       (20)       26 2023-05-28 14:37:03.000000 clementine-0.0.3.dev0/src/clementine/version.py
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-29 01:26:52.209517 clementine-0.0.3.dev0/src/clementine.egg-info/
+-rw-r--r--   0 sue        (501) staff       (20)     1394 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/PKG-INFO
+-rw-r--r--   0 sue        (501) staff       (20)      363 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/SOURCES.txt
+-rw-r--r--   0 sue        (501) staff       (20)        1 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/dependency_links.txt
+-rw-r--r--   0 sue        (501) staff       (20)       51 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/entry_points.txt
+-rw-r--r--   0 sue        (501) staff       (20)      234 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/requires.txt
+-rw-r--r--   0 sue        (501) staff       (20)       11 2023-05-29 01:26:52.000000 clementine-0.0.3.dev0/src/clementine.egg-info/top_level.txt
+drwxr-xr-x   0 sue        (501) staff       (20)        0 2023-05-29 01:26:52.209674 clementine-0.0.3.dev0/tests/
+-rw-r--r--   0 sue        (501) staff       (20)      101 2023-05-29 00:31:28.000000 clementine-0.0.3.dev0/tests/test_clementine.py
```

### Comparing `clementine-0.0.2.dev0/README.md` & `clementine-0.0.3.dev0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -22,16 +22,30 @@
 
 ```sh
 git clone https://github.com/codesue/clementine.git
 cd clementine
 pip install -e .
 ```
 
-Building:
+Linting and formatting:
 
 ```sh
-pip install -e ".[packaging]"
+pip install -e ".[seeds]"
+pre-commit run --all-files
+```
+
+Building the docs:
+
+```sh
+cd docs
+mkdocs build
+```
+
+Distributing:
+
+```sh
+pip install -e ".[rind]"
 python -m build
 twine check dist/*
 twine upload -r testpypi dist/*
 twine upload dist/*
 ```
```

### Comparing `clementine-0.0.2.dev0/pyproject.toml` & `clementine-0.0.3.dev0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,37 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "clementine"
-version = "0.0.2-dev"
+dynamic = ["version"]
 description = "🍊 A sweet little Python package"
 authors = [{name = "Suzen Fylke", email = "codesue@users.noreply.github.com"}]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Intended Audience :: Developers",
 ]
 requires-python = ">=3.7"
 
 [project.optional-dependencies]
-dev = ["pytest"]
-ml = ["matplotlib", "numpy", "pandas", "scikit-learn", "torch"]
-packaging = ["build", "twine"]
+blossom = ["bokeh", "gradio"]
+fruit = ["matplotlib", "numpy", "pandas", "scikit-learn", "torch"]
+leaves = ["mkdocs"]
+rind = ["build", "twine"]
+seeds = ["isort", "pytest", "pre-commit", "ruff", "yapf"]
+sprout = ["notebook"]
+tree = ["clementine[blossom,fruit,leaves,rind,seeds,sprout]"]
 
 [project.urls]
 repository = "https://github.com/codesue/clementine"
 
 [project.scripts]
 clementine = "clementine.cli:main"
+
+[tool.setuptools.dynamic]
+version = {attr = "clementine.__version__"}
+
+[tool.yapf]
+based_on_style = "pep8"
+indent_width = 2
```


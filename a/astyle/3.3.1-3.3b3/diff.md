# Comparing `tmp/astyle-3.3.1.tar.gz` & `tmp/astyle-3.3b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astyle-3.3.1.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
+gzip compressed data, was "astyle-3.3b3.tar", last modified: Wed Nov  9 12:37:21 2022, max compression
```

## Comparing `astyle-3.3.1.tar` & `astyle-3.3b3.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 astyle-3.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 astyle-3.3.1/.github/workflows/main.yml
--rw-r--r--   0        0        0      535 2022-11-09 12:37:21.000000 astyle-3.3.1/.github/workflows/version.yml
--rw-r--r--   0        0        0     2346 2022-11-09 12:37:21.000000 astyle-3.3.1/.gitignore
--rwxr-xr-x   0        0        0      101 2022-11-09 12:37:21.000000 astyle-3.3.1/.gitlint
--rw-r--r--   0        0        0     2836 2022-11-09 12:37:21.000000 astyle-3.3.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 astyle-3.3.1/.pre-commit-hooks.yaml
--rwxr-xr-x   0        0        0      157 2022-11-09 12:37:21.000000 astyle-3.3.1/.yamllint.yaml
--rw-r--r--   0        0        0      771 2022-11-09 12:37:21.000000 astyle-3.3.1/CMakeLists.txt
--rw-r--r--   0        0        0    35149 2022-11-09 12:37:21.000000 astyle-3.3.1/LICENSE
--rw-r--r--   0        0        0     5321 2022-11-09 12:37:21.000000 astyle-3.3.1/README.md
--rw-r--r--   0        0        0     2137 2022-11-09 12:37:21.000000 astyle-3.3.1/pyproject.toml
--rwxr-xr-x   0        0        0      664 2022-11-09 12:37:21.000000 astyle-3.3.1/scripts/git-commit.sh
--rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 astyle-3.3.1/src/astyle/__init__.py
--rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 astyle-3.3.1/src/astyle/__main__.py
--rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 astyle-3.3.1/src/astyle/py.typed
--rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 astyle-3.3.1/tests/astyle_test.py
--rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 astyle-3.3.1/tests/expected.c
--rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 astyle-3.3.1/tests/input.c
--rw-r--r--   0        0        0     6809 2022-11-09 12:37:21.000000 astyle-3.3.1/PKG-INFO
+-rw-r--r--   0        0        0      117 2022-11-09 12:37:21.000000 astyle-3.3b3/.github/dependabot.yml
+-rw-r--r--   0        0        0     2038 2022-11-09 12:37:21.000000 astyle-3.3b3/.github/workflows/main.yml
+-rw-r--r--   0        0        0      345 2022-11-09 12:37:21.000000 astyle-3.3b3/.github/workflows/version.yml
+-rw-r--r--   0        0        0     2346 2022-11-09 12:37:21.000000 astyle-3.3b3/.gitignore
+-rwxr-xr-x   0        0        0      101 2022-11-09 12:37:21.000000 astyle-3.3b3/.gitlint
+-rw-r--r--   0        0        0     2840 2022-11-09 12:37:21.000000 astyle-3.3b3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      328 2022-11-09 12:37:21.000000 astyle-3.3b3/.pre-commit-hooks.yaml
+-rwxr-xr-x   0        0        0      157 2022-11-09 12:37:21.000000 astyle-3.3b3/.yamllint.yaml
+-rw-r--r--   0        0        0      775 2022-11-09 12:37:21.000000 astyle-3.3b3/CMakeLists.txt
+-rw-r--r--   0        0        0     4968 2022-11-09 12:37:21.000000 astyle-3.3b3/README.md
+-rw-r--r--   0        0        0     2141 2022-11-09 12:37:21.000000 astyle-3.3b3/pyproject.toml
+-rwxr-xr-x   0        0        0      784 2022-11-09 12:37:21.000000 astyle-3.3b3/scripts/git-commit.sh
+-rw-r--r--   0        0        0      396 2022-11-09 12:37:21.000000 astyle-3.3b3/src/astyle/__init__.py
+-rw-r--r--   0        0        0      246 2022-11-09 12:37:21.000000 astyle-3.3b3/src/astyle/__main__.py
+-rw-r--r--   0        0        0        0 2022-11-09 12:37:21.000000 astyle-3.3b3/src/astyle/py.typed
+-rw-r--r--   0        0        0      695 2022-11-09 12:37:21.000000 astyle-3.3b3/tests/astyle_test.py
+-rw-r--r--   0        0        0       82 2022-11-09 12:37:21.000000 astyle-3.3b3/tests/expected.c
+-rw-r--r--   0        0        0       78 2022-11-09 12:37:21.000000 astyle-3.3b3/tests/input.c
+-rw-r--r--   0        0        0     6456 2022-11-09 12:37:21.000000 astyle-3.3b3/PKG-INFO
```

### Comparing `astyle-3.3.1/.github/workflows/main.yml` & `astyle-3.3b3/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `astyle-3.3.1/.gitignore` & `astyle-3.3b3/.gitignore`

 * *Files identical despite different names*

### Comparing `astyle-3.3.1/.pre-commit-config.yaml` & `astyle-3.3b3/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     rev: 3.0.0
     hooks:
       - id: check-mailmap
       - id: shellcheck
         exclude_types:
           - zsh
   - repo: https://github.com/adrienverge/yamllint
-    rev: v1.32.0
+    rev: v1.31.0
     hooks:
       - id: yamllint
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
         additional_dependencies:
@@ -85,27 +85,27 @@
   - repo: https://github.com/pycqa/pydocstyle
     rev: 6.3.0
     hooks:
       - id: pydocstyle
         additional_dependencies:
           - tomli
   - repo: https://github.com/kumaraditya303/mirrors-pyright
-    rev: v1.1.309
+    rev: v1.1.308
     hooks:
       - id: pyright
   - repo: https://github.com/PyCQA/bandit
     rev: 1.7.5
     hooks:
       - id: bandit
         args:
           - -cpyproject.toml
         additional_dependencies:
           - tomli
   - repo: https://github.com/Freed-Wu/astyle-wheel
-    rev: "3.3"
+    rev: 3.3-beta3
     hooks:
       - id: astyle
         exclude: ^tests/input\.c$
 
 ci:
   skip:
     - shellcheck
```

### Comparing `astyle-3.3.1/CMakeLists.txt` & `astyle-3.3b3/CMakeLists.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 cmake_minimum_required(VERSION 3.10)
-set(VERSION 3.3.1)
+set(VERSION 3.3-beta3)
 include(ExternalProject)
 ExternalProject_Add(
   astyle
   URL "https://gitlab.com/saalen/astyle/-/archive/${VERSION}/astyle-${VERSION}.tar.gz"
   INSTALL_COMMAND ""
   USES_TERMINAL_DOWNLOAD 1
   USES_TERMINAL_CONFIGURE 1
```

### Comparing `astyle-3.3.1/README.md` & `astyle-3.3b3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -66,34 +66,28 @@
 ### pre-commit
 
 `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/Freed-Wu/astyle-wheel
-    rev: 3.3.1
+    rev: 3.3-beta3
     hooks:
       - id: astyle
 ```
 
 ```shell
 pre-commit install
 git commit
 ```
 
 ## Similar Projects
 
 ### pre-commit hooks
 
 - [mirrors-clang-format](https://github.com/pre-commit/mirrors-clang-format)
-- [astyle_precommit_hook](https://github.com/mellowcandle/astyle_precommit_hook):
-  it uses git hook, not pre-commit, which make it cannot use many hooks at the
-  same time.
-- [pyastyle](https://github.com/timonwong/pyastyle): stop maintaining.
-- [astyle_py](https://github.com/igrr/astyle_py): it uses wasm, not native
-  binary programs like this project.
 
 ### Python distributions
 
 - [clang-format-wheel](https://github.com/ssciwr/clang-format-wheel)
 - [cmake-python-distributions](https://github.com/scikit-build/cmake-python-distributions)
 - [ninja-python-distributions](https://github.com/scikit-build/ninja-python-distributions)
```

### Comparing `astyle-3.3.1/pyproject.toml` & `astyle-3.3b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["scikit-build-core"]
 build-backend = "scikit_build_core.build"
 
 # https://setuptools.pypa.io/en/latest/userguide/pyproject_config.html
 [project]
 name = "astyle"
-version = "3.3.1"
+version = "3.3-beta3"
 description = "Artistic Style is a source code indenter, formatter, and beautifier for the C, C++, C++/CLI, Objective‑C, C# and Java programming languages"
 readme = "README.md"
 requires-python = ">= 3.7"
 keywords = ["astyle"]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `astyle-3.3.1/tests/astyle_test.py` & `astyle-3.3b3/tests/astyle_test.py`

 * *Files identical despite different names*

### Comparing `astyle-3.3.1/PKG-INFO` & `astyle-3.3b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astyle
-Version: 3.3.1
+Version: 3.3b3
 Summary: Artistic Style is a source code indenter, formatter, and beautifier for the C, C++, C++/CLI, Objective‑C, C# and Java programming languages
 Keywords: astyle
 Author-Email: Wu Zhenyu <wuzhenyu@ustc.edu>
 License: GPL v3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -97,34 +97,28 @@
 ### pre-commit
 
 `.pre-commit-config.yaml`:
 
 ```yaml
 repos:
   - repo: https://github.com/Freed-Wu/astyle-wheel
-    rev: 3.3.1
+    rev: 3.3-beta3
     hooks:
       - id: astyle
 ```
 
 ```shell
 pre-commit install
 git commit
 ```
 
 ## Similar Projects
 
 ### pre-commit hooks
 
 - [mirrors-clang-format](https://github.com/pre-commit/mirrors-clang-format)
-- [astyle_precommit_hook](https://github.com/mellowcandle/astyle_precommit_hook):
-  it uses git hook, not pre-commit, which make it cannot use many hooks at the
-  same time.
-- [pyastyle](https://github.com/timonwong/pyastyle): stop maintaining.
-- [astyle_py](https://github.com/igrr/astyle_py): it uses wasm, not native
-  binary programs like this project.
 
 ### Python distributions
 
 - [clang-format-wheel](https://github.com/ssciwr/clang-format-wheel)
 - [cmake-python-distributions](https://github.com/scikit-build/cmake-python-distributions)
 - [ninja-python-distributions](https://github.com/scikit-build/ninja-python-distributions)
```


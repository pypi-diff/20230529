# Comparing `tmp/jaraco.functools-3.6.0.tar.gz` & `tmp/jaraco.functools-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaraco.functools-3.6.0.tar", last modified: Mon Feb 20 00:17:24 2023, max compression
+gzip compressed data, was "jaraco.functools-3.7.0.tar", last modified: Mon May 29 08:12:10 2023, max compression
```

## Comparing `jaraco.functools-3.6.0.tar` & `jaraco.functools-3.7.0.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:17:24.859861 jaraco.functools-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:17:24.859861 jaraco.functools-3.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:17:24.859861 jaraco.functools-3.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-02-20 00:17:24.859861 jaraco.functools-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:17:24.859861 jaraco.functools-3.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:17:24.859861 jaraco.functools-3.6.0/jaraco/
--rw-r--r--   0 runner    (1001) docker     (123)    15035 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/jaraco/functools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 00:17:24.859861 jaraco.functools-3.6.0/jaraco.functools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-02-20 00:17:24.000000 jaraco.functools-3.6.0/jaraco.functools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-02-20 00:17:24.000000 jaraco.functools-3.6.0/jaraco.functools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 00:17:24.000000 jaraco.functools-3.6.0/jaraco.functools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-20 00:17:24.000000 jaraco.functools-3.6.0/jaraco.functools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-20 00:17:24.000000 jaraco.functools-3.6.0/jaraco.functools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-20 00:17:24.859861 jaraco.functools-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/test_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)      821 2023-02-20 00:16:51.000000 jaraco.functools-3.6.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.598692 jaraco.functools-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.590692 jaraco.functools-3.7.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.590692 jaraco.functools-3.7.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 08:12:10.598692 jaraco.functools-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.590692 jaraco.functools-3.7.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.594692 jaraco.functools-3.7.0/jaraco/
+-rw-r--r--   0 runner    (1001) docker     (123)    15950 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/jaraco/functools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:12:10.598692 jaraco.functools-3.7.0/jaraco.functools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 08:12:10.000000 jaraco.functools-3.7.0/jaraco.functools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-29 08:12:10.000000 jaraco.functools-3.7.0/jaraco.functools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:12:10.000000 jaraco.functools-3.7.0/jaraco.functools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-05-29 08:12:10.000000 jaraco.functools-3.7.0/jaraco.functools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 08:12:10.000000 jaraco.functools-3.7.0/jaraco.functools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 08:12:10.598692 jaraco.functools-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7238 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/test_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      821 2023-05-29 08:11:36.000000 jaraco.functools-3.7.0/tox.ini
```

### Comparing `jaraco.functools-3.6.0/.github/workflows/main.yml` & `jaraco.functools-3.7.0/.github/workflows/main.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 name: tests
 
 on: [push, pull_request]
 
+permissions:
+  contents: read
+
 env:
   # Environment variables to support color support (jaraco/skeleton#66):
   # Request colored output from CLI tools supporting it. Different tools
   # interpret the value differently. For some, just being set is sufficient.
   # For others, it must be a non-zero integer. For yet others, being set
   # to a non-empty value is sufficient. For tox, it must be one of
   # <blank>, 0, 1, false, no, off, on, true, yes. The only enabling value
@@ -100,14 +103,16 @@
     steps:
     - name: Decide whether the needed jobs succeeded or failed
       uses: re-actors/alls-green@release/v1
       with:
         jobs: ${{ toJSON(needs) }}
 
   release:
+    permissions:
+      contents: write
     needs:
     - check
     if: github.event_name == 'push' && contains(github.ref, 'refs/tags/')
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
```

### Comparing `jaraco.functools-3.6.0/CHANGES.rst` & `jaraco.functools-3.7.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+v3.7.0
+======
+
+Added ``bypass_unless`` and ``bypass_when`` and ``identity``.
+
 v3.6.0
 ======
 
 #21: Renamed ``call_aside`` to ``invoke``, deprecating ``call_aside``.
 
 v3.5.2
 ======
```

### Comparing `jaraco.functools-3.6.0/LICENSE` & `jaraco.functools-3.7.0/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `jaraco.functools-3.6.0/PKG-INFO` & `jaraco.functools-3.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.functools
-Version: 3.6.0
+Version: 3.7.0
 Summary: Functools like those found in stdlib
 Home-page: https://github.com/jaraco/jaraco.functools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.functools-3.6.0/README.rst` & `jaraco.functools-3.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.6.0/conftest.py` & `jaraco.functools-3.7.0/conftest.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.6.0/docs/conf.py` & `jaraco.functools-3.7.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.6.0/jaraco/functools.py` & `jaraco.functools-3.7.0/jaraco/functools.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
+import collections
 import functools
-import time
 import inspect
-import collections
-import types
 import itertools
+import operator
+import time
+import types
 import warnings
 
 import more_itertools
 
 from typing import Callable, TypeVar
 
 
@@ -550,7 +551,55 @@
                     return eval(use)
                 except TypeError:
                     return replace
 
         return wrapper
 
     return decorate
+
+
+def identity(x):
+    return x
+
+
+def bypass_when(check, *, _op=identity):
+    """
+    Decorate a function to return its parameter when ``check``.
+
+    >>> bypassed = []  # False
+
+    >>> @bypass_when(bypassed)
+    ... def double(x):
+    ...     return x * 2
+    >>> double(2)
+    4
+    >>> bypassed[:] = [object()]  # True
+    >>> double(2)
+    2
+    """
+
+    def decorate(func):
+        @functools.wraps(func)
+        def wrapper(param):
+            return param if _op(check) else func(param)
+
+        return wrapper
+
+    return decorate
+
+
+def bypass_unless(check):
+    """
+    Decorate a function to return its parameter unless ``check``.
+
+    >>> enabled = [object()]  # True
+
+    >>> @bypass_unless(enabled)
+    ... def double(x):
+    ...     return x * 2
+    >>> double(2)
+    4
+    >>> del enabled[:]  # False
+    >>> double(2)
+    2
+    """
+    return bypass_when(check, _op=operator.not_)
```

### Comparing `jaraco.functools-3.6.0/jaraco.functools.egg-info/PKG-INFO` & `jaraco.functools-3.7.0/jaraco.functools.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaraco.functools
-Version: 3.6.0
+Version: 3.7.0
 Summary: Functools like those found in stdlib
 Home-page: https://github.com/jaraco/jaraco.functools
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `jaraco.functools-3.6.0/jaraco.functools.egg-info/SOURCES.txt` & `jaraco.functools-3.7.0/jaraco.functools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 .coveragerc
 .editorconfig
-.flake8
 .pre-commit-config.yaml
 .readthedocs.yaml
 CHANGES.rst
 LICENSE
 README.rst
 conftest.py
 mypy.ini
```

### Comparing `jaraco.functools-3.6.0/pytest.ini` & `jaraco.functools-3.7.0/pytest.ini`

 * *Files 23% similar despite different names*

```diff
@@ -3,30 +3,25 @@
 addopts=--doctest-modules --import-mode=importlib
 filterwarnings=
 	## upstream
 
 	# Ensure ResourceWarnings are emitted
 	default::ResourceWarning
 
-	# Suppress deprecation warning in flake8
-	ignore:SelectableGroups dict interface is deprecated::flake8
-
 	# shopkeep/pytest-black#55
 	ignore:<class 'pytest_black.BlackItem'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
 	ignore:The \(fspath. py.path.local\) argument to BlackItem is deprecated.:pytest.PytestDeprecationWarning
 	ignore:BlackItem is an Item subclass and should not be a collector:pytest.PytestWarning
 
-	# tholo/pytest-flake8#83
-	ignore:<class 'pytest_flake8.Flake8Item'> is not using a cooperative constructor:pytest.PytestDeprecationWarning
-	ignore:The \(fspath. py.path.local\) argument to Flake8Item is deprecated.:pytest.PytestDeprecationWarning
-	ignore:Flake8Item is an Item subclass and should not be a collector:pytest.PytestWarning
-
 	# shopkeep/pytest-black#67
 	ignore:'encoding' argument not specified::pytest_black
 
 	# realpython/pytest-mypy#152
 	ignore:'encoding' argument not specified::pytest_mypy
 
 	# python/cpython#100750
 	ignore:'encoding' argument not specified::platform
 
+	# pypa/build#615
+	ignore:'encoding' argument not specified::build.env
+
 	## end upstream
```

### Comparing `jaraco.functools-3.6.0/setup.cfg` & `jaraco.functools-3.7.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -26,23 +26,21 @@
 	docs*
 	tests*
 
 [options.extras_require]
 testing = 
 	pytest >= 6
 	pytest-checkdocs >= 2.4
-	pytest-flake8; \
-	python_version < "3.12"
-	flake8 < 5
 	pytest-black >= 0.3.7; \
 	python_implementation != "PyPy"
 	pytest-cov
 	pytest-mypy >= 0.9.1; \
 	python_implementation != "PyPy"
 	pytest-enabler >= 1.3
+	pytest-ruff
 	
 	jaraco.classes
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9
 	rst.linker >= 1.9
 	furo
```

### Comparing `jaraco.functools-3.6.0/test_functools.py` & `jaraco.functools-3.7.0/test_functools.py`

 * *Files identical despite different names*

### Comparing `jaraco.functools-3.6.0/tox.ini` & `jaraco.functools-3.7.0/tox.ini`

 * *Files identical despite different names*


# Comparing `tmp/solidago-0.0.1.tar.gz` & `tmp/solidago-0.0.2.tar.gz`

## Comparing `solidago-0.0.1.tar` & `solidago-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,10 @@
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 solidago-0.0.1/src/solidago/__init__.py
--rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 solidago-0.0.1/src/solidago/optimize.py
--rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 solidago-0.0.1/src/solidago/mehestan/primitives.py
--rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 solidago-0.0.1/tests/test_mehestan_primitives.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 solidago-0.0.1/.gitignore
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 solidago-0.0.1/README.md
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 solidago-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 solidago-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 solidago-0.0.2/src/solidago/__init__.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 solidago-0.0.2/src/solidago/__version__.py
+-rw-r--r--   0        0        0     4554 2020-02-02 00:00:00.000000 solidago-0.0.2/src/solidago/optimize.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 solidago-0.0.2/src/solidago/mehestan/__init__.py
+-rw-r--r--   0        0        0     3349 2020-02-02 00:00:00.000000 solidago-0.0.2/src/solidago/mehestan/primitives.py
+-rw-r--r--   0        0        0     3762 2020-02-02 00:00:00.000000 solidago-0.0.2/tests/test_mehestan_primitives.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 solidago-0.0.2/.gitignore
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 solidago-0.0.2/README.md
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 solidago-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 solidago-0.0.2/PKG-INFO
```

### Comparing `solidago-0.0.1/src/solidago/optimize.py` & `solidago-0.0.2/src/solidago/optimize.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.1/src/solidago/mehestan/primitives.py` & `solidago-0.0.2/src/solidago/mehestan/primitives.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.1/tests/test_mehestan_primitives.py` & `solidago-0.0.2/tests/test_mehestan_primitives.py`

 * *Files identical despite different names*

### Comparing `solidago-0.0.1/pyproject.toml` & `solidago-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [project]
 name = "solidago"
 authors = [
   { name="Tournesol Association", email="hello@tournesol.app" },
 ]
-description = "Algorithms for the Tournesol platform"
+description = "Algorithms for Secure Algorithmic Governance"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: GNU Affero General Public License v3",
     "Operating System :: OS Independent",
 ]
@@ -29,14 +29,14 @@
 
 [project.optional-dependencies]
 test = [
     "pytest >=7.1.3,<8.0.0",
 ]
 
 [tool.hatch.version]
-path = "src/solidago/__init__.py"
+path = "src/solidago/__version__.py"
 
 [tool.pytest.ini_options]
 filterwarnings = [
     # Will be removed in Numba 0.58. See https://github.com/numba/numba/issues/8936
     "ignore:Use of isinstance():numba.NumbaExperimentalFeatureWarning",
 ]
```


# Comparing `tmp/keycloak-utils-0.0.1.tar.gz` & `tmp/keycloak-utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keycloak-utils-0.0.1.tar", last modified: Mon May 29 09:01:21 2023, max compression
+gzip compressed data, was "keycloak-utils-0.2.0.tar", last modified: Mon May 29 09:55:45 2023, max compression
```

## Comparing `keycloak-utils-0.0.1.tar` & `keycloak-utils-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:21.867547 keycloak-utils-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-29 09:01:21.867547 keycloak-utils-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:01:21.867547 keycloak-utils-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:21.863547 keycloak-utils-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:21.863547 keycloak-utils-0.0.1/src/keycloak_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:21.867547 keycloak-utils-0.0.1/src/keycloak_utils/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/authentication/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/authentication/rest_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:21.867547 keycloak-utils-0.0.1/src/keycloak_utils/backend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/backend/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/backend/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:21.867547 keycloak-utils-0.0.1/src/keycloak_utils/manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/manager/base.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/manager/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/manager/rest_framework.py
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:21.867547 keycloak-utils-0.0.1/src/keycloak_utils/verifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/verifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/verifier/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/verifier/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-29 09:01:09.000000 keycloak-utils-0.0.1/src/keycloak_utils/verifier/rest_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:01:21.863547 keycloak-utils-0.0.1/src/keycloak_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-05-29 09:01:21.000000 keycloak-utils-0.0.1/src/keycloak_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-29 09:01:21.000000 keycloak-utils-0.0.1/src/keycloak_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:01:21.000000 keycloak-utils-0.0.1/src/keycloak_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-29 09:01:21.000000 keycloak-utils-0.0.1/src/keycloak_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 09:01:21.000000 keycloak-utils-0.0.1/src/keycloak_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:45.280621 keycloak-utils-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-29 09:55:45.280621 keycloak-utils-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:55:45.280621 keycloak-utils-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:45.276621 keycloak-utils-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:45.280621 keycloak-utils-0.2.0/src/keycloak_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:45.280621 keycloak-utils-0.2.0/src/keycloak_utils/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/authentication/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/authentication/rest_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:45.280621 keycloak-utils-0.2.0/src/keycloak_utils/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/backend/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/backend/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:45.280621 keycloak-utils-0.2.0/src/keycloak_utils/manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/manager/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/manager/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/manager/rest_framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:45.280621 keycloak-utils-0.2.0/src/keycloak_utils/verifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/verifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/verifier/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/verifier/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-29 09:55:34.000000 keycloak-utils-0.2.0/src/keycloak_utils/verifier/rest_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:55:45.280621 keycloak-utils-0.2.0/src/keycloak_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-29 09:55:45.000000 keycloak-utils-0.2.0/src/keycloak_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-29 09:55:45.000000 keycloak-utils-0.2.0/src/keycloak_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:55:45.000000 keycloak-utils-0.2.0/src/keycloak_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-29 09:55:45.000000 keycloak-utils-0.2.0/src/keycloak_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 09:55:45.000000 keycloak-utils-0.2.0/src/keycloak_utils.egg-info/top_level.txt
```

### Comparing `keycloak-utils-0.0.1/PKG-INFO` & `keycloak-utils-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-utils
-Version: 0.0.1
+Version: 0.2.0
 Summary: Helper classes for keycloak authentication in Django and FastAPI
 Author-email: Jerin Peter George <jerinpetergeorge@gmail.com>
 Project-URL: Homepage, https://github.com/jerinpetergeorge/keycloak-auth-utils
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -117,7 +117,16 @@
 ```bash
 # Install the dependencies
 pip install .[test]
 
 # Run tests
 python -m pytest
 ```
+
+## Release
+```base
+# do a dry-run first -
+bump2version --dry-run --verbose [major|minor|patch]
+
+# if everything looks good, run the following command to release
+bump2version --verbose [major|minor|patch]
+```
```

### Comparing `keycloak-utils-0.0.1/README.md` & `keycloak-utils-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -91,7 +91,16 @@
 ```bash
 # Install the dependencies
 pip install .[test]
 
 # Run tests
 python -m pytest
 ```
+
+## Release
+```base
+# do a dry-run first -
+bump2version --dry-run --verbose [major|minor|patch]
+
+# if everything looks good, run the following command to release
+bump2version --verbose [major|minor|patch]
+```
```

### Comparing `keycloak-utils-0.0.1/pyproject.toml` & `keycloak-utils-0.2.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "keycloak-utils"
-version = "0.0.1"
+version = "0.2.0"
 authors = [
     { name = "Jerin Peter George", email = "jerinpetergeorge@gmail.com" },
 ]
 description = "Helper classes for keycloak authentication in Django and FastAPI"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -58,13 +58,13 @@
 lint-and-formatting = [
     "black",
     "flake8",
     "flake8-print",
     "isort",
     "pre-commit",
 ]
-dev = ["keycloak-utils[test, lint-and-formatting]"]
+dev = ["keycloak-utils[test, lint-and-formatting]", "bump2version~=1.0.1"]
 
 [tool.pytest.ini_options]
 DJANGO_SETTINGS_MODULE = "tests.test_rest_framework.settings"
 testpaths = ["tests"]
 markers = ["django_db"]
```

### Comparing `keycloak-utils-0.0.1/src/keycloak_utils/authentication/fastapi.py` & `keycloak-utils-0.2.0/src/keycloak_utils/authentication/fastapi.py`

 * *Files identical despite different names*

### Comparing `keycloak-utils-0.0.1/src/keycloak_utils/authentication/rest_framework.py` & `keycloak-utils-0.2.0/src/keycloak_utils/authentication/rest_framework.py`

 * *Files identical despite different names*

### Comparing `keycloak-utils-0.0.1/src/keycloak_utils/backend/base.py` & `keycloak-utils-0.2.0/src/keycloak_utils/backend/base.py`

 * *Files identical despite different names*

### Comparing `keycloak-utils-0.0.1/src/keycloak_utils/errors.py` & `keycloak-utils-0.2.0/src/keycloak_utils/errors.py`

 * *Files identical despite different names*

### Comparing `keycloak-utils-0.0.1/src/keycloak_utils/manager/base.py` & `keycloak-utils-0.2.0/src/keycloak_utils/manager/base.py`

 * *Files identical despite different names*

### Comparing `keycloak-utils-0.0.1/src/keycloak_utils/verifier/base.py` & `keycloak-utils-0.2.0/src/keycloak_utils/verifier/base.py`

 * *Files identical despite different names*

### Comparing `keycloak-utils-0.0.1/src/keycloak_utils.egg-info/PKG-INFO` & `keycloak-utils-0.2.0/src/keycloak_utils.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keycloak-utils
-Version: 0.0.1
+Version: 0.2.0
 Summary: Helper classes for keycloak authentication in Django and FastAPI
 Author-email: Jerin Peter George <jerinpetergeorge@gmail.com>
 Project-URL: Homepage, https://github.com/jerinpetergeorge/keycloak-auth-utils
 Classifier: Environment :: Web Environment
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -117,7 +117,16 @@
 ```bash
 # Install the dependencies
 pip install .[test]
 
 # Run tests
 python -m pytest
 ```
+
+## Release
+```base
+# do a dry-run first -
+bump2version --dry-run --verbose [major|minor|patch]
+
+# if everything looks good, run the following command to release
+bump2version --verbose [major|minor|patch]
+```
```

### Comparing `keycloak-utils-0.0.1/src/keycloak_utils.egg-info/SOURCES.txt` & `keycloak-utils-0.2.0/src/keycloak_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*


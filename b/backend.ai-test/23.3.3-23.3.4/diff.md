# Comparing `tmp/backend.ai-test-23.3.3.tar.gz` & `tmp/backend.ai-test-23.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-test-23.3.3.tar", last modified: Thu May 25 17:30:46 2023, max compression
+gzip compressed data, was "backend.ai-test-23.3.4.tar", last modified: Mon May 29 10:42:35 2023, max compression
```

## Comparing `backend.ai-test-23.3.3.tar` & `backend.ai-test-23.3.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.197153 backend.ai-test-23.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:45.000000 backend.ai-test-23.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-25 17:30:46.193153 backend.ai-test-23.3.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.193153 backend.ai-test-23.3.3/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.193153 backend.ai-test-23.3.3/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.193153 backend.ai-test-23.3.3/ai/backend/test/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:45.000000 backend.ai-test-23.3.3/ai/backend/test/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 17:30:45.000000 backend.ai-test-23.3.3/ai/backend/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.193153 backend.ai-test-23.3.3/ai/backend/test/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:45.000000 backend.ai-test-23.3.3/ai/backend/test/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-25 17:30:45.000000 backend.ai-test-23.3.3/ai/backend/test/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-25 17:30:45.000000 backend.ai-test-23.3.3/ai/backend/test/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-25 17:30:45.000000 backend.ai-test-23.3.3/ai/backend/test/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:45.000000 backend.ai-test-23.3.3/ai/backend/test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.193153 backend.ai-test-23.3.3/backend.ai_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-25 17:30:46.000000 backend.ai-test-23.3.3/backend.ai_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-25 17:30:46.000000 backend.ai-test-23.3.3/backend.ai_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-test-23.3.3/backend.ai_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-25 17:30:46.000000 backend.ai-test-23.3.3/backend.ai_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-test-23.3.3/backend.ai_test.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-test-23.3.3/backend.ai_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 17:30:46.000000 backend.ai-test-23.3.3/backend.ai_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:46.000000 backend.ai-test-23.3.3/backend.ai_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:45.000000 backend.ai-test-23.3.3/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:46.197153 backend.ai-test-23.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-25 17:30:45.000000 backend.ai-test-23.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.582969 backend.ai-test-23.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-29 10:42:35.582969 backend.ai-test-23.3.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.582969 backend.ai-test-23.3.4/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.582969 backend.ai-test-23.3.4/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.582969 backend.ai-test-23.3.4/ai/backend/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/ai/backend/test/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/ai/backend/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.582969 backend.ai-test-23.3.4/ai/backend/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/ai/backend/test/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/ai/backend/test/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/ai/backend/test/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/ai/backend/test/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/ai/backend/test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.582969 backend.ai-test-23.3.4/backend.ai_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/backend.ai_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/backend.ai_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/backend.ai_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/backend.ai_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/backend.ai_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/backend.ai_test.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/backend.ai_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/backend.ai_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:42:35.582969 backend.ai-test-23.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-29 10:42:35.000000 backend.ai-test-23.3.4/setup.py
```

### Comparing `backend.ai-test-23.3.3/PKG-INFO` & `backend.ai-test-23.3.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 23.3.3
+Version: 23.3.4
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-test-23.3.3/ai/backend/test/cli/__main__.py` & `backend.ai-test-23.3.4/ai/backend/test/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.3/ai/backend/test/cli/utils.py` & `backend.ai-test-23.3.4/ai/backend/test/cli/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.3/backend.ai_test.egg-info/PKG-INFO` & `backend.ai-test-23.3.4/backend.ai_test.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 23.3.3
+Version: 23.3.4
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-test-23.3.3/backend.ai_test.egg-info/SOURCES.txt` & `backend.ai-test-23.3.4/backend.ai_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.3/backend_shim.py` & `backend.ai-test-23.3.4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.3/setup.py` & `backend.ai-test-23.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         ],
     },
     'install_requires': (
         'attrs>=20.3',
         'click>=7.1.2',
         'pytest-dependency>=0.5.1',
         'pytest>=7.3.1',
+        'types-click',
     ),
     'license': 'MIT',
     'long_description': """# Backend.AI Testing Toolkit
 
 Automated test suites to validate an installation and integration of clients and servers
 
 
@@ -64,11 +65,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.3
+    'version': """23.03.4
 """,
     'zip_safe': False,
 })
```


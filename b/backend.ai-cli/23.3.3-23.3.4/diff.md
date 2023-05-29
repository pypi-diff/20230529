# Comparing `tmp/backend.ai-cli-23.3.3.tar.gz` & `tmp/backend.ai-cli-23.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-cli-23.3.3.tar", last modified: Thu May 25 17:30:46 2023, max compression
+gzip compressed data, was "backend.ai-cli-23.3.4.tar", last modified: Mon May 29 10:42:35 2023, max compression
```

## Comparing `backend.ai-cli-23.3.3.tar` & `backend.ai-cli-23.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.733155 backend.ai-cli-23.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-25 17:30:46.729155 backend.ai-cli-23.3.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.729155 backend.ai-cli-23.3.3/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.729155 backend.ai-cli-23.3.3/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.729155 backend.ai-cli-23.3.3/ai/backend/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/ai/backend/cli/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/ai/backend/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/ai/backend/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/ai/backend/cli/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/ai/backend/cli/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/ai/backend/cli/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/ai/backend/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/ai/backend/cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/ai/backend/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.729155 backend.ai-cli-23.3.3/backend.ai_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/backend.ai_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/backend.ai_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/backend.ai_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/backend.ai_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/backend.ai_cli.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/backend.ai_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/backend.ai_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/backend.ai_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:46.733155 backend.ai-cli-23.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-25 17:30:46.000000 backend.ai-cli-23.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.938981 backend.ai-cli-23.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-29 10:42:35.938981 backend.ai-cli-23.3.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.934981 backend.ai-cli-23.3.4/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.934981 backend.ai-cli-23.3.4/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.938981 backend.ai-cli-23.3.4/ai/backend/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/ai/backend/cli/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/ai/backend/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/ai/backend/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/ai/backend/cli/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/ai/backend/cli/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/ai/backend/cli/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/ai/backend/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/ai/backend/cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/ai/backend/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:35.938981 backend.ai-cli-23.3.4/backend.ai_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/backend.ai_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/backend.ai_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/backend.ai_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/backend.ai_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/backend.ai_cli.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/backend.ai_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/backend.ai_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/backend.ai_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:42:35.938981 backend.ai-cli-23.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2366 2023-05-29 10:42:35.000000 backend.ai-cli-23.3.4/setup.py
```

### Comparing `backend.ai-cli-23.3.3/PKG-INFO` & `backend.ai-cli-23.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-cli
-Version: 23.3.3
+Version: 23.3.4
 Summary: Backend.AI Command Line Interface Helper
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-cli-23.3.3/ai/backend/cli/extensions.py` & `backend.ai-cli-23.3.4/ai/backend/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.3/ai/backend/cli/interaction.py` & `backend.ai-cli-23.3.4/ai/backend/cli/interaction.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.3/ai/backend/cli/loader.py` & `backend.ai-cli-23.3.4/ai/backend/cli/loader.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.3/ai/backend/cli/main.py` & `backend.ai-cli-23.3.4/ai/backend/cli/main.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.3/backend.ai_cli.egg-info/PKG-INFO` & `backend.ai-cli-23.3.4/backend.ai_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-cli
-Version: 23.3.3
+Version: 23.3.4
 Summary: Backend.AI Command Line Interface Helper
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-cli-23.3.3/backend.ai_cli.egg-info/SOURCES.txt` & `backend.ai-cli-23.3.4/backend.ai_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.3/backend_shim.py` & `backend.ai-cli-23.3.4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.3/setup.py` & `backend.ai-cli-23.3.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,17 +23,18 @@
     'entry_points': {
         'console_scripts': [
             'backend.ai = ai.backend.cli.__main__:main',
         ],
     },
     'install_requires': (
         'attrs>=20.3',
-        """backend.ai-plugin==23.03.3
+        """backend.ai-plugin==23.03.4
 """,
         'click>=7.1.2',
+        'types-click',
     ),
     'license': 'MIT',
     'long_description': """# backend.ai-cli
 
 Unified command-line interface for Backend.AI
 
 
@@ -71,11 +72,11 @@
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


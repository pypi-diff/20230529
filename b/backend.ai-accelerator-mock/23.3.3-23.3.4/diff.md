# Comparing `tmp/backend.ai-accelerator-mock-23.3.3.tar.gz` & `tmp/backend.ai-accelerator-mock-23.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-accelerator-mock-23.3.3.tar", last modified: Thu May 25 17:30:39 2023, max compression
+gzip compressed data, was "backend.ai-accelerator-mock-23.3.4.tar", last modified: Mon May 29 10:42:37 2023, max compression
```

## Comparing `backend.ai-accelerator-mock-23.3.3.tar` & `backend.ai-accelerator-mock-23.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.365121 backend.ai-accelerator-mock-23.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:38.000000 backend.ai-accelerator-mock-23.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-25 17:30:39.365121 backend.ai-accelerator-mock-23.3.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.361121 backend.ai-accelerator-mock-23.3.3/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.361121 backend.ai-accelerator-mock-23.3.3/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.361121 backend.ai-accelerator-mock-23.3.3/ai/backend/accelerator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.361121 backend.ai-accelerator-mock-23.3.3/ai/backend/accelerator/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:38.000000 backend.ai-accelerator-mock-23.3.3/ai/backend/accelerator/mock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 17:30:38.000000 backend.ai-accelerator-mock-23.3.3/ai/backend/accelerator/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-25 17:30:38.000000 backend.ai-accelerator-mock-23.3.3/ai/backend/accelerator/mock/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-05-25 17:30:38.000000 backend.ai-accelerator-mock-23.3.3/ai/backend/accelerator/mock/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-25 17:30:38.000000 backend.ai-accelerator-mock-23.3.3/ai/backend/accelerator/mock/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-25 17:30:38.000000 backend.ai-accelerator-mock-23.3.3/ai/backend/accelerator/mock/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:39.365121 backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-25 17:30:39.000000 backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 17:30:39.000000 backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:39.000000 backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-25 17:30:39.000000 backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:39.000000 backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:39.000000 backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-25 17:30:39.000000 backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:39.000000 backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:38.000000 backend.ai-accelerator-mock-23.3.3/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:39.365121 backend.ai-accelerator-mock-23.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-25 17:30:38.000000 backend.ai-accelerator-mock-23.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:37.295026 backend.ai-accelerator-mock-23.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 10:42:36.000000 backend.ai-accelerator-mock-23.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-29 10:42:37.295026 backend.ai-accelerator-mock-23.3.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:37.295026 backend.ai-accelerator-mock-23.3.4/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:37.295026 backend.ai-accelerator-mock-23.3.4/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:37.295026 backend.ai-accelerator-mock-23.3.4/ai/backend/accelerator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:37.295026 backend.ai-accelerator-mock-23.3.4/ai/backend/accelerator/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 10:42:36.000000 backend.ai-accelerator-mock-23.3.4/ai/backend/accelerator/mock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 10:42:36.000000 backend.ai-accelerator-mock-23.3.4/ai/backend/accelerator/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-29 10:42:36.000000 backend.ai-accelerator-mock-23.3.4/ai/backend/accelerator/mock/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-05-29 10:42:36.000000 backend.ai-accelerator-mock-23.3.4/ai/backend/accelerator/mock/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-29 10:42:36.000000 backend.ai-accelerator-mock-23.3.4/ai/backend/accelerator/mock/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-29 10:42:36.000000 backend.ai-accelerator-mock-23.3.4/ai/backend/accelerator/mock/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 10:42:37.295026 backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-29 10:42:37.000000 backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-29 10:42:37.000000 backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:37.000000 backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-29 10:42:37.000000 backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:37.000000 backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 10:42:37.000000 backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-29 10:42:37.000000 backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 10:42:37.000000 backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-29 10:42:36.000000 backend.ai-accelerator-mock-23.3.4/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 10:42:37.295026 backend.ai-accelerator-mock-23.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-05-29 10:42:36.000000 backend.ai-accelerator-mock-23.3.4/setup.py
```

### Comparing `backend.ai-accelerator-mock-23.3.3/PKG-INFO` & `backend.ai-accelerator-mock-23.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-mock
-Version: 23.3.3
+Version: 23.3.4
 Summary: Backend.AI Mockup Accelerator Plugin
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-accelerator-mock-23.3.3/ai/backend/accelerator/mock/plugin.py` & `backend.ai-accelerator-mock-23.3.4/ai/backend/accelerator/mock/plugin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.3/ai/backend/accelerator/mock/types.py` & `backend.ai-accelerator-mock-23.3.4/ai/backend/accelerator/mock/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/PKG-INFO` & `backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-mock
-Version: 23.3.3
+Version: 23.3.4
 Summary: Backend.AI Mockup Accelerator Plugin
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-accelerator-mock-23.3.3/backend.ai_accelerator_mock.egg-info/SOURCES.txt` & `backend.ai-accelerator-mock-23.3.4/backend.ai_accelerator_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.3/backend_shim.py` & `backend.ai-accelerator-mock-23.3.4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.3/setup.py` & `backend.ai-accelerator-mock-23.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,27 +23,27 @@
     'entry_points': {
         'backendai_accelerator_v21': [
             'mock = ai.backend.accelerator.mock.plugin:MockPlugin',
         ],
     },
     'install_requires': (
         'aiodocker~=0.21.0',
-        """backend.ai-agent==23.03.3
+        """backend.ai-agent==23.03.4
 """,
-        """backend.ai-cli==23.03.3
+        """backend.ai-cli==23.03.4
 """,
-        """backend.ai-common==23.03.3
+        """backend.ai-common==23.03.4
 """,
-        """backend.ai-kernel-binary==23.03.3
+        """backend.ai-kernel-binary==23.03.4
 """,
-        """backend.ai-kernel-helper==23.03.3
+        """backend.ai-kernel-helper==23.03.4
 """,
-        """backend.ai-kernel==23.03.3
+        """backend.ai-kernel==23.03.4
 """,
-        """backend.ai-plugin==23.03.3
+        """backend.ai-plugin==23.03.4
 """,
         'trafaret~=2.1',
     ),
     'license': 'LGPLv3',
     'long_description': """# backend.ai-accelerator-mock
 
 A mockup plugin for accelerators
@@ -75,11 +75,11 @@
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


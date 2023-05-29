# Comparing `tmp/backend.ai-accelerator-cuda-mock-23.3.0a3.tar.gz` & `tmp/backend.ai-accelerator-cuda-mock-23.3.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-accelerator-cuda-mock-23.3.0a3.tar", last modified: Wed Mar 15 08:12:33 2023, max compression
+gzip compressed data, was "backend.ai-accelerator-cuda-mock-23.3.0a4.tar", last modified: Thu Mar 16 02:53:03 2023, max compression
```

## Comparing `backend.ai-accelerator-cuda-mock-23.3.0a3.tar` & `backend.ai-accelerator-cuda-mock-23.3.0a4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 08:12:33.351809 backend.ai-accelerator-cuda-mock-23.3.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-15 08:12:33.351809 backend.ai-accelerator-cuda-mock-23.3.0a3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 08:12:33.351809 backend.ai-accelerator-cuda-mock-23.3.0a3/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 08:12:33.351809 backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 08:12:33.351809 backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/accelerator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 08:12:33.351809 backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/accelerator/cuda_mock/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/accelerator/cuda_mock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/accelerator/cuda_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/accelerator/cuda_mock/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/accelerator/cuda_mock/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/accelerator/cuda_mock/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/accelerator/cuda_mock/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 08:12:33.351809 backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 08:12:33.351809 backend.ai-accelerator-cuda-mock-23.3.0a3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-03-15 08:12:33.000000 backend.ai-accelerator-cuda-mock-23.3.0a3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.484292 backend.ai-accelerator-cuda-mock-23.3.0a4/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-16 02:53:03.484292 backend.ai-accelerator-cuda-mock-23.3.0a4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.480292 backend.ai-accelerator-cuda-mock-23.3.0a4/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.480292 backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.480292 backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/accelerator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.484292 backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/accelerator/cuda_mock/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/accelerator/cuda_mock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/accelerator/cuda_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/accelerator/cuda_mock/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29487 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/accelerator/cuda_mock/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/accelerator/cuda_mock/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/accelerator/cuda_mock/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 02:53:03.484292 backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-16 02:53:03.484292 backend.ai-accelerator-cuda-mock-23.3.0a4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-03-16 02:53:03.000000 backend.ai-accelerator-cuda-mock-23.3.0a4/setup.py
```

### Comparing `backend.ai-accelerator-cuda-mock-23.3.0a3/PKG-INFO` & `backend.ai-accelerator-cuda-mock-23.3.0a4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-cuda-mock
-Version: 23.3.0a3
+Version: 23.3.0a4
 Summary: Backend.AI Accelerator Plugin for CUDA (Mockup)
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/accelerator/cuda_mock/plugin.py` & `backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/accelerator/cuda_mock/plugin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-mock-23.3.0a3/ai/backend/accelerator/cuda_mock/types.py` & `backend.ai-accelerator-cuda-mock-23.3.0a4/ai/backend/accelerator/cuda_mock/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/PKG-INFO` & `backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-cuda-mock
-Version: 23.3.0a3
+Version: 23.3.0a4
 Summary: Backend.AI Accelerator Plugin for CUDA (Mockup)
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-accelerator-cuda-mock-23.3.0a3/backend.ai_accelerator_cuda_mock.egg-info/SOURCES.txt` & `backend.ai-accelerator-cuda-mock-23.3.0a4/backend.ai_accelerator_cuda_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-mock-23.3.0a3/backend_shim.py` & `backend.ai-accelerator-cuda-mock-23.3.0a4/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-cuda-mock-23.3.0a3/setup.py` & `backend.ai-accelerator-cuda-mock-23.3.0a4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,27 @@
     'entry_points': {
         'backendai_accelerator_v21': [
             'cuda_mock = ai.backend.accelerator.cuda_mock.plugin:CUDAPlugin',
         ],
     },
     'install_requires': (
         'aiodocker~=0.21.0',
-        """backend.ai-agent==23.03.0a3
+        """backend.ai-agent==23.03.0a4
 """,
-        """backend.ai-cli==23.03.0a3
+        """backend.ai-cli==23.03.0a4
 """,
-        """backend.ai-common==23.03.0a3
+        """backend.ai-common==23.03.0a4
 """,
-        """backend.ai-kernel-binary==23.03.0a3
+        """backend.ai-kernel-binary==23.03.0a4
 """,
-        """backend.ai-kernel-helper==23.03.0a3
+        """backend.ai-kernel-helper==23.03.0a4
 """,
-        """backend.ai-kernel==23.03.0a3
+        """backend.ai-kernel==23.03.0a4
 """,
-        """backend.ai-plugin==23.03.0a3
+        """backend.ai-plugin==23.03.0a4
 """,
         'trafaret~=2.1',
     ),
     'license': 'LGPLv3',
     'long_description': """# backend.ai-accelerator-cuda-mock
 
 A mockup plugin for CUDA accelerators
@@ -72,11 +72,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.0a3
+    'version': """23.03.0a4
 """,
     'zip_safe': False,
 })
```


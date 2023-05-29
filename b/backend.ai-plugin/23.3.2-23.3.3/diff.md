# Comparing `tmp/backend.ai-plugin-23.3.2.tar.gz` & `tmp/backend.ai-plugin-23.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-plugin-23.3.2.tar", last modified: Fri May  5 07:08:12 2023, max compression
+gzip compressed data, was "backend.ai-plugin-23.3.3.tar", last modified: Thu May 25 17:30:46 2023, max compression
```

## Comparing `backend.ai-plugin-23.3.2.tar` & `backend.ai-plugin-23.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.854858 backend.ai-plugin-23.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 07:08:12.854858 backend.ai-plugin-23.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.850859 backend.ai-plugin-23.3.2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.850859 backend.ai-plugin-23.3.2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.850859 backend.ai-plugin-23.3.2/ai/backend/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/ai/backend/plugin/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/ai/backend/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/ai/backend/plugin/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/ai/backend/plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.854858 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:12.854858 backend.ai-plugin-23.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.801155 backend.ai-plugin-23.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-25 17:30:46.797155 backend.ai-plugin-23.3.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.797155 backend.ai-plugin-23.3.3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.797155 backend.ai-plugin-23.3.3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.797155 backend.ai-plugin-23.3.3/ai/backend/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/ai/backend/plugin/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/ai/backend/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/ai/backend/plugin/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/ai/backend/plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:46.797155 backend.ai-plugin-23.3.3/backend.ai_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/backend.ai_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/backend.ai_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/backend.ai_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/backend.ai_plugin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/backend.ai_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/backend.ai_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:46.801155 backend.ai-plugin-23.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-25 17:30:46.000000 backend.ai-plugin-23.3.3/setup.py
```

### Comparing `backend.ai-plugin-23.3.2/PKG-INFO` & `backend.ai-plugin-23.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 Backend.AI Plugin Subsystem
 ===========================
```

### Comparing `backend.ai-plugin-23.3.2/ai/backend/plugin/entrypoint.py` & `backend.ai-plugin-23.3.3/ai/backend/plugin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/PKG-INFO` & `backend.ai-plugin-23.3.3/backend.ai_plugin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 Backend.AI Plugin Subsystem
 ===========================
```

### Comparing `backend.ai-plugin-23.3.2/backend_shim.py` & `backend.ai-plugin-23.3.3/backend_shim.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 build_wheel = True
 build_sdist = True
 wheel_config_settings = {
 }
 sdist_config_settings = {
 }
 
-os.makedirs(dist_dir, exist_ok=True)
+# Python 2.7 doesn't have the exist_ok arg on os.makedirs().
+try:
+    os.makedirs(dist_dir)
+except OSError as e:
+    if e.errno != errno.EEXIST:
+        raise
+
 wheel_path = backend.build_wheel(dist_dir, wheel_config_settings) if build_wheel else None
 sdist_path = backend.build_sdist(dist_dir, sdist_config_settings) if build_sdist else None
 
 if wheel_path:
     print("wheel: {wheel_path}".format(wheel_path=wheel_path))
 if sdist_path:
     print("sdist: {sdist_path}".format(sdist_path=sdist_path))
```

### Comparing `backend.ai-plugin-23.3.2/setup.py` & `backend.ai-plugin-23.3.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
         'Operating System :: POSIX :: Linux',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
         'Environment :: No Input/Output (Daemon)',
         'Topic :: Scientific/Engineering',
         'Topic :: Software Development',
         'Development Status :: 5 - Production/Stable',
+        'Programming Language :: Python :: 3.11',
         'License :: OSI Approved :: MIT License',
     ],
     'description': 'Backend.AI Plugin Subsystem',
     'install_requires': (
     ),
     'license': 'MIT',
     'long_description': """Backend.AI Plugin Subsystem
@@ -45,11 +46,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.2
+    'version': """23.03.3
 """,
     'zip_safe': False,
 })
```


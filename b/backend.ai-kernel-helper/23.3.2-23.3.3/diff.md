# Comparing `tmp/backend.ai-kernel-helper-23.3.2.tar.gz` & `tmp/backend.ai-kernel-helper-23.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-helper-23.3.2.tar", last modified: Fri May  5 07:08:12 2023, max compression
+gzip compressed data, was "backend.ai-kernel-helper-23.3.3.tar", last modified: Thu May 25 17:30:38 2023, max compression
```

## Comparing `backend.ai-kernel-helper-23.3.2.tar` & `backend.ai-kernel-helper-23.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.046856 backend.ai-kernel-helper-23.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-05 07:08:12.046856 backend.ai-kernel-helper-23.3.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.042856 backend.ai-kernel-helper-23.3.2/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.042856 backend.ai-kernel-helper-23.3.2/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.042856 backend.ai-kernel-helper-23.3.2/ai/backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/ai/backend/helpers/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/ai/backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/ai/backend/helpers/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.042856 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:12.046856 backend.ai-kernel-helper-23.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.165115 backend.ai-kernel-helper-23.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-25 17:30:37.000000 backend.ai-kernel-helper-23.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-25 17:30:38.165115 backend.ai-kernel-helper-23.3.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.161115 backend.ai-kernel-helper-23.3.3/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.161115 backend.ai-kernel-helper-23.3.3/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.165115 backend.ai-kernel-helper-23.3.3/ai/backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-25 17:30:37.000000 backend.ai-kernel-helper-23.3.3/ai/backend/helpers/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-25 17:30:37.000000 backend.ai-kernel-helper-23.3.3/ai/backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-25 17:30:37.000000 backend.ai-kernel-helper-23.3.3/ai/backend/helpers/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 17:30:38.165115 backend.ai-kernel-helper-23.3.3/backend.ai_kernel_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-25 17:30:38.000000 backend.ai-kernel-helper-23.3.3/backend.ai_kernel_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-25 17:30:38.000000 backend.ai-kernel-helper-23.3.3/backend.ai_kernel_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:38.000000 backend.ai-kernel-helper-23.3.3/backend.ai_kernel_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:38.000000 backend.ai-kernel-helper-23.3.3/backend.ai_kernel_helper.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 17:30:38.000000 backend.ai-kernel-helper-23.3.3/backend.ai_kernel_helper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 17:30:38.000000 backend.ai-kernel-helper-23.3.3/backend.ai_kernel_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-25 17:30:38.000000 backend.ai-kernel-helper-23.3.3/backend.ai_kernel_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-25 17:30:37.000000 backend.ai-kernel-helper-23.3.3/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 17:30:38.165115 backend.ai-kernel-helper-23.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-05-25 17:30:37.000000 backend.ai-kernel-helper-23.3.3/setup.py
```

### Comparing `backend.ai-kernel-helper-23.3.2/PKG-INFO` & `backend.ai-kernel-helper-23.3.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel-helper
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Kernel Runner Prebuilt Binaries Package
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,12 +12,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 # Backend.AI In-kernel Helper Package
```

### Comparing `backend.ai-kernel-helper-23.3.2/ai/backend/helpers/package.py` & `backend.ai-kernel-helper-23.3.3/ai/backend/helpers/package.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/PKG-INFO` & `backend.ai-kernel-helper-23.3.3/backend.ai_kernel_helper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel-helper
-Version: 23.3.2
+Version: 23.3.3
 Summary: Backend.AI Kernel Runner Prebuilt Binaries Package
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
@@ -12,12 +12,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.11,<3.12
 Description-Content-Type: text/markdown
 
 # Backend.AI In-kernel Helper Package
```

### Comparing `backend.ai-kernel-helper-23.3.2/backend_shim.py` & `backend.ai-kernel-helper-23.3.3/backend_shim.py`

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

### Comparing `backend.ai-kernel-helper-23.3.2/setup.py` & `backend.ai-kernel-helper-23.3.3/setup.py`

 * *Files 12% similar despite different names*

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
         'License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)',
     ],
     'description': 'Backend.AI Kernel Runner Prebuilt Binaries Package',
     'install_requires': (
         'types-pkg_resources',
     ),
     'license': 'LGPLv3',
@@ -39,11 +40,11 @@
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


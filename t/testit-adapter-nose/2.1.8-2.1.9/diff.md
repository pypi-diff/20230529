# Comparing `tmp/testit-adapter-nose-2.1.8.tar.gz` & `tmp/testit-adapter-nose-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-nose-2.1.8.tar", last modified: Fri May 12 08:34:55 2023, max compression
+gzip compressed data, was "testit-adapter-nose-2.1.9.tar", last modified: Fri May 26 08:37:02 2023, max compression
```

## Comparing `testit-adapter-nose-2.1.8.tar` & `testit-adapter-nose-2.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:55.148847 testit-adapter-nose-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-12 08:34:55.144847 testit-adapter-nose-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:34:55.148847 testit-adapter-nose-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:55.140847 testit-adapter-nose-2.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:55.144847 testit-adapter-nose-2.1.8/src/testit_adapter_nose/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-12 08:34:43.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:55.144847 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 08:34:55.000000 testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/src/testit_adapter_nose/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-05-26 08:36:51.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:02.459878 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10915 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 08:37:02.000000 testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/top_level.txt
```

### Comparing `testit-adapter-nose-2.1.8/PKG-INFO` & `testit-adapter-nose-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-nose
-Version: 2.1.8
+Version: 2.1.9
 Summary: Nose adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-nose-2.1.8/README.md` & `testit-adapter-nose-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.1.8/setup.py` & `testit-adapter-nose-2.1.9/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='testit-adapter-nose',
-    version='2.1.8',
+    version='2.1.9',
     description='Nose adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,14 +16,14 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_nose'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'nose2', 'testit-python-commons==2.1.8'],
+    install_requires=['attrs', 'nose2', 'testit-python-commons==2.1.9'],
     entry_points={
             'nose.plugins.0.10': [
                 'testit_adapter_nose = testit_adapter_nose.plugin:TmsPlugin',
             ]
     }
 )
```

### Comparing `testit-adapter-nose-2.1.8/src/testit_adapter_nose/listener.py` & `testit-adapter-nose-2.1.9/src/testit_adapter_nose/listener.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import testit_python_commons.services as adapter
 from testit_python_commons.services import AdapterManager
 from testit_python_commons.step import Step
 from .utils import (
     form_test,
-    get_outcome
+    get_outcome,
+    convert_executable_test_to_test_result_model
 )
 
 
 class AdapterListener(object):
     __executable_test = None
 
     def __init__(self, adapter_manager: AdapterManager):
@@ -33,15 +34,16 @@
 
     def stop_test(self):
         test_steps, test_results_steps = Step.get_steps_data()
 
         self.__executable_test['steps'] = test_steps
         self.__executable_test['stepResults'] = test_results_steps
 
-        self.__adapter_manager.write_test(self.__executable_test)
+        self.__adapter_manager.write_test(
+            convert_executable_test_to_test_result_model(self.__executable_test))
         self.__executable_test = None
 
     @adapter.hookimpl
     def add_link(self, link):
         if self.__executable_test:
             self.__executable_test['resultLinks'].append(link)
```

### Comparing `testit-adapter-nose-2.1.8/src/testit_adapter_nose/plugin.py` & `testit-adapter-nose-2.1.9/src/testit_adapter_nose/plugin.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-nose-2.1.8/src/testit_adapter_nose.egg-info/PKG-INFO` & `testit-adapter-nose-2.1.9/src/testit_adapter_nose.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-nose
-Version: 2.1.8
+Version: 2.1.9
 Summary: Nose adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```


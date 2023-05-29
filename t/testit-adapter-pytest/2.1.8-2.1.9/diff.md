# Comparing `tmp/testit-adapter-pytest-2.1.8.tar.gz` & `tmp/testit-adapter-pytest-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-pytest-2.1.8.tar", last modified: Fri May 12 08:34:58 2023, max compression
+gzip compressed data, was "testit-adapter-pytest-2.1.9.tar", last modified: Fri May 26 08:37:14 2023, max compression
```

## Comparing `testit-adapter-pytest-2.1.8.tar` & `testit-adapter-pytest-2.1.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14040 2023-05-12 08:34:44.000000 testit-adapter-pytest-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-12 08:34:44.000000 testit-adapter-pytest-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:44.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-05-12 08:34:44.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/listener.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-12 08:34:44.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:58.212296 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 08:34:58.000000 testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:14.716844 testit-adapter-pytest-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-05-26 08:37:14.716844 testit-adapter-pytest-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14034 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:14.716844 testit-adapter-pytest-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:14.708845 testit-adapter-pytest-2.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:14.712844 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/listener.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11524 2023-05-26 08:36:59.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:14.712844 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14570 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 08:37:14.000000 testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/top_level.txt
```

### Comparing `testit-adapter-pytest-2.1.8/PKG-INFO` & `testit-adapter-pytest-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 2.1.8
+Version: 2.1.9
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -21,15 +21,15 @@
 
 ### Installation
 
 ```
 pip install testit-adapter-pytest
 ```
 
-## Usage
+##
 
 ### Configuration
 
 | Description                                                                                                                                                                                                                                                                                                                                                                            | Property                   | Environment variable              | CLI argument                  |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|-----------------------------------|-------------------------------|
 | Location of the TMS instance                                                                                                                                                                                                                                                                                                                                                           | url                        | TMS_URL                           | tmsUrl                        |
 | API secret key [How to getting API secret key?](https://github.com/testit-tms/.github/tree/main/configuration#privatetoken)                                                                                                                                                                                                                                                            | privateToken               | TMS_PRIVATE_TOKEN                 | tmsPrivateToken               |
```

### Comparing `testit-adapter-pytest-2.1.8/README.md` & `testit-adapter-pytest-2.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 ### Installation
 
 ```
 pip install testit-adapter-pytest
 ```
 
-## Usage
+##
 
 ### Configuration
 
 | Description                                                                                                                                                                                                                                                                                                                                                                            | Property                   | Environment variable              | CLI argument                  |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|-----------------------------------|-------------------------------|
 | Location of the TMS instance                                                                                                                                                                                                                                                                                                                                                           | url                        | TMS_URL                           | tmsUrl                        |
 | API secret key [How to getting API secret key?](https://github.com/testit-tms/.github/tree/main/configuration#privatetoken)                                                                                                                                                                                                                                                            | privateToken               | TMS_PRIVATE_TOKEN                 | tmsPrivateToken               |
```

### Comparing `testit-adapter-pytest-2.1.8/setup.py` & `testit-adapter-pytest-2.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-pytest',
-    version='2.1.8',
+    version='2.1.9',
     description='Pytest adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,10 +16,10 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_pytest'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['pytest', 'pytest-xdist', 'testit-python-commons==2.1.8'],
+    install_requires=['pytest', 'pytest-xdist', 'testit-python-commons==2.1.9'],
     entry_points={'pytest11': ['testit_adapter_pytest = testit_adapter_pytest.plugin']}
 )
```

### Comparing `testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/listener.py` & `testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,19 @@
 
 from packaging import version
 
 import pytest
 
 import testit_python_commons.services as adapter
 from testit_python_commons.models.outcome_type import OutcomeType
-from testit_python_commons.services import AdapterManager, Utils
+from testit_python_commons.services import AdapterManager
 from testit_python_commons.step import Step
 
+import testit_adapter_pytest.utils as utils
+
 STATUS = {
     'passed': OutcomeType.PASSED,
     'failed': OutcomeType.FAILED,
     'skipped': OutcomeType.SKIPPED
 }
 
 
@@ -64,63 +66,64 @@
             if 'pytest-check' == dist.project_name:
                 self.__pytest_check_info = dist
                 break
 
         resolved_autotests = self.__adapter_manager.get_autotests_for_launch()
 
         for item in items:
-            if not hasattr(item.function, 'test_external_id'):
-                item.test_external_id = Utils.get_hash(item.nodeid + item.function.__name__)
-
             if hasattr(item.function, 'test_external_id'):
-                if item.own_markers:
-                    for mark in item.own_markers:
-                        if mark.name == 'parametrize':
-                            if not hasattr(item, 'array_parametrize_mark_id'):
-                                item.array_parametrize_mark_id = []
-                            item.array_parametrize_mark_id.append(
-                                item.own_markers.index(mark))
-
-                params = Utils.get_params(item)
-                item.test_external_id = Utils.param_attribute_collector(
-                    item.function.test_external_id,
-                    params)
-
-                item.index = index
-                item_id = items.index(item)
-                index = index + 1 if len(items) > item_id + 1 and items[item_id + 1].originalname == item.originalname \
-                    else 0
-
-                if resolved_autotests \
-                        and item.test_external_id in resolved_autotests:
-                    selected_items.append(item)
+                item.test_external_id = item.function.test_external_id
+            else:
+                item.test_external_id = utils.get_hash(item.nodeid + item.function.__name__)
+
+            if item.own_markers:
+                for mark in item.own_markers:
+                    if mark.name == 'parametrize':
+                        if not hasattr(item, 'array_parametrize_mark_id'):
+                            item.array_parametrize_mark_id = []
+                        item.array_parametrize_mark_id.append(
+                            item.own_markers.index(mark))
+
+            params = utils.get_params(item)
+            item.test_external_id = utils.param_attribute_collector(
+                item.test_external_id,
+                params)
+
+            item.index = index
+            item_id = items.index(item)
+            index = index + 1 if len(items) > item_id + 1 and items[item_id + 1].originalname == item.originalname \
+                else 0
+
+            if resolved_autotests \
+                    and item.test_external_id in resolved_autotests:
+                selected_items.append(item)
         if resolved_autotests:
             if not selected_items:
                 print('The specified tests were not found!')
                 raise SystemExit
 
             config.hook.pytest_deselected(items=deselected_items)
             items[:] = selected_items
 
     @pytest.hookimpl
     def pytest_runtest_protocol(self, item):
         if not hasattr(item.function, 'test_external_id'):
-            item.test_external_id = Utils.get_hash(item.nodeid + item.function.__name__)
+            item.test_external_id = utils.get_hash(item.nodeid + item.function.__name__)
 
         if not hasattr(item.function, 'test_displayname'):
             item.test_displayname = item.function.__doc__ if \
                 item.function.__doc__ else item.function.__name__
         else:
-            params = Utils.get_params(item)
+            params = utils.get_params(item)
 
-            item.test_displayname = Utils.param_attribute_collector(
+            item.test_displayname = utils.param_attribute_collector(
                 item.function.test_displayname,
                 params)
 
-        self.__executable_test = Utils.form_test(item)
+        self.__executable_test = utils.form_test(item)
 
     @pytest.hookimpl(hookwrapper=True)
     def pytest_fixture_setup(self, fixturedef):
         yield
         if self.__executable_test:
             steps_data, results_steps_data = Step.get_steps_data()
 
@@ -171,15 +174,16 @@
             self.__executable_test['duration'] += report.duration * 1000
 
     @pytest.hookimpl
     def pytest_runtest_logfinish(self):
         if not self.__executable_test:
             return
 
-        self.__adapter_manager.write_test(self.__executable_test)
+        self.__adapter_manager.write_test(
+            utils.convert_executable_test_to_test_result_model(self.__executable_test))
 
     @adapter.hookimpl
     def add_link(self, link):
         if self.__executable_test:
             self.__executable_test['resultLinks'].append(link)
 
     @adapter.hookimpl
```

### Comparing `testit-adapter-pytest-2.1.8/src/testit_adapter_pytest/plugin.py` & `testit-adapter-pytest-2.1.9/src/testit_adapter_pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-pytest-2.1.8/src/testit_adapter_pytest.egg-info/PKG-INFO` & `testit-adapter-pytest-2.1.9/src/testit_adapter_pytest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-pytest
-Version: 2.1.8
+Version: 2.1.9
 Summary: Pytest adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -21,15 +21,15 @@
 
 ### Installation
 
 ```
 pip install testit-adapter-pytest
 ```
 
-## Usage
+##
 
 ### Configuration
 
 | Description                                                                                                                                                                                                                                                                                                                                                                            | Property                   | Environment variable              | CLI argument                  |
 |----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|-----------------------------------|-------------------------------|
 | Location of the TMS instance                                                                                                                                                                                                                                                                                                                                                           | url                        | TMS_URL                           | tmsUrl                        |
 | API secret key [How to getting API secret key?](https://github.com/testit-tms/.github/tree/main/configuration#privatetoken)                                                                                                                                                                                                                                                            | privateToken               | TMS_PRIVATE_TOKEN                 | tmsPrivateToken               |
```


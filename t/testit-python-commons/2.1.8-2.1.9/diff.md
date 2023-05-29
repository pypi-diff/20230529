# Comparing `tmp/testit-python-commons-2.1.8.tar.gz` & `tmp/testit-python-commons-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-python-commons-2.1.8.tar", last modified: Fri May 12 08:34:59 2023, max compression
+gzip compressed data, was "testit-python-commons-2.1.9.tar", last modified: Fri May 26 08:37:04 2023, max compression
```

## Comparing `testit-python-commons-2.1.8.tar` & `testit-python-commons-2.1.9.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:59.087036 testit-python-commons-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-12 08:34:59.087036 testit-python-commons-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:34:59.087036 testit-python-commons-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:59.079036 testit-python-commons-2.1.8/src/
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:59.083036 testit-python-commons-2.1.8/src/testit_python_commons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/app_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:59.083036 testit-python-commons-2.1.8/src/testit_python_commons/client/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5160 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/client/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/client/client_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/client/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4554 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/dynamic_methods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:59.087036 testit-python-commons-2.1.8/src/testit_python_commons/models/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/models/adapter_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/models/link_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/models/outcome_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:59.087036 testit-python-commons-2.1.8/src/testit_python_commons/services/
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/services/adapter_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/services/adapter_manager_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/services/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/services/plugin_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    13082 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/services/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-12 08:34:44.000000 testit-python-commons-2.1.8/src/testit_python_commons/step.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:59.083036 testit-python-commons-2.1.8/src/testit_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-12 08:34:59.000000 testit-python-commons-2.1.8/src/testit_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-12 08:34:59.000000 testit-python-commons-2.1.8/src/testit_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:34:59.000000 testit-python-commons-2.1.8/src/testit_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-12 08:34:59.000000 testit-python-commons-2.1.8/src/testit_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-12 08:34:59.000000 testit-python-commons-2.1.8/src/testit_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/testit_python_commons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7576 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/app_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/testit_python_commons/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5312 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/client/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/client/client_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9291 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/client/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4572 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4054 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/dynamic_methods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/testit_python_commons/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/adapter_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/link_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/outcome_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/step_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/models/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/testit_python_commons/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/adapter_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/adapter_manager_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/plugin_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/services/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-26 08:36:53.000000 testit-python-commons-2.1.9/src/testit_python_commons/step.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:04.084880 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      728 2023-05-26 08:37:04.000000 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-05-26 08:37:04.000000 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:04.000000 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 08:37:04.000000 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-26 08:37:04.000000 testit-python-commons-2.1.9/src/testit_python_commons.egg-info/top_level.txt
```

### Comparing `testit-python-commons-2.1.8/PKG-INFO` & `testit-python-commons-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python commons for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-python-commons-2.1.8/setup.py` & `testit-python-commons-2.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-python-commons',
-    version='2.1.8',
+    version='2.1.9',
     description='Python commons for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
```

### Comparing `testit-python-commons-2.1.8/src/testit.py` & `testit-python-commons-2.1.9/src/testit.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons/app_properties.py` & `testit-python-commons-2.1.9/src/testit_python_commons/app_properties.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons/client/api_client.py` & `testit-python-commons-2.1.9/src/testit_python_commons/client/api_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from testit_api_client.models import (
     AttachmentPutModel,
     WorkItemIdModel
 )
 
 from testit_python_commons.client.client_configuration import ClientConfiguration
 from testit_python_commons.client.converter import Converter
+from testit_python_commons.models.test_result import TestResult
 from testit_python_commons.services.logger import adapter_logger
 
 
 class ApiClientWorker:
     def __init__(self, config: ClientConfiguration):
         client_config = Configuration(host=config.get_url())
 
@@ -54,46 +55,47 @@
         response = test_run_api.get_test_run_by_id(self.__config.get_test_run_id())
 
         return Converter.get_resolved_autotests_from_get_test_run_response(
             response,
             self.__config.get_configuration_id())
 
     @adapter_logger
-    def write_test(self, test_result: dict):
+    def write_test(self, test_result: TestResult):
         test_run_api = TestRunsApi(api_client=self.__api_client)
         autotest_api = AutoTestsApi(api_client=self.__api_client)
 
         autotest = autotest_api.get_all_auto_tests(project_id=self.__config.get_project_id(),
-                                                   external_id=test_result['externalID'])
+                                                   external_id=test_result.get_external_id())
 
         if autotest:
-            logging.debug(f'Autotest "{test_result["autoTestName"]}" was found')
+            logging.debug(f'Autotest "{test_result.get_autotest_name()}" was found')
 
             model = Converter.test_result_to_autotest_put_model(
                 test_result,
                 self.__config.get_project_id())
+            model.is_flaky = autotest[0]['is_flaky']
 
             autotest_api.update_auto_test(auto_test_put_model=model)
             autotest_global_id = autotest[0]['id']
 
-            logging.debug(f'Autotest "{test_result["autoTestName"]}" was updated')
+            logging.debug(f'Autotest "{test_result.get_autotest_name()}" was updated')
         else:
-            logging.debug(f'Autotest "{test_result["autoTestName"]}" was not found')
+            logging.debug(f'Autotest "{test_result.get_autotest_name()}" was not found')
 
             model = Converter.test_result_to_autotest_post_model(
                 test_result,
                 self.__config.get_project_id())
 
             autotest_response = autotest_api.create_auto_test(auto_test_post_model=model)
             autotest_global_id = autotest_response['id']
 
-            logging.debug(f'Autotest "{test_result["autoTestName"]}" was created')
+            logging.debug(f'Autotest "{test_result.get_autotest_name()}" was created')
 
         if autotest_global_id:
-            for work_item_id in test_result['workItemsID']:
+            for work_item_id in test_result.get_work_item_ids():
                 try:
                     autotest_api.link_auto_test_to_work_item(
                         autotest_global_id,
                         work_item_id_model=WorkItemIdModel(id=work_item_id))
 
                     logging.debug(f'Autotest "{test_result["autoTestName"]}" was linked with workItem "{work_item_id}"')
                 except Exception as exc:
@@ -103,15 +105,15 @@
             test_result,
             self.__config.get_configuration_id())
 
         test_run_api.set_auto_test_results_for_test_run(
             id=self.__config.get_test_run_id(),
             auto_test_results_for_test_run_model=[model])
 
-        logging.debug(f'Result of the autotest "{test_result["autoTestName"]}" was set '
+        logging.debug(f'Result of the autotest "{test_result.get_autotest_name()}" was set '
                       f'in the test run "{self.__config.get_test_run_id()}"')
 
     @adapter_logger
     def load_attachments(self, attach_paths: list or tuple):
         attachments_api = AttachmentsApi(api_client=self.__api_client)
 
         attachments = []
```

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons/client/client_configuration.py` & `testit-python-commons-2.1.9/src/testit_python_commons/client/client_configuration.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons/decorators.py` & `testit-python-commons-2.1.9/src/testit_python_commons/decorators.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 import types
 from functools import wraps
 
+from testit_python_commons.models.link import Link
 from testit_python_commons.services.logger import adapter_logger
 from testit_python_commons.services.utils import Utils
 
 
 def inner(function):
     @wraps(function)
     def wrapper(*args, **kwargs):
@@ -120,38 +121,46 @@
 
 @Utils.deprecated('Use "links" instead.')
 @adapter_logger
 def link(url: str, title: str = None, type: str = None, description: str = None):  # noqa: A002,VNE003
     def outer(function):
         if not hasattr(function, 'test_links'):
             function.test_links = []
-        function.test_links.append({'url': url, 'title': title, 'type': type, 'description': description})
+
+        function.test_links.append(
+            Link()
+                .set_url(url)
+                .set_title(title)
+                .set_link_type(type)
+                .set_description(description))
+
         return inner(function)
 
     return outer
 
 
 @adapter_logger
 def links(url: str = None, title: str = None, type: str = None,  # noqa: A002,VNE003
           description: str = None, links: list or tuple = None):
     def outer(function):
         if not hasattr(function, 'test_links'):
             function.test_links = []
 
         if url:
-            function.test_links.append({'url': url, 'title': title, 'type': type, 'description': description})
+            function.test_links.append(
+                Link()
+                    .set_url(url)
+                    .set_title(title)
+                    .set_link_type(type)
+                    .set_description(description))
         elif links and (isinstance(links, list) or isinstance(links, tuple)):
             for link in links:
                 if isinstance(link, dict) and 'url' in link:
                     function.test_links.append(
-                        {'url': link['url'],
-                         'title': link['title'] if 'title' in link else None,
-                         'type': link['type'] if 'type' in link else None,
-                         'description': link['description'] if 'description' in link else None}
-                    )
+                        Utils.convert_link_dict_to_link_model(link))
                 else:
                     logging.warning(f'Link ({link}) can\'t be processed!')
         else:
             logging.warning(f'Links for {function.__name__} can\'t be processed!\nPlease, set "url" or "links"!')
         return inner(function)
 
     return outer
```

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons/dynamic_methods.py` & `testit-python-commons-2.1.9/src/testit_python_commons/dynamic_methods.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,49 +1,46 @@
 import logging
 
+from testit_python_commons.models.link import Link
 from testit_python_commons.services import TmsPluginManager
 from testit_python_commons.services.logger import adapter_logger
 from testit_python_commons.services.utils import Utils
 from testit_python_commons.step import Step
 
 
 @Utils.deprecated('Use "addLinks" instead.')
 @adapter_logger
 def addLink(url: str, title: str = None, type: str = None, description: str = None):  # noqa: A002,VNE003,N802
     if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_link'):
         TmsPluginManager.get_plugin_manager().hook \
             .add_link(
-            link={
-                "url": url,
-                "title": title,
-                "type": type,
-                "description": description
-            }
-        )
+            link=Link()
+                .set_url(url)
+                .set_title(title)
+                .set_link_type(type)
+                .set_description(description))
 
 
 @adapter_logger
 def addLinks(url: str = None, title: str = None, type: str = None, description: str = None,  # noqa: A002,VNE003,N802
              links: list or tuple = None):
     if hasattr(TmsPluginManager.get_plugin_manager().hook, 'add_link'):
         if url:
             TmsPluginManager.get_plugin_manager().hook \
                 .add_link(
-                link={
-                    "url": url,
-                    "title": title,
-                    "type": type,
-                    "description": description
-                }
-            )
+                link=Link()
+                    .set_url(url)
+                    .set_title(title)
+                    .set_link_type(type)
+                    .set_description(description))
         elif links and (isinstance(links, list) or isinstance(links, tuple)):
             for link in links:
                 if isinstance(link, dict) and 'url' in link:
                     TmsPluginManager.get_plugin_manager().hook \
-                        .add_link(link=link)
+                        .add_link(link=Utils.convert_link_dict_to_link_model(link))
                 else:
                     logging.warning(f'Link ({link}) can\'t be processed!')
         else:
             logging.warning("Links can't be processed!\nPlease, set 'url' or 'links'!")
 
 
 @Utils.deprecated('Use "addMessage" instead.')
```

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons/services/adapter_manager.py` & `testit-python-commons-2.1.9/src/testit_python_commons/services/adapter_manager.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import uuid
 
 from testit_python_commons.client.api_client import ApiClientWorker
 from testit_python_commons.client.client_configuration import ClientConfiguration
 from testit_python_commons.models.adapter_mode import AdapterMode
+from testit_python_commons.models.test_result import TestResult
 from testit_python_commons.services.adapter_manager_configuration import AdapterManagerConfiguration
 from testit_python_commons.services.logger import adapter_logger
 
 
 class AdapterManager:
     def __init__(
             self,
@@ -32,17 +33,18 @@
     def get_autotests_for_launch(self):
         if self.__config.get_mode() == AdapterMode.USE_FILTER:
             return self.__api_client.get_autotests_by_test_run_id()
 
         return
 
     @adapter_logger
-    def write_test(self, test: dict):
-        test['automaticCreationTestCases'] = self.__config.should_automatic_creation_test_cases()
-        self.__api_client.write_test(test)
+    def write_test(self, test_result: TestResult):
+        test_result.set_automatic_creation_test_cases(
+            self.__config.should_automatic_creation_test_cases())
+        self.__api_client.write_test(test_result)
 
     @adapter_logger
     def load_attachments(self, attach_paths: list or tuple):
         return self.__api_client.load_attachments(attach_paths)
 
     @adapter_logger
     def create_attachment(self, body: str, name: str):
```

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons/services/adapter_manager_configuration.py` & `testit-python-commons-2.1.9/src/testit_python_commons/services/adapter_manager_configuration.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons/services/plugin_manager.py` & `testit-python-commons-2.1.9/src/testit_python_commons/services/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons/step.py` & `testit-python-commons-2.1.9/src/testit_python_commons/step.py`

 * *Files identical despite different names*

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons.egg-info/PKG-INFO` & `testit-python-commons-2.1.9/src/testit_python_commons.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-python-commons
-Version: 2.1.8
+Version: 2.1.9
 Summary: Python commons for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-python-commons-2.1.8/src/testit_python_commons.egg-info/SOURCES.txt` & `testit-python-commons-2.1.9/src/testit_python_commons.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,18 @@
 src/testit_python_commons.egg-info/top_level.txt
 src/testit_python_commons/client/__init__.py
 src/testit_python_commons/client/api_client.py
 src/testit_python_commons/client/client_configuration.py
 src/testit_python_commons/client/converter.py
 src/testit_python_commons/models/__init__.py
 src/testit_python_commons/models/adapter_mode.py
+src/testit_python_commons/models/link.py
 src/testit_python_commons/models/link_type.py
 src/testit_python_commons/models/outcome_type.py
+src/testit_python_commons/models/step_result.py
+src/testit_python_commons/models/test_result.py
 src/testit_python_commons/services/__init__.py
 src/testit_python_commons/services/adapter_manager.py
 src/testit_python_commons/services/adapter_manager_configuration.py
 src/testit_python_commons/services/logger.py
 src/testit_python_commons/services/plugin_manager.py
 src/testit_python_commons/services/utils.py
```


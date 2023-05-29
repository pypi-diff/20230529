# Comparing `tmp/testit-adapter-behave-2.1.8.tar.gz` & `tmp/testit-adapter-behave-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-behave-2.1.8.tar", last modified: Fri May 12 08:35:04 2023, max compression
+gzip compressed data, was "testit-adapter-behave-2.1.9.tar", last modified: Fri May 26 08:37:09 2023, max compression
```

## Comparing `testit-adapter-behave-2.1.8.tar` & `testit-adapter-behave-2.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:04.762863 testit-adapter-behave-2.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/src/testit_adapter_behave/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/listener.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/label.py
--rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/option.py
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/test_result_step.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/models/url_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     4176 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/scenario_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/tags_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-05-12 08:34:49.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:04.766864 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-12 08:35:04.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-12 08:35:04.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:35:04.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-12 08:35:04.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-12 08:35:04.000000 testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:09.894211 testit-adapter-behave-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-26 08:37:09.894211 testit-adapter-behave-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11409 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:09.894211 testit-adapter-behave-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:09.886211 testit-adapter-behave-2.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:09.890211 testit-adapter-behave-2.1.9/src/testit_adapter_behave/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4140 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/listener.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:09.894211 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)      498 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/option.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/test_result_step.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/models/url_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4148 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/scenario_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/tags_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-05-26 08:36:54.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:09.894211 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11945 2023-05-26 08:37:09.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 08:37:09.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:09.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-26 08:37:09.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 08:37:09.000000 testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/top_level.txt
```

### Comparing `testit-adapter-behave-2.1.8/PKG-INFO` & `testit-adapter-behave-2.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-behave
-Version: 2.1.8
+Version: 2.1.9
 Summary: Behave adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-behave-2.1.8/README.md` & `testit-adapter-behave-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.8/setup.py` & `testit-adapter-behave-2.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-behave',
-    version='2.1.8',
+    version='2.1.9',
     description='Behave adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -18,10 +18,10 @@
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_behave'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
     install_requires=[
         'behave',
-        'testit-python-commons==2.1.8',
+        'testit-python-commons==2.1.9',
         'attrs'],
 )
```

### Comparing `testit-adapter-behave-2.1.8/src/testit_adapter_behave/formatter.py` & `testit-adapter-behave-2.1.9/src/testit_adapter_behave/formatter.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-behave-2.1.8/src/testit_adapter_behave/listener.py` & `testit-adapter-behave-2.1.9/src/testit_adapter_behave/listener.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 
 from .models.test_result_step import get_test_result_step_model
 from .scenario_parser import (
     parse_scenario,
     parse_status)
 from .utils import (
     convert_step_to_step,
-    convert_step_to_step_result)
+    convert_step_to_step_result,
+    convert_executable_test_to_test_result_model)
 
 
 class AdapterListener(object):
     __executable_test = None
     __background_steps_count = 0
     __steps_count = 0
 
@@ -30,15 +31,16 @@
 
     def get_scenario(self, scenario):
         self.__executable_test = parse_scenario(scenario)
         self.__background_steps_count = len(scenario.background_steps)
         self.__steps_count = len(scenario.steps)
 
     def set_scenario(self):
-        self.__adapter_manager.write_test(self.__executable_test)
+        self.__adapter_manager.write_test(
+            convert_executable_test_to_test_result_model(self.__executable_test))
 
     def get_step_parameters(self, match):
         scope = self.get_scope()
 
         executable_step = get_test_result_step_model()
 
         for argument in match.arguments:
```

### Comparing `testit-adapter-behave-2.1.8/src/testit_adapter_behave/scenario_parser.py` & `testit-adapter-behave-2.1.9/src/testit_adapter_behave/scenario_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import traceback
 from enum import Enum
 
 from testit_python_commons.models.outcome_type import OutcomeType
-from testit_python_commons.services.utils import Utils
 
 from .models.tags import TagType
 from .tags_parser import parse_tags
 
 STATUS = {
     'passed': OutcomeType.PASSED,
     'failed': OutcomeType.FAILED,
@@ -82,15 +81,17 @@
 
 
 def get_scenario_name(scenario):
     return scenario.name if scenario.name else scenario.keyword
 
 
 def get_scenario_external_id(scenario):
-    return Utils.get_hash(scenario.feature.filename + scenario.name)
+    from .utils import get_hash
+
+    return get_hash(scenario.feature.filename + scenario.name)
 
 
 def get_scenario_namespace(scenario):
     return scenario.feature.filename
 
 
 def get_scenario_parameters(scenario):
```

### Comparing `testit-adapter-behave-2.1.8/src/testit_adapter_behave/tags_parser.py` & `testit-adapter-behave-2.1.9/src/testit_adapter_behave/tags_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from .models.label import get_label_model
 from .models.tags import TagType
-from .models.url_link import get_url_link_model
+from .models.url_link import get_url_to_link_model, get_dict_to_link_model
 
 
 def parse_tags(tags):
     parsed_tags = {
         TagType.LINKS: [],
         TagType.LABELS: [],
         TagType.WORK_ITEM_IDS: []
@@ -61,22 +61,23 @@
 
 
 def parse_links(tag: str):
     parsed_links = []
     json_links = parse_json(tag)
 
     if not json_links:
-        for link in parse_massive(tag):
-            parsed_links.append(get_url_link_model(link))
+        for url in parse_massive(tag):
+            parsed_links.append(get_url_to_link_model(url))
 
     if isinstance(json_links, tuple):
-        parsed_links.extend(json_links)
+        for url in json_links:
+            parsed_links.append(get_url_to_link_model(url))
 
     if isinstance(json_links, dict):
-        parsed_links.append(json_links)
+        parsed_links.append(get_dict_to_link_model(json_links))
 
     return parsed_links
 
 
 def parse_json(json_string: str):
     try:
         return eval(json_string)
```

### Comparing `testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/PKG-INFO` & `testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-behave
-Version: 2.1.8
+Version: 2.1.9
 Summary: Behave adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-behave-2.1.8/src/testit_adapter_behave.egg-info/SOURCES.txt` & `testit-adapter-behave-2.1.9/src/testit_adapter_behave.egg-info/SOURCES.txt`

 * *Files identical despite different names*


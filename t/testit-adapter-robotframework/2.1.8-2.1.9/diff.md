# Comparing `tmp/testit-adapter-robotframework-2.1.8.tar.gz` & `tmp/testit-adapter-robotframework-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-robotframework-2.1.8.tar", last modified: Fri May 12 08:35:01 2023, max compression
+gzip compressed data, was "testit-adapter-robotframework-2.1.9.tar", last modified: Fri May 26 08:37:07 2023, max compression
```

## Comparing `testit-adapter-robotframework-2.1.8.tar` & `testit-adapter-robotframework-2.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:01.702252 testit-adapter-robotframework-2.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-12 08:35:01.702252 testit-adapter-robotframework-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 08:35:01.702252 testit-adapter-robotframework-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:01.698252 testit-adapter-robotframework-2.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:01.702252 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/TMSLibrary.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/listeners.py
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-12 08:34:44.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 08:35:01.702252 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-12 08:35:01.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-12 08:35:01.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 08:35:01.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-12 08:35:01.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-12 08:35:01.000000 testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:07.845603 testit-adapter-robotframework-2.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-26 08:37:07.845603 testit-adapter-robotframework-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12815 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:37:07.845603 testit-adapter-robotframework-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:07.841603 testit-adapter-robotframework-2.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:07.845603 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/TMSLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4160 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-05-26 08:36:52.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:37:07.845603 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-05-26 08:37:07.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 08:37:07.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:37:07.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 08:37:07.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 08:37:07.000000 testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/top_level.txt
```

### Comparing `testit-adapter-robotframework-2.1.8/PKG-INFO` & `testit-adapter-robotframework-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.1.8
+Version: 2.1.9
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-robotframework-2.1.8/README.md` & `testit-adapter-robotframework-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.1.8/setup.py` & `testit-adapter-robotframework-2.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-robotframework',
-    version='2.1.8',
+    version='2.1.9',
     description='Robot Framework adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -16,9 +16,9 @@
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
     py_modules=['testit_adapter_robotframework'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.1.8']
+    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.1.9']
 )
```

### Comparing `testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/TMSLibrary.py` & `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/TMSLibrary.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from robot.libraries.BuiltIn import BuiltIn
 
 from testit_python_commons.services import TmsPluginManager
 
 from .listeners import AutotestAdapter, TestRunAdapter
-from .models import Link, Option
+from .models import Option
 
 
 def enabled(func):
     def wrapped(self, *args, **kwargs):
         if self.enabled:
             return func(self, *args, **kwargs)
         else:
@@ -69,15 +69,21 @@
     def add_link(self, url, type='Defect', title=None, description=None):  # noqa: A002,VNE003
         """
         Adds link to current test.
 
         Valid link types are ``Defect``, ``Issue``, ``Related``, ``BlockedBy``, ``Requirement``, ``Repository``.
 
         """
-        link = Link(url=url, type=type, title=title, description=description)
+        from testit_python_commons.models.link import Link
+
+        link = Link()\
+            .set_url(url)\
+            .set_title(title)\
+            .set_link_type(type)\
+            .set_description(description)
         self.ROBOT_LIBRARY_LISTENER[0].active_test.resultLinks.append(link)
 
     @enabled
     def add_links(self, *links):
         """
         Adds several links to current test.
```

### Comparing `testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/listeners.py` & `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/listeners.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import re
 
 from robot.api import SuiteVisitor, logger
 from robot.libraries.BuiltIn import BuiltIn
 
-from testit_python_commons.services import Utils
-
 from .models import Autotest
-from .utils import STATUSES, convert_time
+from .utils import STATUSES, convert_time, convert_executable_test_to_test_result_model, get_hash
 
 
 class AutotestAdapter:
     ROBOT_LISTENER_API_VERSION = 2
 
     def __init__(self, adapter_manager):
         self.adapter_manager = adapter_manager
@@ -65,15 +63,16 @@
                     for step in (self.active_test.setUpResults + self.active_test.stepResults +
                                  self.active_test.tearDownResults):
                         if step.outcome == 'Failed':
                             self.active_test.message = f"Failed on step: '{step.title}'"
                             break
             self.active_test.traces = attributes['message']
             self.active_test.duration = attributes['elapsedtime']
-            self.adapter_manager.write_test(self.active_test.order())
+            self.adapter_manager.write_test(
+                convert_executable_test_to_test_result_model(self.active_test.order()))
 
 
 class TestRunAdapter:
     ROBOT_LISTENER_API_VERSION = 3
 
     def __init__(self, adapter_manager):
         self.adapter_manager = adapter_manager
@@ -85,24 +84,24 @@
             suite.visit(selector)
 
 
 class ExcludeTests(SuiteVisitor):
 
     def __init__(self, *tests):
         self.tests = tests
-        if len(self.tests):
+        if not len(self.tests):
             logger.error('No tests to run!')
             raise SystemExit
 
     def start_suite(self, suite):
         suite.tests = [t for t in suite.tests if self._is_included(t)]
 
     def _is_included(self, test):
         tags = test.tags
-        external_id = Utils.get_hash(test.longname.split('.', 1)[-1])
+        external_id = get_hash(test.longname.split('.', 1)[-1])
         for tag in tags:
             if str(tag).lower().startswith('testit.externalid'):
                 external_id = tag.split(':', 1)[-1].strip()
         return external_id in self.tests
 
     def end_suite(self, suite):
         suite.suites = [s for s in suite.suites if s.test_count > 0]
```

### Comparing `testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework/models.py` & `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import ast
 import re
 
 from attr import Factory, asdict, attrib, s
 
 from robot.api import logger
+from testit_python_commons.models.link import Link
+
+from .utils import get_hash
 
-from testit_python_commons.services import Utils
 
 LinkTypes = ['Related', 'BlockedBy', 'Defect', 'Issue', 'Requirement', 'Repository']
 
 
 def link_type_check(self, attribute, value):
     if value.title() not in LinkTypes:
         raise ValueError(f"Incorrect Link type: {value}")
@@ -48,25 +50,14 @@
 @s
 class Step(Default):
     title = attrib()
     description = attrib()
     steps = attrib(default=Factory(list))
 
 
-@s(kw_only=True)
-class Link:
-    url = attrib(validator=[url_check])
-    type = attrib(default='Defect', validator=[link_type_check])  # noqa: A003,VNE003
-    title = attrib(default='')
-    description = attrib(default='')
-
-    def __attrs_post_init__(self):
-        self.type = self.type.title()
-
-
 @s
 class Label:
     name = attrib()
 
 
 @s(kw_only=True)
 class Autotest(Default):
@@ -126,17 +117,25 @@
                         self.workItemsID.extend([str(i) for i in value])
                     else:
                         logger.error(f"[TestIt] Wrong workitem format: {value}")
                 elif attr == 'links':
                     value = ast.literal_eval(value)
                     try:
                         if isinstance(value, dict):
-                            self.links.append(Link(**value))
+                            self.links.append(Link()\
+                                .set_url(value['url'])\
+                                .set_title(value.get('title', None))\
+                                .set_link_type(value.get('type', None))\
+                                .set_description(value.get('description', None)))
                         elif isinstance(value, list):
-                            self.links.extend([Link(**link) for link in value if isinstance(link, dict)])
+                            self.links.extend([Link()\
+                                .set_url(link['url'])\
+                                .set_title(link.get('title', None))\
+                                .set_link_type(link.get('type', None))\
+                                .set_description(link.get('description', None)) for link in value if isinstance(link, dict)])
                     except ValueError as e:
                         logger.error(f"[TestIt] Link Error: {e}")
                 elif attr == 'labels':
                     value = ast.literal_eval(value)
                     if isinstance(value, (str, int)):
                         self.labels.append(Label(value))
                     elif isinstance(value, list):
@@ -144,15 +143,15 @@
                 elif attr == 'namespace':
                     self.namespace = str(value).replace("'", "").replace('"', '')
                 elif attr == 'classname':
                     self.classname = str(value).replace("'", "").replace('"', '')
                 else:
                     logger.error(f"[TestIt] Unknown attribute: {attr}")
         if not self.externalID:
-            self.externalID = Utils.get_hash(attrs['longname'].split('.', 1)[-1])
+            self.externalID = get_hash(attrs['longname'].split('.', 1)[-1])
 
     def add_step(self, step_type, title, description, parameters):
         if len(self.step_depth) == 0:
             if step_type.lower() == 'setup':
                 self.setUp.append(Step(title, description))
                 self.step_depth.append(self.setUp[-1])
                 self.setUpResults.append(StepResult(title, description, parameters=parameters))
```

### Comparing `testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/PKG-INFO` & `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.1.8
+Version: 2.1.9
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `testit-adapter-robotframework-2.1.8/src/testit_adapter_robotframework.egg-info/SOURCES.txt` & `testit-adapter-robotframework-2.1.9/src/testit_adapter_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*


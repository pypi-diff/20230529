# Comparing `tmp/customdataclass-0.1.1.3.tar.gz` & `tmp/customdataclass-0.1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "customdataclass-0.1.1.3.tar", last modified: Tue May 16 12:20:33 2023, max compression
+gzip compressed data, was "customdataclass-0.1.1.4.tar", last modified: Mon May 29 16:48:07 2023, max compression
```

## Comparing `customdataclass-0.1.1.3.tar` & `customdataclass-0.1.1.4.tar`

### file list

```diff
@@ -1,25 +1,28 @@
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-16 12:20:33.759563 customdataclass-0.1.1.3/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1074 2023-04-27 13:55:41.000000 customdataclass-0.1.1.3/LICENSE.md
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4760 2023-05-16 12:20:33.759563 customdataclass-0.1.1.3/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4197 2023-05-02 11:45:36.000000 customdataclass-0.1.1.3/README.md
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      685 2023-05-16 12:20:09.000000 customdataclass-0.1.1.3/pyproject.toml
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-05-16 12:20:33.759563 customdataclass-0.1.1.3/setup.cfg
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-16 12:20:33.756230 customdataclass-0.1.1.3/src/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       48 2023-05-16 12:20:11.000000 customdataclass-0.1.1.3/src/__init__.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-16 12:20:33.759563 customdataclass-0.1.1.3/src/customdataclass.egg-info/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4760 2023-05-16 12:20:33.000000 customdataclass-0.1.1.3/src/customdataclass.egg-info/PKG-INFO
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      579 2023-05-16 12:20:33.000000 customdataclass-0.1.1.3/src/customdataclass.egg-info/SOURCES.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-05-16 12:20:33.000000 customdataclass-0.1.1.3/src/customdataclass.egg-info/dependency_links.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       25 2023-05-16 12:20:33.000000 customdataclass-0.1.1.3/src/customdataclass.egg-info/requires.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       25 2023-05-16 12:20:33.000000 customdataclass-0.1.1.3/src/customdataclass.egg-info/top_level.txt
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    15892 2023-05-16 12:19:18.000000 customdataclass-0.1.1.3/src/customdataclass.py
-drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-16 12:20:33.759563 customdataclass-0.1.1.3/tests/
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2223 2023-04-27 15:56:13.000000 customdataclass-0.1.1.3/tests/test_complex_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4377 2023-05-02 11:45:36.000000 customdataclass-0.1.1.3/tests/test_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2116 2023-05-01 13:46:55.000000 customdataclass-0.1.1.3/tests/test_dataclass_list.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      756 2023-04-27 15:56:26.000000 customdataclass-0.1.1.3/tests/test_default_value_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1459 2023-05-02 10:17:05.000000 customdataclass-0.1.1.3/tests/test_incomplete_typing_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1698 2023-05-16 12:10:28.000000 customdataclass-0.1.1.3/tests/test_mutable_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     5043 2023-04-27 16:09:06.000000 customdataclass-0.1.1.3/tests/test_nested_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2766 2023-04-27 15:56:38.000000 customdataclass-0.1.1.3/tests/test_partial_dataclass.py
--rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1131 2023-04-27 15:56:43.000000 customdataclass-0.1.1.3/tests/test_random_dataclass.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-29 16:48:07.478996 customdataclass-0.1.1.4/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1074 2023-04-27 13:55:41.000000 customdataclass-0.1.1.4/LICENSE.md
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     5310 2023-05-29 16:48:07.478996 customdataclass-0.1.1.4/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4747 2023-05-29 16:40:19.000000 customdataclass-0.1.1.4/README.md
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      709 2023-05-29 15:07:08.000000 customdataclass-0.1.1.4/pyproject.toml
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       38 2023-05-29 16:48:07.478996 customdataclass-0.1.1.4/setup.cfg
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-29 16:48:07.475662 customdataclass-0.1.1.4/src/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       48 2023-05-29 15:04:58.000000 customdataclass-0.1.1.4/src/__init__.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-29 16:48:07.475662 customdataclass-0.1.1.4/src/customdataclass.egg-info/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     5310 2023-05-29 16:48:07.000000 customdataclass-0.1.1.4/src/customdataclass.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      672 2023-05-29 16:48:07.000000 customdataclass-0.1.1.4/src/customdataclass.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)        1 2023-05-29 16:48:07.000000 customdataclass-0.1.1.4/src/customdataclass.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       25 2023-05-29 16:48:07.000000 customdataclass-0.1.1.4/src/customdataclass.egg-info/requires.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)       25 2023-05-29 16:48:07.000000 customdataclass-0.1.1.4/src/customdataclass.egg-info/top_level.txt
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)    20284 2023-05-29 16:44:40.000000 customdataclass-0.1.1.4/src/customdataclass.py
+drwxr-xr-x   0 lorenzo   (1000) lorenzo   (1000)        0 2023-05-29 16:48:07.475662 customdataclass-0.1.1.4/tests/
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2223 2023-05-29 12:50:25.000000 customdataclass-0.1.1.4/tests/test_complex_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     4377 2023-05-02 11:45:36.000000 customdataclass-0.1.1.4/tests/test_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     3290 2023-05-29 13:18:29.000000 customdataclass-0.1.1.4/tests/test_dataclass_list.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      756 2023-04-27 15:56:26.000000 customdataclass-0.1.1.4/tests/test_default_value_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1516 2023-05-29 13:40:20.000000 customdataclass-0.1.1.4/tests/test_incomplete_typing_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1970 2023-05-29 14:41:25.000000 customdataclass-0.1.1.4/tests/test_mutable_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     6960 2023-05-29 16:47:47.000000 customdataclass-0.1.1.4/tests/test_nested_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      762 2023-05-29 12:17:56.000000 customdataclass-0.1.1.4/tests/test_null_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     2912 2023-05-29 14:26:52.000000 customdataclass-0.1.1.4/tests/test_partial_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)     1147 2023-05-29 12:48:18.000000 customdataclass-0.1.1.4/tests/test_random_dataclass.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      440 2023-05-29 09:53:20.000000 customdataclass-0.1.1.4/tests/test_subclass_field.py
+-rw-r--r--   0 lorenzo   (1000) lorenzo   (1000)      991 2023-05-29 14:55:02.000000 customdataclass-0.1.1.4/tests/test_unenforced_dataclass.py
```

### Comparing `customdataclass-0.1.1.3/LICENSE.md` & `customdataclass-0.1.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.3/PKG-INFO` & `customdataclass-0.1.1.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: customdataclass
-Version: 0.1.1.3
-Summary: A custom dataclass implementation
-Author-email: Lorenzo Rossi <pypi@lorenzoros.si>
-License: MIT
-Project-URL: Homepage, https://github.com/lorossi/customdataclass
-Project-URL: Bug Tracker, https://github.com/lorossi/customdataclass/issues
-Project-URL: documentation, https://lorossi.github.io/customdataclass/
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # Customdataclass
 
 <p align="center">
 <img src=https://img.shields.io/github/issues-raw/lorossi/customdataclass></img>
 <img src=https://img.shields.io/pypi/l/customdataclass></img>
 <img src=https://img.shields.io/pypi/pyversions/customdataclass></img>
 <img src=https://img.shields.io/pypi/v/customdataclass></img>
@@ -36,40 +21,53 @@
 - dictionary keys are strings and there's no easy way to set a default value for a key
 - there's no way to ensure that a dictionary is well-formed
 - complex attributes that are needed once or twice cannot be generated on the fly and must be stored in the dictionary
 
 After a quick Google-fu session, I found out the existence of the `dataclass` decorator, swiftly provided by the `dataclasses`. This decorator allows you to create a class that is used only to hold data, and it provides a lot of useful features, such as:
 
 - default values for attributes
-- pre-determined methods *(such as `__init__`, `__repr__`, `__hash__`, etc.)*
+- pre-determined methods *(such as `__init__`, `__repr__`, etc.)*
 
 However, it does not handle easily features like:
 
 - complex attributes *(i.e. attributes that are dataclasses themselves)*
 - nested dataclasses *(i.e. a dataclass that has another dataclass as an attribute)*
 - serialization and deserialization
 - hashing and equality
 - type checking
 - inheritance
 
 All these were important for the project *(which once again will be finished, one day)* and so I decided to create a custom class that would handle all these features.
 
 I chose to create a class *(and not a decorator)* because I wanted to be able to inherit from it and to be able to use it as a base class for other dataclasses, thus solving the aforementioned problems.
 
+### Provided features
+
+- default values for attributes
+- type checking *(can be deactivated)*
+- nested dataclasses *(i.e. a dataclass that has another dataclass as an attribute)*
+- frozen dataclasses
+  - a dataclass cannot be modified after its creation *(if the parameter `frozen` is set to `True`, as per default)*
+  - otherwise, a dataclass can be manually frozen using the `freeze` method
+- equality comparison *(via the `__eq__` method)*
+- hashing *(via the `__hash__` method)*
+- full support inheritance
+- full support for methods overriding and custom properties
+
 ## Installing
 
 The package is available on PyPI and can be installed using `pip`:
 
 ```bash
 pip install -u customdataclass
 ```
 
 ## Examples
 
-Examples can be found in the `examples` folder, both in a text file [Examples.md](examples/Examples.md) and in a set of Python scripts.
+Examples can be found in the `examples` folder, both in a text file [EXAMPLES.md](EXAMPLES.md) and in a set of Python scripts.
 
 ## Tests
 
 Unit tests can be found in the `tests` folder.
 Currently, the code coverage for unit tests is close to 100%.
 
 ### Running the tests
```

### Comparing `customdataclass-0.1.1.3/README.md` & `customdataclass-0.1.1.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: customdataclass
+Version: 0.1.1.4
+Summary: A custom dataclass implementation
+Author-email: Lorenzo Rossi <pypi@lorenzoros.si>
+License: MIT
+Project-URL: Homepage, https://github.com/lorossi/customdataclass
+Project-URL: Bug Tracker, https://github.com/lorossi/customdataclass/issues
+Project-URL: documentation, https://lorossi.github.io/customdataclass/
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 # Customdataclass
 
 <p align="center">
 <img src=https://img.shields.io/github/issues-raw/lorossi/customdataclass></img>
 <img src=https://img.shields.io/pypi/l/customdataclass></img>
 <img src=https://img.shields.io/pypi/pyversions/customdataclass></img>
 <img src=https://img.shields.io/pypi/v/customdataclass></img>
@@ -21,40 +36,53 @@
 - dictionary keys are strings and there's no easy way to set a default value for a key
 - there's no way to ensure that a dictionary is well-formed
 - complex attributes that are needed once or twice cannot be generated on the fly and must be stored in the dictionary
 
 After a quick Google-fu session, I found out the existence of the `dataclass` decorator, swiftly provided by the `dataclasses`. This decorator allows you to create a class that is used only to hold data, and it provides a lot of useful features, such as:
 
 - default values for attributes
-- pre-determined methods *(such as `__init__`, `__repr__`, `__hash__`, etc.)*
+- pre-determined methods *(such as `__init__`, `__repr__`, etc.)*
 
 However, it does not handle easily features like:
 
 - complex attributes *(i.e. attributes that are dataclasses themselves)*
 - nested dataclasses *(i.e. a dataclass that has another dataclass as an attribute)*
 - serialization and deserialization
 - hashing and equality
 - type checking
 - inheritance
 
 All these were important for the project *(which once again will be finished, one day)* and so I decided to create a custom class that would handle all these features.
 
 I chose to create a class *(and not a decorator)* because I wanted to be able to inherit from it and to be able to use it as a base class for other dataclasses, thus solving the aforementioned problems.
 
+### Provided features
+
+- default values for attributes
+- type checking *(can be deactivated)*
+- nested dataclasses *(i.e. a dataclass that has another dataclass as an attribute)*
+- frozen dataclasses
+  - a dataclass cannot be modified after its creation *(if the parameter `frozen` is set to `True`, as per default)*
+  - otherwise, a dataclass can be manually frozen using the `freeze` method
+- equality comparison *(via the `__eq__` method)*
+- hashing *(via the `__hash__` method)*
+- full support inheritance
+- full support for methods overriding and custom properties
+
 ## Installing
 
 The package is available on PyPI and can be installed using `pip`:
 
 ```bash
 pip install -u customdataclass
 ```
 
 ## Examples
 
-Examples can be found in the `examples` folder, both in a text file [Examples.md](examples/Examples.md) and in a set of Python scripts.
+Examples can be found in the `examples` folder, both in a text file [EXAMPLES.md](EXAMPLES.md) and in a set of Python scripts.
 
 ## Tests
 
 Unit tests can be found in the `tests` folder.
 Currently, the code coverage for unit tests is close to 100%.
 
 ### Running the tests
```

### Comparing `customdataclass-0.1.1.3/pyproject.toml` & `customdataclass-0.1.1.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
-requires = ["setuptools>=61.0"]
-build-backend = "setuptools.build_meta"
+"requires" = ["setuptools>=61.0"]
+"build-backend" = "setuptools.build_meta"
 
 [project]
-name = "customdataclass"
-version = "0.1.1.3"
-authors = [{ name = "Lorenzo Rossi", email = "pypi@lorenzoros.si" }]
-description = "A custom dataclass implementation"
-readme = "README.md"
-requires-python = ">=3.7"
-classifiers = [
+"name" = "customdataclass"
+"version" = "0.1.1.4"
+"authors" = [{ name = "Lorenzo Rossi", email = "pypi@lorenzoros.si" }]
+"description" = "A custom dataclass implementation"
+"readme" = "README.md"
+"requires-python" = ">=3.7"
+"classifiers" = [
   "Programming Language :: Python :: 3",
   "Operating System :: OS Independent",
 ]
-license = { text = "MIT" }
-dependencies = ["PyYAML>=6.0", "toml>=0.10.2"]
+"license" = { text = "MIT" }
+"dependencies" = ["PyYAML>=6.0", "toml>=0.10.2"]
 
 [project.urls]
 "Homepage" = "https://github.com/lorossi/customdataclass"
 "Bug Tracker" = "https://github.com/lorossi/customdataclass/issues"
-documentation = "https://lorossi.github.io/customdataclass/"
+"documentation" = "https://lorossi.github.io/customdataclass/"
```

### Comparing `customdataclass-0.1.1.3/src/customdataclass.egg-info/PKG-INFO` & `customdataclass-0.1.1.4/src/customdataclass.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: customdataclass
-Version: 0.1.1.3
+Version: 0.1.1.4
 Summary: A custom dataclass implementation
 Author-email: Lorenzo Rossi <pypi@lorenzoros.si>
 License: MIT
 Project-URL: Homepage, https://github.com/lorossi/customdataclass
 Project-URL: Bug Tracker, https://github.com/lorossi/customdataclass/issues
 Project-URL: documentation, https://lorossi.github.io/customdataclass/
 Classifier: Programming Language :: Python :: 3
@@ -36,40 +36,53 @@
 - dictionary keys are strings and there's no easy way to set a default value for a key
 - there's no way to ensure that a dictionary is well-formed
 - complex attributes that are needed once or twice cannot be generated on the fly and must be stored in the dictionary
 
 After a quick Google-fu session, I found out the existence of the `dataclass` decorator, swiftly provided by the `dataclasses`. This decorator allows you to create a class that is used only to hold data, and it provides a lot of useful features, such as:
 
 - default values for attributes
-- pre-determined methods *(such as `__init__`, `__repr__`, `__hash__`, etc.)*
+- pre-determined methods *(such as `__init__`, `__repr__`, etc.)*
 
 However, it does not handle easily features like:
 
 - complex attributes *(i.e. attributes that are dataclasses themselves)*
 - nested dataclasses *(i.e. a dataclass that has another dataclass as an attribute)*
 - serialization and deserialization
 - hashing and equality
 - type checking
 - inheritance
 
 All these were important for the project *(which once again will be finished, one day)* and so I decided to create a custom class that would handle all these features.
 
 I chose to create a class *(and not a decorator)* because I wanted to be able to inherit from it and to be able to use it as a base class for other dataclasses, thus solving the aforementioned problems.
 
+### Provided features
+
+- default values for attributes
+- type checking *(can be deactivated)*
+- nested dataclasses *(i.e. a dataclass that has another dataclass as an attribute)*
+- frozen dataclasses
+  - a dataclass cannot be modified after its creation *(if the parameter `frozen` is set to `True`, as per default)*
+  - otherwise, a dataclass can be manually frozen using the `freeze` method
+- equality comparison *(via the `__eq__` method)*
+- hashing *(via the `__hash__` method)*
+- full support inheritance
+- full support for methods overriding and custom properties
+
 ## Installing
 
 The package is available on PyPI and can be installed using `pip`:
 
 ```bash
 pip install -u customdataclass
 ```
 
 ## Examples
 
-Examples can be found in the `examples` folder, both in a text file [Examples.md](examples/Examples.md) and in a set of Python scripts.
+Examples can be found in the `examples` folder, both in a text file [EXAMPLES.md](EXAMPLES.md) and in a set of Python scripts.
 
 ## Tests
 
 Unit tests can be found in the `tests` folder.
 Currently, the code coverage for unit tests is close to 100%.
 
 ### Running the tests
```

### Comparing `customdataclass-0.1.1.3/src/customdataclass.egg-info/SOURCES.txt` & `customdataclass-0.1.1.4/src/customdataclass.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -11,9 +11,12 @@
 tests/test_complex_dataclass.py
 tests/test_dataclass.py
 tests/test_dataclass_list.py
 tests/test_default_value_dataclass.py
 tests/test_incomplete_typing_dataclass.py
 tests/test_mutable_dataclass.py
 tests/test_nested_dataclass.py
+tests/test_null_dataclass.py
 tests/test_partial_dataclass.py
-tests/test_random_dataclass.py
+tests/test_random_dataclass.py
+tests/test_subclass_field.py
+tests/test_unenforced_dataclass.py
```

### Comparing `customdataclass-0.1.1.3/src/customdataclass.py` & `customdataclass-0.1.1.4/src/customdataclass.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """This module contains a custom dataclass object.
 
 It does work kinda good.
 """
 
 from __future__ import annotations
 
+import json
+import types
 from typing import Any
 
-import json
-import yaml
 import toml
+import yaml
 
 
 class Dataclass:
     """Custom dataclass.
 
     The real reason is that I didn't really like the way dataclasses work,
     and I wanted to have a better control over the attributes.
@@ -23,78 +24,86 @@
 
     This simplifies the code, allowing a better control over the attributes
     and the methods.
 
     Check the examples folder for more information.
 
     Initialization parameters:
-        enforce_types (bool, optional): If True, the types of the attributes \
+        enforce_types (bool, optional): If True, the types of the attributes
             are enforced. Defaults to True.
-        frozen (bool, optional): If True, attributes cannot be changed after \
+        frozen (bool, optional): If True, attributes cannot be changed after
             initialization. Defaults to True
-        partial (bool, optional): If True, parameters can be missing in the \
+        partial (bool, optional): If True, parameters can be missing in the
             initialization. Defaults to False.
     """
 
-    _frozen: bool = False
-    _frozen_after_init: bool = True
-    _enforce_types: bool = True
-    _partial = False
-    _deserialized: bool = False
-    _serializer: __module__ = None
+    _frozen: bool = False  # the class is frozen and cannot be changed
+    _frozen_after_init: bool = True  # the class is frozen after initialization
+    _enforce_types: bool = True  # the types of the attributes are enforced
+    _partial: bool = False  # the class can be initialized with missing attributes
+    _deserialized: bool = False  # the class is being deserialized
+    _serializer: str | None = None  # the serializer used
+    _attributes_dict: dict[str, tuple[type]] | None = None  # cache the attributes
 
     def __init__(self, **kwargs) -> Dataclass:
         """Create a new Dataclass.
 
         Raises:
             AttributeError: an invalid attribute is passed
             AttributeError: an attribute is missing in kwargs.
             TypeError: a value is not of the correct type.
         """
-        if not kwargs:
-            return
-
+        # initialize the attributes dict
+        self._attributes_dict = None
         # unfreeze the class for the initialisation
         self._frozen = False
 
         # check if all the attributes are valid
         self._checkAttributesValid(kwargs)
-
-        if not self._partial:
-            # fix the default values
-            self._fixDefaultValues(kwargs)
-            # check if all the attributes are present
-            self._checkAttributesPresent(kwargs)
-
-        # fix the types
-        self._fixMissingTypes()
+        # set the default values
+        self._setDefaultValues(kwargs)
 
         for k, v in self.__class_attributes__.items():
             # skip the loop if partial is True and the attribute is not present
-            if self._enforce_types and not (self._partial and k not in kwargs):
-                # serialized format don't support tuple and set (they convert \
+            if self._deserialized and self._enforce_types:
+                # serialized format don't support tuple and set (they convert
                 # both to list), so we need to convert them back IMPLICITLY
                 if self._checkDeserializedIterator(kwargs[k], v):
-                    if self._deserialized:
-                        # convert to tuple or set
-                        kwargs[k] = v(kwargs[k])
+                    # convert to tuple or set
+                    kwargs[k] = self._deserializeOperator(kwargs[k], v)
 
-                # serialised format don't support classes (they convert them to \
+                # serialised format don't support classes (they convert them to
                 # dict), so we need to convert them back IMPLICITLY
-                if self._checkDeserializedClass(kwargs[k], v):
+                elif self._checkDeserializedClass(kwargs[k], v):
                     # convert to class
-                    if self._deserialized:
-                        # convert to class
-                        kwargs[k] = v.from_dict(kwargs[k])
-
-                # check that the type is correct
-                if not self._checkTypeCorrect(kwargs[k], v):
-                    raise TypeError(f"{k} should be {v}, not {type(kwargs[k])}")
+                    class_type, is_list = self._getDeserializedClass(v)
+                    kwargs[k] = self._deserializeClass(kwargs[k], class_type, is_list)
+
+            # check that the type is correct
+            current_value = kwargs.get(k, None)
+            if self._enforce_types:
+                correct_type = self._checkTypeCorrect(current_value, v)
+            else:
+                correct_type = True
+            # the type is not correct if:
+            #   - the class is partial, the current value is not None,
+            #       the types are enforced and the type is not correct
+            #   - the class is not partial and the type is not correct
+            raise_condition = (
+                self._partial
+                and current_value is not None
+                and self._enforce_types
+                and not correct_type
+            ) or (not self._partial and not correct_type and self._enforce_types)
+
+            if raise_condition:
+                types = ", ".join(t.__name__ for t in v)
+                raise TypeError(f"{k} should be {types}, not {current_value.__class__}")
 
-            setattr(self, k, kwargs.get(k, None))
+            setattr(self, k, current_value)
 
         # freeze the class
         self._frozen = self._frozen_after_init
         # unset the deserialized flag
         self._deserialized = False
 
     def freeze(
@@ -104,129 +113,206 @@
 
         After this, attributes cannot be changed.
         The action cannot be undone.
         """
         self._frozen = True
 
     def _checkAttributesValid(self, kwargs: dict) -> bool:
-        """Check if all the attributes are valid (as specified in the class \
+        """Check if all the attributes are valid (as specified in the class
             definition).
 
         Args:
             kwargs (dict): kwargs to check
 
         Returns:
             bool: True if all the attributes are valid, False otherwise.
         """
         for k in kwargs.keys():
             if k not in self.__class_attributes__.keys():
                 raise AttributeError(f"{k} is not a valid attribute")
 
         return True
 
-    def _fixDefaultValues(self, kwargs: dict) -> None:
-        """Fix the default values.
+    def _setDefaultValues(self, kwargs: dict) -> None:
+        """Set the default values for the attributes.
 
         Args:
             kwargs (dict): kwargs to check
         """
         for k in self.__class_attributes__:
             if k not in kwargs:
-                kwargs[k] = self.__getattribute__(k)
+                try:
+                    default_value = self.__getattribute__(k)
+                except AttributeError:
+                    if self._partial:
+                        default_value = None
+                    else:
+                        raise AttributeError(f"Missing {k} in kwargs")
 
-    def _checkAttributesPresent(self, kwargs: dict) -> bool:
-        """Check if all the attributes are present (as specified in the class \
-            definition).
-
-        Args:
-            kwargs (dict): kwargs to check
+                kwargs[k] = default_value
 
-        Returns:
-            bool: True if all the attributes are present, False otherwise.
-        """
-        for k in self.__class_attributes__.keys():
-            if k not in kwargs:
-                raise AttributeError(f"Missing {k} in kwargs")
-
-        return True
-
-    def _fixMissingTypes(self) -> None:
-        """Fix the missing types."""
-        for k, v in self.__class_attributes__.items():
-            if v is None:
-                # no type has been specified
-                self.__class__.__annotations__[k] = Any
-
-    def _checkTypeCorrect(self, value: Any, valid_type: type) -> bool:
+    def _checkTypeCorrect(self, value: Any, valid_type: tuple[type]) -> bool:
         """Check if the type of the value is correct.
 
         Args:
             value (Any): value to check
-            valid_type (type): type of the value
+            valid_type (tuple[type]): tuple of valid types
 
         Returns:
             bool: True if the type is correct, False otherwise.
         """
-        if valid_type in (Any, None):
+        if Any in valid_type:
             return True
+        if value is None:
+            return any(t == types.NoneType for t in valid_type)  # noqa: E721
+
+        def check_type(value, type: Any) -> bool:
+            # if the type has the __origin__ attribute, it's a generic type
+            if hasattr(type, "__origin__"):
+                if type.__origin__ is dict:
+                    # check if the type is a dict of the specified type
+                    for k in value:
+                        for t in type.__args__:
+                            if check_type(k, t):
+                                return True
+            try:
+                # isinstance doesn't work with generic types
+                return isinstance(value, type)
+            except TypeError:
+                # check if the type is a tuple of the specified type
+                for i, t in enumerate(type.__args__):
+                    if check_type(value[i], t):
+                        return True
+
+        # at least one of the types must be correct
+        return any(check_type(value, t) for t in valid_type)
+
+    def _deserializeOperator(
+        self, value: list[Any], valid_type: tuple[type]
+    ) -> set[Any] | tuple[Any] | list[Any]:
+        """Return the deserialized iterator.
 
-        try:
-            valid = isinstance(value, valid_type)
-        except TypeError:
-            valid = all(issubclass(v.__class__, valid_type.__args__[0]) for v in value)
-        except Exception:
-            valid = False
+        Args:
+            value (list[Any]): value to check
+            valid_type (type): type of the value
 
-        return valid
+        Returns:
+            bool: True if the value is valid, False otherwise.
+        """
+        class_type = next(t for t in valid_type if t is not None)
+        return class_type(value)
 
     def _checkDeserializedIterator(self, value: list[Any], valid_type: type) -> bool:
-        """Check if the value is a valid iterator.
+        """Check if the value is a deserialized iterator.
+
+        JSON, TOML and YAML convert sets and tuples to lists, so we need to
+        convert them back.
 
         Args:
             value (list[Any]): value to check
             valid_type (type): type of the value
 
         Returns:
             bool: True if the value is valid, False otherwise.
         """
-        if not isinstance(value, list):
-            return False
+        if isinstance(value, list):
+            if list in valid_type:
+                return False
+            if any(t in valid_type for t in (tuple, set)):
+                return True
+        # if value is not a list, then there's no need to convert it
+        return False
+
+    def _deserializeClass(
+        self, value: dict | list[dict], valid_type: type, is_list: bool
+    ) -> list[Dataclass] | Dataclass:
+        """Check if the value is a deserialized class.
+
+        JSON, TOML and YAML convert classes to dicts, so we need to
+        convert them back.
+        Since both lists of dictionaries and single dictionaries
+        can be instances of Dataclass objects (or subclasses of Dataclass),
+        we need to check if the value is a list or not.
+
+        Args:
+            value (dict | list[dict]): value to check
+            valid_type (type): type of the value
+
+        Returns:
+            bool: True if the value is valid, False otherwise.
+        """
+        # a list of Dataclass is converted to a list
+        # a single Dataclass is converted to a dict
+        if is_list:
+            return [valid_type.from_dict(i) for i in value]
+
+        return valid_type.from_dict(value)
 
-        return valid_type in (set, tuple)
+    def _getDeserializedClass(self, valid_type: tuple[type]) -> tuple[type, bool]:
+        """Return the deserialized class.
 
-    def _checkDeserializedClass(self, value: dict, valid_type: type) -> bool:
+        Objects
+
+        Args:
+            valid_type (tuple[type]): type of the value
+
+        Returns:
+            tuple[type, bool]: type of the value and if it's a list
+        """
+        convert_class = next(t for t in valid_type if t is not None)
+        if hasattr(convert_class, "__origin__") and convert_class.__origin__ is list:
+            inner_class = next(t for t in convert_class.__args__ if t is not None)
+            return inner_class, True
+
+        return convert_class, False
+
+    def _checkDeserializedClass(self, value: dict, valid_type: tuple[type]) -> bool:
         """Check if the value is a valid class.
 
         Args:
             value (dict): value to check
             valid_type (type): type of the value
 
         Returns:
             bool: True if the value is valid, False otherwise.
         """
-        if not isinstance(value, dict):
+        # a list of Dataclass is converted to a list
+        # a single Dataclass is converted to a dict
+        if not isinstance(value, dict) and not isinstance(value, list):
             return False
 
-        return issubclass(valid_type, Dataclass)
+        if isinstance(value, dict):
+            return any(issubclass(t, Dataclass) for t in valid_type)
+
+        if isinstance(value, list):
+            for i in value:
+                if not isinstance(i, dict):
+                    return False
+
+            for t in valid_type:
+                if hasattr(t, "__origin__") and t.__origin__ is list:
+                    return any(issubclass(t, Dataclass) for t in t.__args__)
+
+        return False
 
     def __init_subclass__(
         cls,
         enforce_types: bool = True,
         frozen: bool = True,
         partial: bool = False,
         **kwargs,
     ) -> None:
         """Initialize the subclass.
 
         Args:
-            enforce_types (bool, optional): If True, the types of the attributes \
-                are enforced.
-            frozen (bool, optional): If True, attributes cannot be changed after \
+            enforce_types (bool, optional): If True, the types of the attributes
+                are enforced. Defaults to True.
+            frozen (bool, optional): If True, attributes cannot be changed after
                 initialization. Defaults to True.
-            partial (bool, optional): If True, the class can be initialized with \
+            partial (bool, optional): If True, the class can be initialized with
                 missing attributes. Defaults to False.
         """
         cls._enforce_types = enforce_types
         cls._frozen_after_init = frozen
         cls._partial = partial
         super().__init_subclass__(**kwargs)
 
@@ -325,15 +411,15 @@
         """
         ordered = sorted(self.__clean_dict__.items())
         return hash(tuple(ordered))
 
     def __contains__(self, item) -> bool:
         """Check if the object contains an item.
 
-        This is used to check if an attribute exists via the \
+        This is used to check if an attribute exists via the
         built-in `in` operator.
 
         Args:
             item (any): item to check
 
         Returns:
             bool
@@ -351,35 +437,44 @@
     @property
     def __class_attributes__(self) -> dict[str, type]:
         """Return all the attributes of the class and their type.
 
         Returns:
             dict
         """
-        return {
-            k: v if isinstance(v, type) else None
-            for k, v in self.__class__.__annotations__.items()
-            if not k.startswith("_")
-        }
+        # cache the result
+        if self._attributes_dict is not None:
+            return self._attributes_dict
+
+        self._attributes_dict = {}
+        for k, v in self.__class__.__annotations__.items():
+            if v is Any:
+                self._attributes_dict[k] = (Any,)
+            elif isinstance(v, types.UnionType):
+                self._attributes_dict[k] = tuple(t for t in v.__args__)
+            else:
+                self._attributes_dict[k] = (v,)
+
+        return self._attributes_dict
 
     @property
     def __clean_dict__(self) -> dict:
-        """Return a dictionary with all the attributes of the object, \
+        """Return a dictionary with all the attributes of the object,
             except for the ones starting with an underscore (private).
 
         Returns:
             dict
         """
         return {k: v for k, v in self.__dict__.items() if not k.startswith("_")}
 
     def _importDecorator(f, *_, **__) -> None:
         """Import the correct serializer for the function.
 
         The serializer will be put in the `_serializer` attribute of the object.
-        It's mandatory to have all the functions decorated with this decorator \
+        It's mandatory to have all the functions decorated with this decorator
         to contain the name of the serializer in their name.
 
         Unittest will require all the serializers to be installed.
 
         Args:
             f (function): function to decorate
 
@@ -394,17 +489,14 @@
         serializer = None
 
         for k, v in libs.items():
             if k in f.__name__:
                 serializer = v
                 break
 
-        if serializer is None:
-            raise NotImplementedError(f"Serializer for {f.__name__} not implemented.")
-
         def wrapper(self: Dataclass, *args, **kwargs):
             self._serializer = serializer
             return f(self, *args, **kwargs)
 
         return wrapper
 
     @property
@@ -441,15 +533,15 @@
         """Return the frozen status of the object."""
         return self._frozen
 
     @property
     @_importDecorator
     def to_json(self) -> str:
         """
-        Return a json representation of the object. \
+        Return a json representation of the object.
         Attributes are recursively converted to json.
 
         Returns:
             str
         """
         dict_data = self.to_dict
 
@@ -497,61 +589,61 @@
         Returns:
             list
         """
         return list(self.__class_attributes__.keys())
 
     @classmethod
     @_importDecorator
-    def from_json(cls, json_string: str):
+    def from_json(cls, json_string: str) -> Dataclass:
         """Create an object from a json string.
 
         Args:
             json_string (str): json string
 
         Returns:
-            object
+            Dataclass
         """
         cls._deserialized = True
         return cls(**cls._serializer.loads(json_string))
 
     @classmethod
     @_importDecorator
-    def from_toml(cls, toml_string: str):
+    def from_toml(cls, toml_string: str) -> Dataclass:
         """Create an object from a toml string.
 
         Args:
             toml_string (str): toml string
 
         Returns:
-            object
+            Dataclass
         """
         cls._deserialized = True
         return cls(**cls._serializer.loads(toml_string))
 
     @classmethod
     @_importDecorator
-    def from_yaml(cls, yaml_string: str):
+    def from_yaml(cls, yaml_string: str) -> Dataclass:
         """Create an object from a yaml string.
 
         Args:
             yaml_string (str): yaml string
 
         Returns:
-            object
+            Dataclass
         """
         cls._deserialized = True
         return cls(
             **cls._serializer.load(yaml_string, Loader=cls._serializer.FullLoader)
         )
 
     @classmethod
-    def from_dict(cls, d: dict):
+    def from_dict(cls, d: dict) -> Dataclass:
         """Create an object from a dictionary.
 
         Args:
             d (dict): dictionary
 
         Returns:
-            object
+            Dataclass
         """
         cls._deserialized = True
         return cls(**d)
```

### Comparing `customdataclass-0.1.1.3/tests/test_complex_dataclass.py` & `customdataclass-0.1.1.4/tests/test_complex_dataclass.py`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.3/tests/test_dataclass.py` & `customdataclass-0.1.1.4/tests/test_dataclass.py`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.3/tests/test_default_value_dataclass.py` & `customdataclass-0.1.1.4/tests/test_default_value_dataclass.py`

 * *Files identical despite different names*

### Comparing `customdataclass-0.1.1.3/tests/test_incomplete_typing_dataclass.py` & `customdataclass-0.1.1.4/tests/test_incomplete_typing_dataclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 class IncompleteDataclass(Dataclass):
     """Test class."""
 
     int_var: int
     float_var: float
     str_var: str
-    bool_var: False
+    bool_var: bool
 
 
-class MutableIncompleteDataclass(Dataclass, frozen=False):
+class MutableIncompleteDataclass(Dataclass, frozen=False, partial=True):
     """Test class."""
 
-    int_var: False
+    int_var = False
 
 
 class TestIncompleteDataclass(unittest.TestCase):
     def testCreation(self):
         i = IncompleteDataclass(int_var=1, float_var=1.0, str_var="1", bool_var=True)
         self.assertEqual(i.int_var, 1)
         self.assertEqual(i.float_var, 1.0)
@@ -29,14 +29,15 @@
         self.assertIsInstance(i.int_var, int)
         self.assertIsInstance(i.float_var, float)
         self.assertIsInstance(i.str_var, str)
         self.assertIsInstance(i.bool_var, bool)
 
     def testTypeChange(self):
         i = MutableIncompleteDataclass()
+        self.assertEqual(i.int_var, False)
         i.int_var = 1
         self.assertEqual(i.int_var, 1)
 
     def testEquality(self):
         i1 = IncompleteDataclass(int_var=1, float_var=1.0, str_var="1", bool_var=True)
         i2 = IncompleteDataclass(int_var=1, float_var=1.0, str_var="1", bool_var=True)
         self.assertEqual(i1, i2)
```

### Comparing `customdataclass-0.1.1.3/tests/test_mutable_dataclass.py` & `customdataclass-0.1.1.4/tests/test_mutable_dataclass.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,7 +54,16 @@
 
     def testFreeze(self):
         s, _ = self._createDataclass()
         s.freeze()
         self.assertTrue(s.frozen)
         with self.assertRaises(AttributeError):
             s.int_var = 2
+
+    def testUnfreeze(self):
+        s, _ = self._createDataclass()
+        s.freeze()
+        self.assertTrue(s.frozen)
+        with self.assertRaises(AttributeError):
+            s.freeze = False
+        with self.assertRaises(AttributeError):
+            s.int_var = 2
```

### Comparing `customdataclass-0.1.1.3/tests/test_nested_dataclass.py` & `customdataclass-0.1.1.4/tests/test_nested_dataclass.py`

 * *Files 18% similar despite different names*

```diff
@@ -183,7 +183,72 @@
         self.assertEqual(o1, o3)
 
         o4 = Outer.from_toml(o1.to_toml)
         self.assertEqual(o1, o4)
 
         o5 = Outer.from_yaml(o1.to_yaml)
         self.assertEqual(o1, o5)
+
+
+class FakeNestedDataclass(Dataclass):
+    int_var: int
+    dict_var: dict[str, int] = {"a": 1, "b": 2}
+    list_var: list[int] = [1, 2, 3]
+
+
+class TestFakeNestedDataclass(unittest.TestCase):
+    def testCreation(self):
+        f = FakeNestedDataclass(int_var=1)
+        self.assertEqual(f.int_var, 1)
+        self.assertEqual(f.dict_var, {"a": 1, "b": 2})
+        self.assertEqual(f.list_var, [1, 2, 3])
+
+
+class BaseDataclass(Dataclass):
+    """Test class."""
+
+    int_var: int
+    float_var: float
+
+
+class DerivedDataclass(BaseDataclass):
+    """Test class."""
+
+    str_var: str
+    list_var: list
+
+
+class ContainerDataClass2(Dataclass):
+    """Test class."""
+
+    number_dataclass: BaseDataclass
+    string_dataclass: DerivedDataclass
+
+
+class TestNestedDataclass2(unittest.TestCase):
+    def _createNestedDataclass(self) -> ContainerDataClass2:
+        s1 = BaseDataclass(int_var=1, float_var=1.0)
+        s2 = DerivedDataclass(str_var="123", list_var=[1, 2, 3])
+        return ContainerDataClass2(number_dataclass=s1, string_dataclass=s2)
+
+    def testCreation(self):
+        s = self._createNestedDataclass()
+        self.assertEqual(s.number_dataclass.int_var, 1)
+        self.assertEqual(s.number_dataclass.float_var, 1.0)
+        self.assertEqual(s.string_dataclass.str_var, "123")
+        self.assertEqual(s.string_dataclass.list_var, [1, 2, 3])
+
+        self.assertIsInstance(s.number_dataclass.int_var, int)
+        self.assertIsInstance(s.number_dataclass.float_var, float)
+        self.assertIsInstance(s.string_dataclass.str_var, str)
+        self.assertIsInstance(s.string_dataclass.list_var, list)
+
+    def testEquality(self):
+        s1 = self._createNestedDataclass()
+        s2 = self._createNestedDataclass()
+
+        self.assertEqual(s1, s2)
+        self.assertEqual(str(s1), str(s2))
+        self.assertEqual(repr(s1), repr(s2))
+
+        with self.assertRaises(TypeError):
+            hash(s1)
```

### Comparing `customdataclass-0.1.1.3/tests/test_partial_dataclass.py` & `customdataclass-0.1.1.4/tests/test_partial_dataclass.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,14 +53,18 @@
         self.assertIsInstance(p.int_var, int)
         self.assertIsInstance(p.float_var, float)
         self.assertIsInstance(p.str_var, str)
 
         p.bool_var = True
         self.assertEqual(p.bool_var, True)
 
+    def testInvalidField(self):
+        with self.assertRaises(TypeError):
+            PartialDataclass(int_var="1", float_var=1.0, str_var="1")
+
     def testEquality(self):
         p1 = PartialMutableDataclass(int_var=1, float_var=1.0, str_var="1")
         p2 = PartialMutableDataclass(int_var=1, float_var=1.0, str_var="1")
 
         self.assertEqual(p1, p2)
 
         p1.bool_var = True
```


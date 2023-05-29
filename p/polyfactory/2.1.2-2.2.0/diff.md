# Comparing `tmp/polyfactory-2.1.2.tar.gz` & `tmp/polyfactory-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyfactory-2.1.2.tar", max compression
+gzip compressed data, was "polyfactory-2.2.0.tar", max compression
```

## Comparing `polyfactory-2.1.2.tar` & `polyfactory-2.2.0.tar`

### file list

```diff
@@ -1,31 +1,32 @@
--rw-r--r--   0        0        0     1092 2023-05-28 07:11:11.577643 polyfactory-2.1.2/LICENSE
--rw-r--r--   0        0        0     9429 2023-05-28 07:11:11.577643 polyfactory-2.1.2/README.md
--rw-r--r--   0        0        0      425 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/__init__.py
--rw-r--r--   0        0        0      642 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/constants.py
--rw-r--r--   0        0        0     1037 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/decorators.py
--rw-r--r--   0        0        0      591 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/exceptions.py
--rw-r--r--   0        0        0      257 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/__init__.py
--rw-r--r--   0        0        0    30734 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/base.py
--rw-r--r--   0        0        0     2757 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/beanie_odm_factory.py
--rw-r--r--   0        0        0     1603 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/dataclass_factory.py
--rw-r--r--   0        0        0     2193 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/odmantic_odm_factory.py
--rw-r--r--   0        0        0     7552 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/pydantic_factory.py
--rw-r--r--   0        0        0     1471 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/factories/typed_dict_factory.py
--rw-r--r--   0        0        0     2939 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/field_meta.py
--rw-r--r--   0        0        0     3328 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/fields.py
--rw-r--r--   0        0        0     1191 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/persistence.py
--rw-r--r--   0        0        0        0 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/py.typed
--rw-r--r--   0        0        0     2890 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/pytest_plugin.py
--rw-r--r--   0        0        0        0 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/utils/__init__.py
--rw-r--r--   0        0        0     2162 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/utils/helpers.py
--rw-r--r--   0        0        0     3401 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/utils/predicates.py
--rw-r--r--   0        0        0        0 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/__init__.py
--rw-r--r--   0        0        0     2807 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/complex_types.py
--rw-r--r--   0        0        0     1838 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/constrained_collections.py
--rw-r--r--   0        0        0     1069 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/constrained_dates.py
--rw-r--r--   0        0        0    13431 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/constrained_numbers.py
--rw-r--r--   0        0        0     3845 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/constrained_strings.py
--rw-r--r--   0        0        0     3635 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/primitives.py
--rw-r--r--   0        0        0     6185 2023-05-28 07:11:11.581643 polyfactory-2.1.2/polyfactory/value_generators/regex.py
--rw-r--r--   0        0        0     6030 2023-05-28 07:11:11.581643 polyfactory-2.1.2/pyproject.toml
--rw-r--r--   0        0        0    11250 1970-01-01 00:00:00.000000 polyfactory-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-29 16:14:20.435754 polyfactory-2.2.0/LICENSE
+-rw-r--r--   0        0        0     9446 2023-05-29 16:14:20.435754 polyfactory-2.2.0/README.md
+-rw-r--r--   0        0        0      425 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/__init__.py
+-rw-r--r--   0        0        0      642 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/constants.py
+-rw-r--r--   0        0        0     1037 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/decorators.py
+-rw-r--r--   0        0        0      591 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/exceptions.py
+-rw-r--r--   0        0        0      257 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/__init__.py
+-rw-r--r--   0        0        0    30734 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/base.py
+-rw-r--r--   0        0        0     2757 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/beanie_odm_factory.py
+-rw-r--r--   0        0        0     1603 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/dataclass_factory.py
+-rw-r--r--   0        0        0     6812 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/msgspec_factory.py
+-rw-r--r--   0        0        0     2193 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/odmantic_odm_factory.py
+-rw-r--r--   0        0        0     7552 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/pydantic_factory.py
+-rw-r--r--   0        0        0     1471 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/factories/typed_dict_factory.py
+-rw-r--r--   0        0        0     2939 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/field_meta.py
+-rw-r--r--   0        0        0     3328 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/fields.py
+-rw-r--r--   0        0        0     1191 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/persistence.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/py.typed
+-rw-r--r--   0        0        0     2890 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/utils/__init__.py
+-rw-r--r--   0        0        0     2162 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/utils/helpers.py
+-rw-r--r--   0        0        0     3401 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/utils/predicates.py
+-rw-r--r--   0        0        0        0 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/__init__.py
+-rw-r--r--   0        0        0     2807 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/complex_types.py
+-rw-r--r--   0        0        0     1838 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/constrained_collections.py
+-rw-r--r--   0        0        0     1069 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/constrained_dates.py
+-rw-r--r--   0        0        0    13431 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/constrained_numbers.py
+-rw-r--r--   0        0        0     3845 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/constrained_strings.py
+-rw-r--r--   0        0        0     3635 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/primitives.py
+-rw-r--r--   0        0        0     6185 2023-05-29 16:14:20.439754 polyfactory-2.2.0/polyfactory/value_generators/regex.py
+-rw-r--r--   0        0        0     6177 2023-05-29 16:14:20.439754 polyfactory-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11368 1970-01-01 00:00:00.000000 polyfactory-2.2.0/PKG-INFO
```

### Comparing `polyfactory-2.1.2/LICENSE` & `polyfactory-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/README.md` & `polyfactory-2.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 </div>
 <!-- markdownlint-restore -->
 
 Polyfactory is a simple and powerful mock data generation library, based around type
-hints and supporting dataclasses, typed-dicts, Pydantic models and more.
+hints and supporting dataclasses, typed-dicts, pydantic models, msgspec structs and more.
 
 Polyfactory part of the Litestar project and as such actively maintained by a community of maintainers and contributors.
 
 ## Example
 
 ```python
 from dataclasses import dataclass
```

### Comparing `polyfactory-2.1.2/polyfactory/constants.py` & `polyfactory-2.2.0/polyfactory/constants.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/decorators.py` & `polyfactory-2.2.0/polyfactory/decorators.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/exceptions.py` & `polyfactory-2.2.0/polyfactory/exceptions.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/factories/base.py` & `polyfactory-2.2.0/polyfactory/factories/base.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/factories/beanie_odm_factory.py` & `polyfactory-2.2.0/polyfactory/factories/beanie_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/factories/dataclass_factory.py` & `polyfactory-2.2.0/polyfactory/factories/dataclass_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/factories/odmantic_odm_factory.py` & `polyfactory-2.2.0/polyfactory/factories/odmantic_odm_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/factories/pydantic_factory.py` & `polyfactory-2.2.0/polyfactory/factories/pydantic_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/factories/typed_dict_factory.py` & `polyfactory-2.2.0/polyfactory/factories/typed_dict_factory.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/field_meta.py` & `polyfactory-2.2.0/polyfactory/field_meta.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/fields.py` & `polyfactory-2.2.0/polyfactory/fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
-from typing import Any, Callable, Generic, TypeVar, cast
+from typing import Any, Callable, Generic, TypeVar, cast, TypedDict
 
-from typing_extensions import ParamSpec, TypedDict
+from typing_extensions import ParamSpec
 
 from polyfactory.exceptions import ParameterException
 
 T = TypeVar("T")
 P = ParamSpec("P")
```

### Comparing `polyfactory-2.1.2/polyfactory/persistence.py` & `polyfactory-2.2.0/polyfactory/persistence.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/pytest_plugin.py` & `polyfactory-2.2.0/polyfactory/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/utils/helpers.py` & `polyfactory-2.2.0/polyfactory/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/utils/predicates.py` & `polyfactory-2.2.0/polyfactory/utils/predicates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/value_generators/complex_types.py` & `polyfactory-2.2.0/polyfactory/value_generators/complex_types.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/value_generators/constrained_collections.py` & `polyfactory-2.2.0/polyfactory/value_generators/constrained_collections.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/value_generators/constrained_dates.py` & `polyfactory-2.2.0/polyfactory/value_generators/constrained_dates.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/value_generators/constrained_numbers.py` & `polyfactory-2.2.0/polyfactory/value_generators/constrained_numbers.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/value_generators/constrained_strings.py` & `polyfactory-2.2.0/polyfactory/value_generators/constrained_strings.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/value_generators/primitives.py` & `polyfactory-2.2.0/polyfactory/value_generators/primitives.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/polyfactory/value_generators/regex.py` & `polyfactory-2.2.0/polyfactory/value_generators/regex.py`

 * *Files identical despite different names*

### Comparing `polyfactory-2.1.2/pyproject.toml` & `polyfactory-2.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "polyfactory"
-version = "2.1.2"
+version = "2.2.0"
 description = "Mock data generation factories"
 authors = [
     "Na'aman Hirschfeld <nhirschfeld@gmail.com>",
     "Peter Schutt <peter.github@proton.me>",
     "Cody Fincher <cody.fincher@gmail.com>",
     "Janek Nouvertné <provinzkraut@posteo.de>",
     "Jacob Coffee <jacob@z7x.org>",
@@ -18,21 +18,24 @@
 ]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/litestar-org/polyfactory"
 repository = "https://github.com/litestar-org/polyfactory"
 documentation = "https://github.com/litestar-org/polyfactory"
 keywords = [
+    "beanie",
     "dataclasses",
     "factory",
     "faker",
+    "litestar",
     "mock",
+    "msgspec",
+    "odmantic",
     "pydantic",
     "pytest",
-    "litestar",
     "tdd",
     "testing",
     "typeddict",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
@@ -57,42 +60,44 @@
     { include = "polyfactory" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<4.0"
 beanie = { version = "*", optional = true, extras = ["beanie"] }
 faker = "*"
+msgspec = { version = "*", optional = true, extras = ["msgspec"] }
 odmantic = { version = "*", optional = true, extras = ["odmantic"] }
 pydantic = { version = "*", optional = true, extras = ["pydantic", "odmantic", "beanie"] }
 typing-extensions = "*"
 
 [tool.poetry.group.dev.dependencies]
 beanie = "*"
 email-validator = "*"
 hypothesis = "*"
+mongomock-motor = "*"
+msgspec = "*"
 odmantic = "*"
 pre-commit = "*"
 pydantic = "*"
 pytest = "*"
 pytest-asyncio = "*"
 pytest-cov = "*"
-mongomock-motor = "*"
-
 
 [tool.poetry.group.docs.dependencies]
 sphinx-autobuild = "*"
 blacken-docs = "*"
 auto-pytabs = "*"
 sphinxcontrib-mermaid = "*"
 sphinx-copybutton = "*"
 sphinx = "*"
 litestar-sphinx-theme = { git = "https://github.com/litestar-org/litestar-sphinx-theme.git" }
 
 [tool.poetry.extras]
 pydantic = ["pydantic"]
+msgspec = ["msgspec"]
 odmantic = ["odmantic", "pydantic"]
 beanie = ["beanie", "pydantic"]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `polyfactory-2.1.2/PKG-INFO` & `polyfactory-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: polyfactory
-Version: 2.1.2
+Version: 2.2.0
 Summary: Mock data generation factories
 Home-page: https://github.com/litestar-org/polyfactory
 License: MIT
-Keywords: dataclasses,factory,faker,mock,pydantic,pytest,litestar,tdd,testing,typeddict
+Keywords: beanie,dataclasses,factory,faker,litestar,mock,msgspec,odmantic,pydantic,pytest,tdd,testing,typeddict
 Author: Na'aman Hirschfeld
 Author-email: nhirschfeld@gmail.com
 Maintainer: Na'aman Hirschfeld
 Maintainer-email: nhirschfeld@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -26,18 +26,20 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Testing :: Unit
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Provides-Extra: beanie
+Provides-Extra: msgspec
 Provides-Extra: odmantic
 Provides-Extra: pydantic
 Requires-Dist: beanie[beanie] ; extra == "beanie"
 Requires-Dist: faker
+Requires-Dist: msgspec[msgspec] ; extra == "msgspec"
 Requires-Dist: odmantic[odmantic] ; extra == "odmantic"
 Requires-Dist: pydantic[beanie,odmantic,pydantic] ; extra == "pydantic" or extra == "odmantic" or extra == "beanie"
 Requires-Dist: typing-extensions
 Project-URL: Documentation, https://github.com/litestar-org/polyfactory
 Project-URL: Repository, https://github.com/litestar-org/polyfactory
 Description-Content-Type: text/markdown
 
@@ -73,15 +75,15 @@
 
 <!-- ALL-CONTRIBUTORS-BADGE:END -->
 
 </div>
 <!-- markdownlint-restore -->
 
 Polyfactory is a simple and powerful mock data generation library, based around type
-hints and supporting dataclasses, typed-dicts, Pydantic models and more.
+hints and supporting dataclasses, typed-dicts, pydantic models, msgspec structs and more.
 
 Polyfactory part of the Litestar project and as such actively maintained by a community of maintainers and contributors.
 
 ## Example
 
 ```python
 from dataclasses import dataclass
```


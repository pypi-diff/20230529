# Comparing `tmp/rpaframework-core-9.0.1.tar.gz` & `tmp/rpaframework-core-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpaframework-core-9.0.1.tar", max compression
+gzip compressed data, was "rpaframework-core-9.1.0.tar", max compression
```

## Comparing `rpaframework-core-9.0.1.tar` & `rpaframework-core-9.1.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    11358 2021-09-09 09:55:26.356483 rpaframework-core-9.0.1/LICENSE
--rw-r--r--   0        0        0      250 2021-09-09 09:55:26.356630 rpaframework-core-9.0.1/README.rst
--rw-r--r--   0        0        0     1682 2022-06-23 13:36:54.575056 rpaframework-core-9.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-09-09 09:55:26.357660 rpaframework-core-9.0.1/src/RPA/core/__init__.py
--rw-r--r--   0        0        0      730 2021-09-09 09:55:26.357744 rpaframework-core-9.0.1/src/RPA/core/decorators.py
--rw-r--r--   0        0        0     6572 2021-09-09 09:55:26.357859 rpaframework-core-9.0.1/src/RPA/core/geometry.py
--rw-r--r--   0        0        0     3414 2022-05-25 11:29:26.054435 rpaframework-core-9.0.1/src/RPA/core/helpers.py
--rw-r--r--   0        0        0      431 2022-05-25 11:29:26.055242 rpaframework-core-9.0.1/src/RPA/core/locators/__init__.py
--rw-r--r--   0        0        0     4504 2022-05-25 11:29:26.055691 rpaframework-core-9.0.1/src/RPA/core/locators/containers.py
--rw-r--r--   0        0        0     6856 2022-05-25 11:29:26.056142 rpaframework-core-9.0.1/src/RPA/core/locators/database.py
--rw-r--r--   0        0        0     1089 2021-09-09 09:55:26.358432 rpaframework-core-9.0.1/src/RPA/core/locators/literal.py
--rw-r--r--   0        0        0     8713 2021-09-09 09:55:26.358555 rpaframework-core-9.0.1/src/RPA/core/locators/syntax.py
--rw-r--r--   0        0        0    11215 2022-05-25 11:29:26.056456 rpaframework-core-9.0.1/src/RPA/core/logger.py
--rw-r--r--   0        0        0     5190 2022-05-25 11:29:26.056710 rpaframework-core-9.0.1/src/RPA/core/notebook.py
--rw-r--r--   0        0        0      475 2021-09-09 09:55:26.358816 rpaframework-core-9.0.1/src/RPA/core/robocorp.py
--rw-r--r--   0        0        0      521 2021-09-09 09:55:26.358885 rpaframework-core-9.0.1/src/RPA/core/types.py
--rw-r--r--   0        0        0        0 2022-05-25 11:29:26.056759 rpaframework-core-9.0.1/src/RPA/core/vendor/__init__.py
--rw-r--r--   0        0        0     4922 2022-05-25 11:29:26.057109 rpaframework-core-9.0.1/src/RPA/core/vendor/deco.py
--rw-r--r--   0        0        0    10937 2022-05-25 11:29:26.057776 rpaframework-core-9.0.1/src/RPA/core/vendor/robotlibcore.py
--rw-r--r--   0        0        0     3021 2021-09-09 09:55:26.358962 rpaframework-core-9.0.1/src/RPA/core/webdriver.py
--rw-r--r--   0        0        0     1288 2022-06-23 13:37:25.204150 rpaframework-core-9.0.1/src/RPA/core/windows/__init__.py
--rw-r--r--   0        0        0     2655 2022-05-25 11:29:26.058854 rpaframework-core-9.0.1/src/RPA/core/windows/context.py
--rw-r--r--   0        0        0      464 2022-05-25 11:29:26.059288 rpaframework-core-9.0.1/src/RPA/core/windows/helpers.py
--rw-r--r--   0        0        0     4063 2022-05-25 11:29:26.059729 rpaframework-core-9.0.1/src/RPA/core/windows/inspect.py
--rw-r--r--   0        0        0    13035 2022-05-25 11:29:26.060475 rpaframework-core-9.0.1/src/RPA/core/windows/locators.py
--rw-r--r--   0        0        0     3841 2022-05-25 11:29:26.060852 rpaframework-core-9.0.1/src/RPA/core/windows/window.py
--rw-r--r--   0        0        0     1520 2022-06-23 13:40:53.080446 rpaframework-core-9.0.1/setup.py
--rw-r--r--   0        0        0     1934 2022-06-23 13:40:53.080593 rpaframework-core-9.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2021-09-09 09:55:26.356483 rpaframework-core-9.1.0/LICENSE
+-rw-r--r--   0        0        0      250 2021-09-09 09:55:26.356630 rpaframework-core-9.1.0/README.rst
+-rw-r--r--   0        0        0     1682 2022-08-02 07:52:35.154316 rpaframework-core-9.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-09-09 09:55:26.357660 rpaframework-core-9.1.0/src/RPA/core/__init__.py
+-rw-r--r--   0        0        0      730 2021-09-09 09:55:26.357744 rpaframework-core-9.1.0/src/RPA/core/decorators.py
+-rw-r--r--   0        0        0     6572 2021-09-09 09:55:26.357859 rpaframework-core-9.1.0/src/RPA/core/geometry.py
+-rw-r--r--   0        0        0     3414 2022-08-01 15:10:59.480160 rpaframework-core-9.1.0/src/RPA/core/helpers.py
+-rw-r--r--   0        0        0      431 2022-08-01 15:10:59.480297 rpaframework-core-9.1.0/src/RPA/core/locators/__init__.py
+-rw-r--r--   0        0        0     4504 2022-08-01 15:10:59.480424 rpaframework-core-9.1.0/src/RPA/core/locators/containers.py
+-rw-r--r--   0        0        0     6896 2022-08-02 07:52:35.154627 rpaframework-core-9.1.0/src/RPA/core/locators/database.py
+-rw-r--r--   0        0        0     1135 2022-08-02 07:52:35.154898 rpaframework-core-9.1.0/src/RPA/core/locators/literal.py
+-rw-r--r--   0        0        0     9013 2022-08-02 07:52:35.155155 rpaframework-core-9.1.0/src/RPA/core/locators/syntax.py
+-rw-r--r--   0        0        0    11215 2022-07-05 06:13:15.575300 rpaframework-core-9.1.0/src/RPA/core/logger.py
+-rw-r--r--   0        0        0     5190 2022-05-25 11:29:26.056710 rpaframework-core-9.1.0/src/RPA/core/notebook.py
+-rw-r--r--   0        0        0      475 2021-09-09 09:55:26.358816 rpaframework-core-9.1.0/src/RPA/core/robocorp.py
+-rw-r--r--   0        0        0      521 2021-09-09 09:55:26.358885 rpaframework-core-9.1.0/src/RPA/core/types.py
+-rw-r--r--   0        0        0        0 2022-08-01 15:10:59.480471 rpaframework-core-9.1.0/src/RPA/core/vendor/__init__.py
+-rw-r--r--   0        0        0     4922 2022-08-01 15:10:59.480548 rpaframework-core-9.1.0/src/RPA/core/vendor/deco.py
+-rw-r--r--   0        0        0    10937 2022-08-01 15:10:59.480628 rpaframework-core-9.1.0/src/RPA/core/vendor/robotlibcore.py
+-rw-r--r--   0        0        0     3021 2021-09-09 09:55:26.358962 rpaframework-core-9.1.0/src/RPA/core/webdriver.py
+-rw-r--r--   0        0        0     1288 2022-08-01 15:10:59.480785 rpaframework-core-9.1.0/src/RPA/core/windows/__init__.py
+-rw-r--r--   0        0        0     2655 2022-08-01 15:10:59.480859 rpaframework-core-9.1.0/src/RPA/core/windows/context.py
+-rw-r--r--   0        0        0      464 2022-08-01 15:10:59.480919 rpaframework-core-9.1.0/src/RPA/core/windows/helpers.py
+-rw-r--r--   0        0        0     4063 2022-08-01 15:10:59.481001 rpaframework-core-9.1.0/src/RPA/core/windows/inspect.py
+-rw-r--r--   0        0        0    13035 2022-08-01 15:10:59.481099 rpaframework-core-9.1.0/src/RPA/core/windows/locators.py
+-rw-r--r--   0        0        0     3841 2022-08-01 15:10:59.481326 rpaframework-core-9.1.0/src/RPA/core/windows/window.py
+-rw-r--r--   0        0        0     1520 2022-08-02 07:55:04.588423 rpaframework-core-9.1.0/setup.py
+-rw-r--r--   0        0        0     1934 2022-08-02 07:55:04.588649 rpaframework-core-9.1.0/PKG-INFO
```

### Comparing `rpaframework-core-9.0.1/LICENSE` & `rpaframework-core-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/pyproject.toml` & `rpaframework-core-9.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpaframework-core"
-version = "9.0.1"
+version = "9.1.0"
 description = "Core utilities used by RPA Framework"
 authors = [
 	"RPA Framework <rpafw@robocorp.com>",
 ]
 license = "Apache-2.0"
 readme = "README.rst"
```

### Comparing `rpaframework-core-9.0.1/src/RPA/core/decorators.py` & `rpaframework-core-9.1.0/src/RPA/core/decorators.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/geometry.py` & `rpaframework-core-9.1.0/src/RPA/core/geometry.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/helpers.py` & `rpaframework-core-9.1.0/src/RPA/core/helpers.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/locators/containers.py` & `rpaframework-core-9.1.0/src/RPA/core/locators/containers.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/locators/database.py` & `rpaframework-core-9.1.0/src/RPA/core/locators/database.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,29 @@
 import io
 import json
 import logging
 import os
 import re
 from contextlib import contextmanager
 from pathlib import Path
-from RPA.core.locators import Locator, BrowserLocator, ImageLocator
+from typing import Optional, Union
+
+from RPA.core.locators import BrowserLocator, ImageLocator, Locator
 
 
 @contextmanager
-def open_stream(obj, *args, **kwargs):
+def open_stream(path_or_stream, *args, encoding="utf-8", **kwargs) -> io.IOBase:
     """Wrapper for built-in open(), which allows using
     existing IO streams.
     """
-    is_open = False
-    try:
-        if not isinstance(obj, io.IOBase):
-            # pylint: disable=consider-using-with,unspecified-encoding
-            kwargs.setdefault("encoding", "utf-8")
-            obj = open(obj, *args, **kwargs)
-            is_open = True
-
-        yield obj
-    finally:
-        if is_open:
-            obj.close()
+    if not isinstance(path_or_stream, io.IOBase):
+        path_or_stream = open(path_or_stream, *args, encoding=encoding, **kwargs)
+
+    with path_or_stream:  # closes the descriptor even if it errors
+        yield path_or_stream
 
 
 def sanitize_name(name):
     """Sanitize locator name for use in filenames.
     Sanitized name should be unique in database.
 
     Examples:
@@ -56,38 +51,38 @@
 
 
 class LocatorsDatabase:
     """Container for storing locator information,
     and serializing/deserializing database file.
     """
 
-    def __init__(self, path=None):
+    def __init__(self, path: Optional[Union[str, io.IOBase]] = None):
         self.logger = logging.getLogger(__name__)
         self.path = path or self.default_path
         self.locators = {}
         self._error = None
         self._invalid = {}
 
     @classmethod
-    def load_by_name(cls, name, path=None) -> Locator:
+    def load_by_name(cls, name, path: Optional[str] = None) -> Locator:
         """Load locator entry from database with given name."""
         database = cls(path)
         database.load()
 
         if database.error:
             error_msg, error_args = database.error
             raise ValueError(error_msg % error_args)
 
         return database.resolve(name)
 
     @property
-    def default_path(self):
+    def default_path(self) -> str:
         """Return default path for locators database file."""
         dirname = os.getenv("ROBOT_ROOT", "")
-        filename = "locators.json"
+        filename = os.getenv("RPA_LOCATORS_DATABASE", "").strip() or "locators.json"
         return os.path.join(dirname, filename)
 
     @property
     def parent(self):
         """Return parent directory for database."""
         return (
             Path(self.path).parent
@@ -163,16 +158,15 @@
             data[name] = locator.to_dict()
 
         for name, fields in self._invalid.items():
             if name not in data:
                 data[name] = fields
 
         with open_stream(self.path, "w") as fd:
-            output = json.dumps(data, sort_keys=True, indent=4)
-            fd.write(output)
+            json.dump(data, fd, sort_keys=True, indent=4)
 
     def _load(self, data):
         """Load database content as Locator objects."""
         locators = {}
         invalid = {}
 
         # Migrate from old list-based file format
```

### Comparing `rpaframework-core-9.0.1/src/RPA/core/locators/literal.py` & `rpaframework-core-9.1.0/src/RPA/core/locators/literal.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,22 @@
-from typing import Union
+from typing import Optional, Union
+
 from RPA.core.locators import LocatorsDatabase, Locator, TYPES
 
+
 LocatorType = Union[str, Locator]
 
 
 def _unquote(text):
     if text.startswith('"') and text.endswith('"'):
         text = text[1:-1]
     return text
 
 
-def parse(locator: LocatorType) -> Locator:
+def parse(locator: LocatorType, path: Optional[str] = None) -> Locator:
     """Parse locator string literal into a ``Locator`` instance.
 
     For example: "image:path/to/image.png" -> ImageLocator(path="path/to/image-png")
     """
     if isinstance(locator, Locator):
         return locator
 
@@ -24,15 +26,15 @@
         raise ValueError(f"Invalid locator format: {locator}") from err
 
     if not value:
         typename, value = "alias", typename
 
     typename = typename.strip().lower()
     if typename == "alias":
-        return LocatorsDatabase.load_by_name(_unquote(value))
+        return LocatorsDatabase.load_by_name(_unquote(value), path)
     else:
         klass = TYPES.get(typename)
         if not klass:
             raise ValueError(f"Unknown locator type: {typename}")
 
         args = [_unquote(arg) for arg in value.split(",")]
         return klass(*args)
```

### Comparing `rpaframework-core-9.0.1/src/RPA/core/locators/syntax.py` & `rpaframework-core-9.1.0/src/RPA/core/locators/syntax.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import re
 from enum import Enum
-from typing import List, Union, NamedTuple
+from typing import Callable, List, NamedTuple, Optional, Union
 
 from RPA.core.geometry import Point, Region, Undefined
 from RPA.core.locators import literal, Locator
 
+
 Geometry = Union[Point, Region, Undefined]
 
 
 class InvalidSyntax(ValueError):
     """Raised when given syntax is malformed."""
 
 
@@ -132,15 +133,17 @@
         r"(?P<MISMATCH>.+)",
     ]
     # fmt: on
 
     PATTERN = re.compile("|".join(TOKEN_PATTERNS))
 
     @classmethod
-    def tokenize(cls, locator: str) -> List[TokenPair]:
+    def tokenize(
+        cls, locator: str, parser: Callable[[str], Locator]
+    ) -> List[TokenPair]:
         """Convert locator string to list of token pairs."""
         scanner = cls.PATTERN.scanner(locator)
 
         tokens = []
         for match in iter(scanner.match, None):
             name = match.lastgroup
             value = match.group()
@@ -148,15 +151,15 @@
             if name == "MISMATCH":
                 raise InvalidSyntax(f"Unknown token: '{value}'")
 
             if name == "SKIP":
                 continue
 
             if name == "LOCATOR":
-                value = literal.parse(value)
+                value = parser(value)
 
             pair = TokenPair(Token[name], value)
             tokens.append(pair)
 
         if not tokens:
             raise InvalidSyntax("Empty expression")
 
@@ -165,17 +168,17 @@
 
 class SyntaxParser:
     """Methods for parsing a locator string into a tree."""
 
     def __init__(self):
         self.tokens = Peekable([])
 
-    def parse(self, locator: str) -> ValueType:
+    def parse(self, locator: str, parser: Callable[[str], Locator]) -> ValueType:
         """Parse locator string to tokenized expression."""
-        pairs = Tokenizer.tokenize(locator)
+        pairs = Tokenizer.tokenize(locator, parser)
         self.tokens = Peekable(pairs)
         return self._chain()
 
     def _chain(self) -> ValueType:
         """Chain of expressions."""
         links = [self._expression()]
         while self._accept(Token.THEN):
@@ -232,28 +235,32 @@
 
         if not self._accept(token):
             actual = self.tokens.peek.token
             raise InvalidSyntax(f"Expected '{token.value}', was '{actual.value}'")
 
 
 class Resolver:
-    """Parser for locator expressions and resolving them into a set of
-    final values."""
+    """Parser for locator expressions and resolving them into a set of final values."""
 
-    def __init__(self, finder):
+    def __init__(self, finder, database: Optional[str] = None):
         self.finder = finder
+        self.database = database
         self._stack = [Undefined()]
 
     @property
     def current(self):
         return self._stack[-1]
 
     def dispatch(self, locator: str):
         """Visit locator tree."""
-        root = SyntaxParser().parse(locator)
+
+        def from_literal(value: str) -> Locator:
+            return literal.parse(value, self.database)
+
+        root = SyntaxParser().parse(locator=locator, parser=from_literal)
         return sorted(self._resolve(root))
 
     def _resolve(self, value: Union[ValueType, bool]):
         """Resolve value of any type."""
         resolvers = {
             Locator: self._locator,
             Not: self._not,
```

### Comparing `rpaframework-core-9.0.1/src/RPA/core/logger.py` & `rpaframework-core-9.1.0/src/RPA/core/logger.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/notebook.py` & `rpaframework-core-9.1.0/src/RPA/core/notebook.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/types.py` & `rpaframework-core-9.1.0/src/RPA/core/types.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/vendor/deco.py` & `rpaframework-core-9.1.0/src/RPA/core/vendor/deco.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/vendor/robotlibcore.py` & `rpaframework-core-9.1.0/src/RPA/core/vendor/robotlibcore.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/webdriver.py` & `rpaframework-core-9.1.0/src/RPA/core/webdriver.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/windows/__init__.py` & `rpaframework-core-9.1.0/src/RPA/core/windows/__init__.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/windows/context.py` & `rpaframework-core-9.1.0/src/RPA/core/windows/context.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/windows/inspect.py` & `rpaframework-core-9.1.0/src/RPA/core/windows/inspect.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/windows/locators.py` & `rpaframework-core-9.1.0/src/RPA/core/windows/locators.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/src/RPA/core/windows/window.py` & `rpaframework-core-9.1.0/src/RPA/core/windows/window.py`

 * *Files identical despite different names*

### Comparing `rpaframework-core-9.0.1/setup.py` & `rpaframework-core-9.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 extras_require = \
 {':python_full_version < "3.7.6" and sys_platform == "win32" or python_full_version > "3.7.6" and python_full_version < "3.8.1" and sys_platform == "win32" or python_full_version > "3.8.1" and sys_platform == "win32"': ['pywin32>=300,<304'],
  ':sys_platform == "win32"': ['psutil>=5.9.0,<6.0.0',
                               'uiautomation>=2.0.15,<3.0.0']}
 
 setup_kwargs = {
     'name': 'rpaframework-core',
-    'version': '9.0.1',
+    'version': '9.1.0',
     'description': 'Core utilities used by RPA Framework',
     'long_description': 'rpaframework-core\n=================\n\nThis package is a set of core functionality and utilities used\nby `RPA Framework`_. It is not intended to be installed directly, but\nas a dependency to other projects.\n\n.. _RPA Framework: https://rpaframework.org\n',
     'author': 'RPA Framework',
     'author_email': 'rpafw@robocorp.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://rpaframework.org/',
```

### Comparing `rpaframework-core-9.0.1/PKG-INFO` & `rpaframework-core-9.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpaframework-core
-Version: 9.0.1
+Version: 9.1.0
 Summary: Core utilities used by RPA Framework
 Home-page: https://rpaframework.org/
 License: Apache-2.0
 Keywords: robotframework,rpa,automation
 Author: RPA Framework
 Author-email: rpafw@robocorp.com
 Requires-Python: >=3.7,<4.0
```


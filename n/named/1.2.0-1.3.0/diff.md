# Comparing `tmp/named-1.2.0.tar.gz` & `tmp/named-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "named-1.2.0.tar", max compression
+gzip compressed data, was "named-1.3.0.tar", max compression
```

## Comparing `named-1.2.0.tar` & `named-1.3.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1092 2023-05-23 21:52:52.063806 named-1.2.0/LICENSE
--rw-r--r--   0        0        0     3056 2023-05-23 21:52:52.063806 named-1.2.0/README.md
--rw-r--r--   0        0        0     1242 2023-05-23 21:52:52.063806 named-1.2.0/named/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 21:52:52.063806 named-1.2.0/named/py.typed
--rw-r--r--   0        0        0     2646 2023-05-23 21:52:52.063806 named-1.2.0/named/typing.py
--rw-r--r--   0        0        0     3099 2023-05-23 21:52:52.063806 named-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 named-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-29 20:07:48.462711 named-1.3.0/LICENSE
+-rw-r--r--   0        0        0     3056 2023-05-29 20:07:48.462711 named-1.3.0/README.md
+-rw-r--r--   0        0        0     1388 2023-05-29 20:07:48.462711 named-1.3.0/named/__init__.py
+-rw-r--r--   0        0        0     3802 2023-05-29 20:07:48.462711 named-1.3.0/named/core.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:07:48.462711 named-1.3.0/named/py.typed
+-rw-r--r--   0        0        0     3099 2023-05-29 20:07:48.462711 named-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4176 1970-01-01 00:00:00.000000 named-1.3.0/PKG-INFO
```

### Comparing `named-1.2.0/LICENSE` & `named-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `named-1.2.0/README.md` & `named-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 $ poetry add named
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-named = "^1.2.0"
+named = "^1.3.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.named]
 git = "https://github.com/nekitdev/named.git"
```

### Comparing `named-1.2.0/named/__init__.py` & `named-1.3.0/named/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,40 +19,48 @@
 
 __description__ = "Named types."
 __url__ = "https://github.com/nekitdev/named"
 
 __title__ = "named"
 __author__ = "nekitdev"
 __license__ = "MIT"
-__version__ = "1.2.0"
+__version__ = "1.3.0"
 
-from named.typing import (
+from named.core import (
     MODULE,
     NAME,
     Moduled,
     Named,
     get_module,
     get_name,
     get_type_module,
     get_type_name,
     has_module,
     has_name,
     is_moduled,
     is_named,
+    set_module,
+    set_name,
+    set_type_module,
+    set_type_name,
 )
 
 __all__ = (
     # named
     "NAME",
     "Named",
     "get_name",
     "get_type_name",
     "has_name",
     "is_named",
+    "set_name",
+    "set_type_name",
     # moduled
     "MODULE",
     "Moduled",
     "get_module",
     "get_type_module",
     "has_module",
     "is_moduled",
+    "set_module",
+    "set_type_module",
 )
```

### Comparing `named-1.2.0/pyproject.toml` & `named-1.3.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "named"
-version = "1.2.0"
+version = "1.3.0"
 description = "Named types."
 authors = ["nekitdev"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/nekitdev/named"
@@ -131,15 +131,15 @@
 warn_unreachable = true
 
 warn_redundant_casts = true
 warn_unused_ignores = false  # compatibility
 
 [tool.changelogging]
 name = "named"
-version = "1.2.0"
+version = "1.3.0"
 url = "https://github.com/nekitdev/named"
 directory = "changes"
 output = "CHANGELOG.md"
 
 start_string = "<!-- changelogging: start -->"
 
 title_format = "{version} ({date})"
```

### Comparing `named-1.2.0/PKG-INFO` & `named-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: named
-Version: 1.2.0
+Version: 1.3.0
 Summary: Named types.
 Home-page: https://github.com/nekitdev/named
 License: MIT
 Keywords: python,named,name
 Author: nekitdev
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
@@ -69,15 +69,15 @@
 $ poetry add named
 ```
 
 Or by directly specifying it in the configuration like so:
 
 ```toml
 [tool.poetry.dependencies]
-named = "^1.2.0"
+named = "^1.3.0"
 ```
 
 Alternatively, you can add it directly from the source:
 
 ```toml
 [tool.poetry.dependencies.named]
 git = "https://github.com/nekitdev/named.git"
```


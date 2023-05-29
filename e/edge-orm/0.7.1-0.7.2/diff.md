# Comparing `tmp/edge_orm-0.7.1.tar.gz` & `tmp/edge_orm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_orm-0.7.1.tar", max compression
+gzip compressed data, was "edge_orm-0.7.2.tar", max compression
```

## Comparing `edge_orm-0.7.1.tar` & `edge_orm-0.7.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.7.1/README.md
--rw-r--r--   0        0        0      806 2023-04-19 18:28:11.434516 edge_orm-0.7.1/edge_orm/__init__.py
--rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.7.1/edge_orm/cache.py
--rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.7.1/edge_orm/errors.py
--rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.7.1/edge_orm/execute.py
--rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.7.1/edge_orm/external/encoders.py
--rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.7.1/edge_orm/helpers.py
--rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.7.1/edge_orm/logs.py
--rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.7.1/edge_orm/node/__init__.py
--rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.7.1/edge_orm/node/errors.py
--rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.7.1/edge_orm/node/models.py
--rw-r--r--   0        0        0      287 2023-04-19 17:57:56.361008 edge_orm-0.7.1/edge_orm/resolver/__init__.py
--rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.7.1/edge_orm/resolver/enums.py
--rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.7.1/edge_orm/resolver/errors.py
--rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.7.1/edge_orm/resolver/merging.py
--rw-r--r--   0        0        0    42191 2023-05-26 15:20:53.123981 edge_orm-0.7.1/edge_orm/resolver/model.py
--rw-r--r--   0        0        0     5300 2023-05-26 15:22:47.425858 edge_orm-0.7.1/edge_orm/resolver/nested_resolvers.py
--rw-r--r--   0        0        0     3711 2023-04-13 17:11:22.267717 edge_orm-0.7.1/edge_orm/resolver/utils.py
--rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.7.1/edge_orm/span.py
--rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.7.1/edge_orm/types_generator/__init__.py
--rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.7.1/edge_orm/types_generator/introspection.py
--rw-r--r--   0        0        0    39663 2023-04-13 18:56:59.500577 edge_orm-0.7.1/edge_orm/types_generator/main.py
--rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.7.1/edge_orm/unset.py
--rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.7.1/edge_orm/validators.py
--rw-r--r--   0        0        0      785 2023-05-26 15:24:33.886688 edge_orm-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2023-02-08 20:21:01.345400 edge_orm-0.7.2/README.md
+-rw-r--r--   0        0        0      806 2023-04-19 18:28:11.434516 edge_orm-0.7.2/edge_orm/__init__.py
+-rw-r--r--   0        0        0     1729 2023-02-08 20:21:01.355224 edge_orm-0.7.2/edge_orm/cache.py
+-rw-r--r--   0        0        0      108 2023-02-08 20:21:01.355283 edge_orm-0.7.2/edge_orm/errors.py
+-rw-r--r--   0        0        0     2191 2023-02-08 20:21:01.355352 edge_orm-0.7.2/edge_orm/execute.py
+-rw-r--r--   0        0        0     5446 2023-02-08 20:21:01.355464 edge_orm-0.7.2/edge_orm/external/encoders.py
+-rw-r--r--   0        0        0     1036 2023-02-08 20:21:01.355536 edge_orm-0.7.2/edge_orm/helpers.py
+-rw-r--r--   0        0        0     2194 2023-02-08 20:21:01.355611 edge_orm-0.7.2/edge_orm/logs.py
+-rw-r--r--   0        0        0      302 2023-02-08 20:21:01.355706 edge_orm-0.7.2/edge_orm/node/__init__.py
+-rw-r--r--   0        0        0       41 2023-02-08 20:21:01.355784 edge_orm-0.7.2/edge_orm/node/errors.py
+-rw-r--r--   0        0        0     4533 2023-03-03 19:12:38.252561 edge_orm-0.7.2/edge_orm/node/models.py
+-rw-r--r--   0        0        0      287 2023-04-19 17:57:56.361008 edge_orm-0.7.2/edge_orm/resolver/__init__.py
+-rw-r--r--   0        0        0      180 2023-02-08 20:21:01.356047 edge_orm-0.7.2/edge_orm/resolver/enums.py
+-rw-r--r--   0        0        0      135 2023-02-27 21:40:59.506123 edge_orm-0.7.2/edge_orm/resolver/errors.py
+-rw-r--r--   0        0        0     5270 2023-02-08 20:21:01.356166 edge_orm-0.7.2/edge_orm/resolver/merging.py
+-rw-r--r--   0        0        0    42200 2023-05-29 17:49:40.834437 edge_orm-0.7.2/edge_orm/resolver/model.py
+-rw-r--r--   0        0        0     5300 2023-05-26 15:22:47.425858 edge_orm-0.7.2/edge_orm/resolver/nested_resolvers.py
+-rw-r--r--   0        0        0     3711 2023-04-13 17:11:22.267717 edge_orm-0.7.2/edge_orm/resolver/utils.py
+-rw-r--r--   0        0        0      957 2023-02-08 20:21:01.356588 edge_orm-0.7.2/edge_orm/span.py
+-rw-r--r--   0        0        0      251 2023-02-08 20:21:01.356691 edge_orm-0.7.2/edge_orm/types_generator/__init__.py
+-rw-r--r--   0        0        0     8120 2023-04-04 16:56:52.369943 edge_orm-0.7.2/edge_orm/types_generator/introspection.py
+-rw-r--r--   0        0        0    39663 2023-04-13 18:56:59.500577 edge_orm-0.7.2/edge_orm/types_generator/main.py
+-rw-r--r--   0        0        0      791 2023-02-08 20:21:01.357019 edge_orm-0.7.2/edge_orm/unset.py
+-rw-r--r--   0        0        0     1381 2023-04-05 02:25:36.630393 edge_orm-0.7.2/edge_orm/validators.py
+-rw-r--r--   0        0        0      785 2023-05-29 17:48:35.504338 edge_orm-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 edge_orm-0.7.2/PKG-INFO
```

### Comparing `edge_orm-0.7.1/edge_orm/__init__.py` & `edge_orm-0.7.2/edge_orm/__init__.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/cache.py` & `edge_orm-0.7.2/edge_orm/cache.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/execute.py` & `edge_orm-0.7.2/edge_orm/execute.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/external/encoders.py` & `edge_orm-0.7.2/edge_orm/external/encoders.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/helpers.py` & `edge_orm-0.7.2/edge_orm/helpers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/logs.py` & `edge_orm-0.7.2/edge_orm/logs.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/node/models.py` & `edge_orm-0.7.2/edge_orm/node/models.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/resolver/merging.py` & `edge_orm-0.7.2/edge_orm/resolver/merging.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/resolver/model.py` & `edge_orm-0.7.2/edge_orm/resolver/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,15 @@
         if not self._filter:
             return ""
         return f"FILTER {self._filter}"
 
     def _order_by_str(self) -> str:
         if not self._order_by:
             return ""
-        return f"ORDER BY {self._order_by}"
+        return f"ORDER BY {self._order_by} THEN .id"
 
     def _limit_str(self) -> str:
         if not self._limit or self._limit == 0:
             return ""
         return f"LIMIT {self._limit}"
 
     def _offset_str(self) -> str:
```

### Comparing `edge_orm-0.7.1/edge_orm/resolver/nested_resolvers.py` & `edge_orm-0.7.2/edge_orm/resolver/nested_resolvers.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/resolver/utils.py` & `edge_orm-0.7.2/edge_orm/resolver/utils.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/span.py` & `edge_orm-0.7.2/edge_orm/span.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/types_generator/introspection.py` & `edge_orm-0.7.2/edge_orm/types_generator/introspection.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/types_generator/main.py` & `edge_orm-0.7.2/edge_orm/types_generator/main.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/unset.py` & `edge_orm-0.7.2/edge_orm/unset.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/edge_orm/validators.py` & `edge_orm-0.7.2/edge_orm/validators.py`

 * *Files identical despite different names*

### Comparing `edge_orm-0.7.1/pyproject.toml` & `edge_orm-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edge-orm"
-version = "0.7.1"
+version = "0.7.2"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = "edge_orm" }]
 exclude = ["tests/**/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `edge_orm-0.7.1/PKG-INFO` & `edge_orm-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-orm
-Version: 0.7.1
+Version: 0.7.2
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
```


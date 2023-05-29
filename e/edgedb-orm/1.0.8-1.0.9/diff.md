# Comparing `tmp/edgedb_orm-1.0.8.tar.gz` & `tmp/edgedb_orm-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgedb_orm-1.0.8.tar", max compression
+gzip compressed data, was "edgedb_orm-1.0.9.tar", max compression
```

## Comparing `edgedb_orm-1.0.8.tar` & `edgedb_orm-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      379 2023-02-08 21:00:05.436050 edgedb_orm-1.0.8/edgedb_orm/__init__.py
--rw-r--r--   0        0        0      520 2023-02-08 21:00:05.436122 edgedb_orm-1.0.8/edgedb_orm/base_patch.py
--rw-r--r--   0        0        0     3249 2023-02-08 21:00:05.436195 edgedb_orm-1.0.8/edgedb_orm/batch.py
--rw-r--r--   0        0        0     2002 2023-02-08 21:00:05.436266 edgedb_orm-1.0.8/edgedb_orm/cache.py
--rw-r--r--   0        0        0      523 2023-02-08 21:00:05.436326 edgedb_orm-1.0.8/edgedb_orm/constants.py
--rw-r--r--   0        0        0     3504 2023-02-08 21:00:05.436398 edgedb_orm-1.0.8/edgedb_orm/creating_strings.py
--rw-r--r--   0        0        0       96 2023-02-08 21:00:05.436454 edgedb_orm-1.0.8/edgedb_orm/enums.py
--rw-r--r--   0        0        0     3249 2023-02-08 21:00:05.436528 edgedb_orm-1.0.8/edgedb_orm/execute.py
--rw-r--r--   0        0        0    31444 2023-03-06 21:24:22.439968 edgedb_orm-1.0.8/edgedb_orm/generator.py
--rw-r--r--   0        0        0     6470 2023-03-06 21:11:03.541000 edgedb_orm-1.0.8/edgedb_orm/introspection.py
--rw-r--r--   0        0        0     4073 2023-02-08 21:00:05.436868 edgedb_orm-1.0.8/edgedb_orm/nested_resolvers.py
--rw-r--r--   0        0        0    32048 2023-02-09 18:08:28.614065 edgedb_orm-1.0.8/edgedb_orm/node.py
--rw-r--r--   0        0        0    24787 2023-03-20 22:13:53.475285 edgedb_orm-1.0.8/edgedb_orm/resolver.py
--rw-r--r--   0        0        0     4999 2023-02-08 21:00:05.437298 edgedb_orm-1.0.8/edgedb_orm/resolver_helpers.py
--rw-r--r--   0        0        0      839 2023-02-08 21:00:05.437360 edgedb_orm-1.0.8/edgedb_orm/span.py
--rw-r--r--   0        0        0      646 2023-02-08 21:00:05.437416 edgedb_orm-1.0.8/edgedb_orm/unset.py
--rw-r--r--   0        0        0     1144 2023-02-08 21:00:05.437476 edgedb_orm-1.0.8/edgedb_orm/validators.py
--rw-r--r--   0        0        0      473 2023-03-20 22:14:17.783833 edgedb_orm-1.0.8/pyproject.toml
--rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 edgedb_orm-1.0.8/setup.py
--rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 edgedb_orm-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0      379 2023-02-08 21:00:05.436050 edgedb_orm-1.0.9/edgedb_orm/__init__.py
+-rw-r--r--   0        0        0      520 2023-02-08 21:00:05.436122 edgedb_orm-1.0.9/edgedb_orm/base_patch.py
+-rw-r--r--   0        0        0     3249 2023-02-08 21:00:05.436195 edgedb_orm-1.0.9/edgedb_orm/batch.py
+-rw-r--r--   0        0        0     2002 2023-02-08 21:00:05.436266 edgedb_orm-1.0.9/edgedb_orm/cache.py
+-rw-r--r--   0        0        0      523 2023-02-08 21:00:05.436326 edgedb_orm-1.0.9/edgedb_orm/constants.py
+-rw-r--r--   0        0        0     3504 2023-02-08 21:00:05.436398 edgedb_orm-1.0.9/edgedb_orm/creating_strings.py
+-rw-r--r--   0        0        0       96 2023-02-08 21:00:05.436454 edgedb_orm-1.0.9/edgedb_orm/enums.py
+-rw-r--r--   0        0        0     3249 2023-02-08 21:00:05.436528 edgedb_orm-1.0.9/edgedb_orm/execute.py
+-rw-r--r--   0        0        0    31608 2023-03-28 23:20:37.122148 edgedb_orm-1.0.9/edgedb_orm/generator.py
+-rw-r--r--   0        0        0     6470 2023-03-06 21:11:03.541000 edgedb_orm-1.0.9/edgedb_orm/introspection.py
+-rw-r--r--   0        0        0     4073 2023-02-08 21:00:05.436868 edgedb_orm-1.0.9/edgedb_orm/nested_resolvers.py
+-rw-r--r--   0        0        0    32048 2023-02-09 18:08:28.614065 edgedb_orm-1.0.9/edgedb_orm/node.py
+-rw-r--r--   0        0        0    24787 2023-03-20 22:13:53.475285 edgedb_orm-1.0.9/edgedb_orm/resolver.py
+-rw-r--r--   0        0        0     4999 2023-02-08 21:00:05.437298 edgedb_orm-1.0.9/edgedb_orm/resolver_helpers.py
+-rw-r--r--   0        0        0      839 2023-02-08 21:00:05.437360 edgedb_orm-1.0.9/edgedb_orm/span.py
+-rw-r--r--   0        0        0      646 2023-02-08 21:00:05.437416 edgedb_orm-1.0.9/edgedb_orm/unset.py
+-rw-r--r--   0        0        0     1144 2023-02-08 21:00:05.437476 edgedb_orm-1.0.9/edgedb_orm/validators.py
+-rw-r--r--   0        0        0      473 2023-03-28 23:20:47.073748 edgedb_orm-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0      675 1970-01-01 00:00:00.000000 edgedb_orm-1.0.9/setup.py
+-rw-r--r--   0        0        0      522 1970-01-01 00:00:00.000000 edgedb_orm-1.0.9/PKG-INFO
```

### Comparing `edgedb_orm-1.0.8/edgedb_orm/base_patch.py` & `edgedb_orm-1.0.9/edgedb_orm/base_patch.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/batch.py` & `edgedb_orm-1.0.9/edgedb_orm/batch.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/cache.py` & `edgedb_orm-1.0.9/edgedb_orm/cache.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/constants.py` & `edgedb_orm-1.0.9/edgedb_orm/constants.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/creating_strings.py` & `edgedb_orm-1.0.9/edgedb_orm/creating_strings.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/execute.py` & `edgedb_orm-1.0.9/edgedb_orm/execute.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/generator.py` & `edgedb_orm-1.0.9/edgedb_orm/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -709,20 +709,23 @@
                 hydrate=object_type.node_name in nodes_to_hydrate and not dehydrate,
                 dehydrate=dehydrate,
             )
         )
     update_forward_refs_inserts_str = "\n".join(
         [f"{o.node_name}Insert.update_forward_refs()" for o in object_types]
     )
+    update_forward_refs_patch_str = "\n".join(
+        [f"{o.node_name}Patch.update_forward_refs()" for o in object_types]
+    )
     update_forward_refs_nodes_str = "\n".join(
         [f"{o.node_name}.update_forward_refs()" for o in object_types]
     )
     nodes_str = "\n".join(node_strs)
     edge_resolver_map_str = "\n".join(edge_resolver_map_strs)
-    return f"{nodes_str}\n\n{update_forward_refs_inserts_str}\n\n{update_forward_refs_nodes_str}\n\n{edge_resolver_map_str}"
+    return f"{nodes_str}\n\n{update_forward_refs_inserts_str}\n\n{update_forward_refs_patch_str}\n\n{update_forward_refs_nodes_str}\n\n{edge_resolver_map_str}"
 
 
 def add_quotes_to_non_env_vars(s: str) -> str:
     if re.fullmatch(ENV_VAR_PATTERN, s) is not None:
         return s
     return f'"{s}"'
```

### Comparing `edgedb_orm-1.0.8/edgedb_orm/introspection.py` & `edgedb_orm-1.0.9/edgedb_orm/introspection.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/nested_resolvers.py` & `edgedb_orm-1.0.9/edgedb_orm/nested_resolvers.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/node.py` & `edgedb_orm-1.0.9/edgedb_orm/node.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/resolver.py` & `edgedb_orm-1.0.9/edgedb_orm/resolver.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/resolver_helpers.py` & `edgedb_orm-1.0.9/edgedb_orm/resolver_helpers.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/span.py` & `edgedb_orm-1.0.9/edgedb_orm/span.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/unset.py` & `edgedb_orm-1.0.9/edgedb_orm/unset.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/edgedb_orm/validators.py` & `edgedb_orm-1.0.9/edgedb_orm/validators.py`

 * *Files identical despite different names*

### Comparing `edgedb_orm-1.0.8/setup.py` & `edgedb_orm-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
  'edgedb>=1.2.0,<2.0.0',
  'fastapi',
  'orjson>=3.6,<4.0',
  'pydantic[email]']
 
 setup_kwargs = {
     'name': 'edgedb-orm',
-    'version': '1.0.8',
+    'version': '1.0.9',
     'description': '',
     'long_description': 'None',
     'author': 'Jeremy Berman',
     'author_email': 'jerber@sas.upenn.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `edgedb_orm-1.0.8/PKG-INFO` & `edgedb_orm-1.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgedb-orm
-Version: 1.0.8
+Version: 1.0.9
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


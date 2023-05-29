# Comparing `tmp/nornir_routeros-0.5.0.tar.gz` & `tmp/nornir_routeros-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir_routeros-0.5.0.tar", max compression
+gzip compressed data, was "nornir_routeros-0.6.0.tar", max compression
```

## Comparing `nornir_routeros-0.5.0.tar` & `nornir_routeros-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2022-11-21 05:01:18.231293 nornir_routeros-0.5.0/LICENSE
--rw-r--r--   0        0        0        0 2022-11-21 05:01:18.231293 nornir_routeros-0.5.0/nornir_routeros/__init__.py
--rw-r--r--   0        0        0        0 2022-11-21 05:01:18.231293 nornir_routeros-0.5.0/nornir_routeros/plugins/__init__.py
--rw-r--r--   0        0        0     2239 2022-11-21 05:01:18.231293 nornir_routeros-0.5.0/nornir_routeros/plugins/connections/__init__.py
--rw-r--r--   0        0        0      180 2022-11-21 05:01:18.231293 nornir_routeros-0.5.0/nornir_routeros/plugins/tasks/__init__.py
--rw-r--r--   0        0        0     1197 2022-11-21 05:01:18.231293 nornir_routeros-0.5.0/nornir_routeros/plugins/tasks/routeros_command.py
--rw-r--r--   0        0        0     3862 2022-11-21 05:01:18.231293 nornir_routeros-0.5.0/nornir_routeros/plugins/tasks/routeros_config_item.py
--rw-r--r--   0        0        0     1229 2022-11-21 05:01:18.231293 nornir_routeros-0.5.0/nornir_routeros/plugins/tasks/routeros_get.py
--rw-r--r--   0        0        0      199 2022-11-21 05:01:18.231293 nornir_routeros-0.5.0/nornir_routeros/utils.py
--rw-r--r--   0        0        0      848 2022-11-21 05:01:18.231293 nornir_routeros-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      948 1970-01-01 00:00:00.000000 nornir_routeros-0.5.0/setup.py
--rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 nornir_routeros-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/LICENSE
+-rw-r--r--   0        0        0      314 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/nornir_routeros/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/nornir_routeros/plugins/__init__.py
+-rw-r--r--   0        0        0     2239 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/nornir_routeros/plugins/connections/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/nornir_routeros/plugins/tasks/__init__.py
+-rw-r--r--   0        0        0     1197 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/nornir_routeros/plugins/tasks/routeros_command.py
+-rw-r--r--   0        0        0     4642 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/nornir_routeros/plugins/tasks/routeros_config_item.py
+-rw-r--r--   0        0        0     1229 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/nornir_routeros/plugins/tasks/routeros_get.py
+-rw-r--r--   0        0        0      199 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/nornir_routeros/utils.py
+-rw-r--r--   0        0        0      870 2023-05-29 08:42:48.025367 nornir_routeros-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 nornir_routeros-0.6.0/PKG-INFO
```

### Comparing `nornir_routeros-0.5.0/LICENSE` & `nornir_routeros-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nornir_routeros-0.5.0/nornir_routeros/plugins/connections/__init__.py` & `nornir_routeros-0.6.0/nornir_routeros/plugins/connections/__init__.py`

 * *Files identical despite different names*

### Comparing `nornir_routeros-0.5.0/nornir_routeros/plugins/tasks/routeros_command.py` & `nornir_routeros-0.6.0/nornir_routeros/plugins/tasks/routeros_command.py`

 * *Files identical despite different names*

### Comparing `nornir_routeros-0.5.0/nornir_routeros/plugins/tasks/routeros_config_item.py` & `nornir_routeros-0.6.0/nornir_routeros/plugins/tasks/routeros_config_item.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,25 +7,27 @@
 
 
 def routeros_config_item(
     task: Task,
     path: str,
     where: Dict[str, str],
     properties: Optional[Dict[str, str]] = None,
-    add_if_missing=False,
+    add_if_missing: bool = False,
+    template_property_values: bool = True,
 ) -> Result:
     """
     Configures an item.
     Property values can be templated using jinja2. Use ``host`` to access ``task.host``.
 
     Args:
         path: The path to where the item should be. Example: /ip/firewall/filter to configure firewall filters.
         where: Dictionary of properties and values to find the item.
         properties: Desired properties of the item. If ``None``, then any items matching ``where`` will be **removed**.
         add_if_missing: If an item matching the criteria in ``where`` doesn't exist then one will be created.
+        template_property_values: Use Jinja2 for property values.
 
     Returns:
         Result: A ``Result`` with ``result`` set to the item after any changes.
 
     Examples:
 
             Ensure the router hostname is set to the inventory name::
@@ -47,14 +49,31 @@
                     where={
                         "name": "www"
                     },
                     properties={
                         "disabled": "true"
                     }
                 )
+
+            Ensure a script is configured::
+
+                nr.run(
+                    task=routeros_config_item,
+                    path="/system/script",
+                    where={
+                        "name": "test"
+                    },
+                    properties={
+                        "name": "test"
+                        "source": ':log info "hello"\\r\\n:log info "world"\\r\\n'
+                    },
+                    # To preserve \\r\\n line endings:
+                    template_property_values=False
+                )
+
     """
 
     api = task.host.get_connection(CONNECTION_NAME, task.nornir.config)
 
     resource = api.get_resource(path)
     get_results = resource.get(**where)
     dry_run = task.is_dry_run()
@@ -70,22 +89,25 @@
                     resource.remove(id=i["id"])
                 diff += f"-{i}"
 
         return Result(host=task.host, changed=changed, diff=diff, result=get_results)
 
     # Holds the properties of the item
     desired_props = {}
-    for k, v in properties.items():
-        # Render the value using jinja2
-        template = Template(str(v))
-        rendered_val = template.render(host=task.host.dict())
-        if rendered_val:
-            desired_props[k] = rendered_val
-        else:
-            raise ValueError(f"Jinja2 rendered a empty value for property {k}")
+    if template_property_values:
+        for k, v in properties.items():
+            # Render the value using jinja2
+            template = Template(str(v))
+            rendered_val = template.render(host=task.host.dict())
+            if rendered_val:
+                desired_props[k] = rendered_val
+            else:
+                raise ValueError(f"Jinja2 rendered a empty value for property {k}")
+    else:
+        desired_props = properties
 
     if len(get_results) == 0 and add_if_missing:
         if dry_run:
             result = None
         else:
             result = resource.add(**desired_props)
         return Result(host=task.host, changed=True, result=result)
```

### Comparing `nornir_routeros-0.5.0/nornir_routeros/plugins/tasks/routeros_get.py` & `nornir_routeros-0.6.0/nornir_routeros/plugins/tasks/routeros_get.py`

 * *Files identical despite different names*

### Comparing `nornir_routeros-0.5.0/pyproject.toml` & `nornir_routeros-0.6.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [tool.poetry]
 name = "nornir_routeros"
-version = "0.5.0"
+version = "0.6.0"
 description = "RouterOS API plugins for nornir"
 authors = ["Devon Mar <devonm@mdmm.ca>"]
 license = "Apache-2.0"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.6"
 RouterOS-api = "^0.17.0"
 Jinja2 = "^2.11.2|^3.0"
 
 [tool.poetry.dev-dependencies]
 Sphinx = "^4.2"
-sphinx-rtd-theme = "^1.1.1"
+sphinx-rtd-theme = "^1.2.0"
 sphinx-autodoc-typehints = "^1.11.1"
 nornir = "^3.0.0"
 pytest = "^7.0.1"
 pytest-cov = "^4.0.0"
 flake8 = "^4.0.1"
 black = { version = "^22.6.0", python = "^3.7" }
 isort = { version = "^5.10.0", python = "^3.7" }
```


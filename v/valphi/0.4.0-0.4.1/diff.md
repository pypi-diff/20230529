# Comparing `tmp/valphi-0.4.0.tar.gz` & `tmp/valphi-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valphi-0.4.0.tar", max compression
+gzip compressed data, was "valphi-0.4.1.tar", max compression
```

## Comparing `valphi-0.4.0.tar` & `valphi-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1070 2022-09-22 13:08:25.021598 valphi-0.4.0/LICENSE
--rw-r--r--   0        0        0      426 2023-05-27 07:42:09.517912 valphi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-22 13:13:37.919365 valphi-0.4.0/valphi/__init__.py
--rwxr-xr-x   0        0        0       97 2022-09-22 16:30:02.808202 valphi-0.4.0/valphi/__main__.py
--rw-r--r--   0        0        0    10775 2023-05-27 06:50:25.868917 valphi-0.4.0/valphi/cli.py
--rw-r--r--   0        0        0     2266 2023-01-17 17:02:20.445653 valphi-0.4.0/valphi/contexts.py
--rw-r--r--   0        0        0    17336 2023-05-27 07:26:58.452592 valphi-0.4.0/valphi/controllers.py
--rw-r--r--   0        0        0     1899 2023-01-17 17:07:21.715958 valphi-0.4.0/valphi/models.py
--rw-r--r--   0        0        0    16153 2023-05-27 07:42:09.529912 valphi-0.4.0/valphi/networks.py
--rw-r--r--   0        0        0     5570 2023-01-17 17:02:20.453652 valphi-0.4.0/valphi/propagators.py
--rw-r--r--   0        0        0      102 2023-01-13 07:23:53.009969 valphi-0.4.0/valphi/utils.py
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 valphi-0.4.0/setup.py
--rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 valphi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2022-09-22 13:08:25.021598 valphi-0.4.1/LICENSE
+-rw-r--r--   0        0        0      426 2023-05-29 06:41:11.240341 valphi-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-22 13:13:37.919365 valphi-0.4.1/valphi/__init__.py
+-rwxr-xr-x   0        0        0       97 2022-09-22 16:30:02.808202 valphi-0.4.1/valphi/__main__.py
+-rw-r--r--   0        0        0    11003 2023-05-29 06:41:00.144477 valphi-0.4.1/valphi/cli.py
+-rw-r--r--   0        0        0     2266 2023-01-17 17:02:20.445653 valphi-0.4.1/valphi/contexts.py
+-rw-r--r--   0        0        0    17336 2023-05-27 07:26:58.452592 valphi-0.4.1/valphi/controllers.py
+-rw-r--r--   0        0        0     1899 2023-01-17 17:07:21.715958 valphi-0.4.1/valphi/models.py
+-rw-r--r--   0        0        0    16153 2023-05-27 07:42:09.529912 valphi-0.4.1/valphi/networks.py
+-rw-r--r--   0        0        0     5570 2023-01-17 17:02:20.453652 valphi-0.4.1/valphi/propagators.py
+-rw-r--r--   0        0        0      102 2023-01-13 07:23:53.009969 valphi-0.4.1/valphi/utils.py
+-rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 valphi-0.4.1/setup.py
+-rw-r--r--   0        0        0      463 1970-01-01 00:00:00.000000 valphi-0.4.1/PKG-INFO
```

### Comparing `valphi-0.4.0/LICENSE` & `valphi-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `valphi-0.4.0/valphi/cli.py` & `valphi-0.4.1/valphi/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -191,15 +191,15 @@
         graph = app_options.controller.network.network_facts.filter(when=lambda atom: atom.predicate_name == "attack").as_facts
         models = []
         for values in res:
             models.append(graph)
             models.append('\n'.join(f"eval({node},{','.join(value.split('/'))})." for node, value in values.items()))
             models.append('§')
         url += compress_object_for_url({"input": '\n'.join(models[:-1])}, suffix="")
-        url += ";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%21"
+        url += ";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%21"
         webbrowser.open(url, new=0, autoraise=True)
 
 
 @app.command(name="query")
 def command_query(
         query: Optional[str] = typer.Argument(
             None,
```

### Comparing `valphi-0.4.0/valphi/contexts.py` & `valphi-0.4.1/valphi/contexts.py`

 * *Files identical despite different names*

### Comparing `valphi-0.4.0/valphi/controllers.py` & `valphi-0.4.1/valphi/controllers.py`

 * *Files identical despite different names*

### Comparing `valphi-0.4.0/valphi/models.py` & `valphi-0.4.1/valphi/models.py`

 * *Files identical despite different names*

### Comparing `valphi-0.4.0/valphi/networks.py` & `valphi-0.4.1/valphi/networks.py`

 * *Files identical despite different names*

### Comparing `valphi-0.4.0/valphi/propagators.py` & `valphi-0.4.1/valphi/propagators.py`

 * *Files identical despite different names*

### Comparing `valphi-0.4.0/setup.py` & `valphi-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['distlib>=0.3.6,<0.4.0', 'dumbo-asp>=0.0.37,<0.0.38', 'pydot>=1.4.2,<2.0.0']
 
 setup_kwargs = {
     'name': 'valphi',
-    'version': '0.4.0',
+    'version': '0.4.1',
     'description': 'Logic programs ralying on ValPhi semantics',
     'long_description': 'None',
     'author': 'Mario Alviano',
     'author_email': 'mario.alviano@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```


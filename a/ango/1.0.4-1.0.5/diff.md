# Comparing `tmp/ango-1.0.4.tar.gz` & `tmp/ango-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ango-1.0.4.tar", last modified: Wed May 24 08:30:56 2023, max compression
+gzip compressed data, was "ango-1.0.5.tar", last modified: Wed May 24 13:28:44 2023, max compression
```

## Comparing `ango-1.0.4.tar` & `ango-1.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 08:30:56.446047 ango-1.0.4/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-24 08:30:56.446047 ango-1.0.4/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.4/README.md
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 08:30:56.446047 ango-1.0.4/ango/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.4/ango/__init__.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 08:30:56.446047 ango-1.0.4/ango/models/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.4/ango/models/__init__.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.4/ango/models/enums.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.4/ango/models/label_category.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.4/ango/plugin_logger.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     5433 2023-05-24 08:30:39.000000 ango-1.0.4/ango/plugins.py
--rw-rw-r--   0 ofk       (1000) ofk       (1000)    14425 2023-05-17 14:28:05.000000 ango-1.0.4/ango/sdk.py
-drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 08:30:56.446047 ango-1.0.4/ango.egg-info/
--rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-24 08:30:56.000000 ango-1.0.4/ango.egg-info/PKG-INFO
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-24 08:30:56.000000 ango-1.0.4/ango.egg-info/SOURCES.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-24 08:30:56.000000 ango-1.0.4/ango.egg-info/dependency_links.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-24 08:30:56.000000 ango-1.0.4/ango.egg-info/requires.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-24 08:30:56.000000 ango-1.0.4/ango.egg-info/top_level.txt
--rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-24 08:30:56.446047 ango-1.0.4/setup.cfg
--rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-24 08:30:39.000000 ango-1.0.4/setup.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 13:28:44.399697 ango-1.0.5/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-24 13:28:44.399697 ango-1.0.5/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1305 2023-01-23 13:16:24.000000 ango-1.0.5/README.md
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 13:28:44.399697 ango-1.0.5/ango/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.5/ango/__init__.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 13:28:44.399697 ango-1.0.5/ango/models/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        0 2023-01-23 13:16:24.000000 ango-1.0.5/ango/models/__init__.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       93 2023-03-08 06:39:17.000000 ango-1.0.5/ango/models/enums.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5421 2023-01-23 13:16:24.000000 ango-1.0.5/ango/models/label_category.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1304 2023-02-08 11:40:21.000000 ango-1.0.5/ango/plugin_logger.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     5434 2023-05-24 13:28:41.000000 ango-1.0.5/ango/plugins.py
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)    14425 2023-05-17 14:28:05.000000 ango-1.0.5/ango/sdk.py
+drwxrwxr-x   0 ofk       (1000) ofk       (1000)        0 2023-05-24 13:28:44.399697 ango-1.0.5/ango.egg-info/
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)     1644 2023-05-24 13:28:44.000000 ango-1.0.5/ango.egg-info/PKG-INFO
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      299 2023-05-24 13:28:44.000000 ango-1.0.5/ango.egg-info/SOURCES.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        1 2023-05-24 13:28:44.000000 ango-1.0.5/ango.egg-info/dependency_links.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      130 2023-05-24 13:28:44.000000 ango-1.0.5/ango.egg-info/requires.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)        5 2023-05-24 13:28:44.000000 ango-1.0.5/ango.egg-info/top_level.txt
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)       38 2023-05-24 13:28:44.399697 ango-1.0.5/setup.cfg
+-rw-rw-r--   0 ofk       (1000) ofk       (1000)      864 2023-05-24 13:28:41.000000 ango-1.0.5/setup.py
```

### Comparing `ango-1.0.4/PKG-INFO` & `ango-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.4
+Version: 1.0.5
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.4/README.md` & `ango-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ango-1.0.4/ango/models/label_category.py` & `ango-1.0.5/ango/models/label_category.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.4/ango/plugin_logger.py` & `ango-1.0.5/ango/plugin_logger.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.4/ango/plugins.py` & `ango-1.0.5/ango/plugins.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         logger = PluginLogger("logger", self.id, org_id, run_by, session, self)
         return logger
 
 
 class ExportPlugin(Plugin):
 
     def __init__(self, id: str, secret: str, callback: Callable[[str, dict], Tuple[str, BytesIO]],
-                 host="https://imeritapi.ango.ai"):
+                 host="https://imerit.ango.ai"):
         super().__init__(id, secret, callback)
         self.host = host
 
     def on_plugin(self, data):
         """
         :param data: {project_id: str, assignees: List[str] = None, completed_at: List[datetime.datetime] = None,
                updated_at: List[datetime.datetime = None, tags: List[str] = None}
@@ -136,15 +136,15 @@
 
 
 class MarkdownPlugin(Plugin):
     def __init__(self, id: str, secret: str, callback: Callable):
         super().__init__(id, secret, callback)
 
 
-def run(plugin, host="https://imeritapi.ango.ai"):
+def run(plugin, host="https://plugin.imerit.ango.ai"):
     sio = socketio.Client()
     sio.register_namespace(plugin)
     sio.connect(host, namespaces=["/plugin"], wait_timeout=100)
     try:
         asyncio.get_event_loop().run_forever()
     except (KeyboardInterrupt, SystemExit):
         logging.getLogger().warning("Plugin Stopped")
```

### Comparing `ango-1.0.4/ango/sdk.py` & `ango-1.0.5/ango/sdk.py`

 * *Files identical despite different names*

### Comparing `ango-1.0.4/ango.egg-info/PKG-INFO` & `ango-1.0.5/ango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ango
-Version: 1.0.4
+Version: 1.0.5
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: ango,ango-hub,ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ango-1.0.4/setup.py` & `ango-1.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="ango",
-    version="1.0.4",
+    version="1.0.5",
     author="Faruk Karakaya",
     author_email="<faruk@ango.ai>",
     description="Ango-Hub SDK",
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
```


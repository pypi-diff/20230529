# Comparing `tmp/udc-0.2.3.tar.gz` & `tmp/udc-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udc-0.2.3.tar", max compression
+gzip compressed data, was "udc-0.2.4.tar", max compression
```

## Comparing `udc-0.2.3.tar` & `udc-0.2.4.tar`

### file list

```diff
@@ -1,21 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.2.3/LICENSE
--rw-r--r--   0        0        0     2527 2023-05-25 04:58:47.601734 udc-0.2.3/README.md
--rw-r--r--   0        0        0      749 2023-05-25 13:21:33.247471 udc-0.2.3/pyproject.toml
--rw-r--r--   0        0        0      348 2023-05-25 13:21:33.249661 udc-0.2.3/udc/__init__.py
--rw-r--r--   0        0        0      340 2023-05-25 04:58:47.604193 udc-0.2.3/udc/benchling/__init__.py
--rw-r--r--   0        0        0     1231 2023-05-25 13:21:33.250416 udc-0.2.3/udc/benchling/entry.py
--rw-r--r--   0        0        0     1394 2023-05-25 13:21:33.251547 udc-0.2.3/udc/benchling/resource.py
--rw-r--r--   0        0        0     2261 2023-05-25 13:21:33.252248 udc-0.2.3/udc/benchling/root.py
--rw-r--r--   0        0        0      356 2023-05-25 13:21:33.253153 udc-0.2.3/udc/benchling/schema.py
--rw-r--r--   0        0        0      352 2023-05-25 13:21:33.253689 udc-0.2.3/udc/benchling/sequence.py
--rw-r--r--   0        0        0     5713 2023-05-24 21:56:51.803927 udc-0.2.3/udc/config.py
--rw-r--r--   0        0        0      716 2023-05-24 00:02:24.971861 udc-0.2.3/udc/ignore.py
--rw-r--r--   0        0        0      331 2023-05-25 04:20:16.308186 udc-0.2.3/udc/main.py
--rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.2.3/udc/quilt/__init__.py
--rw-r--r--   0        0        0      135 2023-05-25 13:21:33.254424 udc-0.2.3/udc/quilt/resource.py
--rw-r--r--   0        0        0      467 2023-05-24 21:56:51.804905 udc-0.2.3/udc/types.py
--rw-r--r--   0        0        0     2502 2023-05-25 04:58:47.606836 udc-0.2.3/udc/un/cli.yaml
--rw-r--r--   0        0        0     3465 2023-05-25 13:21:33.255166 udc-0.2.3/udc/un/un_cli.py
--rw-r--r--   0        0        0     1265 2023-05-25 13:21:33.255738 udc-0.2.3/udc/un/un_uri.py
--rw-r--r--   0        0        0     2125 2023-05-24 21:56:51.806086 udc-0.2.3/udc/un/un_yaml.py
--rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 udc-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.2.4/LICENSE
+-rw-r--r--   0        0        0     2527 2023-05-25 04:58:47.601734 udc-0.2.4/README.md
+-rw-r--r--   0        0        0      749 2023-05-29 18:14:04.322921 udc-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0      260 2023-05-30 01:15:44.000000 udc-0.2.4/udc/__init__.py
+-rw-r--r--   0        0        0      340 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/__init__.py
+-rw-r--r--   0        0        0     1248 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/entry.py
+-rw-r--r--   0        0        0     1483 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/resource.py
+-rw-r--r--   0        0        0     2257 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/root.py
+-rw-r--r--   0        0        0      357 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/schema.py
+-rw-r--r--   0        0        0      353 2023-05-30 01:15:44.000000 udc-0.2.4/udc/benchling/sequence.py
+-rw-r--r--   0        0        0      331 2023-05-25 04:20:16.308186 udc-0.2.4/udc/main.py
+-rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.2.4/udc/quilt/__init__.py
+-rw-r--r--   0        0        0      275 2023-05-30 01:15:46.000000 udc-0.2.4/udc/quilt/resource.py
+-rw-r--r--   0        0        0      467 2023-05-24 21:56:51.804905 udc-0.2.4/udc/types.py
+-rw-r--r--   0        0        0     2502 2023-05-25 04:58:47.606836 udc-0.2.4/udc/un/cli.yaml
+-rw-r--r--   0        0        0     3494 2023-05-30 01:15:46.000000 udc-0.2.4/udc/un/un_cli.py
+-rw-r--r--   0        0        0     1265 2023-05-25 13:21:33.255738 udc-0.2.4/udc/un/un_uri.py
+-rw-r--r--   0        0        0     2135 2023-05-30 01:24:50.000000 udc-0.2.4/udc/un/un_yaml.py
+-rw-r--r--   0        0        0     3242 1970-01-01 00:00:00.000000 udc-0.2.4/PKG-INFO
```

### Comparing `udc-0.2.3/LICENSE` & `udc-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `udc-0.2.3/README.md` & `udc-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `udc-0.2.3/pyproject.toml` & `udc-0.2.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "udc"
-version = "0.2.3"
+version = "0.2.4"
 description = ""
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 anyio = "^3.6.2"
```

### Comparing `udc-0.2.3/udc/benchling/entry.py` & `udc-0.2.4/udc/benchling/entry.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-from .root import BenchlingRoot, BenchlingById
+from .root import BenchlingById, BenchlingRoot
+
 
 class BenchlingEntryList(BenchlingById):
     def __init__(self, attrs: dict) -> None:
         super().__init__(attrs)
 
     def pages(self):
         return BenchlingRoot.CLIENT.entries.list_entries()
-    
+
+
 class BenchlingEntry(BenchlingRoot):
     def __init__(self, attrs: dict) -> None:
         super().__init__(attrs)
 
     def fetch(self):
         self.entry = BenchlingRoot.CLIENT.entries.get_entry_by_id(self.id)
         self.schema = self.entry.schema.id
         self.children = {
             "authors": [author.id for author in self.entry.authors],
-            "custom_fields": [self.qoute(key) for key in self.entry.custom_fields.additional_keys],
+            "custom_fields": [
+                self.qoute(key) for key in self.entry.custom_fields.additional_keys
+            ],
             "days": [day.date for day in self.entry.days],
             "fields": [self.quote(key) for key in self.entry.fields.additional_keys],
         }
 
     def wrap(self, id, sub_type):
-        item_dict = {'id': id, sub_type: id}
+        item_dict = {"id": id, sub_type: id}
         item = type(f"wrap_{sub_type}", (object,), item_dict)
         return self.item_uri(item, sub_type)
 
     async def list(self) -> list[str]:
         self.fetch()
         kids = self.children
-        return [self.wrap(id, sub_type) for sub_type in kids for id in kids[sub_type]]           
+        return [self.wrap(id, sub_type) for sub_type in kids for id in kids[sub_type]]
```

### Comparing `udc-0.2.3/udc/benchling/root.py` & `udc-0.2.4/udc/benchling/root.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-import os
 import logging
+import os
 import urllib.parse
 
 from benchling_sdk.auth.api_key_auth import ApiKeyAuth
 from benchling_sdk.benchling import Benchling
 
 BENCH_ID = "id"
 BENCH_TYPE = "type"
@@ -22,18 +22,18 @@
         self.attrs = attrs
         self.uri = attrs.get("_uri")
         self.id = attrs.get(BENCH_ID)
         self.set_type(attrs.get(BENCH_TYPE))
 
     def __repr__(self) -> str:
         return f"<{self.__class__}({self.uri})>"
-    
+
     def set_type(self, btype: str):
         type = btype or BENCH_TYPE_DEFAULT
-        types = type.split('.')
+        types = type.split(".")
         self.type = types[0]
         self.sub_type = types[1] if len(types) > 1 else None
 
     def quote(self, value: str) -> str:
         return urllib.parse.quote_plus(value)
 
     def pages(self) -> list:
@@ -46,24 +46,24 @@
         type = f"{self.type}.{sub_type}" if sub_type else self.type
         base = f"benchling+https://{BenchlingRoot.BENCH_TENANT}#type={type}"
         base += f"&id={self.id}" if self.id else ""
         return base
 
     def item_uri(self, item, sub_type=None) -> str:
         base = self.base_uri(sub_type)
-        logging.debug(f'item_uri.base: {base}')
-        if hasattr(item, 'id'):
+        logging.debug(f"item_uri.base: {base}")
+        if hasattr(item, "id"):
             if "&id=" not in base:
                 base += f"&id={item.id}"
         if sub_type and hasattr(item, sub_type):
             base += f"&{sub_type}={getattr(item, sub_type)}"
-        logging.debug(f'item_uri.uri: {base}')
+        logging.debug(f"item_uri.uri: {base}")
         return base
 
     async def list(self) -> list[str]:
         return [self.item_uri(item) for item in self.items()]
 
-class BenchlingById(BenchlingRoot):
 
+class BenchlingById(BenchlingRoot):
     def __init__(self, attrs: dict) -> None:
         super().__init__(attrs)
         self.id = attrs.get(BENCH_ID)
```

### Comparing `udc-0.2.3/udc/un/cli.yaml` & `udc-0.2.4/udc/un/cli.yaml`

 * *Files identical despite different names*

### Comparing `udc-0.2.3/udc/un/un_cli.py` & `udc-0.2.4/udc/un/un_cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from argparse import ArgumentParser, Namespace
 from collections.abc import Sequence
 from importlib.metadata import version
 from sys import stdout
 
-__version__ = version('udc')
+__version__ = version("udc")
 
 from ..types import Listable
 from .un_uri import UnUri
 from .un_yaml import UnYaml
 
 
 class UnCli(UnYaml):
@@ -24,27 +24,30 @@
 
     def cmd_opts(self, cmd: str) -> dict:
         result = self.cmds[cmd]
         result["name"] = cmd
         return result
 
     def parse_version(self, parser: ArgumentParser) -> None:
-        __version__ = version('udc')
+        __version__ = version("udc")
         parser.add_argument(
-            "-v", "--version",
-            action='store_const',
+            "-v",
+            "--version",
+            action="store_const",
             const=f"{self.info('doc')} {__version__}",
             help="Show version and exit.",
         )
+
     def make_parser(self) -> ArgumentParser:
         parser = ArgumentParser(self.get("doc"))
         self.parse_version(parser)
         subparsers = parser.add_subparsers(dest="command")
         for cmd, opts in self.cmds.items():
-            if cmd != "list": continue
+            if cmd != "list":
+                continue
             subparser = subparsers.add_parser(cmd, help=opts["help"])
             args = opts.get("arguments")
             for arg in args or []:
                 subparser.add_argument(arg["name"], help=arg["help"])
         return parser
 
     async def run(self, argv: Sequence[str] = None, out=stdout):
```

### Comparing `udc-0.2.3/udc/un/un_uri.py` & `udc-0.2.4/udc/un/un_uri.py`

 * *Files identical despite different names*

### Comparing `udc-0.2.3/udc/un/un_yaml.py` & `udc-0.2.4/udc/un/un_yaml.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import importlib
+from importlib import import_module, resources
 
 from yaml import safe_load
 
 
 class UnYaml:
     KEY = "_yaml"
     SEP = "/"
     PREFIX = "#/"
     REF = "$ref"
     REF_ERROR = f"Value for Key {REF} does not start with {PREFIX}"
 
     @staticmethod
     def load_yaml(filename: str, pkg: str, sub: str = None):
-        yaml_dir = importlib.resources.files(pkg)
+        yaml_dir = resources.files(pkg)
         if sub:
             yaml_dir = yaml_dir / sub
         yaml_file = yaml_dir / filename
         yaml_string = yaml_file.read_text()
         yaml_data = safe_load(yaml_string)
         return yaml_data
 
@@ -63,9 +63,9 @@
 
     def get_handler(self, key: str) -> object:
         handlers = self.info("handlers")
         handler = handlers.get(key)
         if not handler:
             raise ValueError(f"UnYaml.get_handler: no handler for {key}")
 
-        module = importlib.import_module(handler["module"])
+        module = import_module(handler["module"])
         return getattr(module, handler["method"])
```

### Comparing `udc-0.2.3/PKG-INFO` & `udc-0.2.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udc
-Version: 0.2.3
+Version: 0.2.4
 Summary: 
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


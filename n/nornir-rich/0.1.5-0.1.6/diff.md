# Comparing `tmp/nornir-rich-0.1.5.tar.gz` & `tmp/nornir_rich-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nornir-rich-0.1.5.tar", max compression
+gzip compressed data, was "nornir_rich-0.1.6.tar", max compression
```

## Comparing `nornir-rich-0.1.5.tar` & `nornir_rich-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1374 2022-10-02 09:28:52.553464 nornir-rich-0.1.5/README.md
--rw-r--r--   0        0        0       39 2022-10-02 09:28:37.160274 nornir-rich-0.1.5/nornir_rich/__init__.py
--rw-r--r--   0        0        0     9325 2022-10-02 09:28:37.160274 nornir-rich-0.1.5/nornir_rich/functions.py
--rw-r--r--   0        0        0        0 2022-10-02 09:28:37.160274 nornir-rich-0.1.5/nornir_rich/processor.py
--rw-r--r--   0        0        0     4097 2022-10-02 09:28:37.160274 nornir-rich-0.1.5/nornir_rich/progress_bar.py
--rw-r--r--   0        0        0     1322 2022-10-02 09:28:37.160274 nornir-rich-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2149 1970-01-01 00:00:00.000000 nornir-rich-0.1.5/setup.py
--rw-r--r--   0        0        0     2361 1970-01-01 00:00:00.000000 nornir-rich-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1374 2023-05-29 18:53:26.991804 nornir_rich-0.1.6/README.md
+-rw-r--r--   0        0        0       39 2023-05-29 18:53:07.703822 nornir_rich-0.1.6/nornir_rich/__init__.py
+-rw-r--r--   0        0        0    11518 2023-05-29 18:53:07.703822 nornir_rich-0.1.6/nornir_rich/functions.py
+-rw-r--r--   0        0        0        0 2023-05-29 18:53:07.703822 nornir_rich-0.1.6/nornir_rich/processor.py
+-rw-r--r--   0        0        0     4097 2023-05-29 18:53:07.703822 nornir_rich-0.1.6/nornir_rich/progress_bar.py
+-rw-r--r--   0        0        0     1316 2023-05-29 18:53:07.703822 nornir_rich-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2211 1970-01-01 00:00:00.000000 nornir_rich-0.1.6/PKG-INFO
```

### Comparing `nornir-rich-0.1.5/README.md` & `nornir_rich-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `nornir-rich-0.1.5/nornir_rich/functions.py` & `nornir_rich-0.1.6/nornir_rich/functions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import logging
 import threading
-from typing import Any, List, Union, Dict
-from rich.console import RenderableType
+from typing import Any, List, Union, Dict, Tuple, Optional
+from rich.console import RenderableType, ConsoleRenderable
 
 from nornir.core import Nornir
 from nornir.core.inventory import Inventory
 from nornir.core.task import AggregatedResult, MultiResult, Result
 
 from rich import print
 from rich.columns import Columns
 from rich.panel import Panel
-from rich.scope import render_scope
 from rich.padding import PaddingDimensions
 from rich.pretty import Pretty
 from rich.protocol import is_renderable, rich_cast
+from rich.table import Table
+from rich.text import Text
 
 
 LOCK = threading.Lock()
 
 
 class RichHelper:
     """
@@ -27,34 +28,37 @@
       columns_settings: Settings passed to `rich.columns.Columns` object
       padding: Optional padding around cells. Defaults to (0, 1).
       expand: Expand columns to full width. Defaults to False.
       equal: Equal sized columns. Defaults to False
       vars: Which attributes you want to print
       severity_level: Print only errors with this severity level or higher
       failed: if ``True`` assume the task failed
+      line_breaks: if ``True`` line breaks in strings will be printed
     """
 
     def __init__(
         self,
         columns_settings: Dict[str, Any] = dict(),
-        padding: PaddingDimensions = None,
+        padding: Optional[PaddingDimensions] = None,
         expand: bool = False,
         equal: bool = True,
-        vars: List[str] = None,
+        vars: Optional[List[str]] = None,
         severity_level: int = 0,
-        failed: bool = None,
+        failed: Optional[bool] = None,
+        line_breaks: Optional[bool] = None,
     ) -> None:
         self.columns_settings = columns_settings
         self.columns_settings["expand"] = expand
         self.columns_settings["equal"] = equal
         if padding:
             self.columns_settings["padding"] = padding
         self.vars = vars
         self.severity_level = severity_level
         self.failed = failed
+        self.line_breaks = line_breaks
 
     def print_aggregated_result(self, result: AggregatedResult) -> Panel:
         """
         Render all task results per each host in AggregatedResult
 
         Arguments:
           result: AggregatedResult to render
@@ -106,15 +110,15 @@
         Return:
           rich.panel.Panel
         """
         if result.severity_level < self.severity_level:
             return None
         if self.vars:
             return Panel(
-                render_scope({x: getattr(result, x) for x in self.vars}),
+                self._scope_talbe(scope={x: getattr(result, x) for x in self.vars}),
                 title=result.name,
                 style="red" if result.failed else "green",
             )
 
         result_data: RenderableType
         if not is_renderable(result.result):
             result_data = Pretty(result.result) if result.result is not None else ""
@@ -125,21 +129,23 @@
             title=result.name,
             style="red" if result.failed else "green",
         )
 
     def print_scopes(self, scopes: Dict[str, Any]) -> Columns:
         if self.vars:
             columns = [
-                render_scope(
+                self._scope_talbe(
                     {k: v for k, v in map.items() if k in self.vars}, title=name
                 )
                 for name, map in scopes.items()
             ]
         else:
-            columns = [render_scope(map, title=name) for name, map in scopes.items()]
+            columns = [
+                self._scope_talbe(map, title=name) for name, map in scopes.items()
+            ]
         return Columns(
             columns,
             **self.columns_settings,
         )
 
     def print_dispatch(
         self, result: Union[Result, MultiResult, AggregatedResult]
@@ -157,108 +163,162 @@
             return self.print_aggregated_result(result)
         elif isinstance(result, MultiResult):
             return self.print_multi_result(result)
         elif isinstance(result, Result):
             return self.print_result(result)
         return Panel(f"Unable to find printer function for {result}")
 
+    def _scope_talbe(
+        self,
+        scope: "Dict[str, Any]",
+        title: Optional[str] = None,
+    ) -> Panel:
+        """Render python variables in a given scope.
+
+        ***This code is heavily inspired/copied by/from nornir.scope.render_scope***
+        https://github.com/Textualize/rich/blob/master/rich/scope.py
+
+        Args:
+            scope (Dict[str, Any]): A mapping containing variable names and values.
+
+        Returns:
+            Panel: Panel containing the table with key value mapping
+        """
+        items_table = Table.grid(padding=(0, 1), expand=False)
+        items_table.add_column(justify="right")
+
+        def sort_items(item: Tuple[str, Any]) -> Tuple[bool, str]:
+            """Sort special variables first, then alphabetically."""
+            key, _ = item
+            return (not key.startswith("__"), key.lower())
+
+        items = sorted(scope.items(), key=sort_items)
+
+        for key, value in items:
+            key_text = Text.assemble(
+                (key, "scope.key.special" if key.startswith("__") else "scope.key"),
+                (" =", "scope.equals"),
+            )
+
+            if self.line_breaks and isinstance(value, str):
+                value_text: ConsoleRenderable = Text(value.strip())
+            else:
+                value_text = Pretty(value)
+
+            items_table.add_row(
+                key_text,
+                value_text,
+            )
+        return Panel.fit(
+            items_table,
+            title=title,
+            border_style="scope.border",
+            padding=(0, 1),
+        )
+
 
 def print_result(
     result: Union[Result, MultiResult, AggregatedResult],
-    vars: List[str] = None,
+    vars: Optional[List[str]] = None,
     failed: bool = False,
     severity_level: int = logging.INFO,
     columns_settings: Dict[str, Any] = dict(),
-    padding: PaddingDimensions = None,
+    padding: Optional[PaddingDimensions] = None,
     expand: bool = False,
     equal: bool = True,
+    line_breaks: bool = False,
 ) -> None:
     """
     Prints an object of type `nornir.core.task.Result` || `nornir.core.task.MultiResult` || `nornir.core.task.AggregatedResult`
 
     Arguments:
       result: from a previous task
       vars: Which attributes you want to print
       failed: if ``True`` assume the task failed
       severity_level: Print only errors with this severity level or higher
       columns_settings: Settings passed to `rich.columns.Columns` object
       padding: Optional padding around cells. Defaults to (0, 1).
       expand: Expand columns to full width. Defaults to False.
       equal: Equal sized columns. Defaults to False
+      line_breaks: if ``True`` line breaks in strings will be printed
     """
     LOCK.acquire()
     equal = False if expand else equal
     rh = RichHelper(
         columns_settings=columns_settings,
         padding=padding,
         expand=expand,
         equal=equal,
         vars=vars,
         severity_level=severity_level,
         failed=failed,
+        line_breaks=line_breaks,
     )
     try:
         if isinstance(result, AggregatedResult):
             print(rh.print_aggregated_result(result))
         elif isinstance(result, MultiResult):
             print(rh.print_multi_result(result))
         elif isinstance(result, Result):
             print(rh.print_result(result))
     finally:
         LOCK.release()
 
 
 def print_failed_hosts(
     result: AggregatedResult,
-    vars: List[str] = None,
+    vars: Optional[List[str]] = None,
     failed: bool = False,
     severity_level: int = logging.INFO,
     columns_settings: Dict[str, Any] = dict(),
-    padding: PaddingDimensions = None,
+    padding: Optional[PaddingDimensions] = None,
     expand: bool = False,
     equal: bool = True,
+    line_breaks: bool = False,
 ) -> None:
     """
     Prints results of all failed hosts from `nornir.core.task.AggregatedResult`
 
     Arguments:
       result: from a previous task
       vars: Which attributes you want to print
       failed: if ``True`` assume the task failed
       severity_level: Print only errors with this severity level or higher
       columns_settings: Settings passed to `rich.columns.Columns` object
       padding: Optional padding around cells. Defaults to (0, 1).
       expand: Expand columns to full width. Defaults to False.
       equal: Equal sized columns. Defaults to False
+      line_breaks: if ``True`` line breaks in strings will be printed
     """
     LOCK.acquire()
     equal = False if expand else equal
     rh = RichHelper(
         columns_settings=columns_settings,
         padding=padding,
         expand=expand,
         equal=equal,
         vars=vars,
         severity_level=severity_level,
         failed=failed,
+        line_breaks=line_breaks,
     )
     try:
         for host, multi_result in result.failed_hosts.items():
             print(rh.print_multi_result(multi_result, host))
     finally:
         LOCK.release()
 
 
 def print_inventory(
     inventory: Union[Inventory, Nornir],
-    vars: List[str] = None,
+    vars: Optional[List[str]] = None,
     failed: bool = False,
     severity_level: int = logging.INFO,
     columns_settings: Dict[str, Any] = dict(),
-    padding: PaddingDimensions = None,
+    padding: Optional[PaddingDimensions] = None,
     expand: bool = False,
     equal: bool = True,
 ) -> None:
     """
     Prints results of all failed hosts from `nornir.core.task.AggregatedResult`
 
     Arguments:
```

### Comparing `nornir-rich-0.1.5/nornir_rich/progress_bar.py` & `nornir_rich-0.1.6/nornir_rich/progress_bar.py`

 * *Files identical despite different names*

### Comparing `nornir-rich-0.1.5/pyproject.toml` & `nornir_rich-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nornir-rich"
-version = "0.1.5"
+version = "0.1.6"
 description = "Collection of 'nice looking' functions with rich for nornir"
 authors = ["ubaumann <github@m.ubaumann.ch>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/InfrastructureAsCode-ch/nornir_rich"
 classifiers = [
         "License :: OSI Approved :: Apache Software License",
@@ -13,21 +13,21 @@
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 nornir = "^3"
-rich = "^12"
+rich = "^12|^13"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0"
-black = {extras = ["jupyter"], version = "^22.1.0"}
-mypy = "^0.931"
-ipykernel = "^6.9.1"
+pytest = "^7"
+black = {extras = ["jupyter"], version = "^23.3.0"}
+mypy = "^1"
+ipykernel = "^6"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 
 [tool.mypy]
```

### Comparing `nornir-rich-0.1.5/setup.py` & `nornir_rich-0.1.6/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,88 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: nornir-rich
+Version: 0.1.6
+Summary: Collection of 'nice looking' functions with rich for nornir
+Home-page: https://github.com/InfrastructureAsCode-ch/nornir_rich
+License: Apache-2.0
+Author: ubaumann
+Author-email: github@m.ubaumann.ch
+Requires-Python: >=3.7,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: nornir (>=3,<4)
+Requires-Dist: rich (>=12,<14)
+Project-URL: Repository, https://github.com/InfrastructureAsCode-ch/nornir_rich
+Description-Content-Type: text/markdown
 
-packages = \
-['nornir_rich']
+# nornir_rich
 
-package_data = \
-{'': ['*']}
+## Install
 
-install_requires = \
-['nornir>=3,<4', 'rich>=12,<13']
-
-setup_kwargs = {
-    'name': 'nornir-rich',
-    'version': '0.1.5',
-    'description': "Collection of 'nice looking' functions with rich for nornir",
-    'long_description': '# nornir_rich\n\n## Install\n\n```bash\npip install nornir-rich\n```\n\n## Usage\n\nFeatures\n\n- Print functions\n  - `print_result`\n  - `print_failed_hosts`\n  - `print_inventory`\n- Processors\n  - `progressbar`\n\n\n### Print example\n\n```python\nfrom nornir_rich.functions import print_result\n\nresults = nr.run(\n    task=hello_world\n)\n\nprint_result(results)\nprint_result(results, vars=["diff", "result", "name", "exception", "severity_level"])\n```\n\n### Progress bar example\n\n```python\nfrom time import sleep\nfrom nornir_rich.progress_bar import RichProgressBar\n\n\ndef random_sleep(task: Task) -> Result:\n    delay = randrange(10)\n    sleep(delay)\n    return Result(host=task.host, result=f"{delay} seconds delay")\n\n\nnr_with_processors = nr.with_processors([RichProgressBar()])\nresult = nr_with_processors.run(task=random_sleep)\n```\n\n\n## Images\n\n### Print Inventory\n\n![Print inventory](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nornir_rich/main/docs/imgs/print_inventory.png)\n\n### Print Result\n\n![Print Result](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nornir_rich/main/docs/imgs/print_result.png)\n\n### Progress Bar\n\n![Progress Bar](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nornir_rich/main/docs/imgs/progressbar.png)\n\n\nMore [examples](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nornir_rich/main/docs/imgs/print_functions.ipynb)',
-    'author': 'ubaumann',
-    'author_email': 'github@m.ubaumann.ch',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/InfrastructureAsCode-ch/nornir_rich',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
+```bash
+pip install nornir-rich
+```
 
+## Usage
 
-setup(**setup_kwargs)
+Features
+
+- Print functions
+  - `print_result`
+  - `print_failed_hosts`
+  - `print_inventory`
+- Processors
+  - `progressbar`
+
+
+### Print example
+
+```python
+from nornir_rich.functions import print_result
+
+results = nr.run(
+    task=hello_world
+)
+
+print_result(results)
+print_result(results, vars=["diff", "result", "name", "exception", "severity_level"])
+```
+
+### Progress bar example
+
+```python
+from time import sleep
+from nornir_rich.progress_bar import RichProgressBar
+
+
+def random_sleep(task: Task) -> Result:
+    delay = randrange(10)
+    sleep(delay)
+    return Result(host=task.host, result=f"{delay} seconds delay")
+
+
+nr_with_processors = nr.with_processors([RichProgressBar()])
+result = nr_with_processors.run(task=random_sleep)
+```
+
+
+## Images
+
+### Print Inventory
+
+![Print inventory](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nornir_rich/main/docs/imgs/print_inventory.png)
+
+### Print Result
+
+![Print Result](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nornir_rich/main/docs/imgs/print_result.png)
+
+### Progress Bar
+
+![Progress Bar](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nornir_rich/main/docs/imgs/progressbar.png)
+
+
+More [examples](https://raw.githubusercontent.com/InfrastructureAsCode-ch/nornir_rich/main/docs/imgs/print_functions.ipynb)
```


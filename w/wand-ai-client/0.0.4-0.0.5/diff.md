# Comparing `tmp/wand-ai-client-0.0.4.tar.gz` & `tmp/wand-ai-client-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wand-ai-client-0.0.4.tar", last modified: Mon May 29 11:06:08 2023, max compression
+gzip compressed data, was "wand-ai-client-0.0.5.tar", last modified: Mon May 29 13:20:06 2023, max compression
```

## Comparing `wand-ai-client-0.0.4.tar` & `wand-ai-client-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.4/README.md
--rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.4/pyproject.toml
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1809 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/setup.cfg
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/wand_ai_client.egg-info/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)      508 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/entry_points.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/not-zip-safe
--rw-r--r--   0 romasku   (1000) romasku   (1000)      228 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/requires.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/top_level.txt
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/wand_client/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.4/wand_client/__init__.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/wand_client/cli/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.4/wand_client/cli/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1148 2023-05-28 09:03:50.000000 wand-ai-client-0.0.4/wand_client/cli/config.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     2546 2023-05-28 08:59:31.000000 wand-ai-client-0.0.4/wand_client/cli/formatters.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5010 2023-05-29 11:05:12.000000 wand-ai-client-0.0.4/wand_client/cli/main.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)      384 2023-05-29 11:05:10.000000 wand-ai-client-0.0.4/wand_client/jupiter.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/wand_client/sdk/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.4/wand_client/sdk/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5440 2023-05-29 11:05:12.000000 wand-ai-client-0.0.4/wand_client/sdk/core.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 13:20:06.113360 wand-ai-client-0.0.5/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 13:20:06.113360 wand-ai-client-0.0.5/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.5/README.md
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.5/pyproject.toml
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1860 2023-05-29 13:20:06.113360 wand-ai-client-0.0.5/setup.cfg
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 13:20:06.113360 wand-ai-client-0.0.5/wand_ai_client.egg-info/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 13:20:06.000000 wand-ai-client-0.0.5/wand_ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      508 2023-05-29 13:20:06.000000 wand-ai-client-0.0.5/wand_ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-29 13:20:06.000000 wand-ai-client-0.0.5/wand_ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-29 13:20:06.000000 wand-ai-client-0.0.5/wand_ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.5/wand_ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      228 2023-05-29 13:20:06.000000 wand-ai-client-0.0.5/wand_ai_client.egg-info/requires.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-29 13:20:06.000000 wand-ai-client-0.0.5/wand_ai_client.egg-info/top_level.txt
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 13:20:06.113360 wand-ai-client-0.0.5/wand_client/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.5/wand_client/__init__.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 13:20:06.113360 wand-ai-client-0.0.5/wand_client/cli/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.5/wand_client/cli/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1148 2023-05-28 09:03:50.000000 wand-ai-client-0.0.5/wand_client/cli/config.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     3043 2023-05-29 13:18:26.000000 wand-ai-client-0.0.5/wand_client/cli/formatters.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     5091 2023-05-29 13:07:09.000000 wand-ai-client-0.0.5/wand_client/cli/main.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     2538 2023-05-29 13:18:26.000000 wand-ai-client-0.0.5/wand_client/jupyter.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 13:20:06.113360 wand-ai-client-0.0.5/wand_client/sdk/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.5/wand_client/sdk/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     5635 2023-05-29 13:18:12.000000 wand-ai-client-0.0.5/wand_client/sdk/core.py
```

### Comparing `wand-ai-client-0.0.4/PKG-INFO` & `wand-ai-client-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.4/README.md` & `wand-ai-client-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.4/setup.cfg` & `wand-ai-client-0.0.5/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wand-ai-client
-version = 0.0.4
+version = 0.0.5
 description = Wand AI API client
 author = Wand.AI Team
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -80,11 +80,14 @@
 
 [mypy-firebase_admin]
 ignore_missing_imports = true
 
 [mypy-google.*]
 ignore_missing_imports = true
 
+[mypy-ipywidgets.*]
+ignore_missing_imports = true
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `wand-ai-client-0.0.4/wand_ai_client.egg-info/PKG-INFO` & `wand-ai-client-0.0.5/wand_ai_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.4
+Version: 0.0.5
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.4/wand_client/cli/config.py` & `wand-ai-client-0.0.5/wand_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.4/wand_client/cli/formatters.py` & `wand-ai-client-0.0.5/wand_client/cli/formatters.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import operator
 from typing import Optional, Sequence
 
 from rich import box
 from rich.console import RenderableType
+from rich.progress import Progress
 from rich.table import Table
 
 from wand_client.cli.config import WandCliSettings
-from wand_client.sdk.core import Model, Source
+from wand_client.sdk.core import Model, Source, TrainingListener
 
 
 class SettingsFormatter:
     def __call__(self, settings: WandCliSettings) -> RenderableType:
         table = Table(
             box=None,
             show_header=False,
@@ -73,7 +74,21 @@
         width = len("1ce961e5172a688b842d")
         table.add_column("Id", style="bold", width=width)
         table.add_column("Progress")
         table.add_column("Training Completed")
         for disk in disks:
             table.add_row(*self._model_to_table_row(disk))
         return table
+
+
+class RichProgressListener(TrainingListener):
+    def __init__(self, progress: Progress) -> None:
+        self._progress = progress
+        self._task = progress.add_task("Training model")
+
+    def on_model_progress(self, model: Model) -> None:
+        self._progress.update(
+            self._task,
+            completed=model.status.progress,
+            description=f"Training model {model.id}",
+        )
+        self._progress.refresh()
```

### Comparing `wand-ai-client-0.0.4/wand_client/cli/main.py` & `wand-ai-client-0.0.5/wand_client/cli/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,13 +173,14 @@
 
     session: PromptSession[str] = PromptSession()
     console = rich.console.Console()
     while True:
         prompt_text = session.prompt("> ")
         if prompt_text == "exit":
             return
-        resp = chat.ask(prompt_text)
+        with console.status("Generating answer...", spinner="bouncingBall"):
+            resp = chat.ask(prompt_text)
         console.print(resp, style="bold")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `wand-ai-client-0.0.4/wand_client/sdk/core.py` & `wand-ai-client-0.0.5/wand_client/sdk/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,18 +66,23 @@
         return FileSourceCreationResult(
             source=Source(id=res["source_id"]), upload_url=res["upload_signed_url"]
         )
 
     def create_from_filepath(self, filepath: Union[str, Path]) -> Source:
         path = Path(filepath)
         res = self.create_file(path.name)
-        with path.open() as file:
+        with path.open("rb") as file:
             requests.put(res.upload_url, data=file)
         return res.source
 
+    def create_from_file_data(self, filename: str, data: bytes) -> Source:
+        res = self.create_file(filename)
+        requests.put(res.upload_url, data=data)
+        return res.source
+
 
 class ModelStatus(BaseModel):
     progress: int
     training_completed: bool
 
 
 class Model(BaseModel):
```


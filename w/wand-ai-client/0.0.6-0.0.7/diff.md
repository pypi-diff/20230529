# Comparing `tmp/wand-ai-client-0.0.6.tar.gz` & `tmp/wand-ai-client-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wand-ai-client-0.0.6.tar", last modified: Mon May 29 13:45:22 2023, max compression
+gzip compressed data, was "wand-ai-client-0.0.7.tar", last modified: Mon May 29 14:04:04 2023, max compression
```

## Comparing `wand-ai-client-0.0.6.tar` & `wand-ai-client-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 13:45:22.912567 wand-ai-client-0.0.6/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 13:45:22.912567 wand-ai-client-0.0.6/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.6/README.md
--rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.6/pyproject.toml
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1859 2023-05-29 13:45:22.912567 wand-ai-client-0.0.6/setup.cfg
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 13:45:22.912567 wand-ai-client-0.0.6/wand_ai_client.egg-info/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 13:45:22.000000 wand-ai-client-0.0.6/wand_ai_client.egg-info/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)      508 2023-05-29 13:45:22.000000 wand-ai-client-0.0.6/wand_ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-29 13:45:22.000000 wand-ai-client-0.0.6/wand_ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-29 13:45:22.000000 wand-ai-client-0.0.6/wand_ai_client.egg-info/entry_points.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.6/wand_ai_client.egg-info/not-zip-safe
--rw-r--r--   0 romasku   (1000) romasku   (1000)      227 2023-05-29 13:45:22.000000 wand-ai-client-0.0.6/wand_ai_client.egg-info/requires.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-29 13:45:22.000000 wand-ai-client-0.0.6/wand_ai_client.egg-info/top_level.txt
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 13:45:22.912567 wand-ai-client-0.0.6/wand_client/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.6/wand_client/__init__.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 13:45:22.912567 wand-ai-client-0.0.6/wand_client/cli/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.6/wand_client/cli/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1148 2023-05-28 09:03:50.000000 wand-ai-client-0.0.6/wand_client/cli/config.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     3043 2023-05-29 13:18:26.000000 wand-ai-client-0.0.6/wand_client/cli/formatters.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5091 2023-05-29 13:07:09.000000 wand-ai-client-0.0.6/wand_client/cli/main.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     2885 2023-05-29 13:44:56.000000 wand-ai-client-0.0.6/wand_client/jupyter.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 13:45:22.912567 wand-ai-client-0.0.6/wand_client/sdk/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.6/wand_client/sdk/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5635 2023-05-29 13:18:12.000000 wand-ai-client-0.0.6/wand_client/sdk/core.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 14:04:04.260552 wand-ai-client-0.0.7/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 14:04:04.260552 wand-ai-client-0.0.7/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.7/README.md
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.7/pyproject.toml
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1859 2023-05-29 14:04:04.260552 wand-ai-client-0.0.7/setup.cfg
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 14:04:04.257218 wand-ai-client-0.0.7/wand_ai_client.egg-info/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      508 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      227 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/requires.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-29 14:04:04.000000 wand-ai-client-0.0.7/wand_ai_client.egg-info/top_level.txt
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 14:04:04.257218 wand-ai-client-0.0.7/wand_client/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.7/wand_client/__init__.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 14:04:04.257218 wand-ai-client-0.0.7/wand_client/cli/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.7/wand_client/cli/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1148 2023-05-28 09:03:50.000000 wand-ai-client-0.0.7/wand_client/cli/config.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     3043 2023-05-29 13:18:26.000000 wand-ai-client-0.0.7/wand_client/cli/formatters.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     5091 2023-05-29 13:07:09.000000 wand-ai-client-0.0.7/wand_client/cli/main.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     2773 2023-05-29 14:03:37.000000 wand-ai-client-0.0.7/wand_client/jupyter.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 14:04:04.260552 wand-ai-client-0.0.7/wand_client/sdk/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.7/wand_client/sdk/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     5635 2023-05-29 13:18:12.000000 wand-ai-client-0.0.7/wand_client/sdk/core.py
```

### Comparing `wand-ai-client-0.0.6/PKG-INFO` & `wand-ai-client-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.6/README.md` & `wand-ai-client-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.6/setup.cfg` & `wand-ai-client-0.0.7/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wand-ai-client
-version = 0.0.6
+version = 0.0.7
 description = Wand AI API client
 author = Wand.AI Team
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `wand-ai-client-0.0.6/wand_ai_client.egg-info/PKG-INFO` & `wand-ai-client-0.0.7/wand_ai_client.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.6
+Version: 0.0.7
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.6/wand_client/cli/config.py` & `wand-ai-client-0.0.7/wand_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.6/wand_client/cli/formatters.py` & `wand-ai-client-0.0.7/wand_client/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.6/wand_client/cli/main.py` & `wand-ai-client-0.0.7/wand_client/cli/main.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.6/wand_client/jupyter.py` & `wand-ai-client-0.0.7/wand_client/jupyter.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 from typing import Any, List, Optional
 
 import requests
 from IPython.display import display
 from ipywidgets import FileUpload
-from rich.console import Console
 from rich.progress import Progress
 
 from wand_client.cli.formatters import RichProgressListener
 from wand_client.sdk.core import Model, WandClient
 
 
 def chat(model_id: str, client: WandClient) -> None:
     chat_session = client.models.start_chat(model_id)
 
-    console = Console()
-
-    console.print(f"You are talking to model with id {model_id}. Type 'exit' to close.")
+    print(f"You are talking to model with id {model_id}. Type 'exit' to close.")
 
     while True:
         prompt_text = input("> ")
         if prompt_text == "exit":
             return
-
-        with console.status("Generating answer...", spinner="bouncingBall"):
-            resp = chat_session.ask(prompt_text)
-        console.print(resp, style="bold")
+        print("Generating answer...")
+        print("\n")
+        resp = chat_session.ask(prompt_text)
+        print(resp)
 
 
 class TrainByFileManager:
     def __init__(self, client: WandClient) -> None:
         self._client = client
         self._upload = FileUpload()
         self.model: Optional[Model] = None
```

### Comparing `wand-ai-client-0.0.6/wand_client/sdk/core.py` & `wand-ai-client-0.0.7/wand_client/sdk/core.py`

 * *Files identical despite different names*


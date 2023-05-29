# Comparing `tmp/wand-ai-client-0.0.3.tar.gz` & `tmp/wand-ai-client-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wand-ai-client-0.0.3.tar", last modified: Mon May 29 10:47:11 2023, max compression
+gzip compressed data, was "wand-ai-client-0.0.4.tar", last modified: Mon May 29 11:06:08 2023, max compression
```

## Comparing `wand-ai-client-0.0.3.tar` & `wand-ai-client-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.3/README.md
--rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.3/pyproject.toml
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1809 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/setup.cfg
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/wand_ai_client.egg-info/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)      485 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/entry_points.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/not-zip-safe
--rw-r--r--   0 romasku   (1000) romasku   (1000)      228 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/requires.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/top_level.txt
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/wand_client/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.3/wand_client/__init__.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/wand_client/cli/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.3/wand_client/cli/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1148 2023-05-28 09:03:50.000000 wand-ai-client-0.0.3/wand_client/cli/config.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     2546 2023-05-28 08:59:31.000000 wand-ai-client-0.0.3/wand_client/cli/formatters.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5275 2023-05-29 10:45:32.000000 wand-ai-client-0.0.3/wand_client/cli/main.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/wand_client/sdk/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.3/wand_client/sdk/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     4772 2023-05-29 10:43:09.000000 wand-ai-client-0.0.3/wand_client/sdk/core.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.4/README.md
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.4/pyproject.toml
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1809 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/setup.cfg
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/wand_ai_client.egg-info/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      508 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      228 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/requires.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-29 11:06:08.000000 wand-ai-client-0.0.4/wand_ai_client.egg-info/top_level.txt
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/wand_client/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.4/wand_client/__init__.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/wand_client/cli/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.4/wand_client/cli/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1148 2023-05-28 09:03:50.000000 wand-ai-client-0.0.4/wand_client/cli/config.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     2546 2023-05-28 08:59:31.000000 wand-ai-client-0.0.4/wand_client/cli/formatters.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     5010 2023-05-29 11:05:12.000000 wand-ai-client-0.0.4/wand_client/cli/main.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      384 2023-05-29 11:05:10.000000 wand-ai-client-0.0.4/wand_client/jupiter.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 11:06:08.989541 wand-ai-client-0.0.4/wand_client/sdk/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.4/wand_client/sdk/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     5440 2023-05-29 11:05:12.000000 wand-ai-client-0.0.4/wand_client/sdk/core.py
```

### Comparing `wand-ai-client-0.0.3/PKG-INFO` & `wand-ai-client-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.3/README.md` & `wand-ai-client-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.3/setup.cfg` & `wand-ai-client-0.0.4/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wand-ai-client
-version = 0.0.3
+version = 0.0.4
 description = Wand AI API client
 author = Wand.AI Team
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
```

### Comparing `wand-ai-client-0.0.3/wand_ai_client.egg-info/PKG-INFO` & `wand-ai-client-0.0.4/wand_ai_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.3
+Version: 0.0.4
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `wand-ai-client-0.0.3/wand_client/cli/config.py` & `wand-ai-client-0.0.4/wand_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.3/wand_client/cli/formatters.py` & `wand-ai-client-0.0.4/wand_client/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.3/wand_client/cli/main.py` & `wand-ai-client-0.0.4/wand_client/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,21 +11,15 @@
 from wand_client.cli.config import CONFIG_PATH, WandCliSettings
 from wand_client.cli.formatters import (
     ModelFormatter,
     ModelsFormatter,
     SettingsFormatter,
     SourceFormatter,
 )
-from wand_client.sdk.core import (
-    ChatMessage,
-    ChatMessageAuthor,
-    Model,
-    TrainingListener,
-    WandClient,
-)
+from wand_client.sdk.core import Model, TrainingListener, WandClient
 
 
 class Root:
     def __init__(self, option_settings: Dict[str, Any]) -> None:
         self._option_settings = option_settings
 
     def get_settings(self) -> WandCliSettings:
@@ -169,25 +163,23 @@
 
 @model.command()
 @click.argument("model_id", type=click.STRING)
 @click.pass_context
 def chat(ctx: Context, model_id: str) -> None:
     """Talk with LLM model"""
     client: WandClient = ctx.obj.get_client()
-    history: List[ChatMessage] = []
+    chat = client.models.start_chat(model_id)
 
     print(f"You are talking to model with id {model_id}. Type 'exit' to close.")
 
     session: PromptSession[str] = PromptSession()
     console = rich.console.Console()
     while True:
         prompt_text = session.prompt("> ")
         if prompt_text == "exit":
             return
-        resp = client.models.infer(model_id, prompt=prompt_text, chat_history=history)
+        resp = chat.ask(prompt_text)
         console.print(resp, style="bold")
-        history.append(ChatMessage(author=ChatMessageAuthor.HUMAN, message=prompt_text))
-        history.append(ChatMessage(author=ChatMessageAuthor.AI, message=resp))
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `wand-ai-client-0.0.3/wand_client/sdk/core.py` & `wand-ai-client-0.0.4/wand_client/sdk/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,14 +167,34 @@
             model = self.get(model.id)
             if listener:
                 listener.on_model_progress(model)
             if model.status.training_completed:
                 return model
             time.sleep(1)
 
+    def start_chat(self, model_id: str) -> "ChatSession":
+        return ChatSession(model_id, self)
+
+
+class ChatSession:
+    def __init__(self, model_id: str, client: Models) -> None:
+        self._model_id = model_id
+        self._client = client
+        self._chat_history: List[ChatMessage] = []
+
+    def ask(self, prompt: str) -> str:
+        resp = self._client.infer(self._model_id, prompt, self._chat_history)
+        self._chat_history.append(
+            ChatMessage(author=ChatMessageAuthor.HUMAN, message=prompt)
+        )
+        self._chat_history.append(
+            ChatMessage(author=ChatMessageAuthor.AI, message=resp)
+        )
+        return resp
+
 
 class WandClient:
     def __init__(
         self,
         token: str,
         base_url: str,
     ):
```


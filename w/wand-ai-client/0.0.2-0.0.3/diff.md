# Comparing `tmp/wand-ai-client-0.0.2.tar.gz` & `tmp/wand-ai-client-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wand-ai-client-0.0.2.tar", last modified: Sun May 28 09:05:02 2023, max compression
+gzip compressed data, was "wand-ai-client-0.0.3.tar", last modified: Mon May 29 10:47:11 2023, max compression
```

## Comparing `wand-ai-client-0.0.2.tar` & `wand-ai-client-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      884 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.2/README.md
--rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.2/pyproject.toml
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1861 2023-05-28 09:05:02.339968 wand-ai-client-0.0.2/setup.cfg
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/wand_ai_client.egg-info/
--rw-r--r--   0 romasku   (1000) romasku   (1000)      884 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/PKG-INFO
--rw-r--r--   0 romasku   (1000) romasku   (1000)      485 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/SOURCES.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/dependency_links.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/entry_points.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/not-zip-safe
--rw-r--r--   0 romasku   (1000) romasku   (1000)      228 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/requires.txt
--rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-28 09:05:02.000000 wand-ai-client-0.0.2/wand_ai_client.egg-info/top_level.txt
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/wand_client/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.2/wand_client/__init__.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/wand_client/cli/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.2/wand_client/cli/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     1148 2023-05-28 09:03:50.000000 wand-ai-client-0.0.2/wand_client/cli/config.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     2546 2023-05-28 08:59:31.000000 wand-ai-client-0.0.2/wand_client/cli/formatters.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     5288 2023-05-28 09:03:27.000000 wand-ai-client-0.0.2/wand_client/cli/main.py
-drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-28 09:05:02.336634 wand-ai-client-0.0.2/wand_client/sdk/
--rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.2/wand_client/sdk/__init__.py
--rw-r--r--   0 romasku   (1000) romasku   (1000)     4774 2023-05-28 09:03:50.000000 wand-ai-client-0.0.2/wand_client/sdk/core.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1075 2023-05-22 19:10:31.000000 wand-ai-client-0.0.3/README.md
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      176 2023-05-27 16:26:52.000000 wand-ai-client-0.0.3/pyproject.toml
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1809 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/setup.cfg
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/wand_ai_client.egg-info/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      821 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/PKG-INFO
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      485 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/SOURCES.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/dependency_links.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       54 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/entry_points.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        1 2023-05-27 19:56:31.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/not-zip-safe
+-rw-r--r--   0 romasku   (1000) romasku   (1000)      228 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/requires.txt
+-rw-r--r--   0 romasku   (1000) romasku   (1000)       12 2023-05-29 10:47:11.000000 wand-ai-client-0.0.3/wand_ai_client.egg-info/top_level.txt
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/wand_client/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-26 17:07:29.000000 wand-ai-client-0.0.3/wand_client/__init__.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/wand_client/cli/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:55:30.000000 wand-ai-client-0.0.3/wand_client/cli/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     1148 2023-05-28 09:03:50.000000 wand-ai-client-0.0.3/wand_client/cli/config.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     2546 2023-05-28 08:59:31.000000 wand-ai-client-0.0.3/wand_client/cli/formatters.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     5275 2023-05-29 10:45:32.000000 wand-ai-client-0.0.3/wand_client/cli/main.py
+drwxr-xr-x   0 romasku   (1000) romasku   (1000)        0 2023-05-29 10:47:11.885662 wand-ai-client-0.0.3/wand_client/sdk/
+-rw-r--r--   0 romasku   (1000) romasku   (1000)        0 2023-05-27 15:04:20.000000 wand-ai-client-0.0.3/wand_client/sdk/__init__.py
+-rw-r--r--   0 romasku   (1000) romasku   (1000)     4772 2023-05-29 10:43:09.000000 wand-ai-client-0.0.3/wand_client/sdk/core.py
```

### Comparing `wand-ai-client-0.0.2/PKG-INFO` & `wand-ai-client-0.0.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,10 +13,9 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8.0
 Provides-Extra: dev
```

### Comparing `wand-ai-client-0.0.2/README.md` & `wand-ai-client-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.2/setup.cfg` & `wand-ai-client-0.0.3/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wand-ai-client
-version = 0.0.2
+version = 0.0.3
 description = Wand AI API client
 author = Wand.AI Team
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
@@ -14,15 +14,14 @@
 	Environment :: Console
 	Intended Audience :: Developers
 	Intended Audience :: Science/Research
 	Intended Audience :: Information Technology
 	Topic :: Scientific/Engineering :: Artificial Intelligence
 	Topic :: Software Development
 	Topic :: Utilities
-	License :: OSI Approved :: Apache Software License
 
 [options]
 packages = find:
 zip_safe = False
 python_requires = >=3.8.0
 include_package_data = True
 install_requires =
```

### Comparing `wand-ai-client-0.0.2/wand_ai_client.egg-info/PKG-INFO` & `wand-ai-client-0.0.3/wand_ai_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wand-ai-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: Wand AI API client
 Author: Wand.AI Team
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,10 +13,9 @@
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Information Technology
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
-Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8.0
 Provides-Extra: dev
```

### Comparing `wand-ai-client-0.0.2/wand_client/cli/config.py` & `wand-ai-client-0.0.3/wand_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.2/wand_client/cli/formatters.py` & `wand-ai-client-0.0.3/wand_client/cli/formatters.py`

 * *Files identical despite different names*

### Comparing `wand-ai-client-0.0.2/wand_client/cli/main.py` & `wand-ai-client-0.0.3/wand_client/cli/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,28 +108,28 @@
 
 
 @source.command()
 @click.option("--max-pages", type=int, default=1000)
 @click.argument("url", type=click.STRING, nargs=-1)
 @click.pass_context
 def web(ctx: Context, url: List[str], max_pages: int = 1000) -> None:
-    """Upload a file as a source"""
+    """Create a web scrapper source"""
     client: WandClient = ctx.obj.get_client()
     source = client.source.create_web(url, max_pages)
     rich.print(SourceFormatter()(source))
 
 
 @cli.group()
 def model() -> None:
     """
     Operations with ml models
     """
 
 
-@source.command()
+@model.command()
 @click.argument("source_id", type=click.STRING, nargs=-1)
 @click.pass_context
 def train(ctx: Context, source_id: List[str]) -> None:
     """Upload a file as a source"""
     client: WandClient = ctx.obj.get_client()
 
     with Progress() as progress:
@@ -148,34 +148,34 @@
         rich.print(model.id)
 
 
 @model.command()
 @click.argument("model_id", type=click.STRING)
 @click.pass_context
 def get(ctx: Context, model_id: str) -> None:
-    """Upload a file as a source"""
+    """Get info about model by ID"""
     client: WandClient = ctx.obj.get_client()
     model = client.models.get(model_id=model_id)
     rich.print(ModelFormatter()(model))
 
 
 @model.command(name="list")
 @click.pass_context
 def list_(ctx: Context) -> None:
-    """Upload a file as a source"""
+    """List all models"""
     client: WandClient = ctx.obj.get_client()
     models = client.models.list_all()
     rich.print(ModelsFormatter()(models))
 
 
 @model.command()
 @click.argument("model_id", type=click.STRING)
 @click.pass_context
 def chat(ctx: Context, model_id: str) -> None:
-    """Upload a file as a source"""
+    """Talk with LLM model"""
     client: WandClient = ctx.obj.get_client()
     history: List[ChatMessage] = []
 
     print(f"You are talking to model with id {model_id}. Type 'exit' to close.")
 
     session: PromptSession[str] = PromptSession()
     console = rich.console.Console()
```

### Comparing `wand-ai-client-0.0.2/wand_client/sdk/core.py` & `wand-ai-client-0.0.3/wand_client/sdk/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
                         "author": it.author,
                         "message": it.message,
                     }
                     for it in chat_history
                 ],
             },
         )
-        return res.json()
+        return res.text
 
     def train(
         self, source_ids: List[str], listener: Optional[TrainingListener] = None
     ) -> Model:
         model = self.start_training(source_ids)
         while True:
             model = self.get(model.id)
```


# Comparing `tmp/lanarky-0.7.1.tar.gz` & `tmp/lanarky-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.7.1.tar", max compression
+gzip compressed data, was "lanarky-0.7.2.tar", max compression
```

## Comparing `lanarky-0.7.1.tar` & `lanarky-0.7.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-05-29 08:43:15.238398 lanarky-0.7.1/LICENSE
--rw-r--r--   0        0        0     4279 2023-05-29 08:43:15.238398 lanarky-0.7.1/README.md
--rw-r--r--   0        0        0        0 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/__init__.py
--rw-r--r--   0        0        0     2874 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0     3023 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/callbacks/agents.py
--rw-r--r--   0        0        0     2200 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1685 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     3461 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0     2004 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/register.py
--rw-r--r--   0        0        0       74 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     2926 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/responses/streaming.py
--rw-r--r--   0        0        0       70 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/routing/__init__.py
--rw-r--r--   0        0        0     2891 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/routing/langchain.py
--rw-r--r--   0        0        0     4061 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/routing/utils.py
--rw-r--r--   0        0        0      715 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3844 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/websockets/base.py
--rw-r--r--   0        0        0     1110 2023-05-29 08:43:15.398398 lanarky-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 lanarky-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-29 09:35:50.355512 lanarky-0.7.2/LICENSE
+-rw-r--r--   0        0        0     4289 2023-05-29 09:35:50.355512 lanarky-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/__init__.py
+-rw-r--r--   0        0        0     2874 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     3023 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     2200 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1685 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     3461 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0     2004 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/register.py
+-rw-r--r--   0        0        0       74 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     2926 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0       70 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/routing/__init__.py
+-rw-r--r--   0        0        0     3092 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/routing/langchain.py
+-rw-r--r--   0        0        0     4207 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/routing/utils.py
+-rw-r--r--   0        0        0      715 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     3844 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/websockets/base.py
+-rw-r--r--   0        0        0     1110 2023-05-29 09:35:50.559514 lanarky-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     5110 1970-01-01 00:00:00.000000 lanarky-0.7.2/PKG-INFO
```

### Comparing `lanarky-0.7.1/LICENSE` & `lanarky-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/README.md` & `lanarky-0.7.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
 from lanarky.routing import LangchainRouter
 
 load_dotenv()
 app = FastAPI()
 
 langchain_router = LangchainRouter(
-    url="/chat",
+    langchain_url="/chat",
     langchain_object=ConversationChain(
         llm=ChatOpenAI(temperature=0), verbose=True
     ),
     streaming_mode=0
   )
 app.include_router(langchain_router)
 ```
```

#### html2text {}

```diff
@@ -21,15 +21,15 @@
 infrastructures. ## ð¾ Installation The library is available on PyPI and can
 be installed via `pip`. ```bash pip install lanarky ``` You can find the full
 documentation at [https://lanarky.readthedocs.io/en/latest/](https://
 lanarky.readthedocs.io/en/latest/). ## ð¥ Build your first Langchain app
 ```python from dotenv import load_dotenv from fastapi import FastAPI from
 langchain import ConversationChain from langchain.chat_models import ChatOpenAI
 from lanarky.routing import LangchainRouter load_dotenv() app = FastAPI()
-langchain_router = LangchainRouter( url="/chat",
+langchain_router = LangchainRouter( langchain_url="/chat",
 langchain_object=ConversationChain( llm=ChatOpenAI(temperature=0), verbose=True
 ), streaming_mode=0 ) app.include_router(langchain_router) ``` See [`examples/
 `](https://github.com/ajndkr/lanarky/blob/main/examples/README.md) for list of
 available demo examples. Create a `.env` file using `.env.sample` and add your
 OpenAI API key to it before running the examples. ![demo](https://
 raw.githubusercontent.com/ajndkr/lanarky/main/assets/demo.gif) ## ð Roadmap
 - [x] Add support for [LangChain](https://github.com/hwchase17/langchain) - [x]
```

### Comparing `lanarky-0.7.1/lanarky/callbacks/__init__.py` & `lanarky-0.7.2/lanarky/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/lanarky/callbacks/agents.py` & `lanarky-0.7.2/lanarky/callbacks/agents.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/lanarky/callbacks/base.py` & `lanarky-0.7.2/lanarky/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/lanarky/callbacks/llm.py` & `lanarky-0.7.2/lanarky/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.7.2/lanarky/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/lanarky/register.py` & `lanarky-0.7.2/lanarky/register.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/lanarky/responses/streaming.py` & `lanarky-0.7.2/lanarky/responses/streaming.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/lanarky/routing/langchain.py` & `lanarky-0.7.2/lanarky/routing/langchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import random
+import string
 from typing import Any, Optional, Type
 
 from fastapi.routing import APIRouter
 from fastapi.websockets import WebSocket
 from langchain.chains.base import Chain
 
 from .utils import (
@@ -51,22 +53,29 @@
         langchain_object: Chain,
         streaming_mode: StreamingMode,
         methods: list[str] = ["POST"],
         **kwargs,
     ):
         """Adds a Langchain API route to the router."""
         langchain_dependency = create_langchain_dependency(langchain_object)
+
+        name_prefix = "".join(
+            random.choice(string.ascii_letters) for _ in range(5)
+        ).title()
         endpoint_request = create_request_from_langchain_dependency(
-            langchain_dependency
+            langchain_dependency, name_prefix
         )
         response_model = (
-            create_response_model_from_langchain_dependency(langchain_dependency)
+            create_response_model_from_langchain_dependency(
+                langchain_dependency, name_prefix
+            )
             if streaming_mode == StreamingMode.OFF
             else None
         )
+
         endpoint = create_langchain_endpoint(
             endpoint_request,
             langchain_dependency,
             response_model,
             streaming_mode,
         )
```

### Comparing `lanarky-0.7.1/lanarky/routing/utils.py` & `lanarky-0.7.2/lanarky/routing/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,29 +23,33 @@
     def dependency() -> Chain:
         return langchain_object
 
     return Depends(dependency)
 
 
 def create_request_from_langchain_dependency(
-    langchain_dependency: params.Depends,
+    langchain_dependency: params.Depends, name_prefix: str = ""
 ) -> Type[BaseModel]:
     langchain_object: Chain = langchain_dependency.dependency()
+    model_name = name_prefix + "LangchainRequest"
     return create_model(
-        "LangchainRequest", **{key: (str, "") for key in langchain_object.input_keys}
+        model_name,
+        **{key: (str, "") for key in langchain_object.input_keys},
     )
 
 
 def create_response_model_from_langchain_dependency(
-    langchain_dependency: params.Depends,
+    langchain_dependency: params.Depends, name_prefix: str = ""
 ) -> Type[BaseModel]:
     """Creates a response model from a langchain dependency."""
     langchain_object: Chain = langchain_dependency.dependency()
+    model_name = name_prefix + "LangchainResponse"
     return create_model(
-        "LangchainResponse", **{key: (str, "") for key in langchain_object.output_keys}
+        model_name,
+        **{key: (str, "") for key in langchain_object.output_keys},
     )
 
 
 def create_langchain_base_endpoint(
     endpoint_request: BaseModel,
     langchain_dependency: params.Depends,
     response_model: BaseModel,
```

### Comparing `lanarky-0.7.1/lanarky/schemas.py` & `lanarky-0.7.2/lanarky/schemas.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/lanarky/testing/gradio.py` & `lanarky-0.7.2/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/lanarky/websockets/base.py` & `lanarky-0.7.2/lanarky/websockets/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.1/pyproject.toml` & `lanarky-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.7.1"
+version = "0.7.2"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
```

### Comparing `lanarky-0.7.1/PKG-INFO` & `lanarky-0.7.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.7.1
+Version: 0.7.2
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -72,15 +72,15 @@
 
 from lanarky.routing import LangchainRouter
 
 load_dotenv()
 app = FastAPI()
 
 langchain_router = LangchainRouter(
-    url="/chat",
+    langchain_url="/chat",
     langchain_object=ConversationChain(
         llm=ChatOpenAI(temperature=0), verbose=True
     ),
     streaming_mode=0
   )
 app.include_router(langchain_router)
 ```
```


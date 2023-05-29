# Comparing `tmp/lanarky-0.7.0.tar.gz` & `tmp/lanarky-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.7.0.tar", max compression
+gzip compressed data, was "lanarky-0.7.1.tar", max compression
```

## Comparing `lanarky-0.7.0.tar` & `lanarky-0.7.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2023-05-28 21:14:18.453756 lanarky-0.7.0/LICENSE
--rw-r--r--   0        0        0     4238 2023-05-28 21:14:18.453756 lanarky-0.7.0/README.md
--rw-r--r--   0        0        0        0 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/__init__.py
--rw-r--r--   0        0        0     2874 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0     3023 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/callbacks/agents.py
--rw-r--r--   0        0        0     2200 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1685 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     3461 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0     2004 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/register.py
--rw-r--r--   0        0        0       74 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     2926 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/responses/streaming.py
--rw-r--r--   0        0        0       70 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/routing/__init__.py
--rw-r--r--   0        0        0     2795 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/routing/langchain.py
--rw-r--r--   0        0        0     2627 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/routing/utils.py
--rw-r--r--   0        0        0      715 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3844 2023-05-28 21:14:18.633759 lanarky-0.7.0/lanarky/websockets/base.py
--rw-r--r--   0        0        0     1110 2023-05-28 21:14:18.633759 lanarky-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     5059 1970-01-01 00:00:00.000000 lanarky-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-29 08:43:15.238398 lanarky-0.7.1/LICENSE
+-rw-r--r--   0        0        0     4279 2023-05-29 08:43:15.238398 lanarky-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/__init__.py
+-rw-r--r--   0        0        0     2874 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     3023 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     2200 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1685 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     3461 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0     2004 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/register.py
+-rw-r--r--   0        0        0       74 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     2926 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0       70 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/routing/__init__.py
+-rw-r--r--   0        0        0     2891 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/routing/langchain.py
+-rw-r--r--   0        0        0     4061 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/routing/utils.py
+-rw-r--r--   0        0        0      715 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     3844 2023-05-29 08:43:15.398398 lanarky-0.7.1/lanarky/websockets/base.py
+-rw-r--r--   0        0        0     1110 2023-05-29 08:43:15.398398 lanarky-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5100 1970-01-01 00:00:00.000000 lanarky-0.7.1/PKG-INFO
```

### Comparing `lanarky-0.7.0/LICENSE` & `lanarky-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/README.md` & `lanarky-0.7.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,20 @@
 
 from lanarky.routing import LangchainRouter
 
 load_dotenv()
 app = FastAPI()
 
 langchain_router = LangchainRouter(
+    url="/chat",
     langchain_object=ConversationChain(
         llm=ChatOpenAI(temperature=0), verbose=True
-    )
-)
+    ),
+    streaming_mode=0
+  )
 app.include_router(langchain_router)
 ```
 
 See [`examples/`](https://github.com/ajndkr/lanarky/blob/main/examples/README.md)
 for list of available demo examples.
 
 Create a `.env` file using `.env.sample` and add your OpenAI API key to it
```

#### html2text {}

```diff
@@ -21,35 +21,36 @@
 infrastructures. ## ð¾ Installation The library is available on PyPI and can
 be installed via `pip`. ```bash pip install lanarky ``` You can find the full
 documentation at [https://lanarky.readthedocs.io/en/latest/](https://
 lanarky.readthedocs.io/en/latest/). ## ð¥ Build your first Langchain app
 ```python from dotenv import load_dotenv from fastapi import FastAPI from
 langchain import ConversationChain from langchain.chat_models import ChatOpenAI
 from lanarky.routing import LangchainRouter load_dotenv() app = FastAPI()
-langchain_router = LangchainRouter( langchain_object=ConversationChain
-( llm=ChatOpenAI(temperature=0), verbose=True ) ) app.include_router
-(langchain_router) ``` See [`examples/`](https://github.com/ajndkr/lanarky/
-blob/main/examples/README.md) for list of available demo examples. Create a
-`.env` file using `.env.sample` and add your OpenAI API key to it before
-running the examples. ![demo](https://raw.githubusercontent.com/ajndkr/lanarky/
-main/assets/demo.gif) ## ð Roadmap - [x] Add support for [LangChain](https:/
-/github.com/hwchase17/langchain) - [x] Add [Gradio](https://github.com/gradio-
-app/gradio) UI for fast prototyping - [ ] Add SQL database integration - [ ]
-Add support for [Guardrails](https://github.com/ShreyaR/guardrails) - [ ] Add
-support for [LlamaIndex](https://github.com/jerryjliu/llama_index) - [ ] Add
-[GPTCache](https://github.com/zilliztech/GPTCache) integration ## ð¤©
-Stargazers Leave a â­ if you find this project useful. [![Star History Chart]
-(https://api.star-history.com/svg?repos=ajndkr/lanarky&type=Date)](https://
-star-history.com/#ajndkr/lanarky&Date) ## ð¤ Contributing [![Code check]
-(https://github.com/ajndkr/lanarky/actions/workflows/code-check.yaml/
-badge.svg)](https://github.com/ajndkr/lanarky/actions/workflows/code-
-check.yaml) [![Publish](https://github.com/ajndkr/lanarky/actions/workflows/
-publish.yaml/badge.svg)](https://github.com/ajndkr/lanarky/actions/workflows/
-publish.yaml) Contributions are more than welcome! If you have an idea for a
-new feature or want to help improve lanarky, please create an issue or submit a
-pull request on [GitHub](https://github.com/ajndkr/lanarky). See
-[CONTRIBUTING.md](https://github.com/ajndkr/lanarky/blob/main/CONTRIBUTING.md)
-for more information. ### Contributors [![](https://img.shields.io/github/
-contributors-anon/ajndkr/lanarky)](https://github.com/ajndkr/lanarky/graphs/
-contributors) [https://contrib.rocks/image?repo=ajndkr/lanarky] ## âï¸
-License The library is released under the [MIT License](https://github.com/
-ajndkr/lanarky/blob/main/LICENSE).
+langchain_router = LangchainRouter( url="/chat",
+langchain_object=ConversationChain( llm=ChatOpenAI(temperature=0), verbose=True
+), streaming_mode=0 ) app.include_router(langchain_router) ``` See [`examples/
+`](https://github.com/ajndkr/lanarky/blob/main/examples/README.md) for list of
+available demo examples. Create a `.env` file using `.env.sample` and add your
+OpenAI API key to it before running the examples. ![demo](https://
+raw.githubusercontent.com/ajndkr/lanarky/main/assets/demo.gif) ## ð Roadmap
+- [x] Add support for [LangChain](https://github.com/hwchase17/langchain) - [x]
+Add [Gradio](https://github.com/gradio-app/gradio) UI for fast prototyping -
+[ ] Add SQL database integration - [ ] Add support for [Guardrails](https://
+github.com/ShreyaR/guardrails) - [ ] Add support for [LlamaIndex](https://
+github.com/jerryjliu/llama_index) - [ ] Add [GPTCache](https://github.com/
+zilliztech/GPTCache) integration ## ð¤© Stargazers Leave a â­ if you find
+this project useful. [![Star History Chart](https://api.star-history.com/
+svg?repos=ajndkr/lanarky&type=Date)](https://star-history.com/#ajndkr/
+lanarky&Date) ## ð¤ Contributing [![Code check](https://github.com/ajndkr/
+lanarky/actions/workflows/code-check.yaml/badge.svg)](https://github.com/
+ajndkr/lanarky/actions/workflows/code-check.yaml) [![Publish](https://
+github.com/ajndkr/lanarky/actions/workflows/publish.yaml/badge.svg)](https://
+github.com/ajndkr/lanarky/actions/workflows/publish.yaml) Contributions are
+more than welcome! If you have an idea for a new feature or want to help
+improve lanarky, please create an issue or submit a pull request on [GitHub]
+(https://github.com/ajndkr/lanarky). See [CONTRIBUTING.md](https://github.com/
+ajndkr/lanarky/blob/main/CONTRIBUTING.md) for more information. ###
+Contributors [![](https://img.shields.io/github/contributors-anon/ajndkr/
+lanarky)](https://github.com/ajndkr/lanarky/graphs/contributors) [https://
+contrib.rocks/image?repo=ajndkr/lanarky] ## âï¸ License The library is
+released under the [MIT License](https://github.com/ajndkr/lanarky/blob/main/
+LICENSE).
```

### Comparing `lanarky-0.7.0/lanarky/callbacks/__init__.py` & `lanarky-0.7.1/lanarky/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/lanarky/callbacks/agents.py` & `lanarky-0.7.1/lanarky/callbacks/agents.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/lanarky/callbacks/base.py` & `lanarky-0.7.1/lanarky/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/lanarky/callbacks/llm.py` & `lanarky-0.7.1/lanarky/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.7.1/lanarky/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/lanarky/register.py` & `lanarky-0.7.1/lanarky/register.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/lanarky/responses/streaming.py` & `lanarky-0.7.1/lanarky/responses/streaming.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/lanarky/routing/langchain.py` & `lanarky-0.7.1/lanarky/routing/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,110 @@
 from enum import IntEnum
-from typing import Any, Type
+from functools import lru_cache
+from typing import Type
 
-from fastapi.routing import APIRouter
+from fastapi import Depends, WebSocket, params
 from langchain.chains.base import Chain
+from pydantic import BaseModel, create_model
 
-from .utils import (
-    create_langchain_base_endpoint,
-    create_langchain_dependency,
-    create_langchain_streaming_endpoint,
-    create_langchain_streaming_json_endpoint,
-    create_request_from_langchain_dependency,
-    create_response_model_from_langchain_dependency,
-)
+from lanarky.responses import StreamingResponse
+from lanarky.websockets import WebsocketConnection
 
 
 class StreamingMode(IntEnum):
     OFF = 0
     TEXT = 1
     JSON = 2
 
 
+def create_langchain_dependency(langchain_object: Type[Chain]) -> params.Depends:
+    """Creates a langchain object dependency."""
+
+    @lru_cache(maxsize=1)
+    def dependency() -> Chain:
+        return langchain_object
+
+    return Depends(dependency)
+
+
+def create_request_from_langchain_dependency(
+    langchain_dependency: params.Depends,
+) -> Type[BaseModel]:
+    langchain_object: Chain = langchain_dependency.dependency()
+    return create_model(
+        "LangchainRequest", **{key: (str, "") for key in langchain_object.input_keys}
+    )
+
+
+def create_response_model_from_langchain_dependency(
+    langchain_dependency: params.Depends,
+) -> Type[BaseModel]:
+    """Creates a response model from a langchain dependency."""
+    langchain_object: Chain = langchain_dependency.dependency()
+    return create_model(
+        "LangchainResponse", **{key: (str, "") for key in langchain_object.output_keys}
+    )
+
+
+def create_langchain_base_endpoint(
+    endpoint_request: BaseModel,
+    langchain_dependency: params.Depends,
+    response_model: BaseModel,
+):
+    async def endpoint(
+        request: endpoint_request,
+        langchain_object: Chain = langchain_dependency,
+    ) -> response_model:
+        """Base chat endpoint."""
+        return await langchain_object.acall(inputs=request.dict())
+
+    return endpoint
+
+
+def create_langchain_streaming_endpoint(
+    endpoint_request: BaseModel, langchain_dependency: params.Depends
+):
+    async def endpoint(
+        request: endpoint_request,
+        langchain_object: Chain = langchain_dependency,
+    ) -> StreamingResponse:
+        """Streaming chat endpoint."""
+        print(f"langchain_object: {langchain_object}")
+        inputs = request.dict()
+        print(f"inputs: {inputs}")
+        return StreamingResponse.from_chain(
+            langchain_object, inputs, media_type="text/event-stream"
+        )
+
+    return endpoint
+
+
+def create_langchain_streaming_json_endpoint(
+    endpoint_request: BaseModel, langchain_dependency: params.Depends
+):
+    async def endpoint(
+        request: endpoint_request,
+        langchain_object: Chain = langchain_dependency,
+    ) -> StreamingResponse:
+        """Streaming JSON chat endpoint."""
+        return StreamingResponse.from_chain(
+            langchain_object,
+            request.dict(),
+            as_json=True,
+            media_type="text/event-stream",
+        )
+
+    return endpoint
+
+
 def create_langchain_endpoint(
-    endpoint_request, langchain_dependency, response_model, streaming_mode
+    endpoint_request: BaseModel,
+    langchain_dependency: params.Depends,
+    response_model: BaseModel,
+    streaming_mode: StreamingMode,
 ):
     """Creates a Langchain endpoint."""
     if streaming_mode == StreamingMode.OFF:
         endpoint = create_langchain_base_endpoint(
             endpoint_request, langchain_dependency, response_model
         )
     elif streaming_mode == StreamingMode.TEXT:
@@ -38,53 +117,21 @@
         )
     else:
         raise ValueError(f"Invalid streaming mode: {streaming_mode}")
 
     return endpoint
 
 
-class LangchainRouter(APIRouter):
-    def __init__(
-        self,
-        *,
-        langchain_url: str = "/chat",
-        langchain_object: Type[Chain] = Chain,
-        langchain_endpoint_kwargs: dict[str, Any] = None,
-        streaming_mode: StreamingMode = StreamingMode.OFF,
-        **kwargs,
-    ):
-        super().__init__(**kwargs)
-        self.langchain_url = langchain_url
-        self.langchain_object = langchain_object
-        self.langchain_endpoint_kwargs = langchain_endpoint_kwargs or {}
-        self.streaming_mode = streaming_mode
-
-        self.langchain_dependency = create_langchain_dependency(langchain_object)
-
-        self.setup()
-
-    def setup(self) -> None:
-        if self.langchain_url:
-            endpoint_request = create_request_from_langchain_dependency(
-                self.langchain_dependency
-            )
-            response_model = (
-                create_response_model_from_langchain_dependency(
-                    self.langchain_dependency
-                )
-                if self.streaming_mode == StreamingMode.OFF
-                else None
-            )
-            endpoint = create_langchain_endpoint(
-                endpoint_request,
-                self.langchain_dependency,
-                response_model,
-                self.streaming_mode,
-            )
-
-            self.add_api_route(
-                self.langchain_url,
-                endpoint,
-                response_model=response_model,
-                methods=["POST"],
-                **self.langchain_endpoint_kwargs,
-            )
+def create_langchain_websocket_endpoint(
+    websocket: Type[WebSocket], langchain_dependency: params.Depends
+):
+    async def endpoint(
+        websocket: websocket,
+        langchain_object: Chain = langchain_dependency,
+    ) -> None:
+        """Websocket chat endpoint."""
+        connection = WebsocketConnection.from_chain(
+            chain=langchain_object, websocket=websocket
+        )
+        await connection.connect()
+
+    return endpoint
```

### Comparing `lanarky-0.7.0/lanarky/schemas.py` & `lanarky-0.7.1/lanarky/schemas.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/lanarky/testing/gradio.py` & `lanarky-0.7.1/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/lanarky/websockets/base.py` & `lanarky-0.7.1/lanarky/websockets/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.0/pyproject.toml` & `lanarky-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.7.0"
+version = "0.7.1"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
```

### Comparing `lanarky-0.7.0/PKG-INFO` & `lanarky-0.7.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.7.0
+Version: 0.7.1
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -72,18 +72,20 @@
 
 from lanarky.routing import LangchainRouter
 
 load_dotenv()
 app = FastAPI()
 
 langchain_router = LangchainRouter(
+    url="/chat",
     langchain_object=ConversationChain(
         llm=ChatOpenAI(temperature=0), verbose=True
-    )
-)
+    ),
+    streaming_mode=0
+  )
 app.include_router(langchain_router)
 ```
 
 See [`examples/`](https://github.com/ajndkr/lanarky/blob/main/examples/README.md)
 for list of available demo examples.
 
 Create a `.env` file using `.env.sample` and add your OpenAI API key to it
```


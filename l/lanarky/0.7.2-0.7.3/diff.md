# Comparing `tmp/lanarky-0.7.2.tar.gz` & `tmp/lanarky-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lanarky-0.7.2.tar", max compression
+gzip compressed data, was "lanarky-0.7.3.tar", max compression
```

## Comparing `lanarky-0.7.2.tar` & `lanarky-0.7.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
--rw-r--r--   0        0        0     1073 2023-05-29 09:35:50.355512 lanarky-0.7.2/LICENSE
--rw-r--r--   0        0        0     4289 2023-05-29 09:35:50.355512 lanarky-0.7.2/README.md
--rw-r--r--   0        0        0        0 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/__init__.py
--rw-r--r--   0        0        0     2874 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/callbacks/__init__.py
--rw-r--r--   0        0        0     3023 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/callbacks/agents.py
--rw-r--r--   0        0        0     2200 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/callbacks/base.py
--rw-r--r--   0        0        0     1685 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/callbacks/llm.py
--rw-r--r--   0        0        0     3461 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/callbacks/retrieval_qa.py
--rw-r--r--   0        0        0     2004 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/register.py
--rw-r--r--   0        0        0       74 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/responses/__init__.py
--rw-r--r--   0        0        0     2926 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/responses/streaming.py
--rw-r--r--   0        0        0       70 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/routing/__init__.py
--rw-r--r--   0        0        0     3092 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/routing/langchain.py
--rw-r--r--   0        0        0     4207 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/routing/utils.py
--rw-r--r--   0        0        0      715 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/schemas.py
--rw-r--r--   0        0        0       69 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/testing/__init__.py
--rw-r--r--   0        0        0     3212 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/testing/gradio.py
--rw-r--r--   0        0        0      391 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/testing/settings.py
--rw-r--r--   0        0        0       73 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/websockets/__init__.py
--rw-r--r--   0        0        0     3844 2023-05-29 09:35:50.559514 lanarky-0.7.2/lanarky/websockets/base.py
--rw-r--r--   0        0        0     1110 2023-05-29 09:35:50.559514 lanarky-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     5110 1970-01-01 00:00:00.000000 lanarky-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-29 18:18:26.617325 lanarky-0.7.3/LICENSE
+-rw-r--r--   0        0        0     4348 2023-05-29 18:18:26.617325 lanarky-0.7.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/__init__.py
+-rw-r--r--   0        0        0     2874 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/callbacks/__init__.py
+-rw-r--r--   0        0        0     3023 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/callbacks/agents.py
+-rw-r--r--   0        0        0     2200 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/callbacks/base.py
+-rw-r--r--   0        0        0     1685 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/callbacks/llm.py
+-rw-r--r--   0        0        0     3461 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/callbacks/retrieval_qa.py
+-rw-r--r--   0        0        0      422 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/register/__init__.py
+-rw-r--r--   0        0        0     1047 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/register/base.py
+-rw-r--r--   0        0        0     1014 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/register/callbacks.py
+-rw-r--r--   0        0        0       74 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/responses/__init__.py
+-rw-r--r--   0        0        0     2926 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/responses/streaming.py
+-rw-r--r--   0        0        0      150 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/routing/__init__.py
+-rw-r--r--   0        0        0     5266 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/routing/langchain.py
+-rw-r--r--   0        0        0     4299 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/routing/utils.py
+-rw-r--r--   0        0        0      715 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/schemas.py
+-rw-r--r--   0        0        0       69 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/testing/__init__.py
+-rw-r--r--   0        0        0     3212 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/testing/gradio.py
+-rw-r--r--   0        0        0      391 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/testing/settings.py
+-rw-r--r--   0        0        0       73 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/websockets/__init__.py
+-rw-r--r--   0        0        0     3844 2023-05-29 18:18:26.813325 lanarky-0.7.3/lanarky/websockets/base.py
+-rw-r--r--   0        0        0     1270 2023-05-29 18:18:26.813325 lanarky-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     5337 1970-01-01 00:00:00.000000 lanarky-0.7.3/PKG-INFO
```

### Comparing `lanarky-0.7.2/LICENSE` & `lanarky-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.2/README.md` & `lanarky-0.7.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <img src="https://raw.githubusercontent.com/ajndkr/lanarky/main/assets/logo.png" alt="lanarky-logo" width="150">
 
 <h1> Lanarky </h1>
 
 [![stars](https://img.shields.io/github/stars/ajndkr/lanarky)](https://github.com/ajndkr/lanarky/stargazers)
 [![Documentation](https://img.shields.io/badge/documentation-ReadTheDocs-blue.svg)](https://lanarky.readthedocs.io/en/latest/)
 [![PyPI version](https://badge.fury.io/py/lanarky.svg)](https://pypi.org/project/lanarky/)
-![Supported Python Versions](https://img.shields.io/pypi/pyversions/lanarky.svg)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/lanarky.svg)](https://pypi.org/project/lanarky/)
 [![Code Coverage](https://coveralls.io/repos/github/ajndkr/lanarky/badge.svg?branch=main)](https://coveralls.io/github/ajndkr/lanarky?branch=main)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/lanarky/blob/main/LICENSE)
 
 </div>
 
 Lanarky is an open-source framework to deploy LLM applications in production. It is built on top of [FastAPI](https://github.com/tiangolo/fastapi)
 and comes with batteries included.
@@ -71,18 +71,18 @@
 
 ![demo](https://raw.githubusercontent.com/ajndkr/lanarky/main/assets/demo.gif)
 
 ## 📍 Roadmap
 
 - [x] Add support for [LangChain](https://github.com/hwchase17/langchain)
 - [x] Add [Gradio](https://github.com/gradio-app/gradio) UI for fast prototyping
-- [ ] Add SQL database integration
-- [ ] Add support for [Guardrails](https://github.com/ShreyaR/guardrails)
+- [x] Add support for in-memory, Redis and [GPTCache](https://github.com/zilliztech/GPTCache) LLM caching
 - [ ] Add support for [LlamaIndex](https://github.com/jerryjliu/llama_index)
-- [ ] Add [GPTCache](https://github.com/zilliztech/GPTCache) integration
+- [ ] Add SQL database integration
+- [ ] Add support for [Rebuff](https://github.com/woop/rebuff)
 
 ## 🤩 Stargazers
 
 Leave a ⭐ if you find this project useful.
 
 [![Star History Chart](https://api.star-history.com/svg?repos=ajndkr/lanarky&type=Date)](https://star-history.com/#ajndkr/lanarky&Date)
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
                                 [lanarky-logo]
                              ****** Lanarky ******
     [![stars](https://img.shields.io/github/stars/ajndkr/lanarky)](https://
 github.com/ajndkr/lanarky/stargazers) [![Documentation](https://img.shields.io/
  badge/documentation-ReadTheDocs-blue.svg)](https://lanarky.readthedocs.io/en/
    latest/) [![PyPI version](https://badge.fury.io/py/lanarky.svg)](https://
-pypi.org/project/lanarky/) ![Supported Python Versions](https://img.shields.io/
-  pypi/pyversions/lanarky.svg) [![Code Coverage](https://coveralls.io/repos/
-  github/ajndkr/lanarky/badge.svg?branch=main)](https://coveralls.io/github/
-  ajndkr/lanarky?branch=main) [![License: MIT](https://img.shields.io/badge/
- License-MIT-yellow.svg)](https://github.com/ajndkr/lanarky/blob/main/LICENSE)
+       pypi.org/project/lanarky/) [![Supported Python Versions](https://
+img.shields.io/pypi/pyversions/lanarky.svg)](https://pypi.org/project/lanarky/
+     ) [![Code Coverage](https://coveralls.io/repos/github/ajndkr/lanarky/
+badge.svg?branch=main)](https://coveralls.io/github/ajndkr/lanarky?branch=main)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
+                 github.com/ajndkr/lanarky/blob/main/LICENSE)
 Lanarky is an open-source framework to deploy LLM applications in production.
 It is built on top of [FastAPI](https://github.com/tiangolo/fastapi) and comes
 with batteries included. ## ð Features - supports [LangChain](https://
 github.com/hwchase17/langchain) - simple gradio chatbot UI for fast prototyping
 See [Roadmap](#-roadmap) for upcoming features. ## â Why? There are great
 low-code/no-code solutions in the open source to deploy your LLM projects.
 However, most of them are opinionated in terms of cloud or deployment code.
@@ -30,24 +31,24 @@
 ), streaming_mode=0 ) app.include_router(langchain_router) ``` See [`examples/
 `](https://github.com/ajndkr/lanarky/blob/main/examples/README.md) for list of
 available demo examples. Create a `.env` file using `.env.sample` and add your
 OpenAI API key to it before running the examples. ![demo](https://
 raw.githubusercontent.com/ajndkr/lanarky/main/assets/demo.gif) ## ð Roadmap
 - [x] Add support for [LangChain](https://github.com/hwchase17/langchain) - [x]
 Add [Gradio](https://github.com/gradio-app/gradio) UI for fast prototyping -
-[ ] Add SQL database integration - [ ] Add support for [Guardrails](https://
-github.com/ShreyaR/guardrails) - [ ] Add support for [LlamaIndex](https://
-github.com/jerryjliu/llama_index) - [ ] Add [GPTCache](https://github.com/
-zilliztech/GPTCache) integration ## ð¤© Stargazers Leave a â­ if you find
-this project useful. [![Star History Chart](https://api.star-history.com/
-svg?repos=ajndkr/lanarky&type=Date)](https://star-history.com/#ajndkr/
-lanarky&Date) ## ð¤ Contributing [![Code check](https://github.com/ajndkr/
-lanarky/actions/workflows/code-check.yaml/badge.svg)](https://github.com/
-ajndkr/lanarky/actions/workflows/code-check.yaml) [![Publish](https://
-github.com/ajndkr/lanarky/actions/workflows/publish.yaml/badge.svg)](https://
+[x] Add support for in-memory, Redis and [GPTCache](https://github.com/
+zilliztech/GPTCache) LLM caching - [ ] Add support for [LlamaIndex](https://
+github.com/jerryjliu/llama_index) - [ ] Add SQL database integration - [ ] Add
+support for [Rebuff](https://github.com/woop/rebuff) ## ð¤© Stargazers Leave a
+â­ if you find this project useful. [![Star History Chart](https://api.star-
+history.com/svg?repos=ajndkr/lanarky&type=Date)](https://star-history.com/
+#ajndkr/lanarky&Date) ## ð¤ Contributing [![Code check](https://github.com/
+ajndkr/lanarky/actions/workflows/code-check.yaml/badge.svg)](https://
+github.com/ajndkr/lanarky/actions/workflows/code-check.yaml) [![Publish](https:
+//github.com/ajndkr/lanarky/actions/workflows/publish.yaml/badge.svg)](https://
 github.com/ajndkr/lanarky/actions/workflows/publish.yaml) Contributions are
 more than welcome! If you have an idea for a new feature or want to help
 improve lanarky, please create an issue or submit a pull request on [GitHub]
 (https://github.com/ajndkr/lanarky). See [CONTRIBUTING.md](https://github.com/
 ajndkr/lanarky/blob/main/CONTRIBUTING.md) for more information. ###
 Contributors [![](https://img.shields.io/github/contributors-anon/ajndkr/
 lanarky)](https://github.com/ajndkr/lanarky/graphs/contributors) [https://
```

### Comparing `lanarky-0.7.2/lanarky/callbacks/__init__.py` & `lanarky-0.7.3/lanarky/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.2/lanarky/callbacks/agents.py` & `lanarky-0.7.3/lanarky/callbacks/agents.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.2/lanarky/callbacks/base.py` & `lanarky-0.7.3/lanarky/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.2/lanarky/callbacks/llm.py` & `lanarky-0.7.3/lanarky/callbacks/llm.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.2/lanarky/callbacks/retrieval_qa.py` & `lanarky-0.7.3/lanarky/callbacks/retrieval_qa.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.2/lanarky/responses/streaming.py` & `lanarky-0.7.3/lanarky/responses/streaming.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.2/lanarky/routing/utils.py` & `lanarky-0.7.3/lanarky/routing/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,14 +12,21 @@
 
 class StreamingMode(IntEnum):
     OFF = 0
     TEXT = 1
     JSON = 2
 
 
+class LLMCacheMode(IntEnum):
+    OFF = 0
+    IN_MEMORY = 1
+    REDIS = 2
+    GPTCACHE = 3
+
+
 def create_langchain_dependency(langchain_object: Type[Chain]) -> params.Depends:
     """Creates a langchain object dependency."""
 
     @lru_cache(maxsize=1)
     def dependency() -> Chain:
         return langchain_object
```

### Comparing `lanarky-0.7.2/lanarky/schemas.py` & `lanarky-0.7.3/lanarky/schemas.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.2/lanarky/testing/gradio.py` & `lanarky-0.7.3/lanarky/testing/gradio.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.2/lanarky/websockets/base.py` & `lanarky-0.7.3/lanarky/websockets/base.py`

 * *Files identical despite different names*

### Comparing `lanarky-0.7.2/pyproject.toml` & `lanarky-0.7.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lanarky"
-version = "0.7.2"
+version = "0.7.3"
 description = "Ship production-ready LLM projects with FastAPI"
 authors = ["Ajinkya Indulkar <26824103+ajndkr@users.noreply.github.com>"]
 readme = "README.md"
 homepage = "https://github.com/ajndkr/lanarky"
 repository = "https://github.com/ajndkr/lanarky"
 license = "MIT"
 packages = [{include = "lanarky"}]
@@ -12,14 +12,16 @@
 [tool.poetry.dependencies]
 python = "^3.9"
 fastapi = ">=0.95.2"
 langchain = ">=0.0.183"
 urllib3 = "<=1.26.15"  # added due to poetry errors
 python-dotenv = "^1.0.0"
 typing-extensions = "4.5.0"  # added due to https://github.com/hwchase17/langchain/issues/5113
+redis = {version = "^4.5.5", optional = true}
+gptcache = {version = "^0.1.28", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.1"
 
 
 [tool.poetry.group.docs.dependencies]
 furo = "^2023.3.27"
@@ -32,13 +34,17 @@
 
 [tool.poetry.group.tests.dependencies]
 pytest = "^7.3.1"
 pytest-cov = "^4.0.0"
 pytest-asyncio = "^0.21.0"
 coveralls = "^3.3.1"
 
+[tool.poetry.extras]
+redis = ["redis"]
+gptcache = ["gptcache"]
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 ignore = ["E501"]
```

### Comparing `lanarky-0.7.2/PKG-INFO` & `lanarky-0.7.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,39 +1,43 @@
 Metadata-Version: 2.1
 Name: lanarky
-Version: 0.7.2
+Version: 0.7.3
 Summary: Ship production-ready LLM projects with FastAPI
 Home-page: https://github.com/ajndkr/lanarky
 License: MIT
 Author: Ajinkya Indulkar
 Author-email: 26824103+ajndkr@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: gptcache
+Provides-Extra: redis
 Requires-Dist: fastapi (>=0.95.2)
+Requires-Dist: gptcache (>=0.1.28,<0.2.0) ; extra == "gptcache"
 Requires-Dist: langchain (>=0.0.183)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
+Requires-Dist: redis (>=4.5.5,<5.0.0) ; extra == "redis"
 Requires-Dist: typing-extensions (==4.5.0)
 Requires-Dist: urllib3 (<=1.26.15)
 Project-URL: Repository, https://github.com/ajndkr/lanarky
 Description-Content-Type: text/markdown
 
 <div align="center">
 
 <img src="https://raw.githubusercontent.com/ajndkr/lanarky/main/assets/logo.png" alt="lanarky-logo" width="150">
 
 <h1> Lanarky </h1>
 
 [![stars](https://img.shields.io/github/stars/ajndkr/lanarky)](https://github.com/ajndkr/lanarky/stargazers)
 [![Documentation](https://img.shields.io/badge/documentation-ReadTheDocs-blue.svg)](https://lanarky.readthedocs.io/en/latest/)
 [![PyPI version](https://badge.fury.io/py/lanarky.svg)](https://pypi.org/project/lanarky/)
-![Supported Python Versions](https://img.shields.io/pypi/pyversions/lanarky.svg)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/lanarky.svg)](https://pypi.org/project/lanarky/)
 [![Code Coverage](https://coveralls.io/repos/github/ajndkr/lanarky/badge.svg?branch=main)](https://coveralls.io/github/ajndkr/lanarky?branch=main)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/ajndkr/lanarky/blob/main/LICENSE)
 
 </div>
 
 Lanarky is an open-source framework to deploy LLM applications in production. It is built on top of [FastAPI](https://github.com/tiangolo/fastapi)
 and comes with batteries included.
@@ -93,18 +97,18 @@
 
 ![demo](https://raw.githubusercontent.com/ajndkr/lanarky/main/assets/demo.gif)
 
 ## 📍 Roadmap
 
 - [x] Add support for [LangChain](https://github.com/hwchase17/langchain)
 - [x] Add [Gradio](https://github.com/gradio-app/gradio) UI for fast prototyping
-- [ ] Add SQL database integration
-- [ ] Add support for [Guardrails](https://github.com/ShreyaR/guardrails)
+- [x] Add support for in-memory, Redis and [GPTCache](https://github.com/zilliztech/GPTCache) LLM caching
 - [ ] Add support for [LlamaIndex](https://github.com/jerryjliu/llama_index)
-- [ ] Add [GPTCache](https://github.com/zilliztech/GPTCache) integration
+- [ ] Add SQL database integration
+- [ ] Add support for [Rebuff](https://github.com/woop/rebuff)
 
 ## 🤩 Stargazers
 
 Leave a ⭐ if you find this project useful.
 
 [![Star History Chart](https://api.star-history.com/svg?repos=ajndkr/lanarky&type=Date)](https://star-history.com/#ajndkr/lanarky&Date)
```


# Comparing `tmp/speechai-0.0.2.tar.gz` & `tmp/speechai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speechai-0.0.2.tar", max compression
+gzip compressed data, was "speechai-0.0.3.tar", max compression
```

## Comparing `speechai-0.0.2.tar` & `speechai-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1063 2023-05-23 11:48:09.668514 speechai-0.0.2/LICENSE
--rw-r--r--   0        0        0     1224 2023-05-23 11:48:09.668514 speechai-0.0.2/README.md
--rw-r--r--   0        0        0      919 2023-05-23 11:48:09.668514 speechai-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       44 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/core/__init__.py
--rw-r--r--   0        0        0      879 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/core/speechai.py
--rw-r--r--   0        0        0       65 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/llm/__init__.py
--rw-r--r--   0        0        0      137 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/llm/abstract_llm.py
--rw-r--r--   0        0        0      404 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/llm/openai.py
--rw-r--r--   0        0        0       61 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/tts/__init__.py
--rw-r--r--   0        0        0      232 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/tts/abstract_tts.py
--rw-r--r--   0        0        0      626 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/tts/gtts.py
--rw-r--r--   0        0        0       50 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/utils/__init__.py
--rw-r--r--   0        0        0      402 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/utils/directory.py
--rw-r--r--   0        0        0      535 2023-05-23 11:48:09.668514 speechai-0.0.2/speechai/utils/logger.py
--rw-r--r--   0        0        0     2002 1970-01-01 00:00:00.000000 speechai-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-29 14:32:27.159695 speechai-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4631 2023-05-29 14:32:27.159695 speechai-0.0.3/README.md
+-rw-r--r--   0        0        0      987 2023-05-29 14:32:27.159695 speechai-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/core/__init__.py
+-rw-r--r--   0        0        0      879 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/core/speechai.py
+-rw-r--r--   0        0        0       92 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/llm/__init__.py
+-rw-r--r--   0        0        0      137 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/llm/abstract_llm.py
+-rw-r--r--   0        0        0      373 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/llm/cohere.py
+-rw-r--r--   0        0        0      449 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/llm/openai.py
+-rw-r--r--   0        0        0       61 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/tts/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/tts/abstract_tts.py
+-rw-r--r--   0        0        0      626 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/tts/gtts.py
+-rw-r--r--   0        0        0       50 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/utils/__init__.py
+-rw-r--r--   0        0        0      402 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/utils/directory.py
+-rw-r--r--   0        0        0      535 2023-05-29 14:32:27.159695 speechai-0.0.3/speechai/utils/logger.py
+-rw-r--r--   0        0        0     5467 1970-01-01 00:00:00.000000 speechai-0.0.3/PKG-INFO
```

### Comparing `speechai-0.0.2/pyproject.toml` & `speechai-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 [tool.poetry]
 name = "speechai"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Python package that generates conversational speech from text using a combination of Generative AI models and various text-to-speech engines, enabling applications to produce dynamic and contextually aware spoken responses."
 authors = ['Nicola Sebastianelli']
-license = "MIT"
+license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "speechai"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 openai = "^0.27.7"
 python-dotenv = "^1.0.0"
 gtts = "^2.3.2"
+cohere = "^4.5.1"
 
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
 pytest = "^7.3.1"
 pylint = "^2.17.4"
 black = "^23.3.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 pytest-mock = "^3.10.0"
+pytest-cov = "^4.0.0"
+coverage = "^7.2.6"
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
```

### Comparing `speechai-0.0.2/speechai/core/speechai.py` & `speechai-0.0.3/speechai/core/speechai.py`

 * *Files identical despite different names*

### Comparing `speechai-0.0.2/speechai/tts/gtts.py` & `speechai-0.0.3/speechai/tts/gtts.py`

 * *Files identical despite different names*

### Comparing `speechai-0.0.2/speechai/utils/logger.py` & `speechai-0.0.3/speechai/utils/logger.py`

 * *Files identical despite different names*


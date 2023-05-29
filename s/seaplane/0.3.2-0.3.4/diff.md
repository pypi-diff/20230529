# Comparing `tmp/seaplane-0.3.2.tar.gz` & `tmp/seaplane-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaplane-0.3.2.tar", max compression
+gzip compressed data, was "seaplane-0.3.4.tar", max compression
```

## Comparing `seaplane-0.3.2.tar` & `seaplane-0.3.4.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1538 2023-05-10 16:05:26.809759 seaplane-0.3.2/README.md
--rw-r--r--   0        0        0     2501 2023-05-15 18:10:10.506955 seaplane-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      925 2023-05-10 16:07:33.886849 seaplane-0.3.2/src/seaplane/__init__.py
--rw-r--r--   0        0        0       84 2023-05-10 16:07:33.887055 seaplane-0.3.2/src/seaplane/api/__init__.py
--rw-r--r--   0        0        0      527 2023-05-10 16:07:33.887179 seaplane-0.3.2/src/seaplane/api/api_http.py
--rw-r--r--   0        0        0     2558 2023-05-10 16:07:33.887328 seaplane-0.3.2/src/seaplane/api/api_request.py
--rw-r--r--   0        0        0     2987 2023-05-10 16:07:33.887468 seaplane-0.3.2/src/seaplane/api/compute_api.py
--rw-r--r--   0        0        0     3158 2023-05-10 16:07:33.887602 seaplane-0.3.2/src/seaplane/api/formation_configuration_api.py
--rw-r--r--   0        0        0     7410 2023-05-10 16:07:33.887749 seaplane-0.3.2/src/seaplane/api/lock_api.py
--rw-r--r--   0        0        0     5806 2023-05-10 16:07:33.887880 seaplane-0.3.2/src/seaplane/api/metadata_api.py
--rw-r--r--   0        0        0     7724 2023-05-10 16:07:33.888017 seaplane-0.3.2/src/seaplane/api/restrict_api.py
--rw-r--r--   0        0        0     1552 2023-05-10 16:07:33.888145 seaplane-0.3.2/src/seaplane/api/sql_api.py
--rw-r--r--   0        0        0     3141 2023-05-10 16:07:33.888286 seaplane-0.3.2/src/seaplane/api/token_api.py
--rw-r--r--   0        0        0     6898 2023-05-15 17:39:26.659040 seaplane-0.3.2/src/seaplane/configuration.py
--rw-r--r--   0        0        0     1818 2023-05-10 16:07:33.888625 seaplane-0.3.2/src/seaplane/logging/__init__.py
--rw-r--r--   0        0        0      213 2023-05-10 16:07:33.888776 seaplane-0.3.2/src/seaplane/model/__init__.py
--rw-r--r--   0        0        0     1310 2023-05-10 16:07:33.888946 seaplane-0.3.2/src/seaplane/model/compute/__init__.py
--rw-r--r--   0        0        0     1539 2023-05-10 16:07:33.889076 seaplane-0.3.2/src/seaplane/model/compute/formation_configuration.py
--rw-r--r--   0        0        0      129 2023-05-10 16:07:33.889214 seaplane-0.3.2/src/seaplane/model/compute/formation_metadata.py
--rw-r--r--   0        0        0      436 2023-05-10 16:07:33.889338 seaplane-0.3.2/src/seaplane/model/errors.py
--rw-r--r--   0        0        0     3077 2023-05-10 16:07:33.889518 seaplane-0.3.2/src/seaplane/model/locks/__init__.py
--rw-r--r--   0        0        0     3560 2023-05-10 16:07:33.889686 seaplane-0.3.2/src/seaplane/model/metadata/__init__.py
--rw-r--r--   0        0        0      422 2023-05-10 16:07:33.889804 seaplane-0.3.2/src/seaplane/model/provider.py
--rw-r--r--   0        0        0      478 2023-05-10 16:07:33.889921 seaplane-0.3.2/src/seaplane/model/region.py
--rw-r--r--   0        0        0     4221 2023-05-10 16:07:33.890085 seaplane-0.3.2/src/seaplane/model/restrict/__init__.py
--rw-r--r--   0        0        0      530 2023-05-10 16:07:33.890271 seaplane-0.3.2/src/seaplane/model/sql/__init__.py
--rw-r--r--   0        0        0      167 2023-05-10 16:07:33.890455 seaplane-0.3.2/src/seaplane/smartpipes/__init__.py
--rw-r--r--   0        0        0     6283 2023-05-15 16:36:35.977595 seaplane-0.3.2/src/seaplane/smartpipes/coprocessor.py
--rw-r--r--   0        0        0     7507 2023-05-15 16:36:35.993328 seaplane-0.3.2/src/seaplane/smartpipes/decorators.py
--rw-r--r--   0        0        0     1573 2023-05-15 18:10:03.263921 seaplane-0.3.2/src/seaplane/smartpipes/smartapi.py
--rw-r--r--   0        0        0     1420 2023-05-10 16:07:33.891062 seaplane-0.3.2/src/seaplane/smartpipes/smartpipe.py
--rw-r--r--   0        0        0       18 2023-05-10 16:07:33.891248 seaplane-0.3.2/src/seaplane/smartpipes/website/.gitignore
--rw-r--r--   0        0        0     1750 2023-05-10 16:07:33.891373 seaplane-0.3.2/src/seaplane/smartpipes/website/README.md
--rw-r--r--   0        0        0       77 2023-05-10 16:07:33.891483 seaplane-0.3.2/src/seaplane/smartpipes/website/jsconfig.json
--rw-r--r--   0        0        0      118 2023-05-10 16:07:33.891598 seaplane-0.3.2/src/seaplane/smartpipes/website/next.config.js
--rw-r--r--   0        0        0      650 2023-05-10 17:50:07.644968 seaplane-0.3.2/src/seaplane/smartpipes/website/package.json
--rw-r--r--   0        0        0       82 2023-05-10 16:07:33.891848 seaplane-0.3.2/src/seaplane/smartpipes/website/postcss.config.js
--rw-r--r--   0        0        0      717 2023-05-10 16:07:33.892035 seaplane-0.3.2/src/seaplane/smartpipes/website/public/favicon.ico
--rw-r--r--   0        0        0     1375 2023-05-10 16:07:33.892164 seaplane-0.3.2/src/seaplane/smartpipes/website/public/next.svg
--rw-r--r--   0        0        0    39147 2023-05-10 16:07:33.892577 seaplane-0.3.2/src/seaplane/smartpipes/website/public/openai.png
--rw-r--r--   0        0        0    11580 2023-05-10 16:07:33.892822 seaplane-0.3.2/src/seaplane/smartpipes/website/public/seaplane_logo.svg
--rw-r--r--   0        0        0     2296 2023-05-10 16:07:33.892979 seaplane-0.3.2/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg
--rw-r--r--   0        0        0   195272 2023-05-10 16:07:33.894399 seaplane-0.3.2/src/seaplane/smartpipes/website/public/stabilityai.png
--rw-r--r--   0        0        0      629 2023-05-10 16:07:33.894546 seaplane-0.3.2/src/seaplane/smartpipes/website/public/vercel.svg
--rw-r--r--   0        0        0     3691 2023-05-10 16:07:33.894773 seaplane-0.3.2/src/seaplane/smartpipes/website/src/components/Header.jsx
--rw-r--r--   0        0        0    10990 2023-05-10 16:07:33.894919 seaplane-0.3.2/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx
--rw-r--r--   0        0        0     4313 2023-05-10 17:56:17.012227 seaplane-0.3.2/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx
--rw-r--r--   0        0        0      127 2023-05-10 16:07:33.895187 seaplane-0.3.2/src/seaplane/smartpipes/website/src/pages/_app.js
--rw-r--r--   0        0        0      231 2023-05-10 16:07:33.895300 seaplane-0.3.2/src/seaplane/smartpipes/website/src/pages/_document.js
--rw-r--r--   0        0        0     1962 2023-05-10 17:40:10.004727 seaplane-0.3.2/src/seaplane/smartpipes/website/src/pages/index.js
--rw-r--r--   0        0        0     2626 2023-05-10 18:08:41.619834 seaplane-0.3.2/src/seaplane/smartpipes/website/src/pages/tutorial.js
--rw-r--r--   0        0        0      228 2023-05-10 16:07:33.895550 seaplane-0.3.2/src/seaplane/smartpipes/website/src/styles/globals.css
--rw-r--r--   0        0        0      528 2023-05-10 17:31:27.541316 seaplane-0.3.2/src/seaplane/smartpipes/website/tailwind.config.js
--rw-r--r--   0        0        0     1762 2023-05-10 16:07:33.895787 seaplane-0.3.2/src/seaplane/smartpipes/website/yarn-error.log
--rw-r--r--   0        0        0   143162 2023-05-10 17:50:07.642910 seaplane-0.3.2/src/seaplane/smartpipes/website/yarn.lock
--rw-r--r--   0        0        0      424 2023-05-10 16:07:33.896564 seaplane-0.3.2/src/seaplane/util/__init__.py
--rw-r--r--   0        0        0      318 2023-05-10 16:07:33.896679 seaplane-0.3.2/src/seaplane/util/base64url.py
--rw-r--r--   0        0        0     7206 2023-05-15 18:11:14.478100 seaplane-0.3.2/setup.py
--rw-r--r--   0        0        0     2988 2023-05-15 18:11:14.478653 seaplane-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1538 2023-05-10 16:05:26.809759 seaplane-0.3.4/README.md
+-rw-r--r--   0        0        0     2682 2023-05-29 16:57:26.458011 seaplane-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     1120 2023-05-26 12:37:12.573449 seaplane-0.3.4/src/seaplane/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-10 16:07:33.887055 seaplane-0.3.4/src/seaplane/api/__init__.py
+-rw-r--r--   0        0        0      527 2023-05-10 16:07:33.887179 seaplane-0.3.4/src/seaplane/api/api_http.py
+-rw-r--r--   0        0        0     2558 2023-05-26 12:37:12.574515 seaplane-0.3.4/src/seaplane/api/api_request.py
+-rw-r--r--   0        0        0     2987 2023-05-10 16:07:33.887468 seaplane-0.3.4/src/seaplane/api/compute_api.py
+-rw-r--r--   0        0        0     3158 2023-05-10 16:07:33.887602 seaplane-0.3.4/src/seaplane/api/formation_configuration_api.py
+-rw-r--r--   0        0        0     7410 2023-05-10 16:07:33.887749 seaplane-0.3.4/src/seaplane/api/lock_api.py
+-rw-r--r--   0        0        0     5806 2023-05-10 16:07:33.887880 seaplane-0.3.4/src/seaplane/api/metadata_api.py
+-rw-r--r--   0        0        0     7724 2023-05-10 16:07:33.888017 seaplane-0.3.4/src/seaplane/api/restrict_api.py
+-rw-r--r--   0        0        0     1552 2023-05-10 16:07:33.888145 seaplane-0.3.4/src/seaplane/api/sql_api.py
+-rw-r--r--   0        0        0     3141 2023-05-10 16:07:33.888286 seaplane-0.3.4/src/seaplane/api/token_api.py
+-rw-r--r--   0        0        0     7075 2023-05-29 15:51:55.432747 seaplane-0.3.4/src/seaplane/configuration.py
+-rw-r--r--   0        0        0     1818 2023-05-26 12:37:12.575554 seaplane-0.3.4/src/seaplane/logging/__init__.py
+-rw-r--r--   0        0        0      213 2023-05-10 16:07:33.888776 seaplane-0.3.4/src/seaplane/model/__init__.py
+-rw-r--r--   0        0        0     1310 2023-05-10 16:07:33.888946 seaplane-0.3.4/src/seaplane/model/compute/__init__.py
+-rw-r--r--   0        0        0     1539 2023-05-10 16:07:33.889076 seaplane-0.3.4/src/seaplane/model/compute/formation_configuration.py
+-rw-r--r--   0        0        0      129 2023-05-10 16:07:33.889214 seaplane-0.3.4/src/seaplane/model/compute/formation_metadata.py
+-rw-r--r--   0        0        0      436 2023-05-10 16:07:33.889338 seaplane-0.3.4/src/seaplane/model/errors.py
+-rw-r--r--   0        0        0     3077 2023-05-10 16:07:33.889518 seaplane-0.3.4/src/seaplane/model/locks/__init__.py
+-rw-r--r--   0        0        0     3560 2023-05-10 16:07:33.889686 seaplane-0.3.4/src/seaplane/model/metadata/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-10 16:07:33.889804 seaplane-0.3.4/src/seaplane/model/provider.py
+-rw-r--r--   0        0        0      478 2023-05-10 16:07:33.889921 seaplane-0.3.4/src/seaplane/model/region.py
+-rw-r--r--   0        0        0     4221 2023-05-10 16:07:33.890085 seaplane-0.3.4/src/seaplane/model/restrict/__init__.py
+-rw-r--r--   0        0        0      530 2023-05-10 16:07:33.890271 seaplane-0.3.4/src/seaplane/model/sql/__init__.py
+-rw-r--r--   0        0        0      228 2023-05-26 12:37:12.575703 seaplane-0.3.4/src/seaplane/smartpipes/__init__.py
+-rw-r--r--   0        0        0     6919 2023-05-29 16:39:25.320434 seaplane-0.3.4/src/seaplane/smartpipes/coprocessor.py
+-rw-r--r--   0        0        0     8767 2023-05-29 16:37:53.773697 seaplane-0.3.4/src/seaplane/smartpipes/decorators.py
+-rw-r--r--   0        0        0     3435 2023-05-29 16:56:13.680134 seaplane-0.3.4/src/seaplane/smartpipes/smartapi.py
+-rw-r--r--   0        0        0     1810 2023-05-29 14:38:17.372462 seaplane-0.3.4/src/seaplane/smartpipes/smartpipe.py
+-rw-r--r--   0        0        0     2141 2023-05-29 16:25:30.567871 seaplane-0.3.4/src/seaplane/smartpipes/store.py
+-rw-r--r--   0        0        0       33 2023-05-29 06:02:49.125920 seaplane-0.3.4/src/seaplane/smartpipes/website/.gitignore
+-rw-r--r--   0        0        0     1750 2023-05-26 12:37:12.578128 seaplane-0.3.4/src/seaplane/smartpipes/website/README.md
+-rw-r--r--   0        0        0       77 2023-05-26 12:37:12.578349 seaplane-0.3.4/src/seaplane/smartpipes/website/jsconfig.json
+-rw-r--r--   0        0        0      118 2023-05-26 12:37:12.578651 seaplane-0.3.4/src/seaplane/smartpipes/website/next.config.js
+-rw-r--r--   0        0        0      650 2023-05-26 12:37:12.579148 seaplane-0.3.4/src/seaplane/smartpipes/website/package.json
+-rw-r--r--   0        0        0       82 2023-05-26 12:37:12.579367 seaplane-0.3.4/src/seaplane/smartpipes/website/postcss.config.js
+-rw-r--r--   0        0        0      717 2023-05-26 12:37:12.579749 seaplane-0.3.4/src/seaplane/smartpipes/website/public/favicon.ico
+-rw-r--r--   0        0        0     1375 2023-05-26 12:37:12.579990 seaplane-0.3.4/src/seaplane/smartpipes/website/public/next.svg
+-rw-r--r--   0        0        0    39147 2023-05-26 12:37:12.580576 seaplane-0.3.4/src/seaplane/smartpipes/website/public/openai.png
+-rw-r--r--   0        0        0    11580 2023-05-26 12:37:12.581026 seaplane-0.3.4/src/seaplane/smartpipes/website/public/seaplane_logo.svg
+-rw-r--r--   0        0        0     2296 2023-05-26 12:37:12.581272 seaplane-0.3.4/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg
+-rw-r--r--   0        0        0   195272 2023-05-26 12:37:12.582964 seaplane-0.3.4/src/seaplane/smartpipes/website/public/stabilityai.png
+-rw-r--r--   0        0        0      629 2023-05-26 12:37:12.583286 seaplane-0.3.4/src/seaplane/smartpipes/website/public/vercel.svg
+-rw-r--r--   0        0        0     3691 2023-05-26 12:37:12.583538 seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/Header.jsx
+-rw-r--r--   0        0        0    10990 2023-05-29 06:31:52.174486 seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx
+-rw-r--r--   0        0        0     4313 2023-05-26 12:37:12.584085 seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx
+-rw-r--r--   0        0        0      127 2023-05-26 12:37:12.584496 seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/_app.js
+-rw-r--r--   0        0        0      231 2023-05-26 12:37:12.584691 seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/_document.js
+-rw-r--r--   0        0        0     1962 2023-05-29 06:31:52.174956 seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/index.js
+-rw-r--r--   0        0        0     2626 2023-05-26 12:37:12.585484 seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/tutorial.js
+-rw-r--r--   0        0        0      228 2023-05-26 12:37:12.585759 seaplane-0.3.4/src/seaplane/smartpipes/website/src/styles/globals.css
+-rw-r--r--   0        0        0      528 2023-05-26 12:37:12.586061 seaplane-0.3.4/src/seaplane/smartpipes/website/tailwind.config.js
+-rw-r--r--   0        0        0   143162 2023-05-26 12:37:12.587625 seaplane-0.3.4/src/seaplane/smartpipes/website/yarn.lock
+-rw-r--r--   0        0        0      424 2023-05-10 16:07:33.896564 seaplane-0.3.4/src/seaplane/util/__init__.py
+-rw-r--r--   0        0        0      318 2023-05-10 16:07:33.896679 seaplane-0.3.4/src/seaplane/util/base64url.py
+-rw-r--r--   0        0        0     6545 2023-05-29 17:02:42.170563 seaplane-0.3.4/setup.py
+-rw-r--r--   0        0        0     3182 2023-05-29 17:02:42.170917 seaplane-0.3.4/PKG-INFO
```

### Comparing `seaplane-0.3.2/README.md` & `seaplane-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/pyproject.toml` & `seaplane-0.3.4/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "seaplane"
-version = "0.3.2"
+version = "0.3.4"
 description = "Seaplane Python SDK"
 authors = ["Seaplane IO, Inc."]
 license = "Apache License"
 readme = "README.md"
 repository = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 documentation = "https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python"
 
 
 [tool.poetry.dependencies]
-python = ">=3.8.*,<4.0"
+python = ">=3.10.*,<4.0"
 attrs = "21.4.0"
 certifi = "2022.6.15"
 charset-normalizer = "2.1.0"
 idna = "3.3"
 iniconfig = "1.1.1"
 packaging = "21.3"
 pluggy = "1.0.0"
@@ -26,14 +26,21 @@
 types-requests = "^2.28.0"
 returns = "^0.19.0"
 requests-mock = "^1.9.3"
 simplejson = "^3.17.6"
 types-simplejson = "^3.17.7"
 Flask-Cors = "^3.0.10"
 Flask-SocketIO = "^5.3.4"
+openai = "^0.27.7"
+tqdm = "^4.65.0"
+pinecone-client = "^2.2.1"
+tiktoken = "^0.4.0"
+pypdf = "^3.9.0"
+langchain = "^0.0.183"
+boto3 = "^1.26.142"
 
 [tool.poetry.dev-dependencies]
 nox-poetry = "*"
 
 # Testing.
 pytest = "*"
 pytest-cov = "*"
@@ -61,27 +68,28 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 ignore_missing_imports = true
 strict = true
+implicit_reexport = true
 # If certain strict config options are too pedantic for a project,
 # disable them selectively here by setting to false.
 
 # Note: This configuration is supported by pyproject-flake8.
 [tool.flake8]
 # Use the more relaxed max line length permitted in PEP 8.
 max-line-length = 99
 # This ignore is required by black.
 extend-ignore = ["E203"]
 # flake8-bugbear config.
 # TODO: Remove this once flake8 > 4.0.1 is released as this has been fixed
 #   upstream: https://github.com/PyCQA/flake8/pull/1443
-extend-exclude = [".nox", ".env"]
+extend-exclude = [".nox", ".env", "examples"]
 
 [tool.black]
 line-length = 99
 target-version = ["py38", "py39", "py310"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `seaplane-0.3.2/src/seaplane/__init__.py` & `seaplane-0.3.4/src/seaplane/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .api.compute_api import ComputeAPI
 from .api.lock_api import LockAPI
 from .api.metadata_api import MetadataAPI
 from .api.restrict_api import RestrictAPI
 from .api.sql_api import GlobalSQL
 from .api.token_api import TokenAPI
 from .configuration import Configuration, config
-from .smartpipes import *
+from .smartpipes import Coprocessor, SmartPipe, coprocessor, smartpipe, start  # noqa
+from .logging import log
 
 
 class Seaplane:
     @property
     def config(self) -> Configuration:
         return config
 
@@ -35,7 +36,16 @@
 
     @property
     def global_sql(self) -> GlobalSQL:
         return GlobalSQL(config)
 
 
 sea = Seaplane()
+
+__all__ = [
+    "SmartPipe",
+    "Coprocessor",
+    "coprocessor",
+    "smartpipe",
+    "start",
+    "log"
+]
```

### Comparing `seaplane-0.3.2/src/seaplane/api/api_http.py` & `seaplane-0.3.4/src/seaplane/api/api_http.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/api/api_request.py` & `seaplane-0.3.4/src/seaplane/api/api_request.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/api/compute_api.py` & `seaplane-0.3.4/src/seaplane/api/compute_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/api/formation_configuration_api.py` & `seaplane-0.3.4/src/seaplane/api/formation_configuration_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/api/lock_api.py` & `seaplane-0.3.4/src/seaplane/api/lock_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/api/metadata_api.py` & `seaplane-0.3.4/src/seaplane/api/metadata_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/api/restrict_api.py` & `seaplane-0.3.4/src/seaplane/api/restrict_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/api/sql_api.py` & `seaplane-0.3.4/src/seaplane/api/sql_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/api/token_api.py` & `seaplane-0.3.4/src/seaplane/api/token_api.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/configuration.py` & `seaplane-0.3.4/src/seaplane/configuration.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import os 
-
-from typing import Optional
+import os
+from typing import Dict, Optional
 
 from .api.token_api import TokenAPI
 from .logging import log
 from .model.errors import SeaplaneError
 
 _SEAPLANE_COMPUTE_API_ENDPOINT = "https://compute.cplane.cloud/v2beta"
 _SEAPLANE_COORDINATION_API_ENDPOINT = "https://metadata.cplane.cloud/v1"
 _SEAPLANE_IDENTIFY_API_ENDPOINT = "https://flightdeck.cplane.cloud/v1"
 _SEAPLANE_GLOBAL_SQL_API_ENDPOINT = "https://sql.cplane.cloud/v1"
 
 _SEAPLANE_ENV_VAR_PRODUCTION = "SEAPLANE_PRODUCTION"
 
+
 class Configuration:
     """
     Seaplane SDK Configuration.
 
     Everytime the configuration is changed,
     It'll clear local configurations to the default Auth module.
     """
@@ -25,15 +25,19 @@
         self.seaplane_api_key: Optional[str] = None
         self.identify_endpoint = _SEAPLANE_IDENTIFY_API_ENDPOINT
         self.compute_endpoint = _SEAPLANE_COMPUTE_API_ENDPOINT
         self.coordination_endpoint = _SEAPLANE_COORDINATION_API_ENDPOINT
         self.global_sql_endpoint = _SEAPLANE_GLOBAL_SQL_API_ENDPOINT
         self._current_access_token: Optional[str] = None
         self._token_auto_renew = True
-        self._api_keys: Optional[str] = None
+        self._api_keys: Dict[str, str] = {
+            "SEA_API_KEY": os.getenv("SEAPLANE_API_KEY"),
+            "OPENAI_API_KEY": os.getenv("OPENAI_API_KEY"),
+            "RE_API_KEY": os.getenv("RE_API_KEY"),
+        }
         self._production = False
         self._update_token_api()
 
     def set_api_key(self, api_key: str) -> None:
         """Set the Seaplane API Key.
 
         The API Key is needed for the Seaplane Python SDK usage.
@@ -42,15 +46,15 @@
         ----------
         api_key : str
             Seaplane API Key.
         """
         self.seaplane_api_key = api_key
         self._update_token_api()
 
-    def set_api_keys(self, api_keys: object) -> None:
+    def set_api_keys(self, api_keys: Dict[str, str]) -> None:
         """Set the Seaplane API Keys for SmartPipes.
 
         The API Keys is needed for some of the Coprocessors.
 
         Supported Coprocessors API Keys:
 
         Seaplane: SEA_API_KEY
@@ -199,19 +203,19 @@
         enable : bool
             True to enable, False to disable.
         """
         if enable:
             log.enable()
         else:
             log.disable()
-    
+
     def is_production(self) -> bool:
         if not self._production:
-            return os.getenv(_SEAPLANE_ENV_VAR_PRODUCTION) is True
-        
+            return os.getenv(_SEAPLANE_ENV_VAR_PRODUCTION) is not None
+
         return self._production
-    
+
     def set_production(self, is_production: bool) -> None:
         self._production = is_production
 
 
 config = Configuration()
```

### Comparing `seaplane-0.3.2/src/seaplane/logging/__init__.py` & `seaplane-0.3.4/src/seaplane/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/model/compute/__init__.py` & `seaplane-0.3.4/src/seaplane/model/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/model/compute/formation_configuration.py` & `seaplane-0.3.4/src/seaplane/model/compute/formation_configuration.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/model/locks/__init__.py` & `seaplane-0.3.4/src/seaplane/model/locks/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/model/metadata/__init__.py` & `seaplane-0.3.4/src/seaplane/model/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/model/restrict/__init__.py` & `seaplane-0.3.4/src/seaplane/model/restrict/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/model/sql/__init__.py` & `seaplane-0.3.4/src/seaplane/model/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/coprocessor.py` & `seaplane-0.3.4/src/seaplane/smartpipes/coprocessor.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,42 @@
+from typing import Any, Callable, Dict, Optional, Tuple
+
 import requests
 
 from ..api.api_http import headers
 from ..api.api_request import handle_request, provision_req
 from ..configuration import config
 from ..model.errors import SeaplaneError
 from ..util import unwrap
-
+from .store import Store
 
 class CoprocessorEvent:
-    def __init__(self, id=None, input=None):
+    def __init__(self, id: str, input: Any) -> None:
         self.id = id
         self.status = "in_progress"
         self.input = input
-        self.output = None
-        self.error = None
+        self.output: Optional[Any] = None
+        self.error: Optional[Any] = None
 
-    def set_ouput(self, output):
+    def set_ouput(self, output: Any) -> None:
         self.output = output
         self.status = "completed"
 
-    def set_error(self, error):
+    def set_error(self, error: Any) -> None:
         self.error = error
         self.status = "error"
 
 
 SEAPLANE_API_KEY_NAME = "SEA_API_KEY"
 OPENAI_API_KEY_NAME = "OPENAI_API_KEY"
 REPLICATE_API_KEY_NAME = "RE_API_KEY"
 
 
-def inference(version):
-    def model(input_data):
+def inference(version: str) -> Callable[[Dict[str, Any]], Any]:
+    def model(input_data: Dict[str, Any]) -> Any:
         if config._api_keys is None:
             raise SeaplaneError(
                 "Replicate API Key `RE_API_KEY` is not set, use `sea.config.set_api_keys`."
             )
         elif not config._api_keys.get(REPLICATE_API_KEY_NAME, None):
             raise SeaplaneError(
                 "Replicate API Key `RE_API_KEY` is not set, use `sea.config.set_api_keys`."
@@ -77,16 +79,16 @@
                         return result
         else:
             return response.text
 
     return model
 
 
-def bloom():
-    def model(input):
+def bloom() -> Callable[[Dict[str, Any]], Any]:
+    def model(input: Dict[str, Any]) -> Any:
         url = "https://substation.dev.cplane.cloud/v1/completions"
         req = provision_req(config._token_api)
 
         payload = {"prompt": input}
 
         return unwrap(
             req(
@@ -97,23 +99,23 @@
                 )
             )
         )
 
     return model
 
 
-def gpt_3():
-    def model(prompt):
+def gpt_3() -> Callable[[str], Any]:
+    def model(prompt: str) -> Any:
         if config._api_keys is None:
             raise SeaplaneError(
-                f"OPENAI API Key `{OPENAI_API_KEY_NAME}` is not set, use `sea.config.set_api_keys`."
+                f"OPENAI API Key `{OPENAI_API_KEY_NAME}` is not set, use `sea.config.set_api_keys`."  # noqa
             )
         elif not config._api_keys.get(OPENAI_API_KEY_NAME, None):
             raise SeaplaneError(
-                f"OPENAI API Key `{OPENAI_API_KEY_NAME}` is not set, use `sea.config.set_api_keys`."
+                f"OPENAI API Key `{OPENAI_API_KEY_NAME}` is not set, use `sea.config.set_api_keys`."  # noqa
             )
 
         url = "https://api.openai.com/v1/completions"
 
         payload = {"model": "text-davinci-003", "prompt": prompt, "temperature": 0}
 
         return unwrap(
@@ -125,23 +127,23 @@
                 )
             )
         )
 
     return model
 
 
-def gpt_3_5():
-    def model(input):
+def gpt_3_5() -> Callable[[str], Any]:
+    def model(input: str) -> Any:
         if config._api_keys is None:
             raise SeaplaneError(
-                f"OPENAI API Key `{OPENAI_API_KEY_NAME}` is not set, use `sea.config.set_api_keys`."
+                f"OPENAI API Key `{OPENAI_API_KEY_NAME}` is not set, use `sea.config.set_api_keys`."  # noqa
             )
         elif not config._api_keys.get(OPENAI_API_KEY_NAME, None):
             raise SeaplaneError(
-                f"OPENAI API Key `{OPENAI_API_KEY_NAME}` is not set, use `sea.config.set_api_keys`."
+                f"OPENAI API Key `{OPENAI_API_KEY_NAME}` is not set, use `sea.config.set_api_keys`."  # noqa
             )
 
         url = "https://api.openai.com/v1/chat/completions"
 
         payload = {
             "model": "gpt-3.5-turbo",
             "messages": [{"role": "user", "content": input}],
@@ -158,56 +160,60 @@
             )
         )
 
     return model
 
 
 class Coprocessor:
-    def __init__(self, func=None, type=None, model=None, id=None, args=None, kwargs=None):
+    def __init__(self, func: Callable[[Any], Any], type: str, id: str, model: Optional[str]) -> None:
         self.func = func
-        self.args = args
-        self.kwargs = kwargs
+        self.args: Optional[Tuple[Any, ...]] = None
+        self.kwargs: Optional[Dict[str, Any]] = None
         self.type = type
         self.model = model
         self.id = id
 
-    def set_func(self, func):
-        self.func = func
-
-    def process(self, *args, **kwargs):
+    def process(self, *args: Any, **kwargs: Any) -> Any:
         self.args = args
         self.kwargs = kwargs
 
         print(f"Coprocessor type '{self.type}' Model ID {self.model}")
+        
+        if self.type == "vectordb":
+            print("Accessing Vector DB coprocessor...")
+            self.args = self.args + (
+                Store(),
+            )
+            return self.func(*self.args, **self.kwargs)        
 
         if self.model == "bloom":
-            print(f"Processing Bloom Model...")
+            print("Processing Bloom Model...")
             self.args = self.args + (bloom(),)
 
             return self.func(*self.args, **self.kwargs)
         elif self.model == "gpt-3.5":
-            print(f"Procesing GPT-3.5 Model...")
+            print("Procesing GPT-3.5 Model...")
             self.args = self.args + (gpt_3_5(),)
 
             return self.func(*self.args, **self.kwargs)
         elif self.model == "gpt-3":
-            print(f"Procesing GPT-3 Model...")
+            print("Procesing GPT-3 Model...")
             self.args = self.args + (gpt_3(),)
 
             return self.func(*self.args, **self.kwargs)
         elif self.model == "stable-diffusion":
-            print(f"Accessing Replicate coprocessor...")
+            print("Accessing Replicate coprocessor...")
             self.args = self.args + (
                 inference("27b93a2413e7f36cd83da926f3656280b2931564ff050bf9575f1fdf9bcd7478"),
             )
 
             return self.func(*self.args, **self.kwargs)
         elif self.model:
-            print(f"Accessing Replicate coprocessor...")
+            print("Accessing Unknown coprocessor...")
             self.args = self.args + (inference(self.model),)
 
             return self.func(*self.args, **self.kwargs)
         else:
             return self.func(*self.args, **self.kwargs)
 
-    def print(self):
+    def print(self) -> None:
         print(f"id: {self.id}, type: {self.type}, model: {self.model}")
```

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/decorators.py` & `seaplane-0.3.4/src/seaplane/smartpipes/decorators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,166 @@
 import functools
 import json
 import traceback
+from typing import Any, Callable, Dict, List, Optional
 
 from ..logging import log
 from ..model.errors import HTTPError
 from .coprocessor import Coprocessor, CoprocessorEvent
 from .smartpipe import SmartPipe, SmartPipeEvent
 
 
-def format_exception(e):
+def format_exception(e: Optional[Exception]) -> Optional[List[str]]:
     if e is None:
         return None
 
     return traceback.format_exception(type(e), e, e.__traceback__)
 
 
-def event_json(event):
+def event_json(event: SmartPipeEvent) -> Dict[str, Any]:
     return {
         "id": event.id,
         "smart_pipe_id": event.smart_pipe_id,
         "input": event.input,
         "status": event.status,
         "output": event.output,
         "error": format_exception(event.error),
         "coprocessors": [
             coprocessor_event_json(coprocessor) for coprocessor in event.coprocessors
         ],
     }
 
 
-def coprocessor_event_json(event):
+def coprocessor_event_json(event: CoprocessorEvent) -> Dict[str, Any]:
     return {
         "id": event.id,
         "input": event.input,
         "status": event.status,
         "output": event.output,
         "error": format_exception(event.error),
     }
 
 
-def coprocessor_to_json(coprocessor):
+def coprocessor_to_json(coprocessor: Coprocessor) -> Dict[str, Any]:
     return {"id": coprocessor.id, "type": coprocessor.type, "model": coprocessor.model}
 
 
-def smart_pipe_to_json(smart_pipe):
+def smart_pipe_to_json(smart_pipe: SmartPipe) -> Dict[str, Any]:
     return {
         "id": smart_pipe.id,
         "path": smart_pipe.path,
         "method": smart_pipe.method,
         "coprocessors": [
             coprocessor_to_json(coprocessor) for coprocessor in smart_pipe.coprocessors
         ],
     }
 
 
-def smart_pipes_json(smart_pipes):
+def smart_pipes_json(smart_pipes: List[SmartPipe]) -> Dict[str, Any]:
     return {
         "type": "smart_pipes",
         "payload": [smart_pipe_to_json(smart_pipe) for smart_pipe in smart_pipes],
     }
 
 
 class Context:
-    def __init__(self, smart_pipes=[], coprocessors=[]):
-        self.smart_pipes = smart_pipes
-        self.coprocessors = coprocessors
+    def __init__(
+        self,
+        smart_pipes: Optional[List[SmartPipe]] = None,
+        coprocessors: Optional[List[Coprocessor]] = None,
+    ) -> None:
         self.actual_smart_pipe_index = -1
-        self.on_change = lambda x: None
-        self.events = []
-        self.active_event = ["none"]
+        self.on_change: Callable[[Dict[str, Any]], None] = lambda x: None
+        self.events: List[SmartPipeEvent] = []
+        self.active_event: List[str] = ["none"]
 
-    def active_smart_pipe(self, id):
+        if smart_pipes is None:
+            self.smart_pipes = []
+        else:
+            self.smart_pipes = smart_pipes
+
+        if coprocessors is None:
+            self.coprocessors = []
+        else:
+            self.coprocessors = coprocessors
+
+    def active_smart_pipe(self, id: str) -> None:
         for i, smart_pipe in enumerate(self.smart_pipes):
             if smart_pipe.id == id:
                 self.actual_smart_pipe_index = i
                 break
 
-    def set_event(self, event):
-        self.on_change = event
+    def set_event(self, callback: Callable[[Dict[str, Any]], None]) -> None:
+        self.on_change = callback
 
-    def add_event(self, event):
+    def add_event(self, event: SmartPipeEvent) -> None:
         self.active_event[0] = event.id
         self.events.append(event)
 
         self.on_change({"type": "add_request", "payload": event_json(event)})
 
-    def update_event(self, event):
+    def update_event(self, event: SmartPipeEvent) -> None:
         for i, e in enumerate(self.events):
             if e.id == self.active_event[0]:
                 self.events[i] = event
 
                 self.on_change({"type": "update_request", "payload": event_json(event)})
                 break
 
-    def coprocessor_event(self, coprocessor_event):
+    def coprocessor_event(self, coprocessor_event: CoprocessorEvent) -> None:
         for i, event in enumerate(self.events):
             if event.id == self.active_event[0]:
                 event.add_coprocessor_event(coprocessor_event)
 
                 self.events[i] = event
 
                 self.on_change({"type": "update_request", "payload": event_json(event)})
                 break
 
-    def get_actual_smart_pipe(self):
+    def get_actual_smart_pipe(self) -> Optional[SmartPipe]:
         if self.actual_smart_pipe_index == -1:
             return None
 
         return self.smart_pipes[self.actual_smart_pipe_index]
 
-    def add_smart_pipe(self, smart_pipe):
+    def add_smart_pipe(self, smart_pipe: SmartPipe) -> None:
         if len(self.smart_pipes) == 1 and self.smart_pipes[0].id == "temporal":
             self.smart_pipes[0] = smart_pipe
         else:
             self.actual_smart_pipe_index = len(self.smart_pipes)
             self.smart_pipes.append(smart_pipe)
 
         log.info(f"🧠 Smart Pipe: {smart_pipe.id}, Path: {smart_pipe.path}")
         self.on_change(smart_pipes_json(self.smart_pipes))
 
-    def add_coprocessor(self, coprocessor):
+    def add_coprocessor(self, coprocessor: Coprocessor) -> None:
         log.info(f"⌛️ Coprocessor {coprocessor.id} of type: {coprocessor.type}")
         self.coprocessors.append(coprocessor)
 
-    def set_coprocessor_function(self, id, func):
-        for smart_pipe in self.smart_pipes:
-            for coprocessor in smart_pipe.coprocessors:
-                if coprocessor.id == id:
-                    coprocessor.set_func(func)
-                    return coprocessor
-
-        return None
-
-    def assign_to_active_smart_pipe(self, coprocessor):
-
+    def assign_to_active_smart_pipe(self, coprocessor: Coprocessor) -> None:
         self.smart_pipes[self.actual_smart_pipe_index].add_coprocessor(coprocessor)
         smart_pipe = context.get_actual_smart_pipe()
-        log.info(f"⌛️ Assign Coprocessor {coprocessor.id} to Smart Pipe: {smart_pipe.id}")
+        if smart_pipe is not None:
+            log.info(f"⌛️ Assign Coprocessor {coprocessor.id} to Smart Pipe: {smart_pipe.id}")
+        else:
+            log.info(
+                f"🔥 Actual Smart Pipe is None, can't assign Coprocessor {coprocessor.id} to Smart Pipe"  # noqa
+            )
         self.on_change(smart_pipes_json(self.smart_pipes))
 
 
 context = Context()
 
 
 def smartpipe(
-    _func=None,
-    path=None,
-    method=None,
-    id=None,
-):
-    def decorator_smartpipes(func):
+    path: str, method: str, id: str, parameters: Optional[List[str]] = None, _func: Optional[Callable[[Any], Any]] = None
+) -> Callable[[Any, Any], Any]:
+    def decorator_smartpipes(func: Callable[[Any], Any]) -> Callable[[Any, Any], Any]:
         @functools.wraps(func)
-        def wrapper(*args, **kwargs):
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
             print(f"SmartPipe Path: {path}, Method: {method}, ID: {id}")
             context.active_smart_pipe(id)
 
             args_str = tuple(arg.decode() if isinstance(arg, bytes) else arg for arg in args)
             args_json = json.dumps(args_str)
 
             event = SmartPipeEvent(smart_pipe_id=id, input=args_json)
@@ -168,28 +173,30 @@
             except HTTPError as err:
                 log.error(f"Smart Pipe error: {err}")
                 event.set_error(err)
 
             context.update_event(event)
             return result
 
-        smart_pipe = SmartPipe(wrapper, path, method, id)
+        smart_pipe = SmartPipe(wrapper, path, method, id, parameters)
         context.add_smart_pipe(smart_pipe)
         return wrapper
 
     if not _func:
-        return decorator_smartpipes
+        return decorator_smartpipes  # type: ignore
     else:
         return decorator_smartpipes(_func)
 
 
-def import_coprocessor(_func=None, coprocessor=None):
-    def decorator_coprocessor(func):
+def import_coprocessor(
+    _func: Optional[Callable[[Any], Any]], coprocessor: Coprocessor
+) -> Callable[[Any, Any], Any]:
+    def decorator_coprocessor(func: Callable[[Any], Any]) -> Callable[[Any, Any], Any]:
         @functools.wraps(func)
-        def wrapper(*args, **kwargs):
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
             args_str = tuple(arg.decode() if isinstance(arg, bytes) else arg for arg in args)
             args_json = json.dumps(args_str)
 
             event = CoprocessorEvent(coprocessor.id, args_json)
             context.coprocessor_event(event)
 
             result = coprocessor.process(*args, **kwargs)
@@ -200,23 +207,29 @@
             return func(result)
 
         return wrapper
 
     context.add_coprocessor(coprocessor)
 
     if not _func:
-        return decorator_coprocessor
+        return decorator_coprocessor  # type: ignore
     else:
         return decorator_coprocessor(_func)
 
 
-def coprocessor(_func=None, type=None, model=None, id=None):
-    def decorator_coprocessor(func):
+def coprocessor(
+    type: str, id: str, model: Optional[str] = None, _func: Optional[Callable[[Any], Any]] = None,
+) -> Callable[[Any, Any], Any]:
+    def decorator_coprocessor(func: Callable[[Any], Any]) -> Callable[[Any, Any], Any]:
+
+        coprocessor = Coprocessor(func=func, type=type, model=model, id=id)
+        context.add_coprocessor(coprocessor)
+
         @functools.wraps(func)
-        def wrapper(*args, **kwargs):
+        def wrapper(*args: Any, **kwargs: Any) -> Any:
             context.assign_to_active_smart_pipe(coprocessor)
 
             args_str = tuple(arg.decode() if isinstance(arg, bytes) else arg for arg in args)
             args_json = json.dumps(args_str)
 
             event = CoprocessorEvent(coprocessor.id, args_json)
             context.coprocessor_event(event)
@@ -235,16 +248,13 @@
             context.coprocessor_event(event)
 
             if event.error is not None:
                 raise event.error
 
             return result
 
-        coprocessor = Coprocessor(func, type, model, id)
-        context.add_coprocessor(coprocessor)
-
         return wrapper
 
     if not _func:
-        return decorator_coprocessor
+        return decorator_coprocessor  # type: ignore
     else:
         return decorator_coprocessor(_func)
```

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/README.md` & `seaplane-0.3.4/src/seaplane/smartpipes/website/README.md`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/package.json` & `seaplane-0.3.4/src/seaplane/smartpipes/website/package.json`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/public/favicon.ico` & `seaplane-0.3.4/src/seaplane/smartpipes/website/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/public/next.svg` & `seaplane-0.3.4/src/seaplane/smartpipes/website/public/next.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/public/openai.png` & `seaplane-0.3.4/src/seaplane/smartpipes/website/public/openai.png`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/public/seaplane_logo.svg` & `seaplane-0.3.4/src/seaplane/smartpipes/website/public/seaplane_logo.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg` & `seaplane-0.3.4/src/seaplane/smartpipes/website/public/seaplane_logo_mark.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/public/stabilityai.png` & `seaplane-0.3.4/src/seaplane/smartpipes/website/public/stabilityai.png`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/public/vercel.svg` & `seaplane-0.3.4/src/seaplane/smartpipes/website/public/vercel.svg`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/src/components/Header.jsx` & `seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/Header.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx` & `seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/SmartPipe.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx` & `seaplane-0.3.4/src/seaplane/smartpipes/website/src/components/SmartPipesList.jsx`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/src/pages/index.js` & `seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/index.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/src/pages/tutorial.js` & `seaplane-0.3.4/src/seaplane/smartpipes/website/src/pages/tutorial.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/tailwind.config.js` & `seaplane-0.3.4/src/seaplane/smartpipes/website/tailwind.config.js`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/src/seaplane/smartpipes/website/yarn.lock` & `seaplane-0.3.4/src/seaplane/smartpipes/website/yarn.lock`

 * *Files identical despite different names*

### Comparing `seaplane-0.3.2/PKG-INFO` & `seaplane-0.3.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 Metadata-Version: 2.1
 Name: seaplane
-Version: 0.3.2
+Version: 0.3.4
 Summary: Seaplane Python SDK
 Home-page: https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 License: Apache License
 Author: Seaplane IO, Inc.
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: Flask-Cors (>=3.0.10,<4.0.0)
 Requires-Dist: Flask-SocketIO (>=5.3.4,<6.0.0)
 Requires-Dist: attrs (==21.4.0)
+Requires-Dist: boto3 (>=1.26.142,<2.0.0)
 Requires-Dist: certifi (==2022.6.15)
 Requires-Dist: charset-normalizer (==2.1.0)
 Requires-Dist: idna (==3.3)
 Requires-Dist: iniconfig (==1.1.1)
+Requires-Dist: langchain (>=0.0.183,<0.0.184)
+Requires-Dist: openai (>=0.27.7,<0.28.0)
 Requires-Dist: packaging (==21.3)
+Requires-Dist: pinecone-client (>=2.2.1,<3.0.0)
 Requires-Dist: pluggy (==1.0.0)
 Requires-Dist: py (==1.11.0)
 Requires-Dist: pyparsing (==3.0.9)
+Requires-Dist: pypdf (>=3.9.0,<4.0.0)
 Requires-Dist: requests (==2.28.1)
 Requires-Dist: requests-mock (>=1.9.3,<2.0.0)
 Requires-Dist: returns (>=0.19.0,<0.20.0)
 Requires-Dist: simplejson (>=3.17.6,<4.0.0)
+Requires-Dist: tiktoken (>=0.4.0,<0.5.0)
 Requires-Dist: tomli (==2.0.1)
+Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Requires-Dist: types-requests (>=2.28.0,<3.0.0)
 Requires-Dist: types-simplejson (>=3.17.7,<4.0.0)
 Requires-Dist: urllib3 (==1.26.9)
 Project-URL: Documentation, https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 Project-URL: Repository, https://github.com/seaplane-io/seaplane/tree/main/seaplane-sdk/python
 Description-Content-Type: text/markdown
```


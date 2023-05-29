# Comparing `tmp/rororo-3.1.0.tar.gz` & `tmp/rororo-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rororo-3.1.0.tar", max compression
+gzip compressed data, was "rororo-3.2.0.tar", max compression
```

## Comparing `rororo-3.1.0.tar` & `rororo-3.2.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1484 2022-12-26 20:50:03.968384 rororo-3.1.0/LICENSE
--rw-r--r--   0        0        0     4561 2022-12-26 20:50:03.968384 rororo-3.1.0/README.rst
--rw-r--r--   0        0        0     4706 2022-12-26 20:50:03.972384 rororo-3.1.0/pyproject.toml
--rw-r--r--   0        0        0      926 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/__init__.py
--rw-r--r--   0        0        0     4790 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/aio.py
--rw-r--r--   0        0        0      928 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/annotations.py
--rw-r--r--   0        0        0     4780 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/logger.py
--rw-r--r--   0        0        0     1424 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/__init__.py
--rw-r--r--   0        0        0     1050 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/annotations.py
--rw-r--r--   0        0        0      891 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/constants.py
--rw-r--r--   0        0        0     1080 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/contexts.py
--rw-r--r--   0        0        0     4276 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/core_data.py
--rw-r--r--   0        0        0    11538 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/core_validators.py
--rw-r--r--   0        0        0     2846 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/data.py
--rw-r--r--   0        0        0    14272 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/exceptions.py
--rw-r--r--   0        0        0     3721 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/middlewares.py
--rw-r--r--   0        0        0    26481 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/openapi.py
--rw-r--r--   0        0        0        0 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/py.typed
--rw-r--r--   0        0        0     5355 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/security.py
--rw-r--r--   0        0        0     3938 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/utils.py
--rw-r--r--   0        0        0     1505 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/validators.py
--rw-r--r--   0        0        0     1494 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/openapi/views.py
--rw-r--r--   0        0        0        0 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/py.typed
--rw-r--r--   0        0        0    12284 2022-12-26 20:50:03.972384 rororo-3.1.0/src/rororo/settings.py
--rw-r--r--   0        0        0    20469 2022-12-26 20:50:03.976384 rororo-3.1.0/src/rororo/timedelta.py
--rw-r--r--   0        0        0     1719 2022-12-26 20:50:03.976384 rororo-3.1.0/src/rororo/utils.py
--rw-r--r--   0        0        0     5842 1970-01-01 00:00:00.000000 rororo-3.1.0/setup.py
--rw-r--r--   0        0        0     6445 1970-01-01 00:00:00.000000 rororo-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1484 2023-05-29 20:33:02.685188 rororo-3.2.0/LICENSE
+-rw-r--r--   0        0        0     4561 2023-05-29 20:33:02.685188 rororo-3.2.0/README.rst
+-rw-r--r--   0        0        0     4907 2023-05-29 20:33:02.689188 rororo-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0      926 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/__init__.py
+-rw-r--r--   0        0        0     4790 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/aio.py
+-rw-r--r--   0        0        0      928 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/annotations.py
+-rw-r--r--   0        0        0     4780 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/logger.py
+-rw-r--r--   0        0        0     1424 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/__init__.py
+-rw-r--r--   0        0        0     1036 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/annotations.py
+-rw-r--r--   0        0        0      891 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/constants.py
+-rw-r--r--   0        0        0     1080 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/contexts.py
+-rw-r--r--   0        0        0     4276 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/core_data.py
+-rw-r--r--   0        0        0    11538 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/core_validators.py
+-rw-r--r--   0        0        0     2846 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/data.py
+-rw-r--r--   0        0        0    14272 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/exceptions.py
+-rw-r--r--   0        0        0     4828 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/middlewares.py
+-rw-r--r--   0        0        0    26588 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/openapi.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/py.typed
+-rw-r--r--   0        0        0     5355 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/security.py
+-rw-r--r--   0        0        0     3938 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/utils.py
+-rw-r--r--   0        0        0     1505 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/validators.py
+-rw-r--r--   0        0        0     1494 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/openapi/views.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/py.typed
+-rw-r--r--   0        0        0    12341 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/settings.py
+-rw-r--r--   0        0        0    20469 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/timedelta.py
+-rw-r--r--   0        0        0     1719 2023-05-29 20:33:02.689188 rororo-3.2.0/src/rororo/utils.py
+-rw-r--r--   0        0        0     6451 1970-01-01 00:00:00.000000 rororo-3.2.0/PKG-INFO
```

### Comparing `rororo-3.1.0/LICENSE` & `rororo-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/README.rst` & `rororo-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/pyproject.toml` & `rororo-3.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 lines_between_types = 0
 src_paths = [
   "",
   "examples/hobotnica/src/",
   "examples/petstore/src/",
   "examples/simulations/src/",
   "examples/todobackend/src/",
+  "examples/vc-api/src/",
   "src/",
 ]
 virtual_env = ".venv/"
 
 [tool.mypy]
 allow_untyped_globals = true
 check_untyped_defs = true
@@ -71,35 +72,34 @@
 show_error_codes = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unused_ignores = true
 
 [[tool.mypy.overrides]]
 module = [
-  "email_validator.*",
   "environ.*",
   "isodate.*",
   "jsonschema.*",
   "openapi_core.*",
   "openapi_schema_validator.*",
 ]
 ignore_missing_imports = true
 
 [tool.poetry]
 name = "rororo"
-version = "3.1.0"
+version = "3.2.0"
 description = "aiohttp.web OpenAPI 3 schema first server applications."
 authors = ["Igor Davydenko <iam@igordavydenko.com>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://igordavydenko.com/projects/#rororo"
 repository = "https://github.com/playpauseandstop/rororo"
 documentation = "https://rororo.readthedocs.io/"
 packages = [
-  {include = "rororo", from = "src/"},
+  {from = "src/", include = "rororo"},
 ]
 keywords = [
   "aiohttp",
   "aiohttp.web",
   "oas",
   "openapi",
   "openapi schema",
@@ -113,64 +113,67 @@
   "Intended Audience :: Developers",
   "License :: OSI Approved :: BSD License",
   "Operating System :: OS Independent",
   "Topic :: Internet :: WWW/HTTP",
   "Topic :: Internet :: WWW/HTTP :: WSGI",
   "Topic :: Internet :: WWW/HTTP :: WSGI :: Application",
   "Topic :: Utilities",
-  "Typing :: Typed"
+  "Typing :: Typed",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 aiohttp = "^3.8.1"
 aiohttp-middlewares = ">=1.2.0,<3"
-attrs = ">=19.2.0,<23"
-email-validator = "^1.0.5"
-environ-config = ">=20.1,<23"
+attrs = ">=19.2.0,<24"
+email-validator = ">=1.0.5,<3.0.0"
+environ-config = "^23.2.0"
 isodate = "^0.6.0"
 openapi-core = ">=0.13.4,<0.13.7"
 openapi-spec-validator = "0.4.0"
 pyrsistent = ">=0.16,<0.20"
 pyyaml = ">=5.1,<7.0"
 typing-extensions = {python = "<3.8", version = ">=3.7,<5"}
 
 [tool.poetry.group.dev.dependencies]
-mypy = "^0.991"
-types-pyyaml = "^6.0.12.2"
-types-redis = "^4.3.21.6"
+mypy = "^1.0.1"
+types-pyyaml = "^6.0.12.8"
+types-redis = "^4.5.1.3"
+
+[tool.poetry.group.docs.dependencies]
+furo = ">=2022.12.7,<2024.0.0"
+sphinx = "^5.3.0"
+sphinx-autobuild = "^2021.3.14"
+sphinx-autodoc-typehints = "^1.22"
+sphinx-copybutton = "^0.5.1"
+sphinxext-opengraph = "^0.7.5"
 
 [tool.poetry.group.test.dependencies]
 coverage = {extras = ["toml"], version = "^6.5.0"}
 coveralls = "^3.3.1"
-hiredis = "^2.0.0"
-pytest = "^7.2.0"
+hiredis = "^2.2.2"
+pytest = "^7.2.1"
 pytest-aiohttp = "^1.0.4"
-pytest-asyncio = "^0.20.2"
+pytest-asyncio = ">=0.20.3,<0.22.0"
 pytest-cov = "^4.0.0"
-redis = "^4.4.0"
-
-[tool.poetry.group.docs.dependencies]
-furo = "^2022.9.29"
-sphinx = "^5.3.0"
-sphinx-autobuild = "^2021.3.14"
-sphinx-autodoc-typehints = "^1.19.5"
-sphinx-copybutton = "^0.5.1"
-sphinxext-opengraph = "^0.7.3"
+redis = "^4.5.1"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/playpauseandstop/rororo/issues"
 
 [tool.pytest.ini_options]
 minversion = "7.2.0"
 testpaths = ["tests/"]
 addopts = "--cov --no-cov-on-fail"
 log_level = "info"
 # Local pytest options
 asyncio_mode = "auto"
+filterwarnings = [
+  "ignore:You supplied `schema_path` positional argument as well as supplying `schema` & `spec` keyword arguments. `schema_path` will be ignored in favor of `schema` & `spec` args.:UserWarning"
+]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist = py37,py38,py39,py310,py310-minimum-requirements,py311
 skipsdist = True
 
@@ -179,35 +182,34 @@
   3.7: py37
   3.8: py38
   3.9: py39
   3.10: py310
   3.11: py311
 
 [testenv]
+allowlist_externals = poetry
 passenv =
-  PYTHONPATH
+  LEVEL
   PYTEST_ADDOPTS
+  PYTHONPATH
   REDIS_URL
-  LEVEL
 setenv =
   USER=playpauseandstop
 skip_install = True
-whitelist_externals = poetry
 commands_pre =
   poetry install --only main,test
 commands =
-  poetry run python3 -m pytest
+  python3 -m pytest
 
 [testenv:py310-minimum-requirements]
 commands_pre =
   poetry install --only main,test
   poetry run python3 -m pip install \
     aiohttp==3.8.1 \
     aiohttp-middlewares==1.2.0 \
     attrs==19.2.0 \
     email-validator==1.0.5 \
-    environ-config==20.1.0 \
     jsonschema==3.2.0 \
     openapi-core==0.13.4 \
     pyrsistent==0.16 \
     PyYAML==5.1
 """
```

### Comparing `rororo-3.1.0/src/rororo/__init__.py` & `rororo-3.2.0/src/rororo/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,8 +39,8 @@
     "setup_openapi",
     "setup_settings",
     "setup_settings_from_environ",
 )
 
 __author__ = "Igor Davydenko"
 __license__ = "BSD-3-Clause"
-__version__ = "3.1.0"
+__version__ = "3.2.0"
```

### Comparing `rororo-3.1.0/src/rororo/aio.py` & `rororo-3.2.0/src/rororo/aio.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/annotations.py` & `rororo-3.2.0/src/rororo/annotations.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/logger.py` & `rororo-3.2.0/src/rororo/logger.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/__init__.py` & `rororo-3.2.0/src/rororo/openapi/__init__.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/annotations.py` & `rororo-3.2.0/src/rororo/openapi/annotations.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,9 +31,9 @@
     ignore_exceptions: Union[ExceptionType, Tuple[ExceptionType, ...], None]
 
 
 class ValidateEmailKwargsDict(TypedDict, total=False):
     allow_smtputf8: bool
     allow_empty_local: bool
     check_deliverability: bool
-    timeout: Union[int, float]
+    timeout: int
     dns_resolver: Any
```

### Comparing `rororo-3.1.0/src/rororo/openapi/constants.py` & `rororo-3.2.0/src/rororo/openapi/constants.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/contexts.py` & `rororo-3.2.0/src/rororo/openapi/contexts.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/core_data.py` & `rororo-3.2.0/src/rororo/openapi/core_data.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/core_validators.py` & `rororo-3.2.0/src/rororo/openapi/core_validators.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/data.py` & `rororo-3.2.0/src/rororo/openapi/data.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/exceptions.py` & `rororo-3.2.0/src/rororo/openapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/middlewares.py` & `rororo-3.2.0/src/rororo/openapi/middlewares.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from functools import partial
-from typing import Union
+from typing import Tuple, Type, Union
 
 from aiohttp import web
 from aiohttp_middlewares import error_middleware, get_error_response
 from aiohttp_middlewares.annotations import Middleware
 
 from rororo.annotations import Handler
 from rororo.openapi.annotations import ErrorMiddlewareKwargsDict
@@ -31,14 +31,36 @@
     OpenAPI schema.
     """
     if isinstance(handler, partial) and "handler" in handler.keywords:
         return get_actual_handler(handler.keywords["handler"])
     return handler
 
 
+def ensure_ignore_exceptions(
+    kwargs: ErrorMiddlewareKwargsDict, *ignore: Type[Exception]
+) -> None:
+    """Ensure all passed exceptions ignored by error middleware.
+
+    This is useful for ignoring handling redirection exceptions.
+    """
+    current = kwargs.get("ignore_exceptions")
+
+    to_ignore: Tuple[Type[Exception], ...]
+    if current is not None:
+        to_ignore = (
+            current + ignore
+            if isinstance(current, tuple)
+            else (current,) + ignore
+        )
+    else:
+        to_ignore = ignore
+
+    kwargs["ignore_exceptions"] = to_ignore
+
+
 def openapi_middleware(
     *,
     is_validate_response: bool = True,
     use_error_middleware: bool = True,
     error_middleware_kwargs: Union[ErrorMiddlewareKwargsDict, None] = None,
 ) -> Middleware:
     """Middleware to handle requests to handlers covered by OpenAPI schema.
@@ -46,14 +68,19 @@
     In most cases you don't need to add it to list of ``web.Application``
     middlewares as :func:`rororo.openapi.setup_openapi` will setup it for you,
     but if, for some reason, you don't want to call high order
     ``setup_openapi`` function, you'll need to add given middleware to your
     :class:`aiohttp.web.Applicaiton` manually.
     """
 
+    error_middleware_kwargs = error_middleware_kwargs or {}
+    # Do not handle ``HTTPRedirection`` errors by error middleware, as they
+    # will result in meaningless responses of ``{"detail": "Found"}``
+    ensure_ignore_exceptions(error_middleware_kwargs, web.HTTPRedirection)
+
     error_middleware_instance = (
         error_middleware(**error_middleware_kwargs or {})
         if use_error_middleware
         else None
     )
 
     async def get_response(
@@ -86,13 +113,18 @@
             # For performance considerations it is useful to turn off
             # validating responses at production environment as unfortunately
             # it will need to do extra checks after response is ready
             if is_validate_response:
                 validate_response(request, response)
 
             return response
+        except web.HTTPRedirection:
+            # Do not handle redirection errors, it is normal for
+            # ``web.Application`` to ask to redirect to other page via
+            # 301 <= X <= 399 error
+            raise
         except Exception as err:
             return await get_error_response(
                 request, err, **error_middleware_kwargs or {}
             )
 
     return middleware
```

### Comparing `rororo-3.1.0/src/rororo/openapi/openapi.py` & `rororo-3.2.0/src/rororo/openapi/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 import inspect
 import json
 import os
 import warnings
 from functools import lru_cache, partial
 from pathlib import Path
-from typing import Callable, cast, Deque, Dict, List, overload, Tuple, Union
+from typing import (
+    Callable,
+    cast,
+    Deque,
+    Dict,
+    List,
+    overload,
+    Tuple,
+    Type,
+    Union,
+)
 
 import attr
 import yaml
 from aiohttp import hdrs, web
 from aiohttp_middlewares import cors_middleware
 from openapi_core.schema.specs.models import Spec
 from openapi_core.shortcuts import create_spec
@@ -79,14 +89,15 @@
 
     .. code-block:: python
 
         from rororo import OperationTableDef
 
         operations = OperationTableDef()
 
+
         # Expect OpenAPI 3 schema to contain operationId: hello_world
         @operations.register
         async def hello_world(request: web.Request) -> web.Response:
             ...
 
 
         # Explicitly use `operationId: "helloWorld"`
@@ -356,16 +367,18 @@
                 continue
 
             operation.security = mapping[operation.operation_id]
 
     return spec
 
 
-def get_default_yaml_loader() -> SchemaLoader:
-    return cast(SchemaLoader, getattr(yaml, "CSafeLoader", yaml.SafeLoader))
+def get_default_yaml_loader() -> Type[yaml.BaseLoader]:
+    return cast(
+        Type[yaml.BaseLoader], getattr(yaml, "CSafeLoader", yaml.SafeLoader)
+    )
 
 
 def get_route_name(operation_id: str) -> str:
     return operation_id.replace(" ", "-")
 
 
 def get_route_prefix(mixed: Url) -> str:
@@ -700,15 +713,16 @@
                 "3 schema. To get full details about errors run "
                 f"`openapi-spec-validator {path.absolute()}`"
             )
     elif schema_path is not None:
         warnings.warn(
             "You supplied `schema_path` positional argument as well as "
             "supplying `schema` & `spec` keyword arguments. `schema_path` "
-            "will be ignored in favor of `schema` & `spec` args."
+            "will be ignored in favor of `schema` & `spec` args.",
+            stacklevel=2,
         )
 
     # Fix all operation securities within OpenAPI spec
     spec = fix_spec_operations(spec, cast(DictStrAny, schema))
 
     # Store schema, spec, and validate email kwargs in application dict
     app[APP_OPENAPI_SCHEMA_KEY] = schema
```

### Comparing `rororo-3.1.0/src/rororo/openapi/security.py` & `rororo-3.2.0/src/rororo/openapi/security.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/utils.py` & `rororo-3.2.0/src/rororo/openapi/utils.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/validators.py` & `rororo-3.2.0/src/rororo/openapi/validators.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/openapi/views.py` & `rororo-3.2.0/src/rororo/openapi/views.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/settings.py` & `rororo-3.2.0/src/rororo/settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,52 +20,59 @@
 import os
 import time
 import types
 from importlib import import_module
 from logging.config import dictConfig
 from typing import (
     Any,
-    cast,
     Collection,
     Iterator,
     MutableMapping,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 import environ
 from aiohttp import web
+from environ import to_config
 
-from rororo.annotations import DictStrAny, Level, MappingStrAny, Settings, T
+from rororo.annotations import (
+    DictStrAny,
+    DictStrStr,
+    Level,
+    MappingStrAny,
+    Settings,
+    T,
+)
 from rororo.logger import default_logging_dict
 from rororo.utils import ensure_collection, to_bool
 
 
 APP_SETTINGS_KEY = "settings"
 
 TBaseSettings = TypeVar("TBaseSettings", bound="BaseSettings")
 
 
-@environ.config(prefix=None, from_environ=None, frozen=True)
+@environ.config(prefix="", frozen=True)
 class BaseSettings:
     """Base Settings data structure for configuring ``aiohttp.web`` apps.
 
     Provides common attribs, which covers most of settings requires for
     run and configure ``aiohttp.web`` app. In same time it is designed to be
     inherited and completed with missed values in application as,
 
     .. code-block:: python
 
         import environ
         from rororo.settings import BaseSettings
 
 
-        @environ.config(prefix=None, frozen=True)
+        @environ.config(prefix="", frozen=True)
         class Settings(BaseSettings):
             other_name: str = environ.var(
                 name="OTHER_NAME", default="other-value"
             )
 
     """
 
@@ -90,27 +97,28 @@
     sentry_dsn: Union[str, None] = environ.var(name="SENTRY_DSN", default=None)
     sentry_release: Union[str, None] = environ.var(
         name="SENTRY_RELEASE", default=None
     )
 
     @classmethod
     def from_environ(
-        cls: Type[TBaseSettings], environment: "os._Environ[str]" = os.environ
+        cls: Type[TBaseSettings],
+        environ: Union[DictStrStr, "os._Environ[str]"] = os.environ,
     ) -> TBaseSettings:
         """Load the configuration as declared by *cls* from *environ*.
 
         This is a typed helper, which ensures that ``Settings.from_environ()``
         calls within typed context will not result in following mypy error::
 
             error: "Type[Settings]" has no attribute "from_environ"  [attr-defined]
 
         TODO: Move to ``Self`` type annotation as proposed in
         `PEP-673 <https://peps.python.org/pep-0673/#use-in-classmethod-signatures>`_
         """
-        return cast(TBaseSettings, environ.to_config(cls, environment))
+        return to_config(cls, environ)  # type: ignore[arg-type]
 
     def apply(
         self,
         *,
         loggers: Union[Collection[str], None] = None,
         remove_root_handlers: bool = False,
     ) -> None:
@@ -191,18 +199,18 @@
             def create_app(**options):
                 app = ...
                 app.settings = immutable_settings(settings, **options)
                 return app
 
         And yes each additional key overwrite default setting value.
     """
-    settings = {key: value for key, value in iter_settings(defaults)}
+    settings_dict = dict(iter_settings(defaults))
     for key, value in iter_settings(optionals):
-        settings[key] = value
-    return types.MappingProxyType(settings)
+        settings_dict[key] = value
+    return types.MappingProxyType(settings_dict)
 
 
 def inject_settings(
     mixed: Union[str, Settings],
     context: MutableMapping[str, Any],
     fail_silently: bool = False,
 ) -> None:
@@ -349,15 +357,15 @@
     return app
 
 
 def setup_settings_from_environ(
     app: web.Application,
     settings_class: Type[BaseSettings],
     *,
-    environ: Union["os._Environ[str]", None] = None,
+    environ: Union[DictStrStr, "os._Environ[str]", None] = None,
     loggers: Union[Collection[str], None] = None,
     remove_root_handlers: bool = False,
 ) -> web.Application:
     """
     Shortcut for instantiating settings from environ and applying them for
     given ``aiohttp.web`` app.
```

### Comparing `rororo-3.1.0/src/rororo/timedelta.py` & `rororo-3.2.0/src/rororo/timedelta.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/src/rororo/utils.py` & `rororo-3.2.0/src/rororo/utils.py`

 * *Files identical despite different names*

### Comparing `rororo-3.1.0/PKG-INFO` & `rororo-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rororo
-Version: 3.1.0
+Version: 3.2.0
 Summary: aiohttp.web OpenAPI 3 schema first server applications.
 Home-page: https://igordavydenko.com/projects/#rororo
 License: BSD-3-Clause
 Keywords: aiohttp,aiohttp.web,oas,openapi,openapi schema,openapi3,schema first
 Author: Igor Davydenko
 Author-email: iam@igordavydenko.com
 Requires-Python: >=3.7,<4.0
@@ -23,17 +23,17 @@
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI
 Classifier: Topic :: Internet :: WWW/HTTP :: WSGI :: Application
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: aiohttp-middlewares (>=1.2.0,<3)
-Requires-Dist: attrs (>=19.2.0,<23)
-Requires-Dist: email-validator (>=1.0.5,<2.0.0)
-Requires-Dist: environ-config (>=20.1,<23)
+Requires-Dist: attrs (>=19.2.0,<24)
+Requires-Dist: email-validator (>=1.0.5,<3.0.0)
+Requires-Dist: environ-config (>=23.2.0,<24.0.0)
 Requires-Dist: isodate (>=0.6.0,<0.7.0)
 Requires-Dist: openapi-core (>=0.13.4,<0.13.7)
 Requires-Dist: openapi-spec-validator (==0.4.0)
 Requires-Dist: pyrsistent (>=0.16,<0.20)
 Requires-Dist: pyyaml (>=5.1,<7.0)
 Requires-Dist: typing-extensions (>=3.7,<5) ; python_version < "3.8"
 Project-URL: Bug Tracker, https://github.com/playpauseandstop/rororo/issues
```


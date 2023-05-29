# Comparing `tmp/strawberry_django_plus-2.4.2.tar.gz` & `tmp/strawberry_django_plus-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_plus-2.4.2.tar", max compression
+gzip compressed data, was "strawberry_django_plus-2.5.0.tar", max compression
```

## Comparing `strawberry_django_plus-2.4.2.tar` & `strawberry_django_plus-2.5.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1077 2023-05-22 16:44:37.960302 strawberry_django_plus-2.4.2/LICENSE
--rw-r--r--   0        0        0     3299 2023-05-22 16:44:37.960302 strawberry_django_plus-2.4.2/README.md
--rw-r--r--   0        0        0     4290 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/pyproject.toml
--rw-r--r--   0        0        0     2950 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/__init__.py
--rw-r--r--   0        0        0     5562 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/descriptors.py
--rw-r--r--   0        0        0     5751 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/directives.py
--rw-r--r--   0        0        0    26052 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/field.py
--rw-r--r--   0        0        0     3069 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/filters.py
--rw-r--r--   0        0        0     1657 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/gql/__init__.py
--rw-r--r--   0        0        0     1389 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/gql/django.py
--rw-r--r--   0        0        0        0 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/integrations/__init__.py
--rw-r--r--   0        0        0     1939 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/integrations/guardian.py
--rw-r--r--   0        0        0        0 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/management/commands/__init__.py
--rw-r--r--   0        0        0     1168 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/management/commands/export_schema.py
--rw-r--r--   0        0        0        0 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/middlewares/__init__.py
--rw-r--r--   0        0        0     6304 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/middlewares/debug_toolbar.py
--rw-r--r--   0        0        0        0 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/mutations/__init__.py
--rw-r--r--   0        0        0    25062 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/mutations/fields.py
--rw-r--r--   0        0        0    14825 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/mutations/resolvers.py
--rw-r--r--   0        0        0    24443 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/optimizer.py
--rw-r--r--   0        0        0     1372 2023-05-22 16:44:37.964303 strawberry_django_plus-2.4.2/strawberry_django_plus/ordering.py
--rw-r--r--   0        0        0    27526 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/permissions.py
--rw-r--r--   0        0        0        0 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/py.typed
--rw-r--r--   0        0        0    47560 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/relay.py
--rw-r--r--   0        0        0     1107 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/settings.py
--rw-r--r--   0        0        0     1445 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
--rw-r--r--   0        0        0        0 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/test/__init__.py
--rw-r--r--   0        0        0     2337 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/test/client.py
--rw-r--r--   0        0        0    18301 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/type.py
--rw-r--r--   0        0        0    10174 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/types.py
--rw-r--r--   0        0        0        0 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/__init__.py
--rw-r--r--   0        0        0     6916 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/aio.py
--rw-r--r--   0        0        0    13069 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/inspect.py
--rw-r--r--   0        0        0     1077 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/pyutils.py
--rw-r--r--   0        0        0     5865 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/query.py
--rw-r--r--   0        0        0    13142 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/resolvers.py
--rw-r--r--   0        0        0      938 2023-05-22 16:44:37.968303 strawberry_django_plus-2.4.2/strawberry_django_plus/utils/typing.py
--rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1094 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/LICENSE
+-rw-r--r--   0        0        0     3299 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/README.md
+-rw-r--r--   0        0        0     4290 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3001 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/__init__.py
+-rw-r--r--   0        0        0     5562 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/descriptors.py
+-rw-r--r--   0        0        0     5751 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/directives.py
+-rw-r--r--   0        0        0    26052 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/field.py
+-rw-r--r--   0        0        0     3069 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/filters.py
+-rw-r--r--   0        0        0     1657 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/gql/__init__.py
+-rw-r--r--   0        0        0     1389 2023-05-29 19:12:42.096095 strawberry_django_plus-2.5.0/strawberry_django_plus/gql/django.py
+-rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/integrations/__init__.py
+-rw-r--r--   0        0        0     1939 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/integrations/guardian.py
+-rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/management/commands/__init__.py
+-rw-r--r--   0        0        0     1168 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/management/commands/export_schema.py
+-rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/middlewares/__init__.py
+-rw-r--r--   0        0        0     6304 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/middlewares/debug_toolbar.py
+-rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/mutations/__init__.py
+-rw-r--r--   0        0        0    25062 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/mutations/fields.py
+-rw-r--r--   0        0        0    14825 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/mutations/resolvers.py
+-rw-r--r--   0        0        0    26108 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/optimizer.py
+-rw-r--r--   0        0        0     1372 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/ordering.py
+-rw-r--r--   0        0        0    27526 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/permissions.py
+-rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/py.typed
+-rw-r--r--   0        0        0    47560 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/relay.py
+-rw-r--r--   0        0        0     1107 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/settings.py
+-rw-r--r--   0        0        0     1445 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html
+-rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/test/__init__.py
+-rw-r--r--   0        0        0     2337 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/test/client.py
+-rw-r--r--   0        0        0    18301 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/type.py
+-rw-r--r--   0        0        0    10174 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/types.py
+-rw-r--r--   0        0        0        0 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/__init__.py
+-rw-r--r--   0        0        0     6916 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/aio.py
+-rw-r--r--   0        0        0    13069 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/inspect.py
+-rw-r--r--   0        0        0     1077 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/pyutils.py
+-rw-r--r--   0        0        0     5865 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/query.py
+-rw-r--r--   0        0        0    13142 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/resolvers.py
+-rw-r--r--   0        0        0      938 2023-05-29 19:12:42.100095 strawberry_django_plus-2.5.0/strawberry_django_plus/utils/typing.py
+-rw-r--r--   0        0        0     4919 1970-01-01 00:00:00.000000 strawberry_django_plus-2.5.0/PKG-INFO
```

### Comparing `strawberry_django_plus-2.4.2/LICENSE` & `strawberry_django_plus-2.5.0/LICENSE`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2018 Tomás Fox
+Copyright (c) 2021-2023 Thiago Bellini Ribeiro
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `strawberry_django_plus-2.4.2/README.md` & `strawberry_django_plus-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/pyproject.toml` & `strawberry_django_plus-2.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strawberry-django-plus"
-version = "2.4.2"
+version = "2.5.0"
 description = "Enhanced Strawberry GraphQL integration with Django"
 authors = ["Thiago Bellini Ribeiro <thiago@bellini.dev>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/blb-ventures/strawberry-django-plus"
 repository = "https://github.com/blb-ventures/strawberry-django-plus"
 documentation = "https://strawberry-django-plus.readthedocs.io"
@@ -55,15 +55,15 @@
 django-guardian = "^2.4.0"
 mkdocs = "^1.4.2"
 mkdocs-markdownextradata-plugin = "^0.2.5"
 mkdocs-material = "^9.0.9"
 mkdocs-minify-plugin = "^0.6.2"
 pymdown-extensions = ">=9.5,<11.0"
 Markdown = "^3.3.7"
-ruff = "^0.0.269"
+ruff = "^0.0.270"
 
 
 [tool.poetry.extras]
 enum = ["django-choices-field"]
 debug-toolbar = ["django-debug-toolbar"]
 
 [tool.ruff]
```

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/__init__.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 _original_process_type = object_type._process_type
 _original_wrap_dataclass = object_type._wrap_dataclass
 _original_field_init = StrawberryField.__init__
 _original_field_call = StrawberryField.__call__
 _original_enum_init = EnumDefinition.__init__
 _original_from_generic = NameConverter.from_generic
 
+__version__ = "2.5.0"  # x-release-please-version
+
 
 def _get_doc(obj):
     if not obj.__doc__:
         return None
     return inspect.cleandoc(obj.__doc__)
```

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/descriptors.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/descriptors.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/directives.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/directives.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/field.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/filters.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/filters.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/gql/__init__.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/gql/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/gql/django.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/gql/django.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/integrations/guardian.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/integrations/guardian.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/management/commands/export_schema.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/management/commands/export_schema.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/middlewares/debug_toolbar.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/middlewares/debug_toolbar.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/mutations/fields.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/mutations/fields.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/mutations/resolvers.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/mutations/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/optimizer.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/optimizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import contextvars
 import dataclasses
 import itertools
+import typing
 from collections import defaultdict
 from typing import (
     Any,
     Callable,
     Dict,
+    ForwardRef,
     Generator,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
@@ -33,14 +35,15 @@
 from strawberry.lazy_type import LazyType
 from strawberry.schema.schema import Schema
 from strawberry.types.execution import ExecutionContext
 from strawberry.types.info import Info
 from strawberry.types.nodes import InlineFragment, Selection, convert_selections
 from strawberry.types.types import TypeDefinition
 from strawberry.utils.await_maybe import AwaitableOrValue
+from strawberry.utils.typing import eval_type
 from strawberry_django.fields.types import resolve_model_field_name
 from typing_extensions import TypeAlias, assert_never, assert_type
 
 from .descriptors import ModelProperty
 from .relay import Connection, Edge, NodeType
 from .utils import resolvers
 from .utils.inspect import (
@@ -67,14 +70,37 @@
 _interfaces: "defaultdict[Schema, Dict[TypeDefinition, List[TypeDefinition]]]" = defaultdict(dict)
 
 
 PrefetchCallable: TypeAlias = Callable[[GraphQLResolveInfo], Prefetch]
 PrefetchType: TypeAlias = Union[str, Prefetch, PrefetchCallable]
 
 
+def _get_prefetch_queryset(
+    remote_model: Type[models.Model],
+    field,
+    config: Optional["OptimizerConfig"],
+    info: GraphQLResolveInfo,
+) -> QuerySet:
+    """Returns a model's original QuerySet or a user's specified one.
+
+    If config.prefetch_custom_queryset is set True, the type's get_queryset() as well as
+    the model's custom manager/queryset are used to generate the prefetch query.
+    """
+    if not config or not config.prefetch_custom_queryset:
+        return remote_model._base_manager.all()  # type: ignore
+    remote_type_defs = typing.get_args(field.type_annotation.annotation)
+    if len(remote_type_defs) != 1:
+        raise TypeError(f"Expected exactly one remote type: {remote_type_defs}")
+    if type(remote_type_defs[0]) is ForwardRef:
+        remote_type = eval_type(remote_type_defs[0], field.type_annotation.namespace, None)
+    else:
+        remote_type = remote_type_defs[0]
+    return remote_type.get_queryset(remote_model.objects.all(), info)
+
+
 def _get_model_hints(
     model: Type[models.Model],
     schema: Schema,
     type_def: TypeDefinition,
     selection: Selection,
     *,
     info: GraphQLResolveInfo,
@@ -246,18 +272,20 @@
                             store.select_related = [
                                 o for o in store.select_related if o not in extra_sr
                             ]
                             f_store.select_related.extend(o[len(path_lookup) :] for o in extra_sr)
 
                         model_cache.setdefault(remote_model, []).append((level, f_store))
 
-                        # We need to use _base_manager here instead of _default_manager because we
-                        # are getting related objects, and not querying it directly
+                        # If prefetch_custom_queryset is false, use _base_manager here instead of
+                        # _default_manager because we are getting related objects, and not querying
+                        # it directly. Else use the type's get_queryset and model's custom QuerySet.
+                        base_qs = _get_prefetch_queryset(remote_model, field, config, info)
                         f_qs = f_store.apply(
-                            remote_model._base_manager.all(),  # type: ignore
+                            base_qs,
                             info=info,
                             config=config,
                         )
                         f_prefetch = Prefetch(path, queryset=f_qs)
                         f_prefetch._optimizer_sentinel = _sentinel  # type: ignore
                         store.prefetch_related.append(f_prefetch)
             else:
@@ -387,20 +415,23 @@
     Attributes:
         enable_only:
             Enable `QuerySet.only` optimizations
         enable_select_related:
             Enable `QuerySet.select_related` optimizations
         enable_prefetch_related:
             Enable `QuerySet.prefetch_related` optimizations
+        prefetch_custom_queryset:
+            Use custom instead of _base_manager for prefetch querysets
 
     """
 
     enable_only: bool = dataclasses.field(default=True)
     enable_select_related: bool = dataclasses.field(default=True)
     enable_prefetch_related: bool = dataclasses.field(default=True)
+    prefetch_custom_queryset: bool = dataclasses.field(default=False)
 
 
 @dataclasses.dataclass
 class OptimizerStore:
     """Django optimization store.
 
     Attributes:
@@ -586,19 +617,21 @@
     def __init__(
         self,
         *,
         enable_only_optimization: bool = True,
         enable_select_related_optimization: bool = True,
         enable_prefetch_related_optimization: bool = True,
         execution_context: Optional[ExecutionContext] = None,
+        prefetch_custom_queryset: bool = False,
     ):
         super().__init__(execution_context=execution_context)  # type: ignore
         self._enable_ony = enable_only_optimization
         self._enable_select_related = enable_select_related_optimization
         self._enable_prefetch_related = enable_prefetch_related_optimization
+        self._prefetch_custom_queryset = prefetch_custom_queryset
 
     def on_execute(self) -> Generator[None, None, None]:
         if enabled := self.enabled.get():
             optimizer.set(self)
 
         try:
             yield
@@ -624,14 +657,15 @@
             if ret._result_cache is None:  # type: ignore
                 config = OptimizerConfig(
                     enable_only=(
                         self._enable_ony and info.operation.operation == OperationType.QUERY
                     ),
                     enable_select_related=self._enable_select_related,
                     enable_prefetch_related=self._enable_prefetch_related,
+                    prefetch_custom_queryset=self._prefetch_custom_queryset,
                 )
                 return resolvers.resolve_qs(optimize(qs=ret, info=info, config=config))
 
         return ret
 
     def optimize(
         self,
@@ -643,9 +677,10 @@
         if not self.enabled.get():
             return qs
 
         config = OptimizerConfig(
             enable_only=self._enable_ony and info.operation.operation == OperationType.QUERY,
             enable_select_related=self._enable_select_related,
             enable_prefetch_related=self._enable_prefetch_related,
+            prefetch_custom_queryset=self._prefetch_custom_queryset,
         )
         return optimize(qs, info, config=config, store=store)
```

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/ordering.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/ordering.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/permissions.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/permissions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/relay.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/settings.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/settings.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html` & `strawberry_django_plus-2.5.0/strawberry_django_plus/templates/strawberry_django_plus/debug_toolbar.html`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/test/client.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/test/client.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/type.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/type.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/types.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/types.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/aio.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/aio.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/inspect.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/pyutils.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/pyutils.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/query.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/query.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/resolvers.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/resolvers.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/strawberry_django_plus/utils/typing.py` & `strawberry_django_plus-2.5.0/strawberry_django_plus/utils/typing.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_plus-2.4.2/PKG-INFO` & `strawberry_django_plus-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-plus
-Version: 2.4.2
+Version: 2.5.0
 Summary: Enhanced Strawberry GraphQL integration with Django
 Home-page: https://github.com/blb-ventures/strawberry-django-plus
 License: MIT
 Keywords: strawberry,django,graphql,relay,optimizer
 Author: Thiago Bellini Ribeiro
 Author-email: thiago@bellini.dev
 Requires-Python: >=3.8,<4.0
```


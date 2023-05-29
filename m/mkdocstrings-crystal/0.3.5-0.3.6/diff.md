# Comparing `tmp/mkdocstrings-crystal-0.3.5.tar.gz` & `tmp/mkdocstrings_crystal-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocstrings-crystal-0.3.5.tar", max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `mkdocstrings-crystal-0.3.5.tar` & `mkdocstrings_crystal-0.3.6.tar`

### file list

```diff
@@ -1,17 +1,24 @@
--rw-r--r--   0        0        0     1127 2021-05-14 15:33:17.572373 mkdocstrings-crystal-0.3.5/LICENSE.md
--rw-r--r--   0        0        0     2061 2022-04-26 22:23:27.515158 mkdocstrings-crystal-0.3.5/README.md
--rw-r--r--   0        0        0      784 2022-04-26 22:23:27.518491 mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/__init__.py
--rw-r--r--   0        0        0     8053 2022-04-26 22:23:27.518491 mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/collector.py
--rw-r--r--   0        0        0     3608 2022-04-26 22:23:27.518491 mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/crystal_html.py
--rw-r--r--   0        0        0     1024 2021-01-05 18:04:58.950630 mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/deduplicate_toc.py
--rw-r--r--   0        0        0     1022 2022-04-26 22:23:27.518491 mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/inventory.py
--rw-r--r--   0        0        0    18123 2022-05-02 22:17:36.827817 mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/items.py
--rw-r--r--   0        0        0      187 2022-04-26 22:23:27.518491 mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/macros.py
--rw-r--r--   0        0        0     5342 2022-05-02 22:43:46.024001 mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/renderer.py
--rw-r--r--   0        0        0      453 2022-05-02 22:36:29.652453 mkdocstrings-crystal-0.3.5/mkdocstrings/templates/crystal/material/constant.html
--rw-r--r--   0        0        0      704 2022-05-02 22:36:10.596166 mkdocstrings-crystal-0.3.5/mkdocstrings/templates/crystal/material/method.html
--rw-r--r--   0        0        0     3525 2022-05-02 22:51:48.521635 mkdocstrings-crystal-0.3.5/mkdocstrings/templates/crystal/material/style.css
--rw-r--r--   0        0        0     2727 2022-05-02 22:36:43.102186 mkdocstrings-crystal-0.3.5/mkdocstrings/templates/crystal/material/type.html
--rw-r--r--   0        0        0     1543 2022-05-02 23:00:58.228167 mkdocstrings-crystal-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     3213 2022-05-02 23:00:59.841569 mkdocstrings-crystal-0.3.5/setup.py
--rw-r--r--   0        0        0     3013 2022-05-02 23:00:59.841842 mkdocstrings-crystal-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/__init__.py
+-rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/collector.py
+-rw-r--r--   0        0        0     3633 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/crystal_html.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/deduplicate_toc.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/inventory.py
+-rw-r--r--   0        0        0    18493 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/items.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/macros.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/py.typed
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/renderer.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/templates/material/constant.html
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/templates/material/method.html
+-rw-r--r--   0        0        0     3525 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/templates/material/style.css
+-rw-r--r--   0        0        0     2731 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/templates/material/type.html
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/tests/test_crystal_html.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/tests/test_deduplicate_toc.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/tests/crystal_html/arg_only.yml
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/tests/crystal_html/basic.yml
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/tests/crystal_html/basic_2.yml
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/tests/deduplicate_toc/basic.yml
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/LICENSE.md
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/README.md
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     3650 2020-02-02 00:00:00.000000 mkdocstrings_crystal-0.3.6/PKG-INFO
```

### Comparing `mkdocstrings-crystal-0.3.5/LICENSE.md` & `mkdocstrings_crystal-0.3.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mkdocstrings-crystal-0.3.5/README.md` & `mkdocstrings_crystal-0.3.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # mkdocstrings-crystal
 
 **[Crystal][] language doc generator for [MkDocs][], via [mkdocstrings][]**
 
 [![PyPI](https://img.shields.io/pypi/v/mkdocstrings-crystal)](https://pypi.org/project/mkdocstrings-crystal/)
 [![GitHub](https://img.shields.io/github/license/oprypin/mkdocstrings-crystal)](https://github.com/mkdocstrings/crystal/blob/master/LICENSE.md)
-[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/oprypin/mkdocstrings-crystal/CI)](https://github.com/mkdocstrings/crystal/actions?query=event%3Apush+branch%3Amaster)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/oprypin/mkdocstrings-crystal/ci.yml.svg)](https://github.com/mkdocstrings/crystal/actions?query=event%3Apush+branch%3Amaster)
 
 ## Introduction
 
 *mkdocstrings-crystal* allows you to insert API documentation (generated from [Crystal][]'s source code and doc comments) as part of any page on a [MkDocs][] site.
 
 [See it in action][showcase].
```

### Comparing `mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/__init__.py` & `mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,31 @@
-from typing import Any, Mapping, Optional, Sequence
+from __future__ import annotations
+
+from typing import Any, Mapping, Sequence
 
 from mkdocstrings.handlers.base import BaseHandler
 
 from . import inventory
 from .collector import CrystalCollector
 from .renderer import CrystalRenderer
 
+__version__ = "0.3.6"
+
+
+class CrystalHandler(CrystalCollector, CrystalRenderer, BaseHandler):
+    load_inventory = staticmethod(inventory.list_object_urls)  # type: ignore[assignment]
 
-class CrystalHandler(BaseHandler):
-    load_inventory = staticmethod(inventory.list_object_urls)
+    def __init__(
+        self,
+        theme: str,
+        custom_templates: str | None = None,
+        crystal_docs_flags: Sequence[str] = (),
+        source_locations: Mapping[str, str] = {},
+        **config: Any,
+    ) -> None:
+        BaseHandler.__init__(self, "crystal", theme, custom_templates)  # type: ignore
+        CrystalCollector.__init__(
+            self, crystal_docs_flags=crystal_docs_flags, source_locations=source_locations
+        )
 
 
-def get_handler(
-    theme: str,
-    custom_templates: Optional[str] = None,
-    crystal_docs_flags: Sequence[str] = (),
-    source_locations: Mapping[str, str] = {},
-    **config: Any
-) -> CrystalHandler:
-    collector = CrystalCollector(
-        crystal_docs_flags=crystal_docs_flags, source_locations=source_locations
-    )
-    renderer = CrystalRenderer("crystal", theme, custom_templates)
-    renderer.collector = collector
-    return CrystalHandler(collector, renderer)
+get_handler = CrystalHandler
```

### Comparing `mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/collector.py` & `mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,49 @@
+from __future__ import annotations
+
 import collections
 import dataclasses
 import functools
 import logging
 import os
 import re
 import shlex
 import subprocess
-from typing import Any, Callable, Iterable, Iterator, List, Mapping, Sequence, TypeVar, Union, cast
+import sys
+from typing import Any, BinaryIO, Callable, Iterable, Iterator, Mapping, Sequence, TypeVar, cast
+
+if sys.version_info >= (3, 8):
+    from functools import cached_property
+else:
+    from cached_property import cached_property
 
-import mkdocs.exceptions
-import mkdocs.utils
-from cached_property import cached_property
-from mkdocstrings.handlers.base import BaseCollector, CollectionError
+from mkdocstrings.handlers.base import BaseHandler, CollectionError
 
 from . import inventory
 from .items import DocConstant, DocItem, DocLocation, DocMapping, DocMethod, DocModule, DocType
 
 try:
     from mkdocs.exceptions import PluginError
 except ImportError:
-    PluginError = SystemExit
+    PluginError = SystemExit  # type: ignore
 
 log = logging.getLogger(f"mkdocs.plugins.{__name__}")
-log.addFilter(mkdocs.utils.warning_filter)
 
 D = TypeVar("D", bound=DocItem)
 
 
-class CrystalCollector(BaseCollector):
+class CrystalCollector(BaseHandler):
     def __init__(
         self, crystal_docs_flags: Sequence[str] = (), source_locations: Mapping[str, str] = {}
     ):
         """Create a "collector", reading docs from `crystal doc` in the current directory.
 
         Normally this should not be instantiated.
 
-        When using mkdocstrings-crystal within MkDocs, a plugin can access the instance as `config['plugins']['mkdocstrings'].get_handler('crystal').collector`.
+        When using mkdocstrings-crystal within MkDocs, a plugin can access the instance as `config.plugins['mkdocstrings'].get_handler('crystal')`.
 
         See [Extras](extras.md).
         """
         command = [
             "crystal",
             "docs",
             "--format=json",
@@ -60,42 +64,43 @@
                 for k in source_locations
             ),
             key=lambda d: -d.src_path.count("/"),
         )
 
     # pytype: disable=bad-return-type
     @cached_property
-    def root(self) -> "DocRoot":
+    def root(self) -> DocRoot:
         """The top-level namespace, represented as a fake module."""
         try:
             with self._proc:
-                root = inventory.read(self._proc.stdout)
-            root.__class__ = DocRoot
+                module = inventory.read(cast(BinaryIO, self._proc.stdout))
+            module.__class__ = DocRoot
+            root = cast(DocRoot, module)
             root.source_locations = self._source_locations
             return root
         finally:
             if self._proc.returncode:
-                cmd = " ".join(shlex.quote(arg) for arg in self._proc.args)
+                cmd = " ".join(shlex.quote(arg) for arg in cast(Sequence[str], self._proc.args))
                 raise PluginError(f"Command `{cmd}` exited with status {self._proc.returncode}")
 
     # pytype: enable=bad-return-type
 
-    def collect(self, identifier: str, config: Mapping[str, Any]) -> "DocView":
-        """[Find][mkdocstrings.handlers.crystal.items.DocItem.lookup] an item by its identifier.
+    def collect(self, identifier: str, config: Mapping[str, Any]) -> DocView:
+        """[Find][mkdocstrings_handlers.crystal.items.DocItem.lookup] an item by its identifier.
 
         Raises:
             CollectionError: When an item by that identifier couldn't be found.
         """
         config = {
             "nested_types": False,
             "file_filters": True,
             **config,
         }
 
-        item = self.root
+        item: DocItem = self.root
         if identifier != "::":
             item = item.lookup(identifier)
         return DocView(item, config)
 
 
 @dataclasses.dataclass
 class _SourceDestination:
@@ -163,15 +168,15 @@
             raise KeyError(f"Missing key: {e}")
 
 
 _crystal_info = _DictAccess(_CrystalInfo())
 
 
 class DocRoot(DocModule):
-    source_locations: List[_SourceDestination]
+    source_locations: list[_SourceDestination]
 
     def update_url(self, location: DocLocation) -> DocLocation:
         for dest in self.source_locations:
             if (location.filename or "").startswith(dest.src_path):
                 location.url = dest.substitute(location)
                 break
         return location
@@ -179,46 +184,52 @@
 
 class DocView:
     def __init__(self, item: DocItem, config: Mapping[str, Any]):
         self.item = item
         self.config = config
 
     def __getattr__(self, name: str):
-        val = getattr(self.item, name)
-        if isinstance(val, DocMapping) and val:
-            if name == "types" and not self.config["nested_types"]:
-                return DocMapping(())
-            return type(self)._filter(self.config["file_filters"], val, type(self)._get_locations)
-        return val
+        try:
+            val = getattr(self.item, name)
+            if isinstance(val, DocMapping) and val:
+                if name == "types" and not self.config["nested_types"]:
+                    return DocMapping(())
+                return type(self)._filter(
+                    self.config["file_filters"], val, type(self)._get_locations
+                )
+            return val
+        except AttributeError as e:
+            raise RuntimeError(e) from e
 
     def walk_types(self) -> Iterator[DocType]:
         types = cast(DocMapping[DocType], self.types)
         for typ in types:
             yield typ
             yield from typ.walk_types()
 
     @classmethod
     def _get_locations(cls, obj: DocItem) -> Sequence[str]:
         if isinstance(obj, DocConstant):
-            obj = obj.parent
-            if not obj:
+            parent = obj.parent
+            if not parent:
                 return ()
+            obj = parent
         if isinstance(obj, DocType):
-            return [loc.url.rsplit("#", 1)[0] for loc in obj.locations]
+            return [loc.filename for loc in obj.locations]
         elif isinstance(obj, DocMethod):
             if not obj.location:
                 return ()
-            return (obj.location.url.rsplit("#", 1)[0],)
+            return (obj.location.filename,)
         else:
             raise TypeError(obj)
 
     @classmethod
     def _filter(
         cls,
-        filters: Union[bool, Sequence[str]],
+        filters: bool | Sequence[str],
         mapp: DocMapping[D],
         getter: Callable[[D], Sequence[str]],
     ) -> DocMapping[D]:
         if filters is False:
             return DocMapping(())
         if filters is True:
             return mapp
```

### Comparing `mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/crystal_html.py` & `mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/crystal_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from __future__ import annotations
+
 import collections
 import html.parser
 import io
-from typing import Callable, Iterable, List, Optional, Sequence, Tuple
+from typing import Callable, Iterable, Sequence, Tuple
 
 from markupsafe import Markup, escape
 
 LinkToken = Tuple[int, int, str]
 
 
 class TextWithLinks(collections.UserString):
@@ -38,19 +40,19 @@
 ) -> str:
     pygments_parser = _PygmentsHTMLHandler(html_tokens, make_link)
     pygments_parser.feed(pygments_html)
     return Markup(pygments_parser.html.getvalue())
 
 
 class _CrystalHTMLHandler(html.parser.HTMLParser):
-    def __init__(self):
+    def __init__(self) -> None:
         super().__init__()
         self.text = io.StringIO()
-        self.tokens: List[LinkToken] = []
-        self._link_starts: List[Tuple[int, str]] = []
+        self.tokens: list[LinkToken] = []
+        self._link_starts: list[tuple[int, str]] = []
 
     def handle_starttag(self, tag, attrs):
         if tag == "a":
             href = next(v for k, v in attrs if k == "href")
             self._link_starts.append((self.text.tell(), self.link_to_path(href)))
 
     def handle_endtag(self, tag):
@@ -75,15 +77,15 @@
         super().__init__()
         self.tokens = iter(tokens)
         self.make_link = make_link
 
         self.token = next(self.tokens, None)
         self.pos = 0
         self.html = io.StringIO()
-        self.inlink: Optional[int] = None
+        self.inlink: int | None = None
 
     def handle_starttag(self, tag, attrs):
         if tag == "span" and self.inlink is None:
             if self.token and self.token[0] <= self.pos:
                 self.inlink = self.html.tell()
 
         if self.inlink is None:
```

### Comparing `mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/deduplicate_toc.py` & `mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/deduplicate_toc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,32 @@
+from __future__ import annotations
+
 import xml.etree.ElementTree as etree
-from typing import List
 
-from markdown import Markdown  # type: ignore
-from markdown.extensions import Extension, fenced_code  # type: ignore
+from markdown import Markdown
+from markdown.extensions import Extension
 from markdown.treeprocessors import Treeprocessor
 
 
-def _deduplicate_toc(toc: List[dict]) -> None:
+def _deduplicate_toc(toc: list[dict]) -> None:
     i = 0
     while i < len(toc):
         el = toc[i]
         if el.get("children"):
             _deduplicate_toc(el["children"])
         elif i > 0 and el["name"] == toc[i - 1]["name"]:
             del toc[i]
             continue
         i += 1
 
 
 class _TocDeduplicatingTreeprocessor(Treeprocessor):
     def run(self, root: etree.Element):
         try:
-            toc = self.md.toc_tokens
+            toc = self.md.toc_tokens  # type: ignore
         except AttributeError:
             return
         _deduplicate_toc(toc)
 
 
 class DeduplicateTocExtension(Extension):
     def extendMarkdown(self, md: Markdown) -> None:
```

### Comparing `mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/items.py` & `mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/items.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from __future__ import annotations
 
 import abc
 import collections
 import dataclasses
 import re
-from typing import Any, Generic, Iterator, Mapping, Optional, Sequence, TypeVar, Union
+import sys
+from typing import TYPE_CHECKING, Any, Generic, Iterator, Mapping, Sequence, TypeVar, overload
 
-try:
+if sys.version_info >= (3, 8):
     from functools import cached_property
-except ImportError:
+else:
     from cached_property import cached_property
 
 from mkdocstrings.handlers.base import CollectionError
 
 from . import crystal_html
 
+if TYPE_CHECKING:
+    from .collector import DocRoot
+
 
 class DocItem(metaclass=abc.ABCMeta):
     """A representation of a documentable item from Crystal language."""
 
     _TEMPLATE: str
-    parent: Optional["DocItem"] = None
+    parent: DocItem | None = None
     """The item that is the parent namespace for this item."""
-    root: "DocType" = None
+    root: DocRoot
 
-    def __init__(self, data: Mapping[str, Any], parent: Optional[DocItem], root: Optional[DocType]):
+    def __init__(self, data: Mapping[str, Any], parent: DocItem | None, root: DocRoot | None):
         self.data = data
         self.parent = parent
         self.root = root or self  # type: ignore
 
     @property
     def name(self) -> str:
         """The name of this item, e.g. `Foo` or `baz`."""
@@ -43,15 +47,15 @@
     def abs_id(self) -> str:
         """The absolute identifier of this item, sometimes known as "path", e.g. `Foo::Bar` or `Foo::Bar#baz(x,y)`.
 
         This is also the canonical identifier that will be used as its HTML id."""
         return self.data["id"]
 
     @property
-    def doc(self) -> Optional[str]:
+    def doc(self) -> str | None:
         """The doc comment of this item."""
         return self.data.get("doc")
 
     @classmethod
     def _properties(cls):
         for attr in dir(cls):
             if attr.startswith("_") or attr in ("doc", "abs_id", "name", "kind"):
@@ -71,27 +75,27 @@
 
     def __repr__(self) -> str:
         items = ", ".join(
             f"{attr}={getattr(self, attr)!r}" for attr in self._properties() if getattr(self, attr)
         )
         return f"{type(self).__name__}({items})"
 
-    def lookup(self, identifier: Union[str, DocPath]) -> DocItem:
+    def lookup(self, identifier: str | DocPath) -> DocItem:
         """Find an item by its identifier, relative to this item or the root.
 
         Params:
             identifier: The item to search for.
         Returns:
             An object that's a subclass of DocItem.
         Raises:
             CollectionError: When an item by that identifier couldn't be found.
         """
         if isinstance(identifier, DocPath):
             identifier = "::" + identifier.abs_id
-        obj = self.root if identifier.startswith("::") else self
+        obj: DocItem | None = self.root if identifier.startswith("::") else self
         ret_obj = obj
         path = re.split(r"(::|#|\.|:|^)", identifier)
         for sep, name in zip(path[1::2], path[2::2]):
             if isinstance(obj, DocType):
                 try:
                     order = _LOOKUP_ORDER[sep]
                 except KeyError:
@@ -106,14 +110,15 @@
                 raise CollectionError(f"{identifier!r} - can't find {name!r}")
             ret_obj = obj
             if isinstance(obj, DocAlias):
                 try:
                     obj = self.lookup(str(obj.aliased))
                 except CollectionError:
                     pass
+        assert ret_obj is not None
         return ret_obj
 
 
 _LOOKUP_ORDER = {
     "": ["types", "constants", "instance_methods", "class_methods", "constructors", "macros"],
     "::": ["types", "constants"],
     "#": ["instance_methods", "class_methods", "constructors", "macros"],
@@ -122,30 +127,31 @@
 }
 
 
 D = TypeVar("D", bound=DocItem)
 
 
 class DocType(DocItem):
-    """A [DocItem][mkdocstrings.handlers.crystal.items.DocItem] representing a Crystal type."""
+    """A [DocItem][mkdocstrings_handlers.crystal.items.DocItem] representing a Crystal type."""
 
     _TEMPLATE = "type.html"
 
-    def __new__(cls, data: Optional[Mapping[str, Any]] = None, *args, **kwargs) -> DocType:
+    @overload
+    def __new__(cls: type[DocType], data: Mapping[str, Any], *args, **kwargs) -> DocType:
+        ...
+
+    @overload
+    def __new__(cls, data: Mapping[str, Any] | None = None, *args, **kwargs) -> DocType:
+        ...
+
+    def __new__(cls, data=None, *args, **kwargs) -> DocType:
         """Based on Crystal's JSON, create an object of an appropriate subclass of DocType"""
         if cls is DocType:
             try:
-                cls = {
-                    "module": DocModule,
-                    "class": DocClass,
-                    "struct": DocStruct,
-                    "enum": DocEnum,
-                    "alias": DocAlias,
-                    "annotation": DocAnnotation,
-                }[data["kind"]]
+                cls = _doc_type_mapping[data["kind"]]
             except KeyError:
                 raise TypeError(
                     "DocType is abstract, and {kind!r} is not recognized".format_map(data)
                 )
         return super().__new__(cls)
 
     @property
@@ -200,18 +206,19 @@
 
     @cached_property
     def types(self) -> DocMapping[DocType]:
         """The types nested in this type as a namespace."""
         return DocMapping([DocType(x, self, self.root) for x in self.data.get("types", ())])
 
     @cached_property
-    def superclass(self) -> Optional[DocPath]:
+    def superclass(self) -> DocPath | None:
         """The possible superclass of this type."""
         if self.data.get("superclass") is not None:
             return DocPath(self.data["superclass"], self)
+        return None
 
     @cached_property
     def ancestors(self) -> Sequence[DocPath]:
         """The modules and classes this type inherited."""
         return [DocPath(x, self) for x in self.data.get("ancestors", ())]
 
     @cached_property
@@ -232,67 +239,67 @@
     @cached_property
     def including_types(self) -> Sequence[DocPath]:
         """Known types that include this type."""
         return [DocPath(x, self) for x in self.data.get("including_types", ())]
 
     @cached_property
     def locations(self) -> Sequence[DocLocation]:
-        """The [code locations][mkdocstrings.handlers.crystal.items.DocLocation] over which the definitions of this type span."""
+        """The [code locations][mkdocstrings_handlers.crystal.items.DocLocation] over which the definitions of this type span."""
         return [
-            self.root.update_url(DocLocation(loc["filename"], loc["line_number"], loc["url"]))
+            self.root.update_url(DocLocation(loc["filename"], int(loc["line_number"]), loc["url"]))
             for loc in self.data["locations"]
         ]
 
     def walk_types(self) -> Iterator[DocType]:
         """Recusively iterate over all types under this type (excl. itself) in lexicographic order."""
         for typ in self.types:
             yield typ
             yield from typ.walk_types()
 
 
 class DocModule(DocType):
-    """A [DocType][mkdocstrings.handlers.crystal.items.DocType] representing a Crystal module."""
+    """A [DocType][mkdocstrings_handlers.crystal.items.DocType] representing a Crystal module."""
 
 
 class DocClass(DocType):
-    """A [DocType][mkdocstrings.handlers.crystal.items.DocType] representing a Crystal class."""
+    """A [DocType][mkdocstrings_handlers.crystal.items.DocType] representing a Crystal class."""
 
 
 class DocStruct(DocType):
-    """A [DocType][mkdocstrings.handlers.crystal.items.DocType] representing a Crystal struct."""
+    """A [DocType][mkdocstrings_handlers.crystal.items.DocType] representing a Crystal struct."""
 
 
 class DocEnum(DocType):
-    """A [DocType][mkdocstrings.handlers.crystal.items.DocType] representing a Crystal enum."""
+    """A [DocType][mkdocstrings_handlers.crystal.items.DocType] representing a Crystal enum."""
 
 
 class DocAlias(DocType):
-    """A [DocType][mkdocstrings.handlers.crystal.items.DocType] representing a Crystal alias."""
+    """A [DocType][mkdocstrings_handlers.crystal.items.DocType] representing a Crystal alias."""
 
     @cached_property
     def aliased(self) -> crystal_html.TextWithLinks:
-        """[A rich string][mkdocstrings.handlers.crystal.crystal_html.TextWithLinks] containing the definition of what this is aliased to."""
+        """[A rich string][mkdocstrings_handlers.crystal.crystal_html.TextWithLinks] containing the definition of what this is aliased to."""
         # https://github.com/crystal-lang/crystal/pull/10117
         try:
             return crystal_html.parse_crystal_html(self.data["aliased_html"])
         except KeyError:
             return crystal_html.TextWithLinks(self.data["aliased"], ())
 
     @property
     def constants(self):
         # Crystal duplicates constants into aliases, but that's undesirable.
         return DocMapping(())
 
 
 class DocAnnotation(DocType):
-    """A [DocType][mkdocstrings.handlers.crystal.items.DocType] representing a Crystal annotation."""
+    """A [DocType][mkdocstrings_handlers.crystal.items.DocType] representing a Crystal annotation."""
 
 
 class DocConstant(DocItem):
-    """A [DocItem][mkdocstrings.handlers.crystal.items.DocItem] representing a Crystal constant definition."""
+    """A [DocItem][mkdocstrings_handlers.crystal.items.DocItem] representing a Crystal constant definition."""
 
     _TEMPLATE = "constant.html"
 
     @property
     def abs_id(self) -> str:
         return (
             self.parent.abs_id + "::" if self.parent and self.parent.parent else ""
@@ -305,15 +312,15 @@
     @property
     def value(self) -> str:
         """The value of the constant (the code as a string)."""
         return self.data["value"]
 
 
 class DocMethod(DocItem):
-    """A [DocItem][mkdocstrings.handlers.crystal.items.DocItem] representing a Crystal method."""
+    """A [DocItem][mkdocstrings_handlers.crystal.items.DocItem] representing a Crystal method."""
 
     _TEMPLATE = "method.html"
     METHOD_SEP: str = ""
     METHOD_ID_SEP: str
 
     @property
     def rel_id(self):
@@ -333,93 +340,94 @@
     def abs_id(self):
         return (
             self.parent.abs_id + self.METHOD_ID_SEP if self.parent and self.parent.parent else ""
         ) + self.rel_id
 
     @property
     def short_name(self):
-        """Similar to [rel_id][mkdocstrings.handlers.crystal.items.DocItem.rel_id], but also includes the separator first, e.g. `#bar(x,y)` or `.baz()`"""
+        """Similar to [rel_id][mkdocstrings_handlers.crystal.items.DocItem.rel_id], but also includes the separator first, e.g. `#bar(x,y)` or `.baz()`"""
         return (self.METHOD_SEP if self.parent and self.parent.parent else "") + self.name
 
     @property
     def is_abstract(self) -> bool:
         """Whether this method is abstract."""
         return bool(self.data.get("abstract"))
 
     @cached_property
     def args_string(self) -> str:
-        """[A rich string][mkdocstrings.handlers.crystal.crystal_html.TextWithLinks] with the method's parameters.
+        """[A rich string][mkdocstrings_handlers.crystal.crystal_html.TextWithLinks] with the method's parameters.
 
         e.g. `(foo : Bar) : Baz`
         """
         # https://github.com/crystal-lang/crystal/pull/10109
         try:
             html = self.data["args_html"]
         except KeyError:
             html = self.data.get("args_string")
             if html is None:
                 # https://github.com/crystal-lang/crystal/issues/12043
                 ret = self.data["def"].get("return_type", "")
                 return ret and " : " + ret
-        return crystal_html.parse_crystal_html(html)
+        return crystal_html.parse_crystal_html(html)  # type: ignore
 
     @cached_property
-    def location(self) -> Optional[DocLocation]:
-        """[Code location][mkdocstrings.handlers.crystal.items.DocLocation] of this method. Can be `None` if unknown."""
+    def location(self) -> DocLocation | None:
+        """[Code location][mkdocstrings_handlers.crystal.items.DocLocation] of this method. Can be `None` if unknown."""
         # https://github.com/crystal-lang/crystal/pull/10122
         loc = self.data.get("location")
         if loc is None:
             url = self.data.get("source_link")
             if url:
                 regex = r"(?P<url>.+?/(?:blob|tree)/[^/]+/(?P<filename>.+)#L(?P<line>\d+))"
                 m = re.fullmatch(regex, url)
                 if m:
                     loc = m.groupdict()
         if loc:
             return self.root.update_url(
-                DocLocation(loc["filename"], loc["line_number"], loc["url"])
+                DocLocation(loc["filename"], int(loc["line_number"]), loc["url"])
             )
+        return None
 
 
 class DocInstanceMethod(DocMethod):
-    """A [DocMethod][mkdocstrings.handlers.crystal.items.DocMethod] representing a Crystal instance method."""
+    """A [DocMethod][mkdocstrings_handlers.crystal.items.DocMethod] representing a Crystal instance method."""
 
     METHOD_SEP = METHOD_ID_SEP = "#"
 
     @property
     def kind(self) -> str:
         return "instance_method"
 
 
 class DocClassMethod(DocMethod):
-    """A [DocMethod][mkdocstrings.handlers.crystal.items.DocMethod] representing a Crystal class method."""
+    """A [DocMethod][mkdocstrings_handlers.crystal.items.DocMethod] representing a Crystal class method."""
 
     METHOD_SEP = METHOD_ID_SEP = "."
 
     @property
     def kind(self) -> str:
         return "class_method"
 
 
 class DocMacro(DocMethod):
-    """A [DocMethod][mkdocstrings.handlers.crystal.items.DocMethod] representing a Crystal macro."""
+    """A [DocMethod][mkdocstrings_handlers.crystal.items.DocMethod] representing a Crystal macro."""
 
     METHOD_ID_SEP = ":"
 
     @property
     def kind(self) -> str:
         return "macro"
 
 
 class DocConstructor(DocClassMethod):
-    """A [DocInstanceMethod][mkdocstrings.handlers.crystal.items.DocInstanceMethod] representing a Crystal macro."""
+    """A [DocInstanceMethod][mkdocstrings_handlers.crystal.items.DocInstanceMethod] representing a Crystal macro."""
 
 
 class DocMapping(Generic[D]):
-    """Represents items contained within a type. A container of [DocItem][mkdocstrings.handlers.crystal.items.DocItem]s."""
+    """Represents items contained within a type. A container of [DocItem][mkdocstrings_handlers.crystal.items.DocItem]s."""
 
     items: Sequence = ()
     search: Mapping[str, Any] = {}
 
     def __new__(cls, items: Sequence[D]) -> DocMapping:
         if not items:
             try:
@@ -427,15 +435,16 @@
             except AttributeError:
                 cls._empty = empty = object.__new__(cls)
             return empty
         return object.__new__(cls)
 
     def __init__(self, items: Sequence[D]):
         self.items = items
-        self.search = search = {}
+        search: dict[str, Any] = {}
+        self.search = search
         for item in self.items:
             search.setdefault(item.rel_id, item)
             search.setdefault(item.name, item)
 
     def __iter__(self) -> Iterator[D]:
         """Iterate over the items like a list."""
         return iter(self.items)
@@ -445,33 +454,33 @@
         return len(self.items)
 
     def __bool__(self) -> bool:
         """`bool(mapping)` to check whether it's non-empty."""
         return bool(self.items)
 
     def __contains__(self, key: str) -> bool:
-        """`"identifier" in mapping` to check whether the mapping contains an item by this identifier (see [DocItem.rel_id][mkdocstrings.handlers.crystal.items.DocItem.rel_id])."""
+        """`"identifier" in mapping` to check whether the mapping contains an item by this identifier (see [DocItem.rel_id][mkdocstrings_handlers.crystal.items.DocItem.rel_id])."""
         return key in self.search
 
     def __getitem__(self, key: str) -> D:
-        """`mapping["identifier"]` to get the item by this identifier (see [DocItem.rel_id][mkdocstrings.handlers.crystal.items.DocItem.rel_id]).
+        """`mapping["identifier"]` to get the item by this identifier (see [DocItem.rel_id][mkdocstrings_handlers.crystal.items.DocItem.rel_id]).
 
         Returns:
-            A [DocItem][mkdocstrings.handlers.crystal.items.DocItem]
+            A [DocItem][mkdocstrings_handlers.crystal.items.DocItem]
         Raises:
             KeyError: if the item is missing.
         """
         return self.search[key]
 
     def __add__(self, other: DocMapping) -> DocMapping:
         if not other:
             return self
         new = object.__new__(type(self))
         new.items = [*self, *other] if self else other.items
-        new.search = collections.ChainMap(new.search, other.search)
+        new.search = collections.ChainMap(new.search, other.search)  # type: ignore
         return new
 
     def __repr__(self):
         items = ", ".join(repr(item.rel_id) for item in self.items)
         return f"{type(self).__name__}{{{items}}}"
 
 
@@ -479,15 +488,15 @@
 class DocLocation:
     """A location in code where an item was found."""
 
     filename: str
     """The absolute path to the file."""
     line: int
     """The (1-based) line number in the file."""
-    url: Optional[str]
+    url: str | None
     """The derived URL of this location on a source code hosting site."""
 
 
 class DocPath:
     """A path to a documentable Crystal item."""
 
     def __init__(self, data: Mapping[str, Any], root: DocType):
@@ -501,15 +510,15 @@
 
     @property
     def abs_id(self) -> str:
         """The absolute identifier of this item, sometimes known as "path", e.g. `Foo::Bar` or `Foo::Bar#baz`."""
         return self.full_name.split("(", 1)[0]
 
     def lookup(self) -> DocItem:
-        """[Look up][mkdocstrings.handlers.crystal.items.DocItem.lookup] this item in its originating doc structure.
+        """[Look up][mkdocstrings_handlers.crystal.items.DocItem.lookup] this item in its originating doc structure.
 
         Raises:
             CollectionError: When an item by this identifier couldn't be found.
         """
         return self.root.lookup(self.abs_id)
 
     def __str__(self) -> str:
@@ -522,7 +531,17 @@
     def __eq__(self, other) -> bool:
         if isinstance(other, DocPath):
             other = other.abs_id
         return isinstance(other, str) and self.abs_id == other
 
     def __hash__(self):
         return hash(self.abs_id)
+
+
+_doc_type_mapping: Mapping[str, type[DocType]] = {
+    "module": DocModule,
+    "class": DocClass,
+    "struct": DocStruct,
+    "enum": DocEnum,
+    "alias": DocAlias,
+    "annotation": DocAnnotation,
+}
```

### Comparing `mkdocstrings-crystal-0.3.5/mkdocstrings/handlers/crystal/renderer.py` & `mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/renderer.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,34 @@
+from __future__ import annotations
+
 import contextlib
 import xml.etree.ElementTree as etree
-from typing import Optional, TypeVar, Union
+from typing import Any, Mapping, TypeVar
 
 import jinja2
 import markdown_callouts
-from markdown import Markdown  # type: ignore
-from markdown.extensions import Extension, fenced_code  # type: ignore
+from markdown import Markdown
 from markdown.treeprocessors import Treeprocessor
 from markupsafe import Markup
-
 from mkdocstrings.handlers import base
 
 from . import crystal_html
 from .items import DocItem, DocPath
 
 T = TypeVar("T")
 
 
-class CrystalRenderer(base.BaseRenderer):
+class CrystalRenderer(base.BaseHandler):
     fallback_theme = "material"
 
-    def render(self, data: DocItem, config: dict) -> str:
+    @property
+    def collector(self):
+        return self
+
+    def render(self, data: DocItem, config: Mapping[str, Any]) -> str:
         subconfig = {
             "show_source_links": True,
             "heading_level": 2,
             **config,
         }
         template = self.env.get_template(data._TEMPLATE)
 
@@ -42,32 +46,32 @@
     def update_env(self, md: Markdown, config: dict) -> None:
         super().update_env(md, config)
         self._md = md
 
         self._pymdownx_hl = None
         for ext in md.registeredExtensions:
             try:
-                self._pymdownx_hl = ext.get_pymdownx_highlighter()
+                self._pymdownx_hl = ext.get_pymdownx_highlighter()  # type: ignore
             except AttributeError:
                 pass
 
         # Disallow raw HTML.
-        del md.preprocessors["html_block"]
-        del md.inlinePatterns["html"]
+        md.preprocessors.deregister("html_block")
+        md.inlinePatterns.deregister("html")
 
         md.treeprocessors.register(_RefInsertingTreeprocessor(md), "mkdocstrings_crystal_xref", 12)
         markdown_callouts.CalloutsExtension().extendMarkdown(md)
 
         self.env.trim_blocks = True
         self.env.lstrip_blocks = True
         self.env.keep_trailing_newline = False
         self.env.undefined = jinja2.StrictUndefined
 
         self.env.filters["code_highlight"] = self.do_code_highlight
-        self.env.filters["convert_markdown"] = self.do_convert_markdown
+        self.env.filters["convert_markdown_ctx"] = self.do_convert_markdown_ctx
         self.env.filters["reference"] = self.do_reference
 
     def do_code_highlight(self, code, *, title: str = "", **kwargs) -> str:
         text = str(code)
         stext = text.lstrip()
         indent = text[: len(text) - len(stext)]
         html = self.env.filters["highlight"](stext, **kwargs)
@@ -78,28 +82,30 @@
         if isinstance(code, crystal_html.TextWithLinks):
             html = crystal_html.linkify_highlighted_html(html, code.tokens, self.do_reference)
         if title:
             prefix = Markup('<span class="doc-title">{}</span>').format(title)
             html = html.replace(tag_end, tag_end + prefix, 1)
         return html
 
-    def do_reference(self, path: Union[str, DocPath], text: Optional[str] = None) -> str:
+    def do_reference(self, path: str | DocPath, text: str | None = None) -> str:
         if text is None:
             text = str(path)
         if "(" in str(path):
             return text
         try:
             ref_obj = self.collector.root.lookup(path)
         except base.CollectionError:
             return text
         else:
             html = '<span data-autorefs-optional="{}">{}</span>'
             return Markup(html).format(ref_obj.abs_id, text)
 
-    def do_convert_markdown(self, text: str, context: DocItem, heading_level: int, html_id: str):
+    def do_convert_markdown_ctx(
+        self, text: str, context: DocItem, heading_level: int, html_id: str
+    ):
         self._md.treeprocessors["mkdocstrings_crystal_xref"].context = context
         return super().do_convert_markdown(text, heading_level=heading_level, html_id=html_id)
 
     def _monkeypatch_highlight_function(self, default_lang: str):
         """Changes 'pymdownx.highlight' extension to use this lang by default."""
         # Yes, there really isn't a better way. I'd be glad to be proven wrong.
         if self._pymdownx_hl:
@@ -118,15 +124,15 @@
     try:
         yield
     finally:
         setattr(obj, attr, old)
 
 
 class _RefInsertingTreeprocessor(Treeprocessor):
-    context: Optional[DocItem]
+    context: DocItem | None
 
     def __init__(self, md):
         super().__init__(md)
         self.context = None
 
     def run(self, root: etree.Element):
         for i, el in enumerate(root):
```

### Comparing `mkdocstrings-crystal-0.3.5/mkdocstrings/templates/crystal/material/method.html` & `mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/templates/material/method.html`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 <div class="doc doc-object doc-method doc-{{ obj.kind }}">
   {% filter heading(heading_level, id=obj.abs_id, class="doc doc-heading", toc_label=obj.short_name) -%}
     {% if obj.is_abstract %}<small>abstract</small> {% endif %}
     {{ obj.args_string |code_highlight(title=obj.short_name, language="crystal", inline=True) }}
   {%- endfilter %}
 
   <div class="doc doc-contents {% if root %}first{% endif %}">
-    {% if obj.doc %}{{ obj.doc |convert_markdown(obj, heading_level, obj.abs_id) }}{% endif %}
+    {% if obj.doc %}{{ obj.doc |convert_markdown_ctx(obj, heading_level, obj.abs_id) }}{% endif %}
   </div>
 
   {% if config.show_source_links and obj.location and obj.location.url %}
     <a class="doc-source-link" href="{{ obj.location.url }}">View source</a>
   {% endif %}
 </div>
```

### Comparing `mkdocstrings-crystal-0.3.5/mkdocstrings/templates/crystal/material/style.css` & `mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/templates/material/style.css`

 * *Files identical despite different names*

### Comparing `mkdocstrings-crystal-0.3.5/mkdocstrings/templates/crystal/material/type.html` & `mkdocstrings_crystal-0.3.6/mkdocstrings_handlers/crystal/templates/material/type.html`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     {% if obj.superclass %}
       <br/><small>inherits <code>{{ obj.superclass |reference }}</code></small>
     {% endif %}
   {%- endfilter %}
   {% endif %}
 
   <div class="doc doc-contents {% if root %}first{% endif %}">
-    {% if obj.doc %}{{ obj.doc |convert_markdown(obj, heading_level, obj.abs_id) }}{% endif %}
+    {% if obj.doc %}{{ obj.doc |convert_markdown_ctx(obj, heading_level, obj.abs_id) }}{% endif %}
 
     {% with root = False, heading_level = heading_level + 1 %}
       <div class="doc doc-children">
         {% if obj.kind == "alias" %}
           <h{{ heading_level }}>Alias definition</h{{ heading_level }}>
           {{ obj.aliased |code_highlight(language="crystal", inline=True) }}
         {% endif %}
```

### Comparing `mkdocstrings-crystal-0.3.5/setup.py` & `mkdocstrings_crystal-0.3.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,107 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['mkdocstrings', 'mkdocstrings.handlers.crystal']
-
-package_data = \
-{'': ['*'], 'mkdocstrings': ['templates/crystal/material/*']}
-
-install_requires = \
-['Jinja2>=2.11.2,<4.0',
- 'cached-property',
- 'markdown-callouts>=0.1.0',
- 'markupsafe>=1.1.1,<3.0',
- 'mkdocs-autorefs>=0.2.0',
- 'mkdocstrings>=0.15.1']
-
-entry_points = \
-{'markdown.extensions': ['deduplicate-toc = '
-                         'mkdocstrings.handlers.crystal.deduplicate_toc:DeduplicateTocExtension']}
-
-setup_kwargs = {
-    'name': 'mkdocstrings-crystal',
-    'version': '0.3.5',
-    'description': 'Crystal language doc generator for mkdocstrings',
-    'long_description': "# mkdocstrings-crystal\n\n**[Crystal][] language doc generator for [MkDocs][], via [mkdocstrings][]**\n\n[![PyPI](https://img.shields.io/pypi/v/mkdocstrings-crystal)](https://pypi.org/project/mkdocstrings-crystal/)\n[![GitHub](https://img.shields.io/github/license/oprypin/mkdocstrings-crystal)](https://github.com/mkdocstrings/crystal/blob/master/LICENSE.md)\n[![GitHub Workflow Status](https://img.shields.io/github/workflow/status/oprypin/mkdocstrings-crystal/CI)](https://github.com/mkdocstrings/crystal/actions?query=event%3Apush+branch%3Amaster)\n\n## Introduction\n\n*mkdocstrings-crystal* allows you to insert API documentation (generated from [Crystal][]'s source code and doc comments) as part of any page on a [MkDocs][] site.\n\n[See it in action][showcase].\n\nTo install it, run (possibly in a [virtualenv][]):\n\n```shell\npip install mkdocstrings-crystal\n```\n\n**Continue to the [documentation site][].**\n\n## Usage\n\nWith [MkDocs][], add/merge this base config as your _mkdocs.yml_:\n\n```yaml\nsite_name: My Project\n\ntheme:\n  name: material\n\nplugins:\n  - search\n  - mkdocstrings:\n      default_handler: crystal\n\nmarkdown_extensions:\n  - pymdownx.highlight\n  - deduplicate-toc\n```\n\nThen, in any `docs/**/*.md` file, you can **mention a Crystal identifier alone on a line, after `:::`**:\n\n```md\n::: MyClass\n\n::: Other::Class#some_method\n\n::: Foo::CONSTANT\n```\n\n-- and in the output this will be replaced with generated API documentation for it, much like Crystal's own doc generator does.\n\nThis, of course, happens as part of a normal MkDocs build process:\n\n```shell\nmkdocs build  # generate from docs/ into site/\nmkdocs serve  # live preview\n```\n\n**Continue to the [documentation site][].**\n\n\n[crystal]: https://crystal-lang.org/\n[mkdocs]: https://www.mkdocs.org/\n[mkdocstrings]: https://mkdocstrings.github.io/\n[virtualenv]: https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment\n[documentation site]: https://mkdocstrings.github.io/crystal/\n[showcase]: https://mkdocstrings.github.io/crystal/showcase.html\n",
-    'author': 'Oleh Prypin',
-    'author_email': 'oleh@pryp.in',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/mkdocstrings/crystal',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: mkdocstrings-crystal
+Version: 0.3.6
+Summary: Crystal language doc generator for mkdocstrings
+Project-URL: Documentation, https://mkdocstrings.github.io/crystal/
+Project-URL: Source, https://github.com/mkdocstrings/crystal
+Project-URL: Issues, https://github.com/mkdocstrings/crystal/issues
+Project-URL: History, https://github.com/mkdocstrings/crystal/releases
+Author-email: Oleh Prypin <oleh@pryp.in>
+License-Expression: MIT
+License-File: LICENSE.md
+Keywords: crystal,mkdocs,mkdocs-plugin,mkdocstrings
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Console
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Documentation
+Classifier: Topic :: Software Development :: Documentation
+Classifier: Topic :: Text Processing :: Markup :: Markdown
+Classifier: Typing :: Typed
+Requires-Python: >=3.7
+Requires-Dist: cached-property>=1.5.2; python_version < '3.8'
+Requires-Dist: jinja2>=2.11.2
+Requires-Dist: markdown-callouts>=0.1.0
+Requires-Dist: markupsafe>=1.1.1
+Requires-Dist: mkdocs-autorefs>=0.3.1
+Requires-Dist: mkdocstrings>=0.19.0
+Description-Content-Type: text/markdown
+
+# mkdocstrings-crystal
+
+**[Crystal][] language doc generator for [MkDocs][], via [mkdocstrings][]**
+
+[![PyPI](https://img.shields.io/pypi/v/mkdocstrings-crystal)](https://pypi.org/project/mkdocstrings-crystal/)
+[![GitHub](https://img.shields.io/github/license/oprypin/mkdocstrings-crystal)](https://github.com/mkdocstrings/crystal/blob/master/LICENSE.md)
+[![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/oprypin/mkdocstrings-crystal/ci.yml.svg)](https://github.com/mkdocstrings/crystal/actions?query=event%3Apush+branch%3Amaster)
+
+## Introduction
+
+*mkdocstrings-crystal* allows you to insert API documentation (generated from [Crystal][]'s source code and doc comments) as part of any page on a [MkDocs][] site.
+
+[See it in action][showcase].
+
+To install it, run (possibly in a [virtualenv][]):
+
+```shell
+pip install mkdocstrings-crystal
+```
+
+**Continue to the [documentation site][].**
+
+## Usage
+
+With [MkDocs][], add/merge this base config as your _mkdocs.yml_:
+
+```yaml
+site_name: My Project
+
+theme:
+  name: material
+
+plugins:
+  - search
+  - mkdocstrings:
+      default_handler: crystal
+
+markdown_extensions:
+  - pymdownx.highlight
+  - deduplicate-toc
+```
+
+Then, in any `docs/**/*.md` file, you can **mention a Crystal identifier alone on a line, after `:::`**:
+
+```md
+::: MyClass
+
+::: Other::Class#some_method
+
+::: Foo::CONSTANT
+```
+
+-- and in the output this will be replaced with generated API documentation for it, much like Crystal's own doc generator does.
+
+This, of course, happens as part of a normal MkDocs build process:
+
+```shell
+mkdocs build  # generate from docs/ into site/
+mkdocs serve  # live preview
+```
+
+**Continue to the [documentation site][].**
+
+
+[crystal]: https://crystal-lang.org/
+[mkdocs]: https://www.mkdocs.org/
+[mkdocstrings]: https://mkdocstrings.github.io/
+[virtualenv]: https://packaging.python.org/guides/installing-using-pip-and-virtual-environments/#creating-a-virtual-environment
+[documentation site]: https://mkdocstrings.github.io/crystal/
+[showcase]: https://mkdocstrings.github.io/crystal/showcase.html
```


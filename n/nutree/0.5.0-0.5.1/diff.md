# Comparing `tmp/nutree-0.5.0.tar.gz` & `tmp/nutree-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nutree-0.5.0.tar", last modified: Sun May 28 05:58:00 2023, max compression
+gzip compressed data, was "nutree-0.5.1.tar", last modified: Mon May 29 07:27:27 2023, max compression
```

## Comparing `nutree-0.5.0.tar` & `nutree-0.5.1.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-28 05:58:00.289837 nutree-0.5.0/
--rw-r--r--   0 martin     (501) staff       (20)      434 2023-05-27 14:52:54.000000 nutree-0.5.0/CHANGELOG.md
--rw-r--r--   0 martin     (501) staff       (20)     1069 2022-04-14 19:35:21.000000 nutree-0.5.0/LICENSE.txt
--rw-r--r--   0 martin     (501) staff       (20)     4059 2023-05-28 05:58:00.289909 nutree-0.5.0/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     2697 2023-05-20 19:09:46.000000 nutree-0.5.0/README.md
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-28 05:58:00.287783 nutree-0.5.0/nutree/
--rw-r--r--   0 martin     (501) staff       (20)     1083 2023-05-28 05:57:59.000000 nutree-0.5.0/nutree/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     6612 2023-05-27 12:18:02.000000 nutree-0.5.0/nutree/common.py
--rw-r--r--   0 martin     (501) staff       (20)     5910 2023-05-14 15:31:30.000000 nutree-0.5.0/nutree/diff.py
--rw-r--r--   0 martin     (501) staff       (20)     5287 2023-05-14 15:30:35.000000 nutree-0.5.0/nutree/dot.py
--rw-r--r--   0 martin     (501) staff       (20)     2752 2023-03-08 20:01:17.000000 nutree-0.5.0/nutree/fs.py
--rw-r--r--   0 martin     (501) staff       (20)    47535 2023-05-27 14:41:28.000000 nutree-0.5.0/nutree/node.py
--rw-r--r--   0 martin     (501) staff       (20)     4552 2023-05-14 15:37:56.000000 nutree-0.5.0/nutree/rdf.py
--rw-r--r--   0 martin     (501) staff       (20)    21252 2023-05-27 19:31:30.000000 nutree-0.5.0/nutree/tree.py
--rw-r--r--   0 martin     (501) staff       (20)    23420 2023-05-28 05:54:03.000000 nutree-0.5.0/nutree/typed_tree.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-28 05:58:00.288730 nutree-0.5.0/nutree.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)     4059 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)      590 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)       49 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/entry_points.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2022-04-15 09:27:55.000000 nutree-0.5.0/nutree.egg-info/not-zip-safe
--rw-r--r--   0 martin     (501) staff       (20)       31 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)        7 2023-05-28 05:58:00.000000 nutree-0.5.0/nutree.egg-info/top_level.txt
--rw-r--r--   0 martin     (501) staff       (20)      954 2023-05-20 19:10:43.000000 nutree-0.5.0/pyproject.toml
--rw-r--r--   0 martin     (501) staff       (20)     1875 2023-05-28 05:58:00.290294 nutree-0.5.0/setup.cfg
--rw-r--r--   0 martin     (501) staff       (20)      143 2023-03-08 20:01:17.000000 nutree-0.5.0/setup.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-28 05:58:00.289691 nutree-0.5.0/tests/
--rw-r--r--   0 martin     (501) staff       (20)     5838 2023-03-08 20:01:17.000000 nutree-0.5.0/tests/test_bench.py
--rw-r--r--   0 martin     (501) staff       (20)     2076 2023-03-08 20:01:17.000000 nutree-0.5.0/tests/test_clones.py
--rw-r--r--   0 martin     (501) staff       (20)    26832 2023-05-28 05:48:14.000000 nutree-0.5.0/tests/test_core.py
--rw-r--r--   0 martin     (501) staff       (20)     2429 2023-03-08 20:01:17.000000 nutree-0.5.0/tests/test_diff.py
--rw-r--r--   0 martin     (501) staff       (20)     2034 2023-03-08 20:01:17.000000 nutree-0.5.0/tests/test_objects.py
--rw-r--r--   0 martin     (501) staff       (20)     8820 2023-05-27 11:49:59.000000 nutree-0.5.0/tests/test_serialize.py
--rw-r--r--   0 martin     (501) staff       (20)    14762 2023-05-27 14:44:45.000000 nutree-0.5.0/tests/test_typed_tree.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-29 07:27:27.024646 nutree-0.5.1/
+-rw-r--r--   0 martin     (501) staff       (20)      620 2023-05-29 07:14:28.000000 nutree-0.5.1/CHANGELOG.md
+-rw-r--r--   0 martin     (501) staff       (20)     1069 2022-04-14 19:35:21.000000 nutree-0.5.1/LICENSE.txt
+-rw-r--r--   0 martin     (501) staff       (20)     4059 2023-05-29 07:27:27.024710 nutree-0.5.1/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     2697 2023-05-20 19:09:46.000000 nutree-0.5.1/README.md
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-29 07:27:27.022650 nutree-0.5.1/nutree/
+-rw-r--r--   0 martin     (501) staff       (20)     1083 2023-05-29 07:27:26.000000 nutree-0.5.1/nutree/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     6706 2023-05-29 06:52:18.000000 nutree-0.5.1/nutree/common.py
+-rw-r--r--   0 martin     (501) staff       (20)     5910 2023-05-14 15:31:30.000000 nutree-0.5.1/nutree/diff.py
+-rw-r--r--   0 martin     (501) staff       (20)     5269 2023-05-29 06:18:17.000000 nutree-0.5.1/nutree/dot.py
+-rw-r--r--   0 martin     (501) staff       (20)     2752 2023-03-08 20:01:17.000000 nutree-0.5.1/nutree/fs.py
+-rw-r--r--   0 martin     (501) staff       (20)    47535 2023-05-29 07:24:06.000000 nutree-0.5.1/nutree/node.py
+-rw-r--r--   0 martin     (501) staff       (20)     4552 2023-05-14 15:37:56.000000 nutree-0.5.1/nutree/rdf.py
+-rw-r--r--   0 martin     (501) staff       (20)    22000 2023-05-29 07:22:21.000000 nutree-0.5.1/nutree/tree.py
+-rw-r--r--   0 martin     (501) staff       (20)    23518 2023-05-29 06:52:58.000000 nutree-0.5.1/nutree/typed_tree.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-29 07:27:27.023500 nutree-0.5.1/nutree.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)     4059 2023-05-29 07:27:26.000000 nutree-0.5.1/nutree.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)      590 2023-05-29 07:27:27.000000 nutree-0.5.1/nutree.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2023-05-29 07:27:26.000000 nutree-0.5.1/nutree.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)       49 2023-05-29 07:27:26.000000 nutree-0.5.1/nutree.egg-info/entry_points.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2022-04-15 09:27:55.000000 nutree-0.5.1/nutree.egg-info/not-zip-safe
+-rw-r--r--   0 martin     (501) staff       (20)       31 2023-05-29 07:27:26.000000 nutree-0.5.1/nutree.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)        7 2023-05-29 07:27:26.000000 nutree-0.5.1/nutree.egg-info/top_level.txt
+-rw-r--r--   0 martin     (501) staff       (20)      900 2023-05-28 06:10:07.000000 nutree-0.5.1/pyproject.toml
+-rw-r--r--   0 martin     (501) staff       (20)     1875 2023-05-29 07:27:27.025082 nutree-0.5.1/setup.cfg
+-rw-r--r--   0 martin     (501) staff       (20)      143 2023-05-28 06:12:29.000000 nutree-0.5.1/setup.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-29 07:27:27.040570 nutree-0.5.1/tests/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2023-05-29 07:27:27.042899 nutree-0.5.1/tests/__pycache__/
+-rw-r--r--   0 martin     (501) staff       (20)     9558 2023-05-29 07:27:27.042768 nutree-0.5.1/tests/__pycache__/test_bench.cpython-311-pytest-7.2.2.pyc
+-rw-r--r--   0 martin     (501) staff       (20)     5838 2023-03-08 20:01:17.000000 nutree-0.5.1/tests/test_bench.py
+-rw-r--r--   0 martin     (501) staff       (20)     2076 2023-03-08 20:01:17.000000 nutree-0.5.1/tests/test_clones.py
+-rw-r--r--   0 martin     (501) staff       (20)    26832 2023-05-28 05:48:14.000000 nutree-0.5.1/tests/test_core.py
+-rw-r--r--   0 martin     (501) staff       (20)     2429 2023-03-08 20:01:17.000000 nutree-0.5.1/tests/test_diff.py
+-rw-r--r--   0 martin     (501) staff       (20)     2034 2023-03-08 20:01:17.000000 nutree-0.5.1/tests/test_objects.py
+-rw-r--r--   0 martin     (501) staff       (20)     8832 2023-05-29 07:22:57.000000 nutree-0.5.1/tests/test_serialize.py
+-rw-r--r--   0 martin     (501) staff       (20)    15181 2023-05-29 07:15:08.000000 nutree-0.5.1/tests/test_typed_tree.py
```

### Comparing `nutree-0.5.0/LICENSE.txt` & `nutree-0.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/PKG-INFO` & `nutree-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutree
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python library for tree data structures with an intuitive, yet powerful, API.
 Home-page: https://github.com/mar10/nutree/
 Author: Martin Wendt
 Author-email: nutree@wwwendt.de
 Maintainer: Martin Wendt
 Maintainer-email: nutree@wwwendt.de
 License: MIT
```

### Comparing `nutree-0.5.0/README.md` & `nutree-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/nutree/__init__.py` & `nutree-0.5.1/nutree/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     Developmental release (to mark 3.0.0 as 'used'. Don't publish this):
         '3.0.0.dev1'
 NOTE:
     When pywin32 is installed, number must be a.b.c for MSI builds?
     "3.0.0a4" seems not to work in this case!
 """
 # flake8: noqa
-__version__ = "0.5.0"
+__version__ = "0.5.1"
 
 from .common import (
     AmbiguousMatchError,
     IterMethod,
     SelectBranch,
     SkipBranch,
     StopTraversal,
```

### Comparing `nutree-0.5.0/nutree/common.py` & `nutree-0.5.1/nutree/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 if TYPE_CHECKING:  # Imported by type checkers, but prevent circular includes
     from .tree import Node
 
 #: Used as ID for the system root node
 ROOT_ID: str = "__root__"
 
-#: File format version used by `tree.save()` as `meta.$version`
+#: File format version used by `tree.save()` as `meta.$format_version`
 FILE_FORMAT_VERSION: str = "1.0"
 
 ItemIdType = Union[str, int]
 
 
 class TreeError(RuntimeError):
     """Base class for all `nutree` errors."""
@@ -116,14 +116,20 @@
     "round32": ("   ", "│  ", "╰─ ", "├─ "),
     "round42": ("    ", " │  ", " ╰─ ", " ├─ "),
     "round43": ("    ", "│   ", "╰── ", "├── "),
     "round43r": ("    ", " │  ", " ╰──", " ├──"),
 }
 
 
+def get_version() -> str:
+    from nutree import __version__
+
+    return __version__
+
+
 def call_mapper(fn, node: Node, data: dict) -> Any:
     """Call the function and normalize result and exceptions.
 
     Handles `MapperCallbackType`:
     Call `fn(node, data)` if defined and return the result.
     If `fn` is undefined or returns `None`, return `data`.
     """
```

### Comparing `nutree-0.5.0/nutree/diff.py` & `nutree-0.5.1/nutree/diff.py`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/nutree/dot.py` & `nutree-0.5.1/nutree/dot.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 Functions and declarations to support 
 `Graphviz <https://graphviz.org/doc/info/lang.html>`_.
 """
 from __future__ import annotations
 
-from pathlib import Path, PurePath
+from pathlib import Path
 from typing import IO, TYPE_CHECKING, Generator, Union
 
 from .common import MapperCallbackType, call_mapper
 
 if TYPE_CHECKING:  # Imported by type checkers, but prevent circular includes
     from .node import Node
     from .tree import Tree
@@ -105,29 +105,29 @@
         yield f"{indent}{_key(n._parent)} -> {_key(n)}{attr_str}"
 
     yield "}"
 
 
 def tree_to_dotfile(
     tree: Tree,
-    target: Union[IO[str], str, PurePath],
+    target: Union[IO[str], str, Path],
     *,
     format=None,
     add_root=True,
     unique_nodes=True,
     graph_attrs=None,
     node_attrs=None,
     edge_attrs=None,
     node_mapper: MapperCallbackType = None,
     edge_mapper: MapperCallbackType = None,
 ):
     if isinstance(target, str):
         target = Path(target)
 
-    if isinstance(target, PurePath):
+    if isinstance(target, Path):
         if format:
             dot_path = target.with_suffix(".gv")
         else:
             dot_path = target
 
         # print("write", dot_path)
         with open(dot_path, "w") as fp:
```

### Comparing `nutree-0.5.0/nutree/fs.py` & `nutree-0.5.1/nutree/fs.py`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/nutree/node.py` & `nutree-0.5.1/nutree/node.py`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/nutree/rdf.py` & `nutree-0.5.1/nutree/rdf.py`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/nutree/tree.py` & `nutree-0.5.1/nutree/tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 Declare the :class:`~nutree.tree.Tree` class.
 """
 from __future__ import annotations
 
 import json
 import random
 import threading
-from pathlib import PurePath
+from pathlib import Path
 from typing import IO, Any, Dict, Generator, List, Union
 
 from nutree.diff import diff_tree
 
 from .common import (
     FILE_FORMAT_VERSION,
     ROOT_ID,
     AmbiguousMatchError,
     ItemIdType,
     IterMethod,
     MapperCallbackType,
     PredicateCallbackType,
     TraversalCallbackType,
     call_mapper,
+    get_version,
 )
 from .dot import tree_to_dotfile
 from .node import Node
 from .rdf import tree_to_rdf
 
 _DELETED_TAG = "<deleted>"
 
@@ -393,63 +394,72 @@
         """Sort toplevel nodes (optionally recursively).
 
         `key` defaults to ``attrgetter("name")``, so children are sorted by
         their string representation.
         """
         self._root.sort_children(key=key, reverse=reverse, deep=deep)
 
-    def to_dict(self, *, mapper: MapperCallbackType = None) -> List[Dict]:
+    def to_dict_list(self, *, mapper: MapperCallbackType = None) -> List[Dict]:
         """Call Node's :meth:`~nutree.node.Node.to_dict` method for all
         childnodes and return list of results."""
         res = []
         with self:
             for n in self._root._children:
                 res.append(n.to_dict(mapper=mapper))
         return res
 
     @classmethod
     def from_dict(cls, obj: List[Dict], *, mapper=None) -> Tree:
         """Return a new :class:`Tree` instance from a list of dicts.
 
-        See also :meth:`~nutree.tree.Tree.to_dict` and
+        See also :meth:`~nutree.tree.Tree.to_dict_list` and
         Node's :meth:`~nutree.node.Node.find_first` methods, and
         :ref:`iteration callbacks`.
         """
         new_tree = Tree()
         new_tree._root.from_dict(obj, mapper=mapper)
         return new_tree
 
     def to_list_iter(
         self, *, mapper: MapperCallbackType = None
     ) -> Generator[Dict, None, None]:
         """Yield a parent-referencing list of child nodes."""
         return self._root.to_list_iter(mapper=mapper)
 
     def save(
-        self, fp: IO[str], *, mapper: MapperCallbackType = None, meta: dict = None
+        self,
+        target: Union[IO[str], str, Path],
+        *,
+        mapper: MapperCallbackType = None,
+        meta: dict = None,
     ) -> None:
         """Store tree in a compact JSON file stream.
 
         See also :meth:`to_list_iter` and :meth:`load` methods.
         """
+        if isinstance(target, (str, Path)):
+            with Path(target).open("wt") as fp:
+                return self.save(target=fp, mapper=mapper, meta=meta)
+        # target is a file object now
+
         header = {
-            "$version": FILE_FORMAT_VERSION,
-            # "$nutree_version": __version__,
+            "$generator": f"nutree/{get_version()}",
+            "$format_version": FILE_FORMAT_VERSION,
         }
         if meta:
             header.update(meta)
         with self:
             # Materialize node list, so we can lock the snapshot.
             # Also because json.dump() does not support streaming anyway.
             # TODO: Use s.th. like https://github.com/daggaz/json-stream ?
             res = {
                 "meta": header,
                 "nodes": list(self.to_list_iter(mapper=mapper)),
             }
-        json.dump(res, fp)
+        json.dump(res, target)
         return
 
     @classmethod
     def _from_list(cls, obj: List[Dict], *, mapper=None) -> Tree:
         tree = cls()  # Tree or TypedTree
         node_idx_map = {0: tree._root}
         for idx, (parent_idx, data) in enumerate(obj, 1):
@@ -467,25 +477,43 @@
                 raise RuntimeError(f"Need mapper for {data}")  # pragma: no cover
 
             node_idx_map[idx] = n
 
         return tree
 
     @classmethod
-    def load(cls, fp: IO[str], *, mapper=None, file_meta: dict = None) -> Tree:
-        """Create a new :class:`Tree` instance from a JSON file stream.
+    def load(
+        cls,
+        target: Union[IO[str], str, Path],
+        *,
+        mapper=None,
+        file_meta: dict = None,
+    ) -> Tree:
+        """Create a new :class:`Tree` instance from a file path or JSON file stream.
 
         If ``file_meta`` is a dict, it receives the content if the file's
         ``meta`` header.
 
         See also :meth:`save`.
         """
-        obj = json.load(fp)
-        if not isinstance(obj, dict) or "meta" not in obj or "nodes" not in obj:
+        if isinstance(target, (str, Path)):
+            with Path(target).open("rt") as fp:
+                return cls.load(target=fp, mapper=mapper, file_meta=file_meta)
+        # target is a file object now
+
+        obj = json.load(target)
+        if (
+            not isinstance(obj, dict)
+            or "meta" not in obj
+            or "nodes" not in obj
+            or "$generator" not in obj["meta"]
+            or "nutree/" not in str(obj["meta"]["$generator"])
+        ):
             raise RuntimeError("Invalid file format")
+
         if isinstance(file_meta, dict):
             file_meta.update(obj["meta"])
         nodes = obj["nodes"]
         return cls._from_list(nodes, mapper=mapper)
 
     def to_dot(
         self,
@@ -510,15 +538,15 @@
             edge_attrs=edge_attrs,
             node_mapper=node_mapper,
             edge_mapper=edge_mapper,
         )
 
     def to_dotfile(
         self,
-        target: Union[IO[str], str, PurePath],
+        target: Union[IO[str], str, Path],
         *,
         format=None,
         add_root=True,
         unique_nodes=True,
         graph_attrs=None,
         node_attrs=None,
         edge_attrs=None,
```

### Comparing `nutree-0.5.0/nutree/typed_tree.py` & `nutree-0.5.1/nutree/typed_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # (c) 2021-2023 Martin Wendt; see https://github.com/mar10/nutree
 # Licensed under the MIT license: https://www.opensource.org/licenses/mit-license.php
 """
 Declare the :class:`~nutree.tree.TypedTree` class.
 """
 from __future__ import annotations
 
+from pathlib import Path
 from typing import IO, Any, Dict, Generator, List, Union
 
 from nutree.common import (
     ROOT_ID,
     IterMethod,
     MapperCallbackType,
     PredicateCallbackType,
@@ -671,21 +672,27 @@
                 raise RuntimeError(f"Need mapper for {data}")  # pragma: no cover
 
             node_idx_map[idx] = n
 
         return tree
 
     @classmethod
-    def load(cls, fp: IO[str], *, mapper=None, file_meta: dict = None) -> TypedTree:
+    def load(
+        cls,
+        target: Union[IO[str], str, Path],
+        *,
+        mapper=None,
+        file_meta: dict = None,
+    ) -> TypedTree:
         """Create a new :class:`TypedTree` instance from a JSON file stream.
 
         See also Tree's :meth:`~nutree.tree.Tree.save()` and
         :meth:`~nutree.tree.Tree.load()` methods.
         """
-        return super().load(fp, mapper=mapper, file_meta=file_meta)
+        return super().load(target, mapper=mapper, file_meta=file_meta)
 
 
 # ------------------------------------------------------------------------------
 # - _SystemRootTypedNode
 # ------------------------------------------------------------------------------
 class _SystemRootTypedNode(TypedNode):
     """Invisible system root node."""
```

### Comparing `nutree-0.5.0/nutree.egg-info/PKG-INFO` & `nutree-0.5.1/nutree.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nutree
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python library for tree data structures with an intuitive, yet powerful, API.
 Home-page: https://github.com/mar10/nutree/
 Author: Martin Wendt
 Author-email: nutree@wwwendt.de
 Maintainer: Martin Wendt
 Maintainer-email: nutree@wwwendt.de
 License: MIT
```

### Comparing `nutree-0.5.0/nutree.egg-info/SOURCES.txt` & `nutree-0.5.1/nutree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/pyproject.toml` & `nutree-0.5.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 [tool.black]
 line-length = 88
-# py36 = false  # don't strip 'u' from native strings
 target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 /(
     \.git
   | \.hg
   | \.tox
```

### Comparing `nutree-0.5.0/setup.cfg` & `nutree-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/tests/test_bench.py` & `nutree-0.5.1/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/tests/test_clones.py` & `nutree-0.5.1/tests/test_clones.py`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/tests/test_core.py` & `nutree-0.5.1/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/tests/test_diff.py` & `nutree-0.5.1/tests/test_diff.py`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/tests/test_objects.py` & `nutree-0.5.1/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `nutree-0.5.0/tests/test_serialize.py` & `nutree-0.5.1/tests/test_serialize.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         self.tree = None
 
     def test_serialize_dict(self):
         tree = fixture.create_tree()
 
         with tempfile.TemporaryFile("r+t") as fp:
             # Serialize
-            json.dump(tree.to_dict(), fp)
+            json.dump(tree.to_dict_list(), fp)
             # Deserialize
             fp.seek(0)
             obj = json.load(fp)
             tree_2 = Tree.from_dict(obj)
 
         assert fixture.trees_equal(tree, tree_2)
 
@@ -53,15 +53,15 @@
             # Deserialize
             fp.seek(0)
             meta_2 = {}
             tree_2 = Tree.load(fp, file_meta=meta_2)
 
         assert isinstance(tree_2, Tree)
         assert all(isinstance(n, Node) for n in tree_2)
-        assert meta_2["$version"] == FILE_FORMAT_VERSION
+        assert meta_2["$format_version"] == FILE_FORMAT_VERSION
         assert meta_2["foo"] == "bar"
         assert fixture.trees_equal(tree, tree_2)
 
         # print(tree.format(repr="{node}"))
         # print(tree_2.format(repr="{node}"))
 
         assert tree.count == tree_2.count
```

### Comparing `nutree-0.5.0/tests/test_typed_tree.py` & `nutree-0.5.1/tests/test_typed_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,29 +134,41 @@
         assert not fail1.is_clone()
         func2.add(fail1)
         assert fail1.is_clone()
 
         subtree = func2.copy()
         assert isinstance(subtree, TypedTree)
 
+    def test_to_dict_list(self):
+        tree = fixture.create_typed_tree(clones=True)
+        d = tree.to_dict_list()
+        print(d)
+        assert len(d) == 2, "two top nodes"
+        assert isinstance(d, list)
+        assert isinstance(d[0], dict)
+        # TODO:
+        assert isinstance(d[0]["data"], str)
+        # assert "kind" in l[0]
+
     def test_serialize_list(self):
         tree = fixture.create_typed_tree(clones=True)
         assert isinstance(tree, TypedTree)
 
         with tempfile.TemporaryFile("r+t") as fp:
             # Serialize
             tree.save(fp, meta={"foo": "bar"})
             # Deserialize
             fp.seek(0)
             meta_2 = {}
             tree_2 = TypedTree.load(fp, file_meta=meta_2)
 
         assert isinstance(tree_2, TypedTree)
         assert all(isinstance(n, TypedNode) for n in tree_2)
-        assert meta_2["$version"] == FILE_FORMAT_VERSION
+        assert meta_2["$generator"].startswith("nutree/")
+        assert meta_2["$format_version"] == FILE_FORMAT_VERSION
         assert meta_2["foo"] == "bar"
         assert fixture.trees_equal(tree, tree_2)
 
         # print(tree.format(repr="{node}"))
         # print(tree_2.format(repr="{node}"))
 
         assert tree.count == tree_2.count
@@ -227,15 +239,15 @@
             # Deserialize
             fp.seek(0)
             meta_2 = {}
             tree_2 = TypedTree.load(fp, mapper=deserialize_mapper, file_meta=meta_2)
 
         assert isinstance(tree_2, TypedTree)
         assert all(isinstance(n, TypedNode) for n in tree_2)
-        assert meta_2["$version"] == FILE_FORMAT_VERSION
+        assert meta_2["$format_version"] == FILE_FORMAT_VERSION
         assert meta_2["foo"] == "bar"
         assert fixture.trees_equal(tree, tree_2)
 
         assert tree.count == tree_2.count
         assert tree.first_child(kind=ANY_KIND) is not tree_2.first_child(kind=ANY_KIND)
 
         # TODO: also make a test-case, where the mapper returns a data_id,
```


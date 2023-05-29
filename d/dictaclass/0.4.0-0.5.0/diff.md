# Comparing `tmp/dictaclass-0.4.0.tar.gz` & `tmp/dictaclass-0.5.0.tar.gz`

## Comparing `dictaclass-0.4.0.tar` & `dictaclass-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 dictaclass-0.4.0/.dockerignore
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dictaclass-0.4.0/.env
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dictaclass-0.4.0/requirements.dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dictaclass-0.4.0/requirements.txt
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dictaclass-0.4.0/test.Dockerfile
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 dictaclass-0.4.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 dictaclass-0.4.0/.vscode/settings.json
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dictaclass-0.4.0/dictaclass/__init__.py
--rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 dictaclass-0.4.0/dictaclass/dictaclass.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dictaclass-0.4.0/tests/__init__.py
--rw-r--r--   0        0        0    10746 2020-02-02 00:00:00.000000 dictaclass-0.4.0/tests/test_dictaclass.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 dictaclass-0.4.0/tests/test_meta.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 dictaclass-0.4.0/.gitignore
--rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 dictaclass-0.4.0/LICENSE.txt
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 dictaclass-0.4.0/README.md
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 dictaclass-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 dictaclass-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 dictaclass-0.5.0/.dockerignore
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 dictaclass-0.5.0/.env
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 dictaclass-0.5.0/requirements.dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dictaclass-0.5.0/requirements.txt
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 dictaclass-0.5.0/test.Dockerfile
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 dictaclass-0.5.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 dictaclass-0.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 dictaclass-0.5.0/dictaclass/__init__.py
+-rw-r--r--   0        0        0    10477 2020-02-02 00:00:00.000000 dictaclass-0.5.0/dictaclass/dictaclass.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dictaclass-0.5.0/tests/__init__.py
+-rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 dictaclass-0.5.0/tests/test_dictaclass.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 dictaclass-0.5.0/tests/test_meta.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 dictaclass-0.5.0/.gitignore
+-rw-r--r--   0        0        0    11527 2020-02-02 00:00:00.000000 dictaclass-0.5.0/LICENSE.txt
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 dictaclass-0.5.0/README.md
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 dictaclass-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 dictaclass-0.5.0/PKG-INFO
```

### Comparing `dictaclass-0.4.0/.devcontainer/devcontainer.json` & `dictaclass-0.5.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `dictaclass-0.4.0/dictaclass/dictaclass.py` & `dictaclass-0.5.0/dictaclass/dictaclass.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict, Type, TypeVar, List, Set, Dict, Callable, Union, Optional
+from typing import Any, Dict, Type, TypeVar, List, Set, Dict, Callable, Union, Optional, get_type_hints
 from dataclasses import is_dataclass, asdict
 
 import sys
 
 T = TypeVar("T")
 
 
@@ -17,15 +17,15 @@
 def _to_dataclass_38(
     dataclass_type: Type[T],
     data: Any,
     key_transformer: Callable[[str], str],
     on_extra_field: Callable[[Type, str, Any], None],
     implicit_optional: bool,
 ) -> T:
-    from typing import get_args, get_type_hints, get_origin
+    from typing import get_args, get_origin
 
     dict_value: Any
 
     if not is_dataclass(dataclass_type) or data is None:
         return data
 
     assert isinstance(data, dict)
@@ -128,15 +128,15 @@
 
     dataclass_dict: Dict[str, Any] = dict()
     used_keys: Set[str] = set()
 
     annotations = dict()
     for c in dataclass_type.mro():
         try:
-            annotations.update(c.__annotations__)
+            annotations.update(get_type_hints(c))
         except AttributeError:
             pass
 
     for annotation_name, annotation_type in annotations.items():
         try:
             key = key_transformer(annotation_name)
             dict_value = data[key]
```

### Comparing `dictaclass-0.4.0/tests/test_dictaclass.py` & `dictaclass-0.5.0/tests/test_dictaclass.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 
 from typing import Any, Dict, List, Optional, Set, Tuple, Type, Union
 
 import pytest
 
 
 class Test_Dictaclass:
-    def test_flat(self):
+    def test_flat(self) -> None:
         @dataclass(frozen=True)
         class ExampleDC:
             a: str
             b: int
             c: float
 
         v = to_dataclass(ExampleDC, dict(a="asdf", b=10, c=3.1415))
 
         assert isinstance(v, ExampleDC)
         assert v.a == "asdf"
         assert v.b == 10
         assert v.c == 3.1415
 
-    def test_inheritance(self):
+    def test_inheritance(self) -> None:
         @dataclass(frozen=True)
         class Base:
             a: str
 
         @dataclass(frozen=True)
         class Example(Base):
             b: int
@@ -35,15 +35,15 @@
         v = to_dataclass(Example, dict(a="asdf", b=10, c=3.1415))
 
         assert isinstance(v, Example)
         assert v.a == "asdf"
         assert v.b == 10
         assert v.c == 3.1415
 
-    def test_optional_values(self):
+    def test_optional_values(self) -> None:
         @dataclass(frozen=True)
         class Example:
             b: int
             c: float = 0.0
 
         v = to_dataclass(Example, dict(b=10, c=3.1415))
         assert isinstance(v, Example)
@@ -51,54 +51,54 @@
         assert v.c == 3.1415
 
         v = to_dataclass(Example, dict(b=10))
         assert isinstance(v, Example)
         assert v.b == 10
         assert v.c == 0
 
-    def test_with_primitive_list(self):
+    def test_with_primitive_list(self) -> None:
         @dataclass(frozen=True)
         class ExampleDC:
             a: str
             b: List[int]
 
         v = to_dataclass(ExampleDC, dict(a="asdf", b=[1, 2, 3]))
 
         assert isinstance(v, ExampleDC)
         assert v.a == "asdf"
         assert isinstance(v.b, list)
         assert v.b == [1, 2, 3]
 
-    def test_with_primitive_set(self):
+    def test_with_primitive_set(self) -> None:
         @dataclass(frozen=True)
         class ExampleDC:
             a: str
             b: Set[int]
 
         v = to_dataclass(ExampleDC, dict(a="asdf", b=[1, 2, 3]))
 
         assert isinstance(v, ExampleDC)
         assert v.a == "asdf"
         assert isinstance(v.b, set)
         assert v.b == {1, 2, 3}
 
-    def test_with_primitive_dict(self):
+    def test_with_primitive_dict(self) -> None:
         @dataclass(frozen=True)
         class ExampleDC:
             a: str
             b: Dict[str, int]
 
         v = to_dataclass(ExampleDC, dict(a="asdf", b=dict(a=1, b=2)))
 
         assert isinstance(v, ExampleDC)
         assert v.a == "asdf"
         assert isinstance(v.b, dict)
         assert v.b == dict(a=1, b=2)
 
-    def test_with_nested_list(self):
+    def test_with_nested_list(self) -> None:
         @dataclass(frozen=True)
         class Pair:
             first: str
             last: str
 
         @dataclass(frozen=True)
         class Object:
@@ -127,15 +127,15 @@
         assert isinstance(v.pairs[1].last, str)
 
         assert v.pairs[0].first == "f0"
         assert v.pairs[0].last == "l0"
         assert v.pairs[1].first == "f1"
         assert v.pairs[1].last == "l1"
 
-    def test_with_nested_primitive_list(self):
+    def test_with_nested_primitive_list(self) -> None:
         @dataclass(frozen=True)
         class Object:
             pairs: List[List[str]]
 
         v = to_dataclass(
             Object,
             {
@@ -151,15 +151,15 @@
         assert isinstance(v.pairs[0], list)
         assert isinstance(v.pairs[1], list)
         assert v.pairs == [
             ["a", "b", "c"],
             ["d", "e", "f"],
         ]
 
-    def test_with_nested_set(self):
+    def test_with_nested_set(self) -> None:
         @dataclass(frozen=True)
         class Pair:
             first: str
             last: str
 
         @dataclass(frozen=True)
         class Object:
@@ -177,15 +177,15 @@
         assert isinstance(v, Object)
         assert isinstance(v.pairs, set)
         assert v.pairs == {
             Pair("f0", "l0"),
             Pair("f1", "l1"),
         }
 
-    def test_with_nested_dict(self):
+    def test_with_nested_dict(self) -> None:
         @dataclass(frozen=True)
         class Pair:
             first: str
             last: str
 
         @dataclass(frozen=True)
         class Object:
@@ -214,15 +214,15 @@
         assert isinstance(v.pairs["p1"].last, str)
 
         assert v.pairs["p0"].first == "f0"
         assert v.pairs["p0"].last == "l0"
         assert v.pairs["p1"].first == "f1"
         assert v.pairs["p1"].last == "l1"
 
-    def test_with_nested_set_2(self):
+    def test_with_nested_set_2(self) -> None:
         import json
 
         @dataclass(frozen=True)
         class Pair:
             first: str
             last: str
 
@@ -249,15 +249,15 @@
         )
 
         assert isinstance(v, Object)
         assert isinstance(v.pairs, set)
         assert len(v.pairs) == 2
         assert v.pairs == {PairPair(Pair("f0", "l0")), PairPair(Pair("f1", "l1"))}
 
-    def test_flat_with_extra_fields(self):
+    def test_flat_with_extra_fields(self) -> None:
         @dataclass(frozen=True)
         class Pair:
             first: str
             last: str
 
         extras = []
         v = to_dataclass(
@@ -271,31 +271,31 @@
         assert v.first == "a"
         assert v.last == "b"
         assert not hasattr(v, "middle")
         assert extras == [
             (Pair, "middle", "lol"),
         ]
 
-    def test_nested_with_extra_fields(self):
+    def test_nested_with_extra_fields(self) -> None:
         @dataclass(frozen=True)
         class C:
             num: int
 
         @dataclass(frozen=True)
         class B:
             c: C
 
         @dataclass(frozen=True)
         class A:
             b: B
 
         extras: List[Tuple[Type[Any], str, Any]] = []
 
-        def on_extra_field(*args):
-            extras.append(args)
+        def on_extra_field(data_type: Type[Any], key: str, value: Any):
+            extras.append((data_type, key, value))
 
         a = to_dataclass(
             A,
             dict(b=dict(c=dict(num=10, extra_num=11), extra_num=12), extra_num=13),
             on_extra_field=on_extra_field,
         )
         assert isinstance(a, A)
@@ -308,16 +308,50 @@
         assert extras == [
             (C, "extra_num", 11),
             (B, "extra_num", 12),
             (A, "extra_num", 13),
         ]
 
 
+class Test_Dictaclass_OrderedDict:
+    def test_with_nested_class(self) -> None:
+        from collections import OrderedDict
+
+        @dataclass(frozen=True)
+        class Child:
+            name: str
+            level: int
+
+        @dataclass(frozen=True)
+        class Parent:
+            child: Child
+
+        v = to_dataclass(
+            Parent,
+            OrderedDict(
+                {
+                    "child": OrderedDict(
+                        {
+                            "name": "asdf",
+                            "level": 10,
+                        }
+                    )
+                }
+            ),
+        )
+
+        assert isinstance(v, Parent)
+        assert v
+        assert v.child
+        assert v.child.name == "asdf"
+        assert v.child.level == 10
+
+
 class Test_Dataclass_Optional:
-    def test_flat_with_implicit_optional(self):
+    def test_flat_with_implicit_optional(self) -> None:
         @dataclass
         class Example:
             a: int
             b: Dict[str, str]
             c: List[str]
             d: Set[str]
 
@@ -331,15 +365,15 @@
         assert r.d is None
 
         with pytest.raises(AssertionError):
             r = to_dataclass(
                 Example, dict(a=None, b=None, c=None, d=None), implicit_optional=False
             )
 
-    def test_flat_with_explicit_optional(self):
+    def test_flat_with_explicit_optional(self) -> None:
         @dataclass
         class Example:
             a: Optional[int]
             b: Optional[Dict[str, str]]
             c: Optional[List[str]]
             d: Optional[Set[str]]
 
@@ -355,34 +389,35 @@
         r = to_dataclass(Example, dict(a=1, b={}, c=[], d=[]), implicit_optional=False)
         assert isinstance(r, Example)
         assert r.a == 1
         assert r.b == {}
         assert r.c == []
         assert r.d == set()
 
-    def test_nested_with_explicit_optional(self):
+    def test_nested_with_explicit_optional(self) -> None:
         @dataclass
         class ExampleG:
             a: int
 
         @dataclass
         class Example:
             g: Optional[ExampleG]
 
         r = to_dataclass(Example, dict(g=None))
         assert isinstance(r, Example)
         assert r.g is None
 
         r = to_dataclass(Example, dict(g=dict(a=10)))
         assert isinstance(r, Example)
+        assert r.g is not None
         assert r.g.a == 10
 
 
 class Test_Dictaclass_NameTransform:
-    def test_to_snake_case_flat(self):
+    def test_to_snake_case_flat(self) -> None:
         import inflection
 
         @dataclass(frozen=True)
         class ExampleDC:
             url_encoded: str
 
         v = to_dataclass(ExampleDC, dict(UrlEncoded="asdf"), inflection.camelize)
```

### Comparing `dictaclass-0.4.0/tests/test_meta.py` & `dictaclass-0.5.0/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `dictaclass-0.4.0/LICENSE.txt` & `dictaclass-0.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dictaclass-0.4.0/README.md` & `dictaclass-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dictaclass-0.4.0/pyproject.toml` & `dictaclass-0.5.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dictaclass"
-version = "0.4.0"
+version = "0.5.0"
 authors = [
     { name = "Bozhidar Stoyanov", email="glav0r3zzz4@gmail.com"}
 ]
 description = "Convert heirarchies of dicts/list/sets/values (JSON?) to heirarchies of type annotated dataclasses."
 readme = "README.md"
 requires-python = ">=3.7.2"
 classifiers = [
```

### Comparing `dictaclass-0.4.0/PKG-INFO` & `dictaclass-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictaclass
-Version: 0.4.0
+Version: 0.5.0
 Summary: Convert heirarchies of dicts/list/sets/values (JSON?) to heirarchies of type annotated dataclasses.
 Project-URL: Homepage, https://github.com/BraynStorm/dictaclass
 Project-URL: Bug Tracker, https://github.com/BraynStorm/dictaclass/issues
 Author-email: Bozhidar Stoyanov <glav0r3zzz4@gmail.com>
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```


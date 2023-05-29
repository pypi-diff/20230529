# Comparing `tmp/dictkit-0.1.4.tar.gz` & `tmp/dictkit-0.1.5.tar.gz`

## Comparing `dictkit-0.1.4.tar` & `dictkit-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dictkit-0.1.4/dictkit/__init__.py
--rw-r--r--   0        0        0    11072 2020-02-02 00:00:00.000000 dictkit-0.1.4/dictkit/categorize.py
--rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 dictkit-0.1.4/dictkit/render.py
--rw-r--r--   0        0        0    10424 2020-02-02 00:00:00.000000 dictkit-0.1.4/dictkit/utildict.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 dictkit-0.1.4/.gitignore
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 dictkit-0.1.4/README.md
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 dictkit-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 dictkit-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dictkit-0.1.5/dictkit/__init__.py
+-rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 dictkit-0.1.5/dictkit/categorize.py
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 dictkit-0.1.5/dictkit/render.py
+-rw-r--r--   0        0        0    10712 2020-02-02 00:00:00.000000 dictkit-0.1.5/dictkit/utildict.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 dictkit-0.1.5/.gitignore
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 dictkit-0.1.5/README.md
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 dictkit-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 dictkit-0.1.5/PKG-INFO
```

### Comparing `dictkit-0.1.4/dictkit/categorize.py` & `dictkit-0.1.5/dictkit/categorize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import pandas as pd
 from collections import namedtuple
+from typing import (
+    List,
+    Union,
+)
 
 from dictkit import UtilDict
 
 
 def categorize(
     df: pd.DataFrame,
-    by: str | list[str | list[str]],
+    by: Union[str, List[Union[str, List[str]]]],
     drop: bool = False,
     reset_index: bool = True,
     sort_keys: bool = False,
 ) -> UtilDict:
     """
     Break down a dataframe into a nested dictionary of filtered versions
     of the data.
@@ -298,21 +302,21 @@
     if by:
         for k, v in res.items():
             res[k] = categorize(v, by, drop, reset_index, sort_keys)
 
     return res
 
 
-# if __name__ == "__main__":
-#
-#     from dictkit import UtilDict
-#     df = pd.DataFrame(
-#         zip(
-#             ['red'] * 6 + ['gray'] * 6,
-#             ['steak'] * 3 + ['salmon'] * 3 + ['tilapia'] * 3 + ['beef'] * 3,
-#             pd.concat([pd.Series([x] * 2) for x in ['new york', 'vermont', 'kansas', 'florida', 'michigan', 'ohio']]),
-#             list(range(0,12)),
-#             [53,298,2,423,8989,3284,342,2344,2390,243,234,23],
-#         ),
-#         columns=['color','meat','state','ID', 'sales']
-#     )
-#     print(categorize(df, by=['color','meat'], drop=True))
+if __name__ == "__main__":
+
+    from dictkit import UtilDict
+    df = pd.DataFrame(
+        zip(
+            ['red'] * 6 + ['gray'] * 6,
+            ['steak'] * 3 + ['salmon'] * 3 + ['tilapia'] * 3 + ['beef'] * 3,
+            pd.concat([pd.Series([x] * 2) for x in ['new york', 'vermont', 'kansas', 'florida', 'michigan', 'ohio']]),
+            list(range(0,12)),
+            [53,298,2,423,8989,3284,342,2344,2390,243,234,23],
+        ),
+        columns=['color','meat','state','ID', 'sales']
+    )
+    print(categorize(df, by=['color','meat'], drop=True))
```

### Comparing `dictkit-0.1.4/dictkit/render.py` & `dictkit-0.1.5/dictkit/render.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 import re
-from typing import Any, Literal
+from typing import Any, Literal, Union, List, Dict, Tuple, Optional
 
-QuoteOption = bool | Literal["keys"] | Literal["values"]
+QuoteOption = Union[bool, Literal["keys"], Literal["values"]]
 
 def render(
     obj, indent: int = 3, quote: QuoteOption = True, line_spacing=1, shift=" "
 ) -> FormattedReprStr:
     """
     Represent nested dicts, lists, tuples, with json structure, but Python format.
     Displayed content appears as it would when printed, but with nested indentations.
@@ -192,23 +192,23 @@
             return s + indent_existing(fmt_val(val), ind)
 
         items = val.items() if isinstance(val, dict) else [("", x) for x in val]
 
         from_dict = True if isinstance(val, dict) else False
         rendered_items = "".join(
             [_render(k, v, ind + indent, from_dict=from_dict) for k, v in items]
-        ).removesuffix(",")
+        ).rstrip(",")
 
         return s + rendered_items + end
 
     from_dict = True if isinstance(obj, dict) else False
-    return FormattedReprStr(_render("", obj, 0, "", from_dict=from_dict).lstrip("\n").removesuffix(","))
+    return FormattedReprStr(_render("", obj, 0, "", from_dict=from_dict).lstrip("\n").rstrip(","))
 
 
-def get_enclosure(obj) -> tuple[str, str]:
+def get_enclosure(obj) -> Tuple[str, str]:
     if isinstance(obj, list):
         return ("[", "]")
     if isinstance(obj, tuple):
         return ("(", ")")
     if isinstance(obj, dict):
         return ("{", "}")
     return ("", "")
```

### Comparing `dictkit-0.1.4/dictkit/utildict.py` & `dictkit-0.1.5/dictkit/utildict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,21 @@
 from __future__ import annotations
-from collections import ChainMap
-from typing import overload, Iterable, Mapping, TypeVar, Literal
+from collections import ChainMap, abc
+from typing import (
+    overload,
+    Iterable,
+    Mapping,
+    TypeVar,
+    Literal,
+    Optional,
+    Union,
+    Dict,
+    List,
+    Any,
+)
 from copy import copy
 
 
 def is_valid_normal_iterable(item) -> bool:
     """
     Returns True if the average human would say, "Yes, that looks like a
     regular iterable to me"
@@ -22,15 +33,15 @@
 K = TypeVar("K")
 V = TypeVar("V")
 # Key-value types of external arguments passed in
 K2 = TypeVar("K2")
 V2 = TypeVar("V2")
 
 
-class UtilDict(dict[K, V]):
+class UtilDict(Dict[K, V]):
     """
     A better dictionary. Allows getting, setting, adding, and dropping items in useful ways,
     supporting dot notation item access, and getting/setting multiple keys and values at once.
 
     Renders in nested-json style structure, while maintaining default Python value formatting.
 
     Get items with dot notation, if you wish
@@ -143,16 +154,16 @@
                     return super().__init__(zip(*args), **kwargs)  # type:ignore
 
             args = [self._iterable_to_dict(arg) for arg in args]
             args = (ChainMap(*list(reversed(args))),)
         super().__init__(*args, **kwargs)
 
     def add(
-        self, *args: Mapping[K2, V2] | Iterable, **kwargs: V2
-    ) -> UtilDict[K | K2, V | V2]:
+        self, *args: Union[Mapping[K2, V2], Iterable], **kwargs: V2
+    ) -> UtilDict[Union[K, K2], Union[V, V2]]:
         """
         Add items, returning a copy with the new items.
 
         Parameters
         ----------
         *args
             Dictionaries or 2-element iterables
@@ -238,22 +249,24 @@
         for k in keys:
             new.pop(k)
 
         if not inplace:
             return new
 
     @overload
-    def deep_uniform(self, reverse: Literal[False]) -> UtilDict[K, V]:
+    def deep_uniform(self, reverse: Optional[Literal[False]] = False) -> UtilDict[K, V]:
         ...
 
     @overload
-    def deep_uniform(self, reverse: Literal[True]) -> dict:
+    def deep_uniform(self, reverse: Literal[True]) -> Dict:
         ...
 
-    def deep_uniform(self, reverse=False):
+    def deep_uniform(
+        self, reverse: Optional[Literal[True, False]] = False
+    ) -> Union[UtilDict[K, V], Dict]:
         """
         Recursively convert all child instances of `dict` to
         Self's type.
 
         If `reverse=True`, then the opposite happens. Converts all nested UtilDict
         to `dict`, and returns a `dict`
         """
@@ -306,15 +319,15 @@
             super().__setitem__(k, copy(val))
 
     @overload
     def __getitem__(self, key: K) -> V:
         ...
 
     @overload
-    def __getitem__(self, key: list[K]) -> UtilDict[K, V]:
+    def __getitem__(self, key: List[K]) -> UtilDict[K, V]:
         ...
 
     def __getitem__(self, key):
         if not isinstance(key, list):
             return super().__getitem__(key)
 
         new = type(self).__new__(type(self))
@@ -356,37 +369,39 @@
             # When it's an iterable with valid keys but no values,
             # Set each key to None, but don't override where self already contains
             # a value for the key
             return {x: self.get(x) for x in arg}
         except Exception:
             pass
 
-        # Ah, so we've got values that aren't valid keys. Use them as values instead lmao
-        return {i: self.get(v) for i, v in enumerate(arg)}
+        raise ValueError(f"Could not convert arg to dict: {arg}")
 
     def render(self, **kwargs) -> str:
         from dictkit.render import render
 
         return render(self, **kwargs)
 
     def json(self, indent: int = 2, **kwargs) -> str:
         import json
 
-        def fmt(dic) -> dict:
-            return {
-                k: v
-                if isinstance(v, (int, float, str, list, tuple))
-                else fmt(v)
-                if isinstance(v, dict)
-                else str(v)
-                for k, v in dic.items()
-            }
+        def format(obj: Any) -> Any:
 
-        dic = fmt(self)
-        return json.dumps(dic, indent=indent, **kwargs)
+            is_serializable_scalar = isinstance(obj, (int, float, str, bool)) or obj is None
+
+            if is_serializable_scalar:
+                return obj
+            if isinstance(obj, (list, tuple)):
+                return [format(item) for item in obj]
+            if isinstance(obj, abc.Mapping):
+                return {k: format(v) for k, v in obj.items()}
+
+            return str(obj)
+
+        formatted_obj = format(self)
+        return json.dumps(formatted_obj, indent=indent, **kwargs)
 
     def __repr__(self):
         return self.render()
 
 
 if __name__ == "__main__":
     from doctest import testmod
```

### Comparing `dictkit-0.1.4/.gitignore` & `dictkit-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `dictkit-0.1.4/README.md` & `dictkit-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `dictkit-0.1.4/pyproject.toml` & `dictkit-0.1.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dictkit"
-version = "0.1.4"
-python_requires = ">=3.10"
+version = "0.1.5"
+python_requires = ">=3.8"
 description = "Utility data structures with simple but powerful features."
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/ryayoung/dictkit"
```

### Comparing `dictkit-0.1.4/PKG-INFO` & `dictkit-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictkit
-Version: 0.1.4
+Version: 0.1.5
 Summary: Utility data structures with simple but powerful features.
 Author-email: Ryan Young <dev@ryayoung.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```


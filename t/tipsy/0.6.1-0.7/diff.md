# Comparing `tmp/tipsy-0.6.1-py3-none-any.whl.zip` & `tmp/tipsy-0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6626 bytes, number of entries: 13
--rw-r--r--  2.0 unx      152 b- defN 23-Mar-19 09:07 tipsy/__init__.py
--rw-r--r--  2.0 unx      160 b- defN 23-Mar-19 09:07 tipsy/_version.py
--rw-r--r--  2.0 unx      551 b- defN 23-Mar-19 09:07 tipsy/cached.py
--rw-rw-rw-  2.0 unx        0 b- defN 23-Mar-19 09:07 tipsy/py.typed
--rw-r--r--  2.0 unx      828 b- defN 23-Mar-19 09:07 tipsy/registry.py
--rw-r--r--  2.0 unx      925 b- defN 23-Mar-19 09:07 tipsy/registry_helpers.py
--rw-r--r--  2.0 unx     4648 b- defN 23-Mar-19 09:07 tipsy/tipsy.py
--rw-r--r--  2.0 unx      422 b- defN 23-Mar-19 09:07 tipsy/types.py
--rw-rw-rw-  2.0 unx     1072 b- defN 23-Mar-19 09:07 tipsy-0.6.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     2951 b- defN 23-Mar-19 09:07 tipsy-0.6.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-19 09:07 tipsy-0.6.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-Mar-19 09:07 tipsy-0.6.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      955 b- defN 23-Mar-19 09:07 tipsy-0.6.1.dist-info/RECORD
-13 files, 12762 bytes uncompressed, 5052 bytes compressed:  60.4%
+Zip file size: 6634 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      152 b- defN 23-May-29 08:20 tipsy/__init__.py
+-rw-r--r--  2.0 unx      155 b- defN 23-May-29 08:21 tipsy/_version.py
+-rw-r--r--  2.0 unx      551 b- defN 23-May-29 08:20 tipsy/cached.py
+-rw-rw-rw-  2.0 unx        0 b- defN 23-May-29 08:20 tipsy/py.typed
+-rw-r--r--  2.0 unx      828 b- defN 23-May-29 08:20 tipsy/registry.py
+-rw-r--r--  2.0 unx      925 b- defN 23-May-29 08:20 tipsy/registry_helpers.py
+-rw-r--r--  2.0 unx     4816 b- defN 23-May-29 08:20 tipsy/tipsy.py
+-rw-r--r--  2.0 unx      422 b- defN 23-May-29 08:20 tipsy/types.py
+-rw-rw-rw-  2.0 unx     1072 b- defN 23-May-29 08:21 tipsy-0.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2949 b- defN 23-May-29 08:21 tipsy-0.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 08:21 tipsy-0.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-29 08:21 tipsy-0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      945 b- defN 23-May-29 08:21 tipsy-0.7.dist-info/RECORD
+13 files, 12913 bytes uncompressed, 5080 bytes compressed:  60.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: tipsy/tipsy.py
 Comment: 
 
 Filename: tipsy/types.py
 Comment: 
 
-Filename: tipsy-0.6.1.dist-info/LICENSE
+Filename: tipsy-0.7.dist-info/LICENSE
 Comment: 
 
-Filename: tipsy-0.6.1.dist-info/METADATA
+Filename: tipsy-0.7.dist-info/METADATA
 Comment: 
 
-Filename: tipsy-0.6.1.dist-info/WHEEL
+Filename: tipsy-0.7.dist-info/WHEEL
 Comment: 
 
-Filename: tipsy-0.6.1.dist-info/top_level.txt
+Filename: tipsy-0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: tipsy-0.6.1.dist-info/RECORD
+Filename: tipsy-0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## tipsy/_version.py

```diff
@@ -1,4 +1,4 @@
 # file generated by setuptools_scm
 # don't change, don't track in version control
-__version__ = version = '0.6.1'
-__version_tuple__ = version_tuple = (0, 6, 1)
+__version__ = version = '0.7'
+__version_tuple__ = version_tuple = (0, 7)
```

## tipsy/tipsy.py

```diff
@@ -1,9 +1,10 @@
 import inspect
 from collections.abc import Callable, Iterable, Mapping, MutableMapping, MutableSequence, MutableSet, Sequence, Set
+from enum import Enum
 from types import UnionType
 from typing import Any, Literal, TypeGuard, TypeVar, get_args, get_origin, is_typeddict
 
 from .cached import cached
 from .registry import user_generic, user_types
 from .types import TypeGuardFnc
 
@@ -128,13 +129,19 @@
             return False if strict else gg(data)
 
     elif t is Any:
 
         def inner(data: Any) -> TypeGuard[T]:
             return not (strict and invariant)
 
+    elif issubclass(t, Enum):
+        vgs3 = [x.value for x in t]
+
+        def inner(data: Any) -> TypeGuard[T]:
+            return data in vgs3
+
     else:
 
         def inner(data: Any) -> TypeGuard[T]:
             return type(data) is t if (strict and invariant) else isinstance(data, t)
 
     return inner
```

## Comparing `tipsy-0.6.1.dist-info/LICENSE` & `tipsy-0.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `tipsy-0.6.1.dist-info/METADATA` & `tipsy-0.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tipsy
-Version: 0.6.1
+Version: 0.7
 Summary: tiny type narrowing library
 Home-page: https://gitlab.com/martizih/tipsy.git
 Author: Martin Zihlmann
 Author-email: martizih@outlook.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
```

## Comparing `tipsy-0.6.1.dist-info/RECORD` & `tipsy-0.7.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 tipsy/__init__.py,sha256=wCjMXrsyJGnWH6o0PHkS9YGPgC9_SzrbCORaI45YTrI,152
-tipsy/_version.py,sha256=a0yJhWk72IWejRWIifC48k_2JA1SnCm-v-dQs-bk4io,160
+tipsy/_version.py,sha256=hyOraYjeRQdEzXHbUXVuE__DkQz8jzPN8xnb0NzCfZ4,155
 tipsy/cached.py,sha256=3OsEH9a9HpmUw3pSTNWhWK0T0yD8UvDxe7QoSa-4SWA,551
 tipsy/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tipsy/registry.py,sha256=YR6UH8tPnVyY7ThM6qG0AVkegnQxrONerBoz2iKAhlo,828
 tipsy/registry_helpers.py,sha256=OUGkvNcqSuCHGaq9MBQFFtrh2EHfVH0jq9iYlBCmCdg,925
-tipsy/tipsy.py,sha256=CbWovpP_sx6GIO6MYI8EhU1J7xyr0L_0NgkEGU4Cayg,4648
+tipsy/tipsy.py,sha256=2RlsTViZcSRLt2V7aDO6vZG9JmXeioYnkPeFALPocGE,4816
 tipsy/types.py,sha256=LFn6-swX5Grx4eriEswWDkoTGmXx0uAOto7z2euuqO4,422
-tipsy-0.6.1.dist-info/LICENSE,sha256=QHlt5TT5ZTypwtlvPjJJ4NFhuZ3h94uvUOwxI7QXlng,1072
-tipsy-0.6.1.dist-info/METADATA,sha256=6cxfqXyM13Jc81TeOe4Kci3c0ap2Tueam0Fk7-7LWKA,2951
-tipsy-0.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-tipsy-0.6.1.dist-info/top_level.txt,sha256=CvYzmTV7RUUbd36nqJm6gRAWaloOyi0Xx6v7hFSjZ3o,6
-tipsy-0.6.1.dist-info/RECORD,,
+tipsy-0.7.dist-info/LICENSE,sha256=QHlt5TT5ZTypwtlvPjJJ4NFhuZ3h94uvUOwxI7QXlng,1072
+tipsy-0.7.dist-info/METADATA,sha256=vvBrDXrXYoUjA4lZN3J7TM4mcVsMsRr_fh1yRSsbj90,2949
+tipsy-0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+tipsy-0.7.dist-info/top_level.txt,sha256=CvYzmTV7RUUbd36nqJm6gRAWaloOyi0Xx6v7hFSjZ3o,6
+tipsy-0.7.dist-info/RECORD,,
```


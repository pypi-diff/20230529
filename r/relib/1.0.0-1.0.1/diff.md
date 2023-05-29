# Comparing `tmp/relib-1.0.0-py3-none-any.whl.zip` & `tmp/relib-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8200 bytes, number of entries: 10
--rw-r--r--  2.0 unx      409 b- defN 23-May-07 12:15 relib/__init__.py
+Zip file size: 8217 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      421 b- defN 23-May-29 11:47 relib/__init__.py
 -rw-r--r--  2.0 unx     8943 b- defN 23-Jan-21 17:58 relib/hashing.py
 -rw-r--r--  2.0 unx      555 b- defN 23-Jan-21 18:12 relib/measure_duration.py
 -rw-r--r--  2.0 unx     1905 b- defN 23-Jan-21 17:58 relib/raypipe.py
--rw-r--r--  2.0 unx     3963 b- defN 23-May-07 12:20 relib/utils.py
--rw-r--r--  2.0 unx     1054 b- defN 23-May-07 12:20 relib-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      304 b- defN 23-May-07 12:20 relib-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-07 12:20 relib-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-07 12:20 relib-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      749 b- defN 23-May-07 12:20 relib-1.0.0.dist-info/RECORD
-10 files, 17980 bytes uncompressed, 6936 bytes compressed:  61.4%
+-rw-r--r--  2.0 unx     4100 b- defN 23-May-29 11:51 relib/utils.py
+-rw-r--r--  2.0 unx     1054 b- defN 23-May-29 16:09 relib-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      260 b- defN 23-May-29 16:09 relib-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 16:09 relib-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-29 16:09 relib-1.0.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      749 b- defN 23-May-29 16:09 relib-1.0.1.dist-info/RECORD
+10 files, 18085 bytes uncompressed, 6953 bytes compressed:  61.6%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: relib/raypipe.py
 Comment: 
 
 Filename: relib/utils.py
 Comment: 
 
-Filename: relib-1.0.0.dist-info/LICENSE.txt
+Filename: relib-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: relib-1.0.0.dist-info/METADATA
+Filename: relib-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: relib-1.0.0.dist-info/WHEEL
+Filename: relib-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: relib-1.0.0.dist-info/top_level.txt
+Filename: relib-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: relib-1.0.0.dist-info/RECORD
+Filename: relib-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## relib/__init__.py

```diff
@@ -9,14 +9,15 @@
   intersect,
   ensure_tuple,
   omit,
   dict_by,
   tuple_by,
   flatten,
   transpose,
+  map_dict,
   deepen_dict,
   group,
   sized_partitions,
   num_partitions,
   StrFilter,
   str_filterer,
 )
```

## relib/utils.py

```diff
@@ -1,12 +1,13 @@
 from typing import TypeVar, Union, Iterable, Callable
 import re
 
 T = TypeVar('T')
 U = TypeVar('U')
+K = TypeVar('K')
 
 def list_split(l: list[T], sep: T) -> list[list[T]]:
   l = [sep, *l, sep]
   split_at = [i for i, x in enumerate(l) if x is sep]
   ranges = list(zip(split_at[0:-1], split_at[1:]))
   return [
     l[start + 1:end]
@@ -83,14 +84,17 @@
 
 def transpose(tuples, default_num_returns=0):
   result = tuple(zip(*tuples))
   if not result:
     return ([],) * default_num_returns
   return tuple(map(list, result))
 
+def map_dict(fn: Callable[[T], U], d: dict[K, T]) -> dict[K, U]:
+  return {key: fn(value) for key, value in d.items()}
+
 def deepen_dict(d):
   result = {}
   for (*tail, head), value in d.items():
     curr = result
     for key in tail:
       if key not in curr:
         curr[key] = {}
```

## Comparing `relib-1.0.0.dist-info/LICENSE.txt` & `relib-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*


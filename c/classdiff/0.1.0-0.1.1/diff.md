# Comparing `tmp/classdiff-0.1.0.tar.gz` & `tmp/classdiff-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classdiff-0.1.0.tar", max compression
+gzip compressed data, was "classdiff-0.1.1.tar", max compression
```

## Comparing `classdiff-0.1.0.tar` & `classdiff-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1386 2023-05-09 14:50:06.267093 classdiff-0.1.0/README.md
--rw-r--r--   0        0        0       59 2023-05-09 13:58:40.964963 classdiff-0.1.0/classdiff/__init__.py
--rw-r--r--   0        0        0     6614 2023-05-22 07:08:23.115256 classdiff-0.1.0/classdiff/classdiff.py
--rw-r--r--   0        0        0     2256 2023-05-22 07:10:57.913763 classdiff-0.1.0/classdiff/examples/classdiff.py
--rw-r--r--   0        0        0      996 2023-05-09 13:58:40.976016 classdiff-0.1.0/classdiff/json.py
--rw-r--r--   0        0        0      638 2023-05-22 07:09:42.086138 classdiff-0.1.0/classdiff/utils.py
--rw-r--r--   0        0        0     1510 2023-05-24 13:26:06.932059 classdiff-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 classdiff-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1386 2023-05-09 14:50:06.267093 classdiff-0.1.1/README.md
+-rw-r--r--   0        0        0       59 2023-05-09 13:58:40.964963 classdiff-0.1.1/classdiff/__init__.py
+-rw-r--r--   0        0        0     7859 2023-05-29 11:55:55.933166 classdiff-0.1.1/classdiff/classdiff.py
+-rw-r--r--   0        0        0     2706 2023-05-29 11:53:42.400335 classdiff-0.1.1/classdiff/examples/classdiff.py
+-rw-r--r--   0        0        0      996 2023-05-09 13:58:40.976016 classdiff-0.1.1/classdiff/json.py
+-rw-r--r--   0        0        0      638 2023-05-22 07:09:42.086138 classdiff-0.1.1/classdiff/utils.py
+-rw-r--r--   0        0        0     1510 2023-05-29 12:05:06.670311 classdiff-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1861 1970-01-01 00:00:00.000000 classdiff-0.1.1/PKG-INFO
```

### Comparing `classdiff-0.1.0/README.md` & `classdiff-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `classdiff-0.1.0/classdiff/examples/classdiff.py` & `classdiff-0.1.1/classdiff/examples/classdiff.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,14 +19,37 @@
 
 
 def main():
     changed_keys()
     missing_keys()
     with_dict()
     with_dataclasses()
+    enum()
+
+
+def enum():
+    from enum import Enum
+
+    class YesOrNo(Enum):
+        YES = "y"
+        NO = "n"
+
+    @dataclass
+    class A:
+        a: str
+        v: YesOrNo
+
+    a1 = A(a="a1", v=YesOrNo.YES)
+    a2 = A(a="a2", v=YesOrNo.NO)
+
+    for fn in [classdiff.enum_name, classdiff.enum_value, classdiff.enum_full]:
+        for l in classdiff.diff(a1, a2, enum_formatter=fn):
+            print(l)
+
+        print("-" * 40)
 
 
 def changed_keys():
     @dataclass
     class A:
         a: str
 
@@ -106,7 +129,8 @@
     print("")
 
     print("> diff(None, resource_in_db)")
     print("-" * 40)
     removed = classdiff.diff(None, exists_in_db)
     for x in removed:
         print(x)
+    print("-" * 40)
```

### Comparing `classdiff-0.1.0/classdiff/json.py` & `classdiff-0.1.1/classdiff/json.py`

 * *Files identical despite different names*

### Comparing `classdiff-0.1.0/classdiff/utils.py` & `classdiff-0.1.1/classdiff/utils.py`

 * *Files identical despite different names*

### Comparing `classdiff-0.1.0/pyproject.toml` & `classdiff-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "classdiff"
-version = "0.1.0"
+version = "0.1.1"
 description = "Utility to diff classes"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "classdiff"}]
 
 [tool.poetry.dependencies]
```

### Comparing `classdiff-0.1.0/PKG-INFO` & `classdiff-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classdiff
-Version: 0.1.0
+Version: 0.1.1
 Summary: Utility to diff classes
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```


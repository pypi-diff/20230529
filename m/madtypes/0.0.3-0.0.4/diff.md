# Comparing `tmp/madtypes-0.0.3.tar.gz` & `tmp/madtypes-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madtypes-0.0.3.tar", last modified: Sun May 28 09:22:18 2023, max compression
+gzip compressed data, was "madtypes-0.0.4.tar", last modified: Mon May 29 17:35:57 2023, max compression
```

## Comparing `madtypes-0.0.3.tar` & `madtypes-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:22:18.951303 madtypes-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-28 09:22:18.951303 madtypes-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2526 2023-05-28 09:22:08.000000 madtypes-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:22:18.951303 madtypes-0.0.3/madtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-05-28 09:22:08.000000 madtypes-0.0.3/madtypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:22:18.951303 madtypes-0.0.3/madtypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-05-28 09:22:18.000000 madtypes-0.0.3/madtypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-28 09:22:18.000000 madtypes-0.0.3/madtypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 09:22:18.000000 madtypes-0.0.3/madtypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-28 09:22:18.000000 madtypes-0.0.3/madtypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 09:22:18.951303 madtypes-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-28 09:22:08.000000 madtypes-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:22:18.951303 madtypes-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-05-28 09:22:08.000000 madtypes-0.0.3/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:35:57.279113 madtypes-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-29 17:35:57.279113 madtypes-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-29 17:35:43.000000 madtypes-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:35:57.279113 madtypes-0.0.4/madtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5102 2023-05-29 17:35:43.000000 madtypes-0.0.4/madtypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:35:57.279113 madtypes-0.0.4/madtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-29 17:35:57.000000 madtypes-0.0.4/madtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-29 17:35:57.000000 madtypes-0.0.4/madtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:35:57.000000 madtypes-0.0.4/madtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 17:35:57.000000 madtypes-0.0.4/madtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:35:57.279113 madtypes-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-29 17:35:43.000000 madtypes-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:35:57.279113 madtypes-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    11064 2023-05-29 17:35:43.000000 madtypes-0.0.4/tests/test_schema.py
```

### Comparing `madtypes-0.0.3/PKG-INFO` & `madtypes-0.0.4/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: madtypes
-Version: 0.0.3
-Summary: Python typing that raise TypeError at runtime
-Home-page: https://github.com/6r17/madtypes
-Author: 6r17
-Author-email: patrick.borowy@proton.me
-Keywords: typing,json,json-schema
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-
 # madtypes
 - 💢 Python class typing that raise TypeError at runtime
 - 📖 Render to dict or json
 - 🌐 [Json-Schema](https://json-schema.org/)
 
 ### Example
 
@@ -82,14 +67,55 @@
             },
         }
     },
     "required": ["items"]
 }
 ```
 
+### 🔥 Annotation attributes
+It is possible to use the `Annotation` metaclass to add type-check to a class definition.
+
+```python
+class SomeStringAttribute(str, metaclass=Annotation):
+   pass
+
+SomeDescriptedAttribute(2) # raise type error
+```
+
+It is possible to use this to further describe a field.
+
+```python
+class SomeDescriptedAttribute(str, metaclass=Annotation):
+    annotation = str
+    description = "Some description"
+```
+
+Now when we use `schema` on `SomeDescription` to generate the json-schema, it will include the description attribute
+
+```python
+class DescriptedString(str, metaclass=Annotation):
+    description = "Some description"
+    annotation = str
+
+class DescriptedItem(Schema):
+    descripted: DescriptedString
+
+assert schema(DescriptedItem) == {
+    "type": "object",
+    "properties": {
+        "descripted": {
+            "type": "string",
+            "description": "Some description",
+        },
+    },
+    "required": ["descripted"],
+}
+
+```
+
 
 [![Test](https://github.com/6r17/madtypes/actions/workflows/test.yaml/badge.svg)](./tests/test_schema.py)
 [![pypi](https://img.shields.io/pypi/v/madtypes)](https://pypi.org/project/madtypes/)
 ![python: >3.9](https://img.shields.io/badge/python-%3E3.9-informational)
 ### Installation
 
 ```bash
```

### Comparing `madtypes-0.0.3/madtypes/__init__.py` & `madtypes-0.0.4/madtypes/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,17 +6,54 @@
     int: "integer",
     list: "array",
     float: "number",
     tuple: "array",
 }
 
 
-class Annotation:
-    annotation: Union[Type["Type"], Type["Annotation"], Type["Schema"]]
-    description: str
+def is_value_compatible_with_annotation(value, annotation):
+    origin = get_origin(annotation)
+    args = get_args(annotation)
+
+    if origin is None:
+        # Non-generic type
+        return isinstance(value, annotation)
+    elif origin is list:
+        # List annotation
+        if isinstance(value, list):
+            if args:
+                # Parametrized list annotation
+                inner_annotation = args[0]
+                return all(
+                    is_value_compatible_with_annotation(item, inner_annotation)
+                    for item in value
+                )
+
+
+class Annotation(type):
+    def __new__(cls, name, bases, attrs):
+        # Retrieve the annotation from the class attributes
+        annotation = attrs.get("annotation")
+
+        # Override the __new__ method of the list class
+        def new_method(cls, *values, **kwargs):
+            # Check the type of each value before initializing the list
+            for value in values:
+                if not is_value_compatible_with_annotation(value, annotation):
+                    raise TypeError(
+                        f"All values must be compatible with the annotation '{annotation}'"
+                    )
+
+            # Create the list instance and initialize it with the values
+            instance = super(cls, cls).__new__(cls, *values, **kwargs)
+            return instance
+
+        # Assign the overridden __new__ method to the class
+        attrs["__new__"] = new_method
+        return super().__new__(cls, name, bases, attrs)
 
 
 def is_optional_type(annotation):
     return getattr(annotation, "__origin__", None) is Union and type(
         None
     ) in getattr(annotation, "__args__", ())
 
@@ -48,22 +85,15 @@
         if name in self:
             return self[name]
         # I don't know how to trigger the next line, it's more of an `in-case'
         return super().__getattribute__(name)  # pragma: no cover
 
     def __setattr__(self, name, value):
         annotation = self.__annotations__[name]
-        annotation = (
-            annotation.annotation
-            if isinstance(
-                annotation,
-                Annotation,
-            )
-            else annotation
-        )
+
         if not isinstance(value, annotation):
             raise TypeError(f"{value} is not an instance of {annotation}")
         self[name] = value
 
     @classmethod
     def required_fields(cls) -> list[str]:
         return [
@@ -107,21 +137,17 @@
                         for name, field in origin.get_fields()
                     },
                 }
             )
             required = origin.required_fields()
             if len(required) > 0:
                 result.update({"required": required})
-        if issubclass(origin, Annotation):
+        if getattr(origin, "annotation", False):
             extra = {
                 key: value
                 for key, value in origin.__dict__.items()
                 if not callable(value) and not key.startswith("__")
             }
-            try:
-                del extra["annotation"]
-            except KeyError:
-                pass
             return schema(origin.annotation, **extra)
     if is_optional_type(annotation):
         return schema(remove_optional(annotation))
     return result
```

### Comparing `madtypes-0.0.3/setup.py` & `madtypes-0.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="madtypes",
-    version="0.0.3",
+    version="0.0.4",
     author="6r17",
     author_email="patrick.borowy@proton.me",
     description="Python typing that raise TypeError at runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/6r17/madtypes",
     packages=find_packages(include=["madtypes"]),
```

### Comparing `madtypes-0.0.3/tests/test_schema.py` & `madtypes-0.0.4/tests/test_schema.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional
 from madtypes import schema, Schema, Annotation, Immutable
 import pytest
+import json
 
 
 class Gender(Schema):
     female: int
     male: int
 
 
@@ -62,41 +63,41 @@
     a = Item(name="bob", gender=Gender(male=20, female=30))
     a.gender = Gender(male=30, female=10)
     assert a.gender.male == 30
     with pytest.raises(TypeError):
         a.gender.male = "foo"
 
 
-def test_int():
+def test_int_schema():
     assert schema(int) == {"type": "integer"}
 
 
-def test_array():
+def test_array_schema():
     assert schema(list[int]) == {"type": "array", "items": {"type": "integer"}}
 
 
-def test_tuple():
+def test_tuple_schema():
     assert schema(tuple[int, int]) == {
         "type": "array",
         "items": [{"type": "integer"}, {"type": "integer"}],
     }
 
 
-def test_object():
+def test_object_schema():
     class Item(Schema):
         name: str
 
     assert schema(Item) == {
         "type": "object",
         "properties": {"name": {"type": "string"}},
         "required": ["name"],
     }
 
 
-def test_array_of_object():
+def test_array_of_object_schema():
     class Item(Schema):
         name: str
 
     class Basket(Schema):
         items: list[Item]
 
     schem = schema(Basket)
@@ -113,15 +114,15 @@
                 },
             }
         },
         "required": ["items"],
     }
 
 
-def test_tuple_of_object():
+def test_tuple_of_object_schema():
     class Item(Schema):
         name: str
 
     class Basket(Schema):
         some_items: tuple[Item, Item]
 
     schem = schema(Basket)
@@ -145,15 +146,15 @@
                 ],
             }
         },
         "required": ["some_items"],
     }
 
 
-def test_json_schema():
+def test_object_with_object_schema():
     print(schema(Item))
     assert schema(Item) == {
         "type": "object",
         "properties": {
             "name": {"type": "string"},
             "gender": {
                 "type": "object",
@@ -164,37 +165,14 @@
                 "required": ["female", "male"],
             },
         },
         "required": ["name", "gender"],
     }
 
 
-class DescriptedString(Annotation):
-    description = "Some description"
-    annotation = str
-
-
-class DescriptedItem(Schema):
-    descripted: DescriptedString
-
-
-def test_descripted_json_schema():
-    print(schema(DescriptedItem))
-    assert schema(DescriptedItem) == {
-        "type": "object",
-        "properties": {
-            "descripted": {
-                "type": "string",
-                "description": "Some description",
-            },
-        },
-        "required": ["descripted"],
-    }
-
-
 class PrimitiveArray(Schema):
     items: list[str]
 
 
 def test_annotation_array():
     assert schema(PrimitiveArray) == {
         "type": "object",
@@ -421,7 +399,79 @@
     schem = schema(SomeClassWithOptional)
     assert schem == {
         "type": "object",
         "properties": {
             "elements": {"type": "array", "items": {"type": "integer"}}
         },
     }
+
+
+def test_descripted_value_set():
+    class SomeDescriptedField(str, metaclass=Annotation):
+        description = "foo"
+        annotation = str
+
+    class SomeItem(Schema):
+        name: SomeDescriptedField
+
+    with pytest.raises(TypeError):
+        SomeDescriptedField(2)
+    a = SomeItem(name=SomeDescriptedField("foo"))
+    assert a.name == "foo"
+    a.name = SomeDescriptedField("bar")
+    assert a == {"name": "bar"}
+    assert json.dumps(a) == '{"name": "bar"}'
+    assert a.name.description == "foo"
+
+
+def test_descripted_list_value_set():
+    class SomeDescriptedListField(list, metaclass=Annotation):
+        description = "foo"
+        annotation = list[str]
+
+    class SomeListItem(Schema):
+        names: SomeDescriptedListField
+
+    values = SomeDescriptedListField(["1", "2", "3"])
+    print(values)
+    assert values == ["1", "2", "3"]
+    with pytest.raises(TypeError):
+        SomeListItem(names=SomeDescriptedListField([1]))
+    a = SomeListItem(names=SomeDescriptedListField(["1", "2", "3"]))
+    assert len(a.names) == 3
+    assert json.dumps(a) == '{"names": ["1", "2", "3"]}'
+    with pytest.raises(AttributeError):  # append does not exist
+        a.append("foo")
+
+
+def test_descripted_list_object_value_set():
+    class Foo(Schema):
+        name: str
+
+    class DescriptedFoo(Foo, metaclass=Annotation):
+        description = "description"
+        annotation = Foo
+
+    DescriptedFoo(name="foo")
+    with pytest.raises(TypeError):
+        DescriptedFoo(name=2)
+
+
+def test_descripted_json_schema():
+    class DescriptedString(str, metaclass=Annotation):
+        description = "Some description"
+        annotation = str
+
+    class DescriptedItem(Schema):
+        descripted: DescriptedString
+
+    print(schema(DescriptedItem))
+    assert schema(DescriptedItem) == {
+        "type": "object",
+        "properties": {
+            "descripted": {
+                "type": "string",
+                "description": "Some description",
+            },
+        },
+        "required": ["descripted"],
+    }
```


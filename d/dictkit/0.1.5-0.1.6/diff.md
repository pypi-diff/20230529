# Comparing `tmp/dictkit-0.1.5.tar.gz` & `tmp/dictkit-0.1.6.tar.gz`

## Comparing `dictkit-0.1.5.tar` & `dictkit-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dictkit-0.1.5/dictkit/__init__.py
--rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 dictkit-0.1.5/dictkit/categorize.py
--rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 dictkit-0.1.5/dictkit/render.py
--rw-r--r--   0        0        0    10712 2020-02-02 00:00:00.000000 dictkit-0.1.5/dictkit/utildict.py
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 dictkit-0.1.5/.gitignore
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 dictkit-0.1.5/README.md
--rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 dictkit-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 dictkit-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 dictkit-0.1.6/dictkit/__init__.py
+-rw-r--r--   0        0        0    11101 2020-02-02 00:00:00.000000 dictkit-0.1.6/dictkit/categorize.py
+-rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 dictkit-0.1.6/dictkit/render.py
+-rw-r--r--   0        0        0    10752 2020-02-02 00:00:00.000000 dictkit-0.1.6/dictkit/utildict.py
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 dictkit-0.1.6/.gitignore
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 dictkit-0.1.6/README.md
+-rw-r--r--   0        0        0     1364 2020-02-02 00:00:00.000000 dictkit-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3618 2020-02-02 00:00:00.000000 dictkit-0.1.6/PKG-INFO
```

### Comparing `dictkit-0.1.5/dictkit/categorize.py` & `dictkit-0.1.6/dictkit/categorize.py`

 * *Files identical despite different names*

### Comparing `dictkit-0.1.5/dictkit/render.py` & `dictkit-0.1.6/dictkit/render.py`

 * *Files identical despite different names*

### Comparing `dictkit-0.1.5/dictkit/utildict.py` & `dictkit-0.1.6/dictkit/utildict.py`

 * *Files 1% similar despite different names*

```diff
@@ -342,18 +342,18 @@
         return new
 
     def __copy__(self) -> UtilDict:
         return self.copy()
 
     def _iterable_to_dict(self, arg) -> dict:
 
-        if isinstance(arg, Mapping):
+        if isinstance(arg, abc.Mapping):
             return dict(arg)
 
-        if not isinstance(arg, Iterable):
+        if not isinstance(arg, abc.Iterable):
             # Let dict throw the error if not hashable
             return {arg: self.get(arg)}
 
         try:
             return dict(arg)
         except Exception:
             pass
@@ -381,15 +381,17 @@
         return render(self, **kwargs)
 
     def json(self, indent: int = 2, **kwargs) -> str:
         import json
 
         def format(obj: Any) -> Any:
 
-            is_serializable_scalar = isinstance(obj, (int, float, str, bool)) or obj is None
+            is_serializable_scalar = (
+                isinstance(obj, (int, float, str, bool)) or obj is None
+            )
 
             if is_serializable_scalar:
                 return obj
             if isinstance(obj, (list, tuple)):
                 return [format(item) for item in obj]
             if isinstance(obj, abc.Mapping):
                 return {k: format(v) for k, v in obj.items()}
```

### Comparing `dictkit-0.1.5/.gitignore` & `dictkit-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `dictkit-0.1.5/README.md` & `dictkit-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dictkit-0.1.5/pyproject.toml` & `dictkit-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dictkit"
-version = "0.1.5"
+version = "0.1.6"
 python_requires = ">=3.8"
 description = "Utility data structures with simple but powerful features."
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
```

### Comparing `dictkit-0.1.5/PKG-INFO` & `dictkit-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictkit
-Version: 0.1.5
+Version: 0.1.6
 Summary: Utility data structures with simple but powerful features.
 Author-email: Ryan Young <dev@ryayoung.com>
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.11
```


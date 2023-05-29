# Comparing `tmp/filesystem-dict-0.1.8.tar.gz` & `tmp/filesystem-dict-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "filesystem-dict-0.1.8.tar", last modified: Thu May 25 17:04:16 2023, max compression
+gzip compressed data, was "filesystem-dict-0.1.9.tar", last modified: Mon May 29 15:34:56 2023, max compression
```

## Comparing `filesystem-dict-0.1.8.tar` & `filesystem-dict-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/
--rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-23 14:03:54.000000 filesystem-dict-0.1.8/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      834 2023-05-23 14:03:54.000000 filesystem-dict-0.1.8/README.md
--rw-r--r--   0 user      (1000) user      (1000)      476 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)       69 2023-05-23 14:03:54.000000 filesystem-dict-0.1.8/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/src/filesystem_dict.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-25 17:04:16.000000 filesystem-dict-0.1.8/src/filesystem_dict.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      276 2023-05-25 17:04:16.000000 filesystem-dict-0.1.8/src/filesystem_dict.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-25 17:04:16.000000 filesystem-dict-0.1.8/src/filesystem_dict.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-25 17:04:16.000000 filesystem-dict-0.1.8/src/filesystem_dict.egg-info/top_level.txt
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-25 17:04:16.935187 filesystem-dict-0.1.8/src/fsdict/
--rw-r--r--   0 user      (1000) user      (1000)       27 2023-05-23 14:03:54.000000 filesystem-dict-0.1.8/src/fsdict/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     5850 2023-05-23 14:03:54.000000 filesystem-dict-0.1.8/src/fsdict/fsdict.py
--rw-r--r--   0 user      (1000) user      (1000)     1116 2023-05-25 17:01:14.000000 filesystem-dict-0.1.8/src/fsdict/utils.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 15:34:56.384392 filesystem-dict-0.1.9/
+-rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-15 20:22:54.000000 filesystem-dict-0.1.9/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-29 15:34:56.384392 filesystem-dict-0.1.9/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      834 2023-05-17 08:45:31.000000 filesystem-dict-0.1.9/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      476 2023-05-29 15:34:56.384392 filesystem-dict-0.1.9/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)       69 2023-05-15 20:55:49.000000 filesystem-dict-0.1.9/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 15:34:56.381058 filesystem-dict-0.1.9/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 15:34:56.384392 filesystem-dict-0.1.9/src/filesystem_dict.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)     1149 2023-05-29 15:34:56.000000 filesystem-dict-0.1.9/src/filesystem_dict.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      276 2023-05-29 15:34:56.000000 filesystem-dict-0.1.9/src/filesystem_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-29 15:34:56.000000 filesystem-dict-0.1.9/src/filesystem_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-29 15:34:56.000000 filesystem-dict-0.1.9/src/filesystem_dict.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-29 15:34:56.384392 filesystem-dict-0.1.9/src/fsdict/
+-rw-r--r--   0 user      (1000) user      (1000)       27 2023-05-29 15:33:37.000000 filesystem-dict-0.1.9/src/fsdict/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     5870 2023-05-29 15:33:26.000000 filesystem-dict-0.1.9/src/fsdict/fsdict.py
+-rw-r--r--   0 user      (1000) user      (1000)     1116 2023-05-29 15:32:37.000000 filesystem-dict-0.1.9/src/fsdict/utils.py
```

### Comparing `filesystem-dict-0.1.8/LICENSE.txt` & `filesystem-dict-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `filesystem-dict-0.1.8/PKG-INFO` & `filesystem-dict-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesystem-dict
-Version: 0.1.8
+Version: 0.1.9
 Summary: Dictionary like access to the filesystem.
 Home-page: https://github.com/MNayer/fsdict
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: dictionary,filesystem
 Description-Content-Type: text/markdown
```

### Comparing `filesystem-dict-0.1.8/README.md` & `filesystem-dict-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `filesystem-dict-0.1.8/src/filesystem_dict.egg-info/PKG-INFO` & `filesystem-dict-0.1.9/src/filesystem_dict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: filesystem-dict
-Version: 0.1.8
+Version: 0.1.9
 Summary: Dictionary like access to the filesystem.
 Home-page: https://github.com/MNayer/fsdict
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: dictionary,filesystem
 Description-Content-Type: text/markdown
```

### Comparing `filesystem-dict-0.1.8/src/fsdict/fsdict.py` & `filesystem-dict-0.1.9/src/fsdict/fsdict.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,193 +1,205 @@
 import json
 import types
 from fsdict.utils import *
 from pathlib import Path
 
 
 class LazyValue:
-    def __init__(self, path):
+    def __init__(self, basepath, path):
+        self.basepath = basepath
+        if isinstance(basepath, str):
+            self.basepath = Path(basepath)
         self.path = path
 
     def __repr__(self):
-        return f"<LazyValue @ {self.path}>"
+        return f"<LazyValue {self.path} @ {self.basepath}>"
 
     def __str__(self):
         return repr(self)
 
     def read(self):
-        return maybe_deserialize(fread_bytes(self.path))
+        # TODO
+        raise NotImplementedError()
 
 
-class fsdict:
-    def __init__(self, path=None, overwrite=True, create_fsdict_on_keyerror=False):
-        self.path = Path(path) if path else None
+class genfsdict:
+    def __init__(
+        self, basepath=None, path="", overwrite=True, create_fsdict_on_keyerror=False
+    ):
+        self.basepath = Path(basepath) if basepath else None
+        self.path = Path(path)
         self.overwrite = overwrite
         self.create_fsdict_on_keyerror = create_fsdict_on_keyerror
-        if self.path != None:
-            if not self.path.exists():
-                self.path.mkdir()
-            assert self.path.is_dir()
+        if self.basepath != None and not self._fsdict_exists():
+            self._create_empty_fsdict()
 
-    def __len__(self):
-        return len(self.keys())
+    def _fsdict_exists(self):
+        raise NotImplementedError()
 
-    def __iter__(self):
-        yield from self.keys()
+    def _del_item(self, key):
+        raise NotImplementedError()
 
-    def __contains__(self, key):
-        assert not self.dangling()
-        assert isinstance(key, str)
-        key_path = self.__get_path(key)
-        return key_path.exists()
+    def _is_fsdict(self, key):
+        raise NotImplementedError()
 
-    def __getitem__(self, selector):
-        assert not self.dangling()
-        if isinstance(selector, str):
-            return self.__get_item(selector)
-        elif isinstance(selector, types.FunctionType):
-            return self.__get_items(selector)
-
-    def __setitem__(self, selector, value):
-        assert not self.dangling()
-        if isinstance(selector, str):
-            self.__set_item(selector, value)
-        elif isinstance(selector, types.FunctionType):
-            self.__set_items(selector, value)
-
-    def __delitem__(self, selector):
-        assert not self.dangling()
-        if isinstance(selector, str):
-            self.__del_item(selector)
-        elif isinstance(selector, types.FunctionType):
-            self.__del_items(selector)
+    def _read_keyvalue(self, key):
+        raise NotImplementedError()
 
-    def __repr__(self):
-        return json.dumps(self.todict(), indent=2, default=repr)
+    def _write_keyvalue(self, key, value):
+        raise NotImplementedError()
+
+    def _create_empty_fsdict(self, key=""):
+        raise NotImplementedError()
+
+    def _link_fsdict(self, key, other):
+        raise NotImplementedError()
+
+    def _has_key(self, key):
+        return key in self.keys()
 
-    def __get_item(self, key):
+    def _get_item(self, key):
         assert not self.dangling()
-        assert isinstance(key, str)
-        key_path = self.__get_path(key)
-        if not key_path.exists():
+        assert self._valid_keytype(key)
+        if not self._has_key(key):
             if self.create_fsdict_on_keyerror:
-                return fsdict(
-                    key_path,
+                return self.__class__(
+                    self.basepath,
+                    self.path / key,
                     overwrite=self.overwrite,
                     create_fsdict_on_keyerror=self.create_fsdict_on_keyerror,
                 )
             else:
-                raise KeyError(key_path.name)
-        if self.__is_fsdict(key):
-            return fsdict(
-                key_path,
+                raise KeyError(key)
+        if self._is_fsdict(key):
+            return self.__class__(
+                self.basepath,
+                self.path / key,
                 overwrite=self.overwrite,
                 create_fsdict_on_keyerror=self.create_fsdict_on_keyerror,
             )
-        else:
-            return maybe_deserialize(fread_bytes(key_path))
-
-    def __get_items(self, selector):
-        assert not self.dangling()
-        assert isinstance(selector, types.FunctionType)
-        keys = filter(selector, self.keys())
-        yield from (self[key] for key in keys)
+        return self._read_keyvalue(key)
 
-    def __set_item(self, key, value):
-        key_path = self.__get_path(key)
-        if key_path.exists():
+    def _set_item(self, key, value):
+        if self._has_key(key):
             if not self.overwrite:
                 return
             del self[key]
-        if isinstance(value, fsdict):
+        if isinstance(value, self.__class__):
             if value.dangling():
-                key_path.mkdir()
-            else:
-                value.copy(key_path)
-        else:
-            fwrite_bytes(key_path, maybe_serialize(value))
+                self._create_empty_fsdict(key)
+                return
+            self._link_fsdict(key, value)
+            return
+        self._write_keyvalue(key, value)
+
+    def _valid_keytype(self, key):
+        return isinstance(key, str)
+
+    def __len__(self):
+        return len(self.keys())
+
+    def __iter__(self):
+        yield from self.keys()
 
-    def __set_items(self, selector, value):
+    def __contains__(self, key):
         assert not self.dangling()
-        assert isinstance(selector, types.FunctionType)
-        keys = filter(selector, self.keys())
-        for key in keys:
-            self[key] = value
+        assert self._valid_keytype(key)
+        return self._has_key(key)
 
-    def __del_item(self, key):
+    def __getitem__(self, key):
         assert not self.dangling()
-        key_path = self.__get_path(key)
-        if key_path.exists():
-            rm(key_path)
+        return self._get_item(key)
 
-    def __del_items(self, selector):
+    def __setitem__(self, key, value):
         assert not self.dangling()
-        assert isinstance(selector, types.FunctionType)
-        keys = filter(selector, self.keys())
-        for key in keys:
-            del self[key]
+        self._set_item(key, value)
 
-    def dangling(self):
-        return self.path == None
+    def __delitem__(self, key):
+        assert not self.dangling()
+        if not self._has_key(key):
+            raise KeyError(key)
+        self._del_item(key)
 
-    def setpath(self, path):
-        self.path = Path(path)
+    def __repr__(self):
+        return json.dumps(self.todict(), indent=2, default=repr)
+
+    def keys(self):
+        raise NotImplementedError()
 
     def todict(self, lazy=True):
         assert not self.dangling()
         dictionary = dict()
         for key in self.keys():
-            key_path = self.__get_path(key)
-            if self.__is_fsdict(key):
-                dictionary[key] = fsdict(
-                    key_path,
+            if self._is_fsdict(key):
+                dictionary[key] = self.__class__(
+                    self.basepath,
+                    self.path / key,
                     overwrite=self.overwrite,
                     create_fsdict_on_keyerror=self.create_fsdict_on_keyerror,
                 ).todict(lazy)
                 continue
             if lazy:
-                dictionary[key] = LazyValue(key_path)
+                dictionary[key] = LazyValue(self.basepath, self.path / key)
             else:
                 dictionary[key] = self[key]
         return dictionary
 
-    def keys(self, lazy=False):
-        assert not self.dangling()
-        keys = (keypath.name for keypath in self.__get_paths())
-        if lazy:
-            return keys
-        else:
-            return list(keys)
-
     def values(self, lazy=True):
         assert not self.dangling()
         values = (self[key] for key in self.keys())
         if lazy:
             return values
         else:
             return list(values)
 
     def items(self):
         assert not self.dangling()
         for key in self.keys():
             yield key, self[key]
 
-    def copy(self, dst_path):
-        assert not self.dangling()
-        symlink(self.path, dst_path)
+    def dangling(self):
+        return self.basepath == None
 
-    def __get_path(self, key):
-        assert not self.dangling()
-        if isinstance(key, str):
-            return self.path / key
-        raise TypeError(f"Value of key '{key}' must be of type 'str' not '{type(key)}'")
+    def setpath(self, basepath):
+        self.basepath = Path(basepath)
 
-    def __get_paths(self):
-        assert not self.dangling()
-        return self.path.glob("*")
 
-    def __is_fsdict(self, key):
-        assert not self.dangling()
-        if not key in self:
-            raise KeyError(key)
-        key_path = self.path / key
+class fsdict(genfsdict):
+    def _fsdict_exists(self):
+        path = self.basepath / self.path
+        return path.exists()
+
+    def _del_item(self, key):
+        key_path = self.basepath / self.path / key
+        rm(key_path)
+
+    def _is_fsdict(self, key):
+        key_path = self.basepath / self.path / key
         return key_path.is_dir()
+
+    def _read_keyvalue(self, key):
+        key_path = self.basepath / self.path / key
+        return maybe_deserialize(fread_bytes(key_path))
+
+    def _write_keyvalue(self, key, value):
+        key_path = self.basepath / self.path / key
+        fwrite_bytes(key_path, maybe_serialize(value))
+
+    def _create_empty_fsdict(self, key=""):
+        key_path = self.basepath / self.path / key
+        key_path.mkdir()
+
+    def _link_fsdict(self, key, other):
+        src_path = other.basepath
+        dst_path = self.basepath / self.path / key
+        symlink(src_path, dst_path)
+
+    def _has_key(self, key):
+        key_path = self.basepath / self.path / key
+        return key_path.exists()
+
+    def keys(self):
+        assert not self.dangling()
+        path = self.basepath / self.path
+        keys = [keypath.name for keypath in path.glob("*")]
+        return keys
```

### Comparing `filesystem-dict-0.1.8/src/fsdict/utils.py` & `filesystem-dict-0.1.9/src/fsdict/utils.py`

 * *Files identical despite different names*


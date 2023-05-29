# Comparing `tmp/angola-0.10.9.tar.gz` & `tmp/angola-0.11.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "angola-0.10.9.tar", last modified: Tue Feb 21 06:27:33 2023, max compression
+gzip compressed data, was "angola-0.11.0.tar", last modified: Mon May 29 09:34:25 2023, max compression
```

## Comparing `angola-0.10.9.tar` & `angola-0.11.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 06:27:33.841214 angola-0.10.9/
--rw-r--r--   0 mardix     (501) staff       (20)     1084 2022-05-25 02:30:17.000000 angola-0.10.9/LICENSE
--rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.10.9/MANIFEST.in
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-02-21 06:27:33.841283 angola-0.10.9/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.10.9/README.md
--rw-r--r--   0 mardix     (501) staff       (20)       79 2023-02-21 06:27:33.841517 angola-0.10.9/setup.cfg
--rw-r--r--   0 mardix     (501) staff       (20)      799 2023-02-21 06:26:54.000000 angola-0.10.9/setup.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 06:27:33.835954 angola-0.10.9/src/
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 06:27:33.838616 angola-0.10.9/src/angola/
--rw-r--r--   0 mardix     (501) staff       (20)      294 2023-02-05 09:35:54.000000 angola-0.10.9/src/angola/__init__.py
--rw-r--r--   0 mardix     (501) staff       (20)    45123 2023-02-21 06:18:00.000000 angola-0.10.9/src/angola/database.py
--rw-r--r--   0 mardix     (501) staff       (20)    13878 2023-01-21 20:17:47.000000 angola-0.10.9/src/angola/dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.10.9/src/angola/dict_query.py
--rw-r--r--   0 mardix     (501) staff       (20)    16435 2023-02-21 06:17:43.000000 angola-0.10.9/src/angola/lib.py
--rw-r--r--   0 mardix     (501) staff       (20)    16563 2023-02-21 03:11:29.000000 angola-0.10.9/src/angola/lib_xql.py
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 06:27:33.839678 angola-0.10.9/src/angola.egg-info/
--rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-02-21 06:27:33.000000 angola-0.10.9/src/angola.egg-info/PKG-INFO
--rw-r--r--   0 mardix     (501) staff       (20)      464 2023-02-21 06:27:33.000000 angola-0.10.9/src/angola.egg-info/SOURCES.txt
--rw-r--r--   0 mardix     (501) staff       (20)        1 2023-02-21 06:27:33.000000 angola-0.10.9/src/angola.egg-info/dependency_links.txt
--rw-r--r--   0 mardix     (501) staff       (20)       59 2023-02-21 06:27:33.000000 angola-0.10.9/src/angola.egg-info/requires.txt
--rw-r--r--   0 mardix     (501) staff       (20)        7 2023-02-21 06:27:33.000000 angola-0.10.9/src/angola.egg-info/top_level.txt
-drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-02-21 06:27:33.841113 angola-0.10.9/tests/
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.10.9/tests/test_cursor.py
--rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.10.9/tests/test_database.py
--rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.10.9/tests/test_dict_mutator.py
--rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.10.9/tests/test_lib.py
--rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.10.9/tests/test_query.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-29 09:34:25.240895 angola-0.11.0/
+-rw-r--r--   0 mardix     (501) staff       (20)     1084 2023-03-21 05:31:22.000000 angola-0.11.0/LICENSE
+-rw-r--r--   0 mardix     (501) staff       (20)       26 2022-11-28 18:23:44.000000 angola-0.11.0/MANIFEST.in
+-rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-05-29 09:34:25.240975 angola-0.11.0/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      877 2022-11-30 18:28:40.000000 angola-0.11.0/README.md
+-rw-r--r--   0 mardix     (501) staff       (20)       79 2023-05-29 09:34:25.241246 angola-0.11.0/setup.cfg
+-rw-r--r--   0 mardix     (501) staff       (20)      799 2023-05-29 09:33:29.000000 angola-0.11.0/setup.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-29 09:34:25.235483 angola-0.11.0/src/
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-29 09:34:25.238486 angola-0.11.0/src/angola/
+-rw-r--r--   0 mardix     (501) staff       (20)      314 2023-04-30 19:58:20.000000 angola-0.11.0/src/angola/__init__.py
+-rw-r--r--   0 mardix     (501) staff       (20)    48031 2023-05-08 02:57:37.000000 angola-0.11.0/src/angola/database.py
+-rw-r--r--   0 mardix     (501) staff       (20)    13959 2023-05-29 06:51:31.000000 angola-0.11.0/src/angola/dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)    18847 2023-02-21 03:11:29.000000 angola-0.11.0/src/angola/dict_query.py
+-rw-r--r--   0 mardix     (501) staff       (20)    16742 2023-03-08 03:08:31.000000 angola-0.11.0/src/angola/lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)    16737 2023-05-29 09:32:03.000000 angola-0.11.0/src/angola/lib_xql.py
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-29 09:34:25.239141 angola-0.11.0/src/angola.egg-info/
+-rw-r--r--   0 mardix     (501) staff       (20)     1257 2023-05-29 09:34:25.000000 angola-0.11.0/src/angola.egg-info/PKG-INFO
+-rw-r--r--   0 mardix     (501) staff       (20)      464 2023-05-29 09:34:25.000000 angola-0.11.0/src/angola.egg-info/SOURCES.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        1 2023-05-29 09:34:25.000000 angola-0.11.0/src/angola.egg-info/dependency_links.txt
+-rw-r--r--   0 mardix     (501) staff       (20)       59 2023-05-29 09:34:25.000000 angola-0.11.0/src/angola.egg-info/requires.txt
+-rw-r--r--   0 mardix     (501) staff       (20)        7 2023-05-29 09:34:25.000000 angola-0.11.0/src/angola.egg-info/top_level.txt
+drwxr-xr-x   0 mardix     (501) staff       (20)        0 2023-05-29 09:34:25.240779 angola-0.11.0/tests/
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:45.000000 angola-0.11.0/tests/test_cursor.py
+-rw-r--r--   0 mardix     (501) staff       (20)      716 2022-11-28 18:20:13.000000 angola-0.11.0/tests/test_database.py
+-rw-r--r--   0 mardix     (501) staff       (20)     1184 2022-11-28 18:20:13.000000 angola-0.11.0/tests/test_dict_mutator.py
+-rw-r--r--   0 mardix     (501) staff       (20)     3301 2022-06-29 07:01:37.000000 angola-0.11.0/tests/test_lib.py
+-rw-r--r--   0 mardix     (501) staff       (20)        0 2022-05-28 01:11:55.000000 angola-0.11.0/tests/test_query.py
```

### Comparing `angola-0.10.9/LICENSE` & `angola-0.11.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2022 - Forever - Mardix
+Copyright (c) 2023 - Forever - Mardix
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `angola-0.10.9/PKG-INFO` & `angola-0.11.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.10.9
+Version: 0.11.0
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.10.9/README.md` & `angola-0.11.0/README.md`

 * *Files identical despite different names*

### Comparing `angola-0.10.9/setup.py` & `angola-0.11.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 
 def long_description():
     with open('README.md', 'r') as file:
         return file.read()
 
-VERSION = "0.10.9"
+VERSION = "0.11.0"
 setuptools.setup(
     name='angola',
     version=VERSION,
     author='Mardix',
     author_email='mardix@blackdevhub.io',
     description='angola ',
     long_description=long_description(),
```

### Comparing `angola-0.10.9/src/angola/database.py` & `angola-0.11.0/src/angola/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 from . import lib, lib_xql, dict_mutator, dict_query
 
 
 DEFAULT_INDEXES = [
     {
         "type": "persistent",
         "fields": ["_created_at"],
-        "name": "idx_created_at__0"
+        "name": "idx00__created_at"
     },
     {
         "type": "persistent",
         "fields": ["_modified_at"],
-        "name": "idx_modified_at__0"
+        "name": "idx00__modified_at"
     },
     {
         "type": "ttl",
         "fields": ["__ttl"],
-        "name": "idx__ttl__0",
+        "name": "idx00__ttl",
         "expireAfter": 0
     }
 ]
 
 #------------------------------------------------------------------------------
 # Exception
 class AngolaError(Exception): pass
@@ -42,21 +42,23 @@
 class UndeletableError(AngolaError): pass
 class MissingCommitterCallbackError(AngolaError): pass
 class MissingItemKeyError(AngolaError): pass
 class InvalidItemPathError(AngolaError): pass 
 
 #------------------------------------------------------------------------------
 
-class CollectionItemClass(object):
+class CollectionActiveRecordMixin(object):
     """
-    CollectionItemClass
+    CollectionActiveRecordMixin
+
+    An abstraction class to use as an active record on the items
 
     Usage:
 
-      class User(CollectionItemClass):
+      class User(CollectionActiveRecordMixin):
         def full_name(self):
             return "%s %s" % (self.get("first_name), self.get("last_name"))
             
       coll = #db.select_collection(..., item_class=User)
 
       if item := coll.get(_key):
         print(item.full_name())
@@ -72,40 +74,54 @@
         i = copy.deepcopy(self)
         i._item = _item
         return i
 
     def __getattr__(self, __name: str, *a, **kw):
       return self._item.__getattribute__(__name, *a, **kw)
 
-class QueryResult(object):
+   
+#------------------------------------------------------------------------------
+
+class _QueryResultIterator(object):
+    results:list = []
+    pagination:dict = {}
+    cursor:list = []
+    count:int = 0
+    size:int = 0
+
     def __init__(self, cursor, pager, data_mapper=None):
         self.cursor = cursor
         stats = cursor.statistics()
         self.count = self.cursor.count() # current count
         self.size = stats["fullCount"] # total count
         self.pagination = lib.gen_pagination(
                                             size=self.size,
                                             count=self.count,
                                             page=pager[0],
                                             per_page=pager[1])
 
         def _default_data_mapper_cb(item): return item 
     
-        self._data_mapper = _default_data_mapper_cb if not data_mapper else data_mapper
+        _data_mapper = _default_data_mapper_cb if not data_mapper else data_mapper
+
+        self.results = [_data_mapper(item) for item in self.cursor]
 
     def __iter__(self):
-        for item in self.cursor:
-            yield self._data_mapper(item)
+        """
+        Iterate over the results
+        """
+        yield from self.results
 
     def __len__(self):
-        """Get the total count """
+        """
+        Get the total results 
+        """
         return self.size
 
-
-class Item_Impl(dict):
+class _ItemMixin(dict):
     NAMESPACE = None
  
     def _make_path(self, path):
         # if self.NAMESPACE:
         #     return "%s.%s" % (self.NAMESPACE, path)
         return path
 
@@ -349,16 +365,16 @@
         Returns:
             data that was removed        
         """
         op = "%s:$xpopl" % self._make_path(path)
         oplog = self._update({op: True})
         return oplog.get(op)
 
-    def currdate(self, path:str, value:Any=True):
-        op = "%s:$currdate" % self._make_path(path)
+    def timestamp(self, path:str, value:Any=True):
+        op = "%s:$timestamp" % self._make_path(path)
         oplog = self._update({op: value})
         return oplog.get(op)   
 
     def template(self, path:str, value:str):
         op = "%s:$template" % self._make_path(path)
         oplog = self._update({op: value})
         return oplog.get(op)
@@ -381,15 +397,15 @@
 
             or 
             #item.update({k/v...}).commit()
         """
         self._update(data)
         return self
 
-class CollectionItem(Item_Impl):
+class CollectionItem(_ItemMixin):
     """
     CollectionItem
 
     Every row is a document 
     """
 
     # item _key
@@ -397,28 +413,32 @@
 
     # items subcollections
     _subcollections = {}
     
     # immutable keys
     _immut_keys = []
 
+    # _read_only. When read_only, it can update 
+    _read_only = False
+
     @classmethod
-    def new(cls, data:dict, immut_keys:list=[], db=None, collection=None, commiter=None, custom_ops:dict={}):
-      return cls(data=_create_document_item(data), db=db, collection=collection, immut_keys=immut_keys, commiter=commiter, custom_ops=custom_ops)
+    def new(cls, data:dict, immut_keys:list=[], db=None, collection=None, commiter=None, custom_ops:dict={}, read_only:bool=False):
+      return cls(data=_create_document_item(data), db=db, collection=collection, immut_keys=immut_keys, commiter=commiter, custom_ops=custom_ops, read_only=read_only)
 
-    def __init__(self, data: dict, db=None, collection=None, immut_keys:list=[], load_parser=None, commiter=None, custom_ops:dict={}):
+    def __init__(self, data: dict, db=None, collection=None, immut_keys:list=[], load_parser=None, commiter=None, custom_ops:dict={}, read_only:bool=False):
         if "_key" not in data:
             raise MissingItemKeyError()
         self._db = db
         self._collection = collection
         self._load_parser = load_parser
         self._commiter = commiter
         self._immut_keys = immut_keys
         self._cx = False
         self._custom_ops = custom_ops
+        self._read_only = read_only
     
         data, _ = dict_mutator.mutate(mutations=data,  immuts=immut_keys, custom_ops=self._custom_ops)
         self._load(data)
 
     def to_dict(self):
         data = dict(self)
         if self._subcollections:
@@ -487,30 +507,30 @@
                 sc.insert({...})
             
             or refer to #context_subscollection
 
         """
         return SubCollection(item=self, name=name, custom_ops=self._custom_ops, constraints=constraints)
 
-    def get_item(self, path:str) -> "SubCollectionItem":
+    def get_item(self, path:str) -> "_SubCollectionItem":
         """
         To get a subcollection item via path
 
         Path: [SUB_COLLECTION_NAME/DOCUMENT_KEY] -> articles/1234568
 
         Params:
             path:str - str of [sub_collection_name/document_key]
         Return:
             collection.item
 
         Example:
             db.get_item("collection/_key").get_item("sub_collection/_key")
         
         Returns:
-            SubCollectionItem
+            _SubCollectionItem
 
         """
         
         paths = path.split("/")
         if len(paths) != 2:
             raise InvalidItemPathError()
 
@@ -532,25 +552,33 @@
 
     def _set_subcollection(self, name:str, data:Any):
         self._subcollections[name] = data
         self.set("__subcollections", self._subcollections)
 
     def commit(self) -> "Self":
         """ To save """
+
+        if self._read_only:
+            return self
+        
         if not self._commiter:
             raise MissingCommitterCallbackError()
         data = self._commiter(self)
         if data:
             self._load(data)
         return self
         
     def _update(self, mutations: dict):
         """
         Return oplog
         """
+        
+        if self._read_only:
+            return self
+        
         data = self.to_dict()
         doc, oplog = dict_mutator.mutate(mutations=mutations, init_data=data, immuts=self._immut_keys, custom_ops=self._custom_ops)
         self._load(doc)
         return oplog
 
     def _load(self, item: dict):
         """
@@ -601,192 +629,39 @@
         Params:
             - nattime:str - Natural time - ie 1hour, 60seconds
 
         Returns:
             self
         """
         if isinstance(nattime, str):
-            self.update({"__ttl:$currdate": nattime})
+            self.update({"__ttl:$timestamp": nattime})
         elif nattime is False:
             self.update({"__ttl": None})
         return self
 
     def delete(self) -> bool:
         """
         To delete an item
         Todo: deleted links/edges
         """
         self._collection.delete(self._key)
         return True
 
-class SubCollection(object):
-    _data = []
-    _constraints = []
-    _item = None
-    _name = None 
-
-    def __init__(self, item: CollectionItem, name: str, constraints:list=None, custom_ops:dict={}):
-        self._item = item
-        self._name = name
-        self._constraints = constraints
-        self._load()
-        self._custom_ops = custom_ops
-
-    def _load(self):
-        self._data = self._item._subcollections.get(self._name) or []
-
-    def _commit(self):
-        self._item._set_subcollection(self._name, self._data)
-
-    def _save(self, _key, data):
-        _data = self._normalize_data()
-        _data[_key] = data
-        self._data = self._denormalize_data(_data)
-        self._commit()        
-
-    def _normalize_data(self) -> dict:
-        return { d.get("_key"): d for d in self._data}
-
-    def _denormalize_data(self, data:dict) -> list:
-        return list(data.values())
-
-    def __len__(self):
-        return len(self._data)
-
-    def __iter__(self):
-        return iter(self.find())
-
-    @property
-    def items(self):
-        """ 
-        Returns an iterator of all documents
-
-        Returns:
-            Iterator
-        """
-        return self.find()
-
-    def has(self, _key):
-        return bool(self.find_one({"_key": _key}))
-
-    def insert(self, data: dict, _key:str=None):
-        """
-        Insert document
-
-        Params:
-            data:dict
-            _key: to insert with a _key
-        """
-        data, _ = dict_mutator.mutate(mutations=data.copy(), immuts=self._item._immut_keys, custom_ops=self._custom_ops)
-
-        if self._constraints:
-            for c in  self._constraints:
-                if c in data:
-                    if self.find_one({c: data[c]}):
-                        raise ConstraintError("Key: %s" % c)
-
-        if _key or "_key" in data:
-            _key = _key or data["_key"]
-            if self.has(_key):
-                raise ItemExistsError()
-            data["_key"] = _key
-        item = data
-
-        item = _create_document_item(data)
-        self._data.append(item)
-        self._commit()
-        return SubCollectionItem(self, item)
-
-    def update(self, filters:dict, mutations: dict, upsert:bool=False):
-        """
-        Update by filter
-
-        Params:
-            filter:dict - filter document criteria
-            mutations:dict - changes on the found documents
-        """
-        _data = self._normalize_data()
-        res = self.find(filters)
-        if res:
-            for item in res:
-                ts = lib.get_timestamp()
-                _key = item.get("_key")
-                _default = {  # ensuring we do some data can't be overwritten
-                    "_key": _key,
-                    # "_created_at": ts
-                }
-                upd, _ = dict_mutator.mutate(mutations=mutations, init_data=item, immuts=self._item._immut_keys, custom_ops=self._custom_ops)
-                _data[_key] = {**upd, **_default}
-            self._data = self._denormalize_data(_data)
-            self._commit()
-
-        elif upsert:
-            self.insert(mutations)
-  
-
-    def delete(self, filters: dict):
-        """
-        Delete documents based on filters
-
-        Params:
-            filters:dict
+    def get_sizeof(self) -> int:
         """
-        _data = self._normalize_data()
-        for item in self.find(filters):
-            del _data[item.get("_key")]
-        self._data = self._denormalize_data(_data)
-        self._commit()
+        Get the size of the document
 
-    def get(self, _key:str) -> "SubCollectionItem":
+        Returns: int
         """
-        Return a document from subcollection by id 
+        return lib.get_sizeof(self.to_dict())
 
-        Returns: SubCollectionItem
-        """
-        return self.find_one({"_key": _key})
-
-    def find_one(self, filters:dict={}) -> "SubCollectionItem":
-        """
-        Return only one item by criteria
-
-        Return:
-            dict
-        """
-        if res := self.find(filters=filters, limit=1):
-            return list(res)[0]
-        return None 
-
-    def find(self, filters: dict = {}, sorts: dict = {}, limit: int = 10,  offset:int=0) -> dict_query.Cursor:
-        """
-        Perform a query
-
-        Params:
-            filters:
-            sorts:
-            limit:
-            offset:
-        """
-        sorts = _parse_sort_dict(sorts, False)
-        data = [SubCollectionItem(self, d) for d in dict_query.query(data=self._data, filters=filters)]
-        return dict_query.Cursor(data, sort=sorts, limit=limit, offset=offset)
-
-    def filter(self, filters: dict = {}) -> dict_query.Cursor:
-        """
-        Alias to find() but makes it seems fluenty
-        
-        Returns:
-            dict_query:Cursor
-        """
-        data = dict_query.query(data=self._data, filters=filters)
-        return dict_query.Cursor([SubCollectionItem(self, d) for d in data])
-
-class SubCollectionItem(Item_Impl):
+class _SubCollectionItem(_ItemMixin):
     _key = None 
 
-    def __init__(self, subCollection: SubCollection, data):
+    def __init__(self, subCollection: "SubCollection", data):
         self._subcollection = subCollection
         self._load(data)
 
     @property
     def parent(self):
         """
         Holds parent data
@@ -804,42 +679,43 @@
     def _load(self, data):
         self._key = data.get("_key")
         super().__init__(data)
 
     def delete(self):
         self._subcollection.delete({"_key": self._key})
         return True
-        
+     
+#------------------------------------------------------------------------------
 #------------------------------------------------------------------------------
 
 class Database(object):
     """
     Angola Database
     """
     SYSTEM_DB = "_system"
 
     def __init__(self,
                  hosts:str=None,
                  username:str="root",
                  password:str=None, 
                  dbname: str = SYSTEM_DB, 
                  client:"Database"= None, 
-                 default_indexes:dict={},
+                 default_indexes:list=[],
                  query_max_limit=100,
                  collection_prefix:str=None,
                  custom_ops:dict={}):
         """
         
         Params:
             host:str|list
             username:str
             password
             dbname
             client:Database
-            default_indexes:dict
+            default_indexes:list
             query_max_limit
             collection_prefix:str|function - a prefix to add in all collection name
             custom_ops:dict - 
         
         """
 
         self.client = client
@@ -928,41 +804,56 @@
 
         Returns:
             bool
         """
         collection_name = self._prefix_collection_name(collection_name)
         return self.db.has_collection(collection_name)
 
-    def select_collection(self, collection_name:str, indexes=None, immut_keys=None, user_defined=True, item_class=None) -> "Collection":
+    def create_collection(self, collection_name:str, indexes:list=[]) -> bool:
+        """
+        Create a collection if not exists
+        Returns: bool
+        """
+        if not self.has_collection(collection_name):
+            collection_name = self._prefix_collection_name(collection_name)
+            col = self.db.create_collection(collection_name)
+
+            _indexes = DEFAULT_INDEXES
+            if not indexes and self.default_indexes:
+                _indexes = [*self.default_indexes, *_indexes]
+
+            for index in _indexes:
+                col._add_index(index) 
+                
+            return True 
+        return False
+
+    def select_collection(self, collection_name:str, indexes:list=[], immut_keys:list=[], item_class=None, auto_create:bool=True) -> "Collection":
         """
         To select a collection
 
         Params:
             collection_name:str - collectioin name 
             indexes:List[dict] - the indexes to use
             immut_keys:list - immutable keys. Keys that can't be updated once created
+            auto_create:bool - To auto create the collection if doesn't exist
 
-        Return:
-            Collection
+        Return: Collection
 
         """
 
         if self.has_collection(collection_name):
             collection_name = self._prefix_collection_name(collection_name)
             col = self.db.collection(collection_name)
-        else:
+        elif auto_create is True:
+            self.create_collection(collection_name=collection_name, indexes=indexes)
             collection_name = self._prefix_collection_name(collection_name)
-            col = self.db.create_collection(collection_name)
-            if not indexes and user_defined is True and self.default_indexes:
-                indexes = self.default_indexes
-            
-            # indexes
-            if indexes and isinstance(indexes, list):
-                for index in [*indexes, *DEFAULT_INDEXES]:
-                    col._add_index(index) 
+            col = self.db.collection(collection_name)
+        else:
+            raise CollectionNotFoundError()
 
         return Collection(db=self, collection=col, immut_keys=immut_keys, custom_ops=self._custom_ops, item_class=item_class)
 
     def select_edge_collection(self, collection_name:str):
         if self.db.has_collection(collection_name):
             collection_name = self._prefix_collection_name(collection_name)
             return self.db.collection(collection_name)
@@ -1015,32 +906,32 @@
         Params:
             query:str - the AQL to execute 
             bind_vars: dict - the variables to pass in the query
         Return aql cursor
         """
         return self.aql.execute(query=query, bind_vars=bind_vars, *a, **kw)
 
-    def query(self, xql:lib_xql.XQLDEFINITION, data:dict={}, kvmap:dict={}, parser=None, data_mapper=None) -> QueryResult:
+    def query(self, xql:lib_xql.XQLDEFINITION, data:dict={}, kvmap:dict={}, parser=None, data_mapper=None) -> _QueryResultIterator:
         """
         XQL query  a collection based on filters
 
         It will return the cursor:ArangoCursor and a pagination for the current state
         
         Params:
             xql:lib_xql.XQLDEFINITION
             data:dict
             kvmap:dict
             data_mapper:function - a callback function
         Returns
-            QueryResult
+            _QueryResultIterator
         """
 
         aql, bind_vars, pager = self._build_query(xql=xql, data=data, kvmap=kvmap, parser=parser)
         cursor = self.execute_aql(aql, bind_vars=bind_vars, count=True, full_count=True)            
-        return QueryResult(cursor=cursor, pager=pager, data_mapper=data_mapper)
+        return _QueryResultIterator(cursor=cursor, pager=pager, data_mapper=data_mapper)
 
     def _build_query(self, xql:lib_xql.XQLDEFINITION, data:dict={}, kvmap:dict={}, parser=None):
         """
         Build a query from XQL
 
         Return tuple:
             - aql:str
@@ -1254,42 +1145,49 @@
         self.db = db
         self.collection = collection
         self._immut_keys = immut_keys
         self._custom_ops = custom_ops
         self.collection_name = self.collection.name
         self.item_class = item_class
 
-    def _commit(self, item:CollectionItem):
+    def _commit(self, item:CollectionItem, replace_document=False):
         """
-        Save the item in the db
+        To commit/save changes
+
+        Params:
+            item:CollectionItem
+            replace_document:bool - To replace instead of updating. Replace will not merge the data.
         """
         if not item._key:
             raise MissingItemKeyError()
         try:
-            item.currdate('_modified_at')
-            return self.collection.update(item.to_dict(), return_new=True)["new"]
+            if replace_document:
+                return self.collection.replace(item.to_dict(), return_new=True)["new"]
+            else:
+                item.timestamp('_modified_at')
+                return self.collection.update(item.to_dict(), return_new=True)["new"]
         except DocumentUpdateError as due:
             item.update({"_modified_at": None})
             return self.collection.insert(item.to_dict(), return_new=True)["new"]
 
     def __iter__(self):
         return self.find(filters={})
 
-    def item(self, data:dict) -> CollectionItem:
+    def item(self, data:dict, read_only:bool=False) -> CollectionItem:
         """
         Load data as item
 
         Returns:
             CollectionItem
         """
         item = None
         if not isinstance(data, CollectionItem) and "_key" not in data:
             item = CollectionItem.new(data, db=self.db, collection=self.collection, commiter=self._commit, immut_keys=self._immut_keys, custom_ops=self._custom_ops)               
         else:
-            item = CollectionItem(data, db=self.db, collection=self.collection, commiter=self._commit, immut_keys=self._immut_keys, custom_ops=self._custom_ops)
+            item = CollectionItem(data, db=self.db, collection=self.collection, commiter=self._commit, immut_keys=self._immut_keys, custom_ops=self._custom_ops, read_only=read_only)
 
         return self.item_class(item) if item and self.item_class else item
 
     def has(self, _key) -> bool: 
         """
         Check if a collection has _key
 
@@ -1344,24 +1242,29 @@
             data["_key"] = _key
         item = data
         if not isinstance(data, CollectionItem):
             item = CollectionItem.new(data, db=self.db, collection=self.collection, custom_ops=self._custom_ops)
         self.collection.insert(item.to_dict(), silent=True)
         return self.get(item._key) 
 
-    def update(self, _key:str, data:dict) -> CollectionItem:
+    def update(self, _key:str, data:dict, replace_document=False) -> CollectionItem:
         """
-        Update an item
+        To update and item. Can also replace the item
+
+        Params:
+            _key:str - document key 
+            data:dict - data to update
+            replace_document:bool - If true will replace the document and not merge
 
         Returns
             CollectionItem
 
         """
         item = self.item({**data, "_key": _key})
-        self._commit(item)  
+        self._commit(item, replace_document=replace_document)  
         return self.get(item._key) 
 
     def upsert(self, data:dict) -> CollectionItem:
         """
         To update or insert data.
 
         Args:
@@ -1379,36 +1282,47 @@
 
     def delete(self, _key):
         """
         Delete a document by _key
         """
         self.collection.delete(_key)
 
-    def find(self, filters:dict={}, offset=None, limit=10, sort=None, page=None):
+    def find(self, filters:dict={}, offset=None, limit=10, sort=None, page=None, xql:dict=None):
         """
         Perform a find in the collections
 
         Returns
             Generator[CollectionItem]
         """
         
+        if page is None and offset:
+            page = lib.calc_pagination_page_from_offset(offset=offset, per_page=limit)
 
-        if offset is None and page:
+        elif offset is None and page:
             offset = lib.calc_pagination_offset(page=page, per_page=limit)
 
-        xql = {
+        read_only = False
+        _xql = {
             "FROM": self.collection_name, 
             "FILTERS": filters,
             "OFFSET": offset,
             "LIMIT": limit,
-            "SORT": sort
+            "SORT": sort,
+            "PAGE": page
         }
 
-        def data_mapper(item): return self.item(item)
-        return self.db.query(xql, data_mapper=data_mapper)
+        # Extended XQL
+        if xql:
+            _xql.update(xql)
+            if "JOIN" in _xql:
+                read_only = True
+
+
+        def data_mapper(item): return self.item(item, read_only=read_only)
+        return self.db.query(_xql, data_mapper=data_mapper)
 
     def find_one(self, filters:dict, sort=None):
         """
         Retrieve one item based on the criteria
 
         Returns
             CollectionItem
@@ -1429,36 +1343,213 @@
         Returns
             tuple(name, edge_name, from_collection_name, to_collection_name)
         """
         edge_name = _create_edge_name(from_name=self.collection_name, to_name=collection.collection_name)
         name = "%s--%s" % (self.collection_name, collection.collection_name)
         return (name, edge_name, self.collection_name, collection.collection_name)
 
+
+class SubCollection(object):
+    _data = []
+    _constraints = []
+    _item = None
+    _name = None 
+
+    def __init__(self, item: CollectionItem, name: str, constraints:list=None, custom_ops:dict={}):
+        self._item = item
+        self._name = name
+        self._constraints = constraints
+        self._load()
+        self._custom_ops = custom_ops
+
+    def _load(self):
+        self._data = self._item._subcollections.get(self._name) or []
+
+    def _commit(self):
+        self._item._set_subcollection(self._name, self._data)
+
+    def _save(self, _key, data):
+        _data = self._normalize_data()
+        _data[_key] = data
+        self._data = self._denormalize_data(_data)
+        self._commit()        
+
+    def _normalize_data(self) -> dict:
+        return { d.get("_key"): d for d in self._data}
+
+    def _denormalize_data(self, data:dict) -> list:
+        return list(data.values())
+
+    def __len__(self):
+        return len(self._data)
+
+    def __iter__(self):
+        return iter(self.find())
+
+    @property
+    def items(self):
+        """ 
+        Returns an iterator of all documents
+
+        Returns:
+            Iterator
+        """
+        return self.find()
+
+    def has(self, _key):
+        return bool(self.find_one({"_key": _key}))
+
+    def insert(self, data: dict, _key:str=None):
+        """
+        Insert document
+
+        Params:
+            data:dict
+            _key: to insert with a _key
+        """
+        data, _ = dict_mutator.mutate(mutations=data.copy(), immuts=self._item._immut_keys, custom_ops=self._custom_ops)
+
+        if self._constraints:
+            for c in  self._constraints:
+                if c in data:
+                    if self.find_one({c: data[c]}):
+                        raise ConstraintError("Key: %s" % c)
+
+        if _key or "_key" in data:
+            _key = _key or data["_key"]
+            if self.has(_key):
+                raise ItemExistsError()
+            data["_key"] = _key
+        item = data
+
+        item = _create_subdocument_item(data)
+        self._data.append(item)
+        self._commit()
+        return _SubCollectionItem(self, item)
+
+    def update(self, filters:dict, mutations: dict, upsert:bool=False):
+        """
+        Update by filter
+
+        Params:
+            filter:dict - filter document criteria
+            mutations:dict - changes on the found documents
+        """
+        _data = self._normalize_data()
+        res = self.find(filters)
+        if res:
+            for item in res:
+                ts = lib.get_timestamp()
+                _key = item.get("_key")
+                _default = {  # ensuring we do some data can't be overwritten
+                    "_key": _key,
+                    # "_created_at": ts
+                }
+                upd, _ = dict_mutator.mutate(mutations=mutations, init_data=item, immuts=self._item._immut_keys, custom_ops=self._custom_ops)
+                _data[_key] = {**upd, **_default}
+            self._data = self._denormalize_data(_data)
+            self._commit()
+
+        elif upsert:
+            self.insert(mutations)
+  
+
+    def delete(self, filters: dict):
+        """
+        Delete documents based on filters
+
+        Params:
+            filters:dict
+        """
+        _data = self._normalize_data()
+        for item in self.find(filters):
+            del _data[item.get("_key")]
+        self._data = self._denormalize_data(_data)
+        self._commit()
+
+    def get(self, _key:str) -> "_SubCollectionItem":
+        """
+        Return a document from subcollection by id 
+
+        Returns: _SubCollectionItem
+        """
+        return self.find_one({"_key": _key})
+
+    def find_one(self, filters:dict={}) -> "_SubCollectionItem":
+        """
+        Return only one item by criteria
+
+        Return:
+            dict
+        """
+        if res := self.find(filters=filters, limit=1):
+            return list(res)[0]
+        return None 
+
+    def find(self, filters: dict = {}, sort: dict = {}, limit: int = 10,  offset:int=0, page=None) -> dict_query.Cursor:
+        """
+        Perform a query
+
+        Params:
+            filters:
+            sort:
+            limit:
+            offset:
+        """
+
+        if offset is None and page:
+            offset = lib.calc_pagination_offset(page=page, per_page=limit)
+
+        sort = _parse_sort_dict(sort, False)
+        data = [_SubCollectionItem(self, d) for d in dict_query.query(data=self._data, filters=filters)]
+        return dict_query.Cursor(data, sort=sort, limit=limit, offset=offset)
+
+    def filter(self, filters: dict = {}) -> dict_query.Cursor:
+        """
+        Alias to find() but makes it seems fluenty
+        
+        Returns:
+            dict_query:Cursor
+        """
+        data = dict_query.query(data=self._data, filters=filters)
+        return dict_query.Cursor([_SubCollectionItem(self, d) for d in data])
+
+
 #------------------------------------------------------------------------------
 
 def _create_edge_name(from_name, to_name):
     return "edges__%s--%s" % (from_name, to_name)
 
 def _create_document_item(data:dict={}) -> dict:
     _key = data["_key"] if "_key" in data else lib.gen_key()
 
     return {
-        **data,
         "_key": _key,
-        "_created_at:$currdate": True,
-        "_modified_at": None
+        "_created_at:$timestamp": True,
+        "_modified_at": None,
+        "__ttl": None,
+        **data,
     }
 
+def _create_subdocument_item(data:dict={}) -> dict:
+    _key = data["_key"] if "_key" in data else lib.gen_key()
+
+    return {
+        "_key": _key,
+        "_created_at:$timestamp": True,
+        "_modified_at": None,
+        **data,
+    }
 
 def _ascdesc(v, as_str=True):
     if as_str:
         if isinstance(v, int):
             return "DESC" if v == -1 else "ASC"
     else:
         if isinstance(v, str):
             return -1 if v.upper() == "DESC" else 1
     return v
 
 
-def _parse_sort_dict(sorts: dict, as_str=True):
-    return [(k, _ascdesc(v, as_str)) for k, v in sorts.items()]
+def _parse_sort_dict(sort: dict, as_str=True):
+    return [(k, _ascdesc(v, as_str)) for k, v in sort.items()]
```

### Comparing `angola-0.10.9/src/angola/dict_mutator.py` & `angola-0.11.0/src/angola/dict_mutator.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,17 @@
     Operators:
         $set - to set a literal k/v
         $incr - to increase an INT value
         $decr - to decrease an INT value
         $unset - To remove a property
         $rename - To rename a property
         $copy - To copy the value of property to another one
-        $currdate - gen the current datetime. Can manipulate time
+        $datetime - gen the current datetime. Can manipulate time
         $template - Evalute the string as template
-        $uuid4 - gen a UUID4 string, without the dashes
+        $uuid4 - gen a UUID4 string, with the dashes
         $xadd - add item if doesn't exist
         $xadd_many - add many items in the list if not already in the list
         $xrem - remove item
         $xrem_many - remove many items in a list
         $xpush - push item on the right
         $xpush_many - push many items in a list on the right
         $xpushl - push item on the left
@@ -127,16 +127,16 @@
            "some.list:$xpush": Any,
            "some.list:$xpush_many": [Any, Any, Any, ...],   
            "some.list:$xpushl": Any,
            "some.list:$xpushl_many": [Any, Any, Any, ...],    
            "some.list:$xpop": True,
            "some.list:$xpopl: False,
            "some.value:$xlen": "some.data.path",
-           "some.datetimefield:$currdate": True,             
-           "some.datetimefield:$currdate": "+1Day +2Hours 5Minutes",
+           "some.datetimefield:$datetime": True,             
+           "some.datetimefield:$datetime": "+1Day +2Hours 5Minutes",
            "some.key:$template": "Hello {{ name }}!",
            "some.random.id:$uuid4": True             
         }
 
     Custom operations
         Extends the dict mutator with custom operations 
 
@@ -215,31 +215,31 @@
 
             # $unset
             elif op == "unset":
                 v = _pop(data, path)
                 oplog[oplog_path] = v
                 value = _UnOperableValue()
 
-            # $currdate
-            elif op == "currdate":
+            # $datetime 
+            elif op in ["datetime", "timestamp", "currdate"]:
                 dt = _get_datetime()
                 if value is True:
                     value = dt
                 else:
                     try:
                         if isinstance(value, str):
                             value = _arrow_date_shifter(dt=dt, stmt=value)
                         else:
                             value = _UnOperableValue()
                     except:
                         value = _UnOperableValue()
 
             # $uuid4
             elif op == "uuid4":
-                value = str(uuid.uuid4()).replace("-", "")
+                value = str(uuid.uuid4())#.replace("-", "")
 
 
             # LIST operators
 
             elif op in (
                 "xadd", "xadd_many",
                 "xrem", "xrem_many",
@@ -319,15 +319,16 @@
                     if path in immuts:
                         continue 
 
                     # $template
                     if op == "template": 
                         _tpl_data =  {
                             **data,
-                            "CURRDATE": _j2_currdate
+                            "TIMESTAMP": _j2_currdate,
+                            "DATETIME": _j2_currdate
                         }              
                         data[path] = lib.render_template(source=value, data=_tpl_data, is_data_flatten=True)
                     
                     # $xlen
                     elif op == "xlen" and value:
                         v = _get(data, value)
                         try:
```

### Comparing `angola-0.10.9/src/angola/dict_query.py` & `angola-0.11.0/src/angola/dict_query.py`

 * *Files identical despite different names*

### Comparing `angola-0.10.9/src/angola/lib.py` & `angola-0.11.0/src/angola/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,33 @@
 from slugify import slugify
 from jinja2 import Template
 from functools import reduce
 from operator import itemgetter
 from typing import Iterator, Any
 
 
+
+def get_sizeof(obj:Any) -> int:
+    """
+    Get the memory size of the object in byte.
+
+    Note: make use of `sys.getsizeof` to get the size in memory. Do not use `len`
+
+    Example: 
+        get_sizeof('hello') -> 56
+        get_sizeof({'name': 'awesome'}) -> 68
+        get_sizeof(12) -> 51
+        get_size(json.loads($json_string)) -> $x
+        
+    Return: int 
+    """
+    return sys.getsizeof(json_dumps(obj))
+
+
+
 def collection_name_valid(name):
     """
     Valid a collection name 
     length: 2, 64
     pattern: lowercase, letters and numbers and underscore
     """
     pattern = re.compile(r"^[a-z][a-z0-9\_]{2,64}$")
@@ -176,43 +195,14 @@
     Generates the current UTC timestamp with datetime
     Returns:
       int
     """
     return round(datetime.datetime.utcnow().timestamp())
 
 
-
-# === JSON 
-
-def _json_serialize(o):
-    return timestamp_to_str(o)
-
-def _json_deserialize(json_dict):
-    for k, v in json_dict.items():
-        if isinstance(v, str) and timestamp_valid(v):
-            json_dict[k] = arrow.get(v)
-    return json_dict
-
-def timestamp_to_str(dt) -> str:
-    if isinstance(dt, arrow.Arrow):
-        return dt.for_json()
-    elif isinstance(dt, (datetime.date, datetime.datetime)):
-        return dt.isoformat()
-    return dt
-
-
-def timestamp_valid(dt_str) -> bool:
-    try:
-        datetime.datetime.fromisoformat(dt_str.replace('Z', '+00:00'))
-    except:
-        return False
-    return True
-
-
-
 # ----------------------
 # json_ext
 
 class json_ext:
     """ 
     JSON Extension class to loads and dumps json
     """
@@ -302,25 +292,28 @@
       an unflatten dictionnary
     """
     output = {}
     for k, v in flatten_dict.items():
         path = k.split(".")
         if isinstance(v, list):
             v = [unflatten_dict(i2) if isinstance(i2, dict) else i2 for i2 in v]
-        _set_nested(output, path, v)
+        _set_nested(output, path, v, k)
     return output
 
 
 def _get_nested_default(d, path):
     return reduce(lambda d, k: d.setdefault(k, {}), path, d)
 
 
-def _set_nested(d, path, value):
-    _get_nested_default(d, path[:-1])[path[-1]] = value
-
+def _set_nested(d, path, value, full_path=None):
+    try:
+        _get_nested_default(d, path[:-1])[path[-1]] = value
+    except (AttributeError, TypeError) as e:
+        err = "DataTypeAttributeError: %s at '%s'" % (e, full_path)
+        raise AttributeError(err)
 
 def dict_pick(ddict: dict, keys: list, check_keys=False) -> dict:
     """
     To pick and return specific keys from a flatten dict.
 
     Args:
       ddict: dict
@@ -538,18 +531,29 @@
     Args:
         - page:int - the current page
         - per_page:int - items per page
     Returns: int 
     """
     return 0 if page < 1 else (page - 1) * per_page
 
+def calc_pagination_page_from_offset(offset:int, per_page:int) -> int:
+    """
+    To calculate the pagination page having provided an offset and a per_page
+    
+    Args:
+        - offset:int - The offset 
+        - per_page: total items per page
+    Returns: int
+    """
+    return 1 if offset <= 0 else round((offset / per_page))
+
 
 def gen_pagination(size: int, count: int, page: int, per_page: int) -> dict:
     """
-    Create pagination data based on some basic info
+    Create pagination data for pagination components
 
     Args:
         - size:int - The total items
         - count:int - the current count for the subset
         - page:int - the current page
         - per_page:int - total items per page
```

### Comparing `angola-0.10.9/src/angola/lib_xql.py` & `angola-0.11.0/src/angola/lib_xql.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,87 +20,102 @@
 AQL_FILTER_OPERATORS = {
     "$EQ": "==",  # equal
     "$NE": "!=",  # not equal
     "$GT": ">",  # greater than
     "$GTE": ">=",  # greater than or equal
     "$LT": "<",  # lesser than
     "$LTE": "<=",  # lesser than or equal
-    "$IN": "IN",  # left hand in right hand array -> field.value IN [values]
-    # left hand not in right hand array -> field.value NOT IN [values]
-    "$XIN": "NOT IN",
-    # right hand in left hand array -> values IN [field.value]
+
+    # INCLUDES + XINCLUDES
+    # Test if data in RIGHT(string|int) is in data in LEFT(array)
+    # ie: "__subcollections.something[*].value:$INCLUDES": "my-value"
+    # --> "my-value" IN __subcollections.something[*].value 
     "$INCLUDES": "IN",
-    # right hand not in left hand array -> values NOT IN [field.value]
     "$XINCLUDES": "NOT IN",
-    "$LIKE": "LIKE",  # search
-    "$XLIKE": "NOT LIKE"  # ,
 
+    # IN + NIN
+    # reverse the order of INCLUDES
+    # To test if data in (LEFT:str|int) is in the (RIGHT:array)
+    # ie "city:$IN": ["charlotte", "atlanta"]
+    # --> u.city IN ["charlotte", "atlanta"]
+    "$IN": "IN",
+    "$XIN": "NOT IN",
+
+
+    # LIKE + NOTLIKE
+    # right hand in left hand array -> values IN [field.value]
+    "$LIKE": "LIKE",  # search
+    "$NLIKE": "NOT LIKE",  # 
+    #TODO:
+    # == for case insensitive ==
+    # "$ILIKE": "",
+    # "$NILIKE": ""
 }
 # reverse operator, where the right hand will point to left hand
-# ie: cities:$includes:'charlotte' -> 'charlotte' IN cities
+# ie: cities:$INCLUDES: 'charlotte' -> 'charlotte' IN cities
 _rev_ops_order = ['$INCLUDES', '$XINCLUDES']
 
 
+
 # -----------------------------------------------------------------------------
 # === MACROS ------------------------------------------------------------------
 
 def _re_match(pattern, value) -> re:
     return re.match(pattern, value, flags=re.IGNORECASE)
 
 
-def _macro_currdate(re_match:re):
+def _macro_now(re_match:re):
     """
-    This macros eval the @@CURRENDATE in the query
+    This macro eval the NOW|DATETIME in the query
     
     :Params:
         :re_match: regexp match the 
 
     Regex: 
 
+
     Example:
         {
-            "_created_at:$gt": "@@CURRDATE() -5days"
+            "_created_at:$gt": "[[@MACRO:NOW, -3hours]]",
         }
 
-    Format: [@@CURRDATE($format) $shifter]
-    Regex: ^\@\@CURRDATE\((.*)\)\s*(.*)$
-
-        match[1] = format
-        match[2] = shifter
+    Format: [[@MACRO:NOW, shifter, format]]
+    Regex: "^\[\[\@MACRO:NOW\s*,?\s*(.*)]]$",
+        re_match[1]
     """
-    dt_format = re_match[1] or "YYYY-MM-DD"
-    shifter = re_match[2]
+
+    dt_format = "YYYY-MM-DD"
+    shifter = re_match[1]
+    if "," in shifter:
+        shifter, dt_format = shifter.split(",", 1)
+        shifter = shifter.strip()
+        dt_format = dt_format.strip()
+
     now = lib.get_datetime()
     if shifter:
         now = lib.arrow_date_shifter(now, shifter)
     return now.format(dt_format )
 
 
 MACROS_DEFS = [
     {
-        # '@@CURRDATE(format=YYYY-MM-DD) shifter=+3Days 4Weeks'
-        "name": "CURRDATE",
-        "pattern": "^\@\@CURRDATE\((.*)\)\s*(.*)$",
-        "func": _macro_currdate
+        # [[@MACRO:NOW, +2Days, YYYY-MM-DD HH:mm:ss]]
+        "name": "NOW",
+        "pattern": "^\[\[\@MACRO:NOW\s*,?\s*(.*)]]$",
+        "func": _macro_now
     }
 ]
 
 
 def eval_macros(value):
     for item in MACROS_DEFS:
         if isinstance(value, str) and (m := _re_match(item.get("pattern"), value)):
             return item.get("func")(m)
         elif isinstance(value, list):
-            vs = []
-            for v in value:
-                if m := _re_match(item.get("pattern"), v):
-                    vs.append(item.get("func")(m))
-                else:
-                    vs.append(v)
-            return vs
+            return [eval_macros(v) for v in value]
     return value
 
 # -----------------------------------------------------------------------------
 # -----------------------------------------------------------------------------
 
 
 def aql_sort_builder(sorts: list, propkey: str) -> str:
@@ -258,28 +273,30 @@
         # params[ukey] = value
     return aql, params
 
 
 def prepare_xql(xql: dict) -> dict:
     _defaults = {
         "FROM": None,
-        "ON": None,
-        "AS": "doc__",
+        "ALIAS": "root__",
         "FILTERS": {},
         "SORT": None,
         "OFFSET": None,
         "COUNT_AS": None,
         "LIMIT": 10,
         "PAGE": 1,
         "JOIN": [],
-        "RETURN": "doc__",
+        "RETURN": None,
         "RETURN_WITH": None,
         **xql
     }
-    return {k.upper(): v for k, v in _defaults.items()}
+    r = {k.upper(): v for k, v in _defaults.items()}
+    if r["RETURN"] is None:
+        r["RETURN"] = r["ALIAS"]
+    return r
 
 
 def xql_take_skip_page(xql: dict, max_limit=100) -> tuple:
     """
     Returns:
         type: tuple(LIMIT:int, OFFSET:int, PAGE:1)
             - LIMIT: limit/per_page
@@ -305,38 +322,36 @@
 
 
 class XQLDEFINITION:
     """
     XQL Schema Definition:
 
         :param FROM: str = the collection name
-        :param AS: str = alias
+        :param ALIAS: str = alias
         :param FILTERS: dict = filters
         :param SORT: list/str = sort 
         :param OFFSET: int = the offset of the limit, default=0
         :param LIMIT: int = the limit of result, default=10
         :param PAGE: int = help calculate the skip by using a page number. 
         :param JOIN: list[XQL]
-        :param ON: str = when using join, it links the primary _key 
         :param COUNT_AS: str =  To count all the document, and return the value. Alias to `COLLECT WITH COUNT INTO`
         :param RETURN: str = string representation
         :param MERGE: str = on JOIN, to merge the data.
             ie: MERGE: "{__profile: profile}" 
             Can be done manually with RETURN MERGE(doc, {data})
 
     """
     FROM: str = None
-    AS: str = None
+    ALIAS: str = None
     FILTERS: dict = {}
     SORT: list = []
     OFFSET: int = 0
     LIMIT: int = 10
     PAGE: int = 1
     JOIN: list = []
-    ON: str = None
     COUNT_AS: str = None
     RETURN: str = None
     MERGE: str = None
 
 
 def xql_to_aql(xql: dict, vars: dict = {}, max_limit=100, parser=None):
     """
@@ -355,44 +370,42 @@
 
     Returns:
         tuple(AQL:string, BIND_VARS:dict)
 
     ===
     XQL Schema Definition:
         FROM: str = the collection name
-        AS: str = alias
+        ALIAS: str = alias
         FILTERS: dict = filters
         SORT: list/str = sort 
         OFFSET: int = the offset of the limit, default=0
         LIMIT: int = the limit of result, default=10
         PAGE: int = help calculate the offset by using a page number. 
         JOIN: list[XQL]
-        ON: str = when using join, it links the primary _key 
         COUNT_AS: str =  To count all the document, and return the value. Alias to `COLLECT WITH COUNT INTO`
         RETURN: str = string representation
         MERGE: str = on JOIN, to merge the data.
             ie: MERGE: "{__profile: profile}" 
             Can be done manually with RETURN MERGE(doc, {data})
 
-
         # TODO
         - WHEN: ? = a conditional to evaluate before running
         - FILTER_WHEN: add additional filters when a condition is true
 
     === 
     schema example:
         FROM: collection
-        AS: alias1
+        ALIAS: alias1
         FILTERS:
             x:y
             "z:$gt": 5
         SORT: name:desc
         JOIN:
             FROM: collection2
-            AS: c2
+            ALIAS: c2
             FILTERS:
                 d: "#alias1.d"
             LIMIT: 5
             PAGE: 2
             RETURN: c2
         LIMIT: 10
         OFFSET: 2
@@ -400,60 +413,60 @@
             d
             c2
 
 
         === code example
         q = {
             "FROM": "job_posts",
-            "AS": "post",
+            "ALIAS": "post",
             "FILTERS": {
                 "a": "b",
                 "c:$gt": 5
             },
             "SORT": ["id:desc"],
             "LIMIT": 10,
             "OFFSET": 47,
             "JOIN": [
                 {
-                    "AS": "app",
+                    "ALIAS": "app",
                     "FROM": "application",
                     "FILTERS": {
                         "a": "b",
                         "c": "d",
                         "d": "#job.v_d"
                     },
                     "JOIN": [        {
-                        "AS": "J_loco",
+                        "ALIAS": "J_loco",
                         "FROM": "bam",
                         "FILTERS": {
                             "a": "b",
                             "c": "d",
                             "d": "#app.v_d"
                         }
                     }]
                 },
                 {
                     "FROM": "loco",
-                    "AS": "bam",
+                    "ALIAS": "bam",
                     "FILTERS": {
                         "a": "b",
                         "c": "d",
                         "d": "#app.v_d"
                     }
                 }
             ],
             "RETURN": "MERGE(post, {__account: loco})"
     """
 
     xql = prepare_xql(xql)
 
-    if not xql.get("AS"):
-        xql["AS"] = "doc__"
+    if not xql.get("ALIAS"):
+        xql["ALIAS"] = "root__"
 
-    ALIAS = xql.get("AS") or "doc__"
+    ALIAS = xql.get("ALIAS") or "root__"
 
     if parser:
         xql = parser(xql)
 
     COLLECTION = xql.get("FROM")
     FILTERS = xql.get("FILTERS") or {}
     SORTS = xql.get("SORT")
@@ -472,14 +485,15 @@
         if per_page > max_limit:
             per_page = max_limit
         OFFSET = lib.calc_pagination_offset(page=page, per_page=per_page)
         LIMIT = per_page
     if LIMIT > max_limit:
         LIMIT = max_limit
 
+
     # unique num to give each field to prevent name collision
     num_ = lib.gen_number(6)
     aql_filter, filter_vars = aql_filter_builder(FILTERS, propkey=ALIAS)
     aql_sorting = aql_sort_builder(SORTS, propkey=ALIAS)
     aql_collects = xql_collects_builder(COLLECTS, propkey=ALIAS)
     if COUNT_AS:
         aql_collects += " COLLECT WITH COUNT INTO %s " % COUNT_AS
@@ -487,34 +501,32 @@
     bind_vars = {}
 
     # SUBQUERY/JOINS
     subquery = ""
     for xql2 in JOINS:
         xql2 = prepare_xql(xql2)
         X = xql_to_aql(xql=xql2, parser=parser, max_limit=max_limit)
-        subquery += "\nLET %s = (%s) \n" % (xql2.get("AS"), X[0])
+        subquery += "\nLET %s = (%s) \n" % (xql2.get("ALIAS"), X[0])
         bind_vars.update(X[1])
 
     # Query
-    query = "FOR {alias} IN @@collection_{num_} ".format(
-        alias=ALIAS, num_=num_)
+    query = "FOR {alias} IN @@collection_{num_} ".format(alias=ALIAS, num_=num_)
     query += aql_filter
     query += subquery
     query += aql_collects
     query += " LIMIT @offset_%s, @limit_%s " % (num_, num_)
     query += aql_sorting
     query += "RETURN UNSET_RECURSIVE(%s, ['_id', '_rev', '_old_rev'])" % RETURN
 
     bind_vars.update({
         **filter_vars,
         "offset_%s" % num_: OFFSET,
         "limit_%s" % num_: LIMIT,
         "@collection_%s" % num_: COLLECTION
     })
-
     return query, bind_vars
 
 
 def xql_extract_collections(xql: dict) -> list:
     """
     Extract all the collection names. 
     This can help with testing collection name
```

### Comparing `angola-0.10.9/src/angola.egg-info/PKG-INFO` & `angola-0.11.0/src/angola.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: angola
-Version: 0.10.9
+Version: 0.11.0
 Summary: angola 
 Home-page: https://github.com/mardix/angola
 Author: Mardix
 Author-email: mardix@blackdevhub.io
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Database
```

### Comparing `angola-0.10.9/tests/test_database.py` & `angola-0.11.0/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `angola-0.10.9/tests/test_dict_mutator.py` & `angola-0.11.0/tests/test_dict_mutator.py`

 * *Files identical despite different names*

### Comparing `angola-0.10.9/tests/test_lib.py` & `angola-0.11.0/tests/test_lib.py`

 * *Files identical despite different names*


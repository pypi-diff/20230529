# Comparing `tmp/atlasq-0.8.0.tar.gz` & `tmp/atlasq-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlasq-0.8.0.tar", last modified: Mon Dec 19 17:04:22 2022, max compression
+gzip compressed data, was "atlasq-0.9.0.tar", last modified: Tue Dec 20 13:44:17 2022, max compression
```

## Comparing `atlasq-0.8.0.tar` & `atlasq-0.9.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:04:22.710278 atlasq-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-19 17:04:10.000000 atlasq-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-19 17:04:10.000000 atlasq-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2022-12-19 17:04:22.710278 atlasq-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2022-12-19 17:04:10.000000 atlasq-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:04:22.710278 atlasq-0.8.0/atlasq/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-19 17:04:10.000000 atlasq-0.8.0/atlasq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:04:22.710278 atlasq-0.8.0/atlasq/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 17:04:10.000000 atlasq-0.8.0/atlasq/queryset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7706 2022-12-19 17:04:10.000000 atlasq-0.8.0/atlasq/queryset/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-19 17:04:10.000000 atlasq-0.8.0/atlasq/queryset/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2022-12-19 17:04:10.000000 atlasq-0.8.0/atlasq/queryset/index.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2022-12-19 17:04:10.000000 atlasq-0.8.0/atlasq/queryset/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2022-12-19 17:04:10.000000 atlasq-0.8.0/atlasq/queryset/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2022-12-19 17:04:10.000000 atlasq-0.8.0/atlasq/queryset/queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    11683 2022-12-19 17:04:10.000000 atlasq-0.8.0/atlasq/queryset/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2022-12-19 17:04:10.000000 atlasq-0.8.0/atlasq/queryset/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:04:22.710278 atlasq-0.8.0/atlasq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2022-12-19 17:04:22.000000 atlasq-0.8.0/atlasq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      790 2022-12-19 17:04:22.000000 atlasq-0.8.0/atlasq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-19 17:04:22.000000 atlasq-0.8.0/atlasq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      440 2022-12-19 17:04:22.000000 atlasq-0.8.0/atlasq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-19 17:04:22.000000 atlasq-0.8.0/atlasq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      156 2022-12-19 17:04:10.000000 atlasq-0.8.0/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-19 17:04:10.000000 atlasq-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-19 17:04:10.000000 atlasq-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-19 17:04:22.710278 atlasq-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2022-12-19 17:04:10.000000 atlasq-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:04:22.710278 atlasq-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 17:04:10.000000 atlasq-0.8.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-19 17:04:22.710278 atlasq-0.8.0/tests/queryset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-19 17:04:10.000000 atlasq-0.8.0/tests/queryset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6622 2022-12-19 17:04:10.000000 atlasq-0.8.0/tests/queryset/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6710 2022-12-19 17:04:10.000000 atlasq-0.8.0/tests/queryset/test_index.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2022-12-19 17:04:10.000000 atlasq-0.8.0/tests/queryset/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2022-12-19 17:04:10.000000 atlasq-0.8.0/tests/queryset/test_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6613 2022-12-19 17:04:10.000000 atlasq-0.8.0/tests/queryset/test_queryset.py
--rw-r--r--   0 runner    (1001) docker     (123)    37822 2022-12-19 17:04:10.000000 atlasq-0.8.0/tests/queryset/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2022-12-19 17:04:10.000000 atlasq-0.8.0/tests/queryset/test_visitor.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-19 17:04:10.000000 atlasq-0.8.0/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-19 17:04:10.000000 atlasq-0.8.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 13:44:17.565806 atlasq-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2022-12-20 13:44:05.000000 atlasq-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2022-12-20 13:44:05.000000 atlasq-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2022-12-20 13:44:17.565806 atlasq-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5064 2022-12-20 13:44:05.000000 atlasq-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 13:44:17.561806 atlasq-0.9.0/atlasq/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2022-12-20 13:44:05.000000 atlasq-0.9.0/atlasq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 13:44:17.561806 atlasq-0.9.0/atlasq/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 13:44:05.000000 atlasq-0.9.0/atlasq/queryset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 2022-12-20 13:44:05.000000 atlasq-0.9.0/atlasq/queryset/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2022-12-20 13:44:05.000000 atlasq-0.9.0/atlasq/queryset/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5499 2022-12-20 13:44:05.000000 atlasq-0.9.0/atlasq/queryset/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2022-12-20 13:44:05.000000 atlasq-0.9.0/atlasq/queryset/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2022-12-20 13:44:05.000000 atlasq-0.9.0/atlasq/queryset/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2022-12-20 13:44:05.000000 atlasq-0.9.0/atlasq/queryset/queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2022-12-20 13:44:05.000000 atlasq-0.9.0/atlasq/queryset/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2022-12-20 13:44:05.000000 atlasq-0.9.0/atlasq/queryset/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 13:44:17.561806 atlasq-0.9.0/atlasq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2022-12-20 13:44:17.000000 atlasq-0.9.0/atlasq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2022-12-20 13:44:17.000000 atlasq-0.9.0/atlasq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 13:44:17.000000 atlasq-0.9.0/atlasq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2022-12-20 13:44:17.000000 atlasq-0.9.0/atlasq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-20 13:44:17.000000 atlasq-0.9.0/atlasq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2022-12-20 13:44:05.000000 atlasq-0.9.0/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2022-12-20 13:44:05.000000 atlasq-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2022-12-20 13:44:05.000000 atlasq-0.9.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 13:44:17.565806 atlasq-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2022-12-20 13:44:05.000000 atlasq-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 13:44:17.565806 atlasq-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 13:44:05.000000 atlasq-0.9.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 13:44:17.565806 atlasq-0.9.0/tests/queryset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 13:44:05.000000 atlasq-0.9.0/tests/queryset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6622 2022-12-20 13:44:05.000000 atlasq-0.9.0/tests/queryset/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2022-12-20 13:44:05.000000 atlasq-0.9.0/tests/queryset/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2022-12-20 13:44:05.000000 atlasq-0.9.0/tests/queryset/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2022-12-20 13:44:05.000000 atlasq-0.9.0/tests/queryset/test_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6613 2022-12-20 13:44:05.000000 atlasq-0.9.0/tests/queryset/test_queryset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37822 2022-12-20 13:44:05.000000 atlasq-0.9.0/tests/queryset/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2022-12-20 13:44:05.000000 atlasq-0.9.0/tests/queryset/test_visitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2022-12-20 13:44:05.000000 atlasq-0.9.0/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 13:44:05.000000 atlasq-0.9.0/version.py
```

### Comparing `atlasq-0.8.0/LICENSE` & `atlasq-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/PKG-INFO` & `atlasq-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlasq
-Version: 0.8.0
+Version: 0.9.0
 Summary: Query proxy that allows the usage of AtlasSearch with mongoengine specific syntax
 Home-page: https://github.com/certego/atlasq
 Author: Certego S.R.L
 Project-URL: Documentation, https://github.com/certego/atlasq
 Project-URL: Source, https://github.com/certego/atlasq
 Project-URL: Tracker, https://github.com/certego/atlasq/issues
 Keywords: certego atlas mongoengine python search textsearch atlassearch
@@ -73,30 +73,82 @@
 
 obj2_from_atlas = MyDocument.atlas.get(AtlasQ(name="value") & AtlasQ(surname="value2"))
 assert obj == obj2_from_atlas
 
 
 obj3_from_atlas = MyDocument.atlas.get(AtlasQ(wrong_field="value"))
 assert obj3_from_atlas is None
-
-result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
-assert result is True
-obj3_from_atlas = MyDocument.atlas.get(AtlasQ(wrong_field="value")) # raises AtlasIndexFieldError
-
-
-
 ```
 
 ##  Extended Features
 
 ### Validation
 We also decided to have, optionally, a validation of the index.
 Two things are checked:
 - The index actually exists (If you query a non-existing index, Atlas as default behaviour will not raise any error).
 - The fields that you are querying are actually indexed(If you query a field that is not indexed, Atlas as default behaviour will not raise any error, and will return an empty list).
-To make these check, you need to call the function `ensure_index` on the queryset:
+To make these check, you need to call the function `ensure_index` on the queryset.
+
+```python3
+from mongoengine import Document, fields
+
+from atlasq import AtlasManager, AtlasQ
+
+index_name = str("my_index")
+
+class MyDocument(Document):
+    name = fields.StringField(required=True)
+    surname = fields.StringField(required=True)
+    atlas = AtlasManager(index_name)
+
+result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
+assert result is True
+obj1_from_atlas = MyDocument.atlas.get(AtlasQ(name="value")) 
+obj2_from_atlas = MyDocument.atlas.get(AtlasQ(wrong_field="value")) # raises AtlasIndexFieldError
+```
 
 ### EmbeddedDocuments
 Embedded documents are queried in two different ways, depending on how you created your Search Index.
 Remember to ensure the index so that AtlasQ can know how your index is defined
 If you used the [embeddedDocuments](https://www.mongodb.com/docs/atlas/atlas-search/define-field-mappings/#std-label-bson-data-types-embedded-documents) type, AtlasQ will use the [embeddedDocument](https://www.mongodb.com/docs/atlas/atlas-search/embedded-document/) query syntax.
 Otherwise, if you used the [document](https://www.mongodb.com/docs/atlas/atlas-search/define-field-mappings/#document) type, or you did not ensure the index, a normal `text` search with the `.` syntax will be used.
+
+### Upload index
+It is possible to upload directly the Search index using AtlasQ, calling the function `upload_index` on the queryset. Syntax checks on the index itself are performed.
+If the `_id` is not present but `pk` or `id` was specified, it will be automatically added, allowing valid text query on the
+primary key.
+
+```python3
+from mongoengine import Document, fields
+
+from atlasq import AtlasManager
+
+index_name = str("my_index")
+index = {
+  "analyzer": "lucene.keyword",
+  "mappings": {
+    "dynamic": False,
+    "fields": {
+      "_id": {
+        "type": "objectId"
+      },
+        "name": {
+        "type": "string"
+      },
+      "surname": {
+        "type": "string"
+      },
+    }
+  }
+}
+class MyDocument(Document):
+    name = fields.StringField(required=True)
+    surname = fields.StringField(required=True)
+    atlas = AtlasManager(index_name)
+
+result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
+assert result is False
+MyDocument.atlas.upload_index(index, "user", "pwd", "group", "cluster")
+result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
+assert result is True
+
+```
```

### Comparing `atlasq-0.8.0/README.md` & `atlasq-0.9.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -48,30 +48,82 @@
 
 obj2_from_atlas = MyDocument.atlas.get(AtlasQ(name="value") & AtlasQ(surname="value2"))
 assert obj == obj2_from_atlas
 
 
 obj3_from_atlas = MyDocument.atlas.get(AtlasQ(wrong_field="value"))
 assert obj3_from_atlas is None
-
-result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
-assert result is True
-obj3_from_atlas = MyDocument.atlas.get(AtlasQ(wrong_field="value")) # raises AtlasIndexFieldError
-
-
-
 ```
 
 ##  Extended Features
 
 ### Validation
 We also decided to have, optionally, a validation of the index.
 Two things are checked:
 - The index actually exists (If you query a non-existing index, Atlas as default behaviour will not raise any error).
 - The fields that you are querying are actually indexed(If you query a field that is not indexed, Atlas as default behaviour will not raise any error, and will return an empty list).
-To make these check, you need to call the function `ensure_index` on the queryset:
+To make these check, you need to call the function `ensure_index` on the queryset.
+
+```python3
+from mongoengine import Document, fields
+
+from atlasq import AtlasManager, AtlasQ
+
+index_name = str("my_index")
+
+class MyDocument(Document):
+    name = fields.StringField(required=True)
+    surname = fields.StringField(required=True)
+    atlas = AtlasManager(index_name)
+
+result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
+assert result is True
+obj1_from_atlas = MyDocument.atlas.get(AtlasQ(name="value")) 
+obj2_from_atlas = MyDocument.atlas.get(AtlasQ(wrong_field="value")) # raises AtlasIndexFieldError
+```
 
 ### EmbeddedDocuments
 Embedded documents are queried in two different ways, depending on how you created your Search Index.
 Remember to ensure the index so that AtlasQ can know how your index is defined
 If you used the [embeddedDocuments](https://www.mongodb.com/docs/atlas/atlas-search/define-field-mappings/#std-label-bson-data-types-embedded-documents) type, AtlasQ will use the [embeddedDocument](https://www.mongodb.com/docs/atlas/atlas-search/embedded-document/) query syntax.
 Otherwise, if you used the [document](https://www.mongodb.com/docs/atlas/atlas-search/define-field-mappings/#document) type, or you did not ensure the index, a normal `text` search with the `.` syntax will be used.
+
+### Upload index
+It is possible to upload directly the Search index using AtlasQ, calling the function `upload_index` on the queryset. Syntax checks on the index itself are performed.
+If the `_id` is not present but `pk` or `id` was specified, it will be automatically added, allowing valid text query on the
+primary key.
+
+```python3
+from mongoengine import Document, fields
+
+from atlasq import AtlasManager
+
+index_name = str("my_index")
+index = {
+  "analyzer": "lucene.keyword",
+  "mappings": {
+    "dynamic": False,
+    "fields": {
+      "_id": {
+        "type": "objectId"
+      },
+        "name": {
+        "type": "string"
+      },
+      "surname": {
+        "type": "string"
+      },
+    }
+  }
+}
+class MyDocument(Document):
+    name = fields.StringField(required=True)
+    surname = fields.StringField(required=True)
+    atlas = AtlasManager(index_name)
+
+result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
+assert result is False
+MyDocument.atlas.upload_index(index, "user", "pwd", "group", "cluster")
+result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
+assert result is True
+
+```
```

### Comparing `atlasq-0.8.0/atlasq/queryset/cache.py` & `atlasq-0.9.0/atlasq/queryset/cache.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/atlasq/queryset/index.py` & `atlasq-0.9.0/atlasq/queryset/index.py`

 * *Files 25% similar despite different names*

```diff
@@ -64,14 +64,32 @@
         user: str,
         password: str,
         group_id: str,
         cluster_name: str,
     ):
         if not self.index:
             raise AtlasIndexError("No index defined")
+
+        if not isinstance(data, dict):
+            raise AtlasIndexError("The index should be a dictionary")
+        if "mappings" not in data:
+            raise AtlasIndexError("There is no 'mappings' in the index")
+        if not isinstance(data["mappings"], dict):
+            raise AtlasIndexError("The mappings keyword should be a dictionary")
+        if "fields" not in data["mappings"]:
+            raise AtlasIndexError("There is no 'mappings' in the index")
+        if not isinstance(data["mappings"]["fields"], dict):
+            raise AtlasIndexError("The fields keyword should be a dictionary")
+
+        if any(id_keyword in data["mappings"]["fields"] for id_keyword in ["id", "pk"]):
+            if "_id" not in data["mappings"]["fields"]:
+                data["mappings"]["fields"]["_id"] = {
+                    "type": AtlasIndexType.OBJECT_ID.value
+                }
+
         url = TEXT_INDEXES_ENDPOINT.format(
             GROUP_ID=group_id,
             CLUSTER_NAME=cluster_name,
         )
         response = requests.post(
             url,
             json=data,
```

### Comparing `atlasq-0.8.0/atlasq/queryset/manager.py` & `atlasq-0.9.0/atlasq/queryset/manager.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/atlasq/queryset/node.py` & `atlasq-0.9.0/atlasq/queryset/node.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/atlasq/queryset/queryset.py` & `atlasq-0.9.0/atlasq/queryset/queryset.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/atlasq/queryset/transform.py` & `atlasq-0.9.0/atlasq/queryset/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,21 @@
 from atlasq.queryset.exceptions import AtlasFieldError, AtlasIndexFieldError
 from atlasq.queryset.index import AtlasIndex, AtlasIndexType
 
 logger = logging.getLogger(__name__)
 
 
 class AtlasTransform:
+
+    id_keywords = [
+        "pk",
+        "id",
+        "_id",
+    ]
+
     keywords = [
         "ne",
         "lt",
         "gt",
         "lte",
         "gte",
         "in",
@@ -203,23 +210,25 @@
                 logger.debug(
                     "Casting queryset to list, otherwise the aggregation will fail"
                 )
                 value = list(value)
             key_parts = key.split("__")
             obj = None
             path = ""
-            for i, key_part in enumerate(key_parts):
-                if key_part not in self.keywords:
+            for i, keyword in enumerate(key_parts):
+
+                if keyword in self.id_keywords:
+                    keyword = "_id"
+                if keyword not in self.keywords:
                     continue
                 # the key_part is made of "field__subfield__keywords
                 # meaning that the first time that we find a keyword, we have the entire path
                 if not path:
                     path = ".".join(key_parts[:i])
 
-                keyword = key_part
                 if keyword in self.not_converted:
                     raise NotImplementedError(f"Keyword {keyword} not implemented yet")
                 if keyword in self.negative_keywords:
                     to_go *= -1
 
                 if keyword in self.size_keywords:
                     # it must the last keyword, otherwise we do not support it
```

### Comparing `atlasq-0.8.0/atlasq/queryset/visitor.py` & `atlasq-0.9.0/atlasq/queryset/visitor.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/atlasq.egg-info/PKG-INFO` & `atlasq-0.9.0/atlasq.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlasq
-Version: 0.8.0
+Version: 0.9.0
 Summary: Query proxy that allows the usage of AtlasSearch with mongoengine specific syntax
 Home-page: https://github.com/certego/atlasq
 Author: Certego S.R.L
 Project-URL: Documentation, https://github.com/certego/atlasq
 Project-URL: Source, https://github.com/certego/atlasq
 Project-URL: Tracker, https://github.com/certego/atlasq/issues
 Keywords: certego atlas mongoengine python search textsearch atlassearch
@@ -73,30 +73,82 @@
 
 obj2_from_atlas = MyDocument.atlas.get(AtlasQ(name="value") & AtlasQ(surname="value2"))
 assert obj == obj2_from_atlas
 
 
 obj3_from_atlas = MyDocument.atlas.get(AtlasQ(wrong_field="value"))
 assert obj3_from_atlas is None
-
-result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
-assert result is True
-obj3_from_atlas = MyDocument.atlas.get(AtlasQ(wrong_field="value")) # raises AtlasIndexFieldError
-
-
-
 ```
 
 ##  Extended Features
 
 ### Validation
 We also decided to have, optionally, a validation of the index.
 Two things are checked:
 - The index actually exists (If you query a non-existing index, Atlas as default behaviour will not raise any error).
 - The fields that you are querying are actually indexed(If you query a field that is not indexed, Atlas as default behaviour will not raise any error, and will return an empty list).
-To make these check, you need to call the function `ensure_index` on the queryset:
+To make these check, you need to call the function `ensure_index` on the queryset.
+
+```python3
+from mongoengine import Document, fields
+
+from atlasq import AtlasManager, AtlasQ
+
+index_name = str("my_index")
+
+class MyDocument(Document):
+    name = fields.StringField(required=True)
+    surname = fields.StringField(required=True)
+    atlas = AtlasManager(index_name)
+
+result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
+assert result is True
+obj1_from_atlas = MyDocument.atlas.get(AtlasQ(name="value")) 
+obj2_from_atlas = MyDocument.atlas.get(AtlasQ(wrong_field="value")) # raises AtlasIndexFieldError
+```
 
 ### EmbeddedDocuments
 Embedded documents are queried in two different ways, depending on how you created your Search Index.
 Remember to ensure the index so that AtlasQ can know how your index is defined
 If you used the [embeddedDocuments](https://www.mongodb.com/docs/atlas/atlas-search/define-field-mappings/#std-label-bson-data-types-embedded-documents) type, AtlasQ will use the [embeddedDocument](https://www.mongodb.com/docs/atlas/atlas-search/embedded-document/) query syntax.
 Otherwise, if you used the [document](https://www.mongodb.com/docs/atlas/atlas-search/define-field-mappings/#document) type, or you did not ensure the index, a normal `text` search with the `.` syntax will be used.
+
+### Upload index
+It is possible to upload directly the Search index using AtlasQ, calling the function `upload_index` on the queryset. Syntax checks on the index itself are performed.
+If the `_id` is not present but `pk` or `id` was specified, it will be automatically added, allowing valid text query on the
+primary key.
+
+```python3
+from mongoengine import Document, fields
+
+from atlasq import AtlasManager
+
+index_name = str("my_index")
+index = {
+  "analyzer": "lucene.keyword",
+  "mappings": {
+    "dynamic": False,
+    "fields": {
+      "_id": {
+        "type": "objectId"
+      },
+        "name": {
+        "type": "string"
+      },
+      "surname": {
+        "type": "string"
+      },
+    }
+  }
+}
+class MyDocument(Document):
+    name = fields.StringField(required=True)
+    surname = fields.StringField(required=True)
+    atlas = AtlasManager(index_name)
+
+result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
+assert result is False
+MyDocument.atlas.upload_index(index, "user", "pwd", "group", "cluster")
+result = MyDocument.atlas.ensure_index("user", "pwd", "group", "cluster")
+assert result is True
+
+```
```

### Comparing `atlasq-0.8.0/atlasq.egg-info/SOURCES.txt` & `atlasq-0.9.0/atlasq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/setup.py` & `atlasq-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/tests/queryset/test_cache.py` & `atlasq-0.9.0/tests/queryset/test_cache.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/tests/queryset/test_index.py` & `atlasq-0.9.0/tests/queryset/test_index.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/tests/queryset/test_manager.py` & `atlasq-0.9.0/tests/queryset/test_manager.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/tests/queryset/test_node.py` & `atlasq-0.9.0/tests/queryset/test_node.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/tests/queryset/test_queryset.py` & `atlasq-0.9.0/tests/queryset/test_queryset.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/tests/queryset/test_transform.py` & `atlasq-0.9.0/tests/queryset/test_transform.py`

 * *Files identical despite different names*

### Comparing `atlasq-0.8.0/tests/queryset/test_visitor.py` & `atlasq-0.9.0/tests/queryset/test_visitor.py`

 * *Files identical despite different names*


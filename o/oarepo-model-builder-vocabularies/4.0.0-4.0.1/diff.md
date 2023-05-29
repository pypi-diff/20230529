# Comparing `tmp/oarepo-model-builder-vocabularies-4.0.0.tar.gz` & `tmp/oarepo-model-builder-vocabularies-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-model-builder-vocabularies-4.0.0.tar", last modified: Tue May 23 08:21:20 2023, max compression
+gzip compressed data, was "oarepo-model-builder-vocabularies-4.0.1.tar", last modified: Mon May 29 11:44:26 2023, max compression
```

## Comparing `oarepo-model-builder-vocabularies-4.0.0.tar` & `oarepo-model-builder-vocabularies-4.0.1.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:21:20.429694 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/builders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/builders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/builders/setup_cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/datatypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/vocabulary.json
--rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/vocabulary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:18:39.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 08:21:20.000000 oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-23 08:21:20.433694 oarepo-model-builder-vocabularies-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-23 08:17:49.000000 oarepo-model-builder-vocabularies-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:44:26.151791 oarepo-model-builder-vocabularies-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-29 11:44:26.155791 oarepo-model-builder-vocabularies-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:44:26.151791 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:44:26.151791 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/builders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/builders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/builders/setup_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/datatypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:44:26.151791 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/vocabulary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3780 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/vocabulary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:44:26.151791 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:42:01.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 11:44:26.000000 oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-05-29 11:44:26.155791 oarepo-model-builder-vocabularies-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-29 11:40:59.000000 oarepo-model-builder-vocabularies-4.0.1/setup.py
```

### Comparing `oarepo-model-builder-vocabularies-4.0.0/PKG-INFO` & `oarepo-model-builder-vocabularies-4.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 4.0.0
+Version: 4.0.1
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/datatypes.py` & `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/datatypes.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from oarepo_model_builder.datatypes.datatypes import DataType
 from oarepo_model_builder.validation import InvalidModelException
 from oarepo_model_builder_relations.datatypes import RelationDataType
 
 
 class VocabularyDataType(RelationDataType):
     model_type = "vocabulary"
-    default_facet_class = "VocabularyFacet"
-    default_facet_imports = [
-        {"import": "oarepo_vocabularies.services.facets.VocabularyFacet"}
-    ]
+    facets = {
+        'facet-class': "VocabularyFacet",
+        'imports': [
+            {"import": "oarepo_vocabularies.services.facets.VocabularyFacet"}
+        ],
+    }
 
     class ModelSchema(RelationDataType.ModelSchema):
         vocabulary_type = ma.fields.String(
             attribute="vocabulary-type", data_key="vocabulary-type"
         )
 
     def prepare(self, context):
@@ -45,14 +47,19 @@
                     raise InvalidModelException(
                         "{self.stack.path}: Can not have both vocabulary class and type specified"
                     )
                 pid_field = f"{vocabulary_class}.pid"
 
         # self.definition["type"] = "relation"
         self.definition["pid-field"] = pid_field
+
+        # set up vocabulary argument to facets
+        facets = self.definition.setdefault('facets', {})
+        facets.setdefault('args', []).append(f'vocabulary={repr(vocabulary_type)}')
+
         super().prepare(context)
 
     def get_facet(self, stack, parent_path):
         if not stack:
             # we are the facet, unlike normal container, for which a facet is not generated,
             # we need to generate it -> calling direct data type
             return DataType.get_facet(self, stack, parent_path)
@@ -85,18 +92,20 @@
             attribute="vocabulary-type", data_key="vocabulary-type", required=False
         )
         model = fields.String(required=False)
 
 
 class TaxonomyDataType(VocabularyDataType):
     model_type = "taxonomy"
-    default_facet_class = "HierarchyVocabularyFacet"
-    default_facet_imports = [
-        {"import": "oarepo_vocabularies.services.facets.HierarchyVocabularyFacet"}
-    ]
+    facets = {
+        'facet-class': "HierarchyVocabularyFacet",
+        'imports': [
+            {"import": "oarepo_vocabularies.services.facets.HierarchyVocabularyFacet"}
+        ],
+    }
 
     def prepare(self, context):
         keys = list(self.definition.get("keys", []))
         self.definition.setdefault("ui", {}).setdefault("detail", "taxonomy_item")
         self.definition["ui"].setdefault("edit", "taxonomy_item")
 
         def has_key(fields, field_name):
```

### Comparing `oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/vocabulary.json` & `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/vocabulary.json`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies/models/vocabulary.yaml` & `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies/models/vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/PKG-INFO` & `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-model-builder-vocabularies
-Version: 4.0.0
+Version: 4.0.1
 Summary: "A model builder plugin to reference vocabularies"
 Home-page: https://github.com/oarepo/oarepo-model-builder-vocabularies
 Author: Miroslav Simek
 Author-email: simek.miroslav@techlib.cz
 License: MIT
 Keywords: invenio vocabulary model builder
 Platform: any
```

### Comparing `oarepo-model-builder-vocabularies-4.0.0/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt` & `oarepo-model-builder-vocabularies-4.0.1/oarepo_model_builder_vocabularies.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 oarepo_model_builder_vocabularies/__init__.py
+oarepo_model_builder_vocabularies/components.py
 oarepo_model_builder_vocabularies/datatypes.py
 oarepo_model_builder_vocabularies.egg-info/PKG-INFO
 oarepo_model_builder_vocabularies.egg-info/SOURCES.txt
 oarepo_model_builder_vocabularies.egg-info/dependency_links.txt
 oarepo_model_builder_vocabularies.egg-info/entry_points.txt
 oarepo_model_builder_vocabularies.egg-info/not-zip-safe
 oarepo_model_builder_vocabularies.egg-info/requires.txt
```

### Comparing `oarepo-model-builder-vocabularies-4.0.0/setup.cfg` & `oarepo-model-builder-vocabularies-4.0.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-model-builder-vocabularies
-version = 4.0.0
+version = 4.0.1
 description = "A model builder plugin to reference vocabularies"
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = invenio vocabulary model builder
 license = MIT
 author = Miroslav Simek
 author_email = simek.miroslav@techlib.cz
@@ -31,14 +31,16 @@
 	pytest
 
 [options.entry_points]
 oarepo.models = 
 	vocabularies = oarepo_model_builder_vocabularies.models:vocabulary.json
 oarepo_model_builder.datatypes = 
 	vocabulary = oarepo_model_builder_vocabularies.datatypes:DATATYPES
+oarepo_model_builder.datatypes.components = 
+	vocabulary = oarepo_model_builder_vocabularies.components:COMPONENTS
 oarepo_model_builder.builders.record = 
 	2000-vocabularies  = oarepo_model_builder_vocabularies.builders.setup_cfg:VocabulariesSetupCfgBuilder
 
 [build_sphinx]
 source-dir = docs/
 build-dir = docs/_build
 all_files = 1
```


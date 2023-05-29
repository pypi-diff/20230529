# Comparing `tmp/aimped-0.1.43.tar.gz` & `tmp/aimped-0.1.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimped-0.1.43.tar", last modified: Sun May 28 23:22:35 2023, max compression
+gzip compressed data, was "aimped-0.1.44.tar", last modified: Mon May 29 12:37:17 2023, max compression
```

## Comparing `aimped-0.1.43.tar` & `aimped-0.1.44.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.390569 aimped-0.1.43/
--rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.43/LICENSE
--rw-rw-rw-   0        0        0     1791 2023-05-28 23:22:35.391131 aimped-0.1.43/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.43/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.334471 aimped-0.1.43/aimped/
--rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.43/aimped/__init__.py
--rw-rw-rw-   0        0        0     8553 2023-05-28 23:20:53.000000 aimped-0.1.43/aimped/io_tasks.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.346225 aimped-0.1.43/aimped/model/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/model/__init__.py
--rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/model/load.py
--rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/models.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.347865 aimped-0.1.43/aimped/nitro/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nitro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.367879 aimped-0.1.43/aimped/nlp/
--rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/assertion.py
--rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/chunker.py
--rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/deid.py
--rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/ner.py
--rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/ner_cls_report.py
--rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/pipeline.py
--rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/regex_parser.py
--rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.43/aimped/nlp/relation.py
--rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.43/aimped/nlp/relation_visualizer.py
--rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/tokenizer.py
--rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/tools.py
--rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.43/aimped/nlp/translation.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.388335 aimped-0.1.43/aimped/test/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/__init__.py
--rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_assertion.py
--rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_chunk_merger.py
--rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_deid_pipeline.py
--rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_ner_results.py
--rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_regex_parser.py
--rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_relation_pipeline.py
--rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_tokenizer.py
--rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_translation_pipeline.py
--rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/utils.py
--rw-rw-rw-   0        0        0      130 2023-05-28 23:20:53.000000 aimped-0.1.43/aimped/version.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.343428 aimped-0.1.43/aimped.egg-info/
--rw-rw-rw-   0        0        0     1791 2023-05-28 23:22:35.000000 aimped-0.1.43/aimped.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-05-28 23:22:35.000000 aimped-0.1.43/aimped.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 23:22:35.000000 aimped-0.1.43/aimped.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-28 23:22:35.000000 aimped-0.1.43/aimped.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 23:22:35.000000 aimped-0.1.43/aimped.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-28 23:22:35.393459 aimped-0.1.43/setup.cfg
--rw-rw-rw-   0        0        0     1139 2023-04-03 13:18:42.000000 aimped-0.1.43/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.379902 aimped-0.1.44/
+-rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.44/LICENSE
+-rw-rw-rw-   0        0        0     1791 2023-05-29 12:37:17.379902 aimped-0.1.44/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.44/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.320900 aimped-0.1.44/aimped/
+-rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.44/aimped/__init__.py
+-rw-rw-rw-   0        0        0     8755 2023-05-29 10:16:48.000000 aimped-0.1.44/aimped/io_tasks.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.333902 aimped-0.1.44/aimped/model/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/model/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/model/load.py
+-rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/models.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.334904 aimped-0.1.44/aimped/nitro/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nitro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.360907 aimped-0.1.44/aimped/nlp/
+-rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/assertion.py
+-rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/chunker.py
+-rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/deid.py
+-rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/ner.py
+-rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/ner_cls_report.py
+-rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/pipeline.py
+-rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/regex_parser.py
+-rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.44/aimped/nlp/relation.py
+-rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.44/aimped/nlp/relation_visualizer.py
+-rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/tokenizer.py
+-rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/tools.py
+-rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.44/aimped/nlp/translation.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.377905 aimped-0.1.44/aimped/test/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/__init__.py
+-rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_assertion.py
+-rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_chunk_merger.py
+-rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_deid_pipeline.py
+-rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_ner_results.py
+-rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_regex_parser.py
+-rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_relation_pipeline.py
+-rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_tokenizer.py
+-rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_translation_pipeline.py
+-rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/utils.py
+-rw-rw-rw-   0        0        0      130 2023-05-29 12:19:28.000000 aimped-0.1.44/aimped/version.py
+drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.330904 aimped-0.1.44/aimped.egg-info/
+-rw-rw-rw-   0        0        0     1791 2023-05-29 12:37:17.000000 aimped-0.1.44/aimped.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-05-29 12:37:17.000000 aimped-0.1.44/aimped.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 12:37:17.000000 aimped-0.1.44/aimped.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-29 12:37:17.000000 aimped-0.1.44/aimped.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 12:37:17.000000 aimped-0.1.44/aimped.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-29 12:37:17.381914 aimped-0.1.44/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2023-04-03 13:18:42.000000 aimped-0.1.44/setup.py
```

### Comparing `aimped-0.1.43/LICENSE` & `aimped-0.1.44/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/PKG-INFO` & `aimped-0.1.44/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.43
+Version: 0.1.44
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.ml-hub.nioyatechai.com/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimped-0.1.43/README.md` & `aimped-0.1.44/README.md`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/io_tasks.py` & `aimped-0.1.44/aimped/io_tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,15 @@
         self.output['data_json']['result'] = model_prediction
 
 
 ################ Task: Name Entity Recognition ################
 
 class NameEntityRecognitionInput(BaseModel):
     text: List[str] = Field(..., description="List of texts", example=["This is an example text for NER."])
+    entity: List[str] = Field(..., description="List of entities", example=["PERSON", "ORG", "GPE"])
 
 
 class NameEntityRecognitionOutput(BaseModel):
     status: bool = True
     data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
     output: Dict[str, Any] = Field(
         default={"data_json": {"result": None}},
@@ -92,15 +93,15 @@
         self.output['data_json']['result'] = model_prediction
 
 
 ######################### Task: Deidentification #########################
 
 class DeidentificationInput(BaseModel):
     text: List[str] = Field(..., description="List of texts", example=["This is an example text for deidentification."])
-
+    entity: List[str] = Field(..., description="List of entities", example=["PERSON", "ORG", "GPE"])
 
 class DeidentificationOutput(BaseModel):
     status: bool = True
     data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
     output: Dict[str, Any] = Field(
                                     default={"data_json": {"result": None}},
                                     description="Output dictionary",
```

### Comparing `aimped-0.1.43/aimped/model/load.py` & `aimped-0.1.44/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/assertion.py` & `aimped-0.1.44/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/chunker.py` & `aimped-0.1.44/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/deid.py` & `aimped-0.1.44/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/ner.py` & `aimped-0.1.44/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/ner_cls_report.py` & `aimped-0.1.44/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/pipeline.py` & `aimped-0.1.44/aimped/nlp/pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/regex_parser.py` & `aimped-0.1.44/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/relation.py` & `aimped-0.1.44/aimped/nlp/relation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/relation_visualizer.py` & `aimped-0.1.44/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/tokenizer.py` & `aimped-0.1.44/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/tools.py` & `aimped-0.1.44/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/nlp/translation.py` & `aimped-0.1.44/aimped/nlp/translation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/test/test_assertion.py` & `aimped-0.1.44/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/test/test_chunk_merger.py` & `aimped-0.1.44/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/test/test_deid_pipeline.py` & `aimped-0.1.44/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/test/test_ner_results.py` & `aimped-0.1.44/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/test/test_regex_parser.py` & `aimped-0.1.44/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/test/test_relation_pipeline.py` & `aimped-0.1.44/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/test/test_tokenizer.py` & `aimped-0.1.44/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/test/test_translation_pipeline.py` & `aimped-0.1.44/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped/utils.py` & `aimped-0.1.44/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/aimped.egg-info/PKG-INFO` & `aimped-0.1.44/aimped.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.43
+Version: 0.1.44
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.ml-hub.nioyatechai.com/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimped-0.1.43/aimped.egg-info/SOURCES.txt` & `aimped-0.1.44/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimped-0.1.43/setup.py` & `aimped-0.1.44/setup.py`

 * *Files identical despite different names*


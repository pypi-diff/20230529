# Comparing `tmp/aimped-0.1.44.tar.gz` & `tmp/aimped-0.1.45.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimped-0.1.44.tar", last modified: Mon May 29 12:37:17 2023, max compression
+gzip compressed data, was "aimped-0.1.45.tar", last modified: Mon May 29 13:49:39 2023, max compression
```

## Comparing `aimped-0.1.44.tar` & `aimped-0.1.45.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.379902 aimped-0.1.44/
--rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.44/LICENSE
--rw-rw-rw-   0        0        0     1791 2023-05-29 12:37:17.379902 aimped-0.1.44/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.44/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.320900 aimped-0.1.44/aimped/
--rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.44/aimped/__init__.py
--rw-rw-rw-   0        0        0     8755 2023-05-29 10:16:48.000000 aimped-0.1.44/aimped/io_tasks.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.333902 aimped-0.1.44/aimped/model/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/model/__init__.py
--rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/model/load.py
--rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/models.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.334904 aimped-0.1.44/aimped/nitro/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nitro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.360907 aimped-0.1.44/aimped/nlp/
--rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/assertion.py
--rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/chunker.py
--rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/deid.py
--rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/ner.py
--rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/ner_cls_report.py
--rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/pipeline.py
--rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/regex_parser.py
--rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.44/aimped/nlp/relation.py
--rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.44/aimped/nlp/relation_visualizer.py
--rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/tokenizer.py
--rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/nlp/tools.py
--rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.44/aimped/nlp/translation.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.377905 aimped-0.1.44/aimped/test/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/__init__.py
--rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_assertion.py
--rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_chunk_merger.py
--rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_deid_pipeline.py
--rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_ner_results.py
--rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_regex_parser.py
--rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_relation_pipeline.py
--rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_tokenizer.py
--rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/test/test_translation_pipeline.py
--rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.44/aimped/utils.py
--rw-rw-rw-   0        0        0      130 2023-05-29 12:19:28.000000 aimped-0.1.44/aimped/version.py
-drwxrwxrwx   0        0        0        0 2023-05-29 12:37:17.330904 aimped-0.1.44/aimped.egg-info/
--rw-rw-rw-   0        0        0     1791 2023-05-29 12:37:17.000000 aimped-0.1.44/aimped.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-05-29 12:37:17.000000 aimped-0.1.44/aimped.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 12:37:17.000000 aimped-0.1.44/aimped.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-29 12:37:17.000000 aimped-0.1.44/aimped.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 12:37:17.000000 aimped-0.1.44/aimped.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-29 12:37:17.381914 aimped-0.1.44/setup.cfg
--rw-rw-rw-   0        0        0     1139 2023-04-03 13:18:42.000000 aimped-0.1.44/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.147406 aimped-0.1.45/
+-rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.45/LICENSE
+-rw-rw-rw-   0        0        0     1791 2023-05-29 13:49:39.147406 aimped-0.1.45/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.45/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.093404 aimped-0.1.45/aimped/
+-rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.45/aimped/__init__.py
+-rw-rw-rw-   0        0        0     9074 2023-05-29 13:38:05.000000 aimped-0.1.45/aimped/io_tasks.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.104406 aimped-0.1.45/aimped/model/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/model/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/model/load.py
+-rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/models.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.105404 aimped-0.1.45/aimped/nitro/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nitro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.129402 aimped-0.1.45/aimped/nlp/
+-rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/assertion.py
+-rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/chunker.py
+-rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/deid.py
+-rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/ner.py
+-rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/ner_cls_report.py
+-rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/pipeline.py
+-rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/regex_parser.py
+-rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.45/aimped/nlp/relation.py
+-rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.45/aimped/nlp/relation_visualizer.py
+-rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/tokenizer.py
+-rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/tools.py
+-rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.45/aimped/nlp/translation.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.146404 aimped-0.1.45/aimped/test/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/__init__.py
+-rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_assertion.py
+-rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_chunk_merger.py
+-rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_deid_pipeline.py
+-rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_ner_results.py
+-rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_regex_parser.py
+-rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_relation_pipeline.py
+-rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_tokenizer.py
+-rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_translation_pipeline.py
+-rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/utils.py
+-rw-rw-rw-   0        0        0      130 2023-05-29 13:48:50.000000 aimped-0.1.45/aimped/version.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.101410 aimped-0.1.45/aimped.egg-info/
+-rw-rw-rw-   0        0        0     1791 2023-05-29 13:49:38.000000 aimped-0.1.45/aimped.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-05-29 13:49:38.000000 aimped-0.1.45/aimped.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 13:49:38.000000 aimped-0.1.45/aimped.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-29 13:49:38.000000 aimped-0.1.45/aimped.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 13:49:38.000000 aimped-0.1.45/aimped.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-29 13:49:39.149409 aimped-0.1.45/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2023-05-29 13:48:50.000000 aimped-0.1.45/setup.py
```

### Comparing `aimped-0.1.44/LICENSE` & `aimped-0.1.45/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/PKG-INFO` & `aimped-0.1.45/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.44
+Version: 0.1.45
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.ml-hub.nioyatechai.com/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **aimped**
 ![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
 
 **Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**
```

### Comparing `aimped-0.1.44/README.md` & `aimped-0.1.45/README.md`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/io_tasks.py` & `aimped-0.1.45/aimped/io_tasks.py`

 * *Files 3% similar despite different names*

```diff
@@ -142,17 +142,17 @@
 
 # TODO: Add post_init function to check if messages are in correct format
 class ChatbotOutput(BaseModel):
     status: bool = True
     data_type: List[str] = Field(default=["data_json", "data_audio"],
                                  description="List of data types",
                                  enum=data_types)
-    data_json: Dict[str, Any] = Field(default=None, description="Text API Output in dictionary", repr=False)
-    data_audio: str = Field(default=None, description="Audio API Output in base64 format", repr=False,
-                            example="data:audio/mp3;base64,//tQxA-audio-base64-format-string", )
+    # data_json: Dict[str, Any] = Field(default=None, description="Text API Output in dictionary", repr=False, exclude=True,)
+    # data_audio: str = Field(default=None, description="Audio API Output in base64 format", repr=False, exclude=True,
+    #                         example="data:audio/mp3;base64,//tQxA-audio-base64-format-string", )
     raw_output: Dict[str, Any] = Field(default=None, description="Raw API Output in dictionary", repr=False,
                                        exclude=True)
     output: Dict[str, Any] = Field(
         default={"data_json": {"text": None}, "data_audio": None, "raw_output": None},
         description="Output dictionary",
         keys={"enum": data_types},
         example={
@@ -165,14 +165,23 @@
                            'object': 'chat.completion',
                            'usage': {'completion_tokens': 27,
                                      'prompt_tokens': 186,
                                      'total_tokens': 213}},
             "data_audio": "data:audio/mp3;base64,//tQxA-audio-base64-format-audio-file...==="},
     )
 
+    def __init__(self, api_text: Any, api_result: Any, api_audio: Any, **data: Any):
+        super().__init__(**data)
+        self.output['data_json']['text'] = api_text
+        self.output['raw_output'] = api_result
+        self.output['data_audio'] = api_audio
+
+        
+
+
 
 ######################## Task: OCR ######################## TODO: Still in development
 
 class OcrInput(BaseModel):
     text: str
     file_type: str
     file: str
```

### Comparing `aimped-0.1.44/aimped/model/load.py` & `aimped-0.1.45/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/assertion.py` & `aimped-0.1.45/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/chunker.py` & `aimped-0.1.45/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/deid.py` & `aimped-0.1.45/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/ner.py` & `aimped-0.1.45/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/ner_cls_report.py` & `aimped-0.1.45/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/pipeline.py` & `aimped-0.1.45/aimped/nlp/pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/regex_parser.py` & `aimped-0.1.45/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/relation.py` & `aimped-0.1.45/aimped/nlp/relation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/relation_visualizer.py` & `aimped-0.1.45/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/tokenizer.py` & `aimped-0.1.45/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/tools.py` & `aimped-0.1.45/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/nlp/translation.py` & `aimped-0.1.45/aimped/nlp/translation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/test/test_assertion.py` & `aimped-0.1.45/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/test/test_chunk_merger.py` & `aimped-0.1.45/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/test/test_deid_pipeline.py` & `aimped-0.1.45/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/test/test_ner_results.py` & `aimped-0.1.45/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/test/test_regex_parser.py` & `aimped-0.1.45/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/test/test_relation_pipeline.py` & `aimped-0.1.45/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/test/test_tokenizer.py` & `aimped-0.1.45/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/test/test_translation_pipeline.py` & `aimped-0.1.45/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped/utils.py` & `aimped-0.1.45/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/aimped.egg-info/PKG-INFO` & `aimped-0.1.45/aimped.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.44
+Version: 0.1.45
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.ml-hub.nioyatechai.com/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # **aimped**
 ![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
 
 **Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**
```

### Comparing `aimped-0.1.44/aimped.egg-info/SOURCES.txt` & `aimped-0.1.45/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimped-0.1.44/setup.py` & `aimped-0.1.45/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,10 +27,10 @@
     url="https://dev.ml-hub.nioyatechai.com/", 
     
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',
+    python_requires='>=3.7',
 )
```


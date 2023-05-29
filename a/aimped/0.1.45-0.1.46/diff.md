# Comparing `tmp/aimped-0.1.45.tar.gz` & `tmp/aimped-0.1.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimped-0.1.45.tar", last modified: Mon May 29 13:49:39 2023, max compression
+gzip compressed data, was "aimped-0.1.46.tar", last modified: Mon May 29 19:52:10 2023, max compression
```

## Comparing `aimped-0.1.45.tar` & `aimped-0.1.46.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.147406 aimped-0.1.45/
--rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.45/LICENSE
--rw-rw-rw-   0        0        0     1791 2023-05-29 13:49:39.147406 aimped-0.1.45/PKG-INFO
--rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.45/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.093404 aimped-0.1.45/aimped/
--rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.45/aimped/__init__.py
--rw-rw-rw-   0        0        0     9074 2023-05-29 13:38:05.000000 aimped-0.1.45/aimped/io_tasks.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.104406 aimped-0.1.45/aimped/model/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/model/__init__.py
--rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/model/load.py
--rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/models.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.105404 aimped-0.1.45/aimped/nitro/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nitro/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.129402 aimped-0.1.45/aimped/nlp/
--rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/__init__.py
--rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/assertion.py
--rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/chunker.py
--rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/deid.py
--rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/ner.py
--rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/ner_cls_report.py
--rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/pipeline.py
--rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/regex_parser.py
--rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.45/aimped/nlp/relation.py
--rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.45/aimped/nlp/relation_visualizer.py
--rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/tokenizer.py
--rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/nlp/tools.py
--rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.45/aimped/nlp/translation.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.146404 aimped-0.1.45/aimped/test/
--rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/__init__.py
--rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_assertion.py
--rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_chunk_merger.py
--rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_deid_pipeline.py
--rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_ner_results.py
--rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_regex_parser.py
--rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_relation_pipeline.py
--rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_tokenizer.py
--rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/test/test_translation_pipeline.py
--rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.45/aimped/utils.py
--rw-rw-rw-   0        0        0      130 2023-05-29 13:48:50.000000 aimped-0.1.45/aimped/version.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:49:39.101410 aimped-0.1.45/aimped.egg-info/
--rw-rw-rw-   0        0        0     1791 2023-05-29 13:49:38.000000 aimped-0.1.45/aimped.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      952 2023-05-29 13:49:38.000000 aimped-0.1.45/aimped.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 13:49:38.000000 aimped-0.1.45/aimped.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-29 13:49:38.000000 aimped-0.1.45/aimped.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 13:49:38.000000 aimped-0.1.45/aimped.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      111 2023-05-29 13:49:39.149409 aimped-0.1.45/setup.cfg
--rw-rw-rw-   0        0        0     1139 2023-05-29 13:48:50.000000 aimped-0.1.45/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.273401 aimped-0.1.46/
+-rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.46/LICENSE
+-rw-rw-rw-   0        0        0     1791 2023-05-29 19:52:10.274401 aimped-0.1.46/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.46/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.231400 aimped-0.1.46/aimped/
+-rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.46/aimped/__init__.py
+-rw-rw-rw-   0        0        0    12442 2023-05-29 19:36:23.000000 aimped-0.1.46/aimped/io_tasks.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.241400 aimped-0.1.46/aimped/model/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/model/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/model/load.py
+-rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/models.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.242396 aimped-0.1.46/aimped/nitro/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nitro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.260400 aimped-0.1.46/aimped/nlp/
+-rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/assertion.py
+-rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/chunker.py
+-rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/deid.py
+-rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/ner.py
+-rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/ner_cls_report.py
+-rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/pipeline.py
+-rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/regex_parser.py
+-rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.46/aimped/nlp/relation.py
+-rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.46/aimped/nlp/relation_visualizer.py
+-rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/tokenizer.py
+-rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/nlp/tools.py
+-rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.46/aimped/nlp/translation.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.272398 aimped-0.1.46/aimped/test/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/__init__.py
+-rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_assertion.py
+-rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_chunk_merger.py
+-rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_deid_pipeline.py
+-rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_ner_results.py
+-rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_regex_parser.py
+-rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_relation_pipeline.py
+-rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_tokenizer.py
+-rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/test/test_translation_pipeline.py
+-rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.46/aimped/utils.py
+-rw-rw-rw-   0        0        0      130 2023-05-29 19:50:28.000000 aimped-0.1.46/aimped/version.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:52:10.238400 aimped-0.1.46/aimped.egg-info/
+-rw-rw-rw-   0        0        0     1791 2023-05-29 19:52:10.000000 aimped-0.1.46/aimped.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-05-29 19:52:10.000000 aimped-0.1.46/aimped.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 19:52:10.000000 aimped-0.1.46/aimped.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-29 19:52:10.000000 aimped-0.1.46/aimped.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 19:52:10.000000 aimped-0.1.46/aimped.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-29 19:52:10.275400 aimped-0.1.46/setup.cfg
+-rw-rw-rw-   0        0        0     1176 2023-05-29 19:50:28.000000 aimped-0.1.46/setup.py
```

### Comparing `aimped-0.1.45/LICENSE` & `aimped-0.1.46/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/PKG-INFO` & `aimped-0.1.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.45
+Version: 0.1.46
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.ml-hub.nioyatechai.com/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimped-0.1.45/README.md` & `aimped-0.1.46/README.md`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/io_tasks.py` & `aimped-0.1.46/aimped/io_tasks.py`

 * *Files 27% similar despite different names*

```diff
@@ -27,18 +27,20 @@
     'raw_output'
 ]
 
 
 ################ Task: Text Classification ################
 
 class TextClassificationInput(BaseModel):
+    """Input data for text classification task"""
     text: List[str] = Field(..., description="List of texts", example=["This is an example text for classification.",
                                                                        "This is another example text for classification."])
 
 class TextClassificationOutput(BaseModel):
+    """Output data for text classification task"""
     status: bool = True
     data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
     output: Dict[str, Any] = Field(
         default={"data_json": {"result": None}},
         description="data_json output dictionary",
         keys={"enum": data_types},
         example={
@@ -58,19 +60,21 @@
         super().__init__(**data)
         self.output['data_json']['result'] = model_prediction
 
 
 ################ Task: Name Entity Recognition ################
 
 class NameEntityRecognitionInput(BaseModel):
+    """Input data for name entity recognition task"""
     text: List[str] = Field(..., description="List of texts", example=["This is an example text for NER."])
     entity: List[str] = Field(..., description="List of entities", example=["PERSON", "ORG", "GPE"])
 
 
 class NameEntityRecognitionOutput(BaseModel):
+    """Output data for name entity recognition task"""
     status: bool = True
     data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
     output: Dict[str, Any] = Field(
         default={"data_json": {"result": None}},
         description="Output dictionary",
         keys={"enum": data_types},
         example={
@@ -92,18 +96,20 @@
         super().__init__(**data)
         self.output['data_json']['result'] = model_prediction
 
 
 ######################### Task: Deidentification #########################
 
 class DeidentificationInput(BaseModel):
+    """Input data for deidentification task"""
     text: List[str] = Field(..., description="List of texts", example=["This is an example text for deidentification."])
     entity: List[str] = Field(..., description="List of entities", example=["PERSON", "ORG", "GPE"])
 
 class DeidentificationOutput(BaseModel):
+    """Output data for deidentification task"""
     status: bool = True
     data_type: List[str] = Field(default=["data_json"], description="List of data types", enum=data_types)
     output: Dict[str, Any] = Field(
                                     default={"data_json": {"result": None}},
                                     description="Output dictionary",
                                     keys={"enum": data_types},
                                     example={
@@ -127,25 +133,26 @@
         super().__init__(**data)
         self.output['data_json']['result'] = model_prediction
 
 
 ####################### Task: Chatbot ###################### TODO: Still in development
 
 class ChatbotInput(BaseModel):
+    """Input data for chatbot task"""
     messages: List[Dict[str, str]] = Field(..., description="List of messages",
                                            example=[{"role": "user", "content": "Who are you?"},
                                                     {"role": "assistant", "content": "I am Chat Bot. Who are you?"},
                                                     {"role": "user", "content": "I am Joseph."}
                                                     ])
     stream: bool = False
     max_tokens: int = 256
     temperature: float = 0.7
 
-# TODO: Add post_init function to check if messages are in correct format
 class ChatbotOutput(BaseModel):
+    """Output data for chatbot task"""
     status: bool = True
     data_type: List[str] = Field(default=["data_json", "data_audio"],
                                  description="List of data types",
                                  enum=data_types)
     # data_json: Dict[str, Any] = Field(default=None, description="Text API Output in dictionary", repr=False, exclude=True,)
     # data_audio: str = Field(default=None, description="Audio API Output in base64 format", repr=False, exclude=True,
     #                         example="data:audio/mp3;base64,//tQxA-audio-base64-format-string", )
@@ -173,32 +180,92 @@
         super().__init__(**data)
         self.output['data_json']['text'] = api_text
         self.output['raw_output'] = api_result
         self.output['data_audio'] = api_audio
 
         
 
-
-
 ######################## Task: OCR ######################## TODO: Still in development
+""" ocr = {
+        'input': {
+                'file_type': str,
+                'file': str
+        },
+        'output': {
+                'status': bool,
+                'data_type': [str],
+                'output': {
+                        'data_image': [str]
+                }
+        }
+} """
 
-class OcrInput(BaseModel):
-    text: str
-    file_type: str
-    file: str
 
+class OcrInput(BaseModel):
+    """Input data for OCR task"""
+    file_type: str = Field(..., description="File type image or pdf", example="image/png")
+    file: str = Field(..., description="File in base64 format", example="data:image/png;base64,//tQxA-image-base64-format-string")
 
 class OcrOutput(BaseModel):
-    status: bool
+    """Output data for OCR task"""
+    status: bool = True
     data_type: List[str] = Field(default=["data_image"], description="List of data types", enum=data_types)
     output: Dict[str, Any] = Field(
-        default={"data_image": None},
-        description="Output dictionary",
-        keys={"enum": data_types}
-    )
+                                    default={},
+                                    description="Output dictionary",
+                                    keys={"enum": data_types},
+                                    example={"data_image": ["data:image/png;base64,//tQxA-image-base64-format-string"]}
+                                )
+
+    def __init__(self, model_prediction: Any, data_type: List[str]=["data_image"], **data: Any):
+        super().__init__(**data)
+        self.data_type = data_type
+
+        if "data_image" in self.data_type:
+            self.output['data_image'] = model_prediction
+        elif "data_pdf" in self.data_type:
+            self.output['data_pdf'] = model_prediction
+        else:
+            raise ValueError("Invalid data_type, data_type must be data_image or data_pdf")
+        
+
+
+
+######################## Task: Translation ########################
+
+class TranslationInput(BaseModel):
+    """Input data for translation task"""
+    text: List[str] = Field(..., description="List of texts", example=["This is an example text for translation."])
+    source_language: str = Field(..., description="Source language", example="en")
+    output_language: str = Field(..., description="Output language", example="de")
+
+
+class TranslationOutput(BaseModel):
+    """Output data for translation task"""
+    status: bool = True
+    data_type: List[str] = Field(default=["data_json"], description="List of data types one or more item of data_types", enum=data_types)
+    output: Dict[str, Any] = Field(
+                                    default={"data_json": {"result": {'output_language':None, 'translated_text':None}}},
+                                    description="Output dictionary",
+                                    keys={"enum": data_types},
+                                    example={
+                                            "data_json": {
+                                                            "result": {
+                                                                        "output_language": "<output_language>",
+                                                                        "translated_text": ["<translated_text>"]
+                                                                    }}}
+                                )
+
+    def __init__(self, model_prediction: Any, output_language: str, **data: Any):
+        super().__init__(**data)
+        self.output['data_json']['result']['output_language'] = output_language
+        self.output['data_json']['result']['translated_text'] = model_prediction
+
+
+
 
 
 if __name__ == "__main__":
     from pprint import pprint
 
     # Creating an instance of TextClassificationInput
     input_data = TextClassificationInput(
```

### Comparing `aimped-0.1.45/aimped/model/load.py` & `aimped-0.1.46/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/assertion.py` & `aimped-0.1.46/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/chunker.py` & `aimped-0.1.46/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/deid.py` & `aimped-0.1.46/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/ner.py` & `aimped-0.1.46/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/ner_cls_report.py` & `aimped-0.1.46/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/pipeline.py` & `aimped-0.1.46/aimped/nlp/pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/regex_parser.py` & `aimped-0.1.46/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/relation.py` & `aimped-0.1.46/aimped/nlp/relation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/relation_visualizer.py` & `aimped-0.1.46/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/tokenizer.py` & `aimped-0.1.46/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/tools.py` & `aimped-0.1.46/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/nlp/translation.py` & `aimped-0.1.46/aimped/nlp/translation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/test/test_assertion.py` & `aimped-0.1.46/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/test/test_chunk_merger.py` & `aimped-0.1.46/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/test/test_deid_pipeline.py` & `aimped-0.1.46/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/test/test_ner_results.py` & `aimped-0.1.46/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/test/test_regex_parser.py` & `aimped-0.1.46/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/test/test_relation_pipeline.py` & `aimped-0.1.46/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/test/test_tokenizer.py` & `aimped-0.1.46/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/test/test_translation_pipeline.py` & `aimped-0.1.46/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped/utils.py` & `aimped-0.1.46/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/aimped.egg-info/PKG-INFO` & `aimped-0.1.46/aimped.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aimped
-Version: 0.1.45
+Version: 0.1.46
 Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
 Home-page: https://dev.ml-hub.nioyatechai.com/
 Author: Russell C.
 Author-email: russell@aimped.com
 Maintainer: aimped
 Maintainer-email: contact@aimped.com
 Classifier: Programming Language :: Python :: 3
```

### Comparing `aimped-0.1.45/aimped.egg-info/SOURCES.txt` & `aimped-0.1.46/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aimped-0.1.45/setup.py` & `aimped-0.1.46/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,15 +11,16 @@
     version= __version__,
     packages=setuptools.find_packages(),
     install_requires=[ 
                         'nltk',
                         'numpy',
                         'pandas',
                         'scikit-learn',
-                        "seqeval"
+                        "seqeval",
+                        "pydantic",
                         ],
     author="Russell C.",
     author_email="russell@aimped.com",
     maintainer="aimped",
     maintainer_email="contact@aimped.com",
     description="Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.",
     long_description=open('README.md').read(),
```


# Comparing `tmp/aimped-0.1.42.tar.gz` & `tmp/aimped-0.1.43.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aimped-0.1.42.tar", last modified: Thu May 11 09:15:00 2023, max compression
+gzip compressed data, was "aimped-0.1.43.tar", last modified: Sun May 28 23:22:35 2023, max compression
```

## Comparing `aimped-0.1.42.tar` & `aimped-0.1.43.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/
--rw-rw-r--   0 forest    (1000) forest    (1000)     1063 2023-05-05 13:49:40.000000 aimped-0.1.42/LICENSE
--rw-rw-r--   0 forest    (1000) forest    (1000)     1740 2023-05-11 09:15:00.684665 aimped-0.1.42/PKG-INFO
--rw-rw-r--   0 forest    (1000) forest    (1000)     1170 2023-05-05 13:52:11.000000 aimped-0.1.42/README.md
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.680665 aimped-0.1.42/aimped/
--rw-rw-r--   0 forest    (1000) forest    (1000)      165 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/__init__.py
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/aimped/model/
--rw-rw-r--   0 forest    (1000) forest    (1000)        0 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/model/__init__.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2338 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/model/load.py
--rw-rw-r--   0 forest    (1000) forest    (1000)      502 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/models.py
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/aimped/nitro/
--rw-rw-r--   0 forest    (1000) forest    (1000)        0 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nitro/__init__.py
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/aimped/nlp/
--rw-rw-r--   0 forest    (1000) forest    (1000)      353 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/__init__.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2228 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/assertion.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     3917 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/chunker.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2825 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/deid.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     4521 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/ner.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2629 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/ner_cls_report.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     7231 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/pipeline.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     3899 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/regex_parser.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     4592 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/relation.py
--rw-rw-r--   0 forest    (1000) forest    (1000)    19853 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/relation_visualizer.py
--rw-rw-r--   0 forest    (1000) forest    (1000)      803 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/tokenizer.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2251 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/nlp/tools.py
--rwxrwxrwx   0 forest    (1000) forest    (1000)     2524 2023-05-11 09:11:50.000000 aimped-0.1.42/aimped/nlp/translation.py
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/aimped/test/
--rw-rw-r--   0 forest    (1000) forest    (1000)        0 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/__init__.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2748 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_assertion.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     1313 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_chunk_merger.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     1866 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_deid_pipeline.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     1297 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_ner_results.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     1592 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_regex_parser.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     3320 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_relation_pipeline.py
--rw-rw-r--   0 forest    (1000) forest    (1000)      610 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_tokenizer.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     5585 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/test/test_translation_pipeline.py
--rw-rw-r--   0 forest    (1000) forest    (1000)     2056 2023-05-05 13:49:40.000000 aimped-0.1.42/aimped/utils.py
--rw-rw-r--   0 forest    (1000) forest    (1000)      123 2023-05-11 09:13:14.000000 aimped-0.1.42/aimped/version.py
-drwxrwxr-x   0 forest    (1000) forest    (1000)        0 2023-05-11 09:15:00.684665 aimped-0.1.42/aimped.egg-info/
--rw-rw-r--   0 forest    (1000) forest    (1000)     1740 2023-05-11 09:15:00.000000 aimped-0.1.42/aimped.egg-info/PKG-INFO
--rw-rw-r--   0 forest    (1000) forest    (1000)      933 2023-05-11 09:15:00.000000 aimped-0.1.42/aimped.egg-info/SOURCES.txt
--rw-rw-r--   0 forest    (1000) forest    (1000)        1 2023-05-11 09:15:00.000000 aimped-0.1.42/aimped.egg-info/dependency_links.txt
--rw-rw-r--   0 forest    (1000) forest    (1000)       39 2023-05-11 09:15:00.000000 aimped-0.1.42/aimped.egg-info/requires.txt
--rw-rw-r--   0 forest    (1000) forest    (1000)        7 2023-05-11 09:15:00.000000 aimped-0.1.42/aimped.egg-info/top_level.txt
--rw-rw-r--   0 forest    (1000) forest    (1000)      103 2023-05-11 09:15:00.684665 aimped-0.1.42/setup.cfg
--rw-rw-r--   0 forest    (1000) forest    (1000)     1139 2023-05-05 13:49:40.000000 aimped-0.1.42/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.390569 aimped-0.1.43/
+-rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.43/LICENSE
+-rw-rw-rw-   0        0        0     1791 2023-05-28 23:22:35.391131 aimped-0.1.43/PKG-INFO
+-rw-rw-rw-   0        0        0     1205 2023-05-24 09:20:26.000000 aimped-0.1.43/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.334471 aimped-0.1.43/aimped/
+-rw-rw-rw-   0        0        0      193 2023-05-26 14:08:03.000000 aimped-0.1.43/aimped/__init__.py
+-rw-rw-rw-   0        0        0     8553 2023-05-28 23:20:53.000000 aimped-0.1.43/aimped/io_tasks.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.346225 aimped-0.1.43/aimped/model/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/model/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/model/load.py
+-rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/models.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.347865 aimped-0.1.43/aimped/nitro/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nitro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.367879 aimped-0.1.43/aimped/nlp/
+-rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/assertion.py
+-rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/chunker.py
+-rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/deid.py
+-rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/ner.py
+-rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/ner_cls_report.py
+-rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/pipeline.py
+-rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/regex_parser.py
+-rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.43/aimped/nlp/relation.py
+-rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.43/aimped/nlp/relation_visualizer.py
+-rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/tokenizer.py
+-rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/nlp/tools.py
+-rw-rw-rw-   0        0        0     2587 2023-05-24 09:15:05.000000 aimped-0.1.43/aimped/nlp/translation.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.388335 aimped-0.1.43/aimped/test/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/__init__.py
+-rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_assertion.py
+-rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_chunk_merger.py
+-rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_deid_pipeline.py
+-rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_ner_results.py
+-rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_regex_parser.py
+-rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_relation_pipeline.py
+-rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_tokenizer.py
+-rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/test/test_translation_pipeline.py
+-rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.43/aimped/utils.py
+-rw-rw-rw-   0        0        0      130 2023-05-28 23:20:53.000000 aimped-0.1.43/aimped/version.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:22:35.343428 aimped-0.1.43/aimped.egg-info/
+-rw-rw-rw-   0        0        0     1791 2023-05-28 23:22:35.000000 aimped-0.1.43/aimped.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-05-28 23:22:35.000000 aimped-0.1.43/aimped.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:22:35.000000 aimped-0.1.43/aimped.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-28 23:22:35.000000 aimped-0.1.43/aimped.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 23:22:35.000000 aimped-0.1.43/aimped.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-28 23:22:35.393459 aimped-0.1.43/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2023-04-03 13:18:42.000000 aimped-0.1.43/setup.py
```

### Comparing `aimped-0.1.42/LICENSE` & `aimped-0.1.43/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/PKG-INFO` & `aimped-0.1.43/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-Metadata-Version: 2.1
-Name: aimped
-Version: 0.1.42
-Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.ml-hub.nioyatechai.com/
-Author: Russell C.
-Author-email: russell@aimped.com
-Maintainer: aimped
-Maintainer-email: contact@aimped.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **aimped**
-![aimped](https://dev.ml-hub.nioyatechai.com/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
+Metadata-Version: 2.1
+Name: aimped
+Version: 0.1.43
+Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
+Home-page: https://dev.ml-hub.nioyatechai.com/
+Author: Russell C.
+Author-email: russell@aimped.com
+Maintainer: aimped
+Maintainer-email: contact@aimped.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
```

### Comparing `aimped-0.1.42/README.md` & `aimped-0.1.43/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# **aimped**
-![aimped](https://dev.ml-hub.nioyatechai.com/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
```

### Comparing `aimped-0.1.42/aimped/model/load.py` & `aimped-0.1.43/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/assertion.py` & `aimped-0.1.43/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/chunker.py` & `aimped-0.1.43/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/deid.py` & `aimped-0.1.43/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/ner.py` & `aimped-0.1.43/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/ner_cls_report.py` & `aimped-0.1.43/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/pipeline.py` & `aimped-0.1.43/aimped/nlp/pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/regex_parser.py` & `aimped-0.1.43/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/relation.py` & `aimped-0.1.43/aimped/nlp/relation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/relation_visualizer.py` & `aimped-0.1.43/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/tokenizer.py` & `aimped-0.1.43/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/nlp/tools.py` & `aimped-0.1.43/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/test/test_assertion.py` & `aimped-0.1.43/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/test/test_chunk_merger.py` & `aimped-0.1.43/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/test/test_deid_pipeline.py` & `aimped-0.1.43/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/test/test_ner_results.py` & `aimped-0.1.43/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/test/test_regex_parser.py` & `aimped-0.1.43/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/test/test_relation_pipeline.py` & `aimped-0.1.43/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/test/test_tokenizer.py` & `aimped-0.1.43/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/test/test_translation_pipeline.py` & `aimped-0.1.43/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped/utils.py` & `aimped-0.1.43/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.42/aimped.egg-info/PKG-INFO` & `aimped-0.1.43/aimped.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-Metadata-Version: 2.1
-Name: aimped
-Version: 0.1.42
-Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.ml-hub.nioyatechai.com/
-Author: Russell C.
-Author-email: russell@aimped.com
-Maintainer: aimped
-Maintainer-email: contact@aimped.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **aimped**
-![aimped](https://dev.ml-hub.nioyatechai.com/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-
+Metadata-Version: 2.1
+Name: aimped
+Version: 0.1.43
+Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
+Home-page: https://dev.ml-hub.nioyatechai.com/
+Author: Russell C.
+Author-email: russell@aimped.com
+Maintainer: aimped
+Maintainer-email: contact@aimped.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **aimped**
+![aimped](https://dev.aimped.ai/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+
```

### Comparing `aimped-0.1.42/aimped.egg-info/SOURCES.txt` & `aimped-0.1.43/aimped.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.cfg
 setup.py
 aimped/__init__.py
+aimped/io_tasks.py
 aimped/models.py
 aimped/utils.py
 aimped/version.py
 aimped.egg-info/PKG-INFO
 aimped.egg-info/SOURCES.txt
 aimped.egg-info/dependency_links.txt
 aimped.egg-info/requires.txt
```

### Comparing `aimped-0.1.42/setup.py` & `aimped-0.1.43/setup.py`

 * *Files identical despite different names*


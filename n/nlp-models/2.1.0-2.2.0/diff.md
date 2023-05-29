# Comparing `tmp/nlp-models-2.1.0.tar.gz` & `tmp/nlp-models-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlp-models-2.1.0.tar", last modified: Sun May 28 20:27:34 2023, max compression
+gzip compressed data, was "nlp-models-2.2.0.tar", last modified: Mon May 29 08:56:40 2023, max compression
```

## Comparing `nlp-models-2.1.0.tar` & `nlp-models-2.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:34.219632 nlp-models-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-28 20:27:19.000000 nlp-models-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-28 20:27:34.219632 nlp-models-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-28 20:27:19.000000 nlp-models-2.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-28 20:27:19.000000 nlp-models-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-28 20:27:34.219632 nlp-models-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 20:27:19.000000 nlp-models-2.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:34.215632 nlp-models-2.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:34.215632 nlp-models-2.1.0/src/bert_classifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:19.000000 nlp-models-2.1.0/src/bert_classifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-28 20:27:19.000000 nlp-models-2.1.0/src/bert_classifier/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-28 20:27:19.000000 nlp-models-2.1.0/src/bert_classifier/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/bert_classifier/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/bert_classifier/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/bert_classifier/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/bert_classifier/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:34.219632 nlp-models-2.1.0/src/multi_task_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/mtl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-28 20:27:20.000000 nlp-models-2.1.0/src/multi_task_model/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 20:27:34.219632 nlp-models-2.1.0/src/nlp_models.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-28 20:27:34.000000 nlp-models-2.1.0/src/nlp_models.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-28 20:27:34.000000 nlp-models-2.1.0/src/nlp_models.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 20:27:34.000000 nlp-models-2.1.0/src/nlp_models.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-28 20:27:34.000000 nlp-models-2.1.0/src/nlp_models.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 20:27:34.000000 nlp-models-2.1.0/src/nlp_models.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:40.389879 nlp-models-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-29 08:56:28.000000 nlp-models-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-29 08:56:40.389879 nlp-models-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-29 08:56:28.000000 nlp-models-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-29 08:56:28.000000 nlp-models-2.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-29 08:56:40.389879 nlp-models-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 08:56:28.000000 nlp-models-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:40.385878 nlp-models-2.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:40.389879 nlp-models-2.2.0/src/bert_classifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/bert_classifier/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:40.389879 nlp-models-2.2.0/src/multi_task_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/mtl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9589 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-29 08:56:28.000000 nlp-models-2.2.0/src/multi_task_model/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:56:40.389879 nlp-models-2.2.0/src/nlp_models.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-29 08:56:40.000000 nlp-models-2.2.0/src/nlp_models.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-29 08:56:40.000000 nlp-models-2.2.0/src/nlp_models.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:56:40.000000 nlp-models-2.2.0/src/nlp_models.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 08:56:40.000000 nlp-models-2.2.0/src/nlp_models.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 08:56:40.000000 nlp-models-2.2.0/src/nlp_models.egg-info/top_level.txt
```

### Comparing `nlp-models-2.1.0/LICENSE` & `nlp-models-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/PKG-INFO` & `nlp-models-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.1.0
+Version: 2.2.0
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-2.1.0/README.md` & `nlp-models-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/setup.cfg` & `nlp-models-2.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = nlp-models
-version = 2.1.0
+version = 2.2.0
 author = Ming Gao
 author_email = ming_gao@outlook.com
 url = https://github.com/minggnim/nlp-models
 description = Transformers based NLP models
 long_description = file: README.md
 long_description_content_type = text/markdown
 classifiers =
```

### Comparing `nlp-models-2.1.0/src/bert_classifier/bert.py` & `nlp-models-2.2.0/src/bert_classifier/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/src/bert_classifier/data.py` & `nlp-models-2.2.0/src/bert_classifier/data.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/src/bert_classifier/io.py` & `nlp-models-2.2.0/src/bert_classifier/io.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/src/bert_classifier/metrics.py` & `nlp-models-2.2.0/src/bert_classifier/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/src/bert_classifier/predict.py` & `nlp-models-2.2.0/src/bert_classifier/predict.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/src/bert_classifier/train.py` & `nlp-models-2.2.0/src/bert_classifier/train.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/src/multi_task_model/layers.py` & `nlp-models-2.2.0/src/multi_task_model/layers.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/src/multi_task_model/metrics.py` & `nlp-models-2.2.0/src/multi_task_model/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/src/multi_task_model/mtl.py` & `nlp-models-2.2.0/src/multi_task_model/mtl.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,25 +35,25 @@
         return model_output[0][:,0]
     
     @staticmethod
     def save_model(model, dir):
         torch.save(model, dir)
 
     @staticmethod
-    def load_model(dir):
-        return torch.load(dir)
+    def load_model(dir, device=torch.device('cpu')):
+        return torch.load(dir, device)
 
 
 class MTLInference:
-    def __init__(self, tokenizer_card, model_card, num_labels=None, pretrained_model=True) -> None:
+    def __init__(self, tokenizer_card, model_card, num_labels=None, pretrained_model=True, device=torch.device('cpu')) -> None:
         self.tokenizer = transformers.AutoTokenizer.from_pretrained(tokenizer_card)
         if pretrained_model:
             self.mtl_model = AutoModelForMTL(model_card, num_labels)
         else:
-            self.mtl_model = AutoModelForMTL.load_model(model_card)
+            self.mtl_model = AutoModelForMTL.load_model(model_card, device)
         self.mtl_model.eval()
 
     def encode(self, inputs):
         return self.tokenizer(inputs, return_tensors='pt', padding=True)
 
     def predict(self, query):
         with torch.no_grad():
```

### Comparing `nlp-models-2.1.0/src/multi_task_model/trainer.py` & `nlp-models-2.2.0/src/multi_task_model/trainer.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/src/multi_task_model/utils.py` & `nlp-models-2.2.0/src/multi_task_model/utils.py`

 * *Files identical despite different names*

### Comparing `nlp-models-2.1.0/src/nlp_models.egg-info/PKG-INFO` & `nlp-models-2.2.0/src/nlp_models.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-models
-Version: 2.1.0
+Version: 2.2.0
 Summary: Transformers based NLP models
 Home-page: https://github.com/minggnim/nlp-models
 Author: Ming Gao
 Author-email: ming_gao@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `nlp-models-2.1.0/src/nlp_models.egg-info/SOURCES.txt` & `nlp-models-2.2.0/src/nlp_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*


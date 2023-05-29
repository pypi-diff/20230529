# Comparing `tmp/adaptor-0.2.1.tar.gz` & `tmp/adaptor-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adaptor-0.2.1.tar", last modified: Wed Mar 22 08:46:01 2023, max compression
+gzip compressed data, was "adaptor-0.2.2.tar", last modified: Mon May 29 19:57:56 2023, max compression
```

## Comparing `adaptor-0.2.1.tar` & `adaptor-0.2.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-03-22 08:46:01.019406 adaptor-0.2.1/
--rw-r--r--   0 xstefan3   (501) staff       (20)      202 2022-07-29 08:31:53.000000 adaptor-0.2.1/.gitignore
--rw-r--r--   0 xstefan3   (501) staff       (20)     1086 2022-04-27 08:43:57.000000 adaptor-0.2.1/LICENSE
--rw-r--r--   0 xstefan3   (501) staff       (20)    12449 2023-03-22 08:46:01.019677 adaptor-0.2.1/PKG-INFO
--rw-r--r--   0 xstefan3   (501) staff       (20)    11748 2022-07-29 08:06:21.000000 adaptor-0.2.1/README.md
-drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-03-22 08:46:01.008583 adaptor-0.2.1/adaptor/
--rw-r--r--   0 xstefan3   (501) staff       (20)        0 2022-01-31 14:03:17.000000 adaptor-0.2.1/adaptor/__init__.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     6122 2022-07-29 08:06:21.000000 adaptor-0.2.1/adaptor/adapter.py
-drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-03-22 08:46:01.011897 adaptor-0.2.1/adaptor/evaluators/
--rw-r--r--   0 xstefan3   (501) staff       (20)        0 2022-01-24 21:13:53.000000 adaptor-0.2.1/adaptor/evaluators/__init__.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     1927 2022-02-17 11:47:50.000000 adaptor-0.2.1/adaptor/evaluators/evaluator_base.py
--rw-r--r--   0 xstefan3   (501) staff       (20)    12373 2022-02-17 11:47:50.000000 adaptor-0.2.1/adaptor/evaluators/generative.py
--rw-r--r--   0 xstefan3   (501) staff       (20)    20650 2022-01-31 14:03:17.000000 adaptor-0.2.1/adaptor/evaluators/prism.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     4119 2022-08-08 14:38:29.000000 adaptor-0.2.1/adaptor/evaluators/question_answering.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     1245 2022-02-17 11:47:50.000000 adaptor-0.2.1/adaptor/evaluators/sequence_classification.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     3068 2022-07-29 08:06:21.000000 adaptor-0.2.1/adaptor/evaluators/token_classification.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     9711 2022-09-23 12:20:35.000000 adaptor-0.2.1/adaptor/lang_module.py
-drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-03-22 08:46:01.015243 adaptor-0.2.1/adaptor/objectives/
--rw-r--r--   0 xstefan3   (501) staff       (20)     5549 2022-07-20 14:50:08.000000 adaptor-0.2.1/adaptor/objectives/CLM.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     3686 2023-03-20 14:52:59.000000 adaptor-0.2.1/adaptor/objectives/MLM.py
--rw-r--r--   0 xstefan3   (501) staff       (20)        0 2022-01-24 21:13:53.000000 adaptor-0.2.1/adaptor/objectives/__init__.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     5599 2022-02-10 17:32:33.000000 adaptor-0.2.1/adaptor/objectives/backtranslation.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     8426 2023-03-20 14:52:59.000000 adaptor-0.2.1/adaptor/objectives/classification.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     5876 2022-02-10 08:19:10.000000 adaptor-0.2.1/adaptor/objectives/denoising.py
--rw-r--r--   0 xstefan3   (501) staff       (20)    10985 2022-09-23 12:20:35.000000 adaptor-0.2.1/adaptor/objectives/distillation.py
--rw-r--r--   0 xstefan3   (501) staff       (20)    30195 2023-03-22 08:45:02.000000 adaptor-0.2.1/adaptor/objectives/objective_base.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     3701 2022-07-29 08:06:21.000000 adaptor-0.2.1/adaptor/objectives/question_answering.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     6027 2023-03-20 14:52:59.000000 adaptor-0.2.1/adaptor/objectives/seq2seq.py
--rw-r--r--   0 xstefan3   (501) staff       (20)    15228 2022-08-08 14:38:29.000000 adaptor-0.2.1/adaptor/schedules.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     4264 2022-07-29 08:06:21.000000 adaptor-0.2.1/adaptor/utils.py
-drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-03-22 08:46:01.009426 adaptor-0.2.1/adaptor.egg-info/
--rw-r--r--   0 xstefan3   (501) staff       (20)    12449 2023-03-22 08:46:00.000000 adaptor-0.2.1/adaptor.egg-info/PKG-INFO
--rw-r--r--   0 xstefan3   (501) staff       (20)     1120 2023-03-22 08:46:00.000000 adaptor-0.2.1/adaptor.egg-info/SOURCES.txt
--rw-r--r--   0 xstefan3   (501) staff       (20)        1 2023-03-22 08:46:00.000000 adaptor-0.2.1/adaptor.egg-info/dependency_links.txt
--rw-r--r--   0 xstefan3   (501) staff       (20)      147 2023-03-22 08:46:00.000000 adaptor-0.2.1/adaptor.egg-info/requires.txt
--rw-r--r--   0 xstefan3   (501) staff       (20)        8 2023-03-22 08:46:00.000000 adaptor-0.2.1/adaptor.egg-info/top_level.txt
--rw-r--r--   0 xstefan3   (501) staff       (20)        1 2022-01-26 12:37:19.000000 adaptor-0.2.1/adaptor.egg-info/zip-safe
--rw-r--r--   0 xstefan3   (501) staff       (20)      297 2022-01-24 21:13:53.000000 adaptor-0.2.1/dockerfile.in
-drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-03-22 08:46:01.015514 adaptor-0.2.1/docs/
--rw-r--r--   0 xstefan3   (501) staff       (20)   103706 2022-01-24 21:13:53.000000 adaptor-0.2.1/docs/user_flow.png
--rw-r--r--   0 xstefan3   (501) staff       (20)      348 2023-03-22 08:46:01.020229 adaptor-0.2.1/setup.cfg
--rw-r--r--   0 xstefan3   (501) staff       (20)     1465 2023-03-22 08:45:02.000000 adaptor-0.2.1/setup.py
-drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-03-22 08:46:01.019200 adaptor-0.2.1/tests/
--rw-r--r--   0 xstefan3   (501) staff       (20)     3516 2022-02-10 17:32:33.000000 adaptor-0.2.1/tests/adapter_test.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     7009 2023-03-20 14:52:59.000000 adaptor-0.2.1/tests/end2end_usecases_test.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     7264 2022-07-29 08:06:21.000000 adaptor-0.2.1/tests/evaluators_test.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     1834 2022-02-10 08:05:33.000000 adaptor-0.2.1/tests/lang_module_test.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     5756 2022-09-23 12:20:35.000000 adaptor-0.2.1/tests/objectives_test.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     6260 2022-05-03 12:19:33.000000 adaptor-0.2.1/tests/schedules_test.py
--rw-r--r--   0 xstefan3   (501) staff       (20)     1656 2023-03-20 14:52:59.000000 adaptor-0.2.1/tests/utils.py
+drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-05-29 19:57:56.119542 adaptor-0.2.2/
+-rw-r--r--   0 xstefan3   (501) staff       (20)      202 2022-07-29 08:31:53.000000 adaptor-0.2.2/.gitignore
+-rw-r--r--   0 xstefan3   (501) staff       (20)     1086 2022-04-27 08:43:57.000000 adaptor-0.2.2/LICENSE
+-rw-r--r--   0 xstefan3   (501) staff       (20)    12449 2023-05-29 19:57:56.119750 adaptor-0.2.2/PKG-INFO
+-rw-r--r--   0 xstefan3   (501) staff       (20)    11748 2023-05-29 10:25:30.000000 adaptor-0.2.2/README.md
+drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-05-29 19:57:56.109848 adaptor-0.2.2/adaptor/
+-rw-r--r--   0 xstefan3   (501) staff       (20)        0 2022-01-31 14:03:17.000000 adaptor-0.2.2/adaptor/__init__.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     6122 2022-07-29 08:06:21.000000 adaptor-0.2.2/adaptor/adapter.py
+drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-05-29 19:57:56.112706 adaptor-0.2.2/adaptor/evaluators/
+-rw-r--r--   0 xstefan3   (501) staff       (20)        0 2022-01-24 21:13:53.000000 adaptor-0.2.2/adaptor/evaluators/__init__.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     1927 2022-02-17 11:47:50.000000 adaptor-0.2.2/adaptor/evaluators/evaluator_base.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)    12373 2022-02-17 11:47:50.000000 adaptor-0.2.2/adaptor/evaluators/generative.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)    20650 2022-01-31 14:03:17.000000 adaptor-0.2.2/adaptor/evaluators/prism.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     4119 2022-08-08 14:38:29.000000 adaptor-0.2.2/adaptor/evaluators/question_answering.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     1245 2022-02-17 11:47:50.000000 adaptor-0.2.2/adaptor/evaluators/sequence_classification.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     3068 2022-07-29 08:06:21.000000 adaptor-0.2.2/adaptor/evaluators/token_classification.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     9941 2023-05-29 10:27:35.000000 adaptor-0.2.2/adaptor/lang_module.py
+drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-05-29 19:57:56.115683 adaptor-0.2.2/adaptor/objectives/
+-rw-r--r--   0 xstefan3   (501) staff       (20)     5549 2022-07-20 14:50:08.000000 adaptor-0.2.2/adaptor/objectives/CLM.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     3686 2023-03-20 14:52:59.000000 adaptor-0.2.2/adaptor/objectives/MLM.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)        0 2022-01-24 21:13:53.000000 adaptor-0.2.2/adaptor/objectives/__init__.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     5599 2022-02-10 17:32:33.000000 adaptor-0.2.2/adaptor/objectives/backtranslation.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     8426 2023-03-20 14:52:59.000000 adaptor-0.2.2/adaptor/objectives/classification.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     5876 2022-02-10 08:19:10.000000 adaptor-0.2.2/adaptor/objectives/denoising.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)    10985 2022-09-23 12:20:35.000000 adaptor-0.2.2/adaptor/objectives/distillation.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)    30195 2023-03-22 08:45:02.000000 adaptor-0.2.2/adaptor/objectives/objective_base.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     3701 2022-07-29 08:06:21.000000 adaptor-0.2.2/adaptor/objectives/question_answering.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     6027 2023-03-20 14:52:59.000000 adaptor-0.2.2/adaptor/objectives/seq2seq.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)    15228 2022-08-08 14:38:29.000000 adaptor-0.2.2/adaptor/schedules.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     4264 2022-07-29 08:06:21.000000 adaptor-0.2.2/adaptor/utils.py
+drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-05-29 19:57:56.110880 adaptor-0.2.2/adaptor.egg-info/
+-rw-r--r--   0 xstefan3   (501) staff       (20)    12449 2023-05-29 19:57:55.000000 adaptor-0.2.2/adaptor.egg-info/PKG-INFO
+-rw-r--r--   0 xstefan3   (501) staff       (20)     1120 2023-05-29 19:57:55.000000 adaptor-0.2.2/adaptor.egg-info/SOURCES.txt
+-rw-r--r--   0 xstefan3   (501) staff       (20)        1 2023-05-29 19:57:55.000000 adaptor-0.2.2/adaptor.egg-info/dependency_links.txt
+-rw-r--r--   0 xstefan3   (501) staff       (20)      148 2023-05-29 19:57:55.000000 adaptor-0.2.2/adaptor.egg-info/requires.txt
+-rw-r--r--   0 xstefan3   (501) staff       (20)        8 2023-05-29 19:57:55.000000 adaptor-0.2.2/adaptor.egg-info/top_level.txt
+-rw-r--r--   0 xstefan3   (501) staff       (20)        1 2022-01-26 12:37:19.000000 adaptor-0.2.2/adaptor.egg-info/zip-safe
+-rw-r--r--   0 xstefan3   (501) staff       (20)      297 2022-01-24 21:13:53.000000 adaptor-0.2.2/dockerfile.in
+drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-05-29 19:57:56.116012 adaptor-0.2.2/docs/
+-rw-r--r--   0 xstefan3   (501) staff       (20)   103706 2022-01-24 21:13:53.000000 adaptor-0.2.2/docs/user_flow.png
+-rw-r--r--   0 xstefan3   (501) staff       (20)      348 2023-05-29 19:57:56.122597 adaptor-0.2.2/setup.cfg
+-rw-r--r--   0 xstefan3   (501) staff       (20)     1466 2023-05-29 19:56:25.000000 adaptor-0.2.2/setup.py
+drwxr-xr-x   0 xstefan3   (501) staff       (20)        0 2023-05-29 19:57:56.119321 adaptor-0.2.2/tests/
+-rw-r--r--   0 xstefan3   (501) staff       (20)     3516 2022-02-10 17:32:33.000000 adaptor-0.2.2/tests/adapter_test.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     7009 2023-03-20 14:52:59.000000 adaptor-0.2.2/tests/end2end_usecases_test.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     7264 2022-07-29 08:06:21.000000 adaptor-0.2.2/tests/evaluators_test.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     1834 2022-02-10 08:05:33.000000 adaptor-0.2.2/tests/lang_module_test.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     5756 2022-09-23 12:20:35.000000 adaptor-0.2.2/tests/objectives_test.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     6260 2022-05-03 12:19:33.000000 adaptor-0.2.2/tests/schedules_test.py
+-rw-r--r--   0 xstefan3   (501) staff       (20)     1656 2023-03-20 14:52:59.000000 adaptor-0.2.2/tests/utils.py
```

### Comparing `adaptor-0.2.1/LICENSE` & `adaptor-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/PKG-INFO` & `adaptor-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptor
-Version: 0.2.1
+Version: 0.2.2
 Summary: Adaptor: Objective-centric Adaptation Framework for Language Models.
 Home-page: https://github.com/gaussalgo/adaptor
 Author: Michal Stefanik & Adaptor Authors & Contributors
 Author-email: stefanik.m@mail.muni.cz
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `adaptor-0.2.1/README.md` & `adaptor-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/adapter.py` & `adaptor-0.2.2/adaptor/adapter.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/evaluators/evaluator_base.py` & `adaptor-0.2.2/adaptor/evaluators/evaluator_base.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/evaluators/generative.py` & `adaptor-0.2.2/adaptor/evaluators/generative.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/evaluators/prism.py` & `adaptor-0.2.2/adaptor/evaluators/prism.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/evaluators/question_answering.py` & `adaptor-0.2.2/adaptor/evaluators/question_answering.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/evaluators/sequence_classification.py` & `adaptor-0.2.2/adaptor/evaluators/sequence_classification.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/evaluators/token_classification.py` & `adaptor-0.2.2/adaptor/evaluators/token_classification.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/lang_module.py` & `adaptor-0.2.2/adaptor/lang_module.py`

 * *Files 9% similar despite different names*

```diff
@@ -179,7 +179,12 @@
                     if hasattr(m_child, "reset_parameters"):
                         m_child.reset_parameters()
                     reinit_model_weights(m_child)
 
         torch.manual_seed(seed)
         for head, head_model in self.trainable_models.items():
             head_model.apply(reinit_model_weights)
+
+    def gradient_checkpointing_enable(self):
+        for module_id, module in self.trainable_models.items():
+            if hasattr(module, "gradient_checkpointing_enable"):
+                module.gradient_checkpointing_enable()
```

### Comparing `adaptor-0.2.1/adaptor/objectives/CLM.py` & `adaptor-0.2.2/adaptor/objectives/CLM.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/objectives/MLM.py` & `adaptor-0.2.2/adaptor/objectives/MLM.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/objectives/backtranslation.py` & `adaptor-0.2.2/adaptor/objectives/backtranslation.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/objectives/classification.py` & `adaptor-0.2.2/adaptor/objectives/classification.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/objectives/denoising.py` & `adaptor-0.2.2/adaptor/objectives/denoising.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/objectives/distillation.py` & `adaptor-0.2.2/adaptor/objectives/distillation.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/objectives/objective_base.py` & `adaptor-0.2.2/adaptor/objectives/objective_base.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/objectives/question_answering.py` & `adaptor-0.2.2/adaptor/objectives/question_answering.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/objectives/seq2seq.py` & `adaptor-0.2.2/adaptor/objectives/seq2seq.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/schedules.py` & `adaptor-0.2.2/adaptor/schedules.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor/utils.py` & `adaptor-0.2.2/adaptor/utils.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/adaptor.egg-info/PKG-INFO` & `adaptor-0.2.2/adaptor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adaptor
-Version: 0.2.1
+Version: 0.2.2
 Summary: Adaptor: Objective-centric Adaptation Framework for Language Models.
 Home-page: https://github.com/gaussalgo/adaptor
 Author: Michal Stefanik & Adaptor Authors & Contributors
 Author-email: stefanik.m@mail.muni.cz
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `adaptor-0.2.1/adaptor.egg-info/SOURCES.txt` & `adaptor-0.2.2/adaptor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/docs/user_flow.png` & `adaptor-0.2.2/docs/user_flow.png`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/setup.py` & `adaptor-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     readme = fh.read()
 
 
 setup(
     name="adaptor",
-    version='0.2.1',
+    version='0.2.2',
     description="Adaptor: Objective-centric Adaptation Framework for Language Models.",
     long_description_content_type="text/markdown",
     long_description=readme,
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Education",
         "Intended Audience :: Science/Research",
@@ -26,15 +26,15 @@
     python_requires=">=3.7",
     license="MIT",
     packages=find_packages(include=["adaptor", "adaptor.*"]),
     include_package_data=True,
     zip_safe=True,
     install_requires=[
         "torch>=1.7",
-        "transformers>=4.10.2<=4.19.1",  # upper-closed on 4.19.1 for now, due to minor bug in eval loss logging
+        "transformers>=4.10.2,<=4.19.1",  # upper-closed on 4.19.1 for now, due to minor bug in eval loss logging
         "sentencepiece",
     ],
     test_require=[
         "pytest"
     ],
     extras_require={
         "generative": [
```

### Comparing `adaptor-0.2.1/tests/adapter_test.py` & `adaptor-0.2.2/tests/adapter_test.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/tests/end2end_usecases_test.py` & `adaptor-0.2.2/tests/end2end_usecases_test.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/tests/evaluators_test.py` & `adaptor-0.2.2/tests/evaluators_test.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/tests/lang_module_test.py` & `adaptor-0.2.2/tests/lang_module_test.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/tests/objectives_test.py` & `adaptor-0.2.2/tests/objectives_test.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/tests/schedules_test.py` & `adaptor-0.2.2/tests/schedules_test.py`

 * *Files identical despite different names*

### Comparing `adaptor-0.2.1/tests/utils.py` & `adaptor-0.2.2/tests/utils.py`

 * *Files identical despite different names*


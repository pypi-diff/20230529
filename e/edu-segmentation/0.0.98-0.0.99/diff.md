# Comparing `tmp/edu-segmentation-0.0.98.tar.gz` & `tmp/edu_segmentation-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu-segmentation-0.0.98.tar", last modified: Mon May 29 11:09:40 2023, max compression
+gzip compressed data, was "edu_segmentation-0.0.99.tar", max compression
```

## Comparing `edu-segmentation-0.0.98.tar` & `edu_segmentation-0.0.99.tar`

### file list

```diff
@@ -1,37 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.340275 edu-segmentation-0.0.98/
--rw-rw-rw-   0        0        0      178 2023-05-29 11:09:40.340275 edu-segmentation-0.0.98/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.263271 edu-segmentation-0.0.98/edu_segmentation/
-drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.305271 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/
--rw-rw-rw-   0        0        0      325 2023-04-27 10:53:24.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
--rw-rw-rw-   0        0        0      298 2023-04-27 10:53:24.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/config.py
--rw-rw-rw-   0        0        0     3930 2023-04-28 12:33:56.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/import_data_bart.py
--rw-rw-rw-   0        0        0    12186 2023-04-27 10:53:24.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model.py
-drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.309270 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model_dependencies/
--rw-rw-rw-   0        0        0    11216 2023-04-27 10:53:24.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py
--rw-rw-rw-   0        0        0     1510 2023-04-28 12:35:01.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py
--rw-rw-rw-   0        0        0     4364 2023-04-28 16:04:21.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/run_segbot.py
--rw-rw-rw-   0        0        0     7480 2023-05-26 09:43:38.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
--rw-rw-rw-   0        0        0     8974 2023-04-27 10:53:24.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/solver.py
--rw-rw-rw-   0        0        0    10912 2023-05-25 11:53:51.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/solver_bart.py
-drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.338271 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/
--rw-rw-rw-   0        0        0      231 2023-04-27 10:53:25.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/config.py
--rw-rw-rw-   0        0        0     4322 2023-05-26 08:19:05.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/import_data_bert.py
--rw-rw-rw-   0        0        0     4883 2023-05-26 08:18:45.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
--rw-rw-rw-   0        0        0     3313 2023-05-26 08:19:16.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/postagging.py
--rw-rw-rw-   0        0        0     3227 2023-05-26 08:19:11.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/postagging_new.py
--rw-rw-rw-   0        0        0    85404 2023-04-27 10:53:26.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
--rw-rw-rw-   0        0        0     6168 2023-05-26 11:39:49.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/run_bert.py
--rw-rw-rw-   0        0        0     6410 2023-05-26 08:19:56.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/solver.py
--rw-rw-rw-   0        0        0     6979 2023-05-26 08:19:44.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/solver_postag.py
--rw-rw-rw-   0        0        0      537 2023-04-27 10:53:26.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/test_model.py
--rw-rw-rw-   0        0        0     1025 2023-05-26 08:20:25.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/train_model.py
--rw-rw-rw-   0        0        0     1315 2023-05-26 08:20:17.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-rw-rw-   0        0        0     1885 2023-05-29 09:01:51.000000 edu-segmentation-0.0.98/edu_segmentation/main.py
-drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.281273 edu-segmentation-0.0.98/edu_segmentation.egg-info/
--rw-rw-rw-   0        0        0      178 2023-05-29 11:09:40.000000 edu-segmentation-0.0.98/edu_segmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1530 2023-05-29 11:09:40.000000 edu-segmentation-0.0.98/edu_segmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 11:09:40.000000 edu-segmentation-0.0.98/edu_segmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1221 2023-05-29 11:09:40.000000 edu-segmentation-0.0.98/edu_segmentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-29 11:09:40.000000 edu-segmentation-0.0.98/edu_segmentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 11:09:40.341273 edu-segmentation-0.0.98/setup.cfg
--rw-rw-rw-   0        0        0     6463 2023-05-29 11:09:35.000000 edu-segmentation-0.0.98/setup.py
+-rw-r--r--   0        0        0      613 2023-05-26 08:17:47.941910 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     5783 2023-05-26 08:17:50.553203 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/__pycache__/import_data_bart.cpython-311.pyc
+-rw-r--r--   0        0        0     7833 2023-05-26 08:17:46.311741 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/__pycache__/run_segbot_bart.cpython-311.pyc
+-rw-r--r--   0        0        0    14804 2023-05-26 08:17:50.841087 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/__pycache__/solver_bart.cpython-311.pyc
+-rw-r--r--   0        0        0      325 2023-04-27 10:53:24.371538 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
+-rw-r--r--   0        0        0      298 2023-04-27 10:53:24.434065 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/config.py
+-rw-r--r--   0        0        0     3930 2023-04-28 12:33:56.340151 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/import_data_bart.py
+-rw-r--r--   0        0        0    12186 2023-04-27 10:53:24.480926 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/model.py
+-rw-r--r--   0        0        0   590031 2023-04-27 10:53:24.340305 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/model_dependencies/all_vocabulary.pickle
+-rw-r--r--   0        0        0    11216 2023-04-27 10:53:24.512189 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py
+-rw-r--r--   0        0        0     1510 2023-04-28 12:35:01.251942 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py
+-rw-r--r--   0        0        0     4364 2023-04-28 16:04:21.009998 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/run_segbot.py
+-rw-r--r--   0        0        0     7480 2023-05-26 09:43:38.583962 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
+-rw-r--r--   0        0        0     8974 2023-04-27 10:53:24.652797 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/solver.py
+-rw-r--r--   0        0        0    10912 2023-05-25 11:53:51.052894 edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/solver_bart.py
+-rw-r--r--   0        0        0      635 2023-05-26 03:02:12.777337 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/__pycache__/config.cpython-311.pyc
+-rw-r--r--   0        0        0     8950 2023-05-26 08:29:52.430340 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/__pycache__/run_bert.cpython-311.pyc
+-rw-r--r--   0        0        0      671 2023-04-27 12:36:01.129982 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/__pycache__/test_model.cpython-310-pytest-7.1.2.pyc
+-rw-r--r--   0        0        0      231 2023-04-27 10:53:25.896516 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/config.py
+-rw-r--r--   0        0        0     4322 2023-05-26 08:19:05.456679 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/import_data_bert.py
+-rw-r--r--   0        0        0     4883 2023-05-26 08:18:45.924774 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
+-rw-r--r--   0        0        0     3313 2023-05-26 08:19:16.939435 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/postagging.py
+-rw-r--r--   0        0        0     3227 2023-05-26 08:19:11.902948 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/postagging_new.py
+-rw-r--r--   0        0        0    85404 2023-04-27 10:53:26.056731 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
+-rw-r--r--   0        0        0     6168 2023-05-26 11:39:49.671484 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/run_bert.py
+-rw-r--r--   0        0        0     6410 2023-05-26 08:19:56.100659 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/solver.py
+-rw-r--r--   0        0        0     6979 2023-05-26 08:19:44.556860 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/solver_postag.py
+-rw-r--r--   0        0        0      537 2023-04-27 10:53:26.166114 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/test_model.py
+-rw-r--r--   0        0        0     1025 2023-05-26 08:20:25.421048 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/train_model.py
+-rw-r--r--   0        0        0     1315 2023-05-26 08:20:17.707417 edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/train_model_postag.py
+-rw-r--r--   0        0        0     3653 2023-05-29 11:21:59.867098 edu_segmentation-0.0.99/edu_segmentation/download.py
+-rw-r--r--   0        0        0     1885 2023-05-29 09:01:51.545612 edu_segmentation-0.0.99/edu_segmentation/main.py
+-rw-r--r--   0        0        0     2339 2023-05-29 11:32:48.736309 edu_segmentation-0.0.99/pyproject.toml
+-rw-r--r--   0        0        0      704 2023-05-29 07:05:32.388693 edu_segmentation-0.0.99/readme.md
+-rw-r--r--   0        0        0     3890 1970-01-01 00:00:00.000000 edu_segmentation-0.0.99/PKG-INFO
```

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/import_data_bart.py` & `edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/import_data_bart.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model.py` & `edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/model.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py` & `edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py` & `edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/run_segbot.py` & `edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/run_segbot.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/run_segbot_bart.py` & `edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/run_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/solver.py` & `edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/solver_bart.py` & `edu_segmentation-0.0.99/edu_segmentation/BARTTokenClassification/solver_bart.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/import_data_bert.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/import_data_bert.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/postagging.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/postagging.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/postagging_new.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/postagging_new.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/python38bert_modelling.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/python38bert_modelling.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/run_bert.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/run_bert.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/solver.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/solver_postag.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/solver_postag.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/test_model.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/test_model.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/train_model.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/train_model.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/train_model_postag.py` & `edu_segmentation-0.0.99/edu_segmentation/BERTTokenClassification/train_model_postag.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.98/edu_segmentation/main.py` & `edu_segmentation-0.0.99/edu_segmentation/main.py`

 * *Files identical despite different names*


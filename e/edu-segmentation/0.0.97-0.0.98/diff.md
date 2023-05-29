# Comparing `tmp/edu-segmentation-0.0.97.tar.gz` & `tmp/edu-segmentation-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu-segmentation-0.0.97.tar", last modified: Mon May 29 10:53:07 2023, max compression
+gzip compressed data, was "edu-segmentation-0.0.98.tar", last modified: Mon May 29 11:09:40 2023, max compression
```

## Comparing `edu-segmentation-0.0.97.tar` & `edu-segmentation-0.0.98.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.767459 edu-segmentation-0.0.97/
--rw-rw-rw-   0        0        0      178 2023-05-29 10:53:07.766459 edu-segmentation-0.0.97/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.714934 edu-segmentation-0.0.97/edu_segmentation/
-drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.738939 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/
--rw-rw-rw-   0        0        0      325 2023-04-27 10:53:24.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
--rw-rw-rw-   0        0        0      298 2023-04-27 10:53:24.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/config.py
--rw-rw-rw-   0        0        0     3930 2023-04-28 12:33:56.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/import_data_bart.py
--rw-rw-rw-   0        0        0    12186 2023-04-27 10:53:24.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model.py
-drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.743461 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model_dependencies/
--rw-rw-rw-   0        0        0    11216 2023-04-27 10:53:24.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py
--rw-rw-rw-   0        0        0     1510 2023-04-28 12:35:01.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py
--rw-rw-rw-   0        0        0     4364 2023-04-28 16:04:21.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/run_segbot.py
--rw-rw-rw-   0        0        0     7480 2023-05-26 09:43:38.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
--rw-rw-rw-   0        0        0     8974 2023-04-27 10:53:24.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/solver.py
--rw-rw-rw-   0        0        0    10912 2023-05-25 11:53:51.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/solver_bart.py
-drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.765460 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/
--rw-rw-rw-   0        0        0      231 2023-04-27 10:53:25.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/config.py
--rw-rw-rw-   0        0        0     4322 2023-05-26 08:19:05.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/import_data_bert.py
--rw-rw-rw-   0        0        0     4883 2023-05-26 08:18:45.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
--rw-rw-rw-   0        0        0     3313 2023-05-26 08:19:16.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/postagging.py
--rw-rw-rw-   0        0        0     3227 2023-05-26 08:19:11.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/postagging_new.py
--rw-rw-rw-   0        0        0    85404 2023-04-27 10:53:26.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
--rw-rw-rw-   0        0        0     6168 2023-05-26 11:39:49.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/run_bert.py
--rw-rw-rw-   0        0        0     6410 2023-05-26 08:19:56.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/solver.py
--rw-rw-rw-   0        0        0     6979 2023-05-26 08:19:44.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/solver_postag.py
--rw-rw-rw-   0        0        0      537 2023-04-27 10:53:26.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/test_model.py
--rw-rw-rw-   0        0        0     1025 2023-05-26 08:20:25.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/train_model.py
--rw-rw-rw-   0        0        0     1315 2023-05-26 08:20:17.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-rw-rw-   0        0        0     1885 2023-05-29 09:01:51.000000 edu-segmentation-0.0.97/edu_segmentation/main.py
-drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.725932 edu-segmentation-0.0.97/edu_segmentation.egg-info/
--rw-rw-rw-   0        0        0      178 2023-05-29 10:53:07.000000 edu-segmentation-0.0.97/edu_segmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1530 2023-05-29 10:53:07.000000 edu-segmentation-0.0.97/edu_segmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 10:53:07.000000 edu-segmentation-0.0.97/edu_segmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1221 2023-05-29 10:53:07.000000 edu-segmentation-0.0.97/edu_segmentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-29 10:53:07.000000 edu-segmentation-0.0.97/edu_segmentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 10:53:07.767459 edu-segmentation-0.0.97/setup.cfg
--rw-rw-rw-   0        0        0     6343 2023-05-29 10:52:20.000000 edu-segmentation-0.0.97/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.340275 edu-segmentation-0.0.98/
+-rw-rw-rw-   0        0        0      178 2023-05-29 11:09:40.340275 edu-segmentation-0.0.98/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.263271 edu-segmentation-0.0.98/edu_segmentation/
+drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.305271 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/
+-rw-rw-rw-   0        0        0      325 2023-04-27 10:53:24.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
+-rw-rw-rw-   0        0        0      298 2023-04-27 10:53:24.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/config.py
+-rw-rw-rw-   0        0        0     3930 2023-04-28 12:33:56.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/import_data_bart.py
+-rw-rw-rw-   0        0        0    12186 2023-04-27 10:53:24.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.309270 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model_dependencies/
+-rw-rw-rw-   0        0        0    11216 2023-04-27 10:53:24.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py
+-rw-rw-rw-   0        0        0     1510 2023-04-28 12:35:01.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py
+-rw-rw-rw-   0        0        0     4364 2023-04-28 16:04:21.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/run_segbot.py
+-rw-rw-rw-   0        0        0     7480 2023-05-26 09:43:38.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
+-rw-rw-rw-   0        0        0     8974 2023-04-27 10:53:24.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/solver.py
+-rw-rw-rw-   0        0        0    10912 2023-05-25 11:53:51.000000 edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/solver_bart.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.338271 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/
+-rw-rw-rw-   0        0        0      231 2023-04-27 10:53:25.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/config.py
+-rw-rw-rw-   0        0        0     4322 2023-05-26 08:19:05.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/import_data_bert.py
+-rw-rw-rw-   0        0        0     4883 2023-05-26 08:18:45.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
+-rw-rw-rw-   0        0        0     3313 2023-05-26 08:19:16.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/postagging.py
+-rw-rw-rw-   0        0        0     3227 2023-05-26 08:19:11.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/postagging_new.py
+-rw-rw-rw-   0        0        0    85404 2023-04-27 10:53:26.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
+-rw-rw-rw-   0        0        0     6168 2023-05-26 11:39:49.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/run_bert.py
+-rw-rw-rw-   0        0        0     6410 2023-05-26 08:19:56.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/solver.py
+-rw-rw-rw-   0        0        0     6979 2023-05-26 08:19:44.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/solver_postag.py
+-rw-rw-rw-   0        0        0      537 2023-04-27 10:53:26.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/test_model.py
+-rw-rw-rw-   0        0        0     1025 2023-05-26 08:20:25.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/train_model.py
+-rw-rw-rw-   0        0        0     1315 2023-05-26 08:20:17.000000 edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/train_model_postag.py
+-rw-rw-rw-   0        0        0     1885 2023-05-29 09:01:51.000000 edu-segmentation-0.0.98/edu_segmentation/main.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:09:40.281273 edu-segmentation-0.0.98/edu_segmentation.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-05-29 11:09:40.000000 edu-segmentation-0.0.98/edu_segmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1530 2023-05-29 11:09:40.000000 edu-segmentation-0.0.98/edu_segmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 11:09:40.000000 edu-segmentation-0.0.98/edu_segmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1221 2023-05-29 11:09:40.000000 edu-segmentation-0.0.98/edu_segmentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-29 11:09:40.000000 edu-segmentation-0.0.98/edu_segmentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 11:09:40.341273 edu-segmentation-0.0.98/setup.cfg
+-rw-rw-rw-   0        0        0     6463 2023-05-29 11:09:35.000000 edu-segmentation-0.0.98/setup.py
```

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/import_data_bart.py` & `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/import_data_bart.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model.py` & `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py` & `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py` & `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/run_segbot.py` & `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/run_segbot.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/run_segbot_bart.py` & `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/run_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/solver.py` & `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/solver_bart.py` & `edu-segmentation-0.0.98/edu_segmentation/BARTTokenClassification/solver_bart.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/import_data_bert.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/import_data_bert.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/postagging.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/postagging.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/postagging_new.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/postagging_new.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/python38bert_modelling.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/python38bert_modelling.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/run_bert.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/run_bert.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/solver.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/solver_postag.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/solver_postag.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/test_model.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/test_model.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/train_model.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/train_model.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/train_model_postag.py` & `edu-segmentation-0.0.98/edu_segmentation/BERTTokenClassification/train_model_postag.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation/main.py` & `edu-segmentation-0.0.98/edu_segmentation/main.py`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation.egg-info/SOURCES.txt` & `edu-segmentation-0.0.98/edu_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/edu_segmentation.egg-info/requires.txt` & `edu-segmentation-0.0.98/edu_segmentation.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edu-segmentation-0.0.97/setup.py` & `edu-segmentation-0.0.98/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from setuptools import setup
 from setuptools.command.install import install
 import os
 
 
 # Download your models from a specific URL
 def download_models():
+    print("download models was being accessed")
     import requests
     # function is placed here because requirements.txt needs to be downloaded first to get requests
     def download_torch_models(model_folder, model_name):
         username = "patrialyx"
         repo_name = "edu-segmentation-models"
         tag = "v1.0.0"
         model_url = f"https://github.com/{username}/{repo_name}/releases/download/{tag}/{model_name}"
@@ -84,21 +85,23 @@
 
 
 
 class InstallCommand(install):
     def run(self):
         # Call the parent install command
         install.run(self)
-        
+        print("this command was being run")
         # Download your models from the GitHub release
         download_models()
 
+print("setup.py was being run.")
+
 setup(
     name='edu-segmentation',
-    version='0.0.97',
+    version='0.0.98',
     description='To improve EDU segmentation performance using Segbot.',
     author='Your Name',
     author_email='you@example.com',
     install_requires=[
         'attrs==23.1.0',
         'bleach==6.0.0',
         'build==0.10.0',
```


# Comparing `tmp/edu_segmentation-0.0.96.tar.gz` & `tmp/edu-segmentation-0.0.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edu_segmentation-0.0.96.tar", last modified: Mon May 29 10:42:01 2023, max compression
+gzip compressed data, was "edu-segmentation-0.0.97.tar", last modified: Mon May 29 10:53:07 2023, max compression
```

## Comparing `edu_segmentation-0.0.96.tar` & `edu-segmentation-0.0.97.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 10:42:01.297170 edu_segmentation-0.0.96/
--rw-rw-rw-   0        0        0      178 2023-05-29 10:42:01.295174 edu_segmentation-0.0.96/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 10:42:01.228596 edu_segmentation-0.0.96/edu_segmentation/
-drwxrwxrwx   0        0        0        0 2023-05-29 10:42:01.266170 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/
--rw-rw-rw-   0        0        0      325 2023-04-27 10:53:24.000000 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
--rw-rw-rw-   0        0        0      298 2023-04-27 10:53:24.000000 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/config.py
--rw-rw-rw-   0        0        0     3930 2023-04-28 12:33:56.000000 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/import_data_bart.py
--rw-rw-rw-   0        0        0    12186 2023-04-27 10:53:24.000000 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/model.py
-drwxrwxrwx   0        0        0        0 2023-05-29 10:42:01.269171 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/model_dependencies/
--rw-rw-rw-   0        0        0    11216 2023-04-27 10:53:24.000000 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py
--rw-rw-rw-   0        0        0     1510 2023-04-28 12:35:01.000000 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py
--rw-rw-rw-   0        0        0     4364 2023-04-28 16:04:21.000000 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/run_segbot.py
--rw-rw-rw-   0        0        0     7480 2023-05-26 09:43:38.000000 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
--rw-rw-rw-   0        0        0     8974 2023-04-27 10:53:24.000000 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/solver.py
--rw-rw-rw-   0        0        0    10912 2023-05-25 11:53:51.000000 edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/solver_bart.py
-drwxrwxrwx   0        0        0        0 2023-05-29 10:42:01.292171 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/
--rw-rw-rw-   0        0        0      231 2023-04-27 10:53:25.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/config.py
--rw-rw-rw-   0        0        0     4322 2023-05-26 08:19:05.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/import_data_bert.py
--rw-rw-rw-   0        0        0     4883 2023-05-26 08:18:45.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
--rw-rw-rw-   0        0        0     3313 2023-05-26 08:19:16.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/postagging.py
--rw-rw-rw-   0        0        0     3227 2023-05-26 08:19:11.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/postagging_new.py
--rw-rw-rw-   0        0        0    85404 2023-04-27 10:53:26.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
--rw-rw-rw-   0        0        0     6168 2023-05-26 11:39:49.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/run_bert.py
--rw-rw-rw-   0        0        0     6410 2023-05-26 08:19:56.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/solver.py
--rw-rw-rw-   0        0        0     6979 2023-05-26 08:19:44.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/solver_postag.py
--rw-rw-rw-   0        0        0      537 2023-04-27 10:53:26.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/test_model.py
--rw-rw-rw-   0        0        0     1025 2023-05-26 08:20:25.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/train_model.py
--rw-rw-rw-   0        0        0     1315 2023-05-26 08:20:17.000000 edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-rw-rw-   0        0        0     1885 2023-05-29 09:01:51.000000 edu_segmentation-0.0.96/edu_segmentation/main.py
-drwxrwxrwx   0        0        0        0 2023-05-29 10:42:01.249172 edu_segmentation-0.0.96/edu_segmentation.egg-info/
--rw-rw-rw-   0        0        0      178 2023-05-29 10:42:01.000000 edu_segmentation-0.0.96/edu_segmentation.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1530 2023-05-29 10:42:01.000000 edu_segmentation-0.0.96/edu_segmentation.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 10:42:01.000000 edu_segmentation-0.0.96/edu_segmentation.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1221 2023-05-29 10:42:01.000000 edu_segmentation-0.0.96/edu_segmentation.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-29 10:42:01.000000 edu_segmentation-0.0.96/edu_segmentation.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 10:42:01.297170 edu_segmentation-0.0.96/setup.cfg
--rw-rw-rw-   0        0        0     6088 2023-05-29 10:41:28.000000 edu_segmentation-0.0.96/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.767459 edu-segmentation-0.0.97/
+-rw-rw-rw-   0        0        0      178 2023-05-29 10:53:07.766459 edu-segmentation-0.0.97/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.714934 edu-segmentation-0.0.97/edu_segmentation/
+drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.738939 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/
+-rw-rw-rw-   0        0        0      325 2023-04-27 10:53:24.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/bart_tokenizer.py
+-rw-rw-rw-   0        0        0      298 2023-04-27 10:53:24.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/config.py
+-rw-rw-rw-   0        0        0     3930 2023-04-28 12:33:56.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/import_data_bart.py
+-rw-rw-rw-   0        0        0    12186 2023-04-27 10:53:24.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.743461 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model_dependencies/
+-rw-rw-rw-   0        0        0    11216 2023-04-27 10:53:24.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py
+-rw-rw-rw-   0        0        0     1510 2023-04-28 12:35:01.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py
+-rw-rw-rw-   0        0        0     4364 2023-04-28 16:04:21.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/run_segbot.py
+-rw-rw-rw-   0        0        0     7480 2023-05-26 09:43:38.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/run_segbot_bart.py
+-rw-rw-rw-   0        0        0     8974 2023-04-27 10:53:24.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/solver.py
+-rw-rw-rw-   0        0        0    10912 2023-05-25 11:53:51.000000 edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/solver_bart.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.765460 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/
+-rw-rw-rw-   0        0        0      231 2023-04-27 10:53:25.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/config.py
+-rw-rw-rw-   0        0        0     4322 2023-05-26 08:19:05.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/import_data_bert.py
+-rw-rw-rw-   0        0        0     4883 2023-05-26 08:18:45.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py
+-rw-rw-rw-   0        0        0     3313 2023-05-26 08:19:16.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/postagging.py
+-rw-rw-rw-   0        0        0     3227 2023-05-26 08:19:11.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/postagging_new.py
+-rw-rw-rw-   0        0        0    85404 2023-04-27 10:53:26.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/python38bert_modelling.py
+-rw-rw-rw-   0        0        0     6168 2023-05-26 11:39:49.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/run_bert.py
+-rw-rw-rw-   0        0        0     6410 2023-05-26 08:19:56.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/solver.py
+-rw-rw-rw-   0        0        0     6979 2023-05-26 08:19:44.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/solver_postag.py
+-rw-rw-rw-   0        0        0      537 2023-04-27 10:53:26.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/test_model.py
+-rw-rw-rw-   0        0        0     1025 2023-05-26 08:20:25.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/train_model.py
+-rw-rw-rw-   0        0        0     1315 2023-05-26 08:20:17.000000 edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/train_model_postag.py
+-rw-rw-rw-   0        0        0     1885 2023-05-29 09:01:51.000000 edu-segmentation-0.0.97/edu_segmentation/main.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:53:07.725932 edu-segmentation-0.0.97/edu_segmentation.egg-info/
+-rw-rw-rw-   0        0        0      178 2023-05-29 10:53:07.000000 edu-segmentation-0.0.97/edu_segmentation.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1530 2023-05-29 10:53:07.000000 edu-segmentation-0.0.97/edu_segmentation.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 10:53:07.000000 edu-segmentation-0.0.97/edu_segmentation.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1221 2023-05-29 10:53:07.000000 edu-segmentation-0.0.97/edu_segmentation.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-29 10:53:07.000000 edu-segmentation-0.0.97/edu_segmentation.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 10:53:07.767459 edu-segmentation-0.0.97/setup.cfg
+-rw-rw-rw-   0        0        0     6343 2023-05-29 10:52:20.000000 edu-segmentation-0.0.97/setup.py
```

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/import_data_bart.py` & `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/import_data_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/model.py` & `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py` & `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model_dependencies/model_bart_v2.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py` & `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/model_dependencies/train_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/run_segbot.py` & `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/run_segbot.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/run_segbot_bart.py` & `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/run_segbot_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/solver.py` & `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BARTTokenClassification/solver_bart.py` & `edu-segmentation-0.0.97/edu_segmentation/BARTTokenClassification/solver_bart.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/import_data_bert.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/import_data_bert.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/import_data_bert_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/postagging.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/postagging.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/postagging_new.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/postagging_new.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/python38bert_modelling.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/python38bert_modelling.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/run_bert.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/run_bert.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/solver.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/solver.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/solver_postag.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/solver_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/test_model.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/test_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/train_model.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/train_model.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/BERTTokenClassification/train_model_postag.py` & `edu-segmentation-0.0.97/edu_segmentation/BERTTokenClassification/train_model_postag.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation/main.py` & `edu-segmentation-0.0.97/edu_segmentation/main.py`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation.egg-info/SOURCES.txt` & `edu-segmentation-0.0.97/edu_segmentation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/edu_segmentation.egg-info/requires.txt` & `edu-segmentation-0.0.97/edu_segmentation.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edu_segmentation-0.0.96/setup.py` & `edu-segmentation-0.0.97/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,10 @@
 from setuptools import setup
+from setuptools.command.install import install
 import os
-# import subprocess
-# import sys
-
-setup(
-    name='edu_segmentation',
-    version='0.0.96',
-    description='To improve EDU segmentation performance using Segbot.',
-    author='Your Name',
-    author_email='you@example.com',
-    install_requires=[
-        'attrs==23.1.0',
-        'bleach==6.0.0',
-        'build==0.10.0',
-        'CacheControl==0.12.11',
-        'certifi==2022.12.7',
-        'charset-normalizer==3.1.0',
-        'cleo==2.0.1',
-        'click==8.1.3',
-        'colorama==0.4.6',
-        'crashtest==0.4.1',
-        'distlib==0.3.6',
-        'docutils==0.19',
-        'dulwich==0.21.3',
-        'filelock==3.12.0',
-        'fsspec==2023.4.0',
-        'html5lib==1.1',
-        'huggingface-hub==0.14.1',
-        'idna==3.4',
-        'importlib-metadata==6.6.0',
-        'installer==0.7.0',
-        'jaraco.classes==3.2.3',
-        'Jinja2==3.1.2',
-        'joblib==1.2.0',
-        'jsonschema==4.17.3',
-        'keyring==23.13.1',
-        'lockfile==0.12.2',
-        'markdown-it-py==2.2.0',
-        'MarkupSafe==2.1.2',
-        'mdurl==0.1.2',
-        'more-itertools==9.1.0',
-        'mpmath==1.3.0',
-        'msgpack==1.0.5',
-        'networkx==3.1',
-        'nltk==3.8.1',
-        'numpy==1.24.3',
-        'packaging==23.1',
-        'pexpect==4.8.0',
-        'pkginfo==1.9.6',
-        'platformdirs==2.6.2',
-        'poetry==1.4.2',
-        'poetry-core==1.5.2',
-        'poetry-plugin-export==1.3.1',
-        'ptyprocess==0.7.0',
-        'Pygments==2.15.1',
-        'pyproject_hooks==1.0.0',
-        'pyrsistent==0.19.3',
-        'pywin32-ctypes==0.2.0',
-        'PyYAML==6.0',
-        'rapidfuzz==2.15.1',
-        'readme-renderer==37.3',
-        'regex==2023.3.23',
-        'requests==2.29.0',
-        'requests-toolbelt==0.10.1',
-        'rfc3986==2.0.0',
-        'rich==13.3.5',
-        'shellingham==1.5.0.post1',
-        'six==1.16.0',
-        'sympy==1.11.1',
-        'tokenizers==0.13.3',
-        'tomlkit==0.11.8',
-        'torch==2.0.0',
-        'tqdm==4.65.0',
-        'transformers==4.28.1',
-        'trove-classifiers==2023.4.25',
-        'twine==4.0.2',
-        'typing_extensions==4.5.0',
-        'urllib3==1.26.15',
-        'virtualenv==20.21.1',
-        'webencodings==0.5.1',
-        'zipp==3.15.0',
-    ],
-)
 
 
 # Download your models from a specific URL
 def download_models():
     import requests
     # function is placed here because requirements.txt needs to be downloaded first to get requests
     def download_torch_models(model_folder, model_name):
@@ -160,8 +79,96 @@
             print("Downloading Segbot BART Model...")
             download_torch_models(model_folder, model_name)
             print("Segbot BART Model downloaded successfully.")
     except:
         print("Failed to download Segbot BART Model.")
 
 
-download_models()
+
+class InstallCommand(install):
+    def run(self):
+        # Call the parent install command
+        install.run(self)
+        
+        # Download your models from the GitHub release
+        download_models()
+
+setup(
+    name='edu-segmentation',
+    version='0.0.97',
+    description='To improve EDU segmentation performance using Segbot.',
+    author='Your Name',
+    author_email='you@example.com',
+    install_requires=[
+        'attrs==23.1.0',
+        'bleach==6.0.0',
+        'build==0.10.0',
+        'CacheControl==0.12.11',
+        'certifi==2022.12.7',
+        'charset-normalizer==3.1.0',
+        'cleo==2.0.1',
+        'click==8.1.3',
+        'colorama==0.4.6',
+        'crashtest==0.4.1',
+        'distlib==0.3.6',
+        'docutils==0.19',
+        'dulwich==0.21.3',
+        'filelock==3.12.0',
+        'fsspec==2023.4.0',
+        'html5lib==1.1',
+        'huggingface-hub==0.14.1',
+        'idna==3.4',
+        'importlib-metadata==6.6.0',
+        'installer==0.7.0',
+        'jaraco.classes==3.2.3',
+        'Jinja2==3.1.2',
+        'joblib==1.2.0',
+        'jsonschema==4.17.3',
+        'keyring==23.13.1',
+        'lockfile==0.12.2',
+        'markdown-it-py==2.2.0',
+        'MarkupSafe==2.1.2',
+        'mdurl==0.1.2',
+        'more-itertools==9.1.0',
+        'mpmath==1.3.0',
+        'msgpack==1.0.5',
+        'networkx==3.1',
+        'nltk==3.8.1',
+        'numpy==1.24.3',
+        'packaging==23.1',
+        'pexpect==4.8.0',
+        'pkginfo==1.9.6',
+        'platformdirs==2.6.2',
+        'poetry==1.4.2',
+        'poetry-core==1.5.2',
+        'poetry-plugin-export==1.3.1',
+        'ptyprocess==0.7.0',
+        'Pygments==2.15.1',
+        'pyproject_hooks==1.0.0',
+        'pyrsistent==0.19.3',
+        'pywin32-ctypes==0.2.0',
+        'PyYAML==6.0',
+        'rapidfuzz==2.15.1',
+        'readme-renderer==37.3',
+        'regex==2023.3.23',
+        'requests==2.29.0',
+        'requests-toolbelt==0.10.1',
+        'rfc3986==2.0.0',
+        'rich==13.3.5',
+        'shellingham==1.5.0.post1',
+        'six==1.16.0',
+        'sympy==1.11.1',
+        'tokenizers==0.13.3',
+        'tomlkit==0.11.8',
+        'torch==2.0.0',
+        'tqdm==4.65.0',
+        'transformers==4.28.1',
+        'trove-classifiers==2023.4.25',
+        'twine==4.0.2',
+        'typing_extensions==4.5.0',
+        'urllib3==1.26.15',
+        'virtualenv==20.21.1',
+        'webencodings==0.5.1',
+        'zipp==3.15.0',
+    ],
+    cmdclass={'install': InstallCommand}
+)
```


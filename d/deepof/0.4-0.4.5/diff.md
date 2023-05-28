# Comparing `tmp/deepof-0.4.tar.gz` & `tmp/deepof-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepof-0.4.tar", last modified: Sun May 28 23:16:44 2023, max compression
+gzip compressed data, was "deepof-0.4.5.tar", last modified: Sun May 28 23:35:28 2023, max compression
```

## Comparing `deepof-0.4.tar` & `deepof-0.4.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:16:44.950097 deepof-0.4/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     1070 2022-08-29 09:41:22.000000 deepof-0.4/LICENSE
--rw-r--r--   0 lucas_miranda (1672059496) 75350028       77 2023-03-30 11:55:09.000000 deepof-0.4/MANIFEST.in
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     8054 2023-05-28 23:16:44.949861 deepof-0.4/PKG-INFO
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     7549 2023-05-28 23:09:50.000000 deepof-0.4/README.md
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:16:44.917014 deepof-0.4/deepof/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     6148 2023-03-09 17:44:01.000000 deepof-0.4/deepof/.DS_Store
--rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2022-08-29 09:41:22.000000 deepof-0.4/deepof/__init__.py
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:16:44.935799 deepof-0.4/deepof/__pycache__/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028      104 2023-03-30 11:25:12.000000 deepof-0.4/deepof/__pycache__/__init__.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028      153 2023-05-08 08:17:29.000000 deepof-0.4/deepof/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    22221 2023-05-20 09:15:40.000000 deepof-0.4/deepof/__pycache__/annotation_utils.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    71538 2023-05-20 09:15:50.000000 deepof-0.4/deepof/__pycache__/data.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     9319 2023-05-20 09:16:02.000000 deepof-0.4/deepof/__pycache__/deepof_train_embeddings.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     8804 2023-04-26 16:06:24.000000 deepof-0.4/deepof/__pycache__/hypermodels.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     6353 2023-05-08 08:17:38.000000 deepof-0.4/deepof/__pycache__/hypermodels.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    14803 2023-04-26 16:06:24.000000 deepof-0.4/deepof/__pycache__/model_utils.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    48088 2023-05-20 09:15:55.000000 deepof-0.4/deepof/__pycache__/model_utils.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     9325 2023-04-26 16:06:24.000000 deepof-0.4/deepof/__pycache__/models.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    49614 2023-05-15 14:00:18.000000 deepof-0.4/deepof/__pycache__/models.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    26124 2023-03-30 11:25:12.000000 deepof-0.4/deepof/__pycache__/pose_utils.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    39569 2023-05-20 09:15:55.000000 deepof-0.4/deepof/__pycache__/post_hoc.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    26524 2023-03-30 11:25:12.000000 deepof-0.4/deepof/__pycache__/preprocess.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    37167 2023-04-26 16:06:24.000000 deepof-0.4/deepof/__pycache__/utils.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    50602 2023-05-20 09:15:43.000000 deepof-0.4/deepof/__pycache__/utils.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     4586 2023-04-26 16:06:24.000000 deepof-0.4/deepof/__pycache__/visuals.cpython-36.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    69682 2023-05-20 09:16:01.000000 deepof-0.4/deepof/__pycache__/visuals.cpython-39.pyc
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    26207 2023-05-20 00:53:20.000000 deepof-0.4/deepof/annotation_utils.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    96978 2023-05-20 00:53:20.000000 deepof-0.4/deepof/data.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    15220 2023-05-20 00:53:20.000000 deepof-0.4/deepof/deepof_train_embeddings.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     8274 2023-04-26 16:00:17.000000 deepof-0.4/deepof/hypermodels.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    61556 2023-05-20 00:53:20.000000 deepof-0.4/deepof/model_utils.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    78665 2023-05-15 09:53:25.000000 deepof-0.4/deepof/models.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    48910 2023-05-20 00:53:20.000000 deepof-0.4/deepof/post_hoc.py
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:16:44.936655 deepof-0.4/deepof/trained_models/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028        0 2022-08-29 09:41:22.000000 deepof-0.4/deepof/trained_models/.gitkeep
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:16:44.939726 deepof-0.4/deepof/trained_models/deepof_supervised/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028  1133126 2023-03-30 11:55:02.000000 deepof-0.4/deepof/trained_models/deepof_supervised/deepof_supervised_dig_estimator.pkl
--rw-r--r--   0 lucas_miranda (1672059496) 75350028 10139395 2023-03-30 11:55:02.000000 deepof-0.4/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl
--rw-r--r--   0 lucas_miranda (1672059496) 75350028    62958 2023-05-20 00:53:20.000000 deepof-0.4/deepof/utils.py
--rw-r--r--   0 lucas_miranda (1672059496) 75350028   100784 2023-05-20 00:53:20.000000 deepof-0.4/deepof/visuals.py
-drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:16:44.918326 deepof-0.4/deepof.egg-info/
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     8054 2023-05-28 23:16:44.000000 deepof-0.4/deepof.egg-info/PKG-INFO
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     1413 2023-05-28 23:16:44.000000 deepof-0.4/deepof.egg-info/SOURCES.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028        1 2023-05-28 23:16:44.000000 deepof-0.4/deepof.egg-info/dependency_links.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028      841 2023-05-28 23:16:44.000000 deepof-0.4/deepof.egg-info/requires.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028        7 2023-05-28 23:16:44.000000 deepof-0.4/deepof.egg-info/top_level.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028      951 2023-05-28 22:06:16.000000 deepof-0.4/requirements.txt
--rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2023-05-28 23:16:44.950203 deepof-0.4/setup.cfg
--rw-r--r--   0 lucas_miranda (1672059496) 75350028     1017 2023-05-28 23:09:50.000000 deepof-0.4/setup.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:35:28.132697 deepof-0.4.5/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     1070 2022-08-29 09:41:22.000000 deepof-0.4.5/LICENSE
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028       77 2023-03-30 11:55:09.000000 deepof-0.4.5/MANIFEST.in
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     8058 2023-05-28 23:35:28.132519 deepof-0.4.5/PKG-INFO
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     7551 2023-05-28 23:35:01.000000 deepof-0.4.5/README.md
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:35:28.103476 deepof-0.4.5/deepof/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     6148 2023-03-09 17:44:01.000000 deepof-0.4.5/deepof/.DS_Store
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2022-08-29 09:41:22.000000 deepof-0.4.5/deepof/__init__.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:35:28.115949 deepof-0.4.5/deepof/__pycache__/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      104 2023-03-30 11:25:12.000000 deepof-0.4.5/deepof/__pycache__/__init__.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      153 2023-05-08 08:17:29.000000 deepof-0.4.5/deepof/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    22221 2023-05-20 09:15:40.000000 deepof-0.4.5/deepof/__pycache__/annotation_utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    71538 2023-05-20 09:15:50.000000 deepof-0.4.5/deepof/__pycache__/data.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     9319 2023-05-20 09:16:02.000000 deepof-0.4.5/deepof/__pycache__/deepof_train_embeddings.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     8804 2023-04-26 16:06:24.000000 deepof-0.4.5/deepof/__pycache__/hypermodels.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     6353 2023-05-08 08:17:38.000000 deepof-0.4.5/deepof/__pycache__/hypermodels.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    14803 2023-04-26 16:06:24.000000 deepof-0.4.5/deepof/__pycache__/model_utils.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    48088 2023-05-20 09:15:55.000000 deepof-0.4.5/deepof/__pycache__/model_utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     9325 2023-04-26 16:06:24.000000 deepof-0.4.5/deepof/__pycache__/models.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    49614 2023-05-15 14:00:18.000000 deepof-0.4.5/deepof/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    26124 2023-03-30 11:25:12.000000 deepof-0.4.5/deepof/__pycache__/pose_utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    39569 2023-05-20 09:15:55.000000 deepof-0.4.5/deepof/__pycache__/post_hoc.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    26524 2023-03-30 11:25:12.000000 deepof-0.4.5/deepof/__pycache__/preprocess.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    37167 2023-04-26 16:06:24.000000 deepof-0.4.5/deepof/__pycache__/utils.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    50602 2023-05-20 09:15:43.000000 deepof-0.4.5/deepof/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     4586 2023-04-26 16:06:24.000000 deepof-0.4.5/deepof/__pycache__/visuals.cpython-36.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    69682 2023-05-20 09:16:01.000000 deepof-0.4.5/deepof/__pycache__/visuals.cpython-39.pyc
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    26207 2023-05-20 00:53:20.000000 deepof-0.4.5/deepof/annotation_utils.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    96978 2023-05-20 00:53:20.000000 deepof-0.4.5/deepof/data.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    15220 2023-05-20 00:53:20.000000 deepof-0.4.5/deepof/deepof_train_embeddings.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     8274 2023-04-26 16:00:17.000000 deepof-0.4.5/deepof/hypermodels.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    61556 2023-05-20 00:53:20.000000 deepof-0.4.5/deepof/model_utils.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    78665 2023-05-15 09:53:25.000000 deepof-0.4.5/deepof/models.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    48910 2023-05-20 00:53:20.000000 deepof-0.4.5/deepof/post_hoc.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:35:28.120228 deepof-0.4.5/deepof/trained_models/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028        0 2022-08-29 09:41:22.000000 deepof-0.4.5/deepof/trained_models/.gitkeep
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:35:28.123333 deepof-0.4.5/deepof/trained_models/deepof_supervised/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028  1133126 2023-03-30 11:55:02.000000 deepof-0.4.5/deepof/trained_models/deepof_supervised/deepof_supervised_dig_estimator.pkl
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028 10139395 2023-03-30 11:55:02.000000 deepof-0.4.5/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028    62958 2023-05-20 00:53:20.000000 deepof-0.4.5/deepof/utils.py
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028   100784 2023-05-20 00:53:20.000000 deepof-0.4.5/deepof/visuals.py
+drwxr-xr-x   0 lucas_miranda (1672059496) 75350028        0 2023-05-28 23:35:28.105078 deepof-0.4.5/deepof.egg-info/
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     8058 2023-05-28 23:35:28.000000 deepof-0.4.5/deepof.egg-info/PKG-INFO
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     1413 2023-05-28 23:35:28.000000 deepof-0.4.5/deepof.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028        1 2023-05-28 23:35:28.000000 deepof-0.4.5/deepof.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      839 2023-05-28 23:35:28.000000 deepof-0.4.5/deepof.egg-info/requires.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028        7 2023-05-28 23:35:28.000000 deepof-0.4.5/deepof.egg-info/top_level.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028      949 2023-05-28 23:34:23.000000 deepof-0.4.5/requirements.txt
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028       38 2023-05-28 23:35:28.132743 deepof-0.4.5/setup.cfg
+-rw-r--r--   0 lucas_miranda (1672059496) 75350028     1019 2023-05-28 23:35:01.000000 deepof-0.4.5/setup.py
```

### Comparing `deepof-0.4/LICENSE` & `deepof-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `deepof-0.4/PKG-INFO` & `deepof-0.4.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepof
-Version: 0.4
+Version: 0.4.5
 Summary: A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut
 Home-page: https://gitlab.mpcdf.mpg.de/lucasmir/deepof/
 Author: Lucas Miranda
 Author-email: lucas_miranda@psych.mpg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.4-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.4.5-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 <br>
 
 <div align="center">
   <img width="350" height="350" src="https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/raw/master/logos/deepOF_logo_w_text.png">
```

### Comparing `deepof-0.4/README.md` & `deepof-0.4.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.4-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.4.5-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 <br>
 
 <div align="center">
   <img width="350" height="350" src="https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/raw/master/logos/deepOF_logo_w_text.png">
```

### Comparing `deepof-0.4/deepof/.DS_Store` & `deepof-0.4.5/deepof/.DS_Store`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/annotation_utils.cpython-39.pyc` & `deepof-0.4.5/deepof/__pycache__/annotation_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/data.cpython-39.pyc` & `deepof-0.4.5/deepof/__pycache__/data.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/deepof_train_embeddings.cpython-39.pyc` & `deepof-0.4.5/deepof/__pycache__/deepof_train_embeddings.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/hypermodels.cpython-36.pyc` & `deepof-0.4.5/deepof/__pycache__/hypermodels.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/hypermodels.cpython-39.pyc` & `deepof-0.4.5/deepof/__pycache__/hypermodels.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/model_utils.cpython-36.pyc` & `deepof-0.4.5/deepof/__pycache__/model_utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/model_utils.cpython-39.pyc` & `deepof-0.4.5/deepof/__pycache__/model_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/models.cpython-36.pyc` & `deepof-0.4.5/deepof/__pycache__/models.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/models.cpython-39.pyc` & `deepof-0.4.5/deepof/__pycache__/models.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/pose_utils.cpython-39.pyc` & `deepof-0.4.5/deepof/__pycache__/pose_utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/post_hoc.cpython-39.pyc` & `deepof-0.4.5/deepof/__pycache__/post_hoc.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/preprocess.cpython-36.pyc` & `deepof-0.4.5/deepof/__pycache__/preprocess.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/utils.cpython-36.pyc` & `deepof-0.4.5/deepof/__pycache__/utils.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/utils.cpython-39.pyc` & `deepof-0.4.5/deepof/__pycache__/utils.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/visuals.cpython-36.pyc` & `deepof-0.4.5/deepof/__pycache__/visuals.cpython-36.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/__pycache__/visuals.cpython-39.pyc` & `deepof-0.4.5/deepof/__pycache__/visuals.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/annotation_utils.py` & `deepof-0.4.5/deepof/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/data.py` & `deepof-0.4.5/deepof/data.py`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/deepof_train_embeddings.py` & `deepof-0.4.5/deepof/deepof_train_embeddings.py`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/hypermodels.py` & `deepof-0.4.5/deepof/hypermodels.py`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/model_utils.py` & `deepof-0.4.5/deepof/model_utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/models.py` & `deepof-0.4.5/deepof/models.py`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/post_hoc.py` & `deepof-0.4.5/deepof/post_hoc.py`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/trained_models/deepof_supervised/deepof_supervised_dig_estimator.pkl` & `deepof-0.4.5/deepof/trained_models/deepof_supervised/deepof_supervised_dig_estimator.pkl`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl` & `deepof-0.4.5/deepof/trained_models/deepof_supervised/deepof_supervised_huddle_estimator.pkl`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/utils.py` & `deepof-0.4.5/deepof/utils.py`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof/visuals.py` & `deepof-0.4.5/deepof/visuals.py`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof.egg-info/PKG-INFO` & `deepof-0.4.5/deepof.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepof
-Version: 0.4
+Version: 0.4.5
 Summary: A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut
 Home-page: https://gitlab.mpcdf.mpg.de/lucasmir/deepof/
 Author: Lucas Miranda
 Author-email: lucas_miranda@psych.mpg.de
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![Pipeline](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/pipeline.svg)](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/pipelines)
 [![Coverage](https://gitlab.mpcdf.mpg.de/lucasmir/deepof/badges/master/coverage.svg)](https://coverage.readthedocs.io/en/coverage-5.3/)
 [![Documentation Status](https://readthedocs.org/projects/deepof/badge/?version=latest)](https://deepof.readthedocs.io/en/latest)
 [![CodeFactor](https://www.codefactor.io/repository/github/lucasmiranda42/deepof/badge)](https://www.codefactor.io/repository/github/lucasmiranda42/deepof)
-[![Version](https://img.shields.io/badge/release-v0.4-informational)](https://pypi.org/project/deepof/)
+[![Version](https://img.shields.io/badge/release-v0.4.5-informational)](https://pypi.org/project/deepof/)
 [![MLFPM](https://img.shields.io/badge/funding-MLFPM-informational)](https://mlfpm.eu/)
 [![Black](https://img.shields.io/badge/code%20style-black-black)](https://github.com/psf/black)
 
 <br>
 
 <div align="center">
   <img width="350" height="350" src="https://gitlab.mpcdf.mpg.de/lucasmir/deepof/-/raw/master/logos/deepOF_logo_w_text.png">
```

### Comparing `deepof-0.4/deepof.egg-info/SOURCES.txt` & `deepof-0.4.5/deepof.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepof-0.4/deepof.egg-info/requires.txt` & `deepof-0.4.5/deepof.egg-info/requires.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 networkx>=2.8.8
 numpy>=1.23.5
 opencv_python>=4.7.0.72
 pandas~=1.5
 PIMS>=0.6.1
 pomegranate>=1.0.0
 POT>=0.8.2
-pytables>=3.7.0
+tables>=3.7.0
 regex>=2022.3.15
 regex>=2022.10.31
 ruptures>=1.1.7
 scikit_learn>=1.2.2
 scipy>=1.7.3
 seaborn>=0.11.2
 seglearn>=1.2.5
```

### Comparing `deepof-0.4/requirements.txt` & `deepof-0.4.5/requirements.txt`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 networkx>=2.8.8
 numpy>=1.23.5
 opencv_python>=4.7.0.72
 pandas~=1.5
 PIMS>=0.6.1
 pomegranate>=1.0.0
 POT>=0.8.2
-pytables>=3.7.0
+tables>=3.7.0
 regex>=2022.3.15
 regex>=2022.10.31
 ruptures>=1.1.7
 scikit_learn>=1.2.2
 scipy>=1.7.3
 seaborn>=0.11.2
 seglearn>=1.2.5
```

### Comparing `deepof-0.4/setup.py` & `deepof-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt", "r") as fp:
     install_requires = [pkg.replace("\n", "") for pkg in fp]
 
 setuptools.setup(
     name="deepof",
-    version="0.4",
+    version="0.4.5",
     author="Lucas Miranda",
     author_email="lucas_miranda@psych.mpg.de",
     description="A suite for postprocessing time-series extracted from videos of freely moving rodents using DeepLabCut",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.mpcdf.mpg.de/lucasmir/deepof/",
     packages=setuptools.find_packages(
```


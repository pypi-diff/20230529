# Comparing `tmp/VisageSnap-0.2.3.tar.gz` & `tmp/VisageSnap-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisageSnap-0.2.3.tar", last modified: Mon Mar  6 11:31:50 2023, max compression
+gzip compressed data, was "VisageSnap-0.3.0.tar", last modified: Mon May 29 09:39:46 2023, max compression
```

## Comparing `VisageSnap-0.2.3.tar` & `VisageSnap-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:31:50.533791 VisageSnap-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-03-06 11:31:41.000000 VisageSnap-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-06 11:31:50.529791 VisageSnap-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-03-06 11:31:41.000000 VisageSnap-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:31:50.529791 VisageSnap-0.2.3/VisageSnap/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-06 11:31:41.000000 VisageSnap-0.2.3/VisageSnap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-03-06 11:31:41.000000 VisageSnap-0.2.3/VisageSnap/classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13019 2023-03-06 11:31:41.000000 VisageSnap-0.2.3/VisageSnap/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-03-06 11:31:41.000000 VisageSnap-0.2.3/VisageSnap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:31:50.529791 VisageSnap-0.2.3/VisageSnap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-03-06 11:31:50.000000 VisageSnap-0.2.3/VisageSnap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-03-06 11:31:50.000000 VisageSnap-0.2.3/VisageSnap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 11:31:50.000000 VisageSnap-0.2.3/VisageSnap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-06 11:31:50.000000 VisageSnap-0.2.3/VisageSnap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-06 11:31:50.000000 VisageSnap-0.2.3/VisageSnap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 11:31:50.533791 VisageSnap-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-03-06 11:31:41.000000 VisageSnap-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 11:31:50.529791 VisageSnap-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-03-06 11:31:41.000000 VisageSnap-0.2.3/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.742438 VisageSnap-0.3.0/VisageSnap/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.742438 VisageSnap-0.3.0/VisageSnap/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/image/imageloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/VisageSnap/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/model/modelhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/VisageSnap/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/processor/faceprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/processor/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/processor/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.742438 VisageSnap-0.3.0/VisageSnap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-29 09:39:46.000000 VisageSnap-0.3.0/VisageSnap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-29 09:39:46.000000 VisageSnap-0.3.0/VisageSnap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:39:46.000000 VisageSnap-0.3.0/VisageSnap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 09:39:46.000000 VisageSnap-0.3.0/VisageSnap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 09:39:46.000000 VisageSnap-0.3.0/VisageSnap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/tests/test.py
```

### Comparing `VisageSnap-0.2.3/LICENSE` & `VisageSnap-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.2.3/PKG-INFO` & `VisageSnap-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,43 +1,28 @@
-Metadata-Version: 2.1
-Name: VisageSnap
-Version: 0.2.3
-Summary: Face Classification package
-Home-page: https://github.com/asheswook/VisageSnap
-Author: Jaewook Lee
-Author-email: me@jwlee.xyz
-Project-URL: Bug Tracker, https://github.com/asheswook/VisageSnap/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # VisageSnap
 
 ![Release](https://shields.io/github/v/release/asheswook/VisageSnap?display_name=tag&sort=semver) ![build](https://img.shields.io/github/actions/workflow/status/asheswook/VisageSnap/docker-workflow.yml?branch=main)
 
 **English** | [한국어](README-Korean.md)
 
 Recognizes faces and trains models, brings in the pictures and provides identification predictions and face classification. It also performs semi-supervised learning.
 
 ## Feature
 
--   Recognize faces.
--   Train the model through semi-supervised learning with labeled or unlabeled pictures.
--   Predicts if the face belongs to someone it knows and whose face it is.
+- Recognize faces.
+- Train the model through semi-supervised learning with labeled or unlabeled pictures.
+- Predicts if the face belongs to someone it knows and whose face it is.
 
 ## Installation
 
 ### Requirements
 
--   Python 3.9+
-    -   Versions below 3.9 have not been tested, and pickle module must be installed via pip.
--   dilb
+- Python 3.9+
+  - Versions below 3.9 have not been tested, and pickle module must be installed via pip.
+- dilb
 
 First, you need to install dilb. You can install it by following the instructions on the [here](https://gist.github.com/ageitgey/629d75c1baac34dfa5ca2a1928a7aeaf).
 
 Then, you can install VisageSnap by using pip:
 
 ```bash
 pip install visagesnap
@@ -76,14 +61,21 @@
 > Tom-126.jpeg<br>
 > Jerry-2.png<br>
 > Jerry-3.png<br>
 > Jerry-4.png<br>
 
 **Recognize faces and train the model**
 
+Before training, you need to load model.
+You don't have a model? It's okay. It'll be created automatically if it doesn't exist.
+
+```python
+vs.load_model()
+```
+
 Train with the picture files in the directory.
 
 ```
 vs.train_labeled_data()
 ```
 
 If you want to train with unlabeled data, you can also try to like this:
@@ -106,28 +98,68 @@
    "target1.png": "Tom",
    "target2.jpeg": "Jerry",
    "target3.jpeg": ["Tom", "Jerry"], # multiple faces in one picture
    "target4.jpeg": None # If the face is unknown
 }
 ```
 
+**Full example**
+
+You can see the full code [here](tests/test.py).
+
+---
+
 **To change the directory you work with**
 
 You should put the picture files into configured directory, and also model file is stored in model directory.
 
 ```python
-vs.set_directory({
-    "labeled": "labeled_pic",
-    "unlabeled": "unlabeled_pic",
-    "model": "my_model.d"
-})
+from VisageSnap import Directory
+
+my_dir = Directory( "labeled_pic",
+                    "unlabeled_pic",
+                    "my_model.d",
+                    "predict_dir")
+vs.set_directory(my_dir)
 ```
 
 _Default Directory:_
 
 ```python
 {
     "labeled": "labeled",
     "unlabeled": "unlabeled",
     "model": "model"
 }
 ```
+
+### Others
+
+**To get the face information**
+
+You can get the faceObject by using `get_faceObject` method. The faceObject is a dataclass that contains the face information.
+
+```python
+from visagesnap import From
+# From.LABEL, From.FILENAME
+```
+
+```python
+face_tom = vs.get_faceObject(From.LABEL, "Tom")
+face_tom = vs.get_faceObject(From.FILENAME, "Tom-123.png")
+# face_tom = Face(label, encodings, filenames)
+
+name: str = face_tom.label
+encodings: NDArray = face_tom.encodings
+filenames: list = face_tom.filenames
+```
+
+**To change prediction threshold**
+
+```python
+vs.threshold = 0.5  # Default: 0.48
+```
+
+## Acknowledgement
+
+- [scikit-learn](https://scikit-learn.org/stable/)
+- [face_recognition](https://github.com/ageitgey/face_recognition)
```

### Comparing `VisageSnap-0.2.3/setup.py` & `VisageSnap-0.3.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'scikit-learn',
     'dlib',
     'face_recognition',
 ]
 
 setuptools.setup(
     name='VisageSnap',
-    version='0.2.3',
+    version='0.3.0',
     author='Jaewook Lee',
     author_email='me@jwlee.xyz',
     description='Face Classification package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/asheswook/VisageSnap',
     project_urls={
```


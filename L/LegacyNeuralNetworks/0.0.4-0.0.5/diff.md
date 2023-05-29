# Comparing `tmp/LegacyNeuralNetworks-0.0.4.tar.gz` & `tmp/LegacyNeuralNetworks-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LegacyNeuralNetworks-0.0.4.tar", last modified: Sun May 28 18:36:29 2023, max compression
+gzip compressed data, was "LegacyNeuralNetworks-0.0.5.tar", last modified: Sun May 28 18:51:53 2023, max compression
```

## Comparing `LegacyNeuralNetworks-0.0.4.tar` & `LegacyNeuralNetworks-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 18:36:29.857357 LegacyNeuralNetworks-0.0.4/
-drwxrwxrwx   0        0        0        0 2023-05-28 18:36:29.829495 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/
--rw-rw-rw-   0        0        0    29928 2023-05-28 18:33:46.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/Fill.py
--rw-rw-rw-   0        0        0    19189 2023-05-27 08:44:43.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/LegacyNeuralNetworks.py
--rw-rw-rw-   0        0        0      151 2023-05-27 14:39:50.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/__init__.py
--rw-rw-rw-   0        0        0    14578 2023-05-27 14:39:19.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/ann_fill.py
-drwxrwxrwx   0        0        0        0 2023-05-28 18:36:29.855358 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/
--rw-rw-rw-   0        0        0     4398 2023-05-28 18:36:29.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2023-05-28 18:36:29.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 18:36:29.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-05-28 18:36:29.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-28 18:36:29.000000 LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4398 2023-05-28 18:36:29.856354 LegacyNeuralNetworks-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3284 2023-05-27 14:44:31.000000 LegacyNeuralNetworks-0.0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-28 18:36:29.857357 LegacyNeuralNetworks-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      907 2023-05-28 18:36:05.000000 LegacyNeuralNetworks-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 18:51:53.622008 LegacyNeuralNetworks-0.0.5/
+drwxrwxrwx   0        0        0        0 2023-05-28 18:51:53.612991 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks/
+-rw-rw-rw-   0        0        0    30117 2023-05-28 18:50:48.000000 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks/Fill.py
+-rw-rw-rw-   0        0        0    19189 2023-05-27 08:44:43.000000 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks/LegacyNeuralNetworks.py
+-rw-rw-rw-   0        0        0      200 2023-05-28 18:51:14.000000 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks/__init__.py
+-rw-rw-rw-   0        0        0    14578 2023-05-27 14:39:19.000000 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks/ann_fill.py
+-rw-rw-rw-   0        0        0     9677 2023-05-28 16:18:51.000000 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks/ds_fill.py
+drwxrwxrwx   0        0        0        0 2023-05-28 18:51:53.617986 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks.egg-info/
+-rw-rw-rw-   0        0        0     4398 2023-05-28 18:51:53.000000 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      409 2023-05-28 18:51:53.000000 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 18:51:53.000000 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-28 18:51:53.000000 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-28 18:51:53.000000 LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4398 2023-05-28 18:51:53.618987 LegacyNeuralNetworks-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3284 2023-05-27 14:44:31.000000 LegacyNeuralNetworks-0.0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 18:51:53.622008 LegacyNeuralNetworks-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      907 2023-05-28 18:51:25.000000 LegacyNeuralNetworks-0.0.5/setup.py
```

### Comparing `LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/Fill.py` & `LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks/Fill.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,15 +266,18 @@
         X_test = np.array(test_data)
         predictions = self.clf.predict(X_test)
         majority_vote = np.argmax(np.bincount(predictions))
         return majority_vote
 
 recognizer = PerceptronNN(16)
 recognizer.train()
+# test_data = [[1, 1, 1], [1, 0, 1], [1, 0, 1], [1, 0, 1], [1, 1, 1]]
+test_data = [[1, 1, 1], [1, 0, 0], [1, 1, 1], [1, 0, 1], [1, 1, 1]]
 test_data = np.array([test_data]).flatten()
+predictions = recognizer.recognize([test_data])
 print(predictions)
 """
 
 ann_forward_backward = """ 
 import numpy as np
 import tensorflow as tf
 import matplotlib.pyplot as plt
```

### Comparing `LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/LegacyNeuralNetworks.py` & `LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks/LegacyNeuralNetworks.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks/ann_fill.py` & `LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks/ann_fill.py`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.0.4/LegacyNeuralNetworks.egg-info/PKG-INFO` & `LegacyNeuralNetworks-0.0.5/LegacyNeuralNetworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LegacyNeuralNetworks
-Version: 0.0.4
+Version: 0.0.5
 Summary: Legacy Neural Networks
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: # Legacy Neural Networks
```

### Comparing `LegacyNeuralNetworks-0.0.4/PKG-INFO` & `LegacyNeuralNetworks-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LegacyNeuralNetworks
-Version: 0.0.4
+Version: 0.0.5
 Summary: Legacy Neural Networks
 Home-page: UNKNOWN
 Author: Hrushikesh Kachgunde
 Author-email: <hrushiskachgunde@gmail.com>
 License: UNKNOWN
 Description: # Legacy Neural Networks
```

### Comparing `LegacyNeuralNetworks-0.0.4/README.md` & `LegacyNeuralNetworks-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `LegacyNeuralNetworks-0.0.4/setup.py` & `LegacyNeuralNetworks-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Legacy Neural Networks'
  
 # Setting up
 setup(
     name="LegacyNeuralNetworks",
     version=VERSION,
     author="Hrushikesh Kachgunde",
```


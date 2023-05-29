# Comparing `tmp/rsbox-0.0.8.tar.gz` & `tmp/rsbox-0.0.9.tar.gz`

## Comparing `rsbox-0.0.8.tar` & `rsbox-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 rsbox-0.0.8/.DS_Store
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 rsbox-0.0.8/changelog.md
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 rsbox-0.0.8/requirements.txt
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 rsbox-0.0.8/.github/workflows/docs.yml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsbox-0.0.8/src/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rsbox-0.0.8/src/rsbox/__init__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 rsbox-0.0.8/src/rsbox/example.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 rsbox-0.0.8/src/rsbox/misc.py
--rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 rsbox-0.0.8/src/rsbox/ml.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 rsbox-0.0.8/LICENSE
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 rsbox-0.0.8/README.md
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 rsbox-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 rsbox-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 rsbox-0.0.9/.DS_Store
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 rsbox-0.0.9/changelog.md
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 rsbox-0.0.9/requirements.txt
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 rsbox-0.0.9/.github/workflows/docs.yml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 rsbox-0.0.9/src/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 rsbox-0.0.9/src/rsbox/__init__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 rsbox-0.0.9/src/rsbox/example.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 rsbox-0.0.9/src/rsbox/misc.py
+-rw-r--r--   0        0        0     7496 2020-02-02 00:00:00.000000 rsbox-0.0.9/src/rsbox/ml.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 rsbox-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 rsbox-0.0.9/README.md
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 rsbox-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2955 2020-02-02 00:00:00.000000 rsbox-0.0.9/PKG-INFO
```

### Comparing `rsbox-0.0.8/.DS_Store` & `rsbox-0.0.9/.DS_Store`

 * *Files identical despite different names*

### Comparing `rsbox-0.0.8/changelog.md` & `rsbox-0.0.9/changelog.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ## Version changelog 
 
+### `0.0.8`
+- Added `ml.MeanMetric`
+
+
 ### `0.0.7`
 
 - Fixed bug in `misc.timestamp`
 
 ### `0.0.6`
 - Added `print_model_size`, `img_dataset_from_dir`, `get_img` functions.
```

### Comparing `rsbox-0.0.8/.github/workflows/docs.yml` & `rsbox-0.0.9/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `rsbox-0.0.8/src/.DS_Store` & `rsbox-0.0.9/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `rsbox-0.0.8/src/rsbox/misc.py` & `rsbox-0.0.9/src/rsbox/misc.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 -------------- 
 Miscellaneous utils. 
 """ 
 
 import pickle
 from datetime import datetime
 from pytz import timezone
+import requests
+import cloudpickle as cp
+from urllib.request import urlopen
 
 
 def timestamp():
     """
     Simple function that retrieves the current date and time
     and returns a properly formatted string (i.e., a timestamp).  
     """
@@ -35,7 +38,20 @@
 	Takes in a path to a pickled 
 	.pkl file (type: 'str') and
 	returns the unpickled object. 
 	"""
 	in_file = open(filepath, 'rb')
 	loaded_object = pickle.load(in_file) 
 	return loaded_object
+
+
+def load_dataset(urlpath=None):
+	"""
+	Given a url to a .pkl dataset file,
+	loads and returns the dataset object. 
+	"""
+	if urlpath is None:
+		urlpath = r"https://stanford.edu/~rsikand/assets/datasets/mini_cifar.pkl"
+	
+	dataset = cp.load(urlopen(urlpath)) 
+	return dataset
+
```

### Comparing `rsbox-0.0.8/src/rsbox/ml.py` & `rsbox-0.0.9/src/rsbox/ml.py`

 * *Files identical despite different names*

### Comparing `rsbox-0.0.8/LICENSE` & `rsbox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rsbox-0.0.8/README.md` & `rsbox-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `rsbox-0.0.8/pyproject.toml` & `rsbox-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "rsbox"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Rohan Sikand", email="rsikand29@gmail.com" },
 ]
 description = "A toolbox of utility functions I commonly use when programming in Python."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `rsbox-0.0.8/PKG-INFO` & `rsbox-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rsbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: A toolbox of utility functions I commonly use when programming in Python.
 Project-URL: Homepage, https://github.com/rosikand/rsbox
 Author-email: Rohan Sikand <rsikand29@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```


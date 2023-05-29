# Comparing `tmp/lrservice-0.0.1.tar.gz` & `tmp/lrservice-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lrservice-0.0.1.tar", last modified: Mon May 29 15:11:36 2023, max compression
+gzip compressed data, was "lrservice-0.0.2.tar", last modified: Mon May 29 15:44:40 2023, max compression
```

## Comparing `lrservice-0.0.1.tar` & `lrservice-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-29 15:11:36.692081 lrservice-0.0.1/
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1054 2023-05-29 14:57:14.000000 lrservice-0.0.1/LICENSE
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      601 2023-05-29 15:11:36.691779 lrservice-0.0.1/PKG-INFO
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      130 2023-05-29 15:01:43.000000 lrservice-0.0.1/README.md
-drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-29 15:11:36.689821 lrservice-0.0.1/lrservice/
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)       19 2023-05-29 14:46:13.000000 lrservice-0.0.1/lrservice/__init__.py
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1363 2022-02-16 23:54:46.000000 lrservice-0.0.1/lrservice/benchmark.py
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1883 2023-05-29 14:38:51.000000 lrservice-0.0.1/lrservice/main.py
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)     3417 2023-05-29 14:38:50.000000 lrservice-0.0.1/lrservice/simple_linear_regr.py
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1836 2022-02-16 23:54:46.000000 lrservice-0.0.1/lrservice/simple_linear_regr_utils.py
-drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-29 15:11:36.691353 lrservice-0.0.1/lrservice.egg-info/
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      601 2023-05-29 15:11:36.000000 lrservice-0.0.1/lrservice.egg-info/PKG-INFO
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      291 2023-05-29 15:11:36.000000 lrservice-0.0.1/lrservice.egg-info/SOURCES.txt
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)        1 2023-05-29 15:11:36.000000 lrservice-0.0.1/lrservice.egg-info/dependency_links.txt
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)       10 2023-05-29 15:11:36.000000 lrservice-0.0.1/lrservice.egg-info/top_level.txt
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)       38 2023-05-29 15:11:36.692249 lrservice-0.0.1/setup.cfg
--rwxrwxrwx   0 tyler     (1000) tyler     (1000)      679 2023-05-29 15:05:02.000000 lrservice-0.0.1/setup.py
+drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-29 15:44:40.617577 lrservice-0.0.2/
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1054 2023-05-29 14:57:14.000000 lrservice-0.0.2/LICENSE
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      601 2023-05-29 15:44:40.617271 lrservice-0.0.2/PKG-INFO
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      130 2023-05-29 15:01:43.000000 lrservice-0.0.2/README.md
+drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-29 15:44:40.614954 lrservice-0.0.2/lrservice/
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      159 2023-05-29 15:44:10.000000 lrservice-0.0.2/lrservice/__init__.py
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1363 2022-02-16 23:54:46.000000 lrservice-0.0.2/lrservice/benchmark.py
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1882 2023-05-29 15:29:59.000000 lrservice-0.0.2/lrservice/main.py
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)     3416 2023-05-29 15:29:52.000000 lrservice-0.0.2/lrservice/simple_linear_regr.py
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)     1840 2023-05-29 15:36:07.000000 lrservice-0.0.2/lrservice/simple_linear_regr_utils.py
+drwxrwxrwx   0 tyler     (1000) tyler     (1000)        0 2023-05-29 15:44:40.616845 lrservice-0.0.2/lrservice.egg-info/
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      601 2023-05-29 15:44:40.000000 lrservice-0.0.2/lrservice.egg-info/PKG-INFO
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      291 2023-05-29 15:44:40.000000 lrservice-0.0.2/lrservice.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)        1 2023-05-29 15:44:40.000000 lrservice-0.0.2/lrservice.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)       10 2023-05-29 15:44:40.000000 lrservice-0.0.2/lrservice.egg-info/top_level.txt
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)       38 2023-05-29 15:44:40.617654 lrservice-0.0.2/setup.cfg
+-rwxrwxrwx   0 tyler     (1000) tyler     (1000)      679 2023-05-29 15:41:16.000000 lrservice-0.0.2/setup.py
```

### Comparing `lrservice-0.0.1/LICENSE` & `lrservice-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lrservice-0.0.1/PKG-INFO` & `lrservice-0.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lrservice
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for demonstrating how to make REST API service for linear regression
 Home-page: https://github.com/CyberPlayerOne/lrservice
 Author: Tyler Tang
 Author-email: tyler.x.tang@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lrservice-0.0.1/lrservice/benchmark.py` & `lrservice-0.0.2/lrservice/benchmark.py`

 * *Files identical despite different names*

### Comparing `lrservice-0.0.1/lrservice/main.py` & `lrservice-0.0.2/lrservice/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from flask import Flask, request, jsonify
 import dill
 import numpy as np
 
 app = Flask('app')
 
-with open('../save/model.pickle', 'rb') as f:
+with open('./save/model.pickle', 'rb') as f:
     model = dill.load(f)
 
 
 @app.route('/', methods=['GET'])
 def home():
     return 'Simple Linear Regression'
```

### Comparing `lrservice-0.0.1/lrservice/simple_linear_regr.py` & `lrservice-0.0.2/lrservice/simple_linear_regr.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,12 +90,12 @@
     evaluate(model, X_test, y_test, predicted)
 
     # import matplotlib.pyplot as plt
     # plt.plot(model.losses, range(len(model.losses)))
     # plt.show()
     #
 
-    model_pickle_path = '../save/model.pickle'
+    model_pickle_path = './save/model.pickle'
     with open(model_pickle_path, 'wb') as f:
         dill.dump(model, f, recurse=True)
 
     print(f'SimpleLinearRegression model is trained and saved to: {model_pickle_path}')
```

### Comparing `lrservice-0.0.1/lrservice/simple_linear_regr_utils.py` & `lrservice-0.0.2/lrservice/simple_linear_regr_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 from sklearn.datasets import load_diabetes
 from sklearn.metrics import mean_squared_error, r2_score
 import matplotlib.pyplot as plt
 
+
 def generate_data():
     """
     Generates a random dataset from a normal distribution.
 
     Returns:
         diabetes_X_train: the training dataset
         diabetes_y_train: The output corresponding to the training set
@@ -21,16 +22,16 @@
     diabetes_X = diabetes_X[:, np.newaxis, 2]
 
     # Split the data into training/testing sets
     diabetes_X_train = diabetes_X[:-20]
     diabetes_X_test = diabetes_X[-20:]
 
     # Split the targets into training/testing sets
-    diabetes_y_train = diabetes_y[:-20].reshape(-1,1)
-    diabetes_y_test = diabetes_y[-20:].reshape(-1,1)
+    diabetes_y_train = diabetes_y[:-20].reshape(-1, 1)
+    diabetes_y_test = diabetes_y[-20:].reshape(-1, 1)
 
     print(f"# Training Samples: {len(diabetes_X_train)}; # Test samples: {len(diabetes_X_test)};")
     return diabetes_X_train, diabetes_y_train, diabetes_X_test, diabetes_y_test
 
 
 def evaluate(model, X, y, y_predicted):
     """ Calculates and prints evaluation metrics. """
@@ -51,8 +52,8 @@
     plt.yticks(())
 
     plt.show()
 
     if r2 >= 0.4:
         print("****** Success ******")
     else:
-        print("****** Failed ******")
+        print("****** Failed ******")
```

### Comparing `lrservice-0.0.1/lrservice.egg-info/PKG-INFO` & `lrservice-0.0.2/lrservice.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lrservice
-Version: 0.0.1
+Version: 0.0.2
 Summary: A python package for demonstrating how to make REST API service for linear regression
 Home-page: https://github.com/CyberPlayerOne/lrservice
 Author: Tyler Tang
 Author-email: tyler.x.tang@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `lrservice-0.0.1/setup.py` & `lrservice-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lrservice",
-    version="0.0.1",
+    version="0.0.2",
     author="Tyler Tang",
     author_email="tyler.x.tang@outlook.com",
     description="A python package for demonstrating how to make REST API service for linear regression",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CyberPlayerOne/lrservice",
     packages=setuptools.find_packages(),
```


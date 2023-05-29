# Comparing `tmp/deepapi-0.4.2.tar.gz` & `tmp/deepapi-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepapi-0.4.2.tar", last modified: Tue Nov  1 21:12:39 2022, max compression
+gzip compressed data, was "/home/wuhanstudio/Desktop/deepapi/dist/.tmp-a07pxpab/deepapi-0.4.3.tar", last modified: Mon May 29 15:35:49 2023, max compression
```

## Comparing `deepapi-0.4.2.tar` & `deepapi-0.4.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 dongyawang   (501) staff       (20)        0 2022-11-01 21:12:39.673067 deepapi-0.4.2/
--rw-r--r--   0 dongyawang   (501) staff       (20)     1063 2022-11-01 21:10:56.000000 deepapi-0.4.2/LICENSE
--rw-r--r--   0 dongyawang   (501) staff       (20)     3269 2022-11-01 21:12:39.672636 deepapi-0.4.2/PKG-INFO
--rw-r--r--   0 dongyawang   (501) staff       (20)     2584 2022-11-01 21:10:56.000000 deepapi-0.4.2/README.md
-drwxr-xr-x   0 dongyawang   (501) staff       (20)        0 2022-11-01 21:12:39.651862 deepapi-0.4.2/deepapi/
--rw-r--r--   0 dongyawang   (501) staff       (20)      147 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/__init__.py
--rw-r--r--   0 dongyawang   (501) staff       (20)       32 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/__main__.py
--rw-r--r--   0 dongyawang   (501) staff       (20)     4231 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/_main.py
-drwxr-xr-x   0 dongyawang   (501) staff       (20)        0 2022-11-01 21:12:39.655372 deepapi-0.4.2/deepapi/api/
--rw-r--r--   0 dongyawang   (501) staff       (20)     7285 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/api/__init__.py
-drwxr-xr-x   0 dongyawang   (501) staff       (20)        0 2022-11-01 21:12:39.658461 deepapi-0.4.2/deepapi/dataset/
--rw-r--r--   0 dongyawang   (501) staff       (20)      176 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/dataset/__init__.py
--rw-r--r--   0 dongyawang   (501) staff       (20)      108 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/dataset/cifar10.py
--rw-r--r--   0 dongyawang   (501) staff       (20)     1356 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/dataset/imagenet.py
--rw-r--r--   0 dongyawang   (501) staff       (20)    35379 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/dataset/imagenet_class_index.py
-drwxr-xr-x   0 dongyawang   (501) staff       (20)        0 2022-11-01 21:12:39.661706 deepapi-0.4.2/deepapi/models/
--rw-r--r--   0 dongyawang   (501) staff       (20)      179 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/models/__init__.py
--rw-r--r--   0 dongyawang   (501) staff       (20)      734 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/models/inceptionv3.py
--rw-r--r--   0 dongyawang   (501) staff       (20)      716 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/models/resnet50.py
--rw-r--r--   0 dongyawang   (501) staff       (20)     5626 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/models/vgg16.py
-drwxr-xr-x   0 dongyawang   (501) staff       (20)        0 2022-11-01 21:12:39.667867 deepapi-0.4.2/deepapi/static/
--rw-r--r--   0 dongyawang   (501) staff       (20)    10865 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/static/font.js
--rw-r--r--   0 dongyawang   (501) staff       (20)     9967 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/static/index.html
--rw-r--r--   0 dongyawang   (501) staff       (20)     7810 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/static/script.js
--rw-r--r--   0 dongyawang   (501) staff       (20)     2158 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/static/simpleSnackbar.min.css
--rw-r--r--   0 dongyawang   (501) staff       (20)     8740 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/static/simpleSnackbar.min.js
--rw-r--r--   0 dongyawang   (501) staff       (20)     2139 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/static/style.css
--rw-r--r--   0 dongyawang   (501) staff       (20)     2677 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/static/upload.js
-drwxr-xr-x   0 dongyawang   (501) staff       (20)        0 2022-11-01 21:12:39.669241 deepapi-0.4.2/deepapi/utils/
--rw-r--r--   0 dongyawang   (501) staff       (20)       53 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/utils/__init__.py
--rw-r--r--   0 dongyawang   (501) staff       (20)     1789 2022-11-01 21:10:56.000000 deepapi-0.4.2/deepapi/utils/response.py
-drwxr-xr-x   0 dongyawang   (501) staff       (20)        0 2022-11-01 21:12:39.654876 deepapi-0.4.2/deepapi.egg-info/
--rw-r--r--   0 dongyawang   (501) staff       (20)     3269 2022-11-01 21:12:39.000000 deepapi-0.4.2/deepapi.egg-info/PKG-INFO
--rw-r--r--   0 dongyawang   (501) staff       (20)      860 2022-11-01 21:12:39.000000 deepapi-0.4.2/deepapi.egg-info/SOURCES.txt
--rw-r--r--   0 dongyawang   (501) staff       (20)        1 2022-11-01 21:12:39.000000 deepapi-0.4.2/deepapi.egg-info/dependency_links.txt
--rw-r--r--   0 dongyawang   (501) staff       (20)       47 2022-11-01 21:12:39.000000 deepapi-0.4.2/deepapi.egg-info/entry_points.txt
--rw-r--r--   0 dongyawang   (501) staff       (20)      103 2022-11-01 21:12:39.000000 deepapi-0.4.2/deepapi.egg-info/requires.txt
--rw-r--r--   0 dongyawang   (501) staff       (20)        8 2022-11-01 21:12:39.000000 deepapi-0.4.2/deepapi.egg-info/top_level.txt
--rw-r--r--   0 dongyawang   (501) staff       (20)     1260 2022-11-01 21:10:56.000000 deepapi-0.4.2/pyproject.toml
--rw-r--r--   0 dongyawang   (501) staff       (20)       38 2022-11-01 21:12:39.673216 deepapi-0.4.2/setup.cfg
--rw-r--r--   0 dongyawang   (501) staff       (20)     2280 2022-11-01 21:10:56.000000 deepapi-0.4.2/setup.py
-drwxr-xr-x   0 dongyawang   (501) staff       (20)        0 2022-11-01 21:12:39.671740 deepapi-0.4.2/test/
--rw-r--r--   0 dongyawang   (501) staff       (20)      389 2022-11-01 21:10:56.000000 deepapi-0.4.2/test/test_deepapi.py
--rw-r--r--   0 dongyawang   (501) staff       (20)     1662 2022-11-01 21:10:56.000000 deepapi-0.4.2/test/test_minimal.py
--rw-r--r--   0 dongyawang   (501) staff       (20)     2785 2022-11-01 21:10:56.000000 deepapi-0.4.2/test/test_multi_client.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-29 15:35:48.000000 deepapi-0.4.3/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1063 2023-05-29 14:34:06.000000 deepapi-0.4.3/LICENSE
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3330 2023-05-29 15:35:48.000000 deepapi-0.4.3/PKG-INFO
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2645 2023-05-29 15:32:44.000000 deepapi-0.4.3/README.md
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      147 2023-05-29 15:33:17.000000 deepapi-0.4.3/deepapi/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       32 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/__main__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     4231 2023-05-29 15:32:19.000000 deepapi-0.4.3/deepapi/_main.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi/api/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7285 2023-05-29 15:32:44.000000 deepapi-0.4.3/deepapi/api/__init__.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi/dataset/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      176 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/dataset/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      108 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/dataset/cifar10.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1356 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/dataset/imagenet.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    35379 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/dataset/imagenet_class_index.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi/models/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      179 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/models/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      734 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/models/inceptionv3.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      716 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/models/resnet50.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     5626 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/models/vgg16.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi/static/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)    10865 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/static/font.js
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     9955 2023-05-29 15:32:44.000000 deepapi-0.4.3/deepapi/static/index.html
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     7880 2023-05-29 15:32:44.000000 deepapi-0.4.3/deepapi/static/script.js
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2158 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/static/simpleSnackbar.min.css
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     8740 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/static/simpleSnackbar.min.js
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2139 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/static/style.css
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2677 2023-05-29 15:32:19.000000 deepapi-0.4.3/deepapi/static/upload.js
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi/utils/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       53 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/utils/__init__.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1789 2023-05-29 14:34:06.000000 deepapi-0.4.3/deepapi/utils/response.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi.egg-info/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     3330 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi.egg-info/PKG-INFO
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      860 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        1 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       47 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi.egg-info/entry_points.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      103 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi.egg-info/requires.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)        8 2023-05-29 15:35:48.000000 deepapi-0.4.3/deepapi.egg-info/top_level.txt
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1260 2023-05-29 15:34:43.000000 deepapi-0.4.3/pyproject.toml
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)       38 2023-05-29 15:35:48.000000 deepapi-0.4.3/setup.cfg
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2280 2023-05-29 15:32:44.000000 deepapi-0.4.3/setup.py
+drwxrwxr-x   0 wuhanstudio  (1000) wuhanstudio  (1000)        0 2023-05-29 15:35:48.000000 deepapi-0.4.3/test/
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)      389 2023-05-29 15:32:44.000000 deepapi-0.4.3/test/test_deepapi.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     1886 2023-05-29 15:32:44.000000 deepapi-0.4.3/test/test_minimal.py
+-rw-rw-r--   0 wuhanstudio  (1000) wuhanstudio  (1000)     2978 2023-05-29 15:32:44.000000 deepapi-0.4.3/test/test_multi_client.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `deepapi-0.4.2/LICENSE` & `deepapi-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/PKG-INFO` & `deepapi-0.4.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepapi
-Version: 0.4.2
+Version: 0.4.3
 Summary: Deep Learning as a Cloud API Service.
 Home-page: https://github.com/wuhanstudio/deepapi
 Author: wuhanstudio
 Author-email: wuhanstudio <wuhanstudios@gmail.com>
 Maintainer: wuhanstudio
 Maintainer-email: wuhanstudio <wuhanstudios@gmail.com>
 License: MIT License
@@ -35,28 +35,33 @@
 ```
 
 #### Python 3:
 
 ```
 $ pip install deepapi
 
+# For development
+# python setup.py develop
+
 # By default, we enable all models on the server.
 # Use deepapi -h to see more options.
 
 $ python -m deepapi
 Serving on port 8080...
 ```
 
 The website and API service are available at https://localhost:8080.
 
 
 
 ### DeepAPI Client
 
-To initiate **black-box adversarial attacks**, we can get predictions by sending a POST request to http://localhost:8080/vgg16_cifar10 without knowing details about deep learning models behind the cloud service.
+To initiate **black-box adversarial attacks**, we can get predictions from a cloud API using `model.predict()`.
+
+Behind the scene, this `model` makes predictions by sending a POST request to http://localhost:8080/vgg16_cifar10.
 
 ```
 import numpy as np
 from PIL import Image
 
 from deepapi.api import DeepAPI_VGG16_Cifar10
```

### Comparing `deepapi-0.4.2/README.md` & `deepapi-0.4.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,28 +16,33 @@
 ```
 
 #### Python 3:
 
 ```
 $ pip install deepapi
 
+# For development
+# python setup.py develop
+
 # By default, we enable all models on the server.
 # Use deepapi -h to see more options.
 
 $ python -m deepapi
 Serving on port 8080...
 ```
 
 The website and API service are available at https://localhost:8080.
 
 
 
 ### DeepAPI Client
 
-To initiate **black-box adversarial attacks**, we can get predictions by sending a POST request to http://localhost:8080/vgg16_cifar10 without knowing details about deep learning models behind the cloud service.
+To initiate **black-box adversarial attacks**, we can get predictions from a cloud API using `model.predict()`.
+
+Behind the scene, this `model` makes predictions by sending a POST request to http://localhost:8080/vgg16_cifar10.
 
 ```
 import numpy as np
 from PIL import Image
 
 from deepapi.api import DeepAPI_VGG16_Cifar10
```

### Comparing `deepapi-0.4.2/deepapi/_main.py` & `deepapi-0.4.3/deepapi/_main.py`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/api/__init__.py` & `deepapi-0.4.3/deepapi/api/__init__.py`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/dataset/imagenet.py` & `deepapi-0.4.3/deepapi/dataset/imagenet.py`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/dataset/imagenet_class_index.py` & `deepapi-0.4.3/deepapi/dataset/imagenet_class_index.py`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/models/inceptionv3.py` & `deepapi-0.4.3/deepapi/models/inceptionv3.py`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/models/resnet50.py` & `deepapi-0.4.3/deepapi/models/resnet50.py`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/models/vgg16.py` & `deepapi-0.4.3/deepapi/models/vgg16.py`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/static/font.js` & `deepapi-0.4.3/deepapi/static/font.js`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/static/index.html` & `deepapi-0.4.3/deepapi/static/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -138,29 +138,27 @@
         </div>
     </div>
 
     <div class="container mb-5" id="prediction">
         <div class="row">
             <div class="col col-12">
                 <h1 class="h1 text-center">Predictions</h1>
-                <div id="with-prob">
-                    <div>
-                        <canvas id="myChart"></canvas>
-                    </div>
+                <div id="with-prob" style="position: relative; height:60vh;">
+                    <canvas id="myChart"></canvas>
                 </div>
                 <div id="no-prob">
 
                 </div>
             </div>
         </div>
     </div>
 
-    <div class="container mb-5" id="codegen">
+    <div class="container mb-5 mx-auto" id="codegen">
         <div class="row">
-            <div class="col col-12">
+            <div class="col-12">
                 <h1 class="h1 text-center">API Client</h1>
                 <ul class="nav nav-tabs" id="myTab" role="tablist">
                     <li class="nav-item" role="presentation">
                         <button class="nav-link active" id="python-tab" data-bs-toggle="tab" data-bs-target="#python" type="button" role="tab" aria-controls="python" aria-selected="true">Python</button>
                     </li>
                     <li class="nav-item" role="presentation">
                         <button class="nav-link" id="curl-tab" data-bs-toggle="tab" data-bs-target="#curl" type="button" role="tab" aria-controls="curl" aria-selected="false">Curl</button>
```

### Comparing `deepapi-0.4.2/deepapi/static/script.js` & `deepapi-0.4.3/deepapi/static/script.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,13 +1,15 @@
 var myChart = new Chart(
     document.getElementById('myChart'), {
         type: 'bar',
         data: [],
         options: {
+            responsive: true,
             indexAxis: 'y',
+            maintainAspectRatio: false,
         }
     }
 );
 
 var model = '';
 var dataset = '';
 var topk = 10;
```

### Comparing `deepapi-0.4.2/deepapi/static/simpleSnackbar.min.css` & `deepapi-0.4.3/deepapi/static/simpleSnackbar.min.css`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/static/simpleSnackbar.min.js` & `deepapi-0.4.3/deepapi/static/simpleSnackbar.min.js`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/static/style.css` & `deepapi-0.4.3/deepapi/static/style.css`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/static/upload.js` & `deepapi-0.4.3/deepapi/static/upload.js`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi/utils/response.py` & `deepapi-0.4.3/deepapi/utils/response.py`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/deepapi.egg-info/PKG-INFO` & `deepapi-0.4.3/deepapi.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepapi
-Version: 0.4.2
+Version: 0.4.3
 Summary: Deep Learning as a Cloud API Service.
 Home-page: https://github.com/wuhanstudio/deepapi
 Author: wuhanstudio
 Author-email: wuhanstudio <wuhanstudios@gmail.com>
 Maintainer: wuhanstudio
 Maintainer-email: wuhanstudio <wuhanstudios@gmail.com>
 License: MIT License
@@ -35,28 +35,33 @@
 ```
 
 #### Python 3:
 
 ```
 $ pip install deepapi
 
+# For development
+# python setup.py develop
+
 # By default, we enable all models on the server.
 # Use deepapi -h to see more options.
 
 $ python -m deepapi
 Serving on port 8080...
 ```
 
 The website and API service are available at https://localhost:8080.
 
 
 
 ### DeepAPI Client
 
-To initiate **black-box adversarial attacks**, we can get predictions by sending a POST request to http://localhost:8080/vgg16_cifar10 without knowing details about deep learning models behind the cloud service.
+To initiate **black-box adversarial attacks**, we can get predictions from a cloud API using `model.predict()`.
+
+Behind the scene, this `model` makes predictions by sending a POST request to http://localhost:8080/vgg16_cifar10.
 
 ```
 import numpy as np
 from PIL import Image
 
 from deepapi.api import DeepAPI_VGG16_Cifar10
```

### Comparing `deepapi-0.4.2/deepapi.egg-info/SOURCES.txt` & `deepapi-0.4.3/deepapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/pyproject.toml` & `deepapi-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
             "requests",
             "tensorflow",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "deepapi"
-version = "0.4.2"
+version = "0.4.3"
 authors = [
   { name="wuhanstudio", email="wuhanstudios@gmail.com" },
 ]
 maintainers = [
   { name="wuhanstudio", email="wuhanstudios@gmail.com" },
 ]
 description = "Deep Learning as a Cloud API Service."
```

### Comparing `deepapi-0.4.2/setup.py` & `deepapi-0.4.3/setup.py`

 * *Files identical despite different names*

### Comparing `deepapi-0.4.2/test/test_minimal.py` & `deepapi-0.4.3/test/test_minimal.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,26 +9,37 @@
 import base64
 
 import argparse
 
 def classification(url, file):
 
     # Load the input image and construct the payload for the request
-    image = Image.open(file)
+    try:
+        image = Image.open(file)
+    except Exception as e:
+        print(e)
+        return
+
     buff = BytesIO()
     image.save(buff, format="JPEG")
 
     print('Sending requests')
     data = {'file': base64.b64encode(buff.getvalue()).decode("utf-8")}
 
     return  requests.post(url, json=data).json()
 
 
 parser = argparse.ArgumentParser(description='Distributed Image Classification Client')
 parser.add_argument(
+    '--image',
+    type=str,
+    help='image file',
+    default='cat.jpg'
+)
+parser.add_argument(
     '--url',
     type=str,
     help='API url',
     default='http://localhost:8080'
 )
 parser.add_argument(
     '--top',
@@ -47,15 +58,19 @@
 parser.add_argument('--no-prob', dest='no_prob', action='store_true')
 parser.set_defaults(no_prob=False)
 
 args = parser.parse_args()
 
 no_prob = 1 if args.no_prob else 0;
 
-res = classification(args.url + '/' + args.model + '?top=' + str(args.top) + '&no-prob=' + str(no_prob), 'cat.jpg')
+res = classification(args.url + '/' + args.model + '?top=' + str(args.top) + '&no-prob=' + str(no_prob), args.image)
+
+if res is None:
+    print('No response')
+    exit()
 
 # Print prediction results
 if res['success']:
     if no_prob == 0:
         res = sorted(res['predictions'], key=itemgetter('probability'), reverse=True)
         for i in res:
             print('{:<15s}{:.5f}'.format(i['label'], i['probability']))
```

### Comparing `deepapi-0.4.2/test/test_multi_client.py` & `deepapi-0.4.3/test/test_multi_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 from PIL import Image
 from io import BytesIO
 import base64
 
 def classification(url, file):
 
     # load the input image and construct the payload for the request
-    image = Image.open(file)
+    try:
+        image = Image.open(file)
+    except Exception as e:
+        print(e)
+        return
+
     buff = BytesIO()
     image.save(buff, format="JPEG")
 
     print('Sending requests')
     data = {'file': base64.b64encode(buff.getvalue()).decode("utf-8")}
 
     return requests.post(url, json=data).json()
@@ -36,17 +41,18 @@
         print(e)
 
     return r, (time.time() - start_time)
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser(description='Distributed Image Classification API')
     parser.add_argument(
-        'image',
+        '--image',
         type=str,
-        help='image file'
+        help='image file',
+        default='cat.jpg'
     )
     parser.add_argument(
         '--url',
         type=str,
         help='API url',
         default='http://localhost:8080'
     )
@@ -82,19 +88,25 @@
     with concurrent.futures.ProcessPoolExecutor(max_workers=num_workers) as executor:
         futures = {executor.submit(task, args.url + '/' + args.model + '?top=' + str(args.top) + '&no-prob=' + str(no_prob), args.image) for i in range(num_workers)}
 
         print('----- start -----')
         start_time = time.time()
         for future in concurrent.futures.as_completed(futures):
             r, data = future.result()
+
+            if r is None:
+                print('No response')
+                continue
+
             if(r['success']):
                 if no_prob:
                     print ('{:<15s}'.format(r['predictions'][0]['label']))
                 else:
                     r = sorted(r['predictions'], key=itemgetter('probability'), reverse=True)
                     print ('{:<15s}{:.5f}'.format(r[0]['label'], r[0]['probability']))
             else:
                 print(r['error'])
+
         print('------ end ------')
 
         print('Concurrent Requests: ' + str(num_workers))
         print('Total Runtime: ' + str(time.time() - start_time))
```


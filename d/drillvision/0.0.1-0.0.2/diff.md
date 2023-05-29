# Comparing `tmp/drillvision-0.0.1.tar.gz` & `tmp/drillvision-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/drillvision-0.0.1.tar", last modified: Sun May 21 21:50:10 2023, max compression
+gzip compressed data, was "dist/drillvision-0.0.2.tar", last modified: Mon May 29 04:04:59 2023, max compression
```

## Comparing `drillvision-0.0.1.tar` & `drillvision-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-21 21:50:10.841205 drillvision-0.0.1/
--rw-r--r--   0 amin       (501) staff       (20)      305 2023-05-21 20:38:44.000000 drillvision-0.0.1/MANIFEST.in
--rw-r--r--   0 amin       (501) staff       (20)     6372 2023-05-21 21:50:10.840862 drillvision-0.0.1/PKG-INFO
--rw-r--r--   0 amin       (501) staff       (20)     5601 2023-05-16 02:02:49.000000 drillvision-0.0.1/README.md
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-21 21:50:10.838687 drillvision-0.0.1/drillvision.egg-info/
--rw-r--r--   0 amin       (501) staff       (20)     6372 2023-05-21 21:50:10.000000 drillvision-0.0.1/drillvision.egg-info/PKG-INFO
--rw-r--r--   0 amin       (501) staff       (20)      747 2023-05-21 21:50:10.000000 drillvision-0.0.1/drillvision.egg-info/SOURCES.txt
--rw-r--r--   0 amin       (501) staff       (20)        1 2023-05-21 21:50:10.000000 drillvision-0.0.1/drillvision.egg-info/dependency_links.txt
--rw-r--r--   0 amin       (501) staff       (20)      203 2023-05-21 21:50:10.000000 drillvision-0.0.1/drillvision.egg-info/requires.txt
--rw-r--r--   0 amin       (501) staff       (20)       21 2023-05-21 21:50:10.000000 drillvision-0.0.1/drillvision.egg-info/top_level.txt
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-21 21:50:10.836342 drillvision-0.0.1/neural_network_model/
--rw-r--r--   0 amin       (501) staff       (20)        5 2023-05-21 20:04:57.000000 drillvision-0.0.1/neural_network_model/VERSION
--rw-r--r--   0 amin       (501) staff       (20)        0 2023-05-16 02:02:49.000000 drillvision-0.0.1/neural_network_model/__init__.py
--rw-r--r--   0 amin       (501) staff       (20)    20505 2023-05-21 03:47:02.000000 drillvision-0.0.1/neural_network_model/bit_vision.py
--rw-r--r--   0 amin       (501) staff       (20)     5918 2023-05-21 21:31:27.000000 drillvision-0.0.1/neural_network_model/model.py
--rw-r--r--   0 amin       (501) staff       (20)    13281 2023-05-21 03:47:02.000000 drillvision-0.0.1/neural_network_model/process_data.py
--rw-r--r--   0 amin       (501) staff       (20)     2843 2023-05-20 18:27:45.000000 drillvision-0.0.1/neural_network_model/s3.py
--rw-r--r--   0 amin       (501) staff       (20)     1913 2023-05-21 20:09:15.000000 drillvision-0.0.1/pyproject.toml
--rw-r--r--   0 amin       (501) staff       (20)       97 2023-05-13 20:20:47.000000 drillvision-0.0.1/requirements-test.txt
--rw-r--r--   0 amin       (501) staff       (20)      202 2023-05-21 21:27:49.000000 drillvision-0.0.1/requirements.txt
--rw-r--r--   0 amin       (501) staff       (20)       38 2023-05-21 21:50:10.841331 drillvision-0.0.1/setup.cfg
--rw-r--r--   0 amin       (501) staff       (20)     2271 2023-05-21 21:46:41.000000 drillvision-0.0.1/setup.py
-drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-21 21:50:10.840299 drillvision-0.0.1/tests/
--rw-r--r--   0 amin       (501) staff       (20)      346 2023-05-20 18:27:45.000000 drillvision-0.0.1/tests/test_bitvision.py
--rw-r--r--   0 amin       (501) staff       (20)     3023 2023-05-20 18:27:45.000000 drillvision-0.0.1/tests/test_preprocessing.py
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-29 04:04:59.273536 drillvision-0.0.2/
+-rw-r--r--   0 amin       (501) staff       (20)      305 2023-05-21 20:38:44.000000 drillvision-0.0.2/MANIFEST.in
+-rw-r--r--   0 amin       (501) staff       (20)     6322 2023-05-29 04:04:59.272381 drillvision-0.0.2/PKG-INFO
+-rw-r--r--   0 amin       (501) staff       (20)     5699 2023-05-22 03:34:53.000000 drillvision-0.0.2/README.md
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-29 04:04:59.269879 drillvision-0.0.2/drillvision.egg-info/
+-rw-r--r--   0 amin       (501) staff       (20)     6322 2023-05-29 04:04:59.000000 drillvision-0.0.2/drillvision.egg-info/PKG-INFO
+-rw-r--r--   0 amin       (501) staff       (20)      747 2023-05-29 04:04:59.000000 drillvision-0.0.2/drillvision.egg-info/SOURCES.txt
+-rw-r--r--   0 amin       (501) staff       (20)        1 2023-05-29 04:04:59.000000 drillvision-0.0.2/drillvision.egg-info/dependency_links.txt
+-rw-r--r--   0 amin       (501) staff       (20)      227 2023-05-29 04:04:59.000000 drillvision-0.0.2/drillvision.egg-info/requires.txt
+-rw-r--r--   0 amin       (501) staff       (20)       21 2023-05-29 04:04:59.000000 drillvision-0.0.2/drillvision.egg-info/top_level.txt
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-29 04:04:59.267434 drillvision-0.0.2/neural_network_model/
+-rw-r--r--   0 amin       (501) staff       (20)        5 2023-05-29 04:04:29.000000 drillvision-0.0.2/neural_network_model/VERSION
+-rw-r--r--   0 amin       (501) staff       (20)        0 2023-05-16 02:02:49.000000 drillvision-0.0.2/neural_network_model/__init__.py
+-rw-r--r--   0 amin       (501) staff       (20)    21716 2023-05-29 03:59:31.000000 drillvision-0.0.2/neural_network_model/bit_vision.py
+-rw-r--r--   0 amin       (501) staff       (20)     5962 2023-05-29 03:59:31.000000 drillvision-0.0.2/neural_network_model/model.py
+-rw-r--r--   0 amin       (501) staff       (20)    14713 2023-05-25 23:15:08.000000 drillvision-0.0.2/neural_network_model/process_data.py
+-rw-r--r--   0 amin       (501) staff       (20)     2843 2023-05-20 18:27:45.000000 drillvision-0.0.2/neural_network_model/s3.py
+-rw-r--r--   0 amin       (501) staff       (20)     1913 2023-05-21 20:09:15.000000 drillvision-0.0.2/pyproject.toml
+-rw-r--r--   0 amin       (501) staff       (20)       97 2023-05-13 20:20:47.000000 drillvision-0.0.2/requirements-test.txt
+-rw-r--r--   0 amin       (501) staff       (20)      228 2023-05-24 01:47:09.000000 drillvision-0.0.2/requirements.txt
+-rw-r--r--   0 amin       (501) staff       (20)       38 2023-05-29 04:04:59.273931 drillvision-0.0.2/setup.cfg
+-rw-r--r--   0 amin       (501) staff       (20)     2128 2023-05-29 03:58:58.000000 drillvision-0.0.2/setup.py
+drwxr-xr-x   0 amin       (501) staff       (20)        0 2023-05-29 04:04:59.271494 drillvision-0.0.2/tests/
+-rw-r--r--   0 amin       (501) staff       (20)      346 2023-05-20 18:27:45.000000 drillvision-0.0.2/tests/test_bitvision.py
+-rw-r--r--   0 amin       (501) staff       (20)     3023 2023-05-20 18:27:45.000000 drillvision-0.0.2/tests/test_preprocessing.py
```

### Comparing `drillvision-0.0.1/PKG-INFO` & `drillvision-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.0.1
+Version: 0.0.2
 Summary: # Drill Bit Classifier
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # Drill Bit Classifier
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![PyPI version](https://badge.fury.io/py/drillvision.svg)](https://badge.fury.io/py/drillvision)
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
```

### Comparing `drillvision-0.0.1/README.md` & `drillvision-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Drill Bit Classifier
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![PyPI version](https://badge.fury.io/py/drillvision.svg)](https://badge.fury.io/py/drillvision)
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
```

### Comparing `drillvision-0.0.1/drillvision.egg-info/PKG-INFO` & `drillvision-0.0.2/drillvision.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 Metadata-Version: 2.1
 Name: drillvision
-Version: 0.0.1
+Version: 0.0.2
 Summary: # Drill Bit Classifier
 Home-page: https://github.com/Atashnezhad/DrillBitVision
 Author: Amin Atashnezhad
 Author-email: atashnezhad2@gmail.com
 License: BSD-3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.6.0
 Description-Content-Type: text/markdown
 
 # Drill Bit Classifier
 [![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)](https://www.python.org/downloads/release/python-360/)
+[![PyPI version](https://badge.fury.io/py/drillvision.svg)](https://badge.fury.io/py/drillvision)
 
 The Drill Bit Classifier is an app that uses a Convolutional Neural Network (CNN) to 
 classify images of drill bits. The app can be used by machinists and engineers to 
 quickly and accurately identify the type of drill bit required for a particular job.
 
 ## Description:
 ### Preprocessing Module
```

### Comparing `drillvision-0.0.1/drillvision.egg-info/SOURCES.txt` & `drillvision-0.0.2/drillvision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.1/neural_network_model/bit_vision.py` & `drillvision-0.0.2/neural_network_model/bit_vision.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,54 @@
 import logging
 import random
 
 from keras import Sequential
-from keras.layers import (BatchNormalization, Conv2D, Dense, Dropout, Flatten,
-                          MaxPooling2D)
+from keras.layers import (
+    BatchNormalization,
+    Conv2D,
+    Dense,
+    Dropout,
+    Flatten,
+    MaxPooling2D,
+)
 
 from neural_network_model.model import SETTING
 
 # set seed to get the same random numbers each time
 random.seed(1)
 
 import os
 import warnings
 from pathlib import Path
 from typing import Dict, List
 
 # from tensorflow.keras.callbacks import ModelCheckpoint
 from keras.callbacks import ModelCheckpoint
-from tensorflow.keras.applications.resnet50 import (decode_predictions,
-                                                    preprocess_input)
+from tensorflow.keras.applications.resnet50 import decode_predictions, preprocess_input
 
 warnings.filterwarnings("ignore")
 
 import numpy as np
 import tensorflow
 from tensorflow import keras
 
 warnings.filterwarnings("ignore")
 
 import matplotlib.cm as cm
 import matplotlib.pyplot as plt
 import tensorflow as tf
+
 # Display
 from tensorflow import keras
 from tensorflow.keras.preprocessing import image
-from tensorflow.keras.preprocessing.image import (ImageDataGenerator,
-                                                  img_to_array, load_img)
+from tensorflow.keras.preprocessing.image import (
+    ImageDataGenerator,
+    img_to_array,
+    load_img,
+)
 
 # Initialize the logger
 logger = logging.getLogger()
 logger.setLevel(logging.INFO)
 # Create console handler
 ch = logging.StreamHandler()
 ch.setLevel(logging.INFO)
@@ -60,57 +69,60 @@
     def __init__(self, *args, **kwargs):
         self.train_test_val_dir: str = kwargs.get(
             "train_test_val_dir",
             SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS,
         )
         self.model: tensorflow.keras.models.Sequential = None
         self.assemble_deep_net_model()
-        self.train_vali_gens = {}
+        self.train_val_gens = {}
         self.model_history = None
         self.model_class_indices: Dict[str, int] = {}
 
     @property
     def categories(self) -> List[str]:
         """
         This function returns the list of categories.
         :return: list of categories
         """
         # get the list of dirs in the resource_dir
         subdir_name = os.listdir(self.train_test_val_dir)
         # check if there is .DS_Store in the subdir_name if so remove it
-        subdir_name = self.filter_out_list(list_to_be_edited=subdir_name)
+        subdir_name = self._filter_out_list(list_to_be_edited=subdir_name)
         subdir_path = self.train_test_val_dir / subdir_name[0]
         categories_name = os.listdir(subdir_path)
         # filter the list of categories if there is a case in the IGNORE_LIST
-        categories_name = self.filter_out_list(list_to_be_edited=categories_name)
+        categories_name = self._filter_out_list(list_to_be_edited=categories_name)
         return categories_name
 
     @property
     def data_details(self) -> Dict[str, Dict[str, int]]:
         """
         This property check the dirs and make a dict and save the
         train test val data details in the dict.
         """
-        resource_dir = Path(__file__).parent / ".." / self.train_test_val_dir
+        resource_dir = (
+            self.train_test_val_dir
+            or Path(__file__).parent / ".." / self.train_test_val_dir
+        )
         # get the list of dirs in the resource_dir
         subdir_name = os.listdir(resource_dir)
         # check if there is .DS_Store in the subdir_name if so remove it
-        subdir_name = self.filter_out_list(list_to_be_edited=subdir_name)
+        subdir_name = self._filter_out_list(list_to_be_edited=subdir_name)
         data = {}
         # for each subdir in the resource_dir, get the list of files
         for subdir in subdir_name:
             data[subdir] = {}
             subdir_path = resource_dir / subdir
-            subdir_path_lisr = self.filter_out_list(
+            subdir_path_lisr = self._filter_out_list(
                 list_to_be_edited=os.listdir(subdir_path)
             )
             for category in subdir_path_lisr:
                 category_path = subdir_path / category
                 #  check if there is .DS_Store in the subdir_name if so remove it
-                # category_path = self.filter_out_list(list_to_be_edited=category_path)
+                # category_path = self._filter_out_list(list_to_be_edited=category_path)
                 # for each file in the category, find the number of files
                 num_files = len(os.listdir(category_path))
                 # logger.info(f"Number of files in {category_path.resolve()} is {num_files}")
                 data[subdir][category] = num_files
         return data
 
     def assemble_deep_net_model(self) -> tensorflow.keras.models.Sequential:
@@ -185,15 +197,16 @@
         Here we just rescale them.
         """
         my_list = ["train", "val"]
         for subdir in my_list:
             datagen = image.ImageDataGenerator(rescale=SETTING.DATA_GEN_SETTING.RESCALE)
 
             generator = datagen.flow_from_directory(
-                directory=SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
+                directory=self.train_test_val_dir / subdir
+                or SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
                 / subdir,
                 target_size=SETTING.FLOW_FROM_DIRECTORY_SETTING.TARGET_SIZE,
                 color_mode=SETTING.FLOW_FROM_DIRECTORY_SETTING.COLOR_MODE,
                 classes=None,
                 class_mode=SETTING.FLOW_FROM_DIRECTORY_SETTING.CLASS_MODE,
                 batch_size=SETTING.FLOW_FROM_DIRECTORY_SETTING.BATCH_SIZE,
                 shuffle=True,
@@ -201,54 +214,62 @@
                 save_to_dir=None,
                 save_prefix="",
                 save_format="png",
                 follow_links=False,
                 subset=None,
                 interpolation="nearest",
             )
-            self.train_vali_gens[subdir] = generator
+            self.train_val_gens[subdir] = generator
             self.model_class_indices = dict(
                 zip(generator.class_indices.values(), generator.class_indices.keys())
             )
 
             logger.info(f"Rescaling {subdir} data, {generator.class_indices}:")
 
-    def check_points(self) -> ModelCheckpoint:
-        check_points = ModelCheckpoint(
+    def _check_points(self) -> ModelCheckpoint:
+        check_point = ModelCheckpoint(
             SETTING.MODEL_SETTING.MODEL_PATH,
             monitor=SETTING.MODEL_SETTING.MONITOR,
             verbose=SETTING.MODEL_SETTING.CHECK_POINT_VERBOSE,
             save_best_only=SETTING.MODEL_SETTING.SAVE_BEST_ONLY,
             mode=SETTING.MODEL_SETTING.MODE,
             # period=SETTING.MODEL_SETTING.PERIOD,
         )
-        return check_points
+        return check_point
 
-    def train_model(self):
+    def train_model(self, model_save_address: str = None):
         self._rescaling()
         model_history = self.model.fit_generator(
-            generator=self.train_vali_gens["train"],
+            generator=self.train_val_gens["train"],
             epochs=SETTING.MODEL_SETTING.EPOCHS,
             verbose=SETTING.MODEL_SETTING.FIT_GEN_VERBOSE,
-            validation_data=self.train_vali_gens["val"],
+            validation_data=self.train_val_gens["val"],
             validation_steps=SETTING.MODEL_SETTING.VALIDATION_STEPS,
             class_weight=SETTING.MODEL_SETTING.CLASS_WEIGHT,
             max_queue_size=SETTING.MODEL_SETTING.MAX_QUEUE_SIZE,
             workers=SETTING.MODEL_SETTING.WORKERS,
             use_multiprocessing=SETTING.MODEL_SETTING.USE_MULTIPROCESSING,
             shuffle=SETTING.MODEL_SETTING.SHUFFLE,
             initial_epoch=SETTING.MODEL_SETTING.INITIAL_EPOCH,
-            callbacks=[self.check_points()],
+            callbacks=[self._check_points()],
         )
 
-        self.model.save(SETTING.MODEL_SETTING.MODEL_PATH)
+        self.model.save(model_save_address or SETTING.MODEL_SETTING.MODEL_PATH)
         logger.info(f"Model saved to {SETTING.MODEL_SETTING.MODEL_PATH}")
         self.model_history = model_history
 
-    def plot_history(self):
+    def plot_history(self, *args, **kwargs):
+        """
+        This function is used to plot the history of the model.
+        :param fig_folder_address: the address of the folder to save the figure
+        :return:
+        """
+        fig_folder_address = kwargs.get(
+            "fig_folder_address", SETTING.FIGURE_SETTING.FIG_PRED_OUT_DIR_ADDRESS
+        )
         logger.info(self.model_history.history.keys())
         keys_plot = ["loss", "accuracy"]
         # make two plots side by side and have train and val for loss and accuracy
         fig, axs = plt.subplots(
             SETTING.FIGURE_SETTING.NUM_ROWS_IN_PLOT_HIST,
             SETTING.FIGURE_SETTING.NUM_COLS_IN_PLOT_HIST,
             figsize=SETTING.FIGURE_SETTING.FIGURE_SIZE_IN_PLOT_HIST,
@@ -256,56 +277,67 @@
         for i, key in enumerate(keys_plot):
             axs[i].plot(self.model_history.history[key], color="red")
             axs[i].plot(self.model_history.history[f"val_{key}"], color="green")
             axs[i].set_title(f"model {key}")
             axs[i].set_ylabel(key)
             axs[i].set_xlabel("epoch")
             axs[i].legend(["train", "val"], loc="upper left")
-        fig_path = (
-            SETTING.FIGURE_SETTING.FIG_PRED_OUT_DIR_ADDRESS / "history.png"
-        ).resolve()
+        fig_path = (fig_folder_address / "history.png").resolve()
         plt.savefig(fig_path)
         plt.show()
 
     @staticmethod
-    def filter_out_list(
-        filter_out_list: List[str] = SETTING.IGNORE_SETTING.IGNORE_LIST,
+    def _filter_out_list(
+        ignore_list: List[str] = SETTING.IGNORE_SETTING.IGNORE_LIST,
         list_to_be_edited: List[str] = None,
     ) -> List[str]:
-        for case in filter_out_list:
+        for case in ignore_list:
             if case in list_to_be_edited:
                 list_to_be_edited.remove(case)
         return list_to_be_edited
 
     def predict(self, *args, **kwargs):
+        """
+        This function is used to predict the test data.
+        :param args:
+        :param kwargs: fid_save_address: the address of the folder to save the figure,
+        model_path: the path of the model to be used for prediction
+        :return:
+        """
+        fid_save_address = kwargs.get(
+            "fid_save_address", SETTING.FIGURE_SETTING.FIG_PRED_OUT_DIR_ADDRESS
+        )
         model_path = kwargs.get("model_path", SETTING.MODEL_SETTING.MODEL_PATH)
         if model_path is None:
             raise ValueError("model_path is None")
 
         model = keras.models.load_model(model_path)
         logger.info(f"Model loaded from {model_path}")
 
         for category in self.categories:
             plt.figure(figsize=SETTING.FIGURE_SETTING.FIGURE_SIZE_IN_PRED_MODEL)
             number_of_cols = SETTING.FIGURE_SETTING.NUM_COLS_IN_PRED_MODEL
             number_of_rows = SETTING.FIGURE_SETTING.NUM_ROWS_IN_PRED_MODEL
             number_of_test_to_pred = SETTING.MODEL_SETTING.NUMBER_OF_TEST_TO_PRED
-
+            train_test_val_dir = (
+                self.train_test_val_dir
+                or SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
+            )
             # get the list of test images
             test_images_list = os.listdir(
-                SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
+                train_test_val_dir
                 / SETTING.PREPROCESSING_SETTING.TRAIN_TEST_SPLIT_DIR_NAMES[1]
                 / category
             )
             # check if .DS_Store is in the list if so remove it
-            test_images_list = self.filter_out_list(list_to_be_edited=test_images_list)
+            test_images_list = self._filter_out_list(list_to_be_edited=test_images_list)
 
             for i, img in enumerate(test_images_list[0:number_of_test_to_pred]):
                 path_to_img = (
-                    SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
+                    train_test_val_dir
                     / SETTING.PREPROCESSING_SETTING.TRAIN_TEST_SPLIT_DIR_NAMES[1]
                     / category
                     / str(img)
                 ).resolve()
 
                 img = load_img(
                     path_to_img,
@@ -333,17 +365,15 @@
                     ax.set_title(
                         f"{self.model_class_indices.get(prediction[0])}",
                         color="red",
                     )
 
             # save the figure in the figures folder
             fig_name = f"prediction_{category}.png"
-            fig_path = (
-                SETTING.FIGURE_SETTING.FIG_PRED_OUT_DIR_ADDRESS / fig_name
-            ).resolve()
+            fig_path = (fid_save_address / fig_name).resolve()
             if not os.path.exists(fig_path.parent):
                 os.makedirs(fig_path.parent)
             plt.savefig(fig_path)
             plt.show()
             plt.tight_layout()
 
         datagen = image.ImageDataGenerator(SETTING.DATA_GEN_SETTING.RESCALE)
@@ -362,29 +392,37 @@
             follow_links=False,
             subset=None,
             interpolation="nearest",
         )
 
         model.evaluate(DoubleCheck_generator)
 
+    # TODO: check the addresses and add as kwargs if needed
     def grad_cam_viz(self, *args, **kwargs):
         model_path = kwargs.get("model_path", SETTING.MODEL_SETTING.MODEL_PATH)
+        fig_to_save_address = kwargs.get(
+            "fig_to_save_address", SETTING.GRAD_CAM_SETTING.IMAGE_NEW_NAME
+        )
+        gradcam_fig_name = kwargs.get(
+            "gradcam_fig_name", SETTING.GRAD_CAM_SETTING.GRAD_CAM_FIG_NAME
+        )
+        fig_address = fig_to_save_address / gradcam_fig_name
         if model_path is None:
             raise ValueError("model_path is None")
 
         model = keras.models.load_model(model_path)
         logger.info(f"Model loaded from {model_path}")
 
         # print the model layers
         for idx in range(len(model.layers)):
             print(model.get_layer(index=idx).name)
 
-        model_builder = keras.applications.xception.Xception
+        # model_builder = keras.applications.xception.Xception
         preprocess_input = keras.applications.xception.preprocess_input
-        decode_predictions = keras.applications.xception.decode_predictions
+        # decode_predictions = keras.applications.xception.decode_predictions
 
         last_conv_layer_name = SETTING.GRAD_CAM_SETTING.LAST_CONV_LAYER_NAME
 
         # The local path to our target image
         img_path = SETTING.GRAD_CAM_SETTING.IMG_PATH
 
         # load the image and show it
@@ -411,17 +449,15 @@
         heatmap = BitVision._make_gradcam_heatmap(
             img_array, model, last_conv_layer_name
         )
 
         # Display heatmap
         plt.matshow(heatmap)
         plt.show()
-        BitVision._save_and_display_gradcam(
-            img_path, heatmap, cam_path=SETTING.GRAD_CAM_SETTING.IMAGE_NEW_NAME
-        )
+        BitVision._save_and_display_gradcam(img_path, heatmap, cam_path=fig_address)
 
     @staticmethod
     def _get_img_array(img_path, size):
         # `img` is a PIL image of size 299x299
         img = keras.preprocessing.image.load_img(img_path, target_size=size)
         # `array` is a float32 Numpy array of shape (299, 299, 3)
         array = keras.preprocessing.image.img_to_array(img)
@@ -496,16 +532,18 @@
         superimposed_img = keras.preprocessing.image.array_to_img(superimposed_img)
 
         # Save the superimposed image
         superimposed_img.save(cam_path)
 
 
 if __name__ == "__main__":
-    obj = BitVision()
-    # print(obj.categories)
-    # print(obj.data_details)
-    # obj.plot_image_category()
-    # obj.compile_model()
-    # obj.train_model()
-    # obj.plot_history()
-    # obj.predict()
-    obj.grad_cam_viz()
+    obj = BitVision(
+        train_test_val_dir=Path(__file__).parent / ".." / "dataset_train_test_val"
+    )
+    print(obj.categories)
+    print(obj.data_details)
+    obj.plot_image_category()
+    obj.compile_model()
+    obj.train_model()
+    obj.plot_history()
+    obj.predict()
+    obj.grad_cam_viz(gradcam_fig_name="test.png")
```

### Comparing `drillvision-0.0.1/neural_network_model/model.py` & `drillvision-0.0.2/neural_network_model/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,26 +7,26 @@
 from tensorflow import keras
 
 # Load environment variables from .env file
 load_dotenv()
 
 
 class DataAddressSetting(BaseModel):
-    MAIN_DATA_DIR_ADDRESS: str = Path(__file__).parent / ".." / "dataset"
+    MAIN_DATA_DIR_ADDRESS: str = (Path(__file__).parent / ".." / "dataset").resolve()
     TEST_DIR_ADDRESS: str = (
         Path(__file__).parent
         / ".."
         / "dataset_train_test_val"
         / "test"  # check the TRAIN_TEST_SPLIT_DIR_NAMES in
         # the PreprocessingSetting make sure test is in the list
     )
 
 
 class DownloadImageSetting(BaseModel):
-    LIMIT: int = 50
+    LIMIT: int = 5
 
 
 class AugmentationSetting(BaseModel):
     ROTATION_RANGE: int = 25
     WIDTH_SHIFT_RANGE: float = 0.0
     HEIGHT_SHIFT_RANGE: float = 0.0
     SHEAR_RANGE: float = 0.2
@@ -53,15 +53,15 @@
 class IgnoreSetting(BaseModel):
     IGNORE_LIST: list = [".DS_Store", ".pytest_cache", "__pycache__"]
 
 
 class PreprocessingSetting(BaseModel):
     TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS: str = (
         Path(__file__).parent / ".." / "dataset_train_test_val"
-    )
+    ).resolve()
     TRAIN_TEST_SPLIT_DIR_NAMES: list = ["train", "test", "val"]
     TRAIN_FRACTION: float = 0.7
     TEST_FRACTION: float = 0.2
     VAL_FRACTION: float = 0.1
 
 
 class ModelSetting(BaseModel):
@@ -127,17 +127,16 @@
     RESCALE: float = 1.0 / 255.0
 
 
 class GradCamSetting(BaseModel):
     IMG_PATH: str = Path(__file__).parent / ".." / "dataset" / "pdc_bit" / "Image_1.png"
 
     LAST_CONV_LAYER_NAME: str = "conv2d_2"
-    IMAGE_NEW_NAME: str = (
-        Path(__file__).parent / ".." / "figures" / "grad_cam_pdc_Image_1.png"
-    )
+    IMAGE_NEW_NAME: str = (Path(__file__).parent / ".." / "figures").resolve()
+    GRAD_CAM_FIG_NAME: str = "grad_cam_pdc_Image_1.png"
 
     ALPHA: float = 0.7
 
 
 class S3BucketSetting(BaseModel):
     BUCKET_NAME: str = "bitimages123"
     PARENT_FOLDER_NAME: str = "dataset"
```

### Comparing `drillvision-0.0.1/neural_network_model/process_data.py` & `drillvision-0.0.2/neural_network_model/process_data.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import logging
 import os
 import random
 import shutil
 
 from bing_image_downloader import downloader
 from tensorflow.keras.preprocessing import image
-from tensorflow.keras.preprocessing.image import (ImageDataGenerator,
-                                                  img_to_array, load_img)
+from tensorflow.keras.preprocessing.image import (
+    ImageDataGenerator,
+    img_to_array,
+    load_img,
+)
 
 from neural_network_model.model import SETTING
 from neural_network_model.s3 import MyS3
 
 # set seed to get the same random numbers each time
 random.seed(SETTING.RANDOM_SEED_SETTING.SEED)
 import random
+
 # import sys
 import warnings
 from pathlib import Path
 from typing import Any, Dict, List
 
 # import shutil
 from tqdm import tqdm
 
 warnings.filterwarnings("ignore")
 
-
 # Initialize the logger
 logger = logging.getLogger()
 logger.setLevel(logging.FATAL)
 # Create console handler
 ch = logging.StreamHandler()
 ch.setLevel(logging.FATAL)
 
-
 # Create formatter and add it to the handler
 formatter = logging.Formatter("%(asctime)s - %(levelname)s - %(message)s")
 ch.setFormatter(formatter)
 
 # Add the handler to the logger
 logger.addHandler(ch)
 
@@ -44,41 +46,56 @@
 class Preprocessing:
     """
     This class is used to train the neural network model.
     for the bit type detection.
     """
 
     def __init__(self, *args, **kwargs):
+        """
+        This function is used to initialize the class.
+        :param args:
+        :param kwargs:
+        """
         self.dataset_address = kwargs.get("dataset_address", None)
         self.categories_name_folders = None
 
-    @staticmethod
-    def download_images(category_list=None, from_s3=False) -> None:
+    def download_images(self, category_list=None, from_s3=False, limit=None) -> None:
+        """
+        This function is used to download the images from the internet.
+        :param category_list:
+        :param from_s3: bool
+        :param limit: int
+        :param download_location_address:
+        :return:
+        """
         if from_s3:
             # download the images from the S3 bucket
             s3 = MyS3()
 
             # Specify your bucket name and subfolders
             bucket_name = SETTING.S3_BUCKET_SETTING.BUCKET_NAME
             subfolders = SETTING.S3_BUCKET_SETTING.SUBFOLDER_NAME
-            download_location_address = SETTING.S3_BUCKET_SETTING.DOWNLOAD_LOCATION
+            download_location_address = (
+                self.dataset_address or SETTING.S3_BUCKET_SETTING.DOWNLOAD_LOCATION
+            )
 
             s3.download_files_from_subfolders(
                 bucket_name, subfolders, download_location_address
             )
             logger.info("Downloaded images from S3 bucket")
             return
 
         if category_list is None:
             category_list = SETTING.CATEGORY_SETTING.CATEGORIES
         for category in category_list:
             downloader.download(
                 category,
-                limit=SETTING.DOWNLOAD_IMAGE_SETTING.LIMIT,
-                output_dir=Path(__file__).parent / ".." / "dataset",
+                limit=limit or SETTING.DOWNLOAD_IMAGE_SETTING.LIMIT,
+                output_dir=self.dataset_address
+                or SETTING.DATA_ADDRESS_SETTING.MAIN_DATA_DIR_ADDRESS,
                 adult_filter_off=True,
                 force_replace=False,
                 timeout=120,
             )
         logger.info("Downloaded images")
 
     @property
@@ -94,15 +111,18 @@
         ]
         logger.info(self.categories_name_folders)
         logger.info(f"Categories name: {self.categories_name_folders}")
 
         # for images in each category dir, check if the image is in list_to_ignore, if yes remove from dir
         for category_folder in self.categories_name_folders:
             # read the files in the dataset folder
-            main_dataset_folder = Path(__file__).parent / ".." / "dataset"
+            main_dataset_folder = (
+                self.dataset_address
+                or SETTING.DATA_ADDRESS_SETTING.MAIN_DATA_DIR_ADDRESS
+            )
             data_address = main_dataset_folder / category_folder
 
             for file in os.listdir(data_address):
                 if file in list_to_ignore:
                     os.remove(data_address / file)
                     logger.info(f"Removed {file} from {category_folder}")
 
@@ -114,65 +134,66 @@
         This function reads the data from the dataset folder.
         and stores the data as a dict with categories and values in image_dict.
         :return:
         """
         image_dicts = {}
         for category_folder in self.categorie_name:
             # read the files in the dataset folder
-            main_dataset_folder = SETTING.DATA_ADDRESS_SETTING.MAIN_DATA_DIR_ADDRESS
+            main_dataset_folder = (
+                self.dataset_address
+                or SETTING.DATA_ADDRESS_SETTING.MAIN_DATA_DIR_ADDRESS
+            )
             data_address = main_dataset_folder / category_folder
             image_dicts[category_folder] = {}
             image_dicts[category_folder]["image_list"] = list(data_address.iterdir())
             image_dicts[category_folder]["number_of_images"] = len(
                 list(data_address.iterdir())
             )
 
         return image_dicts
 
     def augment_data(
         self,
         number_of_images_tobe_gen: int = SETTING.AUGMENTATION_SETTING.NUMBER_OF_IMAGES_TOBE_GENERATED,
+        augment_data_address: str = SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS,
     ):
         """
         This function augments the images and save them into the dataset_augmented folder.
         :param number_of_images_tobe_gen: number of images to be generated
+        :param augment_data_address: address to save the augmented images
         :return: None
         """
         Augment_data_gen = image.ImageDataGenerator(
             rotation_range=SETTING.AUGMENTATION_SETTING.ROTATION_RANGE,
             width_shift_range=SETTING.AUGMENTATION_SETTING.WIDTH_SHIFT_RANGE,
             height_shift_range=SETTING.AUGMENTATION_SETTING.HEIGHT_SHIFT_RANGE,
             shear_range=SETTING.AUGMENTATION_SETTING.SHEAR_RANGE,
             zoom_range=SETTING.AUGMENTATION_SETTING.ZOOM_RANGE,
             horizontal_flip=SETTING.AUGMENTATION_SETTING.HORIZONTAL_FLIP,
             fill_mode=SETTING.AUGMENTATION_SETTING.FILL_MODE,
         )
 
+        main_address = (
+            augment_data_address
+            or SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
+        )
+
         for image_category in self.image_dict.keys():
             # check if a dir dataset_augmented exists if not create it
-            if not os.path.exists(
-                SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
-                / image_category
-            ):
-                os.makedirs(
-                    SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
-                    / image_category
-                )
+            if not os.path.exists(main_address / image_category):
+                os.makedirs(main_address / image_category)
             # check if the dir is empty if not delete all the files
             else:
                 # empty the previous augmented images
-                for file in (
-                    SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
-                    / image_category
-                ).iterdir():
+                for file in (main_address / image_category).iterdir():
                     os.remove(file)
 
             number_of_images = self.image_dict[image_category]["number_of_images"]
             for _ in tqdm(
-                range(0, number_of_images_tobe_gen + 1),
+                range(0, number_of_images_tobe_gen),
                 desc=f"Augmenting {image_category} images:",
             ):
                 # generate a random number integer between 0 and number_of_images
                 rand_img_num = int(random.random() * number_of_images)
 
                 img_address = self.image_dict[image_category]["image_list"][
                     rand_img_num
@@ -191,73 +212,75 @@
 
                 x = img_to_array(img)
                 x = x.reshape((1,) + x.shape)
 
                 for _ in Augment_data_gen.flow(
                     x,
                     batch_size=SETTING.AUGMENTATION_SETTING.BATCH_SIZE,
-                    save_to_dir=SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
+                    save_to_dir=main_address / image_category
+                    or SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
                     / image_category,
                     save_prefix=SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_SAVE_PREFIX,
                     save_format=SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_SAVE_FORMAT,
                 ):
                     break
 
     def train_test_split(self, *args, **kwargs):
         """
         This function is used to split the data into train, test and validation.
         And save them into the dataset_train_test_split folder.
+        :param args:
+        :param kwargs: augmented_data_address, train_test_val_split_dir_address
         :return:
         """
-        # get the list of dirs in the AUGMENTED_IMAGES_DIR_ADDRESS
-        augmented_images_dir_list = os.listdir(
-            SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
+        augmented_data_address = (
+            kwargs.get("augmented_data_address")
+            or SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
         )
+        train_test_val_split_dir_address = (
+            kwargs.get("train_test_val_split_dir_address")
+            or SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
+        )
+        # get the list of dirs in the AUGMENTED_IMAGES_DIR_ADDRESS
+        augmented_images_dir_list = os.listdir(augmented_data_address)
         logger.info(f"Augmented images dir list: {augmented_images_dir_list}")
 
         # make a new dir for train and test and validation data
-        if not os.path.exists(
-            SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
-        ):
-            os.makedirs(SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS)
+        if not os.path.exists(train_test_val_split_dir_address):
+            os.makedirs(train_test_val_split_dir_address)
         # make 3 dirs for train, test and validation under AUGMENTATION_SETTING.TRAIN_TEST_SPLIT_DIR_ADDRESS
         for dir_name in SETTING.PREPROCESSING_SETTING.TRAIN_TEST_SPLIT_DIR_NAMES:
-            if not os.path.exists(
-                SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
-                / dir_name
-            ):
-                os.makedirs(
-                    SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
-                    / dir_name
-                )
+            if not os.path.exists(train_test_val_split_dir_address / dir_name):
+                os.makedirs(train_test_val_split_dir_address / dir_name)
         logger.info(f"Created train, test and validation dirs")
 
         # under each train, test and validation dir make a dir for each category
         for dir_name in SETTING.PREPROCESSING_SETTING.TRAIN_TEST_SPLIT_DIR_NAMES:
             for category in augmented_images_dir_list:
                 if not os.path.exists(
-                    SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
-                    / dir_name
-                    / category
+                    train_test_val_split_dir_address / dir_name / category
                 ):
-                    os.makedirs(
-                        SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
-                        / dir_name
-                        / category
-                    )
+                    os.makedirs(train_test_val_split_dir_address / dir_name / category)
         logger.info(f"Created category dirs under train, test and validation dirs")
 
-        self.populated_augmented_images_into_train_test_val_dirs()
+        self._populated_augmented_images_into_train_test_val_dirs(
+            augmented_data_address, train_test_val_split_dir_address
+        )
+
+    def _populated_augmented_images_into_train_test_val_dirs(self, *arges, **kwargs):
+        dataset_augmented_dir_address = arges[0]
+        train_test_val_split_dir_address = arges[1]
+        # dataset_augmented_dir_address = (
+        #         kwargs.get("dataset_augmented")
+        #         or SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
+        # )
 
-    def populated_augmented_images_into_train_test_val_dirs(self):
         for category in self.categories_name_folders:
             # get the list of images in the dataset_augmented category (i.e. pdc_bit) folder
-            original_list = os.listdir(
-                SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS / category
-            )
+            original_list = os.listdir(dataset_augmented_dir_address / category)
 
             # Number of items to select for each new list
             num_train = int(
                 len(original_list) * SETTING.PREPROCESSING_SETTING.TRAIN_FRACTION
             )
             num_test = int(
                 len(original_list) * SETTING.PREPROCESSING_SETTING.TEST_FRACTION
@@ -268,62 +291,79 @@
             selected_items = random.sample(original_list, len(original_list))
 
             # Create three new lists containing 70%, 20%, and 10% of the original list
             train_list = selected_items[:num_train]
             test_list = selected_items[num_train : num_train + num_test]
             val_list = selected_items[num_train + num_test :]
             # copy the images from the dataset_augmented pdc_bit folder to the train, test and validation folders
-            self.copy_images(train_list, category, "train")
-            self.copy_images(test_list, category, "test")
-            self.copy_images(val_list, category, "val")
+            self._copy_images(
+                train_list,
+                category,
+                "train",
+                dataset_augmented_dir_address,
+                train_test_val_split_dir_address,
+            )
+            self._copy_images(
+                test_list,
+                category,
+                "test",
+                dataset_augmented_dir_address,
+                train_test_val_split_dir_address,
+            )
+            self._copy_images(
+                val_list,
+                category,
+                "val",
+                dataset_augmented_dir_address,
+                train_test_val_split_dir_address,
+            )
 
     @staticmethod
-    def copy_images(images, categ, dest_folder):
+    def _copy_images(
+        images,
+        categ,
+        dest_folder,
+        dataset_augmented_dir_address,
+        train_test_val_split_dir_address,
+    ):
+        train_test_val_split_dir_address = (
+            train_test_val_split_dir_address
+            or SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
+        )
+        dataset_augmented_dir_address = (
+            dataset_augmented_dir_address
+            or SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
+        )
+
         # check if the dir is empty, if not delete all the files
-        if os.listdir(
-            SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
-            / dest_folder
-            / categ
-        ):
+        if os.listdir(train_test_val_split_dir_address / dest_folder / categ):
             logger.info(
-                f"Deleting all the files in {SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS / dest_folder / categ}"
+                f"Deleting all the files in {train_test_val_split_dir_address / dest_folder / categ}"
             )
             for file in os.listdir(
-                SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
-                / dest_folder
-                / categ
+                train_test_val_split_dir_address / dest_folder / categ
             ):
-                os.remove(
-                    SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
-                    / dest_folder
-                    / categ
-                    / file
-                )
+                os.remove(train_test_val_split_dir_address / dest_folder / categ / file)
 
         for image in images:
             shutil.copy(
-                SETTING.AUGMENTATION_SETTING.AUGMENTED_IMAGES_DIR_ADDRESS
-                / categ
-                / image,
-                SETTING.PREPROCESSING_SETTING.TRAIN_TEST_VAL_SPLIT_DIR_ADDRESS
-                / dest_folder
-                / categ
-                / image,
+                dataset_augmented_dir_address / categ / image,
+                train_test_val_split_dir_address / dest_folder / categ / image,
             )
         logger.info(
             f"copied {len(images)} images for category {categ} to {dest_folder}"
         )
 
 
 if __name__ == "__main__":
-    # Preprocessing.download_images()
-    # obj = Preprocessing(dataset_address=Path(__file__).parent / ".." / "dataset")
+    obj = Preprocessing(dataset_address=Path(__file__).parent / ".." / "dataset")
+    obj.download_images()
 
     # or download the data from s3. this is after you have downloaded the data
     # using Process.download_images() and uploaded it to s3
-    # this way the data would be consistent for all the team members
-    Preprocessing.download_images(from_s3=True)
-    obj = Preprocessing(dataset_address=Path(__file__).parent / ".." / "s3_dataset")
+    # this way the data would be consistent across all the users
+    # obj = Preprocessing(dataset_address=Path(__file__).parent / ".." / "s3_dataset")
+    # obj.download_images(from_s3=True)
 
     print(obj.image_dict)
-    obj.augment_data(number_of_images_tobe_gen=200)
+    obj.augment_data(number_of_images_tobe_gen=10)
     obj.train_test_split()
```

### Comparing `drillvision-0.0.1/neural_network_model/s3.py` & `drillvision-0.0.2/neural_network_model/s3.py`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.1/pyproject.toml` & `drillvision-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `drillvision-0.0.1/setup.py` & `drillvision-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
 # Package meta-data.
-NAME = 'drillvision'
+NAME = "drillvision"
 DESCRIPTION = long_description
 URL = "https://github.com/Atashnezhad/DrillBitVision"
 EMAIL = "atashnezhad2@gmail.com"
 AUTHOR = "Amin Atashnezhad"
 REQUIRES_PYTHON = ">=3.6.0"
 
 
@@ -23,25 +23,26 @@
 # If you do change the License, remember to change the
 # Trove Classifier for that!
 
 # Load the package's VERSION file as a dictionary.
 about = {}
 ROOT_DIR = Path(__file__).resolve().parent
 REQUIREMENTS_DIR = ROOT_DIR
-PACKAGE_DIR = ROOT_DIR / 'neural_network_model'
+PACKAGE_DIR = ROOT_DIR / "neural_network_model"
 with open(PACKAGE_DIR / "VERSION") as f:
     _version = f.read().strip()
     about["__version__"] = _version
 
 
 # What packages are required for this module to be executed?
 def list_reqs(fname="requirements.txt"):
     with open(REQUIREMENTS_DIR / fname) as fd:
         return fd.read().splitlines()
 
+
 # Where the magic happens:
 setup(
     name=NAME,
     version=about["__version__"],
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type="text/markdown",
@@ -56,19 +57,16 @@
     include_package_data=True,
     license="BSD-3",
     classifiers=[
         # Trove classifiers
         # Full list: https://pypi.python.org/pypi?%3Aaction=list_classifiers
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
 )
 
 if __name__ == "__main__":
-    list_reqs()
+    list_reqs()
```

### Comparing `drillvision-0.0.1/tests/test_preprocessing.py` & `drillvision-0.0.2/tests/test_preprocessing.py`

 * *Files identical despite different names*


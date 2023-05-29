# Comparing `tmp/light_size_constrained_clustering-0.0.5.tar.gz` & `tmp/light_size_constrained_clustering-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "light_size_constrained_clustering-0.0.5.tar", last modified: Thu May 25 17:15:54 2023, max compression
+gzip compressed data, was "light_size_constrained_clustering-0.0.6.tar", last modified: Mon May 29 08:48:16 2023, max compression
```

## Comparing `light_size_constrained_clustering-0.0.5.tar` & `light_size_constrained_clustering-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-25 17:15:54.087889 light_size_constrained_clustering-0.0.5/
--rw-r--r--   0 i0365030   (502) staff       (20)     1074 2023-05-24 18:28:58.000000 light_size_constrained_clustering-0.0.5/LICENSE
--rw-r--r--   0 i0365030   (502) staff       (20)     3646 2023-05-25 17:15:54.087733 light_size_constrained_clustering-0.0.5/PKG-INFO
--rw-r--r--   0 i0365030   (502) staff       (20)     3299 2023-05-25 17:12:16.000000 light_size_constrained_clustering-0.0.5/README.md
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-25 17:15:54.086218 light_size_constrained_clustering-0.0.5/light_size_constrained_clustering/
--rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.5/light_size_constrained_clustering/__init__.py
--rw-r--r--   0 i0365030   (502) staff       (20)     6178 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.5/light_size_constrained_clustering/base.py
--rw-r--r--   0 i0365030   (502) staff       (20)     8612 2023-05-25 17:10:31.000000 light_size_constrained_clustering-0.0.5/light_size_constrained_clustering/da.py
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-25 17:15:54.087227 light_size_constrained_clustering-0.0.5/light_size_constrained_clustering.egg-info/
--rw-r--r--   0 i0365030   (502) staff       (20)     3646 2023-05-25 17:15:54.000000 light_size_constrained_clustering-0.0.5/light_size_constrained_clustering.egg-info/PKG-INFO
--rw-r--r--   0 i0365030   (502) staff       (20)      455 2023-05-25 17:15:54.000000 light_size_constrained_clustering-0.0.5/light_size_constrained_clustering.egg-info/SOURCES.txt
--rw-r--r--   0 i0365030   (502) staff       (20)        1 2023-05-25 17:15:54.000000 light_size_constrained_clustering-0.0.5/light_size_constrained_clustering.egg-info/dependency_links.txt
--rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-25 17:15:54.000000 light_size_constrained_clustering-0.0.5/light_size_constrained_clustering.egg-info/requires.txt
--rw-r--r--   0 i0365030   (502) staff       (20)       34 2023-05-25 17:15:54.000000 light_size_constrained_clustering-0.0.5/light_size_constrained_clustering.egg-info/top_level.txt
--rw-r--r--   0 i0365030   (502) staff       (20)       38 2023-05-25 17:15:54.087928 light_size_constrained_clustering-0.0.5/setup.cfg
--rw-r--r--   0 i0365030   (502) staff       (20)     1140 2023-05-25 17:12:27.000000 light_size_constrained_clustering-0.0.5/setup.py
-drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-25 17:15:54.087452 light_size_constrained_clustering-0.0.5/tests/
--rw-r--r--   0 i0365030   (502) staff       (20)     1341 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.5/tests/test_da.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-29 08:48:16.492337 light_size_constrained_clustering-0.0.6/
+-rw-r--r--   0 i0365030   (502) staff       (20)     1074 2023-05-24 18:28:58.000000 light_size_constrained_clustering-0.0.6/LICENSE
+-rw-r--r--   0 i0365030   (502) staff       (20)     3646 2023-05-29 08:48:16.492120 light_size_constrained_clustering-0.0.6/PKG-INFO
+-rw-r--r--   0 i0365030   (502) staff       (20)     3299 2023-05-25 17:12:16.000000 light_size_constrained_clustering-0.0.6/README.md
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-29 08:48:16.490894 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/
+-rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/__init__.py
+-rw-r--r--   0 i0365030   (502) staff       (20)     6178 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/base.py
+-rw-r--r--   0 i0365030   (502) staff       (20)     9292 2023-05-29 08:46:59.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/da.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-29 08:48:16.491761 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/
+-rw-r--r--   0 i0365030   (502) staff       (20)     3646 2023-05-29 08:48:16.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/PKG-INFO
+-rw-r--r--   0 i0365030   (502) staff       (20)      455 2023-05-29 08:48:16.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/SOURCES.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)        1 2023-05-29 08:48:16.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/dependency_links.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)      106 2023-05-29 08:48:16.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/requires.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)       34 2023-05-29 08:48:16.000000 light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/top_level.txt
+-rw-r--r--   0 i0365030   (502) staff       (20)       38 2023-05-29 08:48:16.492406 light_size_constrained_clustering-0.0.6/setup.cfg
+-rw-r--r--   0 i0365030   (502) staff       (20)     1140 2023-05-29 08:47:37.000000 light_size_constrained_clustering-0.0.6/setup.py
+drwxr-xr-x   0 i0365030   (502) staff       (20)        0 2023-05-29 08:48:16.491891 light_size_constrained_clustering-0.0.6/tests/
+-rw-r--r--   0 i0365030   (502) staff       (20)     1341 2023-05-25 16:50:29.000000 light_size_constrained_clustering-0.0.6/tests/test_da.py
```

### Comparing `light_size_constrained_clustering-0.0.5/LICENSE` & `light_size_constrained_clustering-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.5/PKG-INFO` & `light_size_constrained_clustering-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light_size_constrained_clustering
-Version: 0.0.5
+Version: 0.0.6
 Summary: Size Constrained Clustering solver
 Home-page: https://github.com/AlbertPlaPlanas/size_constrained_clustering
 Author: Albert Pla
 Author-email: plaalbert@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `light_size_constrained_clustering-0.0.5/README.md` & `light_size_constrained_clustering-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.5/light_size_constrained_clustering/base.py` & `light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/base.py`

 * *Files identical despite different names*

### Comparing `light_size_constrained_clustering-0.0.5/light_size_constrained_clustering/da.py` & `light_size_constrained_clustering-0.0.6/light_size_constrained_clustering/da.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 @Paper reference: Clustering with Capacity and Size Constraints: A Deterministic Approach
 '''
 
 import numpy as np
 import collections
 import random
 from scipy.spatial.distance import cdist
+import logging
 
 import os 
 import sys 
 path = os.path.dirname(os.path.abspath(__file__))
 sys.path.append(path)
 import base 
 
@@ -189,27 +190,40 @@
         '''
 
         n_samples = len(X)
         centers = self.cluster_centers_
         labels = self.labels_
         distribution = self.lamb
 
-        # Obtain the expected number of labels in each cluster
-        expected_allocation = np.array(distribution) * n_samples
+        # Obtain the expected number of labels in each cluster as integer
+        expected_allocation = (np.array(distribution) * n_samples).round().astype(int)
         resulting_allocation = np.bincount(labels, minlength=len(expected_allocation))
         
         while not np.array_equal(expected_allocation, resulting_allocation):
+            logging.debug("Expected allocation: %s", expected_allocation)
+            logging.debug("Resulting allocation: %s", resulting_allocation)
+            logging.debug("Total allocation: %s, Expected allocation: %s", np.sum(resulting_allocation), np.sum(expected_allocation))
+
+
             too_big_clusts, = np.where(resulting_allocation > expected_allocation)
             too_small_clusts, = np.where(resulting_allocation < expected_allocation)
+        
+            logging.debug('Too big clusters: %s', too_big_clusts)
+            logging.debug('Too small clusters: %s', too_small_clusts)
+
+            logging.debug("Addressing cluster %s", too_big_clusts[0])
 
             big_indexes = labels == too_big_clusts[0]
             distances_to_center = np.linalg.norm(X - centers[too_big_clusts[0]], axis=1)
             distances_to_center[~big_indexes] = 0
             max_dist_index = np.argmax(distances_to_center)
 
             closest_small_cluster = too_small_clusts[np.argmin(np.linalg.norm(X[max_dist_index] - centers[too_small_clusts], axis=1))]
             labels[max_dist_index] = closest_small_cluster
 
+            logging.debug(f"Moved point {max_dist_index} from cluster {too_big_clusts[0]} to cluster {closest_small_cluster}.")
+
+
             resulting_allocation = np.bincount(labels, minlength=len(expected_allocation))
 
         self.labels_ = labels
         return labels, resulting_allocation
```

### Comparing `light_size_constrained_clustering-0.0.5/light_size_constrained_clustering.egg-info/PKG-INFO` & `light_size_constrained_clustering-0.0.6/light_size_constrained_clustering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: light-size-constrained-clustering
-Version: 0.0.5
+Version: 0.0.6
 Summary: Size Constrained Clustering solver
 Home-page: https://github.com/AlbertPlaPlanas/size_constrained_clustering
 Author: Albert Pla
 Author-email: plaalbert@gmail.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `light_size_constrained_clustering-0.0.5/setup.py` & `light_size_constrained_clustering-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 path = os.path.dirname(os.path.abspath(__file__))
 
 with open(os.path.join(path, "requirements.txt")) as fp:
     install_requires = fp.read().strip().split("\n")
 
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 LICENSE = "MIT"
 setup(
     #ext_modules=extensions,
     version=VERSION,
     setup_requires=["numpy"],
     install_requires=install_requires,
     name="light_size_constrained_clustering",
```

### Comparing `light_size_constrained_clustering-0.0.5/tests/test_da.py` & `light_size_constrained_clustering-0.0.6/tests/test_da.py`

 * *Files identical despite different names*


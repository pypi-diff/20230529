# Comparing `tmp/weavenn-1.0.0.tar.gz` & `tmp/weavenn-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weavenn-1.0.0.tar", last modified: Mon May 29 12:55:50 2023, max compression
+gzip compressed data, was "weavenn-1.0.1.tar", last modified: Mon May 29 15:29:10 2023, max compression
```

## Comparing `weavenn-1.0.0.tar` & `weavenn-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 12:55:50.648534 weavenn-1.0.0/
--rw-r--r--   0 maixent   (1000) maixent   (1000)       31 2022-03-04 17:26:53.000000 weavenn-1.0.0/MANIFEST.in
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      149 2023-05-29 12:55:50.648534 weavenn-1.0.0/PKG-INFO
--rw-r--r--   0 maixent   (1000) maixent   (1000)      260 2022-02-21 10:01:01.000000 weavenn-1.0.0/README.md
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       38 2023-05-29 12:55:50.648534 weavenn-1.0.0/setup.cfg
--rw-r--r--   0 maixent   (1000) maixent   (1000)      703 2023-05-29 12:54:31.000000 weavenn-1.0.0/setup.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 12:55:50.648534 weavenn-1.0.0/src/
--rw-r--r--   0 maixent   (1000) maixent   (1000)     5193 2022-08-03 08:50:43.000000 weavenn-1.0.0/src/algorithm.cpp
--rw-r--r--   0 maixent   (1000) maixent   (1000)      894 2022-06-28 12:20:50.000000 weavenn-1.0.0/src/algorithm.hpp
--rw-r--r--   0 maixent   (1000) maixent   (1000)      303 2023-05-29 12:42:25.000000 weavenn-1.0.0/src/bindings.cpp
--rw-r--r--   0 maixent   (1000) maixent   (1000)    16478 2023-05-29 12:42:37.000000 weavenn-1.0.0/src/louvain.cpp
--rw-r--r--   0 maixent   (1000) maixent   (1000)     2205 2022-04-22 10:21:26.000000 weavenn-1.0.0/src/louvain.hpp
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 12:55:50.648534 weavenn-1.0.0/weavenn/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       52 2023-05-29 12:50:06.000000 weavenn-1.0.0/weavenn/__init__.py
--rw-rw-r--   0 maixent   (1000) maixent   (1000)     1476 2023-05-29 12:41:20.000000 weavenn-1.0.0/weavenn/louvain.py
--rw-r--r--   0 maixent   (1000) maixent   (1000)    10406 2023-05-29 12:53:15.000000 weavenn-1.0.0/weavenn/weavenn.py
-drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 12:55:50.648534 weavenn-1.0.0/weavenn.egg-info/
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      149 2023-05-29 12:55:50.000000 weavenn-1.0.0/weavenn.egg-info/PKG-INFO
--rw-rw-r--   0 maixent   (1000) maixent   (1000)      327 2023-05-29 12:55:50.000000 weavenn-1.0.0/weavenn.egg-info/SOURCES.txt
--rw-rw-r--   0 maixent   (1000) maixent   (1000)        1 2023-05-29 12:55:50.000000 weavenn-1.0.0/weavenn.egg-info/dependency_links.txt
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       42 2023-05-29 12:55:50.000000 weavenn-1.0.0/weavenn.egg-info/requires.txt
--rw-rw-r--   0 maixent   (1000) maixent   (1000)       17 2023-05-29 12:55:50.000000 weavenn-1.0.0/weavenn.egg-info/top_level.txt
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 15:29:10.605526 weavenn-1.0.1/
+-rw-r--r--   0 maixent   (1000) maixent   (1000)       31 2022-03-04 17:26:53.000000 weavenn-1.0.1/MANIFEST.in
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      149 2023-05-29 15:29:10.605526 weavenn-1.0.1/PKG-INFO
+-rw-r--r--   0 maixent   (1000) maixent   (1000)      260 2022-02-21 10:01:01.000000 weavenn-1.0.1/README.md
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       38 2023-05-29 15:29:10.605526 weavenn-1.0.1/setup.cfg
+-rw-r--r--   0 maixent   (1000) maixent   (1000)      703 2023-05-29 15:28:53.000000 weavenn-1.0.1/setup.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 15:29:10.601526 weavenn-1.0.1/src/
+-rw-r--r--   0 maixent   (1000) maixent   (1000)     5193 2022-08-03 08:50:43.000000 weavenn-1.0.1/src/algorithm.cpp
+-rw-r--r--   0 maixent   (1000) maixent   (1000)      894 2022-06-28 12:20:50.000000 weavenn-1.0.1/src/algorithm.hpp
+-rw-r--r--   0 maixent   (1000) maixent   (1000)      303 2023-05-29 12:42:25.000000 weavenn-1.0.1/src/bindings.cpp
+-rw-r--r--   0 maixent   (1000) maixent   (1000)    16478 2023-05-29 12:42:37.000000 weavenn-1.0.1/src/louvain.cpp
+-rw-r--r--   0 maixent   (1000) maixent   (1000)     2205 2022-04-22 10:21:26.000000 weavenn-1.0.1/src/louvain.hpp
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 15:29:10.601526 weavenn-1.0.1/weavenn/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       52 2023-05-29 12:50:06.000000 weavenn-1.0.1/weavenn/__init__.py
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)     1476 2023-05-29 12:41:20.000000 weavenn-1.0.1/weavenn/louvain.py
+-rw-r--r--   0 maixent   (1000) maixent   (1000)    11538 2023-05-29 15:27:24.000000 weavenn-1.0.1/weavenn/weavenn.py
+drwxrwxr-x   0 maixent   (1000) maixent   (1000)        0 2023-05-29 15:29:10.605526 weavenn-1.0.1/weavenn.egg-info/
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      149 2023-05-29 15:29:10.000000 weavenn-1.0.1/weavenn.egg-info/PKG-INFO
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)      327 2023-05-29 15:29:10.000000 weavenn-1.0.1/weavenn.egg-info/SOURCES.txt
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)        1 2023-05-29 15:29:10.000000 weavenn-1.0.1/weavenn.egg-info/dependency_links.txt
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       42 2023-05-29 15:29:10.000000 weavenn-1.0.1/weavenn.egg-info/requires.txt
+-rw-rw-r--   0 maixent   (1000) maixent   (1000)       17 2023-05-29 15:29:10.000000 weavenn-1.0.1/weavenn.egg-info/top_level.txt
```

### Comparing `weavenn-1.0.0/setup.py` & `weavenn-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             pybind11.get_include(),
             pybind11.get_include(True), ],
         extra_compile_args=["-Ofast", "-std=c++17"])
 ]
 
 setup(
     name="weavenn",
-    version="1.0.0",
+    version="1.0.1",
     packages=find_packages(),
     include_package_data=True,
     install_requires=["networkx", "numpy", "scikit-learn", "numba", "hnswlib"],
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `weavenn-1.0.0/src/algorithm.cpp` & `weavenn-1.0.1/src/algorithm.cpp`

 * *Files identical despite different names*

### Comparing `weavenn-1.0.0/src/algorithm.hpp` & `weavenn-1.0.1/src/algorithm.hpp`

 * *Files identical despite different names*

### Comparing `weavenn-1.0.0/src/louvain.cpp` & `weavenn-1.0.1/src/louvain.cpp`

 * *Files identical despite different names*

### Comparing `weavenn-1.0.0/src/louvain.hpp` & `weavenn-1.0.1/src/louvain.hpp`

 * *Files identical despite different names*

### Comparing `weavenn-1.0.0/weavenn/louvain.py` & `weavenn-1.0.1/weavenn/louvain.py`

 * *Files identical despite different names*

### Comparing `weavenn-1.0.0/weavenn/weavenn.py` & `weavenn-1.0.1/weavenn/weavenn.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
         score="silhouette",
         sample_size=3000,
         use_modularity=False,
         use_global_scale=False,
         threshold=.1,
         scale_free_factor=2,
         scale_free_gamma=2.5,
+        ann_method="annoy",
         verbose=False
     ):
         self.k = k
         self.kernel = kernel
         self.metric = metric
         self.reduction_dim = reduction_dim
         self.min_cluster_size = min_cluster_size
@@ -39,28 +40,53 @@
         self.sample_size = sample_size
         self.use_modularity = use_modularity
         self.threshold = threshold
         self.use_global_scale = use_global_scale
         # scale free parameters of the graph
         self.scale_free_factor = scale_free_factor
         self.scale_free_gamma = scale_free_gamma
+        self.ann_method = ann_method
         self.verbose = verbose
 
     def get_knns(self, X):
-        import hnswlib
-
         n, dim = X.shape
 
-        index = hnswlib.Index(space=self.metric, dim=dim)
-        index.init_index(
-            max_elements=n, ef_construction=3 * self.k,
-            M=250, random_seed=100)
-        index.add_items(X, range(n))
-
-        labels, distances = index.knn_query(X, k=self.k)
+        if self.ann_method == "hnsw":
+            import hnswlib
+            index = hnswlib.Index(space=self.metric, dim=dim)
+            index.init_index(
+                max_elements=n, ef_construction=3 * self.k,
+                M=250, random_seed=100)
+            index.add_items(X, range(n))
+            labels, distances = index.knn_query(X, k=self.k)
+        elif self.ann_method == "pynndescent":
+            from pynndescent import NNDescent
+            index = NNDescent(
+                X, metric=self.metric, n_neighbors=self.k,
+                n_jobs=-1, random_state=100)
+            distances, labels = index.query(X, k=self.k)
+        elif self.ann_method == "annoy":
+            from annoy import AnnoyIndex
+            metric = "angular" if self.metric == "cosine" else self.metric
+            metric = "euclidean" if metric == "l2" else metric
+
+            index = AnnoyIndex(dim, metric)
+            for i, x in enumerate(X):
+                index.add_item(i, x)
+            index.build(100)
+            labels = []
+            distances = []
+            for x in X:
+                l, d = index.get_nns_by_vector(
+                    x, self.k,
+                    include_distances=True)
+                labels.append(l)
+                distances.append(d)
+            labels = np.array(labels)
+            distances = np.array(distances)
         return labels, distances
 
     def get_reduced_distances(self):
         labels, distances = self._labels, self._distances
         distances = (distances / self._sigma[:, None]) ** self._beta
         return labels, distances
```


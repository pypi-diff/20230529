# Comparing `tmp/bipartitepandas-1.1.6.tar.gz` & `tmp/bipartitepandas-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bipartitepandas-1.1.6.tar", last modified: Sun May 28 03:42:06 2023, max compression
+gzip compressed data, was "bipartitepandas-1.1.7.tar", last modified: Mon May 29 00:50:13 2023, max compression
```

## Comparing `bipartitepandas-1.1.6.tar` & `bipartitepandas-1.1.7.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.743100 bipartitepandas-1.1.6/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1058 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/LICENSE
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2797 2023-05-28 03:42:06.743205 bipartitepandas-1.1.6/PKG-INFO
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2204 2023-05-28 03:41:14.000000 bipartitepandas-1.1.6/README.rst
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.738546 bipartitepandas-1.1.6/bipartitepandas/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      818 2022-09-02 23:11:52.000000 bipartitepandas-1.1.6/bipartitepandas/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86380 2023-05-28 02:35:42.000000 bipartitepandas-1.1.6/bipartitepandas/bipartitebase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    32553 2022-09-03 22:00:33.000000 bipartitepandas-1.1.6/bipartitepandas/bipartitedataframe.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3582 2023-05-26 18:35:42.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudy.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    58472 2023-05-26 18:17:43.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudybase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3500 2023-01-08 21:22:33.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudycollapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3818 2022-09-02 23:16:52.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudy.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    50571 2023-01-08 21:22:25.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudybase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3758 2023-01-08 21:22:35.000000 bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudycollapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    27925 2023-05-26 18:38:14.000000 bipartitepandas-1.1.6/bipartitepandas/bipartitelong.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    75272 2023-05-26 18:15:28.000000 bipartitepandas-1.1.6/bipartitepandas/bipartitelongbase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34407 2023-01-08 21:22:37.000000 bipartitepandas-1.1.6/bipartitepandas/bipartitelongcollapsed.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.739566 bipartitepandas-1.1.6/bipartitepandas/grouping/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/bipartitepandas/grouping/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3162 2023-05-28 02:59:45.000000 bipartitepandas-1.1.6/bipartitepandas/grouping/grouping.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.740127 bipartitepandas-1.1.6/bipartitepandas/measures/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/bipartitepandas/measures/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     6778 2023-05-28 03:40:11.000000 bipartitepandas-1.1.6/bipartitepandas/measures/measures.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8604 2022-09-02 23:16:50.000000 bipartitepandas-1.1.6/bipartitepandas/simbipartite.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    13173 2022-09-02 23:16:51.000000 bipartitepandas-1.1.6/bipartitepandas/util.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.739273 bipartitepandas-1.1.6/bipartitepandas.egg-info/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2797 2023-05-28 03:42:06.000000 bipartitepandas-1.1.6/bipartitepandas.egg-info/PKG-INFO
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1201 2023-05-28 03:42:06.000000 bipartitepandas-1.1.6/bipartitepandas.egg-info/SOURCES.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)        1 2023-05-28 03:42:06.000000 bipartitepandas-1.1.6/bipartitepandas.egg-info/dependency_links.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       82 2023-05-28 03:42:06.000000 bipartitepandas-1.1.6/bipartitepandas.egg-info/requires.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       16 2023-05-28 03:42:06.000000 bipartitepandas-1.1.6/bipartitepandas.egg-info/top_level.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      103 2022-08-28 19:50:50.000000 bipartitepandas-1.1.6/pyproject.toml
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      763 2023-05-28 03:42:06.743629 bipartitepandas-1.1.6/setup.cfg
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      162 2023-01-08 21:43:24.000000 bipartitepandas-1.1.6/setup.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-28 03:42:06.742961 bipartitepandas-1.1.6/tests/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2900 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/tests/test_bpd.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86879 2022-09-02 23:16:33.000000 bipartitepandas-1.1.6/tests/test_bpd_base.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    17148 2023-05-28 03:00:38.000000 bipartitepandas-1.1.6/tests/test_bpd_clustering.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34290 2023-05-26 18:42:55.000000 bipartitepandas-1.1.6/tests/test_bpd_connectedness.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    16145 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/tests/test_bpd_custom.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2253 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/tests/test_bpd_df.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4536 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/tests/test_bpd_es.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4978 2022-07-24 19:52:06.000000 bipartitepandas-1.1.6/tests/test_bpd_es_collapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    14606 2022-09-02 23:16:46.000000 bipartitepandas-1.1.6/tests/test_bpd_long.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2954 2022-08-06 18:51:15.000000 bipartitepandas-1.1.6/tests/test_bpd_long_collapsed.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 00:50:13.073621 bipartitepandas-1.1.7/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1058 2022-07-24 19:52:06.000000 bipartitepandas-1.1.7/LICENSE
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2797 2023-05-29 00:50:13.073715 bipartitepandas-1.1.7/PKG-INFO
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2204 2023-05-28 03:41:14.000000 bipartitepandas-1.1.7/README.rst
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 00:50:13.068622 bipartitepandas-1.1.7/bipartitepandas/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      818 2022-09-02 23:11:52.000000 bipartitepandas-1.1.7/bipartitepandas/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86380 2023-05-28 02:35:42.000000 bipartitepandas-1.1.7/bipartitepandas/bipartitebase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    32553 2022-09-03 22:00:33.000000 bipartitepandas-1.1.7/bipartitepandas/bipartitedataframe.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3582 2023-05-26 18:35:42.000000 bipartitepandas-1.1.7/bipartitepandas/bipartiteeventstudy.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    58472 2023-05-26 18:17:43.000000 bipartitepandas-1.1.7/bipartitepandas/bipartiteeventstudybase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3500 2023-01-08 21:22:33.000000 bipartitepandas-1.1.7/bipartitepandas/bipartiteeventstudycollapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3818 2022-09-02 23:16:52.000000 bipartitepandas-1.1.7/bipartitepandas/bipartiteextendedeventstudy.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    50571 2023-01-08 21:22:25.000000 bipartitepandas-1.1.7/bipartitepandas/bipartiteextendedeventstudybase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3758 2023-01-08 21:22:35.000000 bipartitepandas-1.1.7/bipartitepandas/bipartiteextendedeventstudycollapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    27925 2023-05-26 18:38:14.000000 bipartitepandas-1.1.7/bipartitepandas/bipartitelong.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    75272 2023-05-26 18:15:28.000000 bipartitepandas-1.1.7/bipartitepandas/bipartitelongbase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34407 2023-01-08 21:22:37.000000 bipartitepandas-1.1.7/bipartitepandas/bipartitelongcollapsed.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 00:50:13.070268 bipartitepandas-1.1.7/bipartitepandas/grouping/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.7/bipartitepandas/grouping/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3043 2023-05-29 00:48:11.000000 bipartitepandas-1.1.7/bipartitepandas/grouping/grouping.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 00:50:13.070705 bipartitepandas-1.1.7/bipartitepandas/measures/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.7/bipartitepandas/measures/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     6778 2023-05-28 03:40:11.000000 bipartitepandas-1.1.7/bipartitepandas/measures/measures.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8604 2022-09-02 23:16:50.000000 bipartitepandas-1.1.7/bipartitepandas/simbipartite.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    13173 2022-09-02 23:16:51.000000 bipartitepandas-1.1.7/bipartitepandas/util.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 00:50:13.069799 bipartitepandas-1.1.7/bipartitepandas.egg-info/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2797 2023-05-29 00:50:13.000000 bipartitepandas-1.1.7/bipartitepandas.egg-info/PKG-INFO
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1201 2023-05-29 00:50:13.000000 bipartitepandas-1.1.7/bipartitepandas.egg-info/SOURCES.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)        1 2023-05-29 00:50:13.000000 bipartitepandas-1.1.7/bipartitepandas.egg-info/dependency_links.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       82 2023-05-29 00:50:13.000000 bipartitepandas-1.1.7/bipartitepandas.egg-info/requires.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       16 2023-05-29 00:50:13.000000 bipartitepandas-1.1.7/bipartitepandas.egg-info/top_level.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      103 2022-08-28 19:50:50.000000 bipartitepandas-1.1.7/pyproject.toml
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      763 2023-05-29 00:50:13.074113 bipartitepandas-1.1.7/setup.cfg
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      162 2023-01-08 21:43:24.000000 bipartitepandas-1.1.7/setup.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-29 00:50:13.073477 bipartitepandas-1.1.7/tests/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2900 2022-07-24 19:52:06.000000 bipartitepandas-1.1.7/tests/test_bpd.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86879 2022-09-02 23:16:33.000000 bipartitepandas-1.1.7/tests/test_bpd_base.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    17134 2023-05-29 00:41:26.000000 bipartitepandas-1.1.7/tests/test_bpd_clustering.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34290 2023-05-26 18:42:55.000000 bipartitepandas-1.1.7/tests/test_bpd_connectedness.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    16145 2022-07-24 19:52:06.000000 bipartitepandas-1.1.7/tests/test_bpd_custom.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2253 2022-07-24 19:52:06.000000 bipartitepandas-1.1.7/tests/test_bpd_df.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4536 2022-07-24 19:52:06.000000 bipartitepandas-1.1.7/tests/test_bpd_es.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4978 2022-07-24 19:52:06.000000 bipartitepandas-1.1.7/tests/test_bpd_es_collapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    14606 2022-09-02 23:16:46.000000 bipartitepandas-1.1.7/tests/test_bpd_long.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2954 2022-08-06 18:51:15.000000 bipartitepandas-1.1.7/tests/test_bpd_long_collapsed.py
```

### Comparing `bipartitepandas-1.1.6/LICENSE` & `bipartitepandas-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/PKG-INFO` & `bipartitepandas-1.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipartitepandas
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python tools for bipartite labor data
 Home-page: https://github.com/tlamadon/bipartitepandas/
 Author: Thibaut Lamadon
 Author-email: thibaut.lamadon@gmail.com
 Project-URL: Documentation, https://tlamadon.github.io/bipartitepandas/
 Project-URL: GitHub, https://github.com/tlamadon/bipartitepandas/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bipartitepandas-1.1.6/README.rst` & `bipartitepandas-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/__init__.py` & `bipartitepandas-1.1.7/bipartitepandas/__init__.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartitebase.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartitebase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartitedataframe.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartitedataframe.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudy.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartiteeventstudy.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudybase.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartiteeventstudybase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartiteeventstudycollapsed.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartiteeventstudycollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudy.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartiteextendedeventstudy.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudybase.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartiteextendedeventstudybase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartiteextendedeventstudycollapsed.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartiteextendedeventstudycollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartitelong.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartitelong.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartitelongbase.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartitelongbase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/bipartitelongcollapsed.py` & `bipartitepandas-1.1.7/bipartitepandas/bipartitelongcollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/grouping/grouping.py` & `bipartitepandas-1.1.7/bipartitepandas/grouping/grouping.py`

 * *Files 12% similar despite different names*

```diff
@@ -61,28 +61,23 @@
         self.n_quantiles = n_quantiles
 
     def _compute_groups(self, data, weights, rng=None):
         '''
         Compute quantiles groups for data.
 
         Arguments:
-            data (NumPy Array): data to group
+            data (NumPy Array): firm-level data to group
             weights (NumPy Array): used for KMeans, not used for Quantiles
             rng (np.random.Generator or None): used for KMeans, not used for Quantiles
 
         Returns:
             (NumPy Array): quantile groups for data
         '''
         n_quantiles = self.n_quantiles
-        groups = np.zeros(shape=len(data))
         quantiles = np.linspace(1 / n_quantiles, 1, n_quantiles)
         quantile_groups = np.quantile(data, quantiles)
-        for i, mean_income in enumerate(data):
-            # Find quantile for each firm
-            quantile_group = 0
-            for quantile in quantile_groups:
-                if mean_income > quantile:
-                    quantile_group += 1
-                else:
-                    break
-            groups[i] = quantile_group
-        return groups
+
+        # Source: https://stackoverflow.com/a/40770360/17333120
+        # NOTE: data may be 1D or 2D
+        if len(data.shape) == 1:
+            return (data[:, None] > quantile_groups[None, :]).sum(axis=1)
+        return (data > quantile_groups[None, :]).sum(axis=1)
```

### Comparing `bipartitepandas-1.1.6/bipartitepandas/measures/measures.py` & `bipartitepandas-1.1.7/bipartitepandas/measures/measures.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/simbipartite.py` & `bipartitepandas-1.1.7/bipartitepandas/simbipartite.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas/util.py` & `bipartitepandas-1.1.7/bipartitepandas/util.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/bipartitepandas.egg-info/PKG-INFO` & `bipartitepandas-1.1.7/bipartitepandas.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipartitepandas
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python tools for bipartite labor data
 Home-page: https://github.com/tlamadon/bipartitepandas/
 Author: Thibaut Lamadon
 Author-email: thibaut.lamadon@gmail.com
 Project-URL: Documentation, https://tlamadon.github.io/bipartitepandas/
 Project-URL: GitHub, https://github.com/tlamadon/bipartitepandas/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bipartitepandas-1.1.6/bipartitepandas.egg-info/SOURCES.txt` & `bipartitepandas-1.1.7/bipartitepandas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/setup.cfg` & `bipartitepandas-1.1.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bipartitepandas
-version = 1.1.6
+version = 1.1.7
 author = Thibaut Lamadon
 author_email = thibaut.lamadon@gmail.com
 description = Python tools for bipartite labor data
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/tlamadon/bipartitepandas/
 project_urls =
```

### Comparing `bipartitepandas-1.1.6/tests/test_bpd.py` & `bipartitepandas-1.1.7/tests/test_bpd.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/tests/test_bpd_base.py` & `bipartitepandas-1.1.7/tests/test_bpd_base.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/tests/test_bpd_clustering.py` & `bipartitepandas-1.1.7/tests/test_bpd_clustering.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 '''
 Tests for bipartitepandas.
 '''
 import pytest
 import numpy as np
 import pandas as pd
 import bipartitepandas as bpd
-import pickle
 
 ################################
 ##### Tests for Clustering #####
 ################################
 
 def test_cluster_1():
     # Test cluster function is working correctly for long format.
```

### Comparing `bipartitepandas-1.1.6/tests/test_bpd_connectedness.py` & `bipartitepandas-1.1.7/tests/test_bpd_connectedness.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/tests/test_bpd_custom.py` & `bipartitepandas-1.1.7/tests/test_bpd_custom.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/tests/test_bpd_df.py` & `bipartitepandas-1.1.7/tests/test_bpd_df.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/tests/test_bpd_es.py` & `bipartitepandas-1.1.7/tests/test_bpd_es.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/tests/test_bpd_es_collapsed.py` & `bipartitepandas-1.1.7/tests/test_bpd_es_collapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/tests/test_bpd_long.py` & `bipartitepandas-1.1.7/tests/test_bpd_long.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.6/tests/test_bpd_long_collapsed.py` & `bipartitepandas-1.1.7/tests/test_bpd_long_collapsed.py`

 * *Files identical despite different names*


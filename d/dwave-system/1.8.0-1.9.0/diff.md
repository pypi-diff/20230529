# Comparing `tmp/dwave-system-1.8.0.tar.gz` & `tmp/dwave-system-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dwave-system-1.8.0.tar", last modified: Thu Sep  9 21:38:28 2021, max compression
+gzip compressed data, was "dist/dwave-system-1.9.0.tar", last modified: Fri Sep 17 18:43:50 2021, max compression
```

## Comparing `dwave-system-1.8.0.tar` & `dwave-system-1.9.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:38:28.000000 dwave-system-1.8.0/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave/embedding/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1237 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15021 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/chain_breaks.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3590 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/chain_strength.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      650 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/chimera.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      653 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/diagnostic.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4197 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/drawing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      653 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      650 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/pegasus.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      661 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/polynomialembedder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    26110 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/transforms.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10054 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/embedding/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave/system/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave/system/cache/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/cache/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2189 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/cache/cache_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    19233 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/cache/database_manager.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4292 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/cache/schema.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave/system/composites/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      865 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/composites/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15317 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/composites/cutoffcomposite.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    24785 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/composites/embedding.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15375 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/composites/reversecomposite.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10239 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/composites/tiling.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10615 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/composites/virtual_graph.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave/system/samplers/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      760 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/samplers/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15146 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/samplers/clique.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    21542 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/samplers/dwave_sampler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    23275 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/samplers/leap_hybrid_sampler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      874 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      657 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/exceptions.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3507 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/flux_bias_offsets.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1240 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/package_info.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1969 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/schedules.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7377 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/testing.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/utilities.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     8721 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/system/warnings.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2021-09-09 21:37:54.000000 dwave-system-1.8.0/dwave/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave_system.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2984 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave_system.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1372 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave_system.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave_system.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave_system.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave_system.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      222 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave_system.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2021-09-09 21:38:28.000000 dwave-system-1.8.0/dwave_system.egg-info/top_level.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11279 2021-09-09 21:37:54.000000 dwave-system-1.8.0/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2662 2021-09-09 21:37:54.000000 dwave-system-1.8.0/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2021-09-09 21:38:28.000000 dwave-system-1.8.0/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2476 2021-09-09 21:37:54.000000 dwave-system-1.8.0/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2984 2021-09-09 21:38:28.000000 dwave-system-1.8.0/PKG-INFO
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-17 18:43:49.000000 dwave-system-1.9.0/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave/embedding/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1237 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15021 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/chain_breaks.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3590 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/chain_strength.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      650 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/chimera.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      653 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/diagnostic.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4197 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/drawing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      653 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      650 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/pegasus.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      661 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/polynomialembedder.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    26110 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/transforms.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10054 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/embedding/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave/system/
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave/system/cache/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      708 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/cache/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2189 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/cache/cache_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    19233 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/cache/database_manager.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     4292 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/cache/schema.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave/system/composites/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      865 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/composites/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15317 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/composites/cutoffcomposite.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    24785 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/composites/embedding.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15375 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/composites/reversecomposite.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10239 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/composites/tiling.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10615 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/composites/virtual_graph.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave/system/samplers/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      760 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/samplers/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15146 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/samplers/clique.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    21738 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/samplers/dwave_sampler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    23275 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/samplers/leap_hybrid_sampler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      874 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      657 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/exceptions.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     3507 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/flux_bias_offsets.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1240 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/package_info.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1969 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/schedules.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     7377 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/testing.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2090 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/utilities.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     8721 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/system/warnings.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      677 2021-09-17 18:43:21.000000 dwave-system-1.9.0/dwave/__init__.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave_system.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2984 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave_system.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1372 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave_system.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave_system.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       66 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave_system.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave_system.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      223 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave_system.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        6 2021-09-17 18:43:49.000000 dwave-system-1.9.0/dwave_system.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11279 2021-09-17 18:43:21.000000 dwave-system-1.9.0/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2662 2021-09-17 18:43:21.000000 dwave-system-1.9.0/README.rst
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       80 2021-09-17 18:43:49.000000 dwave-system-1.9.0/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2477 2021-09-17 18:43:21.000000 dwave-system-1.9.0/setup.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2984 2021-09-17 18:43:49.000000 dwave-system-1.9.0/PKG-INFO
```

### Comparing `dwave-system-1.8.0/dwave/embedding/__init__.py` & `dwave-system-1.9.0/dwave/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/embedding/chain_breaks.py` & `dwave-system-1.9.0/dwave/embedding/chain_breaks.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/embedding/chain_strength.py` & `dwave-system-1.9.0/dwave/embedding/chain_strength.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/embedding/chimera.py` & `dwave-system-1.9.0/dwave/embedding/chimera.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/embedding/diagnostic.py` & `dwave-system-1.9.0/dwave/embedding/diagnostic.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/embedding/drawing.py` & `dwave-system-1.9.0/dwave/embedding/drawing.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/embedding/exceptions.py` & `dwave-system-1.9.0/dwave/embedding/exceptions.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/embedding/pegasus.py` & `dwave-system-1.9.0/dwave/embedding/pegasus.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/embedding/polynomialembedder.py` & `dwave-system-1.9.0/dwave/embedding/polynomialembedder.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/embedding/transforms.py` & `dwave-system-1.9.0/dwave/embedding/transforms.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/embedding/utils.py` & `dwave-system-1.9.0/dwave/embedding/utils.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/cache/__init__.py` & `dwave-system-1.9.0/dwave/system/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/cache/cache_manager.py` & `dwave-system-1.9.0/dwave/system/cache/cache_manager.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/cache/database_manager.py` & `dwave-system-1.9.0/dwave/system/cache/database_manager.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/cache/schema.py` & `dwave-system-1.9.0/dwave/system/cache/schema.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/composites/__init__.py` & `dwave-system-1.9.0/dwave/system/composites/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/composites/cutoffcomposite.py` & `dwave-system-1.9.0/dwave/system/composites/cutoffcomposite.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/composites/embedding.py` & `dwave-system-1.9.0/dwave/system/composites/embedding.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/composites/reversecomposite.py` & `dwave-system-1.9.0/dwave/system/composites/reversecomposite.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/composites/tiling.py` & `dwave-system-1.9.0/dwave/system/composites/tiling.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/composites/virtual_graph.py` & `dwave-system-1.9.0/dwave/system/composites/virtual_graph.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/samplers/__init__.py` & `dwave-system-1.9.0/dwave/system/samplers/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/samplers/clique.py` & `dwave-system-1.9.0/dwave/system/samplers/clique.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/samplers/dwave_sampler.py` & `dwave-system-1.9.0/dwave/system/samplers/dwave_sampler.py`

 * *Files 1% similar despite different names*

```diff
@@ -343,15 +343,16 @@
 
         """
 
         solver = self.solver
 
         if not (solver.nodes.issuperset(bqm.linear) and
                 solver.edges.issuperset(bqm.quadratic)):
-            msg = "Problem graph incompatible with solver."
+            msg = ("Problem graph incompatible with solver. Please use 'EmbeddingComposite' "
+                   "to map the problem graph to the solver.")
             raise BinaryQuadraticModelStructureError(msg)
 
         future = solver.sample_bqm(bqm, **kwargs)
 
         if warnings is None:
             warnings = self.warnings_default
         warninghandler = WarningHandler(warnings)
@@ -372,15 +373,16 @@
         return dimod.SampleSet.from_future(future, _hook)
 
     def sample_ising(self, h, *args, **kwargs):
         # to be consistent with the cloud-client, we ignore the 0 biases
         # on missing nodes for lists
         if isinstance(h, list):
             if len(h) > self.solver.num_qubits:
-                msg = "Problem graph incompatible with solver."
+                msg = ("Problem graph incompatible with solver. Please use 'EmbeddingComposite' "
+                       "to map the problem graph to the solver.")
                 raise BinaryQuadraticModelStructureError(msg)
             nodes = self.solver.nodes
             h = dict((v, b) for v, b in enumerate(h) if b and v in nodes)
 
         return super().sample_ising(h, *args, **kwargs)
 
     def validate_anneal_schedule(self, anneal_schedule):
```

### Comparing `dwave-system-1.8.0/dwave/system/samplers/leap_hybrid_sampler.py` & `dwave-system-1.9.0/dwave/system/samplers/leap_hybrid_sampler.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/__init__.py` & `dwave-system-1.9.0/dwave/system/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/exceptions.py` & `dwave-system-1.9.0/dwave/system/exceptions.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/flux_bias_offsets.py` & `dwave-system-1.9.0/dwave/system/flux_bias_offsets.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/package_info.py` & `dwave-system-1.9.0/dwave/system/package_info.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS,
 #    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #    See the License for the specific language governing permissions and
 #    limitations under the License.
 
 __all__ = ['__version__', '__author__', '__authoremail__', '__description__']
 
-__version__ = '1.8.0'
+__version__ = '1.9.0'
 __author__ = 'D-Wave Systems Inc.'
 __authoremail__ = 'acondello@dwavesys.com'
 __description__ = 'All things D-Wave System.'
 
 
 # register the non-open-source packages required for dwave-drivers to work
 contrib = [{
```

### Comparing `dwave-system-1.8.0/dwave/system/schedules.py` & `dwave-system-1.9.0/dwave/system/schedules.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/testing.py` & `dwave-system-1.9.0/dwave/system/testing.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/utilities.py` & `dwave-system-1.9.0/dwave/system/utilities.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/system/warnings.py` & `dwave-system-1.9.0/dwave/system/warnings.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave/__init__.py` & `dwave-system-1.9.0/dwave/__init__.py`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/dwave_system.egg-info/PKG-INFO` & `dwave-system-1.9.0/dwave_system.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-system
-Version: 1.8.0
+Version: 1.9.0
 Summary: All things D-Wave System.
 Home-page: https://github.com/dwavesystems/dwave-system
 Author: D-Wave Systems Inc.
 Author-email: acondello@dwavesys.com
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.6
```

### Comparing `dwave-system-1.8.0/dwave_system.egg-info/SOURCES.txt` & `dwave-system-1.9.0/dwave_system.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/LICENSE` & `dwave-system-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/README.rst` & `dwave-system-1.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `dwave-system-1.8.0/setup.py` & `dwave-system-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 setup_folder_loc = os.path.dirname(os.path.abspath(__file__))
 os.chdir(setup_folder_loc)
 
 exec(open(os.path.join(".", "dwave", "system", "package_info.py")).read())
 
 
 install_requires = ['dimod>=0.9.16,<0.11.0',
-                    'dwave-cloud-client>=0.8.4,<0.9.0',
+                    'dwave-cloud-client>=0.8.4,<0.10.0',
                     'dwave-networkx>=0.8.4',
                     'networkx>=2.0,<3.0',
                     'homebase>=1.0.0,<2.0.0',
                     'minorminer>=0.2.4,<0.3.0',
                     'numpy>=1.14.0,<2.0.0',
                     'dwave-tabu>=0.2.0',
                     ]
```

### Comparing `dwave-system-1.8.0/PKG-INFO` & `dwave-system-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwave-system
-Version: 1.8.0
+Version: 1.9.0
 Summary: All things D-Wave System.
 Home-page: https://github.com/dwavesystems/dwave-system
 Author: D-Wave Systems Inc.
 Author-email: acondello@dwavesys.com
 License: Apache 2.0
 Platform: UNKNOWN
 Requires-Python: >=3.6
```


# Comparing `tmp/graph_kmer_index-0.0.8.tar.gz` & `tmp/graph_kmer_index-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graph_kmer_index-0.0.8.tar", last modified: Mon Dec  6 20:23:06 2021, max compression
+gzip compressed data, was "graph_kmer_index-0.0.9.tar", last modified: Mon Dec  6 20:42:46 2021, max compression
```

## Comparing `graph_kmer_index-0.0.8.tar` & `graph_kmer_index-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-06 20:23:06.632715 graph_kmer_index-0.0.8/
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      282 2021-12-06 20:23:06.632715 graph_kmer_index-0.0.8/PKG-INFO
-drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-06 20:23:06.632715 graph_kmer_index-0.0.8/graph_kmer_index/
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)      569 2021-02-01 22:49:31.866081 graph_kmer_index-0.0.8/graph_kmer_index/__init__.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)     9780 2021-12-02 12:55:38.532846 graph_kmer_index-0.0.8/graph_kmer_index/collision_free_kmer_index.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)    19353 2021-12-06 20:22:02.896243 graph_kmer_index-0.0.8/graph_kmer_index/command_line_interface.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)     4499 2021-11-22 18:43:43.235660 graph_kmer_index-0.0.8/graph_kmer_index/flat_kmers.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      703 2020-12-09 19:13:47.299704 graph_kmer_index-0.0.8/graph_kmer_index/indel_kmer_finder.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2104 2021-12-02 23:00:08.373518 graph_kmer_index-0.0.8/graph_kmer_index/index_bundle.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     1061 2021-04-12 14:08:31.039685 graph_kmer_index-0.0.8/graph_kmer_index/kmer_frequency_index.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)     1700 2020-04-14 16:59:32.000000 graph_kmer_index-0.0.8/graph_kmer_index/logn_hash_map.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)     3658 2020-06-09 09:23:07.000000 graph_kmer_index-0.0.8/graph_kmer_index/read_kmers.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)     5894 2021-11-30 23:13:58.115204 graph_kmer_index-0.0.8/graph_kmer_index/reference_kmer_index.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)     3282 2021-11-03 10:11:57.976632 graph_kmer_index-0.0.8/graph_kmer_index/reverse_kmer_index.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)     6000 2021-12-06 10:26:57.183647 graph_kmer_index-0.0.8/graph_kmer_index/shared_mem.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)    16554 2021-11-29 09:15:42.223381 graph_kmer_index-0.0.8/graph_kmer_index/snp_kmer_finder.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)     2759 2020-04-22 12:10:24.000000 graph_kmer_index-0.0.8/graph_kmer_index/unique_kmer_index.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     7650 2021-11-20 21:56:18.082696 graph_kmer_index-0.0.8/graph_kmer_index/unique_variant_kmers.py
--rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      605 2021-01-02 19:36:04.771924 graph_kmer_index-0.0.8/graph_kmer_index/variant_nodes_index.py
--rw-r--r--   0 ivargry   (1000) ivargry   (1000)      752 2021-12-06 20:22:15.704338 graph_kmer_index-0.0.8/setup.py
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-06 20:42:46.687415 graph_kmer_index-0.0.9/
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      282 2021-12-06 20:42:46.687415 graph_kmer_index-0.0.9/PKG-INFO
+drwxrwxr-x   0 ivargry   (1000) ivargry   (1000)        0 2021-12-06 20:42:46.687415 graph_kmer_index-0.0.9/graph_kmer_index/
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)      569 2021-02-01 22:49:31.866081 graph_kmer_index-0.0.9/graph_kmer_index/__init__.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)     9781 2021-12-06 20:39:48.710653 graph_kmer_index-0.0.9/graph_kmer_index/collision_free_kmer_index.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)    19353 2021-12-06 20:22:02.896243 graph_kmer_index-0.0.9/graph_kmer_index/command_line_interface.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)     4499 2021-11-22 18:43:43.235660 graph_kmer_index-0.0.9/graph_kmer_index/flat_kmers.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      703 2020-12-09 19:13:47.299704 graph_kmer_index-0.0.9/graph_kmer_index/indel_kmer_finder.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     2104 2021-12-02 23:00:08.373518 graph_kmer_index-0.0.9/graph_kmer_index/index_bundle.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     1061 2021-04-12 14:08:31.039685 graph_kmer_index-0.0.9/graph_kmer_index/kmer_frequency_index.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)     1700 2020-04-14 16:59:32.000000 graph_kmer_index-0.0.9/graph_kmer_index/logn_hash_map.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)     3658 2020-06-09 09:23:07.000000 graph_kmer_index-0.0.9/graph_kmer_index/read_kmers.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)     5894 2021-11-30 23:13:58.115204 graph_kmer_index-0.0.9/graph_kmer_index/reference_kmer_index.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)     3282 2021-11-03 10:11:57.976632 graph_kmer_index-0.0.9/graph_kmer_index/reverse_kmer_index.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)     6000 2021-12-06 10:26:57.183647 graph_kmer_index-0.0.9/graph_kmer_index/shared_mem.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)    16554 2021-11-29 09:15:42.223381 graph_kmer_index-0.0.9/graph_kmer_index/snp_kmer_finder.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)     2759 2020-04-22 12:10:24.000000 graph_kmer_index-0.0.9/graph_kmer_index/unique_kmer_index.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)     7650 2021-11-20 21:56:18.082696 graph_kmer_index-0.0.9/graph_kmer_index/unique_variant_kmers.py
+-rw-rw-r--   0 ivargry   (1000) ivargry   (1000)      605 2021-01-02 19:36:04.771924 graph_kmer_index-0.0.9/graph_kmer_index/variant_nodes_index.py
+-rw-r--r--   0 ivargry   (1000) ivargry   (1000)      752 2021-12-06 20:42:41.915486 graph_kmer_index-0.0.9/setup.py
```

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/__init__.py` & `graph_kmer_index-0.0.9/graph_kmer_index/__init__.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/collision_free_kmer_index.py` & `graph_kmer_index-0.0.9/graph_kmer_index/collision_free_kmer_index.py`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
         lookup = np.zeros(modulo, dtype=np.int)
         lookup[unique_hashes] = unique_entry_positions
         n_entries = np.ediff1d(unique_entry_positions, to_end=len(nodes)-unique_entry_positions[-1])
         n_kmers = np.zeros(modulo, dtype=np.uint32)
         n_kmers[unique_hashes] = n_entries
 
         # Find out how many entries there are for each unique hash
-        object = cls(lookup, n_kmers, nodes, ref_offsets, kmers, modulo, allele_frequencies=allele_frequencies)
+        object = cls(lookup, n_kmers, nodes, ref_offsets, kmers, modulo, _allele_frequencies=allele_frequencies)
         object.set_frequencies(skip_frequencies)
 
         if skip_singletons:
             logging.info("Adding 1 to all frequencies since singletons are skipped")
             object._frequencies += 1
 
         return object
```

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/command_line_interface.py` & `graph_kmer_index-0.0.9/graph_kmer_index/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/flat_kmers.py` & `graph_kmer_index-0.0.9/graph_kmer_index/flat_kmers.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/indel_kmer_finder.py` & `graph_kmer_index-0.0.9/graph_kmer_index/indel_kmer_finder.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/index_bundle.py` & `graph_kmer_index-0.0.9/graph_kmer_index/index_bundle.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/kmer_frequency_index.py` & `graph_kmer_index-0.0.9/graph_kmer_index/kmer_frequency_index.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/logn_hash_map.py` & `graph_kmer_index-0.0.9/graph_kmer_index/logn_hash_map.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/read_kmers.py` & `graph_kmer_index-0.0.9/graph_kmer_index/read_kmers.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/reference_kmer_index.py` & `graph_kmer_index-0.0.9/graph_kmer_index/reference_kmer_index.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/reverse_kmer_index.py` & `graph_kmer_index-0.0.9/graph_kmer_index/reverse_kmer_index.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/shared_mem.py` & `graph_kmer_index-0.0.9/graph_kmer_index/shared_mem.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/snp_kmer_finder.py` & `graph_kmer_index-0.0.9/graph_kmer_index/snp_kmer_finder.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/unique_kmer_index.py` & `graph_kmer_index-0.0.9/graph_kmer_index/unique_kmer_index.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/unique_variant_kmers.py` & `graph_kmer_index-0.0.9/graph_kmer_index/unique_variant_kmers.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/graph_kmer_index/variant_nodes_index.py` & `graph_kmer_index-0.0.9/graph_kmer_index/variant_nodes_index.py`

 * *Files identical despite different names*

### Comparing `graph_kmer_index-0.0.8/setup.py` & `graph_kmer_index-0.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup, Extension
 
 
 
 setup(name='graph_kmer_index',
-      version='0.0.8',
+      version='0.0.9',
       description='Graph Kmer Index',
       url='http://github.com/ivargr/graph_kmer_index',
       author='Ivar Grytten',
       author_email='',
       license='MIT',
       packages=["graph_kmer_index"],
       zip_safe=False,
```


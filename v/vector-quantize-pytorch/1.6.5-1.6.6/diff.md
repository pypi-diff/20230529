# Comparing `tmp/vector_quantize_pytorch-1.6.5.tar.gz` & `tmp/vector_quantize_pytorch-1.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.6.5.tar", last modified: Sun May 28 17:43:45 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.6.6.tar", last modified: Mon May 29 16:34:57 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.6.5.tar` & `vector_quantize_pytorch-1.6.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:43:45.295473 vector_quantize_pytorch-1.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-28 17:43:35.000000 vector_quantize_pytorch-1.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-28 17:43:45.295473 vector_quantize_pytorch-1.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-28 17:43:35.000000 vector_quantize_pytorch-1.6.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 17:43:45.295473 vector_quantize_pytorch-1.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-28 17:43:35.000000 vector_quantize_pytorch-1.6.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:43:45.291473 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-28 17:43:35.000000 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-28 17:43:35.000000 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-28 17:43:35.000000 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (123)    30169 2023-05-28 17:43:35.000000 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 17:43:45.291473 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-28 17:43:45.000000 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-28 17:43:45.000000 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 17:43:45.000000 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-28 17:43:45.000000 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-28 17:43:45.000000 vector_quantize_pytorch-1.6.5/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:34:57.425223 vector_quantize_pytorch-1.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-29 16:34:57.425223 vector_quantize_pytorch-1.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14307 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:34:57.425223 vector_quantize_pytorch-1.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:34:57.425223 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8989 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30182 2023-05-29 16:34:41.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:34:57.425223 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-29 16:34:57.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-05-29 16:34:57.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:34:57.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-29 16:34:57.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 16:34:57.000000 vector_quantize_pytorch-1.6.6/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.6.5/LICENSE` & `vector_quantize_pytorch-1.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.5/PKG-INFO` & `vector_quantize_pytorch-1.6.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.6.5
+Version: 1.6.6
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.6.5/README.md` & `vector_quantize_pytorch-1.6.6/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.5/setup.py` & `vector_quantize_pytorch-1.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.6.5',
+  version = '1.6.6',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.6.5/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.5/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.6.5/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.6.6/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files 0% similar despite different names*

```diff
@@ -588,15 +588,15 @@
         if self.training and self.ema_update:
             bins = embed_onehot.sum(dim = 1)
             self.all_reduce_fn(bins)
 
             self.cluster_size.data.lerp_(bins, 1 - self.decay)
 
             embed_sum = einsum('h n d, h n c -> h c d', flatten, embed_onehot)
-            self.all_reduce_fn(embed_sum)
+            self.all_reduce_fn(embed_sum.contiguous())
             self.embed_avg.data.lerp_(embed_sum, 1 - self.decay)
 
             cluster_size = laplace_smoothing(self.cluster_size, self.codebook_size, self.eps) * self.cluster_size.sum(dim = -1, keepdim = True)
 
             embed_normalized = self.embed_avg / rearrange(cluster_size, '... -> ... 1')
             embed_normalized = l2norm(embed_normalized)
```


# Comparing `tmp/MEGABYTE-pytorch-0.1.0.tar.gz` & `tmp/MEGABYTE-pytorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.1.0.tar", last modified: Mon May 29 16:28:29 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.1.1.tar", last modified: Mon May 29 16:53:58 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.1.0.tar` & `MEGABYTE-pytorch-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:28:29.521912 MEGABYTE-pytorch-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:28:29.517912 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:28:29.517912 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-29 16:28:29.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-29 16:28:29.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:28:29.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-29 16:28:29.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 16:28:29.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-29 16:28:29.517912 MEGABYTE-pytorch-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:28:29.521912 MEGABYTE-pytorch-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:58.616893 MEGABYTE-pytorch-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 16:53:43.000000 MEGABYTE-pytorch-0.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:58.616893 MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 16:53:43.000000 MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-29 16:53:43.000000 MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13466 2023-05-29 16:53:43.000000 MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:53:58.616893 MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-29 16:53:58.000000 MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-29 16:53:58.000000 MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:53:58.000000 MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-29 16:53:58.000000 MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 16:53:58.000000 MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-29 16:53:58.616893 MEGABYTE-pytorch-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-29 16:53:43.000000 MEGABYTE-pytorch-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:53:58.616893 MEGABYTE-pytorch-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-29 16:53:43.000000 MEGABYTE-pytorch-0.1.1/setup.py
```

### Comparing `MEGABYTE-pytorch-0.1.0/LICENSE` & `MEGABYTE-pytorch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/attend.py` & `MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch/megabyte.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,16 +267,16 @@
                 flash_attn = flash_attn
             ))
 
             proj = nn.Identity()
 
             if exists(next_h_dim) and next_h_dim != dim:
                 proj = nn.Sequential(
-                    nn.Linear(h_dim, next_h_dim * (next_seq_len + 1)),
-                    Rearrange('... (n d) -> (...) n d', n = next_seq_len + 1)
+                    nn.Linear(h_dim, next_h_dim * next_seq_len),
+                    Rearrange('... (n d) -> (...) n d', n = next_seq_len)
                 )
 
             self.to_next_transformer_projections.append(proj)
 
         self.to_logits = nn.Linear(fine_dim, num_tokens)
         self.pad_id = pad_id
 
@@ -378,15 +378,16 @@
                 stage_start_tokens,
                 stage_tokens,
             ), dim = -2)
 
             # sum the previous hierarchy's representation
 
             if exists(prev_stage_tokens_repr):
-                stage_tokens = stage_tokens + prev_stage_tokens_repr[..., :stage_tokens.shape[-2], :]
+                prev_stage_tokens_repr = F.pad(prev_stage_tokens_repr, (0, 0, 1, 0), value = 0.)
+                stage_tokens = stage_tokens + prev_stage_tokens_repr
 
             attended = transformer(stage_tokens)
 
             attended = unpack_one(attended, ps, '* n d')
 
             # project for next stage in the hierarchy
```

### Comparing `MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.1.1/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.1.0/PKG-INFO` & `MEGABYTE-pytorch-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.1.0/README.md` & `MEGABYTE-pytorch-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.1.0/setup.py` & `MEGABYTE-pytorch-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.1.0',
+  version = '0.1.1',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```


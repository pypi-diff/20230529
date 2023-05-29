# Comparing `tmp/MEGABYTE-pytorch-0.0.9.tar.gz` & `tmp/MEGABYTE-pytorch-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.0.9.tar", last modified: Fri May 26 16:46:54 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.1.0.tar", last modified: Mon May 29 16:28:29 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.0.9.tar` & `MEGABYTE-pytorch-0.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:46:54.771808 MEGABYTE-pytorch-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:46:54.771808 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:46:54.771808 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 16:46:54.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-26 16:46:54.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:46:54.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 16:46:54.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:46:54.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 16:46:54.771808 MEGABYTE-pytorch-0.0.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:46:54.771808 MEGABYTE-pytorch-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:28:29.521912 MEGABYTE-pytorch-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:28:29.517912 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:28:29.517912 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-29 16:28:29.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-29 16:28:29.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:28:29.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-29 16:28:29.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-29 16:28:29.000000 MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-29 16:28:29.517912 MEGABYTE-pytorch-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:28:29.521912 MEGABYTE-pytorch-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-05-29 16:28:16.000000 MEGABYTE-pytorch-0.1.0/setup.py
```

### Comparing `MEGABYTE-pytorch-0.0.9/LICENSE` & `MEGABYTE-pytorch-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/attend.py` & `MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch/megabyte.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 import torch
 import torch.nn.functional as F
 from torch import nn, einsum
 
 from einops import rearrange, reduce, repeat, pack, unpack
 from einops.layers.torch import Rearrange
 
+from beartype import beartype
+from beartype.typing import Tuple, Union
+
 from MEGABYTE_pytorch.attend import Attend
 
 from tqdm import tqdm
 
 # helpers
 
 def exists(val):
@@ -196,21 +199,23 @@
             x = ff(token_shift(x)) + x
 
         return self.norm(x)
 
 # main class
 
 class MEGABYTE(nn.Module):
+
+    @beartype
     def __init__(
         self,
         *,
         num_tokens,
-        dim,
-        depth: tuple,
-        max_seq_len: tuple,
+        dim: Union[Tuple, int],
+        depth: Tuple,
+        max_seq_len: Tuple,
         dim_head = 64,
         heads = 8,
         attn_dropout = 0.,
         ff_mult = 4,
         ff_dropout = 0.,
         pad_id = 0,
         rel_pos_bias = True,
@@ -229,44 +234,51 @@
         dim = cast_tuple(dim, self.stages)
 
         assert len(dim) == self.stages
 
         coarsest_dim, *_, fine_dim = dim
 
         self.token_emb = nn.Embedding(num_tokens, fine_dim)
-        self.start_tokens = nn.Parameter(torch.randn(coarsest_dim))
 
         self.max_seq_len = max_seq_len
 
+        self.start_tokens = nn.ParameterList([nn.Parameter(torch.randn(h_dim)) for h_dim, seq_len in zip(dim, max_seq_len)])
         self.pos_embs = nn.ModuleList([nn.Embedding(seq_len, h_dim) for h_dim, seq_len in zip(dim, max_seq_len)])
 
         self.patch_embedders = nn.ModuleList([nn.Sequential(
             Rearrange('... r d -> ... (r d)'),
             nn.LayerNorm(seq_len * dim_in),
             nn.Linear(seq_len * dim_in, dim_out),
             nn.LayerNorm(dim_out)
         ) for dim_in, dim_out, seq_len in zip(dim[1:], dim[:-1], max_seq_len[1:])])
 
         self.transformers = nn.ModuleList([])
         self.to_next_transformer_projections = nn.ModuleList([])
 
-        for h_dim, next_h_dim, stage_depth in zip_longest(dim, dim[1:], depth):
+        for h_dim, next_h_dim, stage_depth, next_seq_len in zip_longest(dim, dim[1:], depth, max_seq_len[1:]):
             self.transformers.append(Transformer(
                 dim = h_dim,
                 layers = stage_depth,
                 dim_head = dim_head,
                 heads = heads,
                 attn_dropout = attn_dropout,
                 ff_dropout = ff_dropout,
                 ff_mult = ff_mult,
                 rel_pos_bias = rel_pos_bias,
                 flash_attn = flash_attn
             ))
 
-            proj = nn.Linear(h_dim, next_h_dim) if exists(next_h_dim) and next_h_dim != dim else nn.Identity()
+            proj = nn.Identity()
+
+            if exists(next_h_dim) and next_h_dim != dim:
+                proj = nn.Sequential(
+                    nn.Linear(h_dim, next_h_dim * (next_seq_len + 1)),
+                    Rearrange('... (n d) -> (...) n d', n = next_seq_len + 1)
+                )
+
             self.to_next_transformer_projections.append(proj)
 
         self.to_logits = nn.Linear(fine_dim, num_tokens)
         self.pad_id = pad_id
 
     def generate(self, prime = None, filter_thres = 0.9, temperature = 1., default_batch_size = 1):
         total_seq_len = reduce_mult(self.max_seq_len)
@@ -286,18 +298,24 @@
 
         return seq.reshape(batch, *self.max_seq_len)
 
     def forward_empty(self, batch_size):
         # take care of special case
         # where you sample from input of 0 (start token only)
 
-        tokens = repeat(self.start_tokens, 'd -> b 1 d', b = batch_size)
+        prev_stage_tokens_repr = None
+
+        for stage_start_tokens, transformer, proj in zip(self.start_tokens, self.transformers, self.to_next_transformer_projections):
+            tokens = repeat(stage_start_tokens, 'd -> b 1 d', b = batch_size)
+
+            if exists(prev_stage_tokens_repr):
+                tokens = tokens + prev_stage_tokens_repr[..., :tokens.shape[-2], :]
 
-        for transformer in self.transformers:
             tokens = transformer(tokens)
+            prev_stage_tokens_repr = proj(tokens)
 
         return self.to_logits(tokens)
 
     def forward(self, ids, return_loss = False):
         batch = ids.shape[0]
 
         assert ids.ndim in {2, self.stages + 1}
@@ -339,36 +357,46 @@
             if not is_first:
                 reduced_tokens = patch_emb(reduced_tokens)
 
             positions = pos_emb(torch.arange(reduced_tokens.shape[-2], device = device))
             tokens_with_position = reduced_tokens + positions
             tokens_at_stages.insert(0, tokens_with_position)
 
-        # get start tokens and append to the coarsest stage
+        # the un-pixelshuffled representations of the previous hierarchy, starts with None
 
-        start_tokens = repeat(self.start_tokens, 'f -> b 1 f', b = b)
+        prev_stage_tokens_repr = None
 
         # spatial tokens is tokens with depth pos reduced along depth dimension + spatial positions        
 
-        for ind, (stage_tokens, transformer, proj) in enumerate(zip(tokens_at_stages, self.transformers, self.to_next_transformer_projections)):
-            is_last = ind == (self.stages - 1)
+        for stage_start_tokens, stage_tokens, transformer, proj in zip(self.start_tokens, tokens_at_stages, self.transformers, self.to_next_transformer_projections):
+            stage_tokens, ps = pack_one(stage_tokens, '* n d')
+
+            stage_start_tokens = repeat(stage_start_tokens, 'f -> b 1 f', b = stage_tokens.shape[0])
+
+            # concat start token
 
             stage_tokens = torch.cat((
-                start_tokens,
+                stage_start_tokens,
                 stage_tokens,
             ), dim = -2)
 
-            stage_tokens, ps = pack_one(stage_tokens, '* n d')
+            # sum the previous hierarchy's representation
+
+            if exists(prev_stage_tokens_repr):
+                stage_tokens = stage_tokens + prev_stage_tokens_repr[..., :stage_tokens.shape[-2], :]
 
             attended = transformer(stage_tokens)
-            attended = proj(attended)
 
             attended = unpack_one(attended, ps, '* n d')
 
-            start_tokens = rearrange(attended[..., :-1, :], '... n d -> ... n 1 d')
+            # project for next stage in the hierarchy
+
+            prev_stage_tokens_repr = proj(attended[..., :-1, :])
+
+        # project to logits
 
         logits = self.to_logits(attended)
 
         logits = logits[..., 1:, :]
 
         if not return_loss:
```

### Comparing `MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.1.0/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.9
+Version: 0.1.0
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.9/PKG-INFO` & `MEGABYTE-pytorch-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.9
+Version: 0.1.0
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.9/README.md` & `MEGABYTE-pytorch-0.1.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 # or you can use the generate function
 
 sampled = model.generate(temperature = 0.9, filter_thres = 0.9) # (1, 1024, 4)
 ```
 
 ## Test
 
-Train on character-level enwik8 with patches of size 4
+Train on character-level enwik8 with patches of size 4 - length 8192
 
 ```bash
 $ python train.py
 ```
 
 ## Citations
```

#### html2text {}

```diff
@@ -12,27 +12,27 @@
 layers for global and then local. this can be more than 2, but length must
 match the max_seq_len's dim_head = 64, # dimension per head heads = 8, # number
 of attention heads flash_attn = True # use flash attention ) x = torch.randint
 (0, 16000, (1, 1024, 4)) loss = model(x, return_loss = True) loss.backward() #
 then after much training logits = model(x) # and sample from the logits
 accordingly # or you can use the generate function sampled = model.generate
 (temperature = 0.9, filter_thres = 0.9) # (1, 1024, 4) ``` ## Test Train on
-character-level enwik8 with patches of size 4 ```bash $ python train.py ``` ##
-Citations ```bibtex @misc{yu2023megabyte, title = {MEGABYTE: Predicting
-Million-byte Sequences with Multiscale Transformers}, author = {Lili Yu and
-DÃ¡niel Simig and Colin Flaherty and Armen Aghajanyan and Luke Zettlemoyer and
-Mike Lewis}, year = {2023}, eprint = {2305.07185}, archivePrefix = {arXiv},
-primaryClass = {cs.LG} } ``` ```bibtex @misc{https://doi.org/10.48550/
-arxiv.2302.01327, doi = {10.48550/ARXIV.2302.01327}, url = {https://arxiv.org/
-abs/2302.01327}, author = {Kumar, Manoj and Dehghani, Mostafa and Houlsby,
-Neil}, title = {Dual PatchNorm}, publisher = {arXiv}, year = {2023}, copyright
-= {Creative Commons Attribution 4.0 International} } ``` ```bibtex
-@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
-Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
-Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+character-level enwik8 with patches of size 4 - length 8192 ```bash $ python
+train.py ``` ## Citations ```bibtex @misc{yu2023megabyte, title = {MEGABYTE:
+Predicting Million-byte Sequences with Multiscale Transformers}, author = {Lili
+Yu and DÃ¡niel Simig and Colin Flaherty and Armen Aghajanyan and Luke
+Zettlemoyer and Mike Lewis}, year = {2023}, eprint = {2305.07185},
+archivePrefix = {arXiv}, primaryClass = {cs.LG} } ``` ```bibtex @misc{https://
+doi.org/10.48550/arxiv.2302.01327, doi = {10.48550/ARXIV.2302.01327}, url =
+{https://arxiv.org/abs/2302.01327}, author = {Kumar, Manoj and Dehghani,
+Mostafa and Houlsby, Neil}, title = {Dual PatchNorm}, publisher = {arXiv}, year
+= {2023}, copyright = {Creative Commons Attribution 4.0 International} } ```
+```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
+and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
+and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
 booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
 } ``` ```bibtex @misc{press2021ALiBi, title = {Train Short, Test Long:
 Attention with Linear Biases Enable Input Length Extrapolation}, author = {Ofir
 Press and Noah A. Smith and Mike Lewis}, year = {2021}, url = {https://ofir.io/
 train_short_test_long.pdf} } ``` ```bibtex @software{peng_bo_2021_5196578,
 author = {PENG Bo}, title = {BlinkDL/RWKV-LM: 0.01}, month = {aug}, year =
 {2021}, publisher = {Zenodo}, version = {0.01}, doi = {10.5281/zenodo.5196578},
```

### Comparing `MEGABYTE-pytorch-0.0.9/setup.py` & `MEGABYTE-pytorch-0.1.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.0.9',
+  version = '0.1.0',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
     'artificial intelligence',
     'attention mechanism',
     'transformers'
   ],
   install_requires=[
+    'beartype',
     'einops>=0.6.1',
     'torch>=1.10',
     'tqdm'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
```


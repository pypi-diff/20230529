# Comparing `tmp/semantic-cleaning-0.0.3.tar.gz` & `tmp/semantic-cleaning-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic-cleaning-0.0.3.tar", last modified: Mon May 29 08:45:14 2023, max compression
+gzip compressed data, was "semantic-cleaning-0.0.4.tar", last modified: Mon May 29 20:01:37 2023, max compression
```

## Comparing `semantic-cleaning-0.0.3.tar` & `semantic-cleaning-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,35 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:45:14.868780 semantic-cleaning-0.0.3/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-29 08:41:52.000000 semantic-cleaning-0.0.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-29 08:41:52.000000 semantic-cleaning-0.0.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2870 2023-05-29 08:45:14.868780 semantic-cleaning-0.0.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2066 2023-05-29 08:41:52.000000 semantic-cleaning-0.0.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:45:14.865780 semantic-cleaning-0.0.3/semantic_cleaning/
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-29 08:45:01.000000 semantic-cleaning-0.0.3/semantic_cleaning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-05-29 08:45:01.000000 semantic-cleaning-0.0.3/semantic_cleaning/_modidx.py
--rw-r--r--   0 root         (0) root         (0)     8221 2023-05-29 08:45:01.000000 semantic-cleaning-0.0.3/semantic_cleaning/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:45:14.867780 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2870 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 08:44:11.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      942 2023-05-29 08:45:01.000000 semantic-cleaning-0.0.3/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 08:45:14.868780 semantic-cleaning-0.0.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2596 2023-05-29 08:41:52.000000 semantic-cleaning-0.0.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:01:37.449683 semantic-cleaning-0.0.4/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:01:37.449683 semantic-cleaning-0.0.4/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:01:37.449683 semantic-cleaning-0.0.4/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      242 2023-05-29 16:28:31.000000 semantic-cleaning-0.0.4/.github/workflows/deploy.yaml
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-29 16:28:31.000000 semantic-cleaning-0.0.4/.github/workflows/test.yaml
+-rw-r--r--   0 root         (0) root         (0)     1608 2023-05-29 16:28:31.000000 semantic-cleaning-0.0.4/.gitignore
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-29 16:28:31.000000 semantic-cleaning-0.0.4/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-29 16:28:31.000000 semantic-cleaning-0.0.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4438 2023-05-29 20:01:37.449683 semantic-cleaning-0.0.4/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3614 2023-05-29 19:47:47.000000 semantic-cleaning-0.0.4/README.md
+-rwxr-xr-x   0 root         (0) root         (0)      104 2023-05-29 16:28:31.000000 semantic-cleaning-0.0.4/colab_setup.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:01:37.449683 semantic-cleaning-0.0.4/nbs/
+-rw-r--r--   0 root         (0) root         (0)   176914 2023-05-29 19:47:42.000000 semantic-cleaning-0.0.4/nbs/00_core.ipynb
+-rw-r--r--   0 root         (0) root         (0)      290 2023-05-29 16:28:31.000000 semantic-cleaning-0.0.4/nbs/_quarto.yml
+-rw-r--r--   0 root         (0) root         (0)     6383 2023-05-29 19:47:42.000000 semantic-cleaning-0.0.4/nbs/index.ipynb
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-29 19:47:42.000000 semantic-cleaning-0.0.4/nbs/nbdev.yml
+-rw-r--r--   0 root         (0) root         (0)      600 2023-05-29 16:28:31.000000 semantic-cleaning-0.0.4/nbs/styles.css
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 16:28:31.000000 semantic-cleaning-0.0.4/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     2882 2023-05-29 18:09:05.000000 semantic-cleaning-0.0.4/semantic-cleaning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:01:37.449683 semantic-cleaning-0.0.4/semantic_cleaning/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-29 19:30:29.000000 semantic-cleaning-0.0.4/semantic_cleaning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-05-29 19:30:29.000000 semantic-cleaning-0.0.4/semantic_cleaning/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)     8896 2023-05-29 19:30:29.000000 semantic-cleaning-0.0.4/semantic_cleaning/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:01:37.449683 semantic-cleaning-0.0.4/semantic_cleaning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4438 2023-05-29 20:01:37.000000 semantic-cleaning-0.0.4/semantic_cleaning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      631 2023-05-29 20:01:37.000000 semantic-cleaning-0.0.4/semantic_cleaning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 20:01:37.000000 semantic-cleaning-0.0.4/semantic_cleaning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-29 20:01:37.000000 semantic-cleaning-0.0.4/semantic_cleaning.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 19:53:45.000000 semantic-cleaning-0.0.4/semantic_cleaning.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-29 20:01:37.000000 semantic-cleaning-0.0.4/semantic_cleaning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 20:01:37.000000 semantic-cleaning-0.0.4/semantic_cleaning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      942 2023-05-29 16:33:40.000000 semantic-cleaning-0.0.4/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 20:01:37.449683 semantic-cleaning-0.0.4/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-05-29 16:28:31.000000 semantic-cleaning-0.0.4/setup.py
+-rw-r--r--   0 root         (0) root         (0)       41 2023-05-29 16:33:18.000000 semantic-cleaning-0.0.4/token
```

### Comparing `semantic-cleaning-0.0.3/LICENSE` & `semantic-cleaning-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic-cleaning-0.0.3/semantic_cleaning/_modidx.py` & `semantic-cleaning-0.0.4/semantic_cleaning/_modidx.py`

 * *Files identical despite different names*

### Comparing `semantic-cleaning-0.0.3/semantic_cleaning/core.py` & `semantic-cleaning-0.0.4/semantic_cleaning/core.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 # %% ../nbs/00_core.ipynb 10
 from tqdm.auto import tqdm
 from typing import List, Dict, Set, Union, Callable
 import torch
 from torch.utils.data import DataLoader
-from datasets import Dataset, load_dataset
+from datasets import Dataset, load_dataset, DatasetDict
 import numpy as np
 from transformers import AutoTokenizer, AutoModel, AutoModelForCausalLM
 import torch.nn.functional as F
 import transformers
 
 # %% ../nbs/00_core.ipynb 13
 def preprocess_data(dataset: Dataset, splits: Union[str, List[str]] = None, schema: str = "") -> Dataset:
@@ -118,66 +118,72 @@
     # Clear CUDA memory
     torch.cuda.empty_cache()
 
     return np.concatenate(embeddings_list, 0)
 
 
 # %% ../nbs/00_core.ipynb 18
-def deduplicate_embeddings(embedded, epsilon=1e-2, batch_size=20000):
+def deduplicate_embeddings(embedded, embedded2=None, epsilon=1e-2, batch_size=20000):
     """
-    Perform deduplication on the provided embeddings.
+    Perform deduplication on the provided embeddings. If a second set of embeddings is provided,
+    return the indices of embeddings in the second set that are duplicates of embeddings in the first set.
 
     Args:
-        embedded: A numpy array or PyTorch tensor holding the embeddings.
+        embedded1: A numpy array or PyTorch tensor holding the embeddings of the first set.
+        embedded2: A numpy array or PyTorch tensor holding the embeddings of the second set (optional).
         epsilon: The maximum distance for two embeddings to be considered duplicates (using cosine similarity).
         batch_size: The size of the batches to process at a time.
 
     Note: The embeddings must be L2 normalized.
 
     Returns:
-        A tensor of indices that should be deleted due to duplication.
+        If a second set of embeddings is provided, a tensor of indices of the second set that are duplicates of the first set.
+        If a second set of embeddings is not provided, a tensor of indices that should be deleted due to duplication in the first set.
     """
-
+    embedded1 = embedded
     to_delete = torch.empty(0, dtype=int)
-    embedded_tensor = torch.tensor(embedded, dtype=torch.float16, device='cuda', requires_grad=False)
+    embedded_tensor1 = torch.tensor(embedded1, dtype=torch.float16, device='cuda', requires_grad=False)
 
-    for i in range(embedded.shape[0]//batch_size+1):
-        
-        # Calculate the cosine distance within the current batch
-        cosine_dist = 1 - torch.matmul(embedded_tensor[i*batch_size:(i+1)*batch_size],
-                                        torch.transpose(embedded_tensor[i*batch_size:(i+1)*batch_size], 0, 1))
-        
-        cosine_dist = cosine_dist + torch.eye(cosine_dist.shape[0],device='cuda')
-        
-        # Find duplicate indices within the batch
-        dup_indices = torch.where(cosine_dist < epsilon)
-        to_delete = torch.cat((to_delete, dup_indices[0][torch.where(dup_indices[0] > dup_indices[1])].to('cpu') + (i*batch_size)))
-
-        # Find duplicate indices across the current batch and remaining batches
-        for k in range(i+1, embedded.shape[0]//batch_size+1):
-            cosine_dist = 1 - torch.matmul(embedded_tensor[i*batch_size:(i+1)*batch_size],
-                                            torch.transpose(embedded_tensor[k*batch_size:(k+1)*batch_size], 0, 1))
+    if embedded2 is None:
+        embedded2 = embedded1
+        embedded_tensor2 = embedded_tensor1
+    else:
+        embedded_tensor2 = torch.tensor(embedded2, dtype=torch.float16, device='cuda', requires_grad=False)
+
+    for i in range(embedded1.shape[0]//batch_size+1):
+        start_j = 0 if embedded2 is not embedded1 else i
+        for j in range(start_j, embedded2.shape[0]//batch_size+1):
+            cosine_dist = 1 - torch.matmul(embedded_tensor1[i*batch_size:(i+1)*batch_size],
+                                            torch.transpose(embedded_tensor2[j*batch_size:(j+1)*batch_size], 0, 1))
+
+            if embedded2 is embedded1 and i == j:
+                cosine_dist = cosine_dist + torch.eye(cosine_dist.shape[0], device='cuda')
 
             dup_indices = torch.where(cosine_dist < epsilon)
-            to_delete = torch.cat((to_delete, dup_indices[1].to('cpu') + k*batch_size))
+
+            if embedded2 is embedded1 and i == j:
+                to_delete = torch.cat((to_delete, dup_indices[0][torch.where(dup_indices[0] > dup_indices[1])].to('cpu') + (i*batch_size)))
+            else:
+                to_delete = torch.cat((to_delete, dup_indices[1].to('cpu') + j*batch_size))
 
             torch.cuda.empty_cache()
 
     return to_delete
 
+
 # %% ../nbs/00_core.ipynb 20
 def deduplicate_dataset(
     dataset: Dataset, 
     model: torch.nn.Module, 
     tokenizer,
     epsilon: float = 1e-2, 
     model_batch_size: int = 64, 
     deduplication_batch_size: int =20000, 
     num_workers: int = 16,
-    dataset_feature: str = '_merged'
+    dataset_feature: str = ''
 ) -> Dataset:
     """
     Deduplicate data in a dataset based on the embeddings computed by a given model.
 
     Args:
         dataset: Dataset to be deduplicated.
         model: Model to compute embeddings.
@@ -186,23 +192,27 @@
         deduplication_batch_size: Batch size for deduplication process.
         num_workers: Number of worker processes for data loading.
         dataset_feature: Feature in the dataset to use for deduplication.
 
     Returns:
         Deduplicated dataset.
     """
+    
+    if not dataset_feature:
+        dataset=preprocess_data(dataset)
+        dataset_feature ='_merged'
     # Compute embeddings for the dataset
-    embeddings = compute_embeddings(dataset, 
+    embeddings = compute_embeddings(dataset if not isinstance(dataset,DatasetDict) else dataset[list(dataset.keys())[0]], 
                                     model, 
                                     tokenizer,
                                     batch_size=model_batch_size, 
                                     num_workers=num_workers, 
                                     dataset_feature=dataset_feature)
     
     # Find duplicate indices in the embeddings
-    duplicate_indices = deduplicate_embeddings(embeddings, epsilon, deduplication_batch_size)
+    duplicate_indices = deduplicate_embeddings(embedded = embeddings, epsilon=epsilon, batch_size=deduplication_batch_size)
     
     # Filter out duplicate instances from the dataset
     deduplicated_dataset = dataset.filter(lambda example, idx: idx not in duplicate_indices, with_indices=True)
 
     return deduplicated_dataset
```

### Comparing `semantic-cleaning-0.0.3/settings.ini` & `semantic-cleaning-0.0.4/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = semantic-cleaning
 lib_name = semantic-cleaning
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = semantic_cleaning
 nbs_path = nbs
 recursive = True
```

### Comparing `semantic-cleaning-0.0.3/setup.py` & `semantic-cleaning-0.0.4/setup.py`

 * *Files identical despite different names*


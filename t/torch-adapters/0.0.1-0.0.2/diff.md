# Comparing `tmp/torch_adapters-0.0.1.tar.gz` & `tmp/torch_adapters-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_adapters-0.0.1.tar", max compression
+gzip compressed data, was "torch_adapters-0.0.2.tar", max compression
```

## Comparing `torch_adapters-0.0.1.tar` & `torch_adapters-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1062 2023-05-29 03:00:27.152099 torch_adapters-0.0.1/LICENSE
--rw-r--r--   0        0        0       16 2023-05-29 03:00:27.152099 torch_adapters-0.0.1/README.md
--rw-r--r--   0        0        0      344 2023-05-29 03:11:54.685817 torch_adapters-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 03:01:19.456108 torch_adapters-0.0.1/src/torch_adapters/__init__.py
--rw-r--r--   0        0        0        0 2023-05-29 03:03:05.272210 torch_adapters-0.0.1/src/torch_adapters/adapters/__init__.py
--rw-r--r--   0        0        0      856 2023-05-29 03:15:43.714839 torch_adapters-0.0.1/src/torch_adapters/adapters/lora.py
--rw-r--r--   0        0        0      830 2023-05-29 03:11:05.229614 torch_adapters-0.0.1/src/torch_adapters/utils.py
--rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 torch_adapters-0.0.1/setup.py
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 torch_adapters-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-29 03:00:27.152099 torch_adapters-0.0.2/LICENSE
+-rw-r--r--   0        0        0       16 2023-05-29 03:00:27.152099 torch_adapters-0.0.2/README.md
+-rw-r--r--   0        0        0      344 2023-05-29 03:32:14.756743 torch_adapters-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 03:01:19.456108 torch_adapters-0.0.2/src/torch_adapters/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-29 03:03:05.272210 torch_adapters-0.0.2/src/torch_adapters/adapters/__init__.py
+-rw-r--r--   0        0        0      856 2023-05-29 03:15:43.714839 torch_adapters-0.0.2/src/torch_adapters/adapters/lora.py
+-rw-r--r--   0        0        0      831 2023-05-29 03:28:01.368234 torch_adapters-0.0.2/src/torch_adapters/utils.py
+-rw-r--r--   0        0        0      702 1970-01-01 00:00:00.000000 torch_adapters-0.0.2/setup.py
+-rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 torch_adapters-0.0.2/PKG-INFO
```

### Comparing `torch_adapters-0.0.1/LICENSE` & `torch_adapters-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_adapters-0.0.1/src/torch_adapters/adapters/lora.py` & `torch_adapters-0.0.2/src/torch_adapters/adapters/lora.py`

 * *Files identical despite different names*

### Comparing `torch_adapters-0.0.1/src/torch_adapters/utils.py` & `torch_adapters-0.0.2/src/torch_adapters/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from operator import attrgetter
 from typing import List
 
 import torch
 
-from adapters.lora import LoRA
+from .adapters.lora import LoRA
 
 
 def add_lora(model: torch.nn.Module, layers_names: List[str]) -> torch.nn.Module:
     """
 
     :param model:
     :param layers_names:
```

### Comparing `torch_adapters-0.0.1/setup.py` & `torch_adapters-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['torch>=2.0.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'torch-adapters',
-    'version': '0.0.1',
+    'version': '0.0.2',
     'description': '',
     'long_description': '# torch-adapters',
     'author': 'ma2za',
     'author_email': 'mazzapaolo2019@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```


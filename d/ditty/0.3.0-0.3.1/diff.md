# Comparing `tmp/ditty-0.3.0.tar.gz` & `tmp/ditty-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditty-0.3.0.tar", last modified: Fri May 26 21:59:47 2023, max compression
+gzip compressed data, was "ditty-0.3.1.tar", last modified: Mon May 29 11:54:13 2023, max compression
```

## Comparing `ditty-0.3.0.tar` & `ditty-0.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-26 21:59:47.635318 ditty-0.3.0/
--rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.3.0/LICENSE
--rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-26 21:59:47.635318 ditty-0.3.0/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)     2872 2023-05-23 04:03:46.000000 ditty-0.3.0/README.md
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-26 21:59:47.635318 ditty-0.3.0/lib/
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-26 21:59:47.635318 ditty-0.3.0/lib/ditty/
--rw-rw-r--   0 crow      (1000) crow      (1000)        0 2023-05-21 15:10:10.000000 ditty-0.3.0/lib/ditty/__init__.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     5251 2023-05-26 05:12:23.000000 ditty-0.3.0/lib/ditty/data.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     7238 2023-05-26 06:50:37.000000 ditty-0.3.0/lib/ditty/pipeline.py
--rw-rw-r--   0 crow      (1000) crow      (1000)     6597 2023-05-26 21:56:46.000000 ditty-0.3.0/lib/ditty/trainer.py
-drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-26 21:59:47.635318 ditty-0.3.0/lib/ditty.egg-info/
--rw-rw-r--   0 crow      (1000) crow      (1000)     3170 2023-05-26 21:59:47.000000 ditty-0.3.0/lib/ditty.egg-info/PKG-INFO
--rw-rw-r--   0 crow      (1000) crow      (1000)      283 2023-05-26 21:59:47.000000 ditty-0.3.0/lib/ditty.egg-info/SOURCES.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-26 21:59:47.000000 ditty-0.3.0/lib/ditty.egg-info/dependency_links.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-26 21:59:47.000000 ditty-0.3.0/lib/ditty.egg-info/requires.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)        6 2023-05-26 21:59:47.000000 ditty-0.3.0/lib/ditty.egg-info/top_level.txt
--rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-26 21:59:47.635318 ditty-0.3.0/setup.cfg
--rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-26 21:58:03.000000 ditty-0.3.0/setup.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-29 11:54:13.110935 ditty-0.3.1/
+-rw-rw-r--   0 crow      (1000) crow      (1000)    11357 2023-05-20 22:13:26.000000 ditty-0.3.1/LICENSE
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3435 2023-05-29 11:54:13.110935 ditty-0.3.1/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3138 2023-05-29 11:53:59.000000 ditty-0.3.1/README.md
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-29 11:54:13.110935 ditty-0.3.1/lib/
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-29 11:54:13.110935 ditty-0.3.1/lib/ditty/
+-rw-rw-r--   0 crow      (1000) crow      (1000)        0 2023-05-21 15:10:10.000000 ditty-0.3.1/lib/ditty/__init__.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     5251 2023-05-26 05:12:23.000000 ditty-0.3.1/lib/ditty/data.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     7288 2023-05-29 11:53:59.000000 ditty-0.3.1/lib/ditty/pipeline.py
+-rw-rw-r--   0 crow      (1000) crow      (1000)     6597 2023-05-27 06:36:39.000000 ditty-0.3.1/lib/ditty/trainer.py
+drwxrwxr-x   0 crow      (1000) crow      (1000)        0 2023-05-29 11:54:13.110935 ditty-0.3.1/lib/ditty.egg-info/
+-rw-rw-r--   0 crow      (1000) crow      (1000)     3435 2023-05-29 11:54:13.000000 ditty-0.3.1/lib/ditty.egg-info/PKG-INFO
+-rw-rw-r--   0 crow      (1000) crow      (1000)      283 2023-05-29 11:54:13.000000 ditty-0.3.1/lib/ditty.egg-info/SOURCES.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        1 2023-05-29 11:54:13.000000 ditty-0.3.1/lib/ditty.egg-info/dependency_links.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)       56 2023-05-29 11:54:13.000000 ditty-0.3.1/lib/ditty.egg-info/requires.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)        6 2023-05-29 11:54:13.000000 ditty-0.3.1/lib/ditty.egg-info/top_level.txt
+-rw-rw-r--   0 crow      (1000) crow      (1000)      103 2023-05-29 11:54:13.110935 ditty-0.3.1/setup.cfg
+-rw-rw-r--   0 crow      (1000) crow      (1000)      639 2023-05-29 11:53:59.000000 ditty-0.3.1/setup.py
```

### Comparing `ditty-0.3.0/LICENSE` & `ditty-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ditty-0.3.0/PKG-INFO` & `ditty-0.3.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,30 @@
-Metadata-Version: 2.1
-Name: ditty
-Version: 0.3.0
-Home-page: https://github.com/iantbutler01/ditty
-Author: Ian T Butler (KinglyCrow)
-Author-email: iantbutler01@gmail.com
-License: Apache V2
-Keywords: finetuning,llm,nlp,machine learning
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Ditty
 
 A simple fine-tune.
 
 ## What
 A very simple library for finetuning Huggingface Pretrained AutoModelForCausalLM such as GPTNeoX, leveraging Huggingface Accelerate, Transformers, Datasets and Peft
 
 Ditty has support for LORA, 8bit, and fp32 cpu offloading right out of the box and assumes you are running with a single GPU or distributed over multiple GPUs by default.
 
+Checkpointing supported, currently a bug with pushing to HF model hub though so checkpoints are all local.
+
+FP16, BFLOAT16 now supported.
+
+QLORA 4bit supported under experimental, and requires installing development branches of accelerate, peft, transformers and the latest bitsandbytes.
+
+
 ## What Not
 - Ditty does not support ASICs like TPU or Trainium.
 - Ditty does not handle Sagemaker
 - Ditty does not by default run with the CPU
 - Ditty does not handle evaluation sets or benchmarking, this may or may not change.
 
 ## Soon
-- Ditty will handle FP16
 - Ditty may handle distributed cluster finetuning
 - Ditty will support DeepSpeed
 
 ## Classes
 
 ### Pipeline
```

### Comparing `ditty-0.3.0/README.md` & `ditty-0.3.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,41 @@
+Metadata-Version: 2.1
+Name: ditty
+Version: 0.3.1
+Home-page: https://github.com/iantbutler01/ditty
+Author: Ian T Butler (KinglyCrow)
+Author-email: iantbutler01@gmail.com
+License: Apache V2
+Keywords: finetuning,llm,nlp,machine learning
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Ditty
 
 A simple fine-tune.
 
 ## What
 A very simple library for finetuning Huggingface Pretrained AutoModelForCausalLM such as GPTNeoX, leveraging Huggingface Accelerate, Transformers, Datasets and Peft
 
 Ditty has support for LORA, 8bit, and fp32 cpu offloading right out of the box and assumes you are running with a single GPU or distributed over multiple GPUs by default.
 
+Checkpointing supported, currently a bug with pushing to HF model hub though so checkpoints are all local.
+
+FP16, BFLOAT16 now supported.
+
+QLORA 4bit supported under experimental, and requires installing development branches of accelerate, peft, transformers and the latest bitsandbytes.
+
+
 ## What Not
 - Ditty does not support ASICs like TPU or Trainium.
 - Ditty does not handle Sagemaker
 - Ditty does not by default run with the CPU
 - Ditty does not handle evaluation sets or benchmarking, this may or may not change.
 
 ## Soon
-- Ditty will handle FP16
 - Ditty may handle distributed cluster finetuning
 - Ditty will support DeepSpeed
 
 ## Classes
 
 ### Pipeline
 
@@ -76,8 +93,8 @@
 
 Portions of this library look to Huggingface's transformers Trainer class as a reference and in some cases re-implements functions from Trainer, simplified to only account for GPU based work and overall narrower supported scope.
 
 This statement is both to fulfill the obligations of the ApacheV2 licencse, but also because those folks do super cool work and I appreciate all they've done for the community and its just right to call this out.
 
 ## License
 
-Apache V2 see the LICENSE file for full text.
+Apache V2 see the LICENSE file for full text.
```

### Comparing `ditty-0.3.0/lib/ditty/data.py` & `ditty-0.3.1/lib/ditty/data.py`

 * *Files identical despite different names*

### Comparing `ditty-0.3.0/lib/ditty/pipeline.py` & `ditty-0.3.1/lib/ditty/pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,17 @@
             )
         elif self.l4bit and not experimental:
             raise ValueError("To use 4bit, `experimental` must be set to True.")
         elif self.l8bit:
             self.bnb_config = BitsAndBytesConfig(
                 load_in_8bit=l8bit, llm_int8_enable_fp32_cpu_offload=fp32_cpu_offload
             )
+        else:
+            self.bnb_config = None
+
         self.checkpoint_every = checkpoint_every
         self.load_checkpoint = load_checkpoint
         self.gradient_checkpointing = gradient_checkpointing
 
     def dataset(self) -> DataLoader:
         """
         Subclass Pipeline and customize for your own dataset.
```

### Comparing `ditty-0.3.0/lib/ditty/trainer.py` & `ditty-0.3.1/lib/ditty/trainer.py`

 * *Files identical despite different names*

### Comparing `ditty-0.3.0/lib/ditty.egg-info/PKG-INFO` & `ditty-0.3.1/lib/ditty.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.3.0
+Version: 0.3.1
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -14,22 +14,28 @@
 A simple fine-tune.
 
 ## What
 A very simple library for finetuning Huggingface Pretrained AutoModelForCausalLM such as GPTNeoX, leveraging Huggingface Accelerate, Transformers, Datasets and Peft
 
 Ditty has support for LORA, 8bit, and fp32 cpu offloading right out of the box and assumes you are running with a single GPU or distributed over multiple GPUs by default.
 
+Checkpointing supported, currently a bug with pushing to HF model hub though so checkpoints are all local.
+
+FP16, BFLOAT16 now supported.
+
+QLORA 4bit supported under experimental, and requires installing development branches of accelerate, peft, transformers and the latest bitsandbytes.
+
+
 ## What Not
 - Ditty does not support ASICs like TPU or Trainium.
 - Ditty does not handle Sagemaker
 - Ditty does not by default run with the CPU
 - Ditty does not handle evaluation sets or benchmarking, this may or may not change.
 
 ## Soon
-- Ditty will handle FP16
 - Ditty may handle distributed cluster finetuning
 - Ditty will support DeepSpeed
 
 ## Classes
 
 ### Pipeline
```

### Comparing `ditty-0.3.0/setup.py` & `ditty-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ditty',
-    version='0.3.0',
+    version='0.3.1',
     license='Apache V2',
     author="Ian T Butler (KinglyCrow)",
     author_email='iantbutler01@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```


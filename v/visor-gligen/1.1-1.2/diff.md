# Comparing `tmp/visor_gligen-1.1.tar.gz` & `tmp/visor_gligen-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/visor_gligen-1.1.tar", last modified: Sun May 28 18:55:54 2023, max compression
+gzip compressed data, was "dist/visor_gligen-1.2.tar", last modified: Mon May 29 05:20:27 2023, max compression
```

## Comparing `visor_gligen-1.1.tar` & `visor_gligen-1.2.tar`

### file list

```diff
@@ -1,36 +1,43 @@
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-28 18:55:54.834261 visor_gligen-1.1/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       94 2023-05-28 18:55:54.834261 visor_gligen-1.1/PKG-INFO
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6697 2023-05-28 18:35:53.000000 visor_gligen-1.1/README.md
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       38 2023-05-28 18:55:54.834261 visor_gligen-1.1/setup.cfg
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)      338 2023-05-28 18:54:43.000000 visor_gligen-1.1/setup.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-28 18:55:54.834261 visor_gligen-1.1/visor_gligen/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    36555 2023-05-28 18:35:53.000000 visor_gligen-1.1/visor_gligen/gligen_inference_box.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6039 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/inpaint_mask_func.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-28 18:55:54.834261 visor_gligen-1.1/visor_gligen/ldm/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/ldm/__init__.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-28 18:55:54.834261 visor_gligen-1.1/visor_gligen/ldm/models/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/ldm/models/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     1364 2023-05-28 18:35:53.000000 visor_gligen-1.1/visor_gligen/ldm/models/autoencoder.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-28 18:55:54.834261 visor_gligen-1.1/visor_gligen/ldm/modules/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/ldm/modules/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    10821 2023-05-28 18:35:53.000000 visor_gligen-1.1/visor_gligen/ldm/modules/attention.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2982 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/ldm/modules/ema.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-28 18:55:54.834261 visor_gligen-1.1/visor_gligen/ldm/modules/image_degradation/
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)      234 2023-05-28 18:35:53.000000 visor_gligen-1.1/visor_gligen/ldm/modules/image_degradation/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    25198 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/ldm/modules/image_degradation/bsrgan.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    22238 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/ldm/modules/image_degradation/bsrgan_light.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    29024 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/ldm/modules/image_degradation/utils_image.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-28 18:55:54.834261 visor_gligen-1.1/visor_gligen/ldm/modules/losses/
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)       81 2023-05-28 18:35:53.000000 visor_gligen-1.1/visor_gligen/ldm/modules/losses/__init__.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     5581 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/ldm/modules/losses/contperceptual.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     7941 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/ldm/modules/losses/vqperceptual.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    20168 2023-04-16 05:30:27.000000 visor_gligen-1.1/visor_gligen/ldm/modules/x_transformer.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2517 2023-05-28 18:35:53.000000 visor_gligen-1.1/visor_gligen/ldm/util.py
--rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    19659 2023-05-28 18:35:53.000000 visor_gligen-1.1/visor_gligen/trainer.py
-drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-28 18:55:54.834261 visor_gligen-1.1/visor_gligen.egg-info/
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       94 2023-05-28 18:55:54.000000 visor_gligen-1.1/visor_gligen.egg-info/PKG-INFO
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)      962 2023-05-28 18:55:54.000000 visor_gligen-1.1/visor_gligen.egg-info/SOURCES.txt
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        1 2023-05-28 18:55:54.000000 visor_gligen-1.1/visor_gligen.egg-info/dependency_links.txt
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       92 2023-05-28 18:55:54.000000 visor_gligen-1.1/visor_gligen.egg-info/requires.txt
--rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       13 2023-05-28 18:55:54.000000 visor_gligen-1.1/visor_gligen.egg-info/top_level.txt
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:20:27.777928 visor_gligen-1.2/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       94 2023-05-29 05:20:27.773928 visor_gligen-1.2/PKG-INFO
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6697 2023-05-28 18:35:53.000000 visor_gligen-1.2/README.md
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       38 2023-05-29 05:20:27.777928 visor_gligen-1.2/setup.cfg
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)      338 2023-05-29 05:20:05.000000 visor_gligen-1.2/setup.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:20:27.773928 visor_gligen-1.2/visor_gligen/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    36555 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/gligen_inference_box.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6039 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/inpaint_mask_func.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:20:27.773928 visor_gligen-1.2/visor_gligen/ldm/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/ldm/__init__.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:20:27.773928 visor_gligen-1.2/visor_gligen/ldm/models/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/ldm/models/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     1364 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/ldm/models/autoencoder.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:20:27.773928 visor_gligen-1.2/visor_gligen/ldm/models/diffusion/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:18:26.000000 visor_gligen-1.2/visor_gligen/ldm/models/diffusion/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    10302 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/ldm/models/diffusion/classifier.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     6100 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/ldm/models/diffusion/ddim.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2859 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/ldm/models/diffusion/ddpm.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     3155 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/ldm/models/diffusion/ldm.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     7552 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/ldm/models/diffusion/plms.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:20:27.773928 visor_gligen-1.2/visor_gligen/ldm/modules/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/ldm/modules/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    10821 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/ldm/modules/attention.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2982 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/ldm/modules/ema.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:20:27.773928 visor_gligen-1.2/visor_gligen/ldm/modules/image_degradation/
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)      234 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/ldm/modules/image_degradation/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    25198 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/ldm/modules/image_degradation/bsrgan.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    22238 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/ldm/modules/image_degradation/bsrgan_light.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    29024 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/ldm/modules/image_degradation/utils_image.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:20:27.773928 visor_gligen-1.2/visor_gligen/ldm/modules/losses/
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)       81 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/ldm/modules/losses/__init__.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     5581 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/ldm/modules/losses/contperceptual.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     7941 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/ldm/modules/losses/vqperceptual.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    20168 2023-04-16 05:30:27.000000 visor_gligen-1.2/visor_gligen/ldm/modules/x_transformer.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)     2517 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/ldm/util.py
+-rw-r--r--   0 cvi_demo  (1122) cvi_demo  (1122)    19659 2023-05-28 18:35:53.000000 visor_gligen-1.2/visor_gligen/trainer.py
+drwxrwxr-x   0 cvi_demo  (1122) cvi_demo  (1122)        0 2023-05-29 05:20:27.773928 visor_gligen-1.2/visor_gligen.egg-info/
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       94 2023-05-29 05:20:27.000000 visor_gligen-1.2/visor_gligen.egg-info/PKG-INFO
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)     1223 2023-05-29 05:20:27.000000 visor_gligen-1.2/visor_gligen.egg-info/SOURCES.txt
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)        1 2023-05-29 05:20:27.000000 visor_gligen-1.2/visor_gligen.egg-info/dependency_links.txt
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       92 2023-05-29 05:20:27.000000 visor_gligen-1.2/visor_gligen.egg-info/requires.txt
+-rw-rw-r--   0 cvi_demo  (1122) cvi_demo  (1122)       13 2023-05-29 05:20:27.000000 visor_gligen-1.2/visor_gligen.egg-info/top_level.txt
```

### Comparing `visor_gligen-1.1/README.md` & `visor_gligen-1.2/README.md`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/gligen_inference_box.py` & `visor_gligen-1.2/visor_gligen/gligen_inference_box.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/inpaint_mask_func.py` & `visor_gligen-1.2/visor_gligen/inpaint_mask_func.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/ldm/models/autoencoder.py` & `visor_gligen-1.2/visor_gligen/ldm/models/autoencoder.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/ldm/modules/attention.py` & `visor_gligen-1.2/visor_gligen/ldm/modules/attention.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/ldm/modules/ema.py` & `visor_gligen-1.2/visor_gligen/ldm/modules/ema.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/ldm/modules/image_degradation/bsrgan.py` & `visor_gligen-1.2/visor_gligen/ldm/modules/image_degradation/bsrgan.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/ldm/modules/image_degradation/bsrgan_light.py` & `visor_gligen-1.2/visor_gligen/ldm/modules/image_degradation/bsrgan_light.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/ldm/modules/image_degradation/utils_image.py` & `visor_gligen-1.2/visor_gligen/ldm/modules/image_degradation/utils_image.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/ldm/modules/losses/contperceptual.py` & `visor_gligen-1.2/visor_gligen/ldm/modules/losses/contperceptual.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/ldm/modules/losses/vqperceptual.py` & `visor_gligen-1.2/visor_gligen/ldm/modules/losses/vqperceptual.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/ldm/modules/x_transformer.py` & `visor_gligen-1.2/visor_gligen/ldm/modules/x_transformer.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/ldm/util.py` & `visor_gligen-1.2/visor_gligen/ldm/util.py`

 * *Files identical despite different names*

### Comparing `visor_gligen-1.1/visor_gligen/trainer.py` & `visor_gligen-1.2/visor_gligen/trainer.py`

 * *Files identical despite different names*


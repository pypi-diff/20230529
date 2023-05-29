# Comparing `tmp/draggan-1.1.0b1.tar.gz` & `tmp/draggan-1.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-fxfe41i8/draggan-1.1.0b1.tar", last modified: Sun May 28 15:16:35 2023, max compression
+gzip compressed data, was "/media/exthdd/laizeqiang/lzq/projects/generated_model/DragGAN/dist/.tmp-icj4gqjm/draggan-1.1.0b2.tar", last modified: Mon May 29 12:57:49 2023, max compression
```

## Comparing `draggan-1.1.0b1.tar` & `draggan-1.1.0b2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       53 2023-05-28 15:16:35.000000 draggan-1.1.0b1/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5960 2023-05-28 15:08:51.000000 draggan-1.1.0b1/README.md
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       44 2023-05-28 12:23:03.000000 draggan-1.1.0b1/draggan/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7733 2023-05-28 13:06:42.000000 draggan-1.1.0b1/draggan/api.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan/stylegan2/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/__init__.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/inversion.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/base_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/dist_model.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/networks_basic.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/pretrained_networks.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.1.0b1/draggan/stylegan2/lpips/util.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19711 2023-05-28 02:36:05.000000 draggan-1.1.0b1/draggan/stylegan2/model.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan/stylegan2/op/
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.1.0b1/draggan/stylegan2/op/__init__.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.1.0b1/draggan/stylegan2/op/conv2d_gradfix.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4282 2023-05-26 01:18:57.000000 draggan-1.1.0b1/draggan/stylegan2/op/fused_act.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.1.0b1/draggan/stylegan2/op/fused_bias_act.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.1.0b1/draggan/stylegan2/op/fused_bias_act_kernel.cu
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d.cpp
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6679 2023-05-26 01:19:03.000000 draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d.py
--rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d_kernel.cu
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7296 2023-05-28 14:55:40.000000 draggan-1.1.0b1/draggan/utils.py
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11723 2023-05-28 13:54:13.000000 draggan-1.1.0b1/draggan/web.py
-drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       53 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/PKG-INFO
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      862 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/SOURCES.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/dependency_links.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/requires.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        8 2023-05-28 15:16:35.000000 draggan-1.1.0b1/draggan.egg-info/top_level.txt
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-28 15:16:35.000000 draggan-1.1.0b1/setup.cfg
--rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      618 2023-05-28 15:16:28.000000 draggan-1.1.0b1/setup.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       53 2023-05-29 12:57:49.000000 draggan-1.1.0b2/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5960 2023-05-28 15:08:51.000000 draggan-1.1.0b2/README.md
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       44 2023-05-28 12:23:03.000000 draggan-1.1.0b2/draggan/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7733 2023-05-29 12:57:30.000000 draggan-1.1.0b2/draggan/api.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan/stylegan2/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/__init__.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5029 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/inversion.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      111 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1618 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/base_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12782 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/dist_model.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     7482 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/networks_basic.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6533 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/pretrained_networks.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     5699 2023-05-25 06:58:32.000000 draggan-1.1.0b2/draggan/stylegan2/lpips/util.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    19711 2023-05-28 02:36:05.000000 draggan-1.1.0b2/draggan/stylegan2/model.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan/stylegan2/op/
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)      155 2023-05-25 07:09:27.000000 draggan-1.1.0b2/draggan/stylegan2/op/__init__.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6626 2023-05-25 07:16:40.000000 draggan-1.1.0b2/draggan/stylegan2/op/conv2d_gradfix.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     4282 2023-05-26 01:18:57.000000 draggan-1.1.0b2/draggan/stylegan2/op/fused_act.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1333 2023-05-25 06:58:33.000000 draggan-1.1.0b2/draggan/stylegan2/op/fused_bias_act.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     2828 2023-05-25 06:58:33.000000 draggan-1.1.0b2/draggan/stylegan2/op/fused_bias_act_kernel.cu
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     1343 2023-05-25 06:58:33.000000 draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d.cpp
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)     6679 2023-05-26 01:19:03.000000 draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d.py
+-rwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)    12070 2023-05-25 06:58:33.000000 draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d_kernel.cu
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)     7296 2023-05-28 14:55:40.000000 draggan-1.1.0b2/draggan/utils.py
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)    11723 2023-05-28 13:54:13.000000 draggan-1.1.0b2/draggan/web.py
+drwxrwxr-x   0 laizeqiang  (1000) laizeqiang  (1000)        0 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       53 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/PKG-INFO
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      862 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/SOURCES.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        1 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/dependency_links.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      104 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/requires.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)        8 2023-05-29 12:57:49.000000 draggan-1.1.0b2/draggan.egg-info/top_level.txt
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)       38 2023-05-29 12:57:49.000000 draggan-1.1.0b2/setup.cfg
+-rw-rw-r--   0 laizeqiang  (1000) laizeqiang  (1000)      618 2023-05-29 12:57:40.000000 draggan-1.1.0b2/setup.py
```

### Comparing `draggan-1.1.0b1/README.md` & `draggan-1.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/api.py` & `draggan-1.1.0b2/draggan/api.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/inversion.py` & `draggan-1.1.0b2/draggan/stylegan2/inversion.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/lpips/base_model.py` & `draggan-1.1.0b2/draggan/stylegan2/lpips/base_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/lpips/dist_model.py` & `draggan-1.1.0b2/draggan/stylegan2/lpips/dist_model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/lpips/networks_basic.py` & `draggan-1.1.0b2/draggan/stylegan2/lpips/networks_basic.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/lpips/pretrained_networks.py` & `draggan-1.1.0b2/draggan/stylegan2/lpips/pretrained_networks.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/lpips/util.py` & `draggan-1.1.0b2/draggan/stylegan2/lpips/util.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/model.py` & `draggan-1.1.0b2/draggan/stylegan2/model.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/op/conv2d_gradfix.py` & `draggan-1.1.0b2/draggan/stylegan2/op/conv2d_gradfix.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/op/fused_act.py` & `draggan-1.1.0b2/draggan/stylegan2/op/fused_act.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/op/fused_bias_act.cpp` & `draggan-1.1.0b2/draggan/stylegan2/op/fused_bias_act.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/op/fused_bias_act_kernel.cu` & `draggan-1.1.0b2/draggan/stylegan2/op/fused_bias_act_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d.cpp` & `draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d.cpp`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d.py` & `draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/stylegan2/op/upfirdn2d_kernel.cu` & `draggan-1.1.0b2/draggan/stylegan2/op/upfirdn2d_kernel.cu`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/utils.py` & `draggan-1.1.0b2/draggan/utils.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan/web.py` & `draggan-1.1.0b2/draggan/web.py`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/draggan.egg-info/SOURCES.txt` & `draggan-1.1.0b2/draggan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `draggan-1.1.0b1/setup.py` & `draggan-1.1.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='draggan',
     packages=['draggan'],
-    version='1.1.0b1',
+    version='1.1.0b2',
     package_data={
         'draggan': ['stylegan2/op/fused_bias_act.cpp', 'stylegan2/op/upfirdn2d.cpp',
                     'stylegan2/op/fused_bias_act_kernel.cu', 'stylegan2/op/upfirdn2d_kernel.cu'], 
     },
     include_package_data=True,
     install_requires=[
         'gradio==3.28.1',
```


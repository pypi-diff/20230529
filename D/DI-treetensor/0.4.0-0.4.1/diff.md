# Comparing `tmp/DI-treetensor-0.4.0.tar.gz` & `tmp/DI-treetensor-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DI-treetensor-0.4.0.tar", last modified: Sun Aug 14 06:11:25 2022, max compression
+gzip compressed data, was "DI-treetensor-0.4.1.tar", last modified: Mon May 29 08:30:13 2023, max compression
```

## Comparing `DI-treetensor-0.4.0.tar` & `DI-treetensor-0.4.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:11:25.668876 DI-treetensor-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:11:25.664876 DI-treetensor-0.4.0/DI_treetensor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9264 2022-08-14 06:11:25.000000 DI-treetensor-0.4.0/DI_treetensor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-08-14 06:11:25.000000 DI-treetensor-0.4.0/DI_treetensor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-14 06:11:25.000000 DI-treetensor-0.4.0/DI_treetensor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      526 2022-08-14 06:11:25.000000 DI-treetensor-0.4.0/DI_treetensor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-08-14 06:11:25.000000 DI-treetensor-0.4.0/DI_treetensor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     9264 2022-08-14 06:11:25.668876 DI-treetensor-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8263 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-14 06:11:25.668876 DI-treetensor-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2019 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:11:25.664876 DI-treetensor-0.4.0/treetensor/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:11:25.664876 DI-treetensor-0.4.0/treetensor/common/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1415 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/common/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     1944 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/common/object.py
--rw-r--r--   0 runner    (1001) docker     (121)     2044 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/common/proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3366 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/common/trees.py
--rw-r--r--   0 runner    (1001) docker     (121)      715 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/common/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:11:25.664876 DI-treetensor-0.4.0/treetensor/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      484 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:11:25.664876 DI-treetensor-0.4.0/treetensor/numpy/
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/numpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3697 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/numpy/array.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/numpy/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2608 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/numpy/funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:11:25.664876 DI-treetensor-0.4.0/treetensor/torch/
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:11:25.668876 DI-treetensor-0.4.0/treetensor/torch/base/
--rw-r--r--   0 runner    (1001) docker     (121)      177 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2433 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/base/reduce.py
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/base/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:11:25.668876 DI-treetensor-0.4.0/treetensor/torch/funcs/
--rw-r--r--   0 runner    (1001) docker     (121)      833 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2807 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/funcs/autograd.py
--rw-r--r--   0 runner    (1001) docker     (121)      615 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/funcs/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    11853 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/funcs/comparison.py
--rw-r--r--   0 runner    (1001) docker     (121)    13796 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/funcs/construct.py
--rw-r--r--   0 runner    (1001) docker     (121)    36876 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/funcs/math.py
--rw-r--r--   0 runner    (1001) docker     (121)     3294 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/funcs/matrix.py
--rw-r--r--   0 runner    (1001) docker     (121)    21068 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/funcs/operation.py
--rw-r--r--   0 runner    (1001) docker     (121)    14810 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/funcs/reduction.py
--rw-r--r--   0 runner    (1001) docker     (121)     4171 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/size.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/stream.py
--rw-r--r--   0 runner    (1001) docker     (121)    31110 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/torch/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-14 06:11:25.668876 DI-treetensor-0.4.0/treetensor/utils/
--rw-r--r--   0 runner    (1001) docker     (121)       86 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2421 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/utils/clazz.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/utils/doc.py
--rw-r--r--   0 runner    (1001) docker     (121)      691 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/utils/func.py
--rw-r--r--   0 runner    (1001) docker     (121)     2240 2022-08-14 06:10:20.000000 DI-treetensor-0.4.0/treetensor/utils/reflection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:30:13.010209 DI-treetensor-0.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:30:12.994209 DI-treetensor-0.4.1/DI_treetensor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-05-29 08:30:12.000000 DI-treetensor-0.4.1/DI_treetensor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-29 08:30:12.000000 DI-treetensor-0.4.1/DI_treetensor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 08:30:12.000000 DI-treetensor-0.4.1/DI_treetensor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-29 08:30:12.000000 DI-treetensor-0.4.1/DI_treetensor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 08:30:12.000000 DI-treetensor-0.4.1/DI_treetensor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9264 2023-05-29 08:30:13.010209 DI-treetensor-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8263 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 08:30:13.010209 DI-treetensor-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:30:12.994209 DI-treetensor-0.4.1/treetensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:30:12.998209 DI-treetensor-0.4.1/treetensor/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/common/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/common/object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/common/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/common/trees.py
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/common/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:30:12.998209 DI-treetensor-0.4.1/treetensor/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:30:12.998209 DI-treetensor-0.4.1/treetensor/numpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/numpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/numpy/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/numpy/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/numpy/funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:30:13.002209 DI-treetensor-0.4.1/treetensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:30:13.002209 DI-treetensor-0.4.1/treetensor/torch/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/base/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/base/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:30:13.006209 DI-treetensor-0.4.1/treetensor/torch/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      833 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/funcs/autograd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/funcs/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11853 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/funcs/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13796 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/funcs/construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36876 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/funcs/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/funcs/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/funcs/operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14810 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/funcs/reduction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31110 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/torch/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 08:30:13.010209 DI-treetensor-0.4.1/treetensor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/utils/clazz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/utils/doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/utils/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-05-29 08:27:27.000000 DI-treetensor-0.4.1/treetensor/utils/reflection.py
```

### Comparing `DI-treetensor-0.4.0/DI_treetensor.egg-info/PKG-INFO` & `DI-treetensor-0.4.1/DI_treetensor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DI-treetensor
-Version: 0.4.0
+Version: 0.4.1
 Summary: A flexible, generalized tree-based tensor structure.
 Home-page: https://github.com/opendilab/DI-treetensor
 Author: HansBug, DI-engine's Contributors
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: Tree-structured Value Management
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DI-treetensor Version: 0.4.0 Summary: A flexible,
+Metadata-Version: 2.1 Name: DI-treetensor Version: 0.4.1 Summary: A flexible,
 generalized tree-based tensor structure. Home-page: https://github.com/
 opendilab/DI-treetensor Author: HansBug, DI-engine's Contributors Author-email:
 hansbug@buaa.edu.cn License: Apache License, Version 2.0 Keywords: Tree-
 structured Value Management Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `DI-treetensor-0.4.0/DI_treetensor.egg-info/SOURCES.txt` & `DI-treetensor-0.4.1/DI_treetensor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/DI_treetensor.egg-info/requires.txt` & `DI-treetensor-0.4.1/DI_treetensor.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-treevalue>=1.4.1
-torch<=1.12.1,>=1.1.0
+treevalue>=1.4.11
+torch>=1.1.0
 hbutils>=0.6.13
 numpy
 
 [doc]
 Jinja2~=3.0.0
 sphinx~=3.2.0
 sphinx_rtd_theme~=0.4.3
```

### Comparing `DI-treetensor-0.4.0/LICENSE` & `DI-treetensor-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/PKG-INFO` & `DI-treetensor-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DI-treetensor
-Version: 0.4.0
+Version: 0.4.1
 Summary: A flexible, generalized tree-based tensor structure.
 Home-page: https://github.com/opendilab/DI-treetensor
 Author: HansBug, DI-engine's Contributors
 Author-email: hansbug@buaa.edu.cn
 License: Apache License, Version 2.0
 Keywords: Tree-structured Value Management
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: DI-treetensor Version: 0.4.0 Summary: A flexible,
+Metadata-Version: 2.1 Name: DI-treetensor Version: 0.4.1 Summary: A flexible,
 generalized tree-based tensor structure. Home-page: https://github.com/
 opendilab/DI-treetensor Author: HansBug, DI-engine's Contributors Author-email:
 hansbug@buaa.edu.cn License: Apache License, Version 2.0 Keywords: Tree-
 structured Value Management Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

### Comparing `DI-treetensor-0.4.0/README.md` & `DI-treetensor-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/setup.py` & `DI-treetensor-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/common/module.py` & `DI-treetensor-0.4.1/treetensor/common/module.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/common/object.py` & `DI-treetensor-0.4.1/treetensor/common/object.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/common/proxy.py` & `DI-treetensor-0.4.1/treetensor/common/proxy.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/common/trees.py` & `DI-treetensor-0.4.1/treetensor/common/trees.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/common/wrappers.py` & `DI-treetensor-0.4.1/treetensor/common/wrappers.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/numpy/__init__.py` & `DI-treetensor-0.4.1/treetensor/numpy/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/numpy/array.py` & `DI-treetensor-0.4.1/treetensor/numpy/array.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/numpy/funcs.py` & `DI-treetensor-0.4.1/treetensor/numpy/funcs.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/__init__.py` & `DI-treetensor-0.4.1/treetensor/torch/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/base/reduce.py` & `DI-treetensor-0.4.1/treetensor/torch/base/reduce.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/funcs/__init__.py` & `DI-treetensor-0.4.1/treetensor/torch/funcs/__init__.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/funcs/autograd.py` & `DI-treetensor-0.4.1/treetensor/torch/funcs/autograd.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/funcs/base.py` & `DI-treetensor-0.4.1/treetensor/torch/funcs/base.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/funcs/comparison.py` & `DI-treetensor-0.4.1/treetensor/torch/funcs/comparison.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/funcs/construct.py` & `DI-treetensor-0.4.1/treetensor/torch/funcs/construct.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/funcs/math.py` & `DI-treetensor-0.4.1/treetensor/torch/funcs/math.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/funcs/matrix.py` & `DI-treetensor-0.4.1/treetensor/torch/funcs/matrix.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/funcs/operation.py` & `DI-treetensor-0.4.1/treetensor/torch/funcs/operation.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/funcs/reduction.py` & `DI-treetensor-0.4.1/treetensor/torch/funcs/reduction.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/size.py` & `DI-treetensor-0.4.1/treetensor/torch/size.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/stream.py` & `DI-treetensor-0.4.1/treetensor/torch/stream.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/torch/tensor.py` & `DI-treetensor-0.4.1/treetensor/torch/tensor.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/utils/clazz.py` & `DI-treetensor-0.4.1/treetensor/utils/clazz.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/utils/doc.py` & `DI-treetensor-0.4.1/treetensor/utils/doc.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/utils/func.py` & `DI-treetensor-0.4.1/treetensor/utils/func.py`

 * *Files identical despite different names*

### Comparing `DI-treetensor-0.4.0/treetensor/utils/reflection.py` & `DI-treetensor-0.4.1/treetensor/utils/reflection.py`

 * *Files identical despite different names*


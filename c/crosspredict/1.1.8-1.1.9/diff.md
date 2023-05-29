# Comparing `tmp/crosspredict-1.1.8.tar.gz` & `tmp/crosspredict-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosspredict-1.1.8.tar", last modified: Thu May 25 11:28:22 2023, max compression
+gzip compressed data, was "crosspredict-1.1.9.tar", last modified: Mon May 29 13:21:36 2023, max compression
```

## Comparing `crosspredict-1.1.8.tar` & `crosspredict-1.1.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.439760 crosspredict-1.1.8/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1074 2022-09-26 07:29:13.000000 crosspredict-1.1.8/LICENSE
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       58 2022-09-26 07:29:13.000000 crosspredict-1.1.8/MANIFEST.in
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2023-05-25 11:28:22.438939 crosspredict-1.1.8/PKG-INFO
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     5151 2022-09-26 07:59:16.000000 crosspredict-1.1.8/README.md
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:21.688412 crosspredict-1.1.8/crosspredict/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       44 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/__init__.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:21.691027 crosspredict-1.1.8/crosspredict/__pycache__/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      206 2022-09-26 08:25:52.000000 crosspredict-1.1.8/crosspredict/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     4094 2022-09-26 08:26:01.000000 crosspredict-1.1.8/crosspredict/__pycache__/iterator.cpython-39.pyc
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.383877 crosspredict-1.1.8/crosspredict/crossval/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      241 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/crossval/__init__.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.387813 crosspredict-1.1.8/crosspredict/crossval/__pycache__/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      380 2022-09-26 08:25:52.000000 crosspredict-1.1.8/crosspredict/crossval/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3213 2022-09-26 08:26:02.000000 crosspredict-1.1.8/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     7886 2023-05-25 11:27:14.000000 crosspredict-1.1.8/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2885 2022-09-26 08:57:16.000000 crosspredict-1.1.8/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1763 2022-09-26 08:26:01.000000 crosspredict-1.1.8/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3869 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/crossval/_catboost.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)    11738 2023-05-25 11:26:23.000000 crosspredict-1.1.8/crosspredict/crossval/_crossval.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3848 2022-09-26 08:57:01.000000 crosspredict-1.1.8/crosspredict/crossval/_lightgbm.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2331 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/crossval/_xgboost.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     4965 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/iterator.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.388913 crosspredict-1.1.8/crosspredict/nodes/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      215 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/nodes/__init__.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)    12522 2023-04-13 13:11:46.000000 crosspredict-1.1.8/crosspredict/nodes/_nodes.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1580 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/parameters.yml
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.435022 crosspredict-1.1.8/crosspredict/report_binary/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      138 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/report_binary/__init__.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.436123 crosspredict-1.1.8/crosspredict/report_binary/__pycache__/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      323 2022-09-26 08:27:01.000000 crosspredict-1.1.8/crosspredict/report_binary/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     8606 2023-05-25 10:01:03.000000 crosspredict-1.1.8/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     9111 2022-09-26 08:27:01.000000 crosspredict-1.1.8/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     7896 2023-04-13 13:11:46.000000 crosspredict-1.1.8/crosspredict/report_binary/_curves.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)    12423 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/report_binary/_report_binary.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.436968 crosspredict-1.1.8/crosspredict/target_encoder/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      174 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/target_encoder/__init__.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2836 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/target_encoder/_crosstargetencoder.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     3471 2022-09-26 07:29:13.000000 crosspredict-1.1.8/crosspredict/target_encoder/_target_encoder.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:21.690551 crosspredict-1.1.8/crosspredict.egg-info/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2023-05-25 11:28:21.000000 crosspredict-1.1.8/crosspredict.egg-info/PKG-INFO
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1470 2023-05-25 11:28:21.000000 crosspredict-1.1.8/crosspredict.egg-info/SOURCES.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)        1 2023-05-25 11:28:21.000000 crosspredict-1.1.8/crosspredict.egg-info/dependency_links.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      247 2023-05-25 11:28:21.000000 crosspredict-1.1.8/crosspredict.egg-info/requires.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       19 2023-05-25 11:28:21.000000 crosspredict-1.1.8/crosspredict.egg-info/top_level.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      246 2022-09-26 08:59:16.000000 crosspredict-1.1.8/requirements.txt
--rw-r--r--   0 vboyadzhi   (503) staff       (20)       38 2023-05-25 11:28:22.439974 crosspredict-1.1.8/setup.cfg
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     1272 2023-05-25 11:28:06.000000 crosspredict-1.1.8/setup.py
-drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-25 11:28:22.437784 crosspredict-1.1.8/tests/
--rw-r--r--   0 vboyadzhi   (503) staff       (20)        0 2022-09-26 07:29:13.000000 crosspredict-1.1.8/tests/__init__.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)      556 2022-09-26 07:29:13.000000 crosspredict-1.1.8/tests/conftest.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     7765 2022-09-26 08:47:46.000000 crosspredict-1.1.8/tests/test_binary.py
--rw-r--r--   0 vboyadzhi   (503) staff       (20)     2518 2022-09-26 07:29:13.000000 crosspredict-1.1.8/tests/test_iterator.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:36.105675 crosspredict-1.1.9/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1074 2022-09-26 07:29:13.000000 crosspredict-1.1.9/LICENSE
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       58 2022-09-26 07:29:13.000000 crosspredict-1.1.9/MANIFEST.in
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2023-05-29 13:21:36.105487 crosspredict-1.1.9/PKG-INFO
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     5151 2022-09-26 07:59:16.000000 crosspredict-1.1.9/README.md
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:35.687202 crosspredict-1.1.9/crosspredict/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       44 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/__init__.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:35.689494 crosspredict-1.1.9/crosspredict/__pycache__/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      206 2022-09-26 08:25:52.000000 crosspredict-1.1.9/crosspredict/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     4094 2022-09-26 08:26:01.000000 crosspredict-1.1.9/crosspredict/__pycache__/iterator.cpython-39.pyc
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:35.964719 crosspredict-1.1.9/crosspredict/crossval/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      241 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/crossval/__init__.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:35.966073 crosspredict-1.1.9/crosspredict/crossval/__pycache__/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      380 2022-09-26 08:25:52.000000 crosspredict-1.1.9/crosspredict/crossval/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3213 2022-09-26 08:26:02.000000 crosspredict-1.1.9/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     7886 2023-05-25 11:27:14.000000 crosspredict-1.1.9/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2885 2022-09-26 08:57:16.000000 crosspredict-1.1.9/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1763 2022-09-26 08:26:01.000000 crosspredict-1.1.9/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3869 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/crossval/_catboost.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)    12135 2023-05-29 13:21:28.000000 crosspredict-1.1.9/crosspredict/crossval/_crossval.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3984 2023-05-29 13:21:28.000000 crosspredict-1.1.9/crosspredict/crossval/_lightgbm.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2331 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/crossval/_xgboost.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     4965 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/iterator.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:36.054649 crosspredict-1.1.9/crosspredict/nodes/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      215 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/nodes/__init__.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)    12522 2023-04-13 13:11:46.000000 crosspredict-1.1.9/crosspredict/nodes/_nodes.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1580 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/parameters.yml
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:36.055668 crosspredict-1.1.9/crosspredict/report_binary/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      138 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/report_binary/__init__.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:36.056425 crosspredict-1.1.9/crosspredict/report_binary/__pycache__/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      323 2022-09-26 08:27:01.000000 crosspredict-1.1.9/crosspredict/report_binary/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     8606 2023-05-25 10:01:03.000000 crosspredict-1.1.9/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     9111 2022-09-26 08:27:01.000000 crosspredict-1.1.9/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     7896 2023-04-13 13:11:46.000000 crosspredict-1.1.9/crosspredict/report_binary/_curves.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)    12423 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/report_binary/_report_binary.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:36.104035 crosspredict-1.1.9/crosspredict/target_encoder/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      174 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/target_encoder/__init__.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2836 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/target_encoder/_crosstargetencoder.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     3471 2022-09-26 07:29:13.000000 crosspredict-1.1.9/crosspredict/target_encoder/_target_encoder.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:35.688845 crosspredict-1.1.9/crosspredict.egg-info/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     5584 2023-05-29 13:21:35.000000 crosspredict-1.1.9/crosspredict.egg-info/PKG-INFO
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1470 2023-05-29 13:21:35.000000 crosspredict-1.1.9/crosspredict.egg-info/SOURCES.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)        1 2023-05-29 13:21:35.000000 crosspredict-1.1.9/crosspredict.egg-info/dependency_links.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      247 2023-05-29 13:21:35.000000 crosspredict-1.1.9/crosspredict.egg-info/requires.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       19 2023-05-29 13:21:35.000000 crosspredict-1.1.9/crosspredict.egg-info/top_level.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      246 2022-09-26 08:59:16.000000 crosspredict-1.1.9/requirements.txt
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)       38 2023-05-29 13:21:36.105725 crosspredict-1.1.9/setup.cfg
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     1272 2023-05-29 13:21:28.000000 crosspredict-1.1.9/setup.py
+drwxr-xr-x   0 vboyadzhi   (503) staff       (20)        0 2023-05-29 13:21:36.105070 crosspredict-1.1.9/tests/
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)        0 2022-09-26 07:29:13.000000 crosspredict-1.1.9/tests/__init__.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)      556 2022-09-26 07:29:13.000000 crosspredict-1.1.9/tests/conftest.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     7765 2022-09-26 08:47:46.000000 crosspredict-1.1.9/tests/test_binary.py
+-rw-r--r--   0 vboyadzhi   (503) staff       (20)     2518 2022-09-26 07:29:13.000000 crosspredict-1.1.9/tests/test_iterator.py
```

### Comparing `crosspredict-1.1.8/LICENSE` & `crosspredict-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/PKG-INFO` & `crosspredict-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosspredict
-Version: 1.1.8
+Version: 1.1.9
 Summary: package for easy crossvalidation
 Home-page: UNKNOWN
 Author: Vladislav Boyadzhi
 Author-email: vladislav.boyadzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crosspredict-1.1.8/README.md` & `crosspredict-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/__pycache__/iterator.cpython-39.pyc` & `crosspredict-1.1.9/crosspredict/__pycache__/iterator.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc` & `crosspredict-1.1.9/crosspredict/crossval/__pycache__/_catboost.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc` & `crosspredict-1.1.9/crosspredict/crossval/__pycache__/_crossval.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc` & `crosspredict-1.1.9/crosspredict/crossval/__pycache__/_lightgbm.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc` & `crosspredict-1.1.9/crosspredict/crossval/__pycache__/_xgboost.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/crossval/_catboost.py` & `crosspredict-1.1.9/crosspredict/crossval/_catboost.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/crossval/_crossval.py` & `crosspredict-1.1.9/crosspredict/crossval/_crossval.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,16 @@
             self.params['metric'] = 'l2'
         elif self.params['metric'] in ('l1', 'mean_absolute_error', 'mae', 'regression_l1', 'regression'):
             self.params['metric'] = 'l1'
         elif self.params['metric'] in ('rmse', 'root_mean_squared_error', 'l2_root'):
             self.params['metric'] = 'rmse'
         elif self.params['metric'] in ('binary_logloss', 'binary'):
             self.params['metric'] = 'binary_logloss'
+        elif self.params['metric'] in ('multi_logloss', 'multiclass', 'softmax', 'multiclassova', 'multiclass_ova', 'ova', 'ovr'):
+            self.params['metric'] = 'multi_logloss'
 
         self.feature_name = feature_name
         self.cols_cat = cols_cat
         self.num_boost_round = num_boost_round
         self.early_stopping_rounds = early_stopping_rounds
         self.valid = valid
         self.col_target = col_target
@@ -125,15 +127,16 @@
             if self.valid:
                 # Построение прогнозов при разном виде взаимодействия
                 if self.params['metric'] in ('auc'):
                     scores[fold] = evals_result['eval'][self.params['metric']]
                 elif self.params['metric'] in (
                 'binary_logloss', 'binary', 'l1', 'mean_absolute_error', 'mae', 'regression_l1', 'l2',
                 'mean_squared_error', 'mse', 'regression_l2', 'regression', 'rmse',
-                'root_mean_squared_error', 'l2_root'):
+                'root_mean_squared_error', 'l2_root',
+                'multi_logloss', 'multiclass', 'softmax', 'multiclassova', 'multiclass_ova', 'ova', 'ovr'):
                     scores[fold] = [-1 * x for x in evals_result['eval'][self.params['metric']]]
 
                 best_auc = np.max(evals_result['eval'][self.params['metric']])
                 scores_avg.append(best_auc)
 
                 log.info(
                     f'\tCROSSVALIDATION FOLD {fold % self.iterator.n_splits} ENDS with best `{self.params["metric"]}` = {best_auc}')
@@ -199,15 +202,16 @@
         return predict
 
     def _get_shap_values(self, explainer, df_sample):
         if self.params['metric'] in ('auc', 'binary_logloss', 'binary'):
             return explainer.shap_values(df_sample)[1]
         elif self.params['metric'] in ('l1', 'mean_absolute_error', 'mae', 'regression_l1', 'l2',
                                        'mean_squared_error', 'mse', 'regression_l2', 'regression', 'rmse',
-                                       'root_mean_squared_error', 'l2_root'):
+                                       'root_mean_squared_error', 'l2_root',
+                'multi_logloss', 'multiclass', 'softmax', 'multiclassova', 'multiclass_ova', 'ova', 'ovr'):
             return explainer.shap_values(df_sample)
 
     def shap(self, df: pd.DataFrame, n_samples=500, figsize=(10, 10)):
         '''
 
         :param df:
         :param n_samples: количество записей которое будет семплироваться в каждом тестовом фолде для анализы shap values
```

### Comparing `crosspredict-1.1.8/crosspredict/crossval/_lightgbm.py` & `crosspredict-1.1.9/crosspredict/crossval/_lightgbm.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
         if self.params['objective'] in ('binary'):
             assert self.params['metric'] in ('auc', 'binary_logloss', 'binary'), \
                 f"""params.objective = {self.params['objective']}, and passed params.metrics = {self.params['metric']}, but SHOULD BE one of ['auc', 'binary_logloss', 'binary']"""
         elif self.params['objective'] in ('regression', 'regression_l1', 'mape'):
             assert self.params['metric'] in ('l1', 'mean_absolute_error', 'mae', 'regression_l1', 'l2',
                                               'mean_squared_error', 'mse', 'regression_l2', 'regression', 'rmse',
-                                              'root_mean_squared_error', 'l2_root'), \
+                                              'root_mean_squared_error', 'l2_root',
+                                             'multi_logloss', 'multiclass', 'softmax', 'multiclassova', 'multiclass_ova', 'ova', 'ovr'), \
                 f"""params.objective = {self.params['objective']}, and passed params.metrics = {self.params['metric']}, but SHOULD BE one of ['l1', 'mean_absolute_error', 'mae', 'regression_l1', 'l2', 'mean_squared_error', 'mse', 'regression_l2', 'regression', 'rmse', 'root_mean_squared_error', 'l2_root']"""
         # huber, fair, poisson, quantile, , gamma, tweedie, , multiclass, multiclassova, cross_entropy, cross_entropy_lambda, lambdarank, rank_xendcg, objective_type, app, application, loss
 
     def get_hyperopt_space(self, params={}, random_state=None):
         if random_state is None:
             random_state = self.random_state
         result = {
```

### Comparing `crosspredict-1.1.8/crosspredict/crossval/_xgboost.py` & `crosspredict-1.1.9/crosspredict/crossval/_xgboost.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/iterator.py` & `crosspredict-1.1.9/crosspredict/iterator.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/nodes/_nodes.py` & `crosspredict-1.1.9/crosspredict/nodes/_nodes.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/parameters.yml` & `crosspredict-1.1.9/crosspredict/parameters.yml`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc` & `crosspredict-1.1.9/crosspredict/report_binary/__pycache__/_curves.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc` & `crosspredict-1.1.9/crosspredict/report_binary/__pycache__/_report_binary.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/report_binary/_curves.py` & `crosspredict-1.1.9/crosspredict/report_binary/_curves.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/report_binary/_report_binary.py` & `crosspredict-1.1.9/crosspredict/report_binary/_report_binary.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/target_encoder/_crosstargetencoder.py` & `crosspredict-1.1.9/crosspredict/target_encoder/_crosstargetencoder.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict/target_encoder/_target_encoder.py` & `crosspredict-1.1.9/crosspredict/target_encoder/_target_encoder.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/crosspredict.egg-info/PKG-INFO` & `crosspredict-1.1.9/crosspredict.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crosspredict
-Version: 1.1.8
+Version: 1.1.9
 Summary: package for easy crossvalidation
 Home-page: UNKNOWN
 Author: Vladislav Boyadzhi
 Author-email: vladislav.boyadzhi@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `crosspredict-1.1.8/crosspredict.egg-info/SOURCES.txt` & `crosspredict-1.1.9/crosspredict.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/setup.py` & `crosspredict-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     with open('{0}/requirements.txt'.format(dir_path), 'r') as reqs:
         requirements = reqs.readlines()
     return requirements
 
 if __name__ == "__main__":
     setup(
         name="crosspredict",
-        version="1.1.8",
+        version="1.1.9",
         author="Vladislav Boyadzhi",
         author_email="vladislav.boyadzhi@gmail.com",
         description='package for easy crossvalidation',
         long_description=long_description,
         long_description_content_type="text/markdown",
         packages=find_packages(),
         classifiers=[
```

### Comparing `crosspredict-1.1.8/tests/conftest.py` & `crosspredict-1.1.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/tests/test_binary.py` & `crosspredict-1.1.9/tests/test_binary.py`

 * *Files identical despite different names*

### Comparing `crosspredict-1.1.8/tests/test_iterator.py` & `crosspredict-1.1.9/tests/test_iterator.py`

 * *Files identical despite different names*


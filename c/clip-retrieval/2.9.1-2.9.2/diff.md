# Comparing `tmp/clip_retrieval-2.9.1.tar.gz` & `tmp/clip_retrieval-2.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clip_retrieval-2.9.1.tar", last modified: Sat Sep 11 10:44:09 2021, max compression
+gzip compressed data, was "clip_retrieval-2.9.2.tar", last modified: Sat Sep 11 10:46:38 2021, max compression
```

## Comparing `clip_retrieval-2.9.1.tar` & `clip_retrieval-2.9.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-11 10:44:09.621286 clip_retrieval-2.9.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-09-11 10:43:57.000000 clip_retrieval-2.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    10340 2021-09-11 10:44:09.621286 clip_retrieval-2.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     8182 2021-09-11 10:43:57.000000 clip_retrieval-2.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-11 10:44:09.617286 clip_retrieval-2.9.1/clip_retrieval/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-11 10:43:57.000000 clip_retrieval-2.9.1/clip_retrieval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      436 2021-09-11 10:43:57.000000 clip_retrieval-2.9.1/clip_retrieval/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    12173 2021-09-11 10:43:57.000000 clip_retrieval-2.9.1/clip_retrieval/clip_back.py
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-09-11 10:43:57.000000 clip_retrieval-2.9.1/clip_retrieval/clip_filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1750 2021-09-11 10:43:57.000000 clip_retrieval-2.9.1/clip_retrieval/clip_index.py
--rw-r--r--   0 runner    (1001) docker     (121)    11200 2021-09-11 10:43:57.000000 clip_retrieval-2.9.1/clip_retrieval/clip_inference.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-11 10:44:09.621286 clip_retrieval-2.9.1/clip_retrieval.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    10340 2021-09-11 10:44:09.000000 clip_retrieval-2.9.1/clip_retrieval.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-09-11 10:44:09.000000 clip_retrieval-2.9.1/clip_retrieval.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-11 10:44:09.000000 clip_retrieval-2.9.1/clip_retrieval.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       60 2021-09-11 10:44:09.000000 clip_retrieval-2.9.1/clip_retrieval.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      155 2021-09-11 10:44:09.000000 clip_retrieval-2.9.1/clip_retrieval.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-11 10:44:09.000000 clip_retrieval-2.9.1/clip_retrieval.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-11 10:44:09.621286 clip_retrieval-2.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1784 2021-09-11 10:43:57.000000 clip_retrieval-2.9.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-11 10:46:38.972647 clip_retrieval-2.9.2/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-09-11 10:46:29.000000 clip_retrieval-2.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    10340 2021-09-11 10:46:38.972647 clip_retrieval-2.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     8182 2021-09-11 10:46:29.000000 clip_retrieval-2.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-11 10:46:38.972647 clip_retrieval-2.9.2/clip_retrieval/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-11 10:46:29.000000 clip_retrieval-2.9.2/clip_retrieval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2021-09-11 10:46:29.000000 clip_retrieval-2.9.2/clip_retrieval/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12173 2021-09-11 10:46:29.000000 clip_retrieval-2.9.2/clip_retrieval/clip_back.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2021-09-11 10:46:29.000000 clip_retrieval-2.9.2/clip_retrieval/clip_filter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1750 2021-09-11 10:46:29.000000 clip_retrieval-2.9.2/clip_retrieval/clip_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11200 2021-09-11 10:46:29.000000 clip_retrieval-2.9.2/clip_retrieval/clip_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-11 10:46:38.972647 clip_retrieval-2.9.2/clip_retrieval.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    10340 2021-09-11 10:46:38.000000 clip_retrieval-2.9.2/clip_retrieval.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      425 2021-09-11 10:46:38.000000 clip_retrieval-2.9.2/clip_retrieval.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-11 10:46:38.000000 clip_retrieval-2.9.2/clip_retrieval.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       60 2021-09-11 10:46:38.000000 clip_retrieval-2.9.2/clip_retrieval.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2021-09-11 10:46:38.000000 clip_retrieval-2.9.2/clip_retrieval.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-11 10:46:38.000000 clip_retrieval-2.9.2/clip_retrieval.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-09-11 10:46:38.972647 clip_retrieval-2.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1784 2021-09-11 10:46:29.000000 clip_retrieval-2.9.2/setup.py
```

### Comparing `clip_retrieval-2.9.1/LICENSE` & `clip_retrieval-2.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clip_retrieval-2.9.1/PKG-INFO` & `clip_retrieval-2.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip_retrieval
-Version: 2.9.1
+Version: 2.9.2
 Summary: Easily computing clip embeddings and building a clip retrieval system with them
 Home-page: https://github.com/rom1504/clip-retrieval
 Author: Romain Beaumont
 Author-email: romain.rom1@gmail.com
 License: MIT
 Description: # clip-retrieval
         [![pypi](https://img.shields.io/pypi/v/clip-retrieval.svg)](https://pypi.python.org/pypi/clip-retrieval)
```

### Comparing `clip_retrieval-2.9.1/README.md` & `clip_retrieval-2.9.2/README.md`

 * *Files identical despite different names*

### Comparing `clip_retrieval-2.9.1/clip_retrieval/clip_back.py` & `clip_retrieval-2.9.2/clip_retrieval/clip_back.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 DOWNLOAD_TIME,
                 TEXT_CLIP_INFERENCE_TIME,
                 IMAGE_CLIP_INFERENCE_TIME,
                 METADATA_GET_TIME,
                 KNN_INDEX_TIME,
                 IMAGE_PREPRO_TIME,
                 TEXT_PREPRO_TIME,
-            ]]], key=lambda e:-e[2])
+            ]]], key=lambda e:-e[3])
 
             sub_metrics_strings = [(name, description, int(metric_count), f"{avg:0.4f}s", f"{proportion*100:0.1f}%") \
                 for name, description, metric_count, avg, proportion in sub_metrics]
             
             s=""
             s+=f"Among {full_knn_count} calls to the knn end point with an average latency of {full_knn_avg:0.4f}s "+\
             "per request, the step costs are (in order): \n\n"
```

### Comparing `clip_retrieval-2.9.1/clip_retrieval/clip_filter.py` & `clip_retrieval-2.9.2/clip_retrieval/clip_filter.py`

 * *Files identical despite different names*

### Comparing `clip_retrieval-2.9.1/clip_retrieval/clip_index.py` & `clip_retrieval-2.9.2/clip_retrieval/clip_index.py`

 * *Files identical despite different names*

### Comparing `clip_retrieval-2.9.1/clip_retrieval/clip_inference.py` & `clip_retrieval-2.9.2/clip_retrieval/clip_inference.py`

 * *Files identical despite different names*

### Comparing `clip_retrieval-2.9.1/clip_retrieval.egg-info/PKG-INFO` & `clip_retrieval-2.9.2/clip_retrieval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clip-retrieval
-Version: 2.9.1
+Version: 2.9.2
 Summary: Easily computing clip embeddings and building a clip retrieval system with them
 Home-page: https://github.com/rom1504/clip-retrieval
 Author: Romain Beaumont
 Author-email: romain.rom1@gmail.com
 License: MIT
 Description: # clip-retrieval
         [![pypi](https://img.shields.io/pypi/v/clip-retrieval.svg)](https://pypi.python.org/pypi/clip-retrieval)
```

### Comparing `clip_retrieval-2.9.1/setup.py` & `clip_retrieval-2.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with Path(Path(__file__).parent, "README.md").open(encoding="utf-8") as file:
         long_description = file.read()
 
     setup(
         name = 'clip_retrieval',
         packages = find_packages(),
         include_package_data = True,
-        version = '2.9.1',
+        version = '2.9.2',
         license='MIT',
         description = 'Easily computing clip embeddings and building a clip retrieval system with them',
         long_description=long_description,
         long_description_content_type="text/markdown",
         entry_points={"console_scripts": ["clip-retrieval = clip_retrieval.cli:main"]},
         author = 'Romain Beaumont',
         author_email = 'romain.rom1@gmail.com',
```


# Comparing `tmp/cnmfsns-1.3.1.tar.gz` & `tmp/cnmfsns-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.3.1.tar", last modified: Mon May 29 17:15:48 2023, max compression
+gzip compressed data, was "cnmfsns-1.3.2.tar", last modified: Mon May 29 18:21:07 2023, max compression
```

## Comparing `cnmfsns-1.3.1.tar` & `cnmfsns-1.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 17:15:48.313333 cnmfsns-1.3.1/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.3.1/LICENSE
--rw-rw-rw-   0        0        0     3982 2023-05-29 17:15:48.313333 cnmfsns-1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     3467 2023-05-29 17:14:53.000000 cnmfsns-1.3.1/README.md
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      964 2023-05-29 17:15:48.313333 cnmfsns-1.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 17:15:48.266443 cnmfsns-1.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 17:15:48.282086 cnmfsns-1.3.1/src/cnmfsns/
--rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.3.1/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    56223 2023-05-16 20:25:56.000000 cnmfsns-1.3.1/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.3.1/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.3.1/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.3.1/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    35130 2023-05-29 17:09:43.000000 cnmfsns-1.3.1/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    21163 2023-05-15 22:09:27.000000 cnmfsns-1.3.1/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    57617 2023-05-16 18:55:37.000000 cnmfsns-1.3.1/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    35301 2023-05-16 19:23:15.000000 cnmfsns-1.3.1/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.3.1/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 17:15:48.313333 cnmfsns-1.3.1/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     3982 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      177 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 18:21:07.235811 cnmfsns-1.3.2/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     3982 2023-05-29 18:21:07.235811 cnmfsns-1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3467 2023-05-29 18:20:04.000000 cnmfsns-1.3.2/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0      964 2023-05-29 18:21:07.235811 cnmfsns-1.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 18:21:07.204917 cnmfsns-1.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 18:21:07.221291 cnmfsns-1.3.2/src/cnmfsns/
+-rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.3.2/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    56223 2023-05-16 20:25:56.000000 cnmfsns-1.3.2/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.3.2/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.3.2/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.3.2/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    35130 2023-05-29 17:09:43.000000 cnmfsns-1.3.2/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    21163 2023-05-15 22:09:27.000000 cnmfsns-1.3.2/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    57617 2023-05-16 18:55:37.000000 cnmfsns-1.3.2/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    35301 2023-05-16 19:23:15.000000 cnmfsns-1.3.2/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.3.2/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:21:07.235811 cnmfsns-1.3.2/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     3982 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      177 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-29 18:21:07.000000 cnmfsns-1.3.2/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.3.1/LICENSE` & `cnmfsns-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/PKG-INFO` & `cnmfsns-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.3.1
+Version: 1.3.2
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.3.1-blue)
+![version badge](https://img.shields.io/badge/version-1.3.2-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```

### Comparing `cnmfsns-1.3.1/README.md` & `cnmfsns-1.3.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 00000040: 2070 6f77 6572 6675 6c20 6661 6374 6f72   powerful factor
 00000050: 697a 6174 696f 6e2d 6261 7365 6420 6d75  ization-based mu
 00000060: 6c74 692d 6f6d 6963 7320 696e 7465 6772  lti-omics integr
 00000070: 6174 696f 6e20 746f 6f6c 6b69 740d 0a0d  ation toolkit...
 00000080: 0a21 5b76 6572 7369 6f6e 2062 6164 6765  .![version badge
 00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-000000b0: 6572 7369 6f6e 2d31 2e33 2e31 2d62 6c75  ersion-1.3.1-blu
+000000b0: 6572 7369 6f6e 2d31 2e33 2e32 2d62 6c75  ersion-1.3.2-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
```

### Comparing `cnmfsns-1.3.1/setup.cfg` & `cnmfsns-1.3.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 332e 310d 0a61 7574  ion = 1.3.1..aut
+00000020: 696f 6e20 3d20 312e 332e 320d 0a61 7574  ion = 1.3.2..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `cnmfsns-1.3.1/src/cnmfsns/__init__.py` & `cnmfsns-1.3.2/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/src/cnmfsns/cli.py` & `cnmfsns-1.3.2/src/cnmfsns/cli.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/src/cnmfsns/cnmf.py` & `cnmfsns-1.3.2/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/src/cnmfsns/colors.py` & `cnmfsns-1.3.2/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/src/cnmfsns/config.py` & `cnmfsns-1.3.2/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/src/cnmfsns/dataset.py` & `cnmfsns-1.3.2/src/cnmfsns/dataset.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/src/cnmfsns/integration.py` & `cnmfsns-1.3.2/src/cnmfsns/integration.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/src/cnmfsns/plots.py` & `cnmfsns-1.3.2/src/cnmfsns/plots.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/src/cnmfsns/sns.py` & `cnmfsns-1.3.2/src/cnmfsns/sns.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/src/cnmfsns/utils.py` & `cnmfsns-1.3.2/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.1/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.3.2/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.3.1
+Version: 1.3.2
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.3.1-blue)
+![version badge](https://img.shields.io/badge/version-1.3.2-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
 [![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
```


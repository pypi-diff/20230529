# Comparing `tmp/semantic-cleaning-0.0.2.tar.gz` & `tmp/semantic-cleaning-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic-cleaning-0.0.2.tar", last modified: Mon May 29 08:35:20 2023, max compression
+gzip compressed data, was "semantic-cleaning-0.0.3.tar", last modified: Mon May 29 08:45:14 2023, max compression
```

## Comparing `semantic-cleaning-0.0.2.tar` & `semantic-cleaning-0.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:35:20.398229 semantic-cleaning-0.0.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-05-29 08:27:54.000000 semantic-cleaning-0.0.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2023-05-29 08:27:54.000000 semantic-cleaning-0.0.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2870 2023-05-29 08:35:20.397229 semantic-cleaning-0.0.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2066 2023-05-29 08:27:54.000000 semantic-cleaning-0.0.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:35:20.393228 semantic-cleaning-0.0.2/semantic_cleaning/
--rw-r--r--   0 root         (0) root         (0)      120 2023-05-29 08:31:19.000000 semantic-cleaning-0.0.2/semantic_cleaning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1391 2023-05-29 08:31:19.000000 semantic-cleaning-0.0.2/semantic_cleaning/_modidx.py
--rw-r--r--   0 root         (0) root         (0)     8221 2023-05-29 08:31:19.000000 semantic-cleaning-0.0.2/semantic_cleaning/core.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:35:20.397229 semantic-cleaning-0.0.2/semantic_cleaning.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2870 2023-05-29 08:35:20.000000 semantic-cleaning-0.0.2/semantic_cleaning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      424 2023-05-29 08:35:20.000000 semantic-cleaning-0.0.2/semantic_cleaning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 08:35:20.000000 semantic-cleaning-0.0.2/semantic_cleaning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 08:35:20.000000 semantic-cleaning-0.0.2/semantic_cleaning.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 08:34:50.000000 semantic-cleaning-0.0.2/semantic_cleaning.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       57 2023-05-29 08:35:20.000000 semantic-cleaning-0.0.2/semantic_cleaning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 08:35:20.000000 semantic-cleaning-0.0.2/semantic_cleaning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      942 2023-05-29 08:31:19.000000 semantic-cleaning-0.0.2/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 08:35:20.398229 semantic-cleaning-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2596 2023-05-29 08:27:54.000000 semantic-cleaning-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:45:14.868780 semantic-cleaning-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-29 08:41:52.000000 semantic-cleaning-0.0.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2023-05-29 08:41:52.000000 semantic-cleaning-0.0.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-05-29 08:45:14.868780 semantic-cleaning-0.0.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2066 2023-05-29 08:41:52.000000 semantic-cleaning-0.0.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:45:14.865780 semantic-cleaning-0.0.3/semantic_cleaning/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-29 08:45:01.000000 semantic-cleaning-0.0.3/semantic_cleaning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1391 2023-05-29 08:45:01.000000 semantic-cleaning-0.0.3/semantic_cleaning/_modidx.py
+-rw-r--r--   0 root         (0) root         (0)     8221 2023-05-29 08:45:01.000000 semantic-cleaning-0.0.3/semantic_cleaning/core.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 08:45:14.867780 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2870 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      424 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 08:44:11.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       57 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 08:45:14.000000 semantic-cleaning-0.0.3/semantic_cleaning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      942 2023-05-29 08:45:01.000000 semantic-cleaning-0.0.3/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 08:45:14.868780 semantic-cleaning-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2596 2023-05-29 08:41:52.000000 semantic-cleaning-0.0.3/setup.py
```

### Comparing `semantic-cleaning-0.0.2/LICENSE` & `semantic-cleaning-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `semantic-cleaning-0.0.2/PKG-INFO` & `semantic-cleaning-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-cleaning
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for semantic cleaning of a test dataset
 Home-page: https://github.com/yuval6957/semantic-cleaning
 Author: Yuval Reina
 Author-email: yuval.reina@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: semantic-cleaning Version: 0.0.2 Summary: Tools for
+Metadata-Version: 2.1 Name: semantic-cleaning Version: 0.0.3 Summary: Tools for
 semantic cleaning of a test dataset Home-page: https://github.com/yuval6957/
 semantic-cleaning Author: Yuval Reina Author-email: yuval.reina@gmail.com
 License: Apache Software License 2.0 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `semantic-cleaning-0.0.2/README.md` & `semantic-cleaning-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `semantic-cleaning-0.0.2/semantic_cleaning/_modidx.py` & `semantic-cleaning-0.0.3/semantic_cleaning/_modidx.py`

 * *Files identical despite different names*

### Comparing `semantic-cleaning-0.0.2/semantic_cleaning/core.py` & `semantic-cleaning-0.0.3/semantic_cleaning/core.py`

 * *Files identical despite different names*

### Comparing `semantic-cleaning-0.0.2/semantic_cleaning.egg-info/PKG-INFO` & `semantic-cleaning-0.0.3/semantic_cleaning.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-cleaning
-Version: 0.0.2
+Version: 0.0.3
 Summary: Tools for semantic cleaning of a test dataset
 Home-page: https://github.com/yuval6957/semantic-cleaning
 Author: Yuval Reina
 Author-email: yuval.reina@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: semantic-cleaning Version: 0.0.2 Summary: Tools for
+Metadata-Version: 2.1 Name: semantic-cleaning Version: 0.0.3 Summary: Tools for
 semantic cleaning of a test dataset Home-page: https://github.com/yuval6957/
 semantic-cleaning Author: Yuval Reina Author-email: yuval.reina@gmail.com
 License: Apache Software License 2.0 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: Natural Language :: English Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
```

### Comparing `semantic-cleaning-0.0.2/settings.ini` & `semantic-cleaning-0.0.3/settings.ini`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = semantic-cleaning
 lib_name = semantic-cleaning
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 doc_path = _docs
 lib_path = semantic_cleaning
 nbs_path = nbs
 recursive = True
```

### Comparing `semantic-cleaning-0.0.2/setup.py` & `semantic-cleaning-0.0.3/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/atlassianhw-0.0.2.tar.gz` & `tmp/atlassianhw-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlassianhw-0.0.2.tar", last modified: Mon May 29 09:57:01 2023, max compression
+gzip compressed data, was "atlassianhw-0.0.3.tar", last modified: Mon May 29 10:03:30 2023, max compression
```

## Comparing `atlassianhw-0.0.2.tar` & `atlassianhw-0.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:57:01.308484 atlassianhw-0.0.2/
--rw-r--r--   0 jasonorawe   (501) staff       (20)    11337 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/LICENSE
--rw-r--r--   0 jasonorawe   (501) staff       (20)      111 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/MANIFEST.in
--rw-r--r--   0 jasonorawe   (501) staff       (20)     6059 2023-05-29 09:57:01.308363 atlassianhw-0.0.2/PKG-INFO
--rw-r--r--   0 jasonorawe   (501) staff       (20)     5292 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/README.md
-drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:57:01.301965 atlassianhw-0.0.2/atlassianhw/
--rw-r--r--   0 jasonorawe   (501) staff       (20)       22 2023-05-29 09:13:49.000000 atlassianhw-0.0.2/atlassianhw/__init__.py
-drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:57:01.305948 atlassianhw-0.0.2/atlassianhw/_data/
--rw-r--r--   0 jasonorawe   (501) staff       (20)   600353 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/atlassianhw/_data/Employee_details.xlsx
--rw-r--r--   0 jasonorawe   (501) staff       (20)     5483 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/atlassianhw/_data/Glossary.xlsx
--rw-r--r--   0 jasonorawe   (501) staff       (20)   324952 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/atlassianhw/_data/Manager_details.xlsx
--rw-r--r--   0 jasonorawe   (501) staff       (20)   183171 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/atlassianhw/_data/Manager_mapping.xlsx
--rw-r--r--   0 jasonorawe   (501) staff       (20)   140642 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/atlassianhw/_data/promo_meta_data.xlsx
--rw-r--r--   0 jasonorawe   (501) staff       (20)     1706 2023-05-29 09:13:56.000000 atlassianhw-0.0.2/atlassianhw/_modidx.py
--rw-r--r--   0 jasonorawe   (501) staff       (20)     3767 2023-05-29 09:13:49.000000 atlassianhw-0.0.2/atlassianhw/data.py
--rw-r--r--   0 jasonorawe   (501) staff       (20)     2738 2023-05-29 09:13:49.000000 atlassianhw-0.0.2/atlassianhw/utils.py
-drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:57:01.303102 atlassianhw-0.0.2/atlassianhw.egg-info/
--rw-r--r--   0 jasonorawe   (501) staff       (20)     6059 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/PKG-INFO
--rw-r--r--   0 jasonorawe   (501) staff       (20)      574 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/SOURCES.txt
--rw-r--r--   0 jasonorawe   (501) staff       (20)        1 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/dependency_links.txt
--rw-r--r--   0 jasonorawe   (501) staff       (20)       44 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/entry_points.txt
--rw-r--r--   0 jasonorawe   (501) staff       (20)        1 2023-05-29 09:34:57.000000 atlassianhw-0.0.2/atlassianhw.egg-info/not-zip-safe
--rw-r--r--   0 jasonorawe   (501) staff       (20)       78 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/requires.txt
--rw-r--r--   0 jasonorawe   (501) staff       (20)       12 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/top_level.txt
--rw-r--r--   0 jasonorawe   (501) staff       (20)     1001 2023-05-29 09:56:54.000000 atlassianhw-0.0.2/settings.ini
--rw-r--r--   0 jasonorawe   (501) staff       (20)       38 2023-05-29 09:57:01.308524 atlassianhw-0.0.2/setup.cfg
--rw-r--r--   0 jasonorawe   (501) staff       (20)     2637 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/setup.py
+drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 10:03:30.201704 atlassianhw-0.0.3/
+-rw-r--r--   0 jasonorawe   (501) staff       (20)    11337 2023-05-29 09:08:41.000000 atlassianhw-0.0.3/LICENSE
+-rw-r--r--   0 jasonorawe   (501) staff       (20)      111 2023-05-29 09:08:41.000000 atlassianhw-0.0.3/MANIFEST.in
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     6059 2023-05-29 10:03:30.201562 atlassianhw-0.0.3/PKG-INFO
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     5292 2023-05-29 10:02:14.000000 atlassianhw-0.0.3/README.md
+drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 10:03:30.196960 atlassianhw-0.0.3/atlassianhw/
+-rw-r--r--   0 jasonorawe   (501) staff       (20)       22 2023-05-29 10:02:02.000000 atlassianhw-0.0.3/atlassianhw/__init__.py
+drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 10:03:30.200947 atlassianhw-0.0.3/atlassianhw/_data/
+-rw-r--r--   0 jasonorawe   (501) staff       (20)   600353 2023-05-29 09:08:41.000000 atlassianhw-0.0.3/atlassianhw/_data/Employee_details.xlsx
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     5483 2023-05-29 09:08:41.000000 atlassianhw-0.0.3/atlassianhw/_data/Glossary.xlsx
+-rw-r--r--   0 jasonorawe   (501) staff       (20)   324952 2023-05-29 09:08:41.000000 atlassianhw-0.0.3/atlassianhw/_data/Manager_details.xlsx
+-rw-r--r--   0 jasonorawe   (501) staff       (20)   183171 2023-05-29 09:08:41.000000 atlassianhw-0.0.3/atlassianhw/_data/Manager_mapping.xlsx
+-rw-r--r--   0 jasonorawe   (501) staff       (20)   140642 2023-05-29 09:08:41.000000 atlassianhw-0.0.3/atlassianhw/_data/promo_meta_data.xlsx
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     1706 2023-05-29 10:02:02.000000 atlassianhw-0.0.3/atlassianhw/_modidx.py
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     3767 2023-05-29 10:02:02.000000 atlassianhw-0.0.3/atlassianhw/data.py
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     2738 2023-05-29 10:02:02.000000 atlassianhw-0.0.3/atlassianhw/utils.py
+drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 10:03:30.197929 atlassianhw-0.0.3/atlassianhw.egg-info/
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     6059 2023-05-29 10:03:30.000000 atlassianhw-0.0.3/atlassianhw.egg-info/PKG-INFO
+-rw-r--r--   0 jasonorawe   (501) staff       (20)      574 2023-05-29 10:03:30.000000 atlassianhw-0.0.3/atlassianhw.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonorawe   (501) staff       (20)        1 2023-05-29 10:03:30.000000 atlassianhw-0.0.3/atlassianhw.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonorawe   (501) staff       (20)       44 2023-05-29 10:03:30.000000 atlassianhw-0.0.3/atlassianhw.egg-info/entry_points.txt
+-rw-r--r--   0 jasonorawe   (501) staff       (20)        1 2023-05-29 09:34:57.000000 atlassianhw-0.0.3/atlassianhw.egg-info/not-zip-safe
+-rw-r--r--   0 jasonorawe   (501) staff       (20)       78 2023-05-29 10:03:30.000000 atlassianhw-0.0.3/atlassianhw.egg-info/requires.txt
+-rw-r--r--   0 jasonorawe   (501) staff       (20)       12 2023-05-29 10:03:30.000000 atlassianhw-0.0.3/atlassianhw.egg-info/top_level.txt
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     1001 2023-05-29 10:01:58.000000 atlassianhw-0.0.3/settings.ini
+-rw-r--r--   0 jasonorawe   (501) staff       (20)       38 2023-05-29 10:03:30.201749 atlassianhw-0.0.3/setup.cfg
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     2637 2023-05-29 09:08:41.000000 atlassianhw-0.0.3/setup.py
```

### Comparing `atlassianhw-0.0.2/LICENSE` & `atlassianhw-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/PKG-INFO` & `atlassianhw-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlassianhw
-Version: 0.0.2
+Version: 0.0.3
 Summary: Atlassian application homework
 Home-page: https://github.com/jazon33y/atlassianhw
 Author: jason
 Author-email: jazon33y@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: atlassianhw Version: 0.0.2 Summary: Atlassian
+Metadata-Version: 2.1 Name: atlassianhw Version: 0.0.3 Summary: Atlassian
 application homework Home-page: https://github.com/jazon33y/atlassianhw Author:
 jason Author-email: jazon33y@gmail.com License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `atlassianhw-0.0.2/README.md` & `atlassianhw-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/atlassianhw/_data/Employee_details.xlsx` & `atlassianhw-0.0.3/atlassianhw/_data/Employee_details.xlsx`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/atlassianhw/_data/Glossary.xlsx` & `atlassianhw-0.0.3/atlassianhw/_data/Glossary.xlsx`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/atlassianhw/_data/Manager_details.xlsx` & `atlassianhw-0.0.3/atlassianhw/_data/Manager_details.xlsx`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/atlassianhw/_data/Manager_mapping.xlsx` & `atlassianhw-0.0.3/atlassianhw/_data/Manager_mapping.xlsx`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/atlassianhw/_data/promo_meta_data.xlsx` & `atlassianhw-0.0.3/atlassianhw/_data/promo_meta_data.xlsx`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/atlassianhw/_modidx.py` & `atlassianhw-0.0.3/atlassianhw/_modidx.py`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/atlassianhw/data.py` & `atlassianhw-0.0.3/atlassianhw/data.py`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/atlassianhw/utils.py` & `atlassianhw-0.0.3/atlassianhw/utils.py`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/atlassianhw.egg-info/PKG-INFO` & `atlassianhw-0.0.3/atlassianhw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlassianhw
-Version: 0.0.2
+Version: 0.0.3
 Summary: Atlassian application homework
 Home-page: https://github.com/jazon33y/atlassianhw
 Author: jason
 Author-email: jazon33y@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: atlassianhw Version: 0.0.2 Summary: Atlassian
+Metadata-Version: 2.1 Name: atlassianhw Version: 0.0.3 Summary: Atlassian
 application homework Home-page: https://github.com/jazon33y/atlassianhw Author:
 jason Author-email: jazon33y@gmail.com License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `atlassianhw-0.0.2/atlassianhw.egg-info/SOURCES.txt` & `atlassianhw-0.0.3/atlassianhw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.2/settings.ini` & `atlassianhw-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = atlassianhw
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = atlassianhw
```

### Comparing `atlassianhw-0.0.2/setup.py` & `atlassianhw-0.0.3/setup.py`

 * *Files identical despite different names*


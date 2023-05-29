# Comparing `tmp/atlassianhw-0.0.1.tar.gz` & `tmp/atlassianhw-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atlassianhw-0.0.1.tar", last modified: Mon May 29 09:34:57 2023, max compression
+gzip compressed data, was "atlassianhw-0.0.2.tar", last modified: Mon May 29 09:57:01 2023, max compression
```

## Comparing `atlassianhw-0.0.1.tar` & `atlassianhw-0.0.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:34:57.261563 atlassianhw-0.0.1/
--rw-r--r--   0 jasonorawe   (501) staff       (20)    11337 2023-05-29 09:08:41.000000 atlassianhw-0.0.1/LICENSE
--rw-r--r--   0 jasonorawe   (501) staff       (20)      111 2023-05-29 09:08:41.000000 atlassianhw-0.0.1/MANIFEST.in
--rw-r--r--   0 jasonorawe   (501) staff       (20)     6059 2023-05-29 09:34:57.261408 atlassianhw-0.0.1/PKG-INFO
--rw-r--r--   0 jasonorawe   (501) staff       (20)     5292 2023-05-29 09:08:41.000000 atlassianhw-0.0.1/README.md
-drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:34:57.256459 atlassianhw-0.0.1/atlassianhw/
--rw-r--r--   0 jasonorawe   (501) staff       (20)       22 2023-05-29 09:13:49.000000 atlassianhw-0.0.1/atlassianhw/__init__.py
-drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:34:57.260726 atlassianhw-0.0.1/atlassianhw/_data/
--rw-r--r--   0 jasonorawe   (501) staff       (20)   600353 2023-05-29 09:08:41.000000 atlassianhw-0.0.1/atlassianhw/_data/Employee_details.xlsx
--rw-r--r--   0 jasonorawe   (501) staff       (20)     5483 2023-05-29 09:08:41.000000 atlassianhw-0.0.1/atlassianhw/_data/Glossary.xlsx
--rw-r--r--   0 jasonorawe   (501) staff       (20)   324952 2023-05-29 09:08:41.000000 atlassianhw-0.0.1/atlassianhw/_data/Manager_details.xlsx
--rw-r--r--   0 jasonorawe   (501) staff       (20)   183171 2023-05-29 09:08:41.000000 atlassianhw-0.0.1/atlassianhw/_data/Manager_mapping.xlsx
--rw-r--r--   0 jasonorawe   (501) staff       (20)   140642 2023-05-29 09:08:41.000000 atlassianhw-0.0.1/atlassianhw/_data/promo_meta_data.xlsx
--rw-r--r--   0 jasonorawe   (501) staff       (20)     1706 2023-05-29 09:13:56.000000 atlassianhw-0.0.1/atlassianhw/_modidx.py
--rw-r--r--   0 jasonorawe   (501) staff       (20)     3767 2023-05-29 09:13:49.000000 atlassianhw-0.0.1/atlassianhw/data.py
--rw-r--r--   0 jasonorawe   (501) staff       (20)     2738 2023-05-29 09:13:49.000000 atlassianhw-0.0.1/atlassianhw/utils.py
-drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:34:57.257672 atlassianhw-0.0.1/atlassianhw.egg-info/
--rw-r--r--   0 jasonorawe   (501) staff       (20)     6059 2023-05-29 09:34:57.000000 atlassianhw-0.0.1/atlassianhw.egg-info/PKG-INFO
--rw-r--r--   0 jasonorawe   (501) staff       (20)      574 2023-05-29 09:34:57.000000 atlassianhw-0.0.1/atlassianhw.egg-info/SOURCES.txt
--rw-r--r--   0 jasonorawe   (501) staff       (20)        1 2023-05-29 09:34:57.000000 atlassianhw-0.0.1/atlassianhw.egg-info/dependency_links.txt
--rw-r--r--   0 jasonorawe   (501) staff       (20)       44 2023-05-29 09:34:57.000000 atlassianhw-0.0.1/atlassianhw.egg-info/entry_points.txt
--rw-r--r--   0 jasonorawe   (501) staff       (20)        1 2023-05-29 09:34:57.000000 atlassianhw-0.0.1/atlassianhw.egg-info/not-zip-safe
--rw-r--r--   0 jasonorawe   (501) staff       (20)       70 2023-05-29 09:34:57.000000 atlassianhw-0.0.1/atlassianhw.egg-info/requires.txt
--rw-r--r--   0 jasonorawe   (501) staff       (20)       12 2023-05-29 09:34:57.000000 atlassianhw-0.0.1/atlassianhw.egg-info/top_level.txt
--rw-r--r--   0 jasonorawe   (501) staff       (20)      993 2023-05-29 09:12:54.000000 atlassianhw-0.0.1/settings.ini
--rw-r--r--   0 jasonorawe   (501) staff       (20)       38 2023-05-29 09:34:57.261618 atlassianhw-0.0.1/setup.cfg
--rw-r--r--   0 jasonorawe   (501) staff       (20)     2637 2023-05-29 09:08:41.000000 atlassianhw-0.0.1/setup.py
+drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:57:01.308484 atlassianhw-0.0.2/
+-rw-r--r--   0 jasonorawe   (501) staff       (20)    11337 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/LICENSE
+-rw-r--r--   0 jasonorawe   (501) staff       (20)      111 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/MANIFEST.in
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     6059 2023-05-29 09:57:01.308363 atlassianhw-0.0.2/PKG-INFO
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     5292 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/README.md
+drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:57:01.301965 atlassianhw-0.0.2/atlassianhw/
+-rw-r--r--   0 jasonorawe   (501) staff       (20)       22 2023-05-29 09:13:49.000000 atlassianhw-0.0.2/atlassianhw/__init__.py
+drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:57:01.305948 atlassianhw-0.0.2/atlassianhw/_data/
+-rw-r--r--   0 jasonorawe   (501) staff       (20)   600353 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/atlassianhw/_data/Employee_details.xlsx
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     5483 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/atlassianhw/_data/Glossary.xlsx
+-rw-r--r--   0 jasonorawe   (501) staff       (20)   324952 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/atlassianhw/_data/Manager_details.xlsx
+-rw-r--r--   0 jasonorawe   (501) staff       (20)   183171 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/atlassianhw/_data/Manager_mapping.xlsx
+-rw-r--r--   0 jasonorawe   (501) staff       (20)   140642 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/atlassianhw/_data/promo_meta_data.xlsx
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     1706 2023-05-29 09:13:56.000000 atlassianhw-0.0.2/atlassianhw/_modidx.py
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     3767 2023-05-29 09:13:49.000000 atlassianhw-0.0.2/atlassianhw/data.py
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     2738 2023-05-29 09:13:49.000000 atlassianhw-0.0.2/atlassianhw/utils.py
+drwxr-xr-x   0 jasonorawe   (501) staff       (20)        0 2023-05-29 09:57:01.303102 atlassianhw-0.0.2/atlassianhw.egg-info/
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     6059 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/PKG-INFO
+-rw-r--r--   0 jasonorawe   (501) staff       (20)      574 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/SOURCES.txt
+-rw-r--r--   0 jasonorawe   (501) staff       (20)        1 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/dependency_links.txt
+-rw-r--r--   0 jasonorawe   (501) staff       (20)       44 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/entry_points.txt
+-rw-r--r--   0 jasonorawe   (501) staff       (20)        1 2023-05-29 09:34:57.000000 atlassianhw-0.0.2/atlassianhw.egg-info/not-zip-safe
+-rw-r--r--   0 jasonorawe   (501) staff       (20)       78 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/requires.txt
+-rw-r--r--   0 jasonorawe   (501) staff       (20)       12 2023-05-29 09:57:01.000000 atlassianhw-0.0.2/atlassianhw.egg-info/top_level.txt
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     1001 2023-05-29 09:56:54.000000 atlassianhw-0.0.2/settings.ini
+-rw-r--r--   0 jasonorawe   (501) staff       (20)       38 2023-05-29 09:57:01.308524 atlassianhw-0.0.2/setup.cfg
+-rw-r--r--   0 jasonorawe   (501) staff       (20)     2637 2023-05-29 09:08:41.000000 atlassianhw-0.0.2/setup.py
```

### Comparing `atlassianhw-0.0.1/LICENSE` & `atlassianhw-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/PKG-INFO` & `atlassianhw-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlassianhw
-Version: 0.0.1
+Version: 0.0.2
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
-Metadata-Version: 2.1 Name: atlassianhw Version: 0.0.1 Summary: Atlassian
+Metadata-Version: 2.1 Name: atlassianhw Version: 0.0.2 Summary: Atlassian
 application homework Home-page: https://github.com/jazon33y/atlassianhw Author:
 jason Author-email: jazon33y@gmail.com License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `atlassianhw-0.0.1/README.md` & `atlassianhw-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/atlassianhw/_data/Employee_details.xlsx` & `atlassianhw-0.0.2/atlassianhw/_data/Employee_details.xlsx`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/atlassianhw/_data/Glossary.xlsx` & `atlassianhw-0.0.2/atlassianhw/_data/Glossary.xlsx`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/atlassianhw/_data/Manager_details.xlsx` & `atlassianhw-0.0.2/atlassianhw/_data/Manager_details.xlsx`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/atlassianhw/_data/Manager_mapping.xlsx` & `atlassianhw-0.0.2/atlassianhw/_data/Manager_mapping.xlsx`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/atlassianhw/_data/promo_meta_data.xlsx` & `atlassianhw-0.0.2/atlassianhw/_data/promo_meta_data.xlsx`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/atlassianhw/_modidx.py` & `atlassianhw-0.0.2/atlassianhw/_modidx.py`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/atlassianhw/data.py` & `atlassianhw-0.0.2/atlassianhw/data.py`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/atlassianhw/utils.py` & `atlassianhw-0.0.2/atlassianhw/utils.py`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/atlassianhw.egg-info/PKG-INFO` & `atlassianhw-0.0.2/atlassianhw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atlassianhw
-Version: 0.0.1
+Version: 0.0.2
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
-Metadata-Version: 2.1 Name: atlassianhw Version: 0.0.1 Summary: Atlassian
+Metadata-Version: 2.1 Name: atlassianhw Version: 0.0.2 Summary: Atlassian
 application homework Home-page: https://github.com/jazon33y/atlassianhw Author:
 jason Author-email: jazon33y@gmail.com License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python Classifier: Development Status :: 4 -
 Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
 :: English Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
```

### Comparing `atlassianhw-0.0.1/atlassianhw.egg-info/SOURCES.txt` & `atlassianhw-0.0.2/atlassianhw.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atlassianhw-0.0.1/settings.ini` & `atlassianhw-0.0.2/settings.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = atlassianhw
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = atlassianhw
@@ -34,10 +34,10 @@
 description = Atlassian application homework
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = jazon33y
 
 ### Optional ###
-requirements = fastcore pandas numpy nbdev matplotlib seaborn duckdb openpyxl
+requirements = fastcore pandas numpy nbdev matplotlib seaborn duckdb openpyxl jupyter
 # dev_requirements = 
 # console_scripts =
```

### Comparing `atlassianhw-0.0.1/setup.py` & `atlassianhw-0.0.2/setup.py`

 * *Files identical despite different names*


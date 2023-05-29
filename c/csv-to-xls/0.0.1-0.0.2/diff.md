# Comparing `tmp/csv_to_xls-0.0.1.tar.gz` & `tmp/csv_to_xls-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csv_to_xls-0.0.1.tar", last modified: Mon May 29 19:17:03 2023, max compression
+gzip compressed data, was "csv_to_xls-0.0.2.tar", last modified: Mon May 29 19:23:53 2023, max compression
```

## Comparing `csv_to_xls-0.0.1.tar` & `csv_to_xls-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:17:03.029695 csv_to_xls-0.0.1/
--rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 csv_to_xls-0.0.1/LICENSE
--rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 csv_to_xls-0.0.1/MANIFEST.in
--rw-r--r--   0 hamel      (501) staff       (20)     3119 2023-05-29 19:17:03.029551 csv_to_xls-0.0.1/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)     2332 2023-05-29 19:12:03.000000 csv_to_xls-0.0.1/README.md
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:17:03.028365 csv_to_xls-0.0.1/csv_to_xls/
--rw-r--r--   0 hamel      (501) staff       (20)       22 2023-05-29 19:14:41.000000 csv_to_xls-0.0.1/csv_to_xls/__init__.py
--rw-r--r--   0 hamel      (501) staff       (20)      385 2023-05-29 19:14:41.000000 csv_to_xls-0.0.1/csv_to_xls/_modidx.py
--rw-r--r--   0 hamel      (501) staff       (20)     1491 2023-05-29 19:14:41.000000 csv_to_xls-0.0.1/csv_to_xls/core.py
-drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:17:03.029360 csv_to_xls-0.0.1/csv_to_xls.egg-info/
--rw-r--r--   0 hamel      (501) staff       (20)     3119 2023-05-29 19:17:02.000000 csv_to_xls-0.0.1/csv_to_xls.egg-info/PKG-INFO
--rw-r--r--   0 hamel      (501) staff       (20)      354 2023-05-29 19:17:02.000000 csv_to_xls-0.0.1/csv_to_xls.egg-info/SOURCES.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-05-29 19:17:02.000000 csv_to_xls-0.0.1/csv_to_xls.egg-info/dependency_links.txt
--rw-r--r--   0 hamel      (501) staff       (20)       95 2023-05-29 19:17:02.000000 csv_to_xls-0.0.1/csv_to_xls.egg-info/entry_points.txt
--rw-r--r--   0 hamel      (501) staff       (20)        1 2023-05-29 19:14:53.000000 csv_to_xls-0.0.1/csv_to_xls.egg-info/not-zip-safe
--rw-r--r--   0 hamel      (501) staff       (20)       23 2023-05-29 19:17:02.000000 csv_to_xls-0.0.1/csv_to_xls.egg-info/requires.txt
--rw-r--r--   0 hamel      (501) staff       (20)       11 2023-05-29 19:17:02.000000 csv_to_xls-0.0.1/csv_to_xls.egg-info/top_level.txt
--rw-r--r--   0 hamel      (501) staff       (20)      976 2023-05-29 19:12:37.000000 csv_to_xls-0.0.1/settings.ini
--rw-r--r--   0 hamel      (501) staff       (20)       38 2023-05-29 19:17:03.029735 csv_to_xls-0.0.1/setup.cfg
--rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 csv_to_xls-0.0.1/setup.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:23:53.952527 csv_to_xls-0.0.2/
+-rw-rw-r--   0 hamel      (501) staff       (20)    11337 2023-04-27 10:12:58.000000 csv_to_xls-0.0.2/LICENSE
+-rw-rw-r--   0 hamel      (501) staff       (20)      111 2023-04-27 10:12:58.000000 csv_to_xls-0.0.2/MANIFEST.in
+-rw-r--r--   0 hamel      (501) staff       (20)     3119 2023-05-29 19:23:53.952363 csv_to_xls-0.0.2/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)     2332 2023-05-29 19:23:37.000000 csv_to_xls-0.0.2/README.md
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:23:53.951202 csv_to_xls-0.0.2/csv_to_xls/
+-rw-r--r--   0 hamel      (501) staff       (20)       22 2023-05-29 19:23:31.000000 csv_to_xls-0.0.2/csv_to_xls/__init__.py
+-rw-r--r--   0 hamel      (501) staff       (20)      385 2023-05-29 19:23:31.000000 csv_to_xls-0.0.2/csv_to_xls/_modidx.py
+-rw-r--r--   0 hamel      (501) staff       (20)     1666 2023-05-29 19:23:31.000000 csv_to_xls-0.0.2/csv_to_xls/core.py
+drwxr-xr-x   0 hamel      (501) staff       (20)        0 2023-05-29 19:23:53.952173 csv_to_xls-0.0.2/csv_to_xls.egg-info/
+-rw-r--r--   0 hamel      (501) staff       (20)     3119 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/PKG-INFO
+-rw-r--r--   0 hamel      (501) staff       (20)      354 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/SOURCES.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/dependency_links.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       95 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/entry_points.txt
+-rw-r--r--   0 hamel      (501) staff       (20)        1 2023-05-29 19:14:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/not-zip-safe
+-rw-r--r--   0 hamel      (501) staff       (20)       23 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/requires.txt
+-rw-r--r--   0 hamel      (501) staff       (20)       11 2023-05-29 19:23:53.000000 csv_to_xls-0.0.2/csv_to_xls.egg-info/top_level.txt
+-rw-r--r--   0 hamel      (501) staff       (20)      976 2023-05-29 19:23:25.000000 csv_to_xls-0.0.2/settings.ini
+-rw-r--r--   0 hamel      (501) staff       (20)       38 2023-05-29 19:23:53.952573 csv_to_xls-0.0.2/setup.cfg
+-rw-rw-r--   0 hamel      (501) staff       (20)     2596 2023-04-27 10:12:58.000000 csv_to_xls-0.0.2/setup.py
```

### Comparing `csv_to_xls-0.0.1/LICENSE` & `csv_to_xls-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csv_to_xls-0.0.1/PKG-INFO` & `csv_to_xls-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv_to_xls
-Version: 0.0.1
+Version: 0.0.2
 Summary: convert csvs to excel
 Home-page: https://github.com/hamelsmu/csv_to_xls
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `csv_to_xls-0.0.1/README.md` & `csv_to_xls-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `csv_to_xls-0.0.1/csv_to_xls.egg-info/PKG-INFO` & `csv_to_xls-0.0.2/csv_to_xls.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csv-to-xls
-Version: 0.0.1
+Version: 0.0.2
 Summary: convert csvs to excel
 Home-page: https://github.com/hamelsmu/csv_to_xls
 Author: Hamel Husain
 Author-email: hamel.husain@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `csv_to_xls-0.0.1/settings.ini` & `csv_to_xls-0.0.2/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = csv_to_xls
 lib_name = %(repo)s
-version = 0.0.1
+version = 0.0.2
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = csv_to_xls
```

### Comparing `csv_to_xls-0.0.1/setup.py` & `csv_to_xls-0.0.2/setup.py`

 * *Files identical despite different names*


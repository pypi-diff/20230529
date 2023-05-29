# Comparing `tmp/ma_fi-0.1.6.tar.gz` & `tmp/ma_fi-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma_fi-0.1.6.tar", last modified: Mon May 29 10:32:52 2023, max compression
+gzip compressed data, was "ma_fi-0.1.7.tar", last modified: Mon May 29 11:05:57 2023, max compression
```

## Comparing `ma_fi-0.1.6.tar` & `ma_fi-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 10:32:52.021692 ma_fi-0.1.6/
--rw-rw-rw-   0        0        0      584 2023-05-29 10:32:52.021692 ma_fi-0.1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 10:32:51.964126 ma_fi-0.1.6/ma_fi/
--rw-rw-rw-   0        0        0      194 2023-05-26 14:13:01.000000 ma_fi-0.1.6/ma_fi/__init__.py
--rw-rw-rw-   0        0        0     1951 2023-05-29 10:31:37.000000 ma_fi-0.1.6/ma_fi/download.py
-drwxrwxrwx   0        0        0        0 2023-05-29 10:32:52.011249 ma_fi-0.1.6/ma_fi.egg-info/
--rw-rw-rw-   0        0        0      584 2023-05-29 10:32:51.000000 ma_fi-0.1.6/ma_fi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-05-29 10:32:51.000000 ma_fi-0.1.6/ma_fi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 10:32:51.000000 ma_fi-0.1.6/ma_fi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-29 10:32:51.000000 ma_fi-0.1.6/ma_fi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-29 10:32:51.000000 ma_fi-0.1.6/ma_fi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 10:32:52.021692 ma_fi-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-29 10:32:12.000000 ma_fi-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:05:57.791037 ma_fi-0.1.7/
+-rw-rw-rw-   0        0        0      584 2023-05-29 11:05:57.787321 ma_fi-0.1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-29 11:05:57.708093 ma_fi-0.1.7/ma_fi/
+-rw-rw-rw-   0        0        0      194 2023-05-26 14:13:01.000000 ma_fi-0.1.7/ma_fi/__init__.py
+-rw-rw-rw-   0        0        0     3093 2023-05-29 11:05:28.000000 ma_fi-0.1.7/ma_fi/download.py
+drwxrwxrwx   0        0        0        0 2023-05-29 11:05:57.778580 ma_fi-0.1.7/ma_fi.egg-info/
+-rw-rw-rw-   0        0        0      584 2023-05-29 11:05:57.000000 ma_fi-0.1.7/ma_fi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2023-05-29 11:05:57.000000 ma_fi-0.1.7/ma_fi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 11:05:57.000000 ma_fi-0.1.7/ma_fi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-29 11:05:57.000000 ma_fi-0.1.7/ma_fi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-29 11:05:57.000000 ma_fi-0.1.7/ma_fi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 11:05:57.792487 ma_fi-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-29 11:05:39.000000 ma_fi-0.1.7/setup.py
```

### Comparing `ma_fi-0.1.6/PKG-INFO` & `ma_fi-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma_fi
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library for accessing financial data of Moroccan stock exchange companies
 Home-page: https://github.com/alitalbi/mfinance
 Author: Ali Talbi
 Author-email: alitalbi73@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ma_fi-0.1.6/ma_fi.egg-info/PKG-INFO` & `ma_fi-0.1.7/ma_fi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma-fi
-Version: 0.1.6
+Version: 0.1.7
 Summary: Library for accessing financial data of Moroccan stock exchange companies
 Home-page: https://github.com/alitalbi/mfinance
 Author: Ali Talbi
 Author-email: alitalbi73@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ma_fi-0.1.6/setup.py` & `ma_fi-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='ma_fi',
-    version='0.1.6',
+    version='0.1.7',
     description='Library for accessing financial data of Moroccan stock exchange companies',
     author='Ali Talbi',
     author_email='alitalbi73@gmail.com',
     url='https://github.com/alitalbi/mfinance',
     packages=['ma_fi'],
     install_requires=[
         'pandas',
```


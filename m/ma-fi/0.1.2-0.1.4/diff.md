# Comparing `tmp/ma_fi-0.1.2.tar.gz` & `tmp/ma_fi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ma_fi-0.1.2.tar", last modified: Fri May 26 13:54:54 2023, max compression
+gzip compressed data, was "ma_fi-0.1.4.tar", last modified: Sun May 28 22:57:47 2023, max compression
```

## Comparing `ma_fi-0.1.2.tar` & `ma_fi-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 13:54:54.249026 ma_fi-0.1.2/
--rw-rw-rw-   0        0        0      584 2023-05-26 13:54:54.243950 ma_fi-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 13:54:54.191257 ma_fi-0.1.2/ma_fi/
--rw-rw-rw-   0        0        0      194 2023-05-26 13:53:27.000000 ma_fi-0.1.2/ma_fi/__init__.py
--rw-rw-rw-   0        0        0     1554 2023-05-26 13:39:27.000000 ma_fi-0.1.2/ma_fi/download.py
-drwxrwxrwx   0        0        0        0 2023-05-26 13:54:54.236950 ma_fi-0.1.2/ma_fi.egg-info/
--rw-rw-rw-   0        0        0      584 2023-05-26 13:54:53.000000 ma_fi-0.1.2/ma_fi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-05-26 13:54:53.000000 ma_fi-0.1.2/ma_fi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 13:54:53.000000 ma_fi-0.1.2/ma_fi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-26 13:54:53.000000 ma_fi-0.1.2/ma_fi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-26 13:54:53.000000 ma_fi-0.1.2/ma_fi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 13:54:54.249026 ma_fi-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      836 2023-05-26 13:54:40.000000 ma_fi-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 22:57:47.067618 ma_fi-0.1.4/
+-rw-rw-rw-   0        0        0      584 2023-05-28 22:57:47.059528 ma_fi-0.1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-28 22:57:46.931375 ma_fi-0.1.4/ma_fi/
+-rw-rw-rw-   0        0        0      194 2023-05-26 14:13:01.000000 ma_fi-0.1.4/ma_fi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 22:57:47.048274 ma_fi-0.1.4/ma_fi.egg-info/
+-rw-rw-rw-   0        0        0      584 2023-05-28 22:57:46.000000 ma_fi-0.1.4/ma_fi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      170 2023-05-28 22:57:46.000000 ma_fi-0.1.4/ma_fi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 22:57:46.000000 ma_fi-0.1.4/ma_fi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-28 22:57:46.000000 ma_fi-0.1.4/ma_fi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 22:57:46.000000 ma_fi-0.1.4/ma_fi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 22:57:47.073639 ma_fi-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      836 2023-05-28 22:57:37.000000 ma_fi-0.1.4/setup.py
```

### Comparing `ma_fi-0.1.2/PKG-INFO` & `ma_fi-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma_fi
-Version: 0.1.2
+Version: 0.1.4
 Summary: Library for accessing financial data of Moroccan stock exchange companies
 Home-page: https://github.com/alitalbi/mfinance
 Author: Ali Talbi
 Author-email: alitalbi73@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ma_fi-0.1.2/ma_fi.egg-info/PKG-INFO` & `ma_fi-0.1.4/ma_fi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ma-fi
-Version: 0.1.2
+Version: 0.1.4
 Summary: Library for accessing financial data of Moroccan stock exchange companies
 Home-page: https://github.com/alitalbi/mfinance
 Author: Ali Talbi
 Author-email: alitalbi73@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ma_fi-0.1.2/setup.py` & `ma_fi-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='ma_fi',
-    version='0.1.2',
+    version='0.1.4',
     description='Library for accessing financial data of Moroccan stock exchange companies',
     author='Ali Talbi',
     author_email='alitalbi73@gmail.com',
     url='https://github.com/alitalbi/mfinance',
     packages=['ma_fi'],
     install_requires=[
         'pandas',
```


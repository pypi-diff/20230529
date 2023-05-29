# Comparing `tmp/jatool-1.96.tar.gz` & `tmp/jatool-1.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jatool-1.96.tar", last modified: Mon May 29 02:41:05 2023, max compression
+gzip compressed data, was "jatool-1.97.tar", last modified: Mon May 29 03:15:53 2023, max compression
```

## Comparing `jatool-1.96.tar` & `jatool-1.97.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 02:41:05.944362 jatool-1.96/
--rw-r--r--   0 mac        (501) staff       (20)     2763 2023-05-29 02:41:05.943966 jatool-1.96/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2391 2023-05-29 02:05:05.000000 jatool-1.96/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 02:41:05.941126 jatool-1.96/jatool/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-29 02:05:06.000000 jatool-1.96/jatool/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    25589 2023-05-29 02:40:01.000000 jatool-1.96/jatool/function.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 02:41:05.943448 jatool-1.96/jatool.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2763 2023-05-29 02:41:05.000000 jatool-1.96/jatool.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      205 2023-05-29 02:41:05.000000 jatool-1.96/jatool.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-29 02:41:05.000000 jatool-1.96/jatool.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      132 2023-05-29 02:41:05.000000 jatool-1.96/jatool.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2023-05-29 02:41:05.000000 jatool-1.96/jatool.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-29 02:41:05.944455 jatool-1.96/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      939 2023-05-29 02:40:17.000000 jatool-1.96/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:15:53.212915 jatool-1.97/
+-rw-r--r--   0 mac        (501) staff       (20)       14 2023-05-29 03:14:51.000000 jatool-1.97/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)     2763 2023-05-29 03:15:53.212501 jatool-1.97/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2391 2023-05-29 02:05:05.000000 jatool-1.97/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:15:53.167174 jatool-1.97/data/
+-rw-r--r--   0 mac        (501) staff       (20) 14743588 2023-05-29 02:05:05.000000 jatool-1.97/data/fiction_info_new.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1090 2023-05-29 02:05:06.000000 jatool-1.97/data/stopwords_list_new.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:15:53.209215 jatool-1.97/jatool/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-29 02:05:06.000000 jatool-1.97/jatool/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    25589 2023-05-29 03:14:53.000000 jatool-1.97/jatool/function.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:15:53.211968 jatool-1.97/jatool.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2763 2023-05-29 03:15:53.000000 jatool-1.97/jatool.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      271 2023-05-29 03:15:53.000000 jatool-1.97/jatool.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-29 03:15:53.000000 jatool-1.97/jatool.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      132 2023-05-29 03:15:53.000000 jatool-1.97/jatool.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        7 2023-05-29 03:15:53.000000 jatool-1.97/jatool.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-29 03:15:53.213017 jatool-1.97/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      971 2023-05-29 03:14:52.000000 jatool-1.97/setup.py
```

### Comparing `jatool-1.96/PKG-INFO` & `jatool-1.97/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jatool
-Version: 1.96
+Version: 1.97
 Summary: A Python package for jatools
 Home-page: https://github.com/bigbrolv/jatool
 Author: Pigpig
 Author-email: 21310238@tongji.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jatool-1.96/README.md` & `jatool-1.97/README.md`

 * *Files identical despite different names*

### Comparing `jatool-1.96/jatool/function.py` & `jatool-1.97/jatool/function.py`

 * *Files identical despite different names*

### Comparing `jatool-1.96/jatool.egg-info/PKG-INFO` & `jatool-1.97/jatool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jatool
-Version: 1.96
+Version: 1.97
 Summary: A Python package for jatools
 Home-page: https://github.com/bigbrolv/jatool
 Author: Pigpig
 Author-email: 21310238@tongji.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jatool-1.96/setup.py` & `jatool-1.97/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from setuptools import setup, find_packages
+
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='jatool',
-    version='1.96',
+    version='1.97',
     author='Pigpig',
     author_email='21310238@tongji.edu.cn',
     description='A Python package for jatools',
+    include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bigbrolv/jatool",
     packages=find_packages(),
     classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```


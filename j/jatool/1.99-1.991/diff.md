# Comparing `tmp/jatool-1.99.tar.gz` & `tmp/jatool-1.991.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jatool-1.99.tar", last modified: Mon May 29 03:35:35 2023, max compression
+gzip compressed data, was "jatool-1.991.tar", last modified: Mon May 29 03:42:45 2023, max compression
```

## Comparing `jatool-1.99.tar` & `jatool-1.991.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:35:35.164193 jatool-1.99/
--rw-r--r--   0 mac        (501) staff       (20)       14 2023-05-29 03:14:51.000000 jatool-1.99/MANIFEST.in
--rw-r--r--   0 mac        (501) staff       (20)     2763 2023-05-29 03:35:35.163685 jatool-1.99/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2391 2023-05-29 02:05:05.000000 jatool-1.99/README.md
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:35:35.136155 jatool-1.99/data/
--rw-r--r--   0 mac        (501) staff       (20) 14743588 2023-05-29 02:05:05.000000 jatool-1.99/data/fiction_info_new.txt
--rw-r--r--   0 mac        (501) staff       (20)     1090 2023-05-29 02:05:06.000000 jatool-1.99/data/stopwords_list_new.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:35:35.159984 jatool-1.99/jatool/
--rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-29 02:05:06.000000 jatool-1.99/jatool/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    25589 2023-05-29 03:23:07.000000 jatool-1.99/jatool/function.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:35:35.162968 jatool-1.99/jatool.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     2763 2023-05-29 03:35:35.000000 jatool-1.99/jatool.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)      271 2023-05-29 03:35:35.000000 jatool-1.99/jatool.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-29 03:35:35.000000 jatool-1.99/jatool.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)      132 2023-05-29 03:35:35.000000 jatool-1.99/jatool.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2023-05-29 03:35:35.000000 jatool-1.99/jatool.egg-info/top_level.txt
--rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-29 03:35:35.164298 jatool-1.99/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)      971 2023-05-29 03:35:29.000000 jatool-1.99/setup.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:42:45.149479 jatool-1.991/
+-rw-r--r--   0 mac        (501) staff       (20)       59 2023-05-29 03:41:56.000000 jatool-1.991/MANIFEST.in
+-rw-r--r--   0 mac        (501) staff       (20)     2764 2023-05-29 03:42:45.149079 jatool-1.991/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)     2391 2023-05-29 02:05:05.000000 jatool-1.991/README.md
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:42:45.116450 jatool-1.991/data/
+-rw-r--r--   0 mac        (501) staff       (20) 14743588 2023-05-29 02:05:05.000000 jatool-1.991/data/fiction_info_new.txt
+-rw-r--r--   0 mac        (501) staff       (20)     1090 2023-05-29 02:05:06.000000 jatool-1.991/data/stopwords_list_new.txt
+-rw-r--r--   0 mac        (501) staff       (20) 14743588 2023-05-29 02:05:05.000000 jatool-1.991/fiction_info_new.txt
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:42:45.144982 jatool-1.991/jatool/
+-rw-r--r--   0 mac        (501) staff       (20)        0 2023-05-29 02:05:06.000000 jatool-1.991/jatool/__init__.py
+-rw-r--r--   0 mac        (501) staff       (20)    25589 2023-05-29 03:23:07.000000 jatool-1.991/jatool/function.py
+drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-05-29 03:42:45.148512 jatool-1.991/jatool.egg-info/
+-rw-r--r--   0 mac        (501) staff       (20)     2764 2023-05-29 03:42:44.000000 jatool-1.991/jatool.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (501) staff       (20)      315 2023-05-29 03:42:44.000000 jatool-1.991/jatool.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (501) staff       (20)        1 2023-05-29 03:42:44.000000 jatool-1.991/jatool.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (501) staff       (20)      132 2023-05-29 03:42:44.000000 jatool-1.991/jatool.egg-info/requires.txt
+-rw-r--r--   0 mac        (501) staff       (20)        7 2023-05-29 03:42:44.000000 jatool-1.991/jatool.egg-info/top_level.txt
+-rw-r--r--   0 mac        (501) staff       (20)       38 2023-05-29 03:42:45.149589 jatool-1.991/setup.cfg
+-rw-r--r--   0 mac        (501) staff       (20)      972 2023-05-29 03:42:27.000000 jatool-1.991/setup.py
+-rw-r--r--   0 mac        (501) staff       (20)     1090 2023-05-29 02:05:06.000000 jatool-1.991/stopwords_list_new.txt
```

### Comparing `jatool-1.99/PKG-INFO` & `jatool-1.991/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jatool
-Version: 1.99
+Version: 1.991
 Summary: A Python package for jatools
 Home-page: https://github.com/bigbrolv/jatool
 Author: Pigpig
 Author-email: 21310238@tongji.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jatool-1.99/README.md` & `jatool-1.991/README.md`

 * *Files identical despite different names*

### Comparing `jatool-1.99/data/fiction_info_new.txt` & `jatool-1.991/data/fiction_info_new.txt`

 * *Files identical despite different names*

### Comparing `jatool-1.99/data/stopwords_list_new.txt` & `jatool-1.991/data/stopwords_list_new.txt`

 * *Files identical despite different names*

### Comparing `jatool-1.99/jatool/function.py` & `jatool-1.991/jatool/function.py`

 * *Files identical despite different names*

### Comparing `jatool-1.99/jatool.egg-info/PKG-INFO` & `jatool-1.991/jatool.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jatool
-Version: 1.99
+Version: 1.991
 Summary: A Python package for jatools
 Home-page: https://github.com/bigbrolv/jatool
 Author: Pigpig
 Author-email: 21310238@tongji.edu.cn
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `jatool-1.99/setup.py` & `jatool-1.991/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='jatool',
-    version='1.99',
+    version='1.991',
     author='Pigpig',
     author_email='21310238@tongji.edu.cn',
     description='A Python package for jatools',
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/bigbrolv/jatool",
```


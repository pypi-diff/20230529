# Comparing `tmp/navinfo_tool-0.1.7.tar.gz` & `tmp/navinfo_tool-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\navinfo_tool-0.1.7.tar", last modified: Mon Apr 10 02:15:21 2023, max compression
+gzip compressed data, was "dist\navinfo_tool-0.1.8.tar", last modified: Mon May 29 03:24:47 2023, max compression
```

## Comparing `navinfo_tool-0.1.7.tar` & `navinfo_tool-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 02:15:21.000000 navinfo_tool-0.1.7/
--rw-rw-rw-   0        0        0      168 2023-04-10 02:15:21.000000 navinfo_tool-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0       14 2022-03-11 02:29:07.000000 navinfo_tool-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 02:15:21.000000 navinfo_tool-0.1.7/navinfo_tool/
--rw-rw-rw-   0        0        0     2288 2022-09-20 03:04:32.000000 navinfo_tool-0.1.7/navinfo_tool/__init__.py
--rw-rw-rw-   0        0        0    22792 2022-03-11 02:29:07.000000 navinfo_tool-0.1.7/navinfo_tool/end_words.py
--rw-rw-rw-   0        0        0    42215 2022-06-10 09:27:06.000000 navinfo_tool-0.1.7/navinfo_tool/rule_error_identification.py
--rw-rw-rw-   0        0        0    43398 2022-03-11 02:29:07.000000 navinfo_tool-0.1.7/navinfo_tool/rule_error_identification1009.py
--rw-rw-rw-   0        0        0    25226 2022-03-11 02:29:07.000000 navinfo_tool-0.1.7/navinfo_tool/same_stroke.py
--rw-rw-rw-   0        0        0    18759 2022-06-10 09:51:39.000000 navinfo_tool-0.1.7/navinfo_tool/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-10 02:15:21.000000 navinfo_tool-0.1.7/navinfo_tool.egg-info/
--rw-rw-rw-   0        0        0      168 2023-04-10 02:15:21.000000 navinfo_tool-0.1.7/navinfo_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      386 2023-04-10 02:15:21.000000 navinfo_tool-0.1.7/navinfo_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 02:15:21.000000 navinfo_tool-0.1.7/navinfo_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-10 02:15:21.000000 navinfo_tool-0.1.7/navinfo_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-10 02:15:21.000000 navinfo_tool-0.1.7/navinfo_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 02:15:21.000000 navinfo_tool-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      594 2023-04-10 02:14:59.000000 navinfo_tool-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:24:47.000000 navinfo_tool-0.1.8/
+-rw-rw-rw-   0        0        0      168 2023-05-29 03:24:47.000000 navinfo_tool-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2022-03-11 02:29:07.000000 navinfo_tool-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 03:24:47.000000 navinfo_tool-0.1.8/navinfo_tool/
+-rw-rw-rw-   0        0        0     2288 2022-09-20 03:04:32.000000 navinfo_tool-0.1.8/navinfo_tool/__init__.py
+-rw-rw-rw-   0        0        0    22792 2022-03-11 02:29:07.000000 navinfo_tool-0.1.8/navinfo_tool/end_words.py
+-rw-rw-rw-   0        0        0    42215 2022-06-10 09:27:06.000000 navinfo_tool-0.1.8/navinfo_tool/rule_error_identification.py
+-rw-rw-rw-   0        0        0    43398 2022-03-11 02:29:07.000000 navinfo_tool-0.1.8/navinfo_tool/rule_error_identification1009.py
+-rw-rw-rw-   0        0        0    25226 2022-03-11 02:29:07.000000 navinfo_tool-0.1.8/navinfo_tool/same_stroke.py
+-rw-rw-rw-   0        0        0    18759 2022-06-10 09:51:39.000000 navinfo_tool-0.1.8/navinfo_tool/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:24:47.000000 navinfo_tool-0.1.8/navinfo_tool.egg-info/
+-rw-rw-rw-   0        0        0      168 2023-05-29 03:24:46.000000 navinfo_tool-0.1.8/navinfo_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      386 2023-05-29 03:24:47.000000 navinfo_tool-0.1.8/navinfo_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 03:24:46.000000 navinfo_tool-0.1.8/navinfo_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-05-29 03:24:46.000000 navinfo_tool-0.1.8/navinfo_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 03:24:46.000000 navinfo_tool-0.1.8/navinfo_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 03:24:47.000000 navinfo_tool-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      599 2023-05-29 03:24:23.000000 navinfo_tool-0.1.8/setup.py
```

### Comparing `navinfo_tool-0.1.7/navinfo_tool/__init__.py` & `navinfo_tool-0.1.8/navinfo_tool/__init__.py`

 * *Files identical despite different names*

### Comparing `navinfo_tool-0.1.7/navinfo_tool/end_words.py` & `navinfo_tool-0.1.8/navinfo_tool/end_words.py`

 * *Files identical despite different names*

### Comparing `navinfo_tool-0.1.7/navinfo_tool/rule_error_identification.py` & `navinfo_tool-0.1.8/navinfo_tool/rule_error_identification.py`

 * *Files identical despite different names*

### Comparing `navinfo_tool-0.1.7/navinfo_tool/rule_error_identification1009.py` & `navinfo_tool-0.1.8/navinfo_tool/rule_error_identification1009.py`

 * *Files identical despite different names*

### Comparing `navinfo_tool-0.1.7/navinfo_tool/same_stroke.py` & `navinfo_tool-0.1.8/navinfo_tool/same_stroke.py`

 * *Files identical despite different names*

### Comparing `navinfo_tool-0.1.7/navinfo_tool/utils.py` & `navinfo_tool-0.1.8/navinfo_tool/utils.py`

 * *Files identical despite different names*

### Comparing `navinfo_tool-0.1.7/setup.py` & `navinfo_tool-0.1.8/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python
 # coding=utf-8
 
 from setuptools import setup, find_packages
 
 setup(
     name='navinfo_tool',
-    version='0.1.7',
+    version='0.1.8',
     description=(
         'utils for nlp'
     ),
     author='navinfo_nlp',
     author_email='navinfo_nlp@163.com',
     license='Apache License 2.0',
     packages=find_packages(),
     install_requires=[
         'xlrd==1.2.0',
         'jieba',
         'xlwt',
         'xlutils',
         'matplotlib',
-        'sklearn',
+        'scikit-learn',
         'pandas',
         'fairies',
         'configparser',
         'xpinyin==0.7.6',
         'xlsxwriter==3.0.1',
         'tqdm'
     ],
```


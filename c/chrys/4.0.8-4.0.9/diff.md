# Comparing `tmp/chrys-4.0.8.tar.gz` & `tmp/chrys-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrys-4.0.8.tar", last modified: Tue Nov  2 21:46:49 2021, max compression
+gzip compressed data, was "chrys-4.0.9.tar", last modified: Sun Jan 16 06:55:03 2022, max compression
```

## Comparing `chrys-4.0.8.tar` & `chrys-4.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 hein      (1000) hein      (1000)        0 2021-11-02 21:46:49.579330 chrys-4.0.8/
--rw-rw-r--   0 hein      (1000) hein      (1000)     1511 2021-11-02 13:59:00.000000 chrys-4.0.8/LICENSE
--rw-rw-r--   0 hein      (1000) hein      (1000)     2164 2021-11-02 21:46:49.579330 chrys-4.0.8/PKG-INFO
--rw-rw-r--   0 hein      (1000) hein      (1000)     1125 2021-11-02 13:59:00.000000 chrys-4.0.8/README.md
-drwxrwxr-x   0 hein      (1000) hein      (1000)        0 2021-11-02 21:46:49.575330 chrys-4.0.8/chrys/
--rw-rw-r--   0 hein      (1000) hein      (1000)       15 2021-11-02 13:59:00.000000 chrys-4.0.8/chrys/__init__.py
-drwxrwxr-x   0 hein      (1000) hein      (1000)        0 2021-11-02 21:46:49.579330 chrys-4.0.8/chrys/data/
--rw-rw-r--   0 hein      (1000) hein      (1000)        0 2021-11-02 13:59:00.000000 chrys-4.0.8/chrys/data/__init__.py
--rw-rw-r--   0 hein      (1000) hein      (1000)    92457 2021-11-02 21:46:17.000000 chrys-4.0.8/chrys/data/bokeh_palettes.py
--rw-rw-r--   0 hein      (1000) hein      (1000)   120856 2021-11-02 21:46:17.000000 chrys-4.0.8/chrys/data/vega_palettes.py
--rw-rw-r--   0 hein      (1000) hein      (1000)     9909 2021-11-02 13:59:00.000000 chrys-4.0.8/chrys/palettes.py
--rw-rw-r--   0 hein      (1000) hein      (1000)     1167 2021-11-02 13:59:00.000000 chrys-4.0.8/chrys/utils.py
-drwxrwxr-x   0 hein      (1000) hein      (1000)        0 2021-11-02 21:46:49.575330 chrys-4.0.8/chrys.egg-info/
--rw-rw-r--   0 hein      (1000) hein      (1000)     2164 2021-11-02 21:46:49.000000 chrys-4.0.8/chrys.egg-info/PKG-INFO
--rw-rw-r--   0 hein      (1000) hein      (1000)      311 2021-11-02 21:46:49.000000 chrys-4.0.8/chrys.egg-info/SOURCES.txt
--rw-rw-r--   0 hein      (1000) hein      (1000)        1 2021-11-02 21:46:49.000000 chrys-4.0.8/chrys.egg-info/dependency_links.txt
--rw-rw-r--   0 hein      (1000) hein      (1000)       86 2021-11-02 21:46:49.000000 chrys-4.0.8/chrys.egg-info/requires.txt
--rw-rw-r--   0 hein      (1000) hein      (1000)        6 2021-11-02 21:46:49.000000 chrys-4.0.8/chrys.egg-info/top_level.txt
--rw-rw-r--   0 hein      (1000) hein      (1000)       99 2021-11-02 21:46:49.579330 chrys-4.0.8/setup.cfg
--rw-rw-r--   0 hein      (1000) hein      (1000)      866 2021-11-02 21:45:52.000000 chrys-4.0.8/setup.py
+drwxrwxr-x   0 hein      (1000) hein      (1000)        0 2022-01-16 06:55:03.975468 chrys-4.0.9/
+-rw-rw-r--   0 hein      (1000) hein      (1000)     1511 2021-11-02 13:59:00.000000 chrys-4.0.9/LICENSE
+-rw-rw-r--   0 hein      (1000) hein      (1000)     2164 2022-01-16 06:55:03.975468 chrys-4.0.9/PKG-INFO
+-rw-rw-r--   0 hein      (1000) hein      (1000)     1125 2021-11-02 13:59:00.000000 chrys-4.0.9/README.md
+drwxrwxr-x   0 hein      (1000) hein      (1000)        0 2022-01-16 06:55:03.975468 chrys-4.0.9/chrys/
+-rw-rw-r--   0 hein      (1000) hein      (1000)       15 2021-11-02 13:59:00.000000 chrys-4.0.9/chrys/__init__.py
+drwxrwxr-x   0 hein      (1000) hein      (1000)        0 2022-01-16 06:55:03.975468 chrys-4.0.9/chrys/data/
+-rw-rw-r--   0 hein      (1000) hein      (1000)        0 2021-11-02 13:59:00.000000 chrys-4.0.9/chrys/data/__init__.py
+-rw-rw-r--   0 hein      (1000) hein      (1000)    92457 2022-01-16 06:54:34.000000 chrys-4.0.9/chrys/data/bokeh_palettes.py
+-rw-rw-r--   0 hein      (1000) hein      (1000)   120856 2022-01-16 06:54:34.000000 chrys-4.0.9/chrys/data/vega_palettes.py
+-rw-rw-r--   0 hein      (1000) hein      (1000)     9909 2021-11-02 13:59:00.000000 chrys-4.0.9/chrys/palettes.py
+-rw-rw-r--   0 hein      (1000) hein      (1000)     1167 2021-11-02 13:59:00.000000 chrys-4.0.9/chrys/utils.py
+drwxrwxr-x   0 hein      (1000) hein      (1000)        0 2022-01-16 06:55:03.975468 chrys-4.0.9/chrys.egg-info/
+-rw-rw-r--   0 hein      (1000) hein      (1000)     2164 2022-01-16 06:55:03.000000 chrys-4.0.9/chrys.egg-info/PKG-INFO
+-rw-rw-r--   0 hein      (1000) hein      (1000)      311 2022-01-16 06:55:03.000000 chrys-4.0.9/chrys.egg-info/SOURCES.txt
+-rw-rw-r--   0 hein      (1000) hein      (1000)        1 2022-01-16 06:55:03.000000 chrys-4.0.9/chrys.egg-info/dependency_links.txt
+-rw-rw-r--   0 hein      (1000) hein      (1000)       86 2022-01-16 06:55:03.000000 chrys-4.0.9/chrys.egg-info/requires.txt
+-rw-rw-r--   0 hein      (1000) hein      (1000)        6 2022-01-16 06:55:03.000000 chrys-4.0.9/chrys.egg-info/top_level.txt
+-rw-rw-r--   0 hein      (1000) hein      (1000)       99 2022-01-16 06:55:03.975468 chrys-4.0.9/setup.cfg
+-rw-rw-r--   0 hein      (1000) hein      (1000)      866 2022-01-16 06:53:58.000000 chrys-4.0.9/setup.py
```

### Comparing `chrys-4.0.8/LICENSE` & `chrys-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chrys-4.0.8/PKG-INFO` & `chrys-4.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrys
-Version: 4.0.8
+Version: 4.0.9
 Summary: A collection of color palettes for mapping and visualisation
 Home-page: https://github.com/netbek/chrys
 Author: Hein Bekker
 Author-email: hein@netbek.co.za
 License: BSD-3-Clause
 Description: # chrys
```

### Comparing `chrys-4.0.8/README.md` & `chrys-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `chrys-4.0.8/chrys/data/bokeh_palettes.py` & `chrys-4.0.9/chrys/data/bokeh_palettes.py`

 * *Files identical despite different names*

### Comparing `chrys-4.0.8/chrys/data/vega_palettes.py` & `chrys-4.0.9/chrys/data/vega_palettes.py`

 * *Files identical despite different names*

### Comparing `chrys-4.0.8/chrys/palettes.py` & `chrys-4.0.9/chrys/palettes.py`

 * *Files identical despite different names*

### Comparing `chrys-4.0.8/chrys/utils.py` & `chrys-4.0.9/chrys/utils.py`

 * *Files identical despite different names*

### Comparing `chrys-4.0.8/chrys.egg-info/PKG-INFO` & `chrys-4.0.9/chrys.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrys
-Version: 4.0.8
+Version: 4.0.9
 Summary: A collection of color palettes for mapping and visualisation
 Home-page: https://github.com/netbek/chrys
 Author: Hein Bekker
 Author-email: hein@netbek.co.za
 License: BSD-3-Clause
 Description: # chrys
```

### Comparing `chrys-4.0.8/setup.py` & `chrys-4.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='chrys',
-    version='4.0.8',
+    version='4.0.9',
     author='Hein Bekker',
     author_email='hein@netbek.co.za',
     description='A collection of color palettes for mapping and visualisation',
     long_description=long_description,
     long_description_content_type='text/markdown',
     license='BSD-3-Clause',
     url='https://github.com/netbek/chrys',
```


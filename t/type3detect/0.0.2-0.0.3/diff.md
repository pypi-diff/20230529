# Comparing `tmp/type3detect-0.0.2.tar.gz` & `tmp/type3detect-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "type3detect-0.0.2.tar", last modified: Mon May 29 13:18:57 2023, max compression
+gzip compressed data, was "type3detect-0.0.3.tar", last modified: Mon May 29 13:30:23 2023, max compression
```

## Comparing `type3detect-0.0.2.tar` & `type3detect-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 peijinzh (504179704) ATKK\hyad-all (984178727)        0 2023-05-29 13:18:57.714900 type3detect-0.0.2/
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     3853 2023-05-29 13:18:57.714232 type3detect-0.0.2/PKG-INFO
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       38 2023-05-29 13:18:57.715046 type3detect-0.0.2/setup.cfg
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     1930 2023-05-29 13:16:38.000000 type3detect-0.0.2/setup.py
-drwxr-xr-x   0 peijinzh (504179704) ATKK\hyad-all (984178727)        0 2023-05-29 13:18:57.708742 type3detect-0.0.2/type3detect/
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     2975 2023-05-29 13:02:56.000000 type3detect-0.0.2/type3detect/ACBone.py
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       87 2023-05-29 13:02:56.000000 type3detect-0.0.2/type3detect/__init__.py
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     5905 2023-05-29 13:02:56.000000 type3detect-0.0.2/type3detect/detectRadioburst.py
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     1940 2023-05-29 13:02:56.000000 type3detect-0.0.2/type3detect/radioTools.py
-drwxr-xr-x   0 peijinzh (504179704) ATKK\hyad-all (984178727)        0 2023-05-29 13:18:57.713221 type3detect-0.0.2/type3detect.egg-info/
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     3853 2023-05-29 13:18:57.000000 type3detect-0.0.2/type3detect.egg-info/PKG-INFO
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)      286 2023-05-29 13:18:57.000000 type3detect-0.0.2/type3detect.egg-info/SOURCES.txt
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)        1 2023-05-29 13:18:57.000000 type3detect-0.0.2/type3detect.egg-info/dependency_links.txt
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       42 2023-05-29 13:18:57.000000 type3detect-0.0.2/type3detect.egg-info/requires.txt
--rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       12 2023-05-29 13:18:57.000000 type3detect-0.0.2/type3detect.egg-info/top_level.txt
+drwxr-xr-x   0 peijinzh (504179704) ATKK\hyad-all (984178727)        0 2023-05-29 13:30:23.361129 type3detect-0.0.3/
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     3853 2023-05-29 13:30:23.358690 type3detect-0.0.3/PKG-INFO
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     3241 2023-05-29 13:27:42.000000 type3detect-0.0.3/README.md
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       38 2023-05-29 13:30:23.361385 type3detect-0.0.3/setup.cfg
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     1832 2023-05-29 13:30:15.000000 type3detect-0.0.3/setup.py
+drwxr-xr-x   0 peijinzh (504179704) ATKK\hyad-all (984178727)        0 2023-05-29 13:30:23.353471 type3detect-0.0.3/type3detect/
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     2975 2023-05-29 13:02:56.000000 type3detect-0.0.3/type3detect/ACBone.py
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       87 2023-05-29 13:02:56.000000 type3detect-0.0.3/type3detect/__init__.py
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     5905 2023-05-29 13:02:56.000000 type3detect-0.0.3/type3detect/detectRadioburst.py
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     1940 2023-05-29 13:02:56.000000 type3detect-0.0.3/type3detect/radioTools.py
+drwxr-xr-x   0 peijinzh (504179704) ATKK\hyad-all (984178727)        0 2023-05-29 13:30:23.357755 type3detect-0.0.3/type3detect.egg-info/
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)     3853 2023-05-29 13:30:23.000000 type3detect-0.0.3/type3detect.egg-info/PKG-INFO
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)      296 2023-05-29 13:30:23.000000 type3detect-0.0.3/type3detect.egg-info/SOURCES.txt
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)        1 2023-05-29 13:30:23.000000 type3detect-0.0.3/type3detect.egg-info/dependency_links.txt
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       42 2023-05-29 13:30:23.000000 type3detect-0.0.3/type3detect.egg-info/requires.txt
+-rw-r--r--   0 peijinzh (504179704) ATKK\hyad-all (984178727)       12 2023-05-29 13:30:23.000000 type3detect-0.0.3/type3detect.egg-info/top_level.txt
```

### Comparing `type3detect-0.0.2/PKG-INFO` & `type3detect-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: type3detect
-Version: 0.0.2
+Version: 0.0.3
 Summary: tools to process the lofar solar data
 Home-page: https://github.com/peijin94/type3detect
 Download-URL: https://github.com/peijin94/type3detect/archive/refs/heads/master.zip
 Author: Peijin
 Author-email: pjer1316@gmail.com
 License: MIT
 Keywords: LOFAR,Solar,radio
```

### Comparing `type3detect-0.0.2/setup.py` & `type3detect-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #from distutils.core import setup
 import setuptools
 from setuptools import setup
 from os import path
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory,'../..','README.md'), encoding='utf-8') as f:
-    long_description = f.read()
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
 
 setup(
   name = 'type3detect',         # How you named your package folder 
   packages = setuptools.find_packages(),#['lofarSun','lofarSun.IM','lofarSun.BF','lofarSun.BF.GUI'],   # Chose the same as "name"
   include_package_data=True,
-  version = '0.0.2',      # Start with a small number and increase it with every change you make
+  version = '0.0.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'tools to process the lofar solar data',   # Give a short description about your library
   author = 'Peijin',                   # Type in your name
   author_email = 'pjer1316@gmail.com',      # Type in your E-Mail
   url = 'https://github.com/peijin94/type3detect',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/peijin94/type3detect/archive/refs/heads/master.zip',    
   keywords = ['LOFAR', 'Solar', 'radio'],   # Keywords that define your package best
```

### Comparing `type3detect-0.0.2/type3detect/ACBone.py` & `type3detect-0.0.3/type3detect/ACBone.py`

 * *Files identical despite different names*

### Comparing `type3detect-0.0.2/type3detect/detectRadioburst.py` & `type3detect-0.0.3/type3detect/detectRadioburst.py`

 * *Files identical despite different names*

### Comparing `type3detect-0.0.2/type3detect/radioTools.py` & `type3detect-0.0.3/type3detect/radioTools.py`

 * *Files identical despite different names*

### Comparing `type3detect-0.0.2/type3detect.egg-info/PKG-INFO` & `type3detect-0.0.3/type3detect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: type3detect
-Version: 0.0.2
+Version: 0.0.3
 Summary: tools to process the lofar solar data
 Home-page: https://github.com/peijin94/type3detect
 Download-URL: https://github.com/peijin94/type3detect/archive/refs/heads/master.zip
 Author: Peijin
 Author-email: pjer1316@gmail.com
 License: MIT
 Keywords: LOFAR,Solar,radio
```


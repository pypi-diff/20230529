# Comparing `tmp/flake8_iw-0.0.8.tar.gz` & `tmp/flake8_iw-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flake8_iw-0.0.8.tar", last modified: Tue Dec 13 12:41:58 2022, max compression
+gzip compressed data, was "flake8_iw-0.0.9.tar", last modified: Tue Dec 13 15:50:48 2022, max compression
```

## Comparing `flake8_iw-0.0.8.tar` & `flake8_iw-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 smit       (502) staff       (20)        0 2022-12-13 12:41:58.431868 flake8_iw-0.0.8/
--rw-r--r--   0 smit       (502) staff       (20)       30 2022-11-03 11:15:20.000000 flake8_iw-0.0.8/MANIFEST.in
--rw-r--r--   0 smit       (502) staff       (20)     3232 2022-12-13 12:41:58.431966 flake8_iw-0.0.8/PKG-INFO
--rw-r--r--   0 smit       (502) staff       (20)     2671 2022-12-13 12:08:51.000000 flake8_iw-0.0.8/README.md
-drwxr-xr-x   0 smit       (502) staff       (20)        0 2022-12-13 12:41:58.431621 flake8_iw-0.0.8/flake8_iw.egg-info/
--rw-r--r--   0 smit       (502) staff       (20)     3232 2022-12-13 12:41:58.000000 flake8_iw-0.0.8/flake8_iw.egg-info/PKG-INFO
--rw-r--r--   0 smit       (502) staff       (20)      255 2022-12-13 12:41:58.000000 flake8_iw-0.0.8/flake8_iw.egg-info/SOURCES.txt
--rw-r--r--   0 smit       (502) staff       (20)        1 2022-12-13 12:41:58.000000 flake8_iw-0.0.8/flake8_iw.egg-info/dependency_links.txt
--rw-r--r--   0 smit       (502) staff       (20)       41 2022-12-13 12:41:58.000000 flake8_iw-0.0.8/flake8_iw.egg-info/entry_points.txt
--rw-r--r--   0 smit       (502) staff       (20)       56 2022-12-13 12:41:58.000000 flake8_iw-0.0.8/flake8_iw.egg-info/requires.txt
--rw-r--r--   0 smit       (502) staff       (20)       10 2022-12-13 12:41:58.000000 flake8_iw-0.0.8/flake8_iw.egg-info/top_level.txt
--rw-r--r--   0 smit       (502) staff       (20)       85 2022-11-03 14:16:42.000000 flake8_iw-0.0.8/pyproject.toml
--rw-r--r--   0 smit       (502) staff       (20)      219 2022-12-13 12:41:58.432400 flake8_iw-0.0.8/setup.cfg
--rw-r--r--   0 smit       (502) staff       (20)     1060 2022-12-13 12:41:33.000000 flake8_iw-0.0.8/setup.py
+drwxr-xr-x   0 smit       (502) staff       (20)        0 2022-12-13 15:50:48.377566 flake8_iw-0.0.9/
+-rw-r--r--   0 smit       (502) staff       (20)       78 2022-12-13 15:49:29.000000 flake8_iw-0.0.9/MANIFEST.in
+-rw-r--r--   0 smit       (502) staff       (20)     3232 2022-12-13 15:50:48.377714 flake8_iw-0.0.9/PKG-INFO
+-rw-r--r--   0 smit       (502) staff       (20)     2671 2022-12-13 12:08:51.000000 flake8_iw-0.0.9/README.md
+drwxr-xr-x   0 smit       (502) staff       (20)        0 2022-12-13 15:50:48.373916 flake8_iw-0.0.9/flake8_iw/
+-rw-r--r--   0 smit       (502) staff       (20)       43 2022-12-13 12:08:35.000000 flake8_iw-0.0.9/flake8_iw/__init__.py
+-rw-r--r--   0 smit       (502) staff       (20)     1102 2022-12-13 12:25:35.000000 flake8_iw-0.0.9/flake8_iw/freeze_time.py
+-rw-r--r--   0 smit       (502) staff       (20)     5199 2022-12-13 12:08:35.000000 flake8_iw-0.0.9/flake8_iw/patch_call.py
+-rw-r--r--   0 smit       (502) staff       (20)      776 2022-12-13 12:08:51.000000 flake8_iw-0.0.9/flake8_iw/plugin.py
+drwxr-xr-x   0 smit       (502) staff       (20)        0 2022-12-13 15:50:48.377196 flake8_iw-0.0.9/flake8_iw.egg-info/
+-rw-r--r--   0 smit       (502) staff       (20)     3232 2022-12-13 15:50:48.000000 flake8_iw-0.0.9/flake8_iw.egg-info/PKG-INFO
+-rw-r--r--   0 smit       (502) staff       (20)      346 2022-12-13 15:50:48.000000 flake8_iw-0.0.9/flake8_iw.egg-info/SOURCES.txt
+-rw-r--r--   0 smit       (502) staff       (20)        1 2022-12-13 15:50:48.000000 flake8_iw-0.0.9/flake8_iw.egg-info/dependency_links.txt
+-rw-r--r--   0 smit       (502) staff       (20)       41 2022-12-13 15:50:48.000000 flake8_iw-0.0.9/flake8_iw.egg-info/entry_points.txt
+-rw-r--r--   0 smit       (502) staff       (20)       56 2022-12-13 15:50:48.000000 flake8_iw-0.0.9/flake8_iw.egg-info/requires.txt
+-rw-r--r--   0 smit       (502) staff       (20)       10 2022-12-13 15:50:48.000000 flake8_iw-0.0.9/flake8_iw.egg-info/top_level.txt
+-rw-r--r--   0 smit       (502) staff       (20)       85 2022-11-03 14:16:42.000000 flake8_iw-0.0.9/pyproject.toml
+-rw-r--r--   0 smit       (502) staff       (20)      219 2022-12-13 15:50:48.378371 flake8_iw-0.0.9/setup.cfg
+-rw-r--r--   0 smit       (502) staff       (20)     1060 2022-12-13 15:50:34.000000 flake8_iw-0.0.9/setup.py
```

### Comparing `flake8_iw-0.0.8/PKG-INFO` & `flake8_iw-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8_iw
-Version: 0.0.8
+Version: 0.0.9
 Summary: A plugin to show lint errors for IW
 Home-page: http://github.com/Instawork/flake8-iw
 Author: Smit
 Author-email: smitpatel@instawork.com
 License: MIT
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
```

### Comparing `flake8_iw-0.0.8/README.md` & `flake8_iw-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `flake8_iw-0.0.8/flake8_iw.egg-info/PKG-INFO` & `flake8_iw-0.0.9/flake8_iw.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flake8-iw
-Version: 0.0.8
+Version: 0.0.9
 Summary: A plugin to show lint errors for IW
 Home-page: http://github.com/Instawork/flake8-iw
 Author: Smit
 Author-email: smitpatel@instawork.com
 License: MIT
 Classifier: Framework :: Flake8
 Classifier: Intended Audience :: Developers
```

### Comparing `flake8_iw-0.0.8/setup.py` & `flake8_iw-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 readme = open('README.md').read()
 
 setuptools.setup(
     name='flake8_iw',
     license='MIT',
-    version='0.0.8',
+    version='0.0.9',
     description='A plugin to show lint errors for IW',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='Smit',
     author_email='smitpatel@instawork.com',
     url='http://github.com/Instawork/flake8-iw',
     py_modules=['flake8_iw'],
```


# Comparing `tmp/e2enetworks-0.0.8.tar.gz` & `tmp/e2enetworks-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2enetworks-0.0.8.tar", last modified: Tue May 16 10:30:51 2023, max compression
+gzip compressed data, was "e2enetworks-0.0.9.tar", last modified: Tue May 16 10:51:26 2023, max compression
```

## Comparing `e2enetworks-0.0.8.tar` & `e2enetworks-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:30:51.243261 e2enetworks-0.0.8/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.8/LICENSE.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-16 10:30:51.243338 e2enetworks-0.0.8/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.8/README.rst
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:30:51.240954 e2enetworks-0.0.8/e2enetworks/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.8/e2enetworks/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:30:51.241750 e2enetworks-0.0.8/e2enetworks/cloud/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.8/e2enetworks/cloud/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:30:51.242266 e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:30:51.242569 e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/Dataset/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      838 2023-05-16 09:50:41.000000 e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/Dataset/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:30:51.242803 e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/EndPoint/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      290 2023-05-16 06:13:24.000000 e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/EndPoint/__init__.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:30:51.243044 e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/Model/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     2149 2023-05-16 10:14:22.000000 e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/Model/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      220 2023-05-16 06:52:59.000000 e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/__init__.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      275 2023-05-16 06:15:26.000000 e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/init.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 07:31:42.000000 e2enetworks-0.0.8/e2enetworks/cloud/test.py
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      137 2023-05-16 09:55:48.000000 e2enetworks-0.0.8/e2enetworks/constants.py
-drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:30:51.241544 e2enetworks-0.0.8/e2enetworks.egg-info/
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-16 10:30:50.000000 e2enetworks-0.0.8/e2enetworks.egg-info/PKG-INFO
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)      510 2023-05-16 10:30:51.000000 e2enetworks-0.0.8/e2enetworks.egg-info/SOURCES.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-16 10:30:50.000000 e2enetworks-0.0.8/e2enetworks.egg-info/dependency_links.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-16 10:30:51.000000 e2enetworks-0.0.8/e2enetworks.egg-info/top_level.txt
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-16 10:30:51.243576 e2enetworks-0.0.8/setup.cfg
--rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-16 10:30:15.000000 e2enetworks-0.0.8/setup.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.069581 e2enetworks-0.0.9/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)    10786 2023-05-15 06:38:48.000000 e2enetworks-0.0.9/LICENSE.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-16 10:51:26.069665 e2enetworks-0.0.9/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     4748 2023-05-15 07:01:23.000000 e2enetworks-0.0.9/README.rst
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.067012 e2enetworks-0.0.9/e2enetworks/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.9/e2enetworks/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.067991 e2enetworks-0.0.9/e2enetworks/cloud/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        0 2023-05-15 07:31:42.000000 e2enetworks-0.0.9/e2enetworks/cloud/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.068579 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.068836 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/Dataset/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      838 2023-05-16 09:50:41.000000 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/Dataset/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.069077 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/EndPoint/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      290 2023-05-16 06:13:24.000000 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/EndPoint/__init__.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.069336 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/Model/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     2149 2023-05-16 10:14:22.000000 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/Model/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      220 2023-05-16 06:52:59.000000 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/__init__.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      275 2023-05-16 06:15:26.000000 e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/init.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      147 2023-05-15 07:31:42.000000 e2enetworks-0.0.9/e2enetworks/cloud/test.py
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      137 2023-05-16 09:55:48.000000 e2enetworks-0.0.9/e2enetworks/constants.py
+drwxr-xr-x   0 dhananjaysingh   (501) staff       (20)        0 2023-05-16 10:51:26.067748 e2enetworks-0.0.9/e2enetworks.egg-info/
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     5929 2023-05-16 10:51:25.000000 e2enetworks-0.0.9/e2enetworks.egg-info/PKG-INFO
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)      510 2023-05-16 10:51:26.000000 e2enetworks-0.0.9/e2enetworks.egg-info/SOURCES.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)        1 2023-05-16 10:51:25.000000 e2enetworks-0.0.9/e2enetworks.egg-info/dependency_links.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       12 2023-05-16 10:51:25.000000 e2enetworks-0.0.9/e2enetworks.egg-info/top_level.txt
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)       67 2023-05-16 10:51:26.069917 e2enetworks-0.0.9/setup.cfg
+-rw-r--r--   0 dhananjaysingh   (501) staff       (20)     1833 2023-05-16 10:51:06.000000 e2enetworks-0.0.9/setup.py
```

### Comparing `e2enetworks-0.0.8/LICENSE.txt` & `e2enetworks-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.8/PKG-INFO` & `e2enetworks-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.8
+Version: 0.0.9
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `e2enetworks-0.0.8/README.rst` & `e2enetworks-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/Dataset/__init__.py` & `e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/Dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.8/e2enetworks/cloud/aiplatform/Model/__init__.py` & `e2enetworks-0.0.9/e2enetworks/cloud/aiplatform/Model/__init__.py`

 * *Files identical despite different names*

### Comparing `e2enetworks-0.0.8/e2enetworks.egg-info/PKG-INFO` & `e2enetworks-0.0.9/e2enetworks.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2enetworks
-Version: 0.0.8
+Version: 0.0.9
 Summary: E2E Networks Plugins
 Author: Dhananjay Singh
 Author-email: djs091298@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
```

### Comparing `e2enetworks-0.0.8/setup.py` & `e2enetworks-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 from setuptools import find_packages
 from os import path
 
-version = "0.0.8"
+version = "0.0.9"
 install_requires = [
 
 ]
 # read the contents of your README file
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.rst")) as f:
```


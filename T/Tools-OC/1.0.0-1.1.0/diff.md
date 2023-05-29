# Comparing `tmp/Tools-OC-1.0.0.tar.gz` & `tmp/Tools-OC-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Tools-OC-1.0.0.tar", last modified: Sat Mar 18 21:13:36 2023, max compression
+gzip compressed data, was "Tools-OC-1.1.0.tar", last modified: Mon May 29 10:55:59 2023, max compression
```

## Comparing `Tools-OC-1.0.0.tar` & `Tools-OC-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-18 21:13:36.758369 Tools-OC-1.0.0/
--rw-rw-r--   0 bast      (1002) bast      (1002)     1078 2023-03-18 20:50:27.000000 Tools-OC-1.0.0/LICENSE
--rw-rw-r--   0 bast      (1002) bast      (1002)      604 2023-03-18 21:13:36.758369 Tools-OC-1.0.0/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)       57 2023-03-18 20:50:27.000000 Tools-OC-1.0.0/README.md
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-18 21:13:36.758369 Tools-OC-1.0.0/Tools_OC.egg-info/
--rw-rw-r--   0 bast      (1002) bast      (1002)      604 2023-03-18 21:13:36.000000 Tools-OC-1.0.0/Tools_OC.egg-info/PKG-INFO
--rw-rw-r--   0 bast      (1002) bast      (1002)      227 2023-03-18 21:13:36.000000 Tools-OC-1.0.0/Tools_OC.egg-info/SOURCES.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-03-18 21:13:36.000000 Tools-OC-1.0.0/Tools_OC.egg-info/dependency_links.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        6 2023-03-18 21:13:36.000000 Tools-OC-1.0.0/Tools_OC.egg-info/top_level.txt
--rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-03-18 21:13:36.000000 Tools-OC-1.0.0/Tools_OC.egg-info/zip-safe
--rw-rw-r--   0 bast      (1002) bast      (1002)       79 2023-03-18 21:13:36.758369 Tools-OC-1.0.0/setup.cfg
--rw-rw-r--   0 bast      (1002) bast      (1002)      707 2023-03-18 20:52:44.000000 Tools-OC-1.0.0/setup.py
-drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-03-18 21:13:36.758369 Tools-OC-1.0.0/tools/
--rw-rw-r--   0 bast      (1002) bast      (1002)     6400 2023-03-18 21:03:01.000000 Tools-OC-1.0.0/tools/__init__.py
--rw-rw-r--   0 bast      (1002) bast      (1002)      529 2023-03-18 21:12:32.000000 Tools-OC-1.0.0/tools/__main__.py
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-29 10:55:59.837903 Tools-OC-1.1.0/
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1078 2023-03-18 20:50:27.000000 Tools-OC-1.1.0/LICENSE
+-rw-rw-r--   0 bast      (1002) bast      (1002)      604 2023-05-29 10:55:59.837903 Tools-OC-1.1.0/PKG-INFO
+-rw-rw-r--   0 bast      (1002) bast      (1002)       57 2023-03-18 20:50:27.000000 Tools-OC-1.1.0/README.md
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-29 10:55:59.837903 Tools-OC-1.1.0/Tools_OC.egg-info/
+-rw-rw-r--   0 bast      (1002) bast      (1002)      604 2023-05-29 10:55:59.000000 Tools-OC-1.1.0/Tools_OC.egg-info/PKG-INFO
+-rw-rw-r--   0 bast      (1002) bast      (1002)      258 2023-05-29 10:55:59.000000 Tools-OC-1.1.0/Tools_OC.egg-info/SOURCES.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-05-29 10:55:59.000000 Tools-OC-1.1.0/Tools_OC.egg-info/dependency_links.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)       20 2023-05-29 10:55:59.000000 Tools-OC-1.1.0/Tools_OC.egg-info/requires.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        6 2023-05-29 10:55:59.000000 Tools-OC-1.1.0/Tools_OC.egg-info/top_level.txt
+-rw-rw-r--   0 bast      (1002) bast      (1002)        1 2023-03-18 21:13:36.000000 Tools-OC-1.1.0/Tools_OC.egg-info/zip-safe
+-rw-rw-r--   0 bast      (1002) bast      (1002)       79 2023-05-29 10:55:59.837903 Tools-OC-1.1.0/setup.cfg
+-rw-rw-r--   0 bast      (1002) bast      (1002)      755 2023-05-29 10:55:32.000000 Tools-OC-1.1.0/setup.py
+drwxrwxr-x   0 bast      (1002) bast      (1002)        0 2023-05-29 10:55:59.837903 Tools-OC-1.1.0/tools/
+-rw-rw-r--   0 bast      (1002) bast      (1002)     9404 2023-05-29 10:55:32.000000 Tools-OC-1.1.0/tools/__init__.py
+-rw-rw-r--   0 bast      (1002) bast      (1002)     1232 2023-05-29 10:55:32.000000 Tools-OC-1.1.0/tools/__main__.py
```

### Comparing `Tools-OC-1.0.0/LICENSE` & `Tools-OC-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Tools-OC-1.0.0/PKG-INFO` & `Tools-OC-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tools-OC
-Version: 1.0.0
+Version: 1.1.0
 Summary: A set of tools for common python problems
 Home-page: https://github.com/ouroboroscoding/tools-python
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: MIT
 Project-URL: Source, https://github.com/ouroboroscoding/tools-python
 Project-URL: Tracker, https://github.com/ouroboroscoding/tools-python/issues
```

### Comparing `Tools-OC-1.0.0/Tools_OC.egg-info/PKG-INFO` & `Tools-OC-1.1.0/Tools_OC.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Tools-OC
-Version: 1.0.0
+Version: 1.1.0
 Summary: A set of tools for common python problems
 Home-page: https://github.com/ouroboroscoding/tools-python
 Author: Chris Nasr - Ouroboros Coding Inc.
 Author-email: chris@ouroboroscoding.com
 License: MIT
 Project-URL: Source, https://github.com/ouroboroscoding/tools-python
 Project-URL: Tracker, https://github.com/ouroboroscoding/tools-python/issues
```

### Comparing `Tools-OC-1.0.0/setup.py` & `Tools-OC-1.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from setuptools import setup
 
 with open('README.md', 'r') as oF:
 	long_description=oF.read()
 
 setup(
 	name='Tools-OC',
-	version='1.0.0',
+	version='1.1.0',
 	description='A set of tools for common python problems',
 	long_description=long_description,
 	long_description_content_type='text/markdown',
 	url='https://github.com/ouroboroscoding/tools-python',
 	project_urls={
 		'Source': 'https://github.com/ouroboroscoding/tools-python',
 		'Tracker': 'https://github.com/ouroboroscoding/tools-python/issues'
 	},
 	keywords=['tools', 'clone', 'merge', 'combine'],
 	author='Chris Nasr - Ouroboros Coding Inc.',
 	author_email='chris@ouroboroscoding.com',
 	license='MIT',
 	packages=['tools'],
 	python_requires='>=3.10',
+	install_requires=[
+		"jobject>=1.0.1,<1.1"
+	],
 	zip_safe=True
 )
```


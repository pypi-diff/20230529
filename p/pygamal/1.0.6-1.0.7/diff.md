# Comparing `tmp/pygamal-1.0.6.tar.gz` & `tmp/pygamal-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygamal-1.0.6.tar", last modified: Sun May 28 00:15:30 2023, max compression
+gzip compressed data, was "pygamal-1.0.7.tar", last modified: Mon May 29 16:24:47 2023, max compression
```

## Comparing `pygamal-1.0.6.tar` & `pygamal-1.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 00:15:30.223206 pygamal-1.0.6/
--rw-rw-rw-   0        0        0      861 2023-05-28 00:15:30.223206 pygamal-1.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 00:15:30.201848 pygamal-1.0.6/pygamal/
--rw-rw-rw-   0        0        0       22 2023-05-28 00:15:11.000000 pygamal-1.0.6/pygamal/__init__.py
--rw-rw-rw-   0        0        0     4308 2023-05-27 23:24:32.000000 pygamal-1.0.6/pygamal/pygamal.py
-drwxrwxrwx   0        0        0        0 2023-05-28 00:15:30.223206 pygamal-1.0.6/pygamal.egg-info/
--rw-rw-rw-   0        0        0      861 2023-05-28 00:15:30.000000 pygamal-1.0.6/pygamal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2023-05-28 00:15:30.000000 pygamal-1.0.6/pygamal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 00:15:30.000000 pygamal-1.0.6/pygamal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-28 00:15:30.000000 pygamal-1.0.6/pygamal.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 00:15:30.000000 pygamal-1.0.6/pygamal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 00:15:30.223206 pygamal-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1126 2023-05-28 00:15:18.000000 pygamal-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:24:47.993203 pygamal-1.0.7/
+-rw-rw-rw-   0        0        0      861 2023-05-29 16:24:47.993203 pygamal-1.0.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-29 16:24:47.983279 pygamal-1.0.7/pygamal/
+-rw-rw-rw-   0        0        0       22 2023-05-28 00:15:11.000000 pygamal-1.0.7/pygamal/__init__.py
+-rw-rw-rw-   0        0        0     4308 2023-05-27 23:24:32.000000 pygamal-1.0.7/pygamal/pygamal.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:24:47.993203 pygamal-1.0.7/pygamal.egg-info/
+-rw-rw-rw-   0        0        0      861 2023-05-29 16:24:47.000000 pygamal-1.0.7/pygamal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2023-05-29 16:24:47.000000 pygamal-1.0.7/pygamal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 16:24:47.000000 pygamal-1.0.7/pygamal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-29 16:24:47.000000 pygamal-1.0.7/pygamal.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-29 16:24:47.000000 pygamal-1.0.7/pygamal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 16:24:47.993203 pygamal-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1126 2023-05-29 16:19:54.000000 pygamal-1.0.7/setup.py
```

### Comparing `pygamal-1.0.6/PKG-INFO` & `pygamal-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygamal
-Version: 1.0.6
+Version: 1.0.7
 Summary: This module is for csc281 encryption project 
 Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pygamal-1.0.6/pygamal/pygamal.py` & `pygamal-1.0.7/pygamal/pygamal.py`

 * *Files identical despite different names*

### Comparing `pygamal-1.0.6/pygamal.egg-info/PKG-INFO` & `pygamal-1.0.7/pygamal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygamal
-Version: 1.0.6
+Version: 1.0.7
 Summary: This module is for csc281 encryption project 
 Home-page: https://github.com/Wouze/csc281-project
 Author: Wouze (Mohammad)
 Author-email: m7mdwats1@hotmail.com
 Keywords: python,c,primitive root,encryption,algamal,prime
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```

### Comparing `pygamal-1.0.6/setup.py` & `pygamal-1.0.7/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 """
 This module have been made for the project of discret math CSC281 at ksu university.
 The project supervisor is Aqil Alazimi. LinkedIn: https://www.linkedin.com/in/aqil-azmi-20903960/
 The project repo is: https://github.com/Wouze/csc281-project
 """
 
 setup(name="pygamal",
-      version="1.0.6",
+      version="1.0.7",
       author="Wouze (Mohammad)",
       author_email="m7mdwats1@hotmail.com",
       description="This module is for csc281 encryption project ",
       long_description_content_type="text/markdown",
       long_description=long_description,
       url='https://github.com/Wouze/csc281-project',
       keywords=['python', 'c', 'primitive root', 'encryption', 'algamal', 'prime'],
-      install_requires=["ElGamal-c==1.0.1"],
+      install_requires=["ElGamal-c==2.0.1"],
       classifiers=[
             "Development Status :: 1 - Planning",
             "Intended Audience :: Developers",
             "Programming Language :: Python :: 3",
             "Operating System :: Unix",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
```


# Comparing `tmp/trainkit-0.0.1.tar.gz` & `tmp/trainkit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trainkit-0.0.1.tar", last modified: Mon May 29 19:43:29 2023, max compression
+gzip compressed data, was "trainkit-0.0.2.tar", last modified: Mon May 29 19:58:28 2023, max compression
```

## Comparing `trainkit-0.0.1.tar` & `trainkit-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 enrique    (501) staff       (20)        0 2023-05-29 19:43:29.100357 trainkit-0.0.1/
--rw-r--r--   0 enrique    (501) staff       (20)     1036 2023-05-29 17:30:40.000000 trainkit-0.0.1/LICENSE.md
--rw-r--r--   0 enrique    (501) staff       (20)      191 2023-05-29 19:43:29.100252 trainkit-0.0.1/PKG-INFO
--rw-r--r--   0 enrique    (501) staff       (20)      483 2023-05-29 18:48:16.000000 trainkit-0.0.1/README.md
-drwxr-xr-x   0 enrique    (501) staff       (20)        0 2023-05-29 19:43:29.099473 trainkit-0.0.1/models/
--rw-r--r--   0 enrique    (501) staff       (20)     2898 2023-05-29 19:04:07.000000 trainkit-0.0.1/models/FullyConnected.py
--rw-r--r--   0 enrique    (501) staff       (20)        0 2023-05-29 18:52:52.000000 trainkit-0.0.1/models/__init__.py
--rw-r--r--   0 enrique    (501) staff       (20)       38 2023-05-29 19:43:29.100402 trainkit-0.0.1/setup.cfg
--rw-r--r--   0 enrique    (501) staff       (20)      309 2023-05-29 19:04:06.000000 trainkit-0.0.1/setup.py
-drwxr-xr-x   0 enrique    (501) staff       (20)        0 2023-05-29 19:43:29.100085 trainkit-0.0.1/trainkit.egg-info/
--rw-r--r--   0 enrique    (501) staff       (20)      191 2023-05-29 19:43:29.000000 trainkit-0.0.1/trainkit.egg-info/PKG-INFO
--rw-r--r--   0 enrique    (501) staff       (20)      232 2023-05-29 19:43:29.000000 trainkit-0.0.1/trainkit.egg-info/SOURCES.txt
--rw-r--r--   0 enrique    (501) staff       (20)        1 2023-05-29 19:43:29.000000 trainkit-0.0.1/trainkit.egg-info/dependency_links.txt
--rw-r--r--   0 enrique    (501) staff       (20)        6 2023-05-29 19:43:29.000000 trainkit-0.0.1/trainkit.egg-info/requires.txt
--rw-r--r--   0 enrique    (501) staff       (20)        7 2023-05-29 19:43:29.000000 trainkit-0.0.1/trainkit.egg-info/top_level.txt
+drwxr-xr-x   0 enrique    (501) staff       (20)        0 2023-05-29 19:58:28.859248 trainkit-0.0.2/
+-rw-r--r--   0 enrique    (501) staff       (20)     1036 2023-05-29 17:30:40.000000 trainkit-0.0.2/LICENSE.md
+-rw-r--r--   0 enrique    (501) staff       (20)      731 2023-05-29 19:58:28.859131 trainkit-0.0.2/PKG-INFO
+-rw-r--r--   0 enrique    (501) staff       (20)      483 2023-05-29 18:48:16.000000 trainkit-0.0.2/README.md
+drwxr-xr-x   0 enrique    (501) staff       (20)        0 2023-05-29 19:58:28.858339 trainkit-0.0.2/models/
+-rw-r--r--   0 enrique    (501) staff       (20)     2898 2023-05-29 19:04:07.000000 trainkit-0.0.2/models/FullyConnected.py
+-rw-r--r--   0 enrique    (501) staff       (20)        0 2023-05-29 18:52:52.000000 trainkit-0.0.2/models/__init__.py
+-rw-r--r--   0 enrique    (501) staff       (20)       38 2023-05-29 19:58:28.859297 trainkit-0.0.2/setup.cfg
+-rw-r--r--   0 enrique    (501) staff       (20)      471 2023-05-29 19:57:49.000000 trainkit-0.0.2/setup.py
+drwxr-xr-x   0 enrique    (501) staff       (20)        0 2023-05-29 19:58:28.858954 trainkit-0.0.2/trainkit.egg-info/
+-rw-r--r--   0 enrique    (501) staff       (20)      731 2023-05-29 19:58:28.000000 trainkit-0.0.2/trainkit.egg-info/PKG-INFO
+-rw-r--r--   0 enrique    (501) staff       (20)      232 2023-05-29 19:58:28.000000 trainkit-0.0.2/trainkit.egg-info/SOURCES.txt
+-rw-r--r--   0 enrique    (501) staff       (20)        1 2023-05-29 19:58:28.000000 trainkit-0.0.2/trainkit.egg-info/dependency_links.txt
+-rw-r--r--   0 enrique    (501) staff       (20)        6 2023-05-29 19:58:28.000000 trainkit-0.0.2/trainkit.egg-info/requires.txt
+-rw-r--r--   0 enrique    (501) staff       (20)        7 2023-05-29 19:58:28.000000 trainkit-0.0.2/trainkit.egg-info/top_level.txt
```

### Comparing `trainkit-0.0.1/LICENSE.md` & `trainkit-0.0.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `trainkit-0.0.1/models/FullyConnected.py` & `trainkit-0.0.2/models/FullyConnected.py`

 * *Files identical despite different names*


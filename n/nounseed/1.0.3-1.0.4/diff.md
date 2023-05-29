# Comparing `tmp/nounseed-1.0.3.tar.gz` & `tmp/nounseed-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nounseed-1.0.3.tar", last modified: Mon May 29 00:49:40 2023, max compression
+gzip compressed data, was "nounseed-1.0.4.tar", last modified: Mon May 29 00:52:14 2023, max compression
```

## Comparing `nounseed-1.0.3.tar` & `nounseed-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-29 00:49:40.222531 nounseed-1.0.3/
--rw-r--r--   0 bloom      (501) staff       (20)     1074 2023-05-23 23:15:34.000000 nounseed-1.0.3/LICENSE
--rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-29 00:49:40.222386 nounseed-1.0.3/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)     2626 2023-05-29 00:48:40.000000 nounseed-1.0.3/README
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-29 00:49:40.221650 nounseed-1.0.3/nounseed/
--rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 00:19:28.000000 nounseed-1.0.3/nounseed/__init__.py
--rw-r--r--   0 bloom      (501) staff       (20)     4970 2023-05-29 00:44:03.000000 nounseed-1.0.3/nounseed/__main__.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-29 00:49:40.222253 nounseed-1.0.3/nounseed.egg-info/
--rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)      274 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/SOURCES.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/dependency_links.txt
--rw-r--r--   0 bloom      (501) staff       (20)       53 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/entry_points.txt
--rw-r--r--   0 bloom      (501) staff       (20)       17 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/requires.txt
--rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-29 00:49:40.000000 nounseed-1.0.3/nounseed.egg-info/top_level.txt
--rw-r--r--   0 bloom      (501) staff       (20)       90 2023-05-28 22:55:02.000000 nounseed-1.0.3/pyproject.toml
--rw-r--r--   0 bloom      (501) staff       (20)       38 2023-05-29 00:49:40.222585 nounseed-1.0.3/setup.cfg
--rw-r--r--   0 bloom      (501) staff       (20)      379 2023-05-29 00:49:11.000000 nounseed-1.0.3/setup.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-29 00:52:14.435316 nounseed-1.0.4/
+-rw-r--r--   0 bloom      (501) staff       (20)     1074 2023-05-23 23:15:34.000000 nounseed-1.0.4/LICENSE
+-rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-29 00:52:14.435194 nounseed-1.0.4/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)     2626 2023-05-29 00:48:40.000000 nounseed-1.0.4/README
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-29 00:52:14.434427 nounseed-1.0.4/nounseed/
+-rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 00:19:28.000000 nounseed-1.0.4/nounseed/__init__.py
+-rw-r--r--   0 bloom      (501) staff       (20)     4970 2023-05-29 00:44:03.000000 nounseed-1.0.4/nounseed/__main__.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-29 00:52:14.435014 nounseed-1.0.4/nounseed.egg-info/
+-rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-29 00:52:14.000000 nounseed-1.0.4/nounseed.egg-info/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)      274 2023-05-29 00:52:14.000000 nounseed-1.0.4/nounseed.egg-info/SOURCES.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-29 00:52:14.000000 nounseed-1.0.4/nounseed.egg-info/dependency_links.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       53 2023-05-29 00:52:14.000000 nounseed-1.0.4/nounseed.egg-info/entry_points.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       17 2023-05-29 00:52:14.000000 nounseed-1.0.4/nounseed.egg-info/requires.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-29 00:52:14.000000 nounseed-1.0.4/nounseed.egg-info/top_level.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       90 2023-05-28 22:55:02.000000 nounseed-1.0.4/pyproject.toml
+-rw-r--r--   0 bloom      (501) staff       (20)       38 2023-05-29 00:52:14.435350 nounseed-1.0.4/setup.cfg
+-rw-r--r--   0 bloom      (501) staff       (20)      379 2023-05-29 00:51:57.000000 nounseed-1.0.4/setup.py
```

### Comparing `nounseed-1.0.3/LICENSE` & `nounseed-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nounseed-1.0.3/README` & `nounseed-1.0.4/README`

 * *Files identical despite different names*

### Comparing `nounseed-1.0.3/nounseed/__main__.py` & `nounseed-1.0.4/nounseed/__main__.py`

 * *Files identical despite different names*


# Comparing `tmp/sqlcrafty-0.0.1.tar.gz` & `tmp/sqlcrafty-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlcrafty-0.0.1.tar", last modified: Mon May 29 11:23:10 2023, max compression
+gzip compressed data, was "sqlcrafty-0.0.2.tar", last modified: Mon May 29 12:12:17 2023, max compression
```

## Comparing `sqlcrafty-0.0.1.tar` & `sqlcrafty-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 richardy  (1000) richardy  (1000)        0 2023-05-29 11:23:10.678842 sqlcrafty-0.0.1/
--rw-rw-r--   0 richardy  (1000) richardy  (1000)      181 2023-05-29 11:23:10.678842 sqlcrafty-0.0.1/PKG-INFO
--rw-rw-r--   0 richardy  (1000) richardy  (1000)       38 2023-05-29 11:23:10.678842 sqlcrafty-0.0.1/setup.cfg
--rw-rw-r--   0 richardy  (1000) richardy  (1000)      237 2023-05-29 11:20:43.000000 sqlcrafty-0.0.1/setup.py
-drwxrwxr-x   0 richardy  (1000) richardy  (1000)        0 2023-05-29 11:23:10.674842 sqlcrafty-0.0.1/sqlcrafty/
--rw-rw-r--   0 richardy  (1000) richardy  (1000)        0 2023-05-24 01:51:03.000000 sqlcrafty-0.0.1/sqlcrafty/__init__.py
--rw-rw-r--   0 richardy  (1000) richardy  (1000)     5004 2023-05-29 01:29:43.000000 sqlcrafty-0.0.1/sqlcrafty/functions.py
--rw-rw-r--   0 richardy  (1000) richardy  (1000)     7772 2023-05-29 11:09:10.000000 sqlcrafty-0.0.1/sqlcrafty/models.py
--rw-rw-r--   0 richardy  (1000) richardy  (1000)      791 2023-05-29 10:29:14.000000 sqlcrafty-0.0.1/sqlcrafty/sqlcrafty.py
--rw-rw-r--   0 richardy  (1000) richardy  (1000)      135 2023-05-29 02:01:13.000000 sqlcrafty-0.0.1/sqlcrafty/utils.py
-drwxrwxr-x   0 richardy  (1000) richardy  (1000)        0 2023-05-29 11:23:10.678842 sqlcrafty-0.0.1/sqlcrafty.egg-info/
--rw-rw-r--   0 richardy  (1000) richardy  (1000)      181 2023-05-29 11:23:10.000000 sqlcrafty-0.0.1/sqlcrafty.egg-info/PKG-INFO
--rw-rw-r--   0 richardy  (1000) richardy  (1000)      279 2023-05-29 11:23:10.000000 sqlcrafty-0.0.1/sqlcrafty.egg-info/SOURCES.txt
--rw-rw-r--   0 richardy  (1000) richardy  (1000)        1 2023-05-29 11:23:10.000000 sqlcrafty-0.0.1/sqlcrafty.egg-info/dependency_links.txt
--rw-rw-r--   0 richardy  (1000) richardy  (1000)        7 2023-05-29 11:23:10.000000 sqlcrafty-0.0.1/sqlcrafty.egg-info/requires.txt
--rw-rw-r--   0 richardy  (1000) richardy  (1000)       10 2023-05-29 11:23:10.000000 sqlcrafty-0.0.1/sqlcrafty.egg-info/top_level.txt
+drwxrwxr-x   0 richardy  (1000) richardy  (1000)        0 2023-05-29 12:12:17.250806 sqlcrafty-0.0.2/
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)      181 2023-05-29 12:12:17.250806 sqlcrafty-0.0.2/PKG-INFO
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)       38 2023-05-29 12:12:17.250806 sqlcrafty-0.0.2/setup.cfg
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)      343 2023-05-29 12:11:05.000000 sqlcrafty-0.0.2/setup.py
+drwxrwxr-x   0 richardy  (1000) richardy  (1000)        0 2023-05-29 12:12:17.238806 sqlcrafty-0.0.2/sqlcrafty/
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)        0 2023-05-24 01:51:03.000000 sqlcrafty-0.0.2/sqlcrafty/__init__.py
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)     5004 2023-05-29 01:29:43.000000 sqlcrafty-0.0.2/sqlcrafty/functions.py
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)     7772 2023-05-29 11:09:10.000000 sqlcrafty-0.0.2/sqlcrafty/models.py
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)      775 2023-05-29 12:01:58.000000 sqlcrafty-0.0.2/sqlcrafty/sqlcrafty.py
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)      135 2023-05-29 02:01:13.000000 sqlcrafty-0.0.2/sqlcrafty/utils.py
+drwxrwxr-x   0 richardy  (1000) richardy  (1000)        0 2023-05-29 12:12:17.250806 sqlcrafty-0.0.2/sqlcrafty.egg-info/
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)      181 2023-05-29 12:12:16.000000 sqlcrafty-0.0.2/sqlcrafty.egg-info/PKG-INFO
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)      315 2023-05-29 12:12:16.000000 sqlcrafty-0.0.2/sqlcrafty.egg-info/SOURCES.txt
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)        1 2023-05-29 12:12:16.000000 sqlcrafty-0.0.2/sqlcrafty.egg-info/dependency_links.txt
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)       46 2023-05-29 12:12:16.000000 sqlcrafty-0.0.2/sqlcrafty.egg-info/entry_points.txt
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)        7 2023-05-29 12:12:16.000000 sqlcrafty-0.0.2/sqlcrafty.egg-info/requires.txt
+-rw-rw-r--   0 richardy  (1000) richardy  (1000)       10 2023-05-29 12:12:16.000000 sqlcrafty-0.0.2/sqlcrafty.egg-info/top_level.txt
```

### Comparing `sqlcrafty-0.0.1/sqlcrafty/functions.py` & `sqlcrafty-0.0.2/sqlcrafty/functions.py`

 * *Files identical despite different names*

### Comparing `sqlcrafty-0.0.1/sqlcrafty/models.py` & `sqlcrafty-0.0.2/sqlcrafty/models.py`

 * *Files identical despite different names*


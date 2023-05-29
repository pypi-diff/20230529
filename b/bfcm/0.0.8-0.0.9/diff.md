# Comparing `tmp/bfcm-0.0.8.tar.gz` & `tmp/bfcm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bfcm-0.0.8.tar", last modified: Wed May 17 13:57:43 2023, max compression
+gzip compressed data, was "bfcm-0.0.9.tar", last modified: Mon May 29 19:48:28 2023, max compression
```

## Comparing `bfcm-0.0.8.tar` & `bfcm-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 13:57:43.942000 bfcm-0.0.8/
--rw-rw-rw-   0        0        0     1144 2023-05-17 12:44:41.000000 bfcm-0.0.8/License.txt
--rw-rw-rw-   0        0        0      826 2023-05-17 13:57:43.931000 bfcm-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      789 2023-05-17 13:24:14.000000 bfcm-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-17 13:57:43.861000 bfcm-0.0.8/bfcm/
--rw-rw-rw-   0        0        0       27 2023-05-17 12:44:41.000000 bfcm-0.0.8/bfcm/__init__.py
--rw-rw-rw-   0        0        0     1730 2023-05-17 12:44:41.000000 bfcm-0.0.8/bfcm/bfcm.py
--rw-rw-rw-   0        0        0     7217 2023-05-17 12:44:41.000000 bfcm-0.0.8/bfcm/correlation_matrix.py
-drwxrwxrwx   0        0        0        0 2023-05-17 13:57:43.920000 bfcm-0.0.8/bfcm.egg-info/
--rw-rw-rw-   0        0        0      826 2023-05-17 13:57:43.000000 bfcm-0.0.8/bfcm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      199 2023-05-17 13:57:43.000000 bfcm-0.0.8/bfcm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 13:57:43.000000 bfcm-0.0.8/bfcm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-17 13:57:43.000000 bfcm-0.0.8/bfcm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 13:57:43.940000 bfcm-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-05-17 13:22:16.000000 bfcm-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:48:28.758838 bfcm-0.0.9/
+-rw-rw-rw-   0        0        0     1144 2023-05-29 19:42:02.000000 bfcm-0.0.9/License.txt
+-rw-rw-rw-   0        0        0      490 2023-05-29 19:48:28.757836 bfcm-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      944 2023-05-29 19:42:02.000000 bfcm-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 19:48:28.744835 bfcm-0.0.9/bfcm/
+-rw-rw-rw-   0        0        0       47 2023-05-29 19:45:21.000000 bfcm-0.0.9/bfcm/__init__.py
+-rw-rw-rw-   0        0        0     1730 2023-05-29 19:42:02.000000 bfcm-0.0.9/bfcm/bfcm.py
+-rw-rw-rw-   0        0        0     7217 2023-05-29 19:45:39.000000 bfcm-0.0.9/bfcm/correlation_matrix.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:48:28.754855 bfcm-0.0.9/bfcm.egg-info/
+-rw-rw-rw-   0        0        0      490 2023-05-29 19:48:28.000000 bfcm-0.0.9/bfcm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      199 2023-05-29 19:48:28.000000 bfcm-0.0.9/bfcm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 19:48:28.000000 bfcm-0.0.9/bfcm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-29 19:48:28.000000 bfcm-0.0.9/bfcm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 19:48:28.759834 bfcm-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-05-29 19:45:59.000000 bfcm-0.0.9/setup.py
```

### Comparing `bfcm-0.0.8/License.txt` & `bfcm-0.0.9/License.txt`

 * *Files identical despite different names*

### Comparing `bfcm-0.0.8/bfcm/bfcm.py` & `bfcm-0.0.9/bfcm/bfcm.py`

 * *Files identical despite different names*

### Comparing `bfcm-0.0.8/bfcm/correlation_matrix.py` & `bfcm-0.0.9/bfcm/correlation_matrix.py`

 * *Files identical despite different names*


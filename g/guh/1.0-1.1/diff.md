# Comparing `tmp/guh-1.0.tar.gz` & `tmp/guh-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guh-1.0.tar", last modified: Sun May 28 01:59:29 2023, max compression
+gzip compressed data, was "guh-1.1.tar", last modified: Mon May 29 01:09:41 2023, max compression
```

## Comparing `guh-1.0.tar` & `guh-1.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 01:59:29.225474 guh-1.0/
--rw-rw-rw-   0        0        0     1059 2023-05-28 01:57:46.000000 guh-1.0/LICENSE
--rw-rw-rw-   0        0        0      155 2023-05-28 01:59:29.224476 guh-1.0/PKG-INFO
--rw-rw-rw-   0        0        0        3 2023-05-28 01:57:06.000000 guh-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 01:59:29.214956 guh-1.0/guh/
--rw-rw-rw-   0        0        0        0 2023-05-28 01:45:37.000000 guh-1.0/guh/__init__.py
--rw-rw-rw-   0        0        0       91 2023-05-28 01:44:47.000000 guh-1.0/guh/guh.py
-drwxrwxrwx   0        0        0        0 2023-05-28 01:59:29.223475 guh-1.0/guh.egg-info/
--rw-rw-rw-   0        0        0      155 2023-05-28 01:59:29.000000 guh-1.0/guh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-05-28 01:59:29.000000 guh-1.0/guh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 01:59:29.000000 guh-1.0/guh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-28 01:59:29.000000 guh-1.0/guh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 01:59:29.225474 guh-1.0/setup.cfg
--rw-rw-rw-   0        0        0      200 2023-05-28 01:58:20.000000 guh-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:09:41.018026 guh-1.1/
+-rw-rw-rw-   0        0        0     1059 2023-05-28 01:57:46.000000 guh-1.1/LICENSE
+-rw-rw-rw-   0        0        0      155 2023-05-29 01:09:41.018026 guh-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0        3 2023-05-28 01:57:06.000000 guh-1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 01:09:41.019029 guh-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      213 2023-05-29 01:09:34.000000 guh-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:09:41.010018 guh-1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 01:09:41.016524 guh-1.1/src/guh.egg-info/
+-rw-rw-rw-   0        0        0      155 2023-05-29 01:09:40.000000 guh-1.1/src/guh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-05-29 01:09:40.000000 guh-1.1/src/guh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 01:09:40.000000 guh-1.1/src/guh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-29 01:09:40.000000 guh-1.1/src/guh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       91 2023-05-28 01:44:47.000000 guh-1.1/src/guh.py
```

### Comparing `guh-1.0/LICENSE` & `guh-1.1/LICENSE`

 * *Files identical despite different names*


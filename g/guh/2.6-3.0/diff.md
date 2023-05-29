# Comparing `tmp/guh-2.6.tar.gz` & `tmp/guh-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guh-2.6.tar", last modified: Mon May 29 01:49:48 2023, max compression
+gzip compressed data, was "guh-3.0.tar", last modified: Mon May 29 01:53:14 2023, max compression
```

## Comparing `guh-2.6.tar` & `guh-3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 01:49:48.174637 guh-2.6/
--rw-rw-rw-   0        0        0     1059 2023-05-28 01:57:46.000000 guh-2.6/LICENSE
--rw-rw-rw-   0        0        0      216 2023-05-29 01:49:48.174637 guh-2.6/PKG-INFO
--rw-rw-rw-   0        0        0        3 2023-05-28 01:57:06.000000 guh-2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 01:49:48.167128 guh-2.6/guh/
--rw-rw-rw-   0        0        0      479 2023-05-29 01:49:31.000000 guh-2.6/guh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:49:48.173636 guh-2.6/guh.egg-info/
--rw-rw-rw-   0        0        0      216 2023-05-29 01:49:48.000000 guh-2.6/guh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-05-29 01:49:48.000000 guh-2.6/guh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 01:49:48.000000 guh-2.6/guh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-29 01:49:48.000000 guh-2.6/guh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 01:49:48.175636 guh-2.6/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-05-29 01:49:37.000000 guh-2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:53:14.765500 guh-3.0/
+-rw-rw-rw-   0        0        0     1059 2023-05-28 01:57:46.000000 guh-3.0/LICENSE
+-rw-rw-rw-   0        0        0      216 2023-05-29 01:53:14.765500 guh-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0        3 2023-05-28 01:57:06.000000 guh-3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 01:53:14.760987 guh-3.0/guh/
+-rw-rw-rw-   0        0        0      414 2023-05-29 01:52:37.000000 guh-3.0/guh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:53:14.764496 guh-3.0/guh.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-05-29 01:53:14.000000 guh-3.0/guh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2023-05-29 01:53:14.000000 guh-3.0/guh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 01:53:14.000000 guh-3.0/guh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-29 01:53:14.000000 guh-3.0/guh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 01:53:14.765500 guh-3.0/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-05-29 01:52:41.000000 guh-3.0/setup.py
```

### Comparing `guh-2.6/LICENSE` & `guh-3.0/LICENSE`

 * *Files identical despite different names*


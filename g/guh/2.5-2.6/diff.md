# Comparing `tmp/guh-2.5.tar.gz` & `tmp/guh-2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guh-2.5.tar", last modified: Mon May 29 01:48:58 2023, max compression
+gzip compressed data, was "guh-2.6.tar", last modified: Mon May 29 01:49:48 2023, max compression
```

## Comparing `guh-2.5.tar` & `guh-2.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 01:48:58.686532 guh-2.5/
--rw-rw-rw-   0        0        0     1059 2023-05-28 01:57:46.000000 guh-2.5/LICENSE
--rw-rw-rw-   0        0        0      216 2023-05-29 01:48:58.686532 guh-2.5/PKG-INFO
--rw-rw-rw-   0        0        0        3 2023-05-28 01:57:06.000000 guh-2.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 01:48:58.677021 guh-2.5/guh/
--rw-rw-rw-   0        0        0      441 2023-05-29 01:47:17.000000 guh-2.5/guh/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:48:58.685533 guh-2.5/guh.egg-info/
--rw-rw-rw-   0        0        0      216 2023-05-29 01:48:58.000000 guh-2.5/guh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-05-29 01:48:58.000000 guh-2.5/guh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 01:48:58.000000 guh-2.5/guh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-29 01:48:58.000000 guh-2.5/guh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 01:48:58.686532 guh-2.5/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-05-29 01:48:46.000000 guh-2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:49:48.174637 guh-2.6/
+-rw-rw-rw-   0        0        0     1059 2023-05-28 01:57:46.000000 guh-2.6/LICENSE
+-rw-rw-rw-   0        0        0      216 2023-05-29 01:49:48.174637 guh-2.6/PKG-INFO
+-rw-rw-rw-   0        0        0        3 2023-05-28 01:57:06.000000 guh-2.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 01:49:48.167128 guh-2.6/guh/
+-rw-rw-rw-   0        0        0      479 2023-05-29 01:49:31.000000 guh-2.6/guh/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:49:48.173636 guh-2.6/guh.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-05-29 01:49:48.000000 guh-2.6/guh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      150 2023-05-29 01:49:48.000000 guh-2.6/guh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 01:49:48.000000 guh-2.6/guh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-29 01:49:48.000000 guh-2.6/guh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 01:49:48.175636 guh-2.6/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-05-29 01:49:37.000000 guh-2.6/setup.py
```

### Comparing `guh-2.5/LICENSE` & `guh-2.6/LICENSE`

 * *Files identical despite different names*


# Comparing `tmp/guh-2.1.tar.gz` & `tmp/guh-2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guh-2.1.tar", last modified: Mon May 29 01:28:11 2023, max compression
+gzip compressed data, was "guh-2.2.tar", last modified: Mon May 29 01:32:17 2023, max compression
```

## Comparing `guh-2.1.tar` & `guh-2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 01:28:11.058861 guh-2.1/
--rw-rw-rw-   0        0        0     1059 2023-05-28 01:57:46.000000 guh-2.1/LICENSE
--rw-rw-rw-   0        0        0      216 2023-05-29 01:28:11.058861 guh-2.1/PKG-INFO
--rw-rw-rw-   0        0        0        3 2023-05-28 01:57:06.000000 guh-2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 01:28:11.058861 guh-2.1/setup.cfg
--rw-rw-rw-   0        0        0      302 2023-05-29 01:27:51.000000 guh-2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:28:11.051768 guh-2.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 01:28:11.057860 guh-2.1/src/guh.egg-info/
--rw-rw-rw-   0        0        0      216 2023-05-29 01:28:11.000000 guh-2.1/src/guh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-05-29 01:28:11.000000 guh-2.1/src/guh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 01:28:11.000000 guh-2.1/src/guh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-29 01:28:11.000000 guh-2.1/src/guh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      441 2023-05-29 01:23:07.000000 guh-2.1/src/guh.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:32:17.591563 guh-2.2/
+-rw-rw-rw-   0        0        0     1059 2023-05-28 01:57:46.000000 guh-2.2/LICENSE
+-rw-rw-rw-   0        0        0      216 2023-05-29 01:32:17.590564 guh-2.2/PKG-INFO
+-rw-rw-rw-   0        0        0        3 2023-05-28 01:57:06.000000 guh-2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 01:32:17.591563 guh-2.2/setup.cfg
+-rw-rw-rw-   0        0        0      302 2023-05-29 01:31:53.000000 guh-2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:32:17.582051 guh-2.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 01:32:17.589558 guh-2.2/src/guh.egg-info/
+-rw-rw-rw-   0        0        0      216 2023-05-29 01:32:17.000000 guh-2.2/src/guh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-05-29 01:32:17.000000 guh-2.2/src/guh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 01:32:17.000000 guh-2.2/src/guh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-29 01:32:17.000000 guh-2.2/src/guh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      441 2023-05-29 01:23:07.000000 guh-2.2/src/guh.py
```

### Comparing `guh-2.1/LICENSE` & `guh-2.2/LICENSE`

 * *Files identical despite different names*


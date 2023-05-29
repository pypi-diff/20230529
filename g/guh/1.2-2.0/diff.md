# Comparing `tmp/guh-1.2.tar.gz` & `tmp/guh-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guh-1.2.tar", last modified: Mon May 29 01:16:57 2023, max compression
+gzip compressed data, was "guh-2.0.tar", last modified: Mon May 29 01:22:18 2023, max compression
```

## Comparing `guh-1.2.tar` & `guh-2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 01:16:57.328835 guh-1.2/
--rw-rw-rw-   0        0        0     1059 2023-05-28 01:57:46.000000 guh-1.2/LICENSE
--rw-rw-rw-   0        0        0      155 2023-05-29 01:16:57.328835 guh-1.2/PKG-INFO
--rw-rw-rw-   0        0        0        3 2023-05-28 01:57:06.000000 guh-1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 01:16:57.328835 guh-1.2/setup.cfg
--rw-rw-rw-   0        0        0      213 2023-05-29 01:16:49.000000 guh-1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:16:57.316324 guh-1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-29 01:16:57.327835 guh-1.2/src/guh.egg-info/
--rw-rw-rw-   0        0        0      155 2023-05-29 01:16:57.000000 guh-1.2/src/guh.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2023-05-29 01:16:57.000000 guh-1.2/src/guh.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 01:16:57.000000 guh-1.2/src/guh.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-05-29 01:16:57.000000 guh-1.2/src/guh.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      432 2023-05-29 01:16:22.000000 guh-1.2/src/guh.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:22:18.239084 guh-2.0/
+-rw-rw-rw-   0        0        0     1059 2023-05-28 01:57:46.000000 guh-2.0/LICENSE
+-rw-rw-rw-   0        0        0      155 2023-05-29 01:22:18.237578 guh-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0        3 2023-05-28 01:57:06.000000 guh-2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 01:22:18.239084 guh-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      213 2023-05-29 01:21:21.000000 guh-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:22:18.231489 guh-2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 01:22:18.237578 guh-2.0/src/guh.egg-info/
+-rw-rw-rw-   0        0        0      155 2023-05-29 01:22:18.000000 guh-2.0/src/guh.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2023-05-29 01:22:18.000000 guh-2.0/src/guh.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 01:22:18.000000 guh-2.0/src/guh.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-05-29 01:22:18.000000 guh-2.0/src/guh.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      441 2023-05-29 01:21:58.000000 guh-2.0/src/guh.py
```

### Comparing `guh-1.2/LICENSE` & `guh-2.0/LICENSE`

 * *Files identical despite different names*


# Comparing `tmp/arxiv_update_cli-1.0.3.tar.gz` & `tmp/arxiv_update_cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arxiv_update_cli-1.0.3.tar", last modified: Fri Oct 21 15:11:36 2022, max compression
+gzip compressed data, was "arxiv_update_cli-1.1.0.tar", last modified: Mon May 29 12:19:03 2023, max compression
```

## Comparing `arxiv_update_cli-1.0.3.tar` & `arxiv_update_cli-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 juliette  (1000) juliette  (1000)        0 2022-10-21 15:11:36.513410 arxiv_update_cli-1.0.3/
--rw-r--r--   0 juliette  (1000) juliette  (1000)      130 2022-10-21 15:04:43.000000 arxiv_update_cli-1.0.3/.gitignore
--rw-r--r--   0 juliette  (1000) juliette  (1000)     1023 2022-01-31 10:49:39.000000 arxiv_update_cli-1.0.3/LICENSE
--rw-r--r--   0 juliette  (1000) juliette  (1000)       16 2022-02-07 19:47:25.000000 arxiv_update_cli-1.0.3/MANIFEST.in
--rw-r--r--   0 juliette  (1000) juliette  (1000)     5103 2022-10-21 15:11:36.513410 arxiv_update_cli-1.0.3/PKG-INFO
--rw-r--r--   0 juliette  (1000) juliette  (1000)     4429 2022-10-21 14:37:25.000000 arxiv_update_cli-1.0.3/README.rst
-drwxr-xr-x   0 juliette  (1000) juliette  (1000)        0 2022-10-21 15:11:36.513410 arxiv_update_cli-1.0.3/arxiv_update_cli.egg-info/
--rw-r--r--   0 juliette  (1000) juliette  (1000)     5103 2022-10-21 15:11:36.000000 arxiv_update_cli-1.0.3/arxiv_update_cli.egg-info/PKG-INFO
--rw-r--r--   0 juliette  (1000) juliette  (1000)      341 2022-10-21 15:11:36.000000 arxiv_update_cli-1.0.3/arxiv_update_cli.egg-info/SOURCES.txt
--rw-r--r--   0 juliette  (1000) juliette  (1000)        1 2022-10-21 15:11:36.000000 arxiv_update_cli-1.0.3/arxiv_update_cli.egg-info/dependency_links.txt
--rw-r--r--   0 juliette  (1000) juliette  (1000)       59 2022-10-21 15:11:36.000000 arxiv_update_cli-1.0.3/arxiv_update_cli.egg-info/entry_points.txt
--rw-r--r--   0 juliette  (1000) juliette  (1000)       55 2022-10-21 15:11:36.000000 arxiv_update_cli-1.0.3/arxiv_update_cli.egg-info/requires.txt
--rw-r--r--   0 juliette  (1000) juliette  (1000)       17 2022-10-21 15:11:36.000000 arxiv_update_cli-1.0.3/arxiv_update_cli.egg-info/top_level.txt
--rw-r--r--   0 juliette  (1000) juliette  (1000)    14296 2022-10-21 15:04:43.000000 arxiv_update_cli-1.0.3/arxiv_update_cli.py
-drwxr-xr-x   0 juliette  (1000) juliette  (1000)        0 2022-10-21 15:11:36.513410 arxiv_update_cli-1.0.3/packaging_archlinux/
--rw-r--r--   0 juliette  (1000) juliette  (1000)      767 2022-10-21 15:10:23.000000 arxiv_update_cli-1.0.3/packaging_archlinux/PKGBUILD
--rw-r--r--   0 juliette  (1000) juliette  (1000)       38 2022-10-21 15:11:36.513410 arxiv_update_cli-1.0.3/setup.cfg
--rw-r--r--   0 juliette  (1000) juliette  (1000)     1132 2022-10-21 14:37:25.000000 arxiv_update_cli-1.0.3/setup.py
+drwxr-xr-x   0 juliette  (1000) juliette  (1000)        0 2023-05-29 12:19:03.405548 arxiv_update_cli-1.1.0/
+-rw-r--r--   0 juliette  (1000) juliette  (1000)      739 2023-05-29 12:16:37.000000 arxiv_update_cli-1.1.0/.appveyor.yml
+-rw-r--r--   0 juliette  (1000) juliette  (1000)      141 2022-12-06 17:51:55.000000 arxiv_update_cli-1.1.0/.codecov.yml
+-rw-r--r--   0 juliette  (1000) juliette  (1000)      149 2022-12-05 15:37:37.000000 arxiv_update_cli-1.1.0/.gitignore
+-rw-r--r--   0 juliette  (1000) juliette  (1000)     1023 2022-01-31 10:49:39.000000 arxiv_update_cli-1.1.0/LICENSE
+-rw-r--r--   0 juliette  (1000) juliette  (1000)       16 2022-02-07 19:47:25.000000 arxiv_update_cli-1.1.0/MANIFEST.in
+-rw-r--r--   0 juliette  (1000) juliette  (1000)    10093 2023-05-29 12:19:03.405548 arxiv_update_cli-1.1.0/PKG-INFO
+-rw-r--r--   0 juliette  (1000) juliette  (1000)     9419 2023-05-29 12:16:37.000000 arxiv_update_cli-1.1.0/README.rst
+drwxr-xr-x   0 juliette  (1000) juliette  (1000)        0 2023-05-29 12:19:03.405548 arxiv_update_cli-1.1.0/arxiv_update_cli.egg-info/
+-rw-r--r--   0 juliette  (1000) juliette  (1000)    10093 2023-05-29 12:19:03.000000 arxiv_update_cli-1.1.0/arxiv_update_cli.egg-info/PKG-INFO
+-rw-r--r--   0 juliette  (1000) juliette  (1000)      402 2023-05-29 12:19:03.000000 arxiv_update_cli-1.1.0/arxiv_update_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 juliette  (1000) juliette  (1000)        1 2023-05-29 12:19:03.000000 arxiv_update_cli-1.1.0/arxiv_update_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 juliette  (1000) juliette  (1000)       59 2023-05-29 12:19:03.000000 arxiv_update_cli-1.1.0/arxiv_update_cli.egg-info/entry_points.txt
+-rw-r--r--   0 juliette  (1000) juliette  (1000)       55 2023-05-29 12:19:03.000000 arxiv_update_cli-1.1.0/arxiv_update_cli.egg-info/requires.txt
+-rw-r--r--   0 juliette  (1000) juliette  (1000)       17 2023-05-29 12:19:03.000000 arxiv_update_cli-1.1.0/arxiv_update_cli.egg-info/top_level.txt
+-rw-r--r--   0 juliette  (1000) juliette  (1000)    27653 2023-05-29 12:16:37.000000 arxiv_update_cli-1.1.0/arxiv_update_cli.py
+-rw-r--r--   0 juliette  (1000) juliette  (1000)    27823 2023-05-29 12:16:37.000000 arxiv_update_cli-1.1.0/arxiv_update_cli.py.orig
+drwxr-xr-x   0 juliette  (1000) juliette  (1000)        0 2023-05-29 12:19:03.405548 arxiv_update_cli-1.1.0/packaging_archlinux/
+-rw-r--r--   0 juliette  (1000) juliette  (1000)      870 2023-05-29 12:16:37.000000 arxiv_update_cli-1.1.0/packaging_archlinux/PKGBUILD
+-rw-r--r--   0 juliette  (1000) juliette  (1000)       38 2023-05-29 12:19:03.405548 arxiv_update_cli-1.1.0/setup.cfg
+-rw-r--r--   0 juliette  (1000) juliette  (1000)     1132 2023-05-29 12:16:37.000000 arxiv_update_cli-1.1.0/setup.py
+-rw-r--r--   0 juliette  (1000) juliette  (1000)    33448 2023-05-29 12:16:37.000000 arxiv_update_cli-1.1.0/tests.py
```

### Comparing `arxiv_update_cli-1.0.3/LICENSE` & `arxiv_update_cli-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arxiv_update_cli-1.0.3/setup.py` & `arxiv_update_cli-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open('README.rst', encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name="arxiv_update_cli",
-    version="1.0.3",
+    version="1.1.0",
     description="Fetch new articles on arXiv by keywords",
     author="Juliette Monsel",
     author_email="j_4321@protonmail.com",
     license="MIT",
     url="https://gitlab.com/j_4321/arxivscript",
     py_modules=["arxiv_update_cli"],
     entry_points={
```


# Comparing `tmp/ronnytest-0.2.7.tar.gz` & `tmp/ronnytest-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ronnytest-0.2.7.tar", last modified: Fri May 26 08:54:05 2023, max compression
+gzip compressed data, was "dist/ronnytest-0.2.8.tar", last modified: Mon May 29 11:11:05 2023, max compression
```

## Comparing `ronnytest-0.2.7.tar` & `ronnytest-0.2.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 08:54:05.000000 ronnytest-0.2.7/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 08:54:05.000000 ronnytest-0.2.7/ronnytest.egg-info/
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-26 08:54:05.000000 ronnytest-0.2.7/ronnytest.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 08:54:05.000000 ronnytest-0.2.7/ronnytest.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      158 2023-05-26 08:54:05.000000 ronnytest-0.2.7/ronnytest.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 08:54:05.000000 ronnytest-0.2.7/ronnytest.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.2.7/README.md
--rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)      220 2023-05-26 08:54:05.000000 ronnytest-0.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 08:54:05.000000 ronnytest-0.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1725 2023-05-26 08:49:20.000000 ronnytest-0.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:11:05.000000 ronnytest-0.2.8/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 11:11:05.000000 ronnytest-0.2.8/ronnytest.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-29 11:11:05.000000 ronnytest-0.2.8/ronnytest.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 11:11:05.000000 ronnytest-0.2.8/ronnytest.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      158 2023-05-29 11:11:05.000000 ronnytest-0.2.8/ronnytest.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 11:11:05.000000 ronnytest-0.2.8/ronnytest.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-25 03:55:14.000000 ronnytest-0.2.8/README.md
+-rw-r--r--   0 root         (0) root         (0)     1073 2023-05-25 03:55:14.000000 ronnytest-0.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      220 2023-05-29 11:11:05.000000 ronnytest-0.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 11:11:05.000000 ronnytest-0.2.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1353 2023-05-29 11:10:49.000000 ronnytest-0.2.8/setup.py
```

### Comparing `ronnytest-0.2.7/LICENSE` & `ronnytest-0.2.8/LICENSE`

 * *Files identical despite different names*


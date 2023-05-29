# Comparing `tmp/alpha-filter-0.9.1.tar.gz` & `tmp/alpha-filter-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpha-filter-0.9.1.tar", last modified: Sun May 28 13:17:45 2023, max compression
+gzip compressed data, was "alpha-filter-0.9.2.tar", last modified: Mon May 29 21:50:16 2023, max compression
```

## Comparing `alpha-filter-0.9.1.tar` & `alpha-filter-0.9.2.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxr-x   0 yllen     (1000) yllen     (1000)        0 2023-05-28 13:17:45.423551 alpha-filter-0.9.1/
--rw-rw-r--   0 yllen     (1000) yllen     (1000)      172 2023-05-28 13:17:45.423551 alpha-filter-0.9.1/PKG-INFO
--rw-rw-r--   0 yllen     (1000) yllen     (1000)     1764 2023-05-28 13:10:31.000000 alpha-filter-0.9.1/README.md
-drwxrwxr-x   0 yllen     (1000) yllen     (1000)        0 2023-05-28 13:17:45.423551 alpha-filter-0.9.1/alpha_filter.egg-info/
--rw-rw-r--   0 yllen     (1000) yllen     (1000)      172 2023-05-28 13:17:45.000000 alpha-filter-0.9.1/alpha_filter.egg-info/PKG-INFO
--rw-rw-r--   0 yllen     (1000) yllen     (1000)      162 2023-05-28 13:17:45.000000 alpha-filter-0.9.1/alpha_filter.egg-info/SOURCES.txt
--rw-rw-r--   0 yllen     (1000) yllen     (1000)        1 2023-05-28 13:17:45.000000 alpha-filter-0.9.1/alpha_filter.egg-info/dependency_links.txt
--rw-rw-r--   0 yllen     (1000) yllen     (1000)       13 2023-05-28 13:17:45.000000 alpha-filter-0.9.1/alpha_filter.egg-info/top_level.txt
--rw-rw-r--   0 yllen     (1000) yllen     (1000)       38 2023-05-28 13:17:45.423551 alpha-filter-0.9.1/setup.cfg
--rw-rw-r--   0 yllen     (1000) yllen     (1000)      184 2023-05-28 11:52:34.000000 alpha-filter-0.9.1/setup.py
+drwxrwxr-x   0 yllen     (1000) yllen     (1000)        0 2023-05-29 21:50:16.435242 alpha-filter-0.9.2/
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)     1969 2023-05-29 21:50:16.435242 alpha-filter-0.9.2/PKG-INFO
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)     1764 2023-05-28 13:10:31.000000 alpha-filter-0.9.2/README.md
+drwxrwxr-x   0 yllen     (1000) yllen     (1000)        0 2023-05-29 21:50:16.435242 alpha-filter-0.9.2/alpha_filter.egg-info/
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)     1969 2023-05-29 21:50:16.000000 alpha-filter-0.9.2/alpha_filter.egg-info/PKG-INFO
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)      177 2023-05-29 21:50:16.000000 alpha-filter-0.9.2/alpha_filter.egg-info/SOURCES.txt
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)        1 2023-05-29 21:50:16.000000 alpha-filter-0.9.2/alpha_filter.egg-info/dependency_links.txt
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)       12 2023-05-29 21:50:16.000000 alpha-filter-0.9.2/alpha_filter.egg-info/top_level.txt
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)     6971 2023-05-28 13:13:27.000000 alpha-filter-0.9.2/alphafilter.py
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)       38 2023-05-29 21:50:16.435242 alpha-filter-0.9.2/setup.cfg
+-rw-rw-r--   0 yllen     (1000) yllen     (1000)      364 2023-05-29 21:47:06.000000 alpha-filter-0.9.2/setup.py
```

### Comparing `alpha-filter-0.9.1/README.md` & `alpha-filter-0.9.2/README.md`

 * *Files identical despite different names*


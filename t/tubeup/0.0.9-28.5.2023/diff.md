# Comparing `tmp/tubeup-0.0.9.tar.gz` & `tmp/tubeup-28.5.2023.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tubeup-0.0.9.tar", last modified: Thu Aug 31 02:01:27 2017, max compression
+gzip compressed data, was "tubeup-28.5.2023.tar", last modified: Sun May 28 22:42:49 2023, max compression
```

## Comparing `tubeup-0.0.9.tar` & `tubeup-28.5.2023.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxr-x   0 antonizoon  (1000) antonizoon  (1000)        0 2017-08-31 02:01:27.000000 tubeup-0.0.9/
--rw-rw-r--   0 antonizoon  (1000) antonizoon  (1000)      513 2017-08-31 02:00:52.000000 tubeup-0.0.9/setup.py
-drwxrwxr-x   0 antonizoon  (1000) antonizoon  (1000)        0 2017-08-31 02:01:27.000000 tubeup-0.0.9/tubeup.egg-info/
--rw-rw-r--   0 antonizoon  (1000) antonizoon  (1000)      228 2017-08-31 02:01:27.000000 tubeup-0.0.9/tubeup.egg-info/SOURCES.txt
--rw-rw-r--   0 antonizoon  (1000) antonizoon  (1000)        1 2017-08-31 02:01:27.000000 tubeup-0.0.9/tubeup.egg-info/dependency_links.txt
--rw-rw-r--   0 antonizoon  (1000) antonizoon  (1000)        7 2017-08-31 02:01:27.000000 tubeup-0.0.9/tubeup.egg-info/top_level.txt
--rw-rw-r--   0 antonizoon  (1000) antonizoon  (1000)       49 2017-08-31 02:01:27.000000 tubeup-0.0.9/tubeup.egg-info/entry_points.txt
--rw-rw-r--   0 antonizoon  (1000) antonizoon  (1000)      268 2017-08-31 02:01:27.000000 tubeup-0.0.9/tubeup.egg-info/PKG-INFO
--rw-rw-r--   0 antonizoon  (1000) antonizoon  (1000)       41 2017-08-31 02:01:27.000000 tubeup-0.0.9/tubeup.egg-info/requires.txt
-drwxrwxr-x   0 antonizoon  (1000) antonizoon  (1000)        0 2017-08-31 02:01:27.000000 tubeup-0.0.9/tubeup/
--rw-rw-r--   0 antonizoon  (1000) antonizoon  (1000)        0 2017-03-02 15:50:38.000000 tubeup-0.0.9/tubeup/__init__.py
--rwxrwxr-x   0 antonizoon  (1000) antonizoon  (1000)    11727 2017-08-31 01:57:52.000000 tubeup-0.0.9/tubeup/__main__.py
--rw-rw-r--   0 antonizoon  (1000) antonizoon  (1000)       38 2017-08-31 02:01:27.000000 tubeup-0.0.9/setup.cfg
--rw-rw-r--   0 antonizoon  (1000) antonizoon  (1000)      268 2017-08-31 02:01:27.000000 tubeup-0.0.9/PKG-INFO
+drwxrwxr-x   0 vxbinaca  (1000) vxbinaca  (1000)        0 2023-05-28 22:42:49.780250 tubeup-28.5.2023/
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)    35122 2021-09-28 02:31:45.000000 tubeup-28.5.2023/LICENSE
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)      261 2023-05-28 22:42:49.780250 tubeup-28.5.2023/PKG-INFO
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)    10312 2023-05-28 22:41:06.000000 tubeup-28.5.2023/README.md
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)      233 2023-05-28 22:42:49.780250 tubeup-28.5.2023/setup.cfg
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)      763 2023-01-02 22:16:20.000000 tubeup-28.5.2023/setup.py
+drwxrwxr-x   0 vxbinaca  (1000) vxbinaca  (1000)        0 2023-05-28 22:42:49.776250 tubeup-28.5.2023/tubeup/
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)    24200 2023-05-28 22:41:06.000000 tubeup-28.5.2023/tubeup/TubeUp.py
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)       26 2023-05-28 22:42:40.000000 tubeup-28.5.2023/tubeup/__init__.py
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)     4671 2023-01-02 22:16:20.000000 tubeup-28.5.2023/tubeup/__main__.py
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)      634 2021-09-28 02:31:45.000000 tubeup-28.5.2023/tubeup/utils.py
+drwxrwxr-x   0 vxbinaca  (1000) vxbinaca  (1000)        0 2023-05-28 22:42:49.780250 tubeup-28.5.2023/tubeup.egg-info/
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)      261 2023-05-28 22:42:49.000000 tubeup-28.5.2023/tubeup.egg-info/PKG-INFO
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)      289 2023-05-28 22:42:49.000000 tubeup-28.5.2023/tubeup.egg-info/SOURCES.txt
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)        1 2023-05-28 22:42:49.000000 tubeup-28.5.2023/tubeup.egg-info/dependency_links.txt
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)       49 2023-05-28 22:42:49.000000 tubeup-28.5.2023/tubeup.egg-info/entry_points.txt
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)       61 2023-05-28 22:42:49.000000 tubeup-28.5.2023/tubeup.egg-info/requires.txt
+-rw-rw-r--   0 vxbinaca  (1000) vxbinaca  (1000)        7 2023-05-28 22:42:49.000000 tubeup-28.5.2023/tubeup.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```


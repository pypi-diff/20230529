# Comparing `tmp/trailml-0.1.2.tar.gz` & `tmp/trailml-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trailml-0.1.2.tar", last modified: Tue Mar 28 10:55:57 2023, max compression
+gzip compressed data, was "trailml-1.0.0.tar", last modified: Mon May 29 20:18:59 2023, max compression
```

## Comparing `trailml-0.1.2.tar` & `trailml-1.0.0.tar`

### file list

```diff
@@ -1,15 +1,22 @@
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-03-28 10:55:57.507743 trailml-0.1.2/
--rw-r--r--   0 nikolaus   (501) staff       (20)     2443 2023-03-28 10:55:57.507593 trailml-0.1.2/PKG-INFO
--rw-r--r--   0 nikolaus   (501) staff       (20)     1657 2023-03-28 10:55:53.000000 trailml-0.1.2/README.md
--rw-r--r--   0 nikolaus   (501) staff       (20)       38 2023-03-28 10:55:57.507795 trailml-0.1.2/setup.cfg
--rw-r--r--   0 nikolaus   (501) staff       (20)     1468 2023-03-28 10:50:39.000000 trailml-0.1.2/setup.py
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-03-28 10:55:57.506526 trailml-0.1.2/trailml/
--rw-r--r--   0 nikolaus   (501) staff       (20)       41 2023-03-28 10:47:06.000000 trailml-0.1.2/trailml/__init__.py
--rw-r--r--   0 nikolaus   (501) staff       (20)     3973 2023-03-28 10:47:07.000000 trailml-0.1.2/trailml/db_import.py
--rw-r--r--   0 nikolaus   (501) staff       (20)      209 2023-03-28 10:47:08.000000 trailml-0.1.2/trailml/endpoints.ini
-drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-03-28 10:55:57.507384 trailml-0.1.2/trailml.egg-info/
--rw-r--r--   0 nikolaus   (501) staff       (20)     2443 2023-03-28 10:55:57.000000 trailml-0.1.2/trailml.egg-info/PKG-INFO
--rw-r--r--   0 nikolaus   (501) staff       (20)      235 2023-03-28 10:55:57.000000 trailml-0.1.2/trailml.egg-info/SOURCES.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)        1 2023-03-28 10:55:57.000000 trailml-0.1.2/trailml.egg-info/dependency_links.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)       29 2023-03-28 10:55:57.000000 trailml-0.1.2/trailml.egg-info/requires.txt
--rw-r--r--   0 nikolaus   (501) staff       (20)        8 2023-03-28 10:55:57.000000 trailml-0.1.2/trailml.egg-info/top_level.txt
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.460216 trailml-1.0.0/
+-rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-05-29 20:18:59.460058 trailml-1.0.0/PKG-INFO
+-rw-r--r--   0 nikolaus   (501) staff       (20)      832 2023-05-29 16:34:46.000000 trailml-1.0.0/README.md
+-rw-r--r--   0 nikolaus   (501) staff       (20)      665 2023-05-29 20:17:34.000000 trailml-1.0.0/pyproject.toml
+-rw-r--r--   0 nikolaus   (501) staff       (20)       38 2023-05-29 20:18:59.460265 trailml-1.0.0/setup.cfg
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.455538 trailml-1.0.0/src/
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.456561 trailml-1.0.0/src/trail/
+-rw-r--r--   0 nikolaus   (501) staff       (20)       44 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/__init__.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.457268 trailml-1.0.0/src/trail/libconfig/
+-rw-r--r--   0 nikolaus   (501) staff       (20)      194 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/libconfig/__init__.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)      467 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/libconfig/config.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)     8416 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/trail.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.458068 trailml-1.0.0/src/trail/userconfig/
+-rw-r--r--   0 nikolaus   (501) staff       (20)      650 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/userconfig/__init__.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)     3074 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/userconfig/config.py
+-rw-r--r--   0 nikolaus   (501) staff       (20)      859 2023-05-29 16:34:46.000000 trailml-1.0.0/src/trail/userconfig/exceptions.py
+drwxr-xr-x   0 nikolaus   (501) staff       (20)        0 2023-05-29 20:18:59.459805 trailml-1.0.0/src/trailml.egg-info/
+-rw-r--r--   0 nikolaus   (501) staff       (20)     1281 2023-05-29 20:18:59.000000 trailml-1.0.0/src/trailml.egg-info/PKG-INFO
+-rw-r--r--   0 nikolaus   (501) staff       (20)      400 2023-05-29 20:18:59.000000 trailml-1.0.0/src/trailml.egg-info/SOURCES.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)        1 2023-05-29 20:18:59.000000 trailml-1.0.0/src/trailml.egg-info/dependency_links.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)       62 2023-05-29 20:18:59.000000 trailml-1.0.0/src/trailml.egg-info/requires.txt
+-rw-r--r--   0 nikolaus   (501) staff       (20)        6 2023-05-29 20:18:59.000000 trailml-1.0.0/src/trailml.egg-info/top_level.txt
```


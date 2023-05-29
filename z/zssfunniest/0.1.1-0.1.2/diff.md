# Comparing `tmp/zssfunniest-0.1.1.tar.gz` & `tmp/zssfunniest-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zssfunniest-0.1.1.tar", last modified: Mon May 29 06:03:09 2023, max compression
+gzip compressed data, was "zssfunniest-0.1.2.tar", last modified: Mon May 29 06:20:54 2023, max compression
```

## Comparing `zssfunniest-0.1.1.tar` & `zssfunniest-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 06:03:09.843408 zssfunniest-0.1.1/
--rw-rw-r--   0 zss       (1000) zss       (1000)      205 2023-05-29 06:03:09.843408 zssfunniest-0.1.1/PKG-INFO
--rw-rw-r--   0 zss       (1000) zss       (1000)       38 2023-05-29 06:03:09.843408 zssfunniest-0.1.1/setup.cfg
--rw-rw-r--   0 zss       (1000) zss       (1000)      321 2023-05-29 06:03:07.000000 zssfunniest-0.1.1/setup.py
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 06:03:09.843408 zssfunniest-0.1.1/zssfunniest/
--rw-rw-r--   0 zss       (1000) zss       (1000)       22 2023-05-29 06:01:51.000000 zssfunniest-0.1.1/zssfunniest/__init__.py
--rw-rw-r--   0 zss       (1000) zss       (1000)       29 2023-05-29 06:01:51.000000 zssfunniest-0.1.1/zssfunniest/main.py
-drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 06:03:09.843408 zssfunniest-0.1.1/zssfunniest.egg-info/
--rw-rw-r--   0 zss       (1000) zss       (1000)      205 2023-05-29 06:03:09.000000 zssfunniest-0.1.1/zssfunniest.egg-info/PKG-INFO
--rw-rw-r--   0 zss       (1000) zss       (1000)      226 2023-05-29 06:03:09.000000 zssfunniest-0.1.1/zssfunniest.egg-info/SOURCES.txt
--rw-rw-r--   0 zss       (1000) zss       (1000)        1 2023-05-29 06:03:09.000000 zssfunniest-0.1.1/zssfunniest.egg-info/dependency_links.txt
--rw-rw-r--   0 zss       (1000) zss       (1000)        1 2023-05-29 05:46:02.000000 zssfunniest-0.1.1/zssfunniest.egg-info/not-zip-safe
--rw-rw-r--   0 zss       (1000) zss       (1000)       12 2023-05-29 06:03:09.000000 zssfunniest-0.1.1/zssfunniest.egg-info/top_level.txt
+drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 06:20:54.273236 zssfunniest-0.1.2/
+-rw-rw-r--   0 zss       (1000) zss       (1000)       18 2023-05-29 06:18:46.000000 zssfunniest-0.1.2/MANIFEST.in
+-rw-rw-r--   0 zss       (1000) zss       (1000)      315 2023-05-29 06:20:54.273236 zssfunniest-0.1.2/PKG-INFO
+-rw-rw-r--   0 zss       (1000) zss       (1000)      108 2023-05-29 06:18:39.000000 zssfunniest-0.1.2/README.rst
+-rw-rw-r--   0 zss       (1000) zss       (1000)       38 2023-05-29 06:20:54.273236 zssfunniest-0.1.2/setup.cfg
+-rw-rw-r--   0 zss       (1000) zss       (1000)      573 2023-05-29 06:20:42.000000 zssfunniest-0.1.2/setup.py
+drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 06:20:54.269236 zssfunniest-0.1.2/zssfunniest/
+-rw-rw-r--   0 zss       (1000) zss       (1000)       22 2023-05-29 06:01:51.000000 zssfunniest-0.1.2/zssfunniest/__init__.py
+-rw-rw-r--   0 zss       (1000) zss       (1000)       59 2023-05-29 06:08:59.000000 zssfunniest-0.1.2/zssfunniest/main.py
+drwxrwxr-x   0 zss       (1000) zss       (1000)        0 2023-05-29 06:20:54.273236 zssfunniest-0.1.2/zssfunniest.egg-info/
+-rw-rw-r--   0 zss       (1000) zss       (1000)      315 2023-05-29 06:20:54.000000 zssfunniest-0.1.2/zssfunniest.egg-info/PKG-INFO
+-rw-rw-r--   0 zss       (1000) zss       (1000)      283 2023-05-29 06:20:54.000000 zssfunniest-0.1.2/zssfunniest.egg-info/SOURCES.txt
+-rw-rw-r--   0 zss       (1000) zss       (1000)        1 2023-05-29 06:20:54.000000 zssfunniest-0.1.2/zssfunniest.egg-info/dependency_links.txt
+-rw-rw-r--   0 zss       (1000) zss       (1000)        1 2023-05-29 05:46:02.000000 zssfunniest-0.1.2/zssfunniest.egg-info/not-zip-safe
+-rw-rw-r--   0 zss       (1000) zss       (1000)        9 2023-05-29 06:20:54.000000 zssfunniest-0.1.2/zssfunniest.egg-info/requires.txt
+-rw-rw-r--   0 zss       (1000) zss       (1000)       12 2023-05-29 06:20:54.000000 zssfunniest-0.1.2/zssfunniest.egg-info/top_level.txt
```


# Comparing `tmp/tlcloud-0.1.tar.gz` & `tmp/tlcloud-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tlcloud-0.1.tar", last modified: Mon May 29 03:21:20 2023, max compression
+gzip compressed data, was "tlcloud-0.2.1.tar", last modified: Mon May 29 03:31:49 2023, max compression
```

## Comparing `tlcloud-0.1.tar` & `tlcloud-0.2.1.tar`

### file list

```diff
@@ -1,10 +1,13 @@
-drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-05-29 03:21:20.817907 tlcloud-0.1/
--rw-r--r--   0 craiet     (501) staff       (20)      320 2023-05-29 03:21:20.817799 tlcloud-0.1/PKG-INFO
--rw-r--r--   0 craiet     (501) staff       (20)       23 2023-05-29 03:21:17.000000 tlcloud-0.1/README.md
--rw-r--r--   0 craiet     (501) staff       (20)       38 2023-05-29 03:21:20.817947 tlcloud-0.1/setup.cfg
--rw-r--r--   0 craiet     (501) staff       (20)      503 2023-05-29 03:21:17.000000 tlcloud-0.1/setup.py
-drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-05-29 03:21:20.817641 tlcloud-0.1/tlcloud.egg-info/
--rw-r--r--   0 craiet     (501) staff       (20)      320 2023-05-29 03:21:20.000000 tlcloud-0.1/tlcloud.egg-info/PKG-INFO
--rw-r--r--   0 craiet     (501) staff       (20)      142 2023-05-29 03:21:20.000000 tlcloud-0.1/tlcloud.egg-info/SOURCES.txt
--rw-r--r--   0 craiet     (501) staff       (20)        1 2023-05-29 03:21:20.000000 tlcloud-0.1/tlcloud.egg-info/dependency_links.txt
--rw-r--r--   0 craiet     (501) staff       (20)        1 2023-05-29 03:21:20.000000 tlcloud-0.1/tlcloud.egg-info/top_level.txt
+drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-05-29 03:31:49.685217 tlcloud-0.2.1/
+-rw-r--r--   0 craiet     (501) staff       (20)      322 2023-05-29 03:31:49.685058 tlcloud-0.2.1/PKG-INFO
+-rw-r--r--   0 craiet     (501) staff       (20)       23 2023-05-29 03:21:17.000000 tlcloud-0.2.1/README.md
+-rw-r--r--   0 craiet     (501) staff       (20)       38 2023-05-29 03:31:49.685257 tlcloud-0.2.1/setup.cfg
+-rw-r--r--   0 craiet     (501) staff       (20)      505 2023-05-29 03:30:22.000000 tlcloud-0.2.1/setup.py
+drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-05-29 03:31:49.684423 tlcloud-0.2.1/tlcloud/
+-rw-r--r--   0 craiet     (501) staff       (20)        0 2023-05-29 03:27:53.000000 tlcloud-0.2.1/tlcloud/__init__.py
+-rw-r--r--   0 craiet     (501) staff       (20)    12708 2023-05-29 03:18:34.000000 tlcloud-0.2.1/tlcloud/geo.py
+drwxr-xr-x   0 craiet     (501) staff       (20)        0 2023-05-29 03:31:49.684886 tlcloud-0.2.1/tlcloud.egg-info/
+-rw-r--r--   0 craiet     (501) staff       (20)      322 2023-05-29 03:31:49.000000 tlcloud-0.2.1/tlcloud.egg-info/PKG-INFO
+-rw-r--r--   0 craiet     (501) staff       (20)      177 2023-05-29 03:31:49.000000 tlcloud-0.2.1/tlcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 craiet     (501) staff       (20)        1 2023-05-29 03:31:49.000000 tlcloud-0.2.1/tlcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 craiet     (501) staff       (20)        8 2023-05-29 03:31:49.000000 tlcloud-0.2.1/tlcloud.egg-info/top_level.txt
```


# Comparing `tmp/clu_codes_nester-1.3.0.tar.gz` & `tmp/clu_codes_nester-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clu_codes_nester-1.3.0.tar", last modified: Sun May 28 23:10:17 2023, max compression
+gzip compressed data, was "clu_codes_nester-1.4.0.tar", last modified: Mon May 29 19:41:54 2023, max compression
```

## Comparing `clu_codes_nester-1.3.0.tar` & `clu_codes_nester-1.4.0.tar`

### file list

```diff
@@ -1,3 +1,9 @@
-drwxr-xr-x   0 Connor     (501) staff       (20)        0 2023-05-28 23:10:17.575853 clu_codes_nester-1.3.0/
--rw-r--r--   0 Connor     (501) staff       (20)      229 2023-05-28 23:10:17.575914 clu_codes_nester-1.3.0/PKG-INFO
--rw-r--r--   0 Connor     (501) staff       (20)      246 2023-05-28 23:05:40.153680 clu_codes_nester-1.3.0/setup.py
+drwxr-xr-x   0 Connor     (501) staff       (20)        0 2023-05-29 19:41:54.009083 clu_codes_nester-1.4.0/
+-rw-r--r--   0 Connor     (501) staff       (20)      154 2023-05-29 19:41:54.008969 clu_codes_nester-1.4.0/PKG-INFO
+drwxr-xr-x   0 Connor     (501) staff       (20)        0 2023-05-29 19:41:54.008818 clu_codes_nester-1.4.0/clu_codes_nester.egg-info/
+-rw-r--r--   0 Connor     (501) staff       (20)      154 2023-05-29 19:41:54.000000 clu_codes_nester-1.4.0/clu_codes_nester.egg-info/PKG-INFO
+-rw-r--r--   0 Connor     (501) staff       (20)      168 2023-05-29 19:41:54.000000 clu_codes_nester-1.4.0/clu_codes_nester.egg-info/SOURCES.txt
+-rw-r--r--   0 Connor     (501) staff       (20)        1 2023-05-29 19:41:54.000000 clu_codes_nester-1.4.0/clu_codes_nester.egg-info/dependency_links.txt
+-rw-r--r--   0 Connor     (501) staff       (20)       17 2023-05-29 19:41:54.000000 clu_codes_nester-1.4.0/clu_codes_nester.egg-info/top_level.txt
+-rw-r--r--   0 Connor     (501) staff       (20)       38 2023-05-29 19:41:54.009117 clu_codes_nester-1.4.0/setup.cfg
+-rw-r--r--   0 Connor     (501) staff       (20)      314 2023-05-29 19:14:07.000000 clu_codes_nester-1.4.0/setup.py
```


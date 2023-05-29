# Comparing `tmp/muuusiiik-0.0.5.tar.gz` & `tmp/muuusiiik-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/muuusiiik-0.0.5.tar", last modified: Tue Aug 23 02:07:02 2022, max compression
+gzip compressed data, was "dist/muuusiiik-0.0.6.tar", last modified: Tue Aug 23 03:05:10 2022, max compression
```

## Comparing `muuusiiik-0.0.5.tar` & `muuusiiik-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 prejudice  (1000) prejudice  (1000)        0 2022-08-23 02:07:02.000000 muuusiiik-0.0.5/
--rwxr-xr-x   0 prejudice  (1000) prejudice  (1000)     1075 2022-08-22 17:16:11.000000 muuusiiik-0.0.5/LICENSE
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)      416 2022-08-23 02:07:02.000000 muuusiiik-0.0.5/PKG-INFO
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)       10 2022-08-22 08:07:19.000000 muuusiiik-0.0.5/README.md
-drwxr-xr-x   0 prejudice  (1000) prejudice  (1000)        0 2022-08-23 02:07:02.000000 muuusiiik-0.0.5/muuusiiik/
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)        0 2022-08-22 17:13:21.000000 muuusiiik-0.0.5/muuusiiik/__init__.py
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)       37 2022-08-22 17:41:11.000000 muuusiiik-0.0.5/muuusiiik/util.py
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)     6129 2022-08-22 17:40:20.000000 muuusiiik-0.0.5/muuusiiik/util2.py
-drwxr-xr-x   0 prejudice  (1000) prejudice  (1000)        0 2022-08-23 02:07:02.000000 muuusiiik-0.0.5/muuusiiik.egg-info/
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)      416 2022-08-23 02:07:02.000000 muuusiiik-0.0.5/muuusiiik.egg-info/PKG-INFO
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)      249 2022-08-23 02:07:02.000000 muuusiiik-0.0.5/muuusiiik.egg-info/SOURCES.txt
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)        1 2022-08-23 02:07:02.000000 muuusiiik-0.0.5/muuusiiik.egg-info/dependency_links.txt
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)       33 2022-08-23 02:07:02.000000 muuusiiik-0.0.5/muuusiiik.egg-info/requires.txt
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)        1 2022-08-23 02:07:02.000000 muuusiiik-0.0.5/muuusiiik.egg-info/top_level.txt
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)       38 2022-08-23 02:07:02.000000 muuusiiik-0.0.5/setup.cfg
--rw-r--r--   0 prejudice  (1000) prejudice  (1000)     1063 2022-08-23 02:06:36.000000 muuusiiik-0.0.5/setup.py
+drwxr-xr-x   0 prejudice  (1000) prejudice  (1000)        0 2022-08-23 03:05:10.000000 muuusiiik-0.0.6/
+-rwxr-xr-x   0 prejudice  (1000) prejudice  (1000)     1075 2022-08-22 17:16:11.000000 muuusiiik-0.0.6/LICENSE
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)      439 2022-08-23 03:05:10.000000 muuusiiik-0.0.6/PKG-INFO
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)       10 2022-08-22 08:07:19.000000 muuusiiik-0.0.6/README.md
+drwxr-xr-x   0 prejudice  (1000) prejudice  (1000)        0 2022-08-23 03:05:10.000000 muuusiiik-0.0.6/muuusiiik/
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)        0 2022-08-22 17:13:21.000000 muuusiiik-0.0.6/muuusiiik/__init__.py
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)       37 2022-08-22 17:41:11.000000 muuusiiik-0.0.6/muuusiiik/util.py
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)     6129 2022-08-22 17:40:20.000000 muuusiiik-0.0.6/muuusiiik/util2.py
+drwxr-xr-x   0 prejudice  (1000) prejudice  (1000)        0 2022-08-23 03:05:10.000000 muuusiiik-0.0.6/muuusiiik.egg-info/
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)      439 2022-08-23 03:05:10.000000 muuusiiik-0.0.6/muuusiiik.egg-info/PKG-INFO
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)      249 2022-08-23 03:05:10.000000 muuusiiik-0.0.6/muuusiiik.egg-info/SOURCES.txt
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)        1 2022-08-23 03:05:10.000000 muuusiiik-0.0.6/muuusiiik.egg-info/dependency_links.txt
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)       12 2022-08-23 03:05:10.000000 muuusiiik-0.0.6/muuusiiik.egg-info/requires.txt
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)        1 2022-08-23 03:05:10.000000 muuusiiik-0.0.6/muuusiiik.egg-info/top_level.txt
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)       38 2022-08-23 03:05:10.000000 muuusiiik-0.0.6/setup.cfg
+-rw-r--r--   0 prejudice  (1000) prejudice  (1000)     1228 2022-08-23 03:04:34.000000 muuusiiik-0.0.6/setup.py
```

### Comparing `muuusiiik-0.0.5/LICENSE` & `muuusiiik-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `muuusiiik-0.0.5/muuusiiik/util2.py` & `muuusiiik-0.0.6/muuusiiik/util2.py`

 * *Files identical despite different names*


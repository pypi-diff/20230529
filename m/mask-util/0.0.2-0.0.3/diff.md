# Comparing `tmp/mask_util-0.0.2.tar.gz` & `tmp/mask_util-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mask_util-0.0.2.tar", last modified: Mon May 29 04:02:26 2023, max compression
+gzip compressed data, was "dist\mask_util-0.0.3.tar", last modified: Mon May 29 04:14:01 2023, max compression
```

## Comparing `mask_util-0.0.2.tar` & `mask_util-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 04:02:26.472384 mask_util-0.0.2/
--rw-rw-rw-   0        0        0      251 2023-05-29 04:02:26.471388 mask_util-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-05-29 03:21:44.000000 mask_util-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 04:02:26.460381 mask_util-0.0.2/mask_util/
--rw-rw-rw-   0        0        0        0 2023-05-29 04:00:20.000000 mask_util-0.0.2/mask_util/__init__.py
--rw-rw-rw-   0        0        0      305 2023-05-29 03:05:59.000000 mask_util-0.0.2/mask_util/const.py
--rw-rw-rw-   0        0        0      747 2023-05-29 04:00:37.000000 mask_util-0.0.2/mask_util/main.py
--rw-rw-rw-   0        0        0      315 2023-05-29 02:55:36.000000 mask_util-0.0.2/mask_util/replacer.py
-drwxrwxrwx   0        0        0        0 2023-05-29 04:02:26.470389 mask_util-0.0.2/mask_util.egg-info/
--rw-rw-rw-   0        0        0      251 2023-05-29 04:02:26.000000 mask_util-0.0.2/mask_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-29 04:02:26.000000 mask_util-0.0.2/mask_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 04:02:26.000000 mask_util-0.0.2/mask_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-29 04:02:26.000000 mask_util-0.0.2/mask_util.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 04:02:26.472384 mask_util-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      396 2023-05-29 04:02:02.000000 mask_util-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 04:14:01.227246 mask_util-0.0.3/
+-rw-rw-rw-   0        0        0      271 2023-05-29 04:14:01.227246 mask_util-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-05-29 03:21:44.000000 mask_util-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 04:14:01.212696 mask_util-0.0.3/mask_util/
+-rw-rw-rw-   0        0        0        0 2023-05-29 04:00:20.000000 mask_util-0.0.3/mask_util/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-05-29 03:05:59.000000 mask_util-0.0.3/mask_util/const.py
+-rw-rw-rw-   0        0        0      747 2023-05-29 04:00:37.000000 mask_util-0.0.3/mask_util/mask.py
+-rw-rw-rw-   0        0        0      315 2023-05-29 02:55:36.000000 mask_util-0.0.3/mask_util/replacer.py
+drwxrwxrwx   0        0        0        0 2023-05-29 04:14:01.226247 mask_util-0.0.3/mask_util.egg-info/
+-rw-rw-rw-   0        0        0      271 2023-05-29 04:14:01.000000 mask_util-0.0.3/mask_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-29 04:14:01.000000 mask_util-0.0.3/mask_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 04:14:01.000000 mask_util-0.0.3/mask_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-29 04:14:01.000000 mask_util-0.0.3/mask_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 04:14:01.227246 mask_util-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      439 2023-05-29 04:13:59.000000 mask_util-0.0.3/setup.py
```

### Comparing `mask_util-0.0.2/mask_util/main.py` & `mask_util-0.0.3/mask_util/mask.py`

 * *Files identical despite different names*


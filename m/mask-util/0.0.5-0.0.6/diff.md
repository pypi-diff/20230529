# Comparing `tmp/mask_util-0.0.5.tar.gz` & `tmp/mask_util-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mask_util-0.0.5.tar", last modified: Mon May 29 05:04:29 2023, max compression
+gzip compressed data, was "dist\mask_util-0.0.6.tar", last modified: Mon May 29 08:07:21 2023, max compression
```

## Comparing `mask_util-0.0.5.tar` & `mask_util-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 05:04:29.250670 mask_util-0.0.5/
--rw-rw-rw-   0        0        0      271 2023-05-29 05:04:29.250670 mask_util-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       10 2023-05-29 03:21:44.000000 mask_util-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 05:04:29.235061 mask_util-0.0.5/mask_util/
--rw-rw-rw-   0        0        0       32 2023-05-29 05:04:13.000000 mask_util-0.0.5/mask_util/__init__.py
--rw-rw-rw-   0        0        0      305 2023-05-29 03:05:59.000000 mask_util-0.0.5/mask_util/const.py
--rw-rw-rw-   0        0        0      747 2023-05-29 04:00:37.000000 mask_util-0.0.5/mask_util/mask.py
--rw-rw-rw-   0        0        0      315 2023-05-29 02:55:36.000000 mask_util-0.0.5/mask_util/replacer.py
-drwxrwxrwx   0        0        0        0 2023-05-29 05:04:29.249667 mask_util-0.0.5/mask_util.egg-info/
--rw-rw-rw-   0        0        0      271 2023-05-29 05:04:29.000000 mask_util-0.0.5/mask_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      231 2023-05-29 05:04:29.000000 mask_util-0.0.5/mask_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 05:04:29.000000 mask_util-0.0.5/mask_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-29 05:04:29.000000 mask_util-0.0.5/mask_util.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 05:04:29.250670 mask_util-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      439 2023-05-29 05:04:26.000000 mask_util-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:07:21.873155 mask_util-0.0.6/
+-rw-rw-rw-   0        0        0      271 2023-05-29 08:07:21.872159 mask_util-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       10 2023-05-29 03:21:44.000000 mask_util-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 08:07:21.839151 mask_util-0.0.6/mask_util/
+-rw-rw-rw-   0        0        0       32 2023-05-29 05:04:13.000000 mask_util-0.0.6/mask_util/__init__.py
+-rw-rw-rw-   0        0        0      305 2023-05-29 03:05:59.000000 mask_util-0.0.6/mask_util/const.py
+-rw-rw-rw-   0        0        0      775 2023-05-29 08:07:07.000000 mask_util-0.0.6/mask_util/mask.py
+-rw-rw-rw-   0        0        0      315 2023-05-29 02:55:36.000000 mask_util-0.0.6/mask_util/replacer.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:07:21.870160 mask_util-0.0.6/mask_util.egg-info/
+-rw-rw-rw-   0        0        0      271 2023-05-29 08:07:21.000000 mask_util-0.0.6/mask_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-05-29 08:07:21.000000 mask_util-0.0.6/mask_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 08:07:21.000000 mask_util-0.0.6/mask_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-29 08:07:21.000000 mask_util-0.0.6/mask_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 08:07:21.873155 mask_util-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      439 2023-05-29 08:07:18.000000 mask_util-0.0.6/setup.py
```


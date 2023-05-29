# Comparing `tmp/ccmplots-0.1.1.tar.gz` & `tmp/ccmplots-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccmplots-0.1.1.tar", last modified: Mon May 29 09:35:52 2023, max compression
+gzip compressed data, was "ccmplots-0.1.2.tar", last modified: Mon May 29 09:38:12 2023, max compression
```

## Comparing `ccmplots-0.1.1.tar` & `ccmplots-0.1.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:35:52.650848 ccmplots-0.1.1/
--rw-rw-r--   0 torben    (1000) torben    (1000)       25 2023-05-27 11:41:16.000000 ccmplots-0.1.1/MANIFEST.in
--rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-05-29 09:35:52.650848 ccmplots-0.1.1/PKG-INFO
--rw-rw-r--   0 torben    (1000) torben    (1000)     1540 2023-05-29 08:40:44.000000 ccmplots-0.1.1/README.md
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:35:52.650848 ccmplots-0.1.1/ccmplots/
--rw-rw-r--   0 torben    (1000) torben    (1000)      942 2023-05-27 10:34:26.000000 ccmplots-0.1.1/ccmplots/__init__.py
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:35:52.650848 ccmplots-0.1.1/ccmplots/styles/
--rw-rw-r--   0 torben    (1000) torben    (1000)     1280 2023-05-29 08:20:50.000000 ccmplots-0.1.1/ccmplots/styles/ccm.mplstyle
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:35:52.650848 ccmplots-0.1.1/ccmplots/styles/customization/
--rw-rw-r--   0 torben    (1000) torben    (1000)       81 2023-05-29 09:34:47.000000 ccmplots-0.1.1/ccmplots/styles/customization/large_font.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)       39 2023-05-27 13:56:20.000000 ccmplots-0.1.1/ccmplots/styles/customization/no-latex.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)      429 2023-05-29 08:08:15.000000 ccmplots-0.1.1/ccmplots/styles/customization/sans.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)       91 2023-05-27 13:50:17.000000 ccmplots-0.1.1/ccmplots/styles/customization/square.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)      107 2023-05-29 08:41:08.000000 ccmplots-0.1.1/ccmplots/styles/customization/tum4c.mplstyle
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:35:52.650848 ccmplots-0.1.1/ccmplots.egg-info/
--rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-05-29 09:35:52.000000 ccmplots-0.1.1/ccmplots.egg-info/PKG-INFO
--rw-rw-r--   0 torben    (1000) torben    (1000)      478 2023-05-29 09:35:52.000000 ccmplots-0.1.1/ccmplots.egg-info/SOURCES.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)        1 2023-05-29 09:35:52.000000 ccmplots-0.1.1/ccmplots.egg-info/dependency_links.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)       55 2023-05-29 09:35:52.000000 ccmplots-0.1.1/ccmplots.egg-info/requires.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)        9 2023-05-29 09:35:52.000000 ccmplots-0.1.1/ccmplots.egg-info/top_level.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)      225 2023-05-29 09:35:42.000000 ccmplots-0.1.1/pyproject.toml
--rw-rw-r--   0 torben    (1000) torben    (1000)       38 2023-05-29 09:35:52.650848 ccmplots-0.1.1/setup.cfg
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:38:12.383209 ccmplots-0.1.2/
+-rw-rw-r--   0 torben    (1000) torben    (1000)       25 2023-05-27 11:41:16.000000 ccmplots-0.1.2/MANIFEST.in
+-rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-05-29 09:38:12.383209 ccmplots-0.1.2/PKG-INFO
+-rw-rw-r--   0 torben    (1000) torben    (1000)     1540 2023-05-29 08:40:44.000000 ccmplots-0.1.2/README.md
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:38:12.383209 ccmplots-0.1.2/ccmplots/
+-rw-rw-r--   0 torben    (1000) torben    (1000)      942 2023-05-27 10:34:26.000000 ccmplots-0.1.2/ccmplots/__init__.py
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:38:12.383209 ccmplots-0.1.2/ccmplots/styles/
+-rw-rw-r--   0 torben    (1000) torben    (1000)     1280 2023-05-29 08:20:50.000000 ccmplots-0.1.2/ccmplots/styles/ccm.mplstyle
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:38:12.383209 ccmplots-0.1.2/ccmplots/styles/customization/
+-rw-rw-r--   0 torben    (1000) torben    (1000)       85 2023-05-29 09:37:45.000000 ccmplots-0.1.2/ccmplots/styles/customization/large_font.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)       39 2023-05-27 13:56:20.000000 ccmplots-0.1.2/ccmplots/styles/customization/no-latex.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)      429 2023-05-29 08:08:15.000000 ccmplots-0.1.2/ccmplots/styles/customization/sans.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)       91 2023-05-27 13:50:17.000000 ccmplots-0.1.2/ccmplots/styles/customization/square.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)      107 2023-05-29 08:41:08.000000 ccmplots-0.1.2/ccmplots/styles/customization/tum4c.mplstyle
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 09:38:12.383209 ccmplots-0.1.2/ccmplots.egg-info/
+-rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-05-29 09:38:12.000000 ccmplots-0.1.2/ccmplots.egg-info/PKG-INFO
+-rw-rw-r--   0 torben    (1000) torben    (1000)      478 2023-05-29 09:38:12.000000 ccmplots-0.1.2/ccmplots.egg-info/SOURCES.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)        1 2023-05-29 09:38:12.000000 ccmplots-0.1.2/ccmplots.egg-info/dependency_links.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)       55 2023-05-29 09:38:12.000000 ccmplots-0.1.2/ccmplots.egg-info/requires.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)        9 2023-05-29 09:38:12.000000 ccmplots-0.1.2/ccmplots.egg-info/top_level.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)      225 2023-05-29 09:38:02.000000 ccmplots-0.1.2/pyproject.toml
+-rw-rw-r--   0 torben    (1000) torben    (1000)       38 2023-05-29 09:38:12.383209 ccmplots-0.1.2/setup.cfg
```

### Comparing `ccmplots-0.1.1/README.md` & `ccmplots-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ccmplots-0.1.1/ccmplots/__init__.py` & `ccmplots-0.1.2/ccmplots/__init__.py`

 * *Files identical despite different names*

### Comparing `ccmplots-0.1.1/ccmplots/styles/ccm.mplstyle` & `ccmplots-0.1.2/ccmplots/styles/ccm.mplstyle`

 * *Files identical despite different names*


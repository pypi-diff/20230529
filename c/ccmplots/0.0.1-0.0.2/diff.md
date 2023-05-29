# Comparing `tmp/ccmplots-0.0.1.tar.gz` & `tmp/ccmplots-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccmplots-0.0.1.tar", last modified: Sat May 27 14:32:16 2023, max compression
+gzip compressed data, was "ccmplots-0.0.2.tar", last modified: Mon May 29 07:09:34 2023, max compression
```

## Comparing `ccmplots-0.0.1.tar` & `ccmplots-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-27 14:32:16.975960 ccmplots-0.0.1/
--rw-rw-r--   0 torben    (1000) torben    (1000)       25 2023-05-27 11:41:16.000000 ccmplots-0.0.1/MANIFEST.in
--rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-05-27 14:32:16.975960 ccmplots-0.0.1/PKG-INFO
--rw-rw-r--   0 torben    (1000) torben    (1000)      969 2023-05-27 13:16:21.000000 ccmplots-0.0.1/README.md
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-27 14:32:16.975960 ccmplots-0.0.1/ccmplots/
--rw-rw-r--   0 torben    (1000) torben    (1000)      942 2023-05-27 10:34:26.000000 ccmplots-0.0.1/ccmplots/__init__.py
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-27 14:32:16.975960 ccmplots-0.0.1/ccmplots/styles/
--rw-rw-r--   0 torben    (1000) torben    (1000)     1257 2023-05-27 14:31:25.000000 ccmplots-0.0.1/ccmplots/styles/ccm.mplstyle
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-27 14:32:16.975960 ccmplots-0.0.1/ccmplots/styles/customization/
--rw-rw-r--   0 torben    (1000) torben    (1000)       39 2023-05-27 13:56:20.000000 ccmplots-0.0.1/ccmplots/styles/customization/no-latex.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)      440 2023-05-27 14:30:54.000000 ccmplots-0.0.1/ccmplots/styles/customization/sans.mplstyle
--rw-rw-r--   0 torben    (1000) torben    (1000)       91 2023-05-27 13:50:17.000000 ccmplots-0.0.1/ccmplots/styles/customization/square.mplstyle
-drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-27 14:32:16.975960 ccmplots-0.0.1/ccmplots.egg-info/
--rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-05-27 14:32:16.000000 ccmplots-0.0.1/ccmplots.egg-info/PKG-INFO
--rw-rw-r--   0 torben    (1000) torben    (1000)      383 2023-05-27 14:32:16.000000 ccmplots-0.0.1/ccmplots.egg-info/SOURCES.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)        1 2023-05-27 14:32:16.000000 ccmplots-0.0.1/ccmplots.egg-info/dependency_links.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)       55 2023-05-27 14:32:16.000000 ccmplots-0.0.1/ccmplots.egg-info/requires.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)        9 2023-05-27 14:32:16.000000 ccmplots-0.0.1/ccmplots.egg-info/top_level.txt
--rw-rw-r--   0 torben    (1000) torben    (1000)      225 2023-05-27 11:41:55.000000 ccmplots-0.0.1/pyproject.toml
--rw-rw-r--   0 torben    (1000) torben    (1000)       38 2023-05-27 14:32:16.975960 ccmplots-0.0.1/setup.cfg
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 07:09:34.116048 ccmplots-0.0.2/
+-rw-rw-r--   0 torben    (1000) torben    (1000)       25 2023-05-27 11:41:16.000000 ccmplots-0.0.2/MANIFEST.in
+-rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-05-29 07:09:34.116048 ccmplots-0.0.2/PKG-INFO
+-rw-rw-r--   0 torben    (1000) torben    (1000)     1094 2023-05-27 14:56:19.000000 ccmplots-0.0.2/README.md
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 07:09:34.116048 ccmplots-0.0.2/ccmplots/
+-rw-rw-r--   0 torben    (1000) torben    (1000)      942 2023-05-27 10:34:26.000000 ccmplots-0.0.2/ccmplots/__init__.py
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 07:09:34.116048 ccmplots-0.0.2/ccmplots/styles/
+-rw-rw-r--   0 torben    (1000) torben    (1000)     1257 2023-05-29 07:08:47.000000 ccmplots-0.0.2/ccmplots/styles/ccm.mplstyle
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 07:09:34.116048 ccmplots-0.0.2/ccmplots/styles/customization/
+-rw-rw-r--   0 torben    (1000) torben    (1000)       39 2023-05-27 13:56:20.000000 ccmplots-0.0.2/ccmplots/styles/customization/no-latex.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)      431 2023-05-29 07:09:06.000000 ccmplots-0.0.2/ccmplots/styles/customization/sans.mplstyle
+-rw-rw-r--   0 torben    (1000) torben    (1000)       91 2023-05-27 13:50:17.000000 ccmplots-0.0.2/ccmplots/styles/customization/square.mplstyle
+drwxrwxr-x   0 torben    (1000) torben    (1000)        0 2023-05-29 07:09:34.116048 ccmplots-0.0.2/ccmplots.egg-info/
+-rw-rw-r--   0 torben    (1000) torben    (1000)       52 2023-05-29 07:09:34.000000 ccmplots-0.0.2/ccmplots.egg-info/PKG-INFO
+-rw-rw-r--   0 torben    (1000) torben    (1000)      383 2023-05-29 07:09:34.000000 ccmplots-0.0.2/ccmplots.egg-info/SOURCES.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)        1 2023-05-29 07:09:34.000000 ccmplots-0.0.2/ccmplots.egg-info/dependency_links.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)       55 2023-05-29 07:09:34.000000 ccmplots-0.0.2/ccmplots.egg-info/requires.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)        9 2023-05-29 07:09:34.000000 ccmplots-0.0.2/ccmplots.egg-info/top_level.txt
+-rw-rw-r--   0 torben    (1000) torben    (1000)      225 2023-05-28 07:24:38.000000 ccmplots-0.0.2/pyproject.toml
+-rw-rw-r--   0 torben    (1000) torben    (1000)       38 2023-05-29 07:09:34.116048 ccmplots-0.0.2/setup.cfg
```

### Comparing `ccmplots-0.0.1/ccmplots/__init__.py` & `ccmplots-0.0.2/ccmplots/__init__.py`

 * *Files identical despite different names*

### Comparing `ccmplots-0.0.1/ccmplots/styles/ccm.mplstyle` & `ccmplots-0.0.2/ccmplots/styles/ccm.mplstyle`

 * *Files 4% similar despite different names*

```diff
@@ -46,14 +46,14 @@
 
 # Use LaTeX for math formatting
 # text.usetex : True
 
 # Use serif fonts
 # font.serif : Times
 font.family : serif
-font.serif: TeX Gyre Termes
+font.serif: Times New Roman
 
 # Font Sizes
 font.size: 8
 axes.titlesize: 8
 xtick.labelsize: 8
 ytick.labelsize: 8
```


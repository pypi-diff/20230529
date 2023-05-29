# Comparing `tmp/vbarongdatools001-0.0.3.tar.gz` & `tmp/vbarongdatools001-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbarongdatools001-0.0.3.tar", last modified: Fri May 26 11:16:28 2023, max compression
+gzip compressed data, was "vbarongdatools001-0.0.4.tar", last modified: Mon May 29 07:09:24 2023, max compression
```

## Comparing `vbarongdatools001-0.0.3.tar` & `vbarongdatools001-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 11:16:28.461959 vbarongdatools001-0.0.3/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 vbarongdatools001-0.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 vbarongdatools001-0.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      397 2023-05-26 11:16:28.461959 vbarongdatools001-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 vbarongdatools001-0.0.3/README.md
--rw-rw-rw-   0        0        0      136 2023-05-26 11:16:28.462960 vbarongdatools001-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-05-26 10:19:41.000000 vbarongdatools001-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 11:16:28.448978 vbarongdatools001-0.0.3/vbarongdatools001/
--rw-rw-rw-   0        0        0    53248 2023-05-26 11:15:29.000000 vbarongdatools001-0.0.3/vbarongdatools001/Vbalog.pyd
--rw-rw-rw-   0        0        0        0 2023-05-26 10:19:22.000000 vbarongdatools001-0.0.3/vbarongdatools001/__init__.py
--rw-rw-rw-   0        0        0    69120 2023-05-26 11:15:39.000000 vbarongdatools001-0.0.3/vbarongdatools001/vbaLogin.pyd
--rw-rw-rw-   0        0        0    48640 2023-05-26 11:15:55.000000 vbarongdatools001-0.0.3/vbarongdatools001/vbarongdatools001.pyd
-drwxrwxrwx   0        0        0        0 2023-05-26 11:16:28.459960 vbarongdatools001-0.0.3/vbarongdatools001.egg-info/
--rw-rw-rw-   0        0        0      397 2023-05-26 11:16:28.000000 vbarongdatools001-0.0.3/vbarongdatools001.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-05-26 11:16:28.000000 vbarongdatools001-0.0.3/vbarongdatools001.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 11:16:28.000000 vbarongdatools001-0.0.3/vbarongdatools001.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-26 11:16:28.000000 vbarongdatools001-0.0.3/vbarongdatools001.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 07:09:24.262997 vbarongdatools001-0.0.4/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 vbarongdatools001-0.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 vbarongdatools001-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      397 2023-05-29 07:09:24.263999 vbarongdatools001-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 vbarongdatools001-0.0.4/README.md
+-rw-rw-rw-   0        0        0      136 2023-05-29 07:09:24.266991 vbarongdatools001-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      979 2023-05-29 07:09:00.000000 vbarongdatools001-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:09:24.231988 vbarongdatools001-0.0.4/vbarongdatools001/
+-rw-rw-rw-   0        0        0    53248 2023-05-26 11:15:29.000000 vbarongdatools001-0.0.4/vbarongdatools001/Vbalog.pyd
+-rw-rw-rw-   0        0        0        0 2023-05-26 10:19:22.000000 vbarongdatools001-0.0.4/vbarongdatools001/__init__.py
+-rw-rw-rw-   0        0        0    69120 2023-05-26 11:15:39.000000 vbarongdatools001-0.0.4/vbarongdatools001/vbaLogin.pyd
+-rw-rw-rw-   0        0        0    48640 2023-05-26 11:15:55.000000 vbarongdatools001-0.0.4/vbarongdatools001/vbarongdatools001.pyd
+-rw-rw-rw-   0        0        0   813770 2023-05-26 10:40:08.000000 vbarongdatools001-0.0.4/vbarongdatools001/批量移动或重命名文件、创建文件夹-V0001.xlsm
+drwxrwxrwx   0        0        0        0 2023-05-29 07:09:24.258986 vbarongdatools001-0.0.4/vbarongdatools001.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-05-29 07:09:24.000000 vbarongdatools001-0.0.4/vbarongdatools001.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2023-05-29 07:09:24.000000 vbarongdatools001-0.0.4/vbarongdatools001.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 07:09:24.000000 vbarongdatools001-0.0.4/vbarongdatools001.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-29 07:09:24.000000 vbarongdatools001-0.0.4/vbarongdatools001.egg-info/top_level.txt
```

### Comparing `vbarongdatools001-0.0.3/LICENSE.txt` & `vbarongdatools001-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vbarongdatools001-0.0.3/setup.py` & `vbarongdatools001-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
-PATCH = 3
+PATCH = 4
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "vbarongdatools001",
@@ -26,11 +26,11 @@
     packages=find_packages(),
     # license = '',
     classifiers=[
         'Programming Language :: Python',
 
     ],
     # 包含的类型
-    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db']},  # 这个很重要
+    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db', '*.xlsm']},  # 这个很重要
     include_package_data=True  # 也选上
 
 )
```


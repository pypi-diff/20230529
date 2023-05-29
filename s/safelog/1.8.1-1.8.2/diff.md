# Comparing `tmp/safelog-1.8.1.tar.gz` & `tmp/safelog-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "safelog-1.8.1.tar", last modified: Wed May 24 08:08:46 2023, max compression
+gzip compressed data, was "safelog-1.8.2.tar", last modified: Mon May 29 12:21:23 2023, max compression
```

## Comparing `safelog-1.8.1.tar` & `safelog-1.8.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:46.438609 safelog-1.8.1/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       32 2022-04-23 12:12:52.000000 safelog-1.8.1/MANIFEST.in
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5783 2023-05-24 08:08:46.438609 safelog-1.8.1/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3779 2023-05-24 06:13:24.000000 safelog-1.8.1/README.md
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:46.438609 safelog-1.8.1/safelog.egg-info/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5783 2023-05-24 08:08:46.000000 safelog-1.8.1/safelog.egg-info/PKG-INFO
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)      228 2023-05-24 08:08:46.000000 safelog-1.8.1/safelog.egg-info/SOURCES.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2023-05-24 08:08:46.000000 safelog-1.8.1/safelog.egg-info/dependency_links.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       10 2023-05-24 08:08:46.000000 safelog-1.8.1/safelog.egg-info/requires.txt
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       12 2023-05-24 08:08:46.000000 safelog-1.8.1/safelog.egg-info/top_level.txt
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:46.438609 safelog-1.8.1/sbin/
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)    10690 2023-05-24 08:08:46.000000 safelog-1.8.1/sbin/safelog
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2023-05-24 08:08:46.438609 safelog-1.8.1/setup.cfg
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1683 2023-05-24 08:08:46.000000 safelog-1.8.1/setup.py
-drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-24 08:08:46.438609 safelog-1.8.1/src/
--rw-r--r--   0 ramblin   (1000) ramblin   (1000)        0 2022-04-23 12:12:53.000000 safelog-1.8.1/src/__init__.py
--rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)    10690 2023-05-18 00:05:30.000000 safelog-1.8.1/src/safelog.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:21:23.479695 safelog-1.8.2/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       32 2022-04-23 12:12:52.000000 safelog-1.8.2/MANIFEST.in
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5783 2023-05-29 12:21:23.479695 safelog-1.8.2/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     3779 2023-05-24 06:13:24.000000 safelog-1.8.2/README.md
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:21:23.479695 safelog-1.8.2/safelog.egg-info/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     5783 2023-05-29 12:21:23.000000 safelog-1.8.2/safelog.egg-info/PKG-INFO
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)      228 2023-05-29 12:21:23.000000 safelog-1.8.2/safelog.egg-info/SOURCES.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        1 2023-05-29 12:21:23.000000 safelog-1.8.2/safelog.egg-info/dependency_links.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       10 2023-05-29 12:21:23.000000 safelog-1.8.2/safelog.egg-info/requires.txt
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       12 2023-05-29 12:21:23.000000 safelog-1.8.2/safelog.egg-info/top_level.txt
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:21:23.479695 safelog-1.8.2/sbin/
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)    10690 2023-05-29 12:21:22.000000 safelog-1.8.2/sbin/safelog
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)       38 2023-05-29 12:21:23.479695 safelog-1.8.2/setup.cfg
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)     1683 2023-05-29 12:21:22.000000 safelog-1.8.2/setup.py
+drwxr-xr-x   0 ramblin   (1000) ramblin   (1000)        0 2023-05-29 12:21:23.479695 safelog-1.8.2/src/
+-rw-r--r--   0 ramblin   (1000) ramblin   (1000)        0 2022-04-23 12:12:53.000000 safelog-1.8.2/src/__init__.py
+-rwxr-xr-x   0 ramblin   (1000) ramblin   (1000)    10690 2023-05-29 12:16:22.000000 safelog-1.8.2/src/safelog.py
```

### Comparing `safelog-1.8.1/PKG-INFO` & `safelog-1.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safelog
-Version: 1.8.1
+Version: 1.8.2
 Summary: Safelog is a multithread, multiprocess, multiinstance logging package.
 Home-page: https://github.com/safeapps/safelog/
 Author: safeapps
 Maintainer: safeapps
 License: GNU General Public License v3 (GPLv3)
 Download-URL: https://github.com/safeapps/safelog/
 Project-URL: Source Code, https://github.com/safeapps/safelog/
```

### Comparing `safelog-1.8.1/README.md` & `safelog-1.8.2/README.md`

 * *Files identical despite different names*

### Comparing `safelog-1.8.1/safelog.egg-info/PKG-INFO` & `safelog-1.8.2/safelog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: safelog
-Version: 1.8.1
+Version: 1.8.2
 Summary: Safelog is a multithread, multiprocess, multiinstance logging package.
 Home-page: https://github.com/safeapps/safelog/
 Author: safeapps
 Maintainer: safeapps
 License: GNU General Public License v3 (GPLv3)
 Download-URL: https://github.com/safeapps/safelog/
 Project-URL: Source Code, https://github.com/safeapps/safelog/
```

### Comparing `safelog-1.8.1/sbin/safelog` & `safelog-1.8.2/sbin/safelog`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # in solidlibs.python.log so they can be imported easily by tools
 from solidlibs.python.log import SAFELOG_HOST, SAFELOG_PORT, FIELD_SEPARATOR
 # safelog itself uses the alternative logging in solidlibs.python._log
 from solidlibs.python._log import log as tmp_log
 from solidlibs.python.times import timestamp
 
 
-CURRENT_VERSION = '1.8.1'
+CURRENT_VERSION = '1.8.2'
 COPYRIGHT = 'Copyright 2019-2023 safeapps'
 LICENSE = 'GPLv3'
 
 # must be distinct from solidlibs.python.log.FIELD_SEPARATOR
 NEWLINE_SUBSTITUTE = '\x02'
 
 # analogous to /var/log
```

### Comparing `safelog-1.8.1/setup.py` & `safelog-1.8.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
     Set up for safelog
 
     Copyright 2018-2023 safeapps
-    Last modified: 2023-05-24
+    Last modified: 2023-05-29
 '''
 
 import os.path
 import setuptools
 
 # read long description
 with open(os.path.join(os.path.dirname(__file__), 'README.md'), 'r') as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="safelog",
-    version="1.8.1",
+    version="1.8.2",
     author="safeapps",
     maintainer="safeapps",
     description="Safelog is a multithread, multiprocess, multiinstance logging package.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="logging multiprocess multithread multi-instance",
     license="GNU General Public License v3 (GPLv3)",
```

### Comparing `safelog-1.8.1/src/safelog.py` & `safelog-1.8.2/src/safelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 # in solidlibs.python.log so they can be imported easily by tools
 from solidlibs.python.log import SAFELOG_HOST, SAFELOG_PORT, FIELD_SEPARATOR
 # safelog itself uses the alternative logging in solidlibs.python._log
 from solidlibs.python._log import log as tmp_log
 from solidlibs.python.times import timestamp
 
 
-CURRENT_VERSION = '1.8.1'
+CURRENT_VERSION = '1.8.2'
 COPYRIGHT = 'Copyright 2019-2023 safeapps'
 LICENSE = 'GPLv3'
 
 # must be distinct from solidlibs.python.log.FIELD_SEPARATOR
 NEWLINE_SUBSTITUTE = '\x02'
 
 # analogous to /var/log
```


# Comparing `tmp/rasterstats-0.9.1.zip` & `tmp/rasterstats-0.9.2.zip`

## zipinfo {}

```diff
@@ -1,20 +1,21 @@
-Zip file size: 27079 bytes, number of entries: 18
--rw-r--r--  2.0 unx     1482 b- defN 15-Feb-04 03:29 rasterstats-0.9.1/LICENSE.txt
--rw-r--r--  2.0 unx    12274 b- defN 15-Sep-27 14:10 rasterstats-0.9.1/PKG-INFO
--rw-r--r--  2.0 unx     9415 b- defN 15-Sep-27 13:58 rasterstats-0.9.1/README.rst
--rw-r--r--  2.0 unx      153 b- defN 15-Sep-27 14:10 rasterstats-0.9.1/setup.cfg
--rw-r--r--  2.0 unx     1707 b- defN 15-Sep-27 14:09 rasterstats-0.9.1/setup.py
--rw-r--r--  2.0 unx      192 b- defN 15-Sep-27 13:58 rasterstats-0.9.1/src/rasterstats/__init__.py
--rw-r--r--  2.0 unx     4911 b- defN 15-Sep-27 13:58 rasterstats-0.9.1/src/rasterstats/cli.py
--rw-r--r--  2.0 unx     9375 b- defN 15-Sep-27 13:58 rasterstats-0.9.1/src/rasterstats/io.py
--rw-r--r--  2.0 unx     9285 b- defN 15-Sep-27 13:58 rasterstats-0.9.1/src/rasterstats/main.py
--rw-r--r--  2.0 unx     4651 b- defN 15-Sep-27 14:05 rasterstats-0.9.1/src/rasterstats/point.py
--rw-r--r--  2.0 unx     3628 b- defN 15-Sep-27 13:58 rasterstats-0.9.1/src/rasterstats/utils.py
--rw-r--r--  2.0 unx        1 b- defN 15-Sep-27 14:10 rasterstats-0.9.1/src/rasterstats.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx      123 b- defN 15-Sep-27 14:10 rasterstats-0.9.1/src/rasterstats.egg-info/entry_points.txt
--rw-r--r--  2.0 unx       47 b- defN 15-Jul-28 11:24 rasterstats-0.9.1/src/rasterstats.egg-info/pbr.json
--rw-r--r--  2.0 unx    12274 b- defN 15-Sep-27 14:10 rasterstats-0.9.1/src/rasterstats.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       29 b- defN 15-Sep-27 14:10 rasterstats-0.9.1/src/rasterstats.egg-info/requires.txt
--rw-r--r--  2.0 unx      458 b- defN 15-Sep-27 14:10 rasterstats-0.9.1/src/rasterstats.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       12 b- defN 15-Sep-27 14:10 rasterstats-0.9.1/src/rasterstats.egg-info/top_level.txt
-18 files, 70017 bytes uncompressed, 24141 bytes compressed:  65.5%
+Zip file size: 27469 bytes, number of entries: 19
+-rw-r--r--  2.0 unx     1482 b- defN 15-Feb-04 03:29 rasterstats-0.9.2/LICENSE.txt
+-rw-r--r--  2.0 unx    12274 b- defN 15-Oct-12 12:46 rasterstats-0.9.2/PKG-INFO
+-rw-r--r--  2.0 unx     9415 b- defN 15-Sep-27 13:58 rasterstats-0.9.2/README.rst
+-rw-r--r--  2.0 unx      153 b- defN 15-Oct-12 12:46 rasterstats-0.9.2/setup.cfg
+-rw-r--r--  2.0 unx     2131 b- defN 15-Oct-12 12:31 rasterstats-0.9.2/setup.py
+-rw-r--r--  2.0 unx      237 b- defN 15-Oct-12 12:32 rasterstats-0.9.2/src/rasterstats/__init__.py
+-rw-r--r--  2.0 unx       22 b- defN 15-Oct-12 12:24 rasterstats-0.9.2/src/rasterstats/_version.py
+-rw-r--r--  2.0 unx     4953 b- defN 15-Oct-12 12:35 rasterstats-0.9.2/src/rasterstats/cli.py
+-rw-r--r--  2.0 unx     9375 b- defN 15-Oct-07 10:19 rasterstats-0.9.2/src/rasterstats/io.py
+-rw-r--r--  2.0 unx     9285 b- defN 15-Oct-12 12:16 rasterstats-0.9.2/src/rasterstats/main.py
+-rw-r--r--  2.0 unx     4651 b- defN 15-Sep-27 14:11 rasterstats-0.9.2/src/rasterstats/point.py
+-rw-r--r--  2.0 unx     3628 b- defN 15-Oct-12 12:16 rasterstats-0.9.2/src/rasterstats/utils.py
+-rw-r--r--  2.0 unx        1 b- defN 15-Oct-12 12:46 rasterstats-0.9.2/src/rasterstats.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx      123 b- defN 15-Oct-12 12:46 rasterstats-0.9.2/src/rasterstats.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       47 b- defN 15-Jul-28 11:24 rasterstats-0.9.2/src/rasterstats.egg-info/pbr.json
+-rw-r--r--  2.0 unx    12274 b- defN 15-Oct-12 12:46 rasterstats-0.9.2/src/rasterstats.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       29 b- defN 15-Oct-12 12:46 rasterstats-0.9.2/src/rasterstats.egg-info/requires.txt
+-rw-r--r--  2.0 unx      486 b- defN 15-Oct-12 12:46 rasterstats-0.9.2/src/rasterstats.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       12 b- defN 15-Oct-12 12:46 rasterstats-0.9.2/src/rasterstats.egg-info/top_level.txt
+19 files, 70578 bytes uncompressed, 24365 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -1,55 +1,58 @@
-Filename: rasterstats-0.9.1/LICENSE.txt
+Filename: rasterstats-0.9.2/LICENSE.txt
 Comment: 
 
-Filename: rasterstats-0.9.1/PKG-INFO
+Filename: rasterstats-0.9.2/PKG-INFO
 Comment: 
 
-Filename: rasterstats-0.9.1/README.rst
+Filename: rasterstats-0.9.2/README.rst
 Comment: 
 
-Filename: rasterstats-0.9.1/setup.cfg
+Filename: rasterstats-0.9.2/setup.cfg
 Comment: 
 
-Filename: rasterstats-0.9.1/setup.py
+Filename: rasterstats-0.9.2/setup.py
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats/__init__.py
+Filename: rasterstats-0.9.2/src/rasterstats/__init__.py
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats/cli.py
+Filename: rasterstats-0.9.2/src/rasterstats/_version.py
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats/io.py
+Filename: rasterstats-0.9.2/src/rasterstats/cli.py
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats/main.py
+Filename: rasterstats-0.9.2/src/rasterstats/io.py
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats/point.py
+Filename: rasterstats-0.9.2/src/rasterstats/main.py
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats/utils.py
+Filename: rasterstats-0.9.2/src/rasterstats/point.py
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats.egg-info/dependency_links.txt
+Filename: rasterstats-0.9.2/src/rasterstats/utils.py
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats.egg-info/entry_points.txt
+Filename: rasterstats-0.9.2/src/rasterstats.egg-info/dependency_links.txt
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats.egg-info/pbr.json
+Filename: rasterstats-0.9.2/src/rasterstats.egg-info/entry_points.txt
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats.egg-info/PKG-INFO
+Filename: rasterstats-0.9.2/src/rasterstats.egg-info/pbr.json
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats.egg-info/requires.txt
+Filename: rasterstats-0.9.2/src/rasterstats.egg-info/PKG-INFO
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats.egg-info/SOURCES.txt
+Filename: rasterstats-0.9.2/src/rasterstats.egg-info/requires.txt
 Comment: 
 
-Filename: rasterstats-0.9.1/src/rasterstats.egg-info/top_level.txt
+Filename: rasterstats-0.9.2/src/rasterstats.egg-info/SOURCES.txt
+Comment: 
+
+Filename: rasterstats-0.9.2/src/rasterstats.egg-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## Comparing `rasterstats-0.9.1/LICENSE.txt` & `rasterstats-0.9.2/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `rasterstats-0.9.1/PKG-INFO` & `rasterstats-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rasterstats
-Version: 0.9.1
+Version: 0.9.2
 Summary: Summarize geospatial raster datasets based on vector geometries
 Home-page: https://github.com/perrygeo/python-raster-stats
 Author: Matthew Perry
 Author-email: perrygeo@gmail.com
 License: BSD
 Description: rasterstats
         ===========
```

## Comparing `rasterstats-0.9.1/README.rst` & `rasterstats-0.9.2/README.rst`

 * *Files identical despite different names*

## Comparing `rasterstats-0.9.1/setup.py` & `rasterstats-0.9.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,45 @@
 import os
 import sys
+import re
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
+def get_version():
+    vfile = os.path.join(
+        os.path.dirname(__file__), "src", "rasterstats", "_version.py")
+    with open(vfile, "r") as vfh:
+        vline = vfh.read()
+    vregex = r"^__version__ = ['\"]([^'\"]*)['\"]"
+    match = re.search(vregex, vline, re.M)
+    if match:
+        return match.group(1)
+    else:
+        raise RuntimeError("Unable to find version string in {}.".format(vfile))
+
 class PyTest(TestCommand):
     def finalize_options(self):
         TestCommand.finalize_options(self)
         self.test_args = []
         self.test_suite = True
 
     def run_tests(self):
         import pytest
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
 
 setup(
     name="rasterstats",
-    version='0.9.1',
+    version=get_version(),
     author="Matthew Perry",
     author_email="perrygeo@gmail.com",
     description=("Summarize geospatial raster datasets based on vector geometries"),
     license="BSD",
     keywords="gis geospatial geographic raster vector zonal statistics",
     url="https://github.com/perrygeo/python-raster-stats",
     package_dir={'': 'src'},
```

## Comparing `rasterstats-0.9.1/src/rasterstats/cli.py` & `rasterstats-0.9.2/src/rasterstats/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # -*- coding: utf-8 -*-
 from __future__ import absolute_import
 from __future__ import division
 import click
 from rasterstats import zonal_stats, point_query
 from rasterstats.io import read_features
+from rasterstats._version import __version__ as version
 import logging
 try:
     import simplejson as json
 except:
     import json
 
 SETTINGS = dict(help_option_names=['-h', '--help'])
-version = 0.9
 
 
 @click.command(context_settings=SETTINGS)
 @click.argument('input-geojson', type=click.File('r'), default='-')
 @click.argument('output-geojson', type=click.File('w'), default='-')
 @click.version_option(version=version, message='%(version)s')
 @click.option('--raster', '-r', required=True, type=click.Path(exists=True))
```

## Comparing `rasterstats-0.9.1/src/rasterstats/io.py` & `rasterstats-0.9.2/src/rasterstats/io.py`

 * *Files identical despite different names*

## Comparing `rasterstats-0.9.1/src/rasterstats/main.py` & `rasterstats-0.9.2/src/rasterstats/main.py`

 * *Files identical despite different names*

## Comparing `rasterstats-0.9.1/src/rasterstats/point.py` & `rasterstats-0.9.2/src/rasterstats/point.py`

 * *Files identical despite different names*

## Comparing `rasterstats-0.9.1/src/rasterstats/utils.py` & `rasterstats-0.9.2/src/rasterstats/utils.py`

 * *Files identical despite different names*

## Comparing `rasterstats-0.9.1/src/rasterstats.egg-info/PKG-INFO` & `rasterstats-0.9.2/src/rasterstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: rasterstats
-Version: 0.9.1
+Version: 0.9.2
 Summary: Summarize geospatial raster datasets based on vector geometries
 Home-page: https://github.com/perrygeo/python-raster-stats
 Author: Matthew Perry
 Author-email: perrygeo@gmail.com
 License: BSD
 Description: rasterstats
         ===========
```


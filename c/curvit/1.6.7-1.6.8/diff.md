# Comparing `tmp/curvit-1.6.7.tar.gz` & `tmp/curvit-1.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curvit-1.6.7.tar", last modified: Fri May 19 14:11:25 2023, max compression
+gzip compressed data, was "curvit-1.6.8.tar", last modified: Mon May 29 13:11:43 2023, max compression
```

## Comparing `curvit-1.6.7.tar` & `curvit-1.6.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-19 14:11:25.337669 curvit-1.6.7/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.6.7/LICENSE
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-05-19 14:11:25.336669 curvit-1.6.7/PKG-INFO
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.6.7/README.md
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-19 14:11:25.333669 curvit-1.6.7/curvit/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      170 2023-05-07 09:10:32.000000 curvit-1.6.7/curvit/__init__.py
--rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.6.7/curvit/check_curvit_variability_V.0.4.py
--rwxr-xr-x   0 prajwel   (1000) prajwel   (1000)    76299 2023-05-19 12:12:29.000000 curvit-1.6.7/curvit/curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      352 2023-05-07 09:10:59.000000 curvit-1.6.7/curvit/profile_curvit.py
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      939 2023-05-07 09:11:38.000000 curvit-1.6.7/curvit/test_curvit.py
-drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-19 14:11:25.336669 curvit-1.6.7/curvit.egg-info/
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-05-19 14:11:25.000000 curvit-1.6.7/curvit.egg-info/PKG-INFO
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2023-05-19 14:11:25.000000 curvit-1.6.7/curvit.egg-info/SOURCES.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-05-19 14:11:25.000000 curvit-1.6.7/curvit.egg-info/dependency_links.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       75 2023-05-19 14:11:25.000000 curvit-1.6.7/curvit.egg-info/requires.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2023-05-19 14:11:25.000000 curvit-1.6.7/curvit.egg-info/top_level.txt
--rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-05-19 14:11:25.337669 curvit-1.6.7/setup.cfg
--rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      847 2023-05-19 12:28:28.000000 curvit-1.6.7/setup.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-29 13:11:43.678469 curvit-1.6.8/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)    11358 2019-12-14 12:44:39.000000 curvit-1.6.8/LICENSE
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-05-29 13:11:43.678469 curvit-1.6.8/PKG-INFO
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)     1184 2023-03-22 17:29:10.000000 curvit-1.6.8/README.md
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-29 13:11:43.676469 curvit-1.6.8/curvit/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      170 2023-05-07 09:10:32.000000 curvit-1.6.8/curvit/__init__.py
+-rwxr--r--   0 prajwel   (1000) prajwel   (1000)     1157 2020-11-26 05:54:42.000000 curvit-1.6.8/curvit/check_curvit_variability_V.0.4.py
+-rwxr-xr-x   0 prajwel   (1000) prajwel   (1000)    76303 2023-05-29 13:07:17.000000 curvit-1.6.8/curvit/curvit.py
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      352 2023-05-07 09:10:59.000000 curvit-1.6.8/curvit/profile_curvit.py
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      939 2023-05-07 09:11:38.000000 curvit-1.6.8/curvit/test_curvit.py
+drwxr-xr-x   0 prajwel   (1000) prajwel   (1000)        0 2023-05-29 13:11:43.677469 curvit-1.6.8/curvit.egg-info/
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)     1622 2023-05-29 13:11:43.000000 curvit-1.6.8/curvit.egg-info/PKG-INFO
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)      299 2023-05-29 13:11:43.000000 curvit-1.6.8/curvit.egg-info/SOURCES.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        1 2023-05-29 13:11:43.000000 curvit-1.6.8/curvit.egg-info/dependency_links.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       75 2023-05-29 13:11:43.000000 curvit-1.6.8/curvit.egg-info/requires.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)        7 2023-05-29 13:11:43.000000 curvit-1.6.8/curvit.egg-info/top_level.txt
+-rw-r--r--   0 prajwel   (1000) prajwel   (1000)       38 2023-05-29 13:11:43.678469 curvit-1.6.8/setup.cfg
+-rw-rw-r--   0 prajwel   (1000) prajwel   (1000)      847 2023-05-29 13:10:04.000000 curvit-1.6.8/setup.py
```

### Comparing `curvit-1.6.7/LICENSE` & `curvit-1.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `curvit-1.6.7/PKG-INFO` & `curvit-1.6.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.6.7
+Version: 1.6.8
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.6.7 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.6.8 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # **Curvit** >
 Create light curves from UVIT data. [ascl:2101.013] [https://img.shields.io/
 pypi/v/curvit?color=262255] [![Documentation Status](https://readthedocs.org/
```

### Comparing `curvit-1.6.7/README.md` & `curvit-1.6.8/README.md`

 * *Files identical despite different names*

### Comparing `curvit-1.6.7/curvit/check_curvit_variability_V.0.4.py` & `curvit-1.6.8/curvit/check_curvit_variability_V.0.4.py`

 * *Files identical despite different names*

### Comparing `curvit-1.6.7/curvit/curvit.py` & `curvit-1.6.8/curvit/curvit.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,15 +159,15 @@
 the field and no rotation between frames."""
 shift_algorithm = "multiple_star"  # 'single_star' or 'multiple_star'.
 
 min_exptime = 30  # will ignore orbits with exptimes below limit.
 
 # Aafitrans defaults.
 num_nearest_neighbors = 8
-min_matches = 1
+min_matches = 4
 pixel_tolerance = 2
 
 # For Astrometry.
 AstrometryNet_API_key = "ujmrvwqqyelxmzcj"
 
 # For curve_orbitwise
 time_separation = 30 * 60  # seconds
@@ -1802,15 +1802,15 @@
         The number of nearest neighbors of a given star (including itself)
         to construct the triangle invariants for matching.
         The default value is 8. Only relevant for ``'multiple_star'`` method.
 
     min_matches : int, optional
         The minimum number of triangle matches to be found. A value of 1
         refers to 1 triangle, corresponding to 3 pairs of coordinates.
-        The default value is 1. Only relevant for ``'multiple_star'`` method.
+        The default value is 4. Only relevant for ``'multiple_star'`` method.
 
     pixel_tolerance : int, optional
         The maximum residual error for matches.
         The default value is 2. Only relevant for ``'multiple_star'`` method.
 
     minimum_detections : int, optional
         The minimum number of sources to be detected. The threshold will be
@@ -1891,15 +1891,15 @@
                 if threshold <= 1:
                     print("If you see this, please contact Curvit developer.")
                     break
             while len(uA) > maximum_detections:
                 uA = new_detect_sources_daofind(
                     fx, fy, photons, threshold, framecount_per_sec
                 )
-                threshold = 2 * threshold
+                threshold = 1.5 * threshold
                 if threshold >= 1e20:
                     print("If you see this, please contact Curvit developer.")
                     break
         else:
             while len(uA) <= minimum_detections:
                 uA = new_detect_sources_daofind(
                     fx, fy, photons, threshold, framecount_per_sec
@@ -1908,15 +1908,15 @@
                 if threshold <= 1:
                     print("If you see this, please contact Curvit developer.")
                     break
             while len(uA) > maximum_detections:
                 uA = new_detect_sources_daofind(
                     fx, fy, photons, threshold, framecount_per_sec
                 )
-                threshold = 2 * threshold
+                threshold = 1.5 * threshold
                 if threshold >= 1e20:
                     print("If you see this, please contact Curvit developer.")
                     break
 
         print("{} sources detected in {}".format(len(uA), path))
 
         exptimes.append(time.max() - time.min())
```

### Comparing `curvit-1.6.7/curvit/test_curvit.py` & `curvit-1.6.8/curvit/test_curvit.py`

 * *Files identical despite different names*

### Comparing `curvit-1.6.7/curvit.egg-info/PKG-INFO` & `curvit-1.6.8/curvit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: curvit
-Version: 1.6.7
+Version: 1.6.8
 Summary: light curves from UVIT data
 Home-page: https://github.com/prajwel/curvit
 Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: curvit Version: 1.6.7 Summary: light curves from
+Metadata-Version: 2.1 Name: curvit Version: 1.6.8 Summary: light curves from
 UVIT data Home-page: https://github.com/prajwel/curvit Author: Prajwel Joseph
 Author-email: prajwel.joseph@gmail.com Classifier: Programming Language ::
 Python :: 3 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE # **Curvit** >
 Create light curves from UVIT data. [ascl:2101.013] [https://img.shields.io/
 pypi/v/curvit?color=262255] [![Documentation Status](https://readthedocs.org/
```

### Comparing `curvit-1.6.7/setup.py` & `curvit-1.6.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="curvit",
-    version="1.6.7",
+    version="1.6.8",
     author="Prajwel Joseph",
     author_email="prajwel.joseph@gmail.com",
     description="light curves from UVIT data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/prajwel/curvit",
     packages=setuptools.find_packages(),
```


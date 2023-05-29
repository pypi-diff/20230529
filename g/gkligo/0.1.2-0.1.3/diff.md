# Comparing `tmp/gkligo-0.1.2.tar.gz` & `tmp/gkligo-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.1.2.tar", last modified: Wed May 24 22:13:54 2023, max compression
+gzip compressed data, was "gkligo-0.1.3.tar", last modified: Mon May 29 09:49:15 2023, max compression
```

## Comparing `gkligo-0.1.2.tar` & `gkligo-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-24 22:13:54.411365 gkligo-0.1.2/
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.2/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-24 22:13:54.410944 gkligo-0.1.2/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)     1089 2023-05-24 11:09:44.000000 gkligo-0.1.2/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-24 22:13:54.399936 gkligo-0.1.2/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.2/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-05-24 22:13:17.000000 gkligo-0.1.2/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-24 22:13:54.402663 gkligo-0.1.2/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.2/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-24 22:13:54.409805 gkligo-0.1.2/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.2/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.2/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.2/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.2/gkligo/scripts/python/config_reports_example.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)    11625 2023-05-24 11:05:54.000000 gkligo-0.1.2/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     5667 2023-05-24 22:12:22.000000 gkligo-0.1.2/gkligo/scripts/python/generateGWReports.py
--rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.2/gkligo/scripts/python/test.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.2/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-24 22:13:54.402285 gkligo-0.1.2/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-24 22:13:54.000000 gkligo-0.1.2/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      610 2023-05-24 22:13:54.000000 gkligo-0.1.2/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-05-24 22:13:54.000000 gkligo-0.1.2/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      147 2023-05-24 22:13:54.000000 gkligo-0.1.2/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       85 2023-05-24 22:13:54.000000 gkligo-0.1.2/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-05-24 22:13:54.000000 gkligo-0.1.2/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-05-24 22:13:54.411643 gkligo-0.1.2/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.2/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:49:15.449783 gkligo-0.1.3/
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.3/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 09:49:15.449422 gkligo-0.1.3/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)     1089 2023-05-24 11:09:44.000000 gkligo-0.1.3/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:49:15.438520 gkligo-0.1.3/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.3/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-05-29 09:48:35.000000 gkligo-0.1.3/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:49:15.441495 gkligo-0.1.3/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.3/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:49:15.448513 gkligo-0.1.3/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2023-05-28 12:23:50.000000 gkligo-0.1.3/gkligo/scripts/python/=
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.3/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.3/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.3/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.3/gkligo/scripts/python/config_reports_example.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)    12893 2023-05-29 09:47:08.000000 gkligo-0.1.3/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     5793 2023-05-26 22:32:11.000000 gkligo-0.1.3/gkligo/scripts/python/generateGWReports.py
+-rw-r--r--   0 kws        (502) staff       (20)      267 2023-05-26 22:38:03.000000 gkligo-0.1.3/gkligo/scripts/python/test.py
+-rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.3/gkligo/scripts/python/test.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.3/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:49:15.441100 gkligo-0.1.3/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      664 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      147 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-05-29 09:49:15.449970 gkligo-0.1.3/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.3/setup.py
```

### Comparing `gkligo-0.1.2/PKG-INFO` & `gkligo-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.1.2
+Version: 0.1.3
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkligo
         Code to download GW Alert skymaps from Kafka, and optionally write them
```

### Comparing `gkligo-0.1.2/README.md` & `gkligo-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.2/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.1.3/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,38 +54,70 @@
 from io import BytesIO
 import daemon
 from daemon import pidfile
 import signal
 import os
 import time
 import logging
+from copy import deepcopy
 
 def shutdown(signum, frame):  # signum and frame are mandatory
     """shutdown.
 
     Args:
         signum:
         frame:
     """
     sys.stdout.write("\nOuch...\n")
     sys.exit(0)
 
 
+def getContourArea(inputFilePointer, contour, logger):
+
+    from astropy.table import Table
+    from astropy import units as u
+    import numpy as np
+    import math
+    from ligo.skymap.moc import uniq2pixarea
+
+    # Read and verify the input
+    skymap = Table.read(inputFilePointer, format='fits')
+
+    # Sort by prob density of pixel
+    skymap.sort('PROBDENSITY', reverse=True)
+
+    # Get area*probdensity for each pixel
+    pixel_area = uniq2pixarea(skymap['UNIQ'])
+
+    # Probability per pixel
+    prob = pixel_area*skymap['PROBDENSITY']
+    cumprob = np.cumsum(prob)
+
+    # Should be 1.0. But need not be.
+    sumprob = np.sum(prob)
+
+    # Find the index where contour of prob is inside
+    i = cumprob.searchsorted(contour*sumprob)
+    area = float(pixel_area[:i].sum() * (180/math.pi)**2)
+
+    return area
+
+
+
 def writeMOC(inputFilePointer, outputMOCName, contour, logger):
     """writeMOC.
 
     Args:
         inputFilePointer:
         outputMOCName:
         contour:
         logger:
     """
     from astropy.table import Table
     from astropy import units as u
-    import astropy_healpix as ah
     import numpy as np
     import math
     from ligo.skymap.moc import uniq2pixarea
 
     # Read and verify the input
     skymap = Table.read(inputFilePointer, format='fits')
     #print('Input multi-order skymap:')
@@ -125,16 +157,23 @@
     from astropy.io import fits
 
     mjd = None
     distance = None
     distanceStd = None
     eventMeta = {}
 
+    dataDictCopy = deepcopy(dataDict)
+    skymap = dataDictCopy['event']['skymap']
+
+    areas = {}
+    for c in options.contours:
+        areas['area' + str(c) = getContourArea(BytesIO(base64.b64decode(skymap)), float(c)/100.0, logger)
+
     # Some info (e.g. distance) only in the FITS file
-    h = fits.open(BytesIO(base64.b64decode(dataDict['event']['skymap'])))
+    h = fits.open(BytesIO(base64.b64decode(skymap)))
     header = h[1].header
 
     try:
         mjd = header['MJD-OBS']
     except KeyError as e:
         logger.error("The MJD-OBS variable is missing.")
 
@@ -150,16 +189,26 @@
 
     # Do NOT write to the database, which could potentially be locked and crash the
     # daemon. Write another script (e.g the reports script) that does that. Just
     # record the metadata for loading.
 
 
     # Remove the skymap from the dictionary.
-    dataDict['event'].pop('skymap')
-    eventMeta = {'ALERT': dataDict,
+    try:
+        dataDictCopy['event'].pop('skymap')
+    except KeyError as e:
+        pass
+
+    try:
+        dataDictCopy.pop('external_coinc')
+    except KeyError as e:
+        pass
+
+    eventMeta = {'ALERT': dataDictCopy,
+                 'EXTRA': areas,
                  'HEADER': {'MJD-OBS': mjd,
                             'DISTMEAN': distance,
                             'DISTSTD': distanceStd}}
 
     return eventMeta
 
  
@@ -239,14 +288,15 @@
                             c = float(contour)/100.0
                             writeMOC(BytesIO(base64.b64decode(skymap)), options.directory + '/' + alertName + '_' + contour + '.moc', c, logger)
                         except ValueError as e:
                             logger.error("Contour %s is not a float" % contour)
 
 
             except KeyError as e:
+                logger.error("Something went wrong.")
                 logger.error(e)
                 pass
             logger.info("")
 
 
 def startDaemon(options):
     """startDaemon.
```

### Comparing `gkligo-0.1.2/gkligo/scripts/python/generateGWReports.py` & `gkligo-0.1.3/gkligo/scripts/python/generateGWReports.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,22 @@
 import sys
 __doc__ = __doc__ % (sys.argv[0], sys.argv[0], sys.argv[0], sys.argv[0])
 from docopt import docopt
 import os, shutil, re, csv, subprocess
 from gkutils.commonutils import Struct, cleanOptions, dbConnect
 import MySQLdb
 
+def getFiles(regex, directory):
+
+    fileList = glob.glob(directory + '/' + regex)
+
+    fileList.sort()
+
+    return fileList
+
 
 def getATLASExposures(conn, options):
 
     try:
         cursor = conn.cursor (MySQLdb.cursors.DictCursor)
 
         cursor.execute ("""
```

### Comparing `gkligo-0.1.2/gkligo/scripts/python/test.yaml` & `gkligo-0.1.3/gkligo/scripts/python/test.yaml`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.2/gkligo/scripts/python/testDaemon.py` & `gkligo-0.1.3/gkligo/scripts/python/testDaemon.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.2/gkligo.egg-info/PKG-INFO` & `gkligo-0.1.3/gkligo.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.1.2
+Version: 0.1.3
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkligo
         Code to download GW Alert skymaps from Kafka, and optionally write them
```

### Comparing `gkligo-0.1.2/gkligo.egg-info/SOURCES.txt` & `gkligo-0.1.3/gkligo.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 gkligo.egg-info/PKG-INFO
 gkligo.egg-info/SOURCES.txt
 gkligo.egg-info/dependency_links.txt
 gkligo.egg-info/entry_points.txt
 gkligo.egg-info/requires.txt
 gkligo.egg-info/top_level.txt
 gkligo/scripts/__init__.py
+gkligo/scripts/python/=
 gkligo/scripts/python/__init__.py
 gkligo/scripts/python/config_download_example.yaml
 gkligo/scripts/python/config_reports.yaml
 gkligo/scripts/python/config_reports_example.yaml
 gkligo/scripts/python/downloadGWAlerts.py
 gkligo/scripts/python/generateGWReports.py
+gkligo/scripts/python/test.py
 gkligo/scripts/python/test.yaml
 gkligo/scripts/python/testDaemon.py
```

### Comparing `gkligo-0.1.2/setup.py` & `gkligo-0.1.3/setup.py`

 * *Files identical despite different names*


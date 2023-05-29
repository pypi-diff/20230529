# Comparing `tmp/gkligo-0.1.3.tar.gz` & `tmp/gkligo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gkligo-0.1.3.tar", last modified: Mon May 29 09:49:15 2023, max compression
+gzip compressed data, was "gkligo-0.1.4.tar", last modified: Mon May 29 09:57:49 2023, max compression
```

## Comparing `gkligo-0.1.3.tar` & `gkligo-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:49:15.449783 gkligo-0.1.3/
--rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.3/MANIFEST.in
--rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 09:49:15.449422 gkligo-0.1.3/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)     1089 2023-05-24 11:09:44.000000 gkligo-0.1.3/README.md
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:49:15.438520 gkligo-0.1.3/gkligo/
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.3/gkligo/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       22 2023-05-29 09:48:35.000000 gkligo-0.1.3/gkligo/__version__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:49:15.441495 gkligo-0.1.3/gkligo/scripts/
--rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.3/gkligo/scripts/__init__.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:49:15.448513 gkligo-0.1.3/gkligo/scripts/python/
--rw-r--r--   0 kws        (502) staff       (20)        0 2023-05-28 12:23:50.000000 gkligo-0.1.3/gkligo/scripts/python/=
--rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.3/gkligo/scripts/python/__init__.py
--rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.3/gkligo/scripts/python/config_download_example.yaml
--rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.3/gkligo/scripts/python/config_reports.yaml
--rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.3/gkligo/scripts/python/config_reports_example.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)    12893 2023-05-29 09:47:08.000000 gkligo-0.1.3/gkligo/scripts/python/downloadGWAlerts.py
--rwxr-xr-x   0 kws        (502) staff       (20)     5793 2023-05-26 22:32:11.000000 gkligo-0.1.3/gkligo/scripts/python/generateGWReports.py
--rw-r--r--   0 kws        (502) staff       (20)      267 2023-05-26 22:38:03.000000 gkligo-0.1.3/gkligo/scripts/python/test.py
--rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.3/gkligo/scripts/python/test.yaml
--rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.3/gkligo/scripts/python/testDaemon.py
-drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:49:15.441100 gkligo-0.1.3/gkligo.egg-info/
--rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/PKG-INFO
--rw-r--r--   0 kws        (502) staff       (20)      664 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/SOURCES.txt
--rw-r--r--   0 kws        (502) staff       (20)        1 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/dependency_links.txt
--rw-r--r--   0 kws        (502) staff       (20)      147 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/entry_points.txt
--rw-r--r--   0 kws        (502) staff       (20)       85 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/requires.txt
--rw-r--r--   0 kws        (502) staff       (20)        7 2023-05-29 09:49:15.000000 gkligo-0.1.3/gkligo.egg-info/top_level.txt
--rw-r--r--   0 kws        (502) staff       (20)       38 2023-05-29 09:49:15.449970 gkligo-0.1.3/setup.cfg
--rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.3/setup.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:57:49.134206 gkligo-0.1.4/
+-rw-r--r--   0 kws        (502) staff       (20)       74 2023-03-08 21:39:07.000000 gkligo-0.1.4/MANIFEST.in
+-rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 09:57:49.133827 gkligo-0.1.4/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)     1089 2023-05-24 11:09:44.000000 gkligo-0.1.4/README.md
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:57:49.120690 gkligo-0.1.4/gkligo/
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-04-28 14:27:19.000000 gkligo-0.1.4/gkligo/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       22 2023-05-29 09:56:45.000000 gkligo-0.1.4/gkligo/__version__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:57:49.124251 gkligo-0.1.4/gkligo/scripts/
+-rw-r--r--   0 kws        (502) staff       (20)       21 2023-03-08 21:34:47.000000 gkligo-0.1.4/gkligo/scripts/__init__.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:57:49.132548 gkligo-0.1.4/gkligo/scripts/python/
+-rw-r--r--   0 kws        (502) staff       (20)        0 2023-05-28 12:23:50.000000 gkligo-0.1.4/gkligo/scripts/python/=
+-rw-r--r--   0 kws        (502) staff       (20)       31 2023-04-28 14:27:05.000000 gkligo-0.1.4/gkligo/scripts/python/__init__.py
+-rw-r--r--   0 kws        (502) staff       (20)       89 2023-04-20 16:53:23.000000 gkligo-0.1.4/gkligo/scripts/python/config_download_example.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      426 2023-04-24 12:50:06.000000 gkligo-0.1.4/gkligo/scripts/python/config_reports.yaml
+-rw-r--r--   0 kws        (502) staff       (20)      498 2023-04-24 13:37:26.000000 gkligo-0.1.4/gkligo/scripts/python/config_reports_example.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)    12894 2023-05-29 09:56:23.000000 gkligo-0.1.4/gkligo/scripts/python/downloadGWAlerts.py
+-rwxr-xr-x   0 kws        (502) staff       (20)     5793 2023-05-26 22:32:11.000000 gkligo-0.1.4/gkligo/scripts/python/generateGWReports.py
+-rw-r--r--   0 kws        (502) staff       (20)      267 2023-05-26 22:38:03.000000 gkligo-0.1.4/gkligo/scripts/python/test.py
+-rw-r--r--   0 kws        (502) staff       (20)     1266 2023-05-23 20:34:59.000000 gkligo-0.1.4/gkligo/scripts/python/test.yaml
+-rwxr-xr-x   0 kws        (502) staff       (20)     2792 2023-04-27 21:33:22.000000 gkligo-0.1.4/gkligo/scripts/python/testDaemon.py
+drwxr-xr-x   0 kws        (502) staff       (20)        0 2023-05-29 09:57:49.123563 gkligo-0.1.4/gkligo.egg-info/
+-rw-r--r--   0 kws        (502) staff       (20)     1794 2023-05-29 09:57:49.000000 gkligo-0.1.4/gkligo.egg-info/PKG-INFO
+-rw-r--r--   0 kws        (502) staff       (20)      664 2023-05-29 09:57:49.000000 gkligo-0.1.4/gkligo.egg-info/SOURCES.txt
+-rw-r--r--   0 kws        (502) staff       (20)        1 2023-05-29 09:57:49.000000 gkligo-0.1.4/gkligo.egg-info/dependency_links.txt
+-rw-r--r--   0 kws        (502) staff       (20)      147 2023-05-29 09:57:49.000000 gkligo-0.1.4/gkligo.egg-info/entry_points.txt
+-rw-r--r--   0 kws        (502) staff       (20)       85 2023-05-29 09:57:49.000000 gkligo-0.1.4/gkligo.egg-info/requires.txt
+-rw-r--r--   0 kws        (502) staff       (20)        7 2023-05-29 09:57:49.000000 gkligo-0.1.4/gkligo.egg-info/top_level.txt
+-rw-r--r--   0 kws        (502) staff       (20)       38 2023-05-29 09:57:49.134405 gkligo-0.1.4/setup.cfg
+-rwxr-xr-x   0 kws        (502) staff       (20)     1308 2023-04-24 13:23:15.000000 gkligo-0.1.4/setup.py
```

### Comparing `gkligo-0.1.3/PKG-INFO` & `gkligo-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.1.3
+Version: 0.1.4
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkligo
         Code to download GW Alert skymaps from Kafka, and optionally write them
```

### Comparing `gkligo-0.1.3/README.md` & `gkligo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.3/gkligo/scripts/python/downloadGWAlerts.py` & `gkligo-0.1.4/gkligo/scripts/python/downloadGWAlerts.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
     eventMeta = {}
 
     dataDictCopy = deepcopy(dataDict)
     skymap = dataDictCopy['event']['skymap']
 
     areas = {}
     for c in options.contours:
-        areas['area' + str(c) = getContourArea(BytesIO(base64.b64decode(skymap)), float(c)/100.0, logger)
+        areas['area' + str(c)] = getContourArea(BytesIO(base64.b64decode(skymap)), float(c)/100.0, logger)
 
     # Some info (e.g. distance) only in the FITS file
     h = fits.open(BytesIO(base64.b64decode(skymap)))
     header = h[1].header
 
     try:
         mjd = header['MJD-OBS']
```

### Comparing `gkligo-0.1.3/gkligo/scripts/python/generateGWReports.py` & `gkligo-0.1.4/gkligo/scripts/python/generateGWReports.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.3/gkligo/scripts/python/test.yaml` & `gkligo-0.1.4/gkligo/scripts/python/test.yaml`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.3/gkligo/scripts/python/testDaemon.py` & `gkligo-0.1.4/gkligo/scripts/python/testDaemon.py`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.3/gkligo.egg-info/PKG-INFO` & `gkligo-0.1.4/gkligo.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gkligo
-Version: 0.1.3
+Version: 0.1.4
 Summary: GW (LIGO) utilities
 Home-page: https://github.com/genghisken/gkligo
 Author: genghisken
 Author-email: ken.w.smith@gmail.com
 License: MIT
 Description: # gkligo
         Code to download GW Alert skymaps from Kafka, and optionally write them
```

### Comparing `gkligo-0.1.3/gkligo.egg-info/SOURCES.txt` & `gkligo-0.1.4/gkligo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gkligo-0.1.3/setup.py` & `gkligo-0.1.4/setup.py`

 * *Files identical despite different names*


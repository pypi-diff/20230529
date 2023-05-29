# Comparing `tmp/obrpy-0.0.8.tar.gz` & `tmp/obrpy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "obrpy-0.0.8.tar", last modified: Thu May 18 15:09:10 2023, max compression
+gzip compressed data, was "obrpy-0.0.9.tar", last modified: Thu May 18 15:40:38 2023, max compression
```

## Comparing `obrpy-0.0.8.tar` & `obrpy-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 15:09:10.910730 obrpy-0.0.8/
--rw-rw-rw-   0        0        0      283 2023-05-18 15:09:10.910730 obrpy-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-18 15:09:10.870723 obrpy-0.0.8/obrpy/
--rw-rw-rw-   0        0        0     1341 2023-02-23 12:03:19.000000 obrpy-0.0.8/obrpy/PathSelector.py
--rw-rw-rw-   0        0        0     8506 2023-05-10 14:51:12.000000 obrpy-0.0.8/obrpy/__init__.py
--rw-rw-rw-   0        0        0     1328 2023-05-10 14:52:06.000000 obrpy-0.0.8/obrpy/checkouts.py
--rw-rw-rw-   0        0        0     1063 2023-05-10 14:43:49.000000 obrpy-0.0.8/obrpy/clear.py
--rw-rw-rw-   0        0        0     2246 2023-05-10 14:46:47.000000 obrpy-0.0.8/obrpy/load.py
--rw-rw-rw-   0        0        0     8323 2023-05-10 11:38:23.000000 obrpy-0.0.8/obrpy/obr.py
--rw-rw-rw-   0        0        0     2123 2023-04-25 15:28:15.000000 obrpy-0.0.8/obrpy/obrsdk.py
--rw-rw-rw-   0        0        0     3212 2023-05-10 14:09:36.000000 obrpy-0.0.8/obrpy/save.py
--rw-rw-rw-   0        0        0     3741 2023-05-10 12:02:20.000000 obrpy-0.0.8/obrpy/settings.py
--rw-rw-rw-   0        0        0     3425 2023-05-03 08:58:35.000000 obrpy-0.0.8/obrpy/take_a_look.py
--rw-rw-rw-   0        0        0     3350 2023-05-10 15:00:23.000000 obrpy-0.0.8/obrpy/update.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:09:10.902723 obrpy-0.0.8/obrpy.egg-info/
--rw-rw-rw-   0        0        0      283 2023-05-18 15:09:10.000000 obrpy-0.0.8/obrpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      351 2023-05-18 15:09:10.000000 obrpy-0.0.8/obrpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 15:09:10.000000 obrpy-0.0.8/obrpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 15:09:10.000000 obrpy-0.0.8/obrpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 15:09:10.000000 obrpy-0.0.8/obrpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-18 15:09:10.910730 obrpy-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1333 2023-05-18 15:08:49.000000 obrpy-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 15:09:10.910730 obrpy-0.0.8/test/
--rw-rw-rw-   0        0        0      812 2023-05-10 14:57:34.000000 obrpy-0.0.8/test/test.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:40:38.900665 obrpy-0.0.9/
+-rw-rw-rw-   0        0        0      283 2023-05-18 15:40:38.899665 obrpy-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-18 15:40:38.875665 obrpy-0.0.9/obrpy/
+-rw-rw-rw-   0        0        0     1341 2023-02-23 12:03:19.000000 obrpy-0.0.9/obrpy/PathSelector.py
+-rw-rw-rw-   0        0        0     8519 2023-05-18 15:40:14.000000 obrpy-0.0.9/obrpy/__init__.py
+-rw-rw-rw-   0        0        0     1328 2023-05-10 14:52:06.000000 obrpy-0.0.9/obrpy/checkouts.py
+-rw-rw-rw-   0        0        0     1063 2023-05-10 14:43:49.000000 obrpy-0.0.9/obrpy/clear.py
+-rw-rw-rw-   0        0        0     2246 2023-05-10 14:46:47.000000 obrpy-0.0.9/obrpy/load.py
+-rw-rw-rw-   0        0        0     8323 2023-05-10 11:38:23.000000 obrpy-0.0.9/obrpy/obr.py
+-rw-rw-rw-   0        0        0     2123 2023-04-25 15:28:15.000000 obrpy-0.0.9/obrpy/obrsdk.py
+-rw-rw-rw-   0        0        0     3212 2023-05-10 14:09:36.000000 obrpy-0.0.9/obrpy/save.py
+-rw-rw-rw-   0        0        0     3741 2023-05-10 12:02:20.000000 obrpy-0.0.9/obrpy/settings.py
+-rw-rw-rw-   0        0        0     3425 2023-05-03 08:58:35.000000 obrpy-0.0.9/obrpy/take_a_look.py
+-rw-rw-rw-   0        0        0     3350 2023-05-10 15:00:23.000000 obrpy-0.0.9/obrpy/update.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:40:38.897667 obrpy-0.0.9/obrpy.egg-info/
+-rw-rw-rw-   0        0        0      283 2023-05-18 15:40:38.000000 obrpy-0.0.9/obrpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-18 15:40:38.000000 obrpy-0.0.9/obrpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-18 15:40:38.000000 obrpy-0.0.9/obrpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 15:40:38.000000 obrpy-0.0.9/obrpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-18 15:40:38.000000 obrpy-0.0.9/obrpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-18 15:40:38.900665 obrpy-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2023-05-18 15:40:35.000000 obrpy-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-18 15:40:38.898665 obrpy-0.0.9/test/
+-rw-rw-rw-   0        0        0      812 2023-05-10 14:57:34.000000 obrpy-0.0.9/test/test.py
```

### Comparing `obrpy-0.0.8/obrpy/PathSelector.py` & `obrpy-0.0.9/obrpy/PathSelector.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.8/obrpy/__init__.py` & `obrpy-0.0.9/obrpy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import os
-import sys
-
-sys.path.append(os.path.join(os.path.dirname(__file__), '..'))
 
+from .SIGNAL.cross_spectrum import PSSS
+from .SIGNAL.spectral_shift import spectral_shift, spectral_shift_GPU
 
 class obrpy(object):
     """
         Main class for correct management of .obr files
 
             Initialization:
             
@@ -143,25 +142,24 @@
             self.T0     = str(self.info['Calibration'].loc[0, 1])
             self.T1     = str(self.info['Calibration'].loc[0, 3])
             self.E0     = str(self.info['Calibration'].loc[1, 1])
             self.E1     = str(self.info['Calibration'].loc[1, 3])
             self.z_ini  = float(self.info['Calibration'].loc[2, 1])
             self.z_fin  = float(self.info['Calibration'].loc[3, 1])
 
-
     class Signal(object):
 
         """ Class to contain all singal analysis functions available """
 
         def __init__(self) -> None:
             pass
 
-
-        from .SIGNAL.cross_spectrum import PSSS
-        from .SIGNAL.spectral_shift import spectral_shift, spectral_shift_GPU
+        PSSS = PSSS
+        spectral_shift = spectral_shift
+        spectral_shift_GPU = spectral_shift_GPU
 
     class Slice(object):
         """
         Container class for one slice
         """
 
         def __init__(self):
```

### Comparing `obrpy-0.0.8/obrpy/checkouts.py` & `obrpy-0.0.9/obrpy/checkouts.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.8/obrpy/clear.py` & `obrpy-0.0.9/obrpy/clear.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.8/obrpy/load.py` & `obrpy-0.0.9/obrpy/load.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.8/obrpy/obr.py` & `obrpy-0.0.9/obrpy/obr.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.8/obrpy/obrsdk.py` & `obrpy-0.0.9/obrpy/obrsdk.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.8/obrpy/save.py` & `obrpy-0.0.9/obrpy/save.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.8/obrpy/settings.py` & `obrpy-0.0.9/obrpy/settings.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.8/obrpy/take_a_look.py` & `obrpy-0.0.9/obrpy/take_a_look.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.8/obrpy/update.py` & `obrpy-0.0.9/obrpy/update.py`

 * *Files identical despite different names*

### Comparing `obrpy-0.0.8/setup.py` & `obrpy-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 from setuptools import find_packages, setup
 
 HERE = pathlib.Path(__file__).parent
 
-VERSION = '0.0.8' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
+VERSION = '0.0.9' #Muy importante, deberéis ir cambiando la versión de vuestra librería según incluyáis nuevas funcionalidades
 PACKAGE_NAME = 'obrpy' #Debe coincidir con el nombre de la carpeta 
 AUTHOR = 'Andres Pedraza Rodriguez' #Modificar con vuestros datos
 AUTHOR_EMAIL = 'a.pedraza@upm.es' #Modificar con vuestros datos
 URL = 'https://github.com/temisAP' #Modificar con vuestros datos
 
 LICENSE = 'MIT' #Tipo de licencia
 DESCRIPTION = "This library is aimed for using Luna's OBR-4600 with Python." #Descripción corta
```

### Comparing `obrpy-0.0.8/test/test.py` & `obrpy-0.0.9/test/test.py`

 * *Files identical despite different names*


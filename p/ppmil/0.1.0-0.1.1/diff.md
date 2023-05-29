# Comparing `tmp/ppmil-0.1.0-py3-none-any.whl.zip` & `tmp/ppmil-0.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 20683 bytes, number of entries: 13
--rw-r--r--  2.0 unx      166 b- defN 23-May-27 19:41 ppmil/__init__.py
--rw-r--r--  2.0 unx       21 b- defN 23-May-27 19:41 ppmil/_version.py
--rw-r--r--  2.0 unx     1524 b- defN 23-May-27 19:41 ppmil/cgf.py
--rw-r--r--  2.0 unx     1603 b- defN 23-May-27 19:41 ppmil/gto.py
--rw-r--r--  2.0 unx     4232 b- defN 23-May-27 19:41 ppmil/integrals.py
--rw-r--r--  2.0 unx     4169 b- defN 23-May-27 19:41 ppmil/molecule.py
--rw-r--r--  2.0 unx     9081 b- defN 23-May-27 19:41 ppmil/ppmil.py
--rw-r--r--  2.0 unx     3331 b- defN 23-May-27 19:41 ppmil/quadrature.py
--rw-r--r--  2.0 unx    35121 b- defN 23-May-27 19:41 ppmil-0.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1090 b- defN 23-May-27 19:41 ppmil-0.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 19:41 ppmil-0.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        6 b- defN 23-May-27 19:41 ppmil-0.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      955 b- defN 23-May-27 19:41 ppmil-0.1.0.dist-info/RECORD
-13 files, 61391 bytes uncompressed, 19123 bytes compressed:  68.9%
+Zip file size: 20977 bytes, number of entries: 13
+-rw-r--r--  2.0 unx      166 b- defN 23-May-29 14:40 ppmil/__init__.py
+-rw-r--r--  2.0 unx       21 b- defN 23-May-29 14:40 ppmil/_version.py
+-rw-r--r--  2.0 unx     1524 b- defN 23-May-29 14:40 ppmil/cgf.py
+-rw-r--r--  2.0 unx     1603 b- defN 23-May-29 14:40 ppmil/gto.py
+-rw-r--r--  2.0 unx     4232 b- defN 23-May-29 14:40 ppmil/integrals.py
+-rw-r--r--  2.0 unx     4169 b- defN 23-May-29 14:40 ppmil/molecule.py
+-rw-r--r--  2.0 unx     9397 b- defN 23-May-29 14:40 ppmil/ppmil.py
+-rw-r--r--  2.0 unx     3522 b- defN 23-May-29 14:40 ppmil/quadrature.py
+-rw-r--r--  2.0 unx    35121 b- defN 23-May-29 14:40 ppmil-0.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1274 b- defN 23-May-29 14:40 ppmil-0.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 14:40 ppmil-0.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        6 b- defN 23-May-29 14:40 ppmil-0.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      955 b- defN 23-May-29 14:40 ppmil-0.1.1.dist-info/RECORD
+13 files, 62082 bytes uncompressed, 19417 bytes compressed:  68.7%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: ppmil/ppmil.py
 Comment: 
 
 Filename: ppmil/quadrature.py
 Comment: 
 
-Filename: ppmil-0.1.0.dist-info/LICENSE
+Filename: ppmil-0.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: ppmil-0.1.0.dist-info/METADATA
+Filename: ppmil-0.1.1.dist-info/METADATA
 Comment: 
 
-Filename: ppmil-0.1.0.dist-info/WHEEL
+Filename: ppmil-0.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ppmil-0.1.0.dist-info/top_level.txt
+Filename: ppmil-0.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ppmil-0.1.0.dist-info/RECORD
+Filename: ppmil-0.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ppmil/_version.py

```diff
@@ -1 +1 @@
-__version__ = "0.1.0"
+__version__ = "0.1.1"
```

## ppmil/ppmil.py

```diff
@@ -1,16 +1,22 @@
 import numpy as np
 import scipy
-import os
 from .cgf import CGF
 from .gto import GTO
+import importlib.util
+import warnings
 
 class PPMIL:
     def __init__(self):
-        pass
+        pylebedev_spec = importlib.util.find_spec('pylebedev')
+        if pylebedev_spec is None:
+            warnings.warn(
+                "Some functionality of PPMIL depends on PyLebedev. "
+                "Please install PyLebedev. See: https://ppmil.imc-tue.nl/installation.html."
+            )
     
     def overlap(self, cgf1, cgf2):
         """
         Calculate overlap integral between two contracted Gaussian functions
         """
         # verify that variables are CGFS
         if not isinstance(cgf1, CGF):
```

## ppmil/quadrature.py

```diff
@@ -5,15 +5,19 @@
 
 class Quadrature:
     def __init__(self):
         try:
             from pylebedev import PyLebedev
             self.leblib = PyLebedev()
         except ImportError:
-            raise Exception('PyLebedev package is not installed.')
+            raise Exception(
+                "PyLebedev package is not installed. "
+                "Please install the PyLebedev package to make use of the"
+                " Quadrature class. See: https://ppmil.imc-tue.nl/installation.html."
+            )
 
     def quad_overlap(self, gto1, gto2, radial_points=32, lebedev_order=31):
         """
         Perform Gauss-Chebychev-Lebedev quadrature on trial wave function
         """        
         # verify that variables are GTOs
         if not isinstance(gto1, GTO):
```

## Comparing `ppmil-0.1.0.dist-info/LICENSE` & `ppmil-0.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ppmil-0.1.0.dist-info/METADATA` & `ppmil-0.1.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ppmil
-Version: 0.1.0
+Version: 0.1.1
 Summary: Python package for constructing Wigner-D matrices
 Home-page: https://github.com/ifilot/ppmil
 Author: Ivo Filot
 Author-email: ivo@ivofilot.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
@@ -12,16 +12,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 
 # Pure Python Molecular Integral Library (PPMIL)
 
+![C/C++ CI](https://img.shields.io/static/v1?label=status&message=under%20development&color=ff0000)
 [![C/C++ CI](https://github.com/ifilot/ppmil/actions/workflows/build.yml/badge.svg)](https://github.com/ifilot/ppmil/actions/workflows/build.yml)
 [![Anaconda-Server Badge](https://anaconda.org/ifilot/ppmil/badges/version.svg)](https://anaconda.org/ifilot/ppmil)
 [![PyPI](https://img.shields.io/pypi/v/ppmil?style=flat-square)](https://pypi.org/project/ppmil/)
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 
+## Documentation
+
+Detailed documentation can be found at https://ppmil.imc-tue.nl.
+
 ## Purpose
 
 Evaluate molecular integrals purely in Python, without the need of any
 compiled libraries.
```

## Comparing `ppmil-0.1.0.dist-info/RECORD` & `ppmil-0.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ppmil/__init__.py,sha256=5mH61PC2hU46YFXB4q-up2OlGHTJusmhrSdJeIhQ5ko,166
-ppmil/_version.py,sha256=Pru0BlFBASFCFo7McHdohtKkUtgMPDwbGfyUZlE2_Vw,21
+ppmil/_version.py,sha256=8oAxKUG747GUokmxjkrWejyJa5yPNEsoJDlXxoedxTw,21
 ppmil/cgf.py,sha256=xhG3SNSpdA4gK4KquGssrnLL2rNujxNKKsCPMakdckI,1524
 ppmil/gto.py,sha256=91c2HCYUO6XI8FnqziS7tgiPsdAkz0bUALxe7mR3XsA,1603
 ppmil/integrals.py,sha256=FyEEs0qf8-2VdiVMCTwCSwkIRSZO7ftDpNeZgvWhkDs,4232
 ppmil/molecule.py,sha256=kPpiVM7fFBvOSHcKO6aX8EMs14q92XNM85tEaxjOcEs,4169
-ppmil/ppmil.py,sha256=2DJzvkOeqR3bkNZm_NYOxa8Q_RfX89vWFMUk42fKDJI,9081
-ppmil/quadrature.py,sha256=Aw3bDMZ-L28WdrIqXBpzhQP6PrSw6GExfxN53wRY_2o,3331
-ppmil-0.1.0.dist-info/LICENSE,sha256=4cCtcomD2KVzNeUs8QZPGv_R1FQXPYzr0-2LSnK0hwQ,35121
-ppmil-0.1.0.dist-info/METADATA,sha256=dgoQQFpE5a8W3OXXaVFinnxN0ZsEM5V8-bABHHaD_f8,1090
-ppmil-0.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ppmil-0.1.0.dist-info/top_level.txt,sha256=uBYwz0l_kHyFOn_pSSaMU1hca2kmrAu6lUFViqO9y0c,6
-ppmil-0.1.0.dist-info/RECORD,,
+ppmil/ppmil.py,sha256=IWCHo5UimHVxe9Kq5kfHAppKmK_oQr58728x-6Qmjw4,9397
+ppmil/quadrature.py,sha256=9dOjzQ-3wEG1IARopUXEVC-RBWRpc4mV01eRxZTMYQQ,3522
+ppmil-0.1.1.dist-info/LICENSE,sha256=4cCtcomD2KVzNeUs8QZPGv_R1FQXPYzr0-2LSnK0hwQ,35121
+ppmil-0.1.1.dist-info/METADATA,sha256=ggNDNONNc8ik1Qy_Jqou1hwqGkJQd_DfqTFSCBl1SQs,1274
+ppmil-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ppmil-0.1.1.dist-info/top_level.txt,sha256=uBYwz0l_kHyFOn_pSSaMU1hca2kmrAu6lUFViqO9y0c,6
+ppmil-0.1.1.dist-info/RECORD,,
```


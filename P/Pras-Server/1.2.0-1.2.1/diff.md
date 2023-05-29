# Comparing `tmp/Pras_Server-1.2.0.tar.gz` & `tmp/Pras_Server-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Pras_Server-1.2.0.tar", last modified: Mon May 29 06:02:25 2023, max compression
+gzip compressed data, was "Pras_Server-1.2.1.tar", last modified: Mon May 29 06:23:26 2023, max compression
```

## Comparing `Pras_Server-1.2.0.tar` & `Pras_Server-1.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:02:25.836248 Pras_Server-1.2.0/
--rwxrwxrwx   0 osita     (1000) osita     (1000)     1061 2022-02-07 06:19:51.000000 Pras_Server-1.2.0/LICENSE.txt
--rwxrwxrwx   0 osita     (1000) osita     (1000)      130 2022-05-31 15:51:04.000000 Pras_Server-1.2.0/MANIFEST.in
--rwxrwxrwx   0 osita     (1000) osita     (1000)     7693 2023-05-29 06:02:25.834250 Pras_Server-1.2.0/PKG-INFO
-drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:02:25.742308 Pras_Server-1.2.0/Pras_Server/
--rwxrwxrwx   0 osita     (1000) osita     (1000)    27558 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/CheckPDBatoms.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     2191 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/DownloadPDB.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    13028 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/FixHeavyAtoms.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    10251 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/ForcefieldParam.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    12820 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/LinearAlgebra.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    49426 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/MissingHeavyAtoms.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    50569 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/MissingHydrogenAtoms.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     5579 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/PDBID.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    24667 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/PRAS.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     7564 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/PotentialEnergy.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     7155 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/RamaChandra.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    10843 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/ReadMaster.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    18050 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/ReadStructure.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    11885 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/ReadmmCIF.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    10006 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/RunType.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)    12032 2023-05-29 06:01:25.000000 Pras_Server-1.2.0/Pras_Server/SecondaryStructure.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 05:21:54.000000 Pras_Server-1.2.0/Pras_Server/__init__.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)        6 2023-05-29 06:00:00.000000 Pras_Server-1.2.0/Pras_Server/_version.py
-drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:02:25.800271 Pras_Server-1.2.0/Pras_Server/data/
--rwxrwxrwx   0 osita     (1000) osita     (1000)    80000 2023-05-29 05:21:54.000000 Pras_Server-1.2.0/Pras_Server/data/KD.dat
-drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:02:25.829254 Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/
--rwxrwxrwx   0 osita     (1000) osita     (1000)   109350 2023-05-29 05:21:54.000000 Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/1aho.pdb
--rwxrwxrwx   0 osita     (1000) osita     (1000)   246721 2023-05-29 05:44:59.000000 Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/PRAS_with_FASPR.pdf
--rwxrwxrwx   0 osita     (1000) osita     (1000)      834 2023-05-29 05:21:54.000000 Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/linux_example.py
--rwxrwxrwx   0 osita     (1000) osita     (1000)     1177 2023-05-29 05:21:54.000000 Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/syntax.txt
-drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:02:25.795275 Pras_Server-1.2.0/Pras_Server.egg-info/
--rwxrwxrwx   0 osita     (1000) osita     (1000)     7693 2023-05-29 06:02:25.000000 Pras_Server-1.2.0/Pras_Server.egg-info/PKG-INFO
--rwxrwxrwx   0 osita     (1000) osita     (1000)      923 2023-05-29 06:02:25.000000 Pras_Server-1.2.0/Pras_Server.egg-info/SOURCES.txt
--rwxrwxrwx   0 osita     (1000) osita     (1000)        1 2023-05-29 06:02:25.000000 Pras_Server-1.2.0/Pras_Server.egg-info/dependency_links.txt
--rwxrwxrwx   0 osita     (1000) osita     (1000)       28 2023-05-29 06:02:25.000000 Pras_Server-1.2.0/Pras_Server.egg-info/requires.txt
--rwxrwxrwx   0 osita     (1000) osita     (1000)       12 2023-05-29 06:02:25.000000 Pras_Server-1.2.0/Pras_Server.egg-info/top_level.txt
--rwxrwxrwx   0 osita     (1000) osita     (1000)     7244 2023-05-29 05:50:15.000000 Pras_Server-1.2.0/README.md
--rwxrwxrwx   0 osita     (1000) osita     (1000)       38 2023-05-29 06:02:25.836248 Pras_Server-1.2.0/setup.cfg
--rwxrwxrwx   0 osita     (1000) osita     (1000)      883 2023-05-29 06:02:05.000000 Pras_Server-1.2.0/setup.py
+drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:23:26.895762 Pras_Server-1.2.1/
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     1061 2022-02-07 06:19:51.000000 Pras_Server-1.2.1/LICENSE.txt
+-rwxrwxrwx   0 osita     (1000) osita     (1000)      130 2022-05-31 15:51:04.000000 Pras_Server-1.2.1/MANIFEST.in
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     7693 2023-05-29 06:23:26.893764 Pras_Server-1.2.1/PKG-INFO
+drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:23:26.828804 Pras_Server-1.2.1/Pras_Server/
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    27558 2023-05-29 06:05:59.000000 Pras_Server-1.2.1/Pras_Server/CheckPDBatoms.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     2191 2023-05-29 06:06:18.000000 Pras_Server-1.2.1/Pras_Server/DownloadPDB.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    13028 2023-05-29 06:07:30.000000 Pras_Server-1.2.1/Pras_Server/FixHeavyAtoms.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    10251 2023-05-29 06:07:30.000000 Pras_Server-1.2.1/Pras_Server/ForcefieldParam.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    12820 2023-05-29 06:07:30.000000 Pras_Server-1.2.1/Pras_Server/LinearAlgebra.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    49426 2023-05-29 06:07:30.000000 Pras_Server-1.2.1/Pras_Server/MissingHeavyAtoms.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    50569 2023-05-29 06:07:30.000000 Pras_Server-1.2.1/Pras_Server/MissingHydrogenAtoms.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     5579 2023-05-29 06:07:30.000000 Pras_Server-1.2.1/Pras_Server/PDBID.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    24667 2023-05-29 06:07:30.000000 Pras_Server-1.2.1/Pras_Server/PRAS.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     7564 2023-05-29 06:07:30.000000 Pras_Server-1.2.1/Pras_Server/PotentialEnergy.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     7155 2023-05-29 06:05:36.000000 Pras_Server-1.2.1/Pras_Server/RamaChandra.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    10843 2023-05-29 06:05:36.000000 Pras_Server-1.2.1/Pras_Server/ReadMaster.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    18050 2023-05-29 06:05:36.000000 Pras_Server-1.2.1/Pras_Server/ReadStructure.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    11885 2023-05-29 06:04:40.000000 Pras_Server-1.2.1/Pras_Server/ReadmmCIF.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    10006 2023-05-29 06:05:36.000000 Pras_Server-1.2.1/Pras_Server/RunType.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    12032 2023-05-29 06:05:36.000000 Pras_Server-1.2.1/Pras_Server/SecondaryStructure.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 05:21:54.000000 Pras_Server-1.2.1/Pras_Server/__init__.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)        6 2023-05-29 06:05:36.000000 Pras_Server-1.2.1/Pras_Server/_version.py
+drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:23:26.859785 Pras_Server-1.2.1/Pras_Server/data/
+-rwxrwxrwx   0 osita     (1000) osita     (1000)    80000 2023-05-29 05:21:54.000000 Pras_Server-1.2.1/Pras_Server/data/KD.dat
+drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:23:26.888767 Pras_Server-1.2.1/Pras_Server/run_PRAS_with_FASPR/
+-rwxrwxrwx   0 osita     (1000) osita     (1000)   109350 2023-05-29 05:21:54.000000 Pras_Server-1.2.1/Pras_Server/run_PRAS_with_FASPR/1aho.pdb
+-rwxrwxrwx   0 osita     (1000) osita     (1000)   246016 2023-05-29 06:09:15.000000 Pras_Server-1.2.1/Pras_Server/run_PRAS_with_FASPR/PRAS_with_FASPR.pdf
+-rwxrwxrwx   0 osita     (1000) osita     (1000)      834 2023-05-29 05:21:54.000000 Pras_Server-1.2.1/Pras_Server/run_PRAS_with_FASPR/linux_example.py
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     1183 2023-05-29 06:21:05.000000 Pras_Server-1.2.1/Pras_Server/run_PRAS_with_FASPR/syntax.txt
+drwxrwxrwx   0 osita     (1000) osita     (1000)        0 2023-05-29 06:23:26.853789 Pras_Server-1.2.1/Pras_Server.egg-info/
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     7693 2023-05-29 06:23:26.000000 Pras_Server-1.2.1/Pras_Server.egg-info/PKG-INFO
+-rwxrwxrwx   0 osita     (1000) osita     (1000)      923 2023-05-29 06:23:26.000000 Pras_Server-1.2.1/Pras_Server.egg-info/SOURCES.txt
+-rwxrwxrwx   0 osita     (1000) osita     (1000)        1 2023-05-29 06:23:26.000000 Pras_Server-1.2.1/Pras_Server.egg-info/dependency_links.txt
+-rwxrwxrwx   0 osita     (1000) osita     (1000)       28 2023-05-29 06:23:26.000000 Pras_Server-1.2.1/Pras_Server.egg-info/requires.txt
+-rwxrwxrwx   0 osita     (1000) osita     (1000)       12 2023-05-29 06:23:26.000000 Pras_Server-1.2.1/Pras_Server.egg-info/top_level.txt
+-rwxrwxrwx   0 osita     (1000) osita     (1000)     7244 2023-05-29 06:03:58.000000 Pras_Server-1.2.1/README.md
+-rwxrwxrwx   0 osita     (1000) osita     (1000)       38 2023-05-29 06:23:26.895762 Pras_Server-1.2.1/setup.cfg
+-rwxrwxrwx   0 osita     (1000) osita     (1000)      883 2023-05-29 06:10:10.000000 Pras_Server-1.2.1/setup.py
```

### Comparing `Pras_Server-1.2.0/LICENSE.txt` & `Pras_Server-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Pras_Server-1.2.0/PKG-INFO` & `Pras_Server-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pras_Server
-Version: 1.2.0
+Version: 1.2.1
 Summary: A webserver to repair PDB files
 Home-page: https://www.protein-science.com/
 Author: Osita S. Nnyigide
 Author-email: osita@protein-science.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -37,15 +37,15 @@
 
 ## PRAS installation
 
 On November 20, 2022, a C++ version of the server that is independent of the python counterpart was released. The C++ version is named Pras_Server_C++ and is part of this repository. Both versions produce the same result but the former is 9 to 12 times faster than the latter. To use the C++ version, download this ZIP and extract the Pras_Server_C++ folder and follow the instruction in the INSTALL file included with the distribution.
 
 To use the python distribution on your local machine, use pip as given below or copy Pras_Server folder to any of the directories that Python searches at run-time
 
-`pip install Pras-Server==1.1.0`
+`pip install Pras-Server==1.2.1`
 
 ## PRAS usage
 
 A comprehensive test with 82 or 494 PDB or mmCIF structures may be performed to ensure the program works correctly.
 
 Since PRAS can download these structures automatically, 2 lists are provided which contain all the PDB IDs.
```

### Comparing `Pras_Server-1.2.0/Pras_Server/CheckPDBatoms.py` & `Pras_Server-1.2.1/Pras_Server/CheckPDBatoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
 
@@ -285,15 +285,15 @@
                 ' S.G. Lee, K. Hyun. Protein Repair and Analysis Server: A Web' +'\n'+
                 'Server to Repair PDB Structures, Add Missing Heavy'
                 ' Atoms and Hydrogen Atoms, and Assign Secondary Structures by'
                 ' Amide Interactions. J. Chem. Inf. Model., 2022, 62, 4232–4246.'+'\n')
 
         log.write('#'*183+'\n')
 
-        log.write('PRAS 1.2.0. This is a PRAS-generated log file.'
+        log.write('PRAS 1.2.1. This is a PRAS-generated log file.'
                 ' For your information, all missing or fixed atoms'
                 ' and other relevant information concerning the repair'
                 ' are appended below '+'\n')
 
         log.write('#'*183+'\n\n')
         log.write('This is the log for {}'.format(pdb_pras)+'\n\n')
```

### Comparing `Pras_Server-1.2.0/Pras_Server/DownloadPDB.py` & `Pras_Server-1.2.1/Pras_Server/DownloadPDB.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/FixHeavyAtoms.py` & `Pras_Server-1.2.1/Pras_Server/FixHeavyAtoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/ForcefieldParam.py` & `Pras_Server-1.2.1/Pras_Server/ForcefieldParam.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/LinearAlgebra.py` & `Pras_Server-1.2.1/Pras_Server/LinearAlgebra.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/MissingHeavyAtoms.py` & `Pras_Server-1.2.1/Pras_Server/MissingHeavyAtoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/MissingHydrogenAtoms.py` & `Pras_Server-1.2.1/Pras_Server/MissingHydrogenAtoms.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/PDBID.py` & `Pras_Server-1.2.1/Pras_Server/PDBID.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/PRAS.py` & `Pras_Server-1.2.1/Pras_Server/PRAS.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/PotentialEnergy.py` & `Pras_Server-1.2.1/Pras_Server/PotentialEnergy.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/RamaChandra.py` & `Pras_Server-1.2.1/Pras_Server/RamaChandra.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/ReadMaster.py` & `Pras_Server-1.2.1/Pras_Server/ReadMaster.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/ReadStructure.py` & `Pras_Server-1.2.1/Pras_Server/ReadStructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/ReadmmCIF.py` & `Pras_Server-1.2.1/Pras_Server/ReadmmCIF.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/RunType.py` & `Pras_Server-1.2.1/Pras_Server/RunType.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/SecondaryStructure.py` & `Pras_Server-1.2.1/Pras_Server/SecondaryStructure.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 __copyright__  = "Copyright 2022, Osita Sunday Nnyigide"
 
 __credits__    = ["Tochukwu Olunna Nnyigide", "Lee Sun-Gu", "Hyun Kyu"]
 
 __license__    = "MIT"
 
-__version__    = "1.2.0"
+__version__    = "1.2.1"
 
 __maintainer__ = "Osita Sunday Nnyigide"
 
 __email__      = "osita@protein-science.com"
 
 __status__     = "Production"
```

### Comparing `Pras_Server-1.2.0/Pras_Server/data/KD.dat` & `Pras_Server-1.2.1/Pras_Server/data/KD.dat`

 * *Files identical despite different names*

### Comparing `Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/1aho.pdb` & `Pras_Server-1.2.1/Pras_Server/run_PRAS_with_FASPR/1aho.pdb`

 * *Files identical despite different names*

### Comparing `Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/PRAS_with_FASPR.pdf` & `Pras_Server-1.2.1/Pras_Server/run_PRAS_with_FASPR/PRAS_with_FASPR.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 14% similar despite different names*

#### pdftotext {} -

```diff
@@ -17,15 +17,15 @@
 Then, execute the code below to compile FASPR (it takes ≈ 1 min. to compile):
 
 Now install PRAS server (if not installed) using the command below
 
 g++ -ffast-math -O3 -o FASPR src/*.cpp
 
 Install PRAS server which is added to path automatically with:
-pip install Pras-Server==1.1.0
+pip install Pras-Server==1.2.1
 
 Now download 1aho.pdb and copy to the current folder and run the code in
 syntax.txt that invokes linux_examply.py in the folder containing this
 document to repair several missing atoms using chi from FASPR PDB output.
 It is a good practice to type commands in Linux than copy and paste as
 Linux is extremely sensitive.
```

### Comparing `Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/linux_example.py` & `Pras_Server-1.2.1/Pras_Server/run_PRAS_with_FASPR/linux_example.py`

 * *Files identical despite different names*

### Comparing `Pras_Server-1.2.0/Pras_Server/run_PRAS_with_FASPR/syntax.txt` & `Pras_Server-1.2.1/Pras_Server/run_PRAS_with_FASPR/syntax.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Compile FASPR
 `g++ -ffast-math -O3 -o FASPR src/*.cpp`
 
 Install PRAS server
-`pip install Pras-Server==1.1.0`
+`pip install Pras-Server==1.2.1`
 
 Execute to run PRAS with FASPR output PDB
-`./FASPR –i 1aho.pdb -o output.pdb;python3 linux_example.py 1aho.pdb "" "" output.pdb "" ""`
+`./FASPR –i 1aho.pdb -o output.pdb;python3 linux_example.py 1aho.pdb "" "" output.pdb "" "" "" ""`
 
 You will see that both 	secondary structure assignemnt(ss) and ramachandran plot (rama) 
 are set to False and the reason is because you must install X server for Windows
 in order to run Linux GUI applications using Windows Subsystem for Linux (WSL).
 
 Thus, you need to:
```

### Comparing `Pras_Server-1.2.0/Pras_Server.egg-info/PKG-INFO` & `Pras_Server-1.2.1/Pras_Server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Pras-Server
-Version: 1.2.0
+Version: 1.2.1
 Summary: A webserver to repair PDB files
 Home-page: https://www.protein-science.com/
 Author: Osita S. Nnyigide
 Author-email: osita@protein-science.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -37,15 +37,15 @@
 
 ## PRAS installation
 
 On November 20, 2022, a C++ version of the server that is independent of the python counterpart was released. The C++ version is named Pras_Server_C++ and is part of this repository. Both versions produce the same result but the former is 9 to 12 times faster than the latter. To use the C++ version, download this ZIP and extract the Pras_Server_C++ folder and follow the instruction in the INSTALL file included with the distribution.
 
 To use the python distribution on your local machine, use pip as given below or copy Pras_Server folder to any of the directories that Python searches at run-time
 
-`pip install Pras-Server==1.1.0`
+`pip install Pras-Server==1.2.1`
 
 ## PRAS usage
 
 A comprehensive test with 82 or 494 PDB or mmCIF structures may be performed to ensure the program works correctly.
 
 Since PRAS can download these structures automatically, 2 lists are provided which contain all the PDB IDs.
```

### Comparing `Pras_Server-1.2.0/Pras_Server.egg-info/SOURCES.txt` & `Pras_Server-1.2.1/Pras_Server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Pras_Server-1.2.0/README.md` & `Pras_Server-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 ## PRAS installation
 
 On November 20, 2022, a C++ version of the server that is independent of the python counterpart was released. The C++ version is named Pras_Server_C++ and is part of this repository. Both versions produce the same result but the former is 9 to 12 times faster than the latter. To use the C++ version, download this ZIP and extract the Pras_Server_C++ folder and follow the instruction in the INSTALL file included with the distribution.
 
 To use the python distribution on your local machine, use pip as given below or copy Pras_Server folder to any of the directories that Python searches at run-time
 
-`pip install Pras-Server==1.1.0`
+`pip install Pras-Server==1.2.1`
 
 ## PRAS usage
 
 A comprehensive test with 82 or 494 PDB or mmCIF structures may be performed to ensure the program works correctly.
 
 Since PRAS can download these structures automatically, 2 lists are provided which contain all the PDB IDs.
```

### Comparing `Pras_Server-1.2.0/setup.py` & `Pras_Server-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 current_dir = pathlib.Path(__file__).parent.resolve()
 
 long_description = (current_dir / 'README.md').read_text(encoding='utf-8')
 
 setup(
 
     name = 'Pras_Server',
-    version = '1.2.0',
+    version = '1.2.1',
     description='A webserver to repair PDB files',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://www.protein-science.com/',
     author='Osita S. Nnyigide',
     author_email='osita@protein-science.com',
     classifiers=[
```


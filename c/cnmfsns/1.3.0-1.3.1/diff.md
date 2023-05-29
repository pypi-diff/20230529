# Comparing `tmp/cnmfsns-1.3.0.tar.gz` & `tmp/cnmfsns-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnmfsns-1.3.0.tar", last modified: Tue May 16 19:48:33 2023, max compression
+gzip compressed data, was "cnmfsns-1.3.1.tar", last modified: Mon May 29 17:15:48 2023, max compression
```

## Comparing `cnmfsns-1.3.0.tar` & `cnmfsns-1.3.1.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 19:48:33.290934 cnmfsns-1.3.0/
--rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     3987 2023-05-16 19:48:33.290934 cnmfsns-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     3472 2023-05-16 19:28:48.000000 cnmfsns-1.3.0/README.md
--rw-rw-rw-   0        0        0     4037 2023-05-12 19:39:10.000000 cnmfsns-1.3.0/README.rst
--rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      964 2023-05-16 19:48:33.306556 cnmfsns-1.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-16 19:48:33.244044 cnmfsns-1.3.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-16 19:48:33.275316 cnmfsns-1.3.0/src/cnmfsns/
--rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.3.0/src/cnmfsns/__init__.py
--rw-rw-rw-   0        0        0    56223 2023-05-16 19:30:43.000000 cnmfsns-1.3.0/src/cnmfsns/cli.py
--rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.3.0/src/cnmfsns/cnmf.py
--rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.3.0/src/cnmfsns/colors.py
--rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.3.0/src/cnmfsns/config.py
--rw-rw-rw-   0        0        0    35116 2023-05-16 18:43:11.000000 cnmfsns-1.3.0/src/cnmfsns/dataset.py
--rw-rw-rw-   0        0        0    21163 2023-05-15 22:09:27.000000 cnmfsns-1.3.0/src/cnmfsns/integration.py
--rw-rw-rw-   0        0        0    57617 2023-05-16 18:55:37.000000 cnmfsns-1.3.0/src/cnmfsns/plots.py
--rw-rw-rw-   0        0        0    35301 2023-05-16 19:23:15.000000 cnmfsns-1.3.0/src/cnmfsns/sns.py
--rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.3.0/src/cnmfsns/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-16 19:48:33.290934 cnmfsns-1.3.0/src/cnmfsns.egg-info/
--rw-rw-rw-   0        0        0     3987 2023-05-16 19:48:33.000000 cnmfsns-1.3.0/src/cnmfsns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      483 2023-05-16 19:48:33.000000 cnmfsns-1.3.0/src/cnmfsns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 19:48:33.000000 cnmfsns-1.3.0/src/cnmfsns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-05-16 19:48:33.000000 cnmfsns-1.3.0/src/cnmfsns.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      177 2023-05-16 19:48:33.000000 cnmfsns-1.3.0/src/cnmfsns.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-16 19:48:33.000000 cnmfsns-1.3.0/src/cnmfsns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 17:15:48.313333 cnmfsns-1.3.1/
+-rw-rw-rw-   0        0        0     1090 2023-04-24 20:31:27.000000 cnmfsns-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     3982 2023-05-29 17:15:48.313333 cnmfsns-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3467 2023-05-29 17:14:53.000000 cnmfsns-1.3.1/README.md
+-rw-rw-rw-   0        0        0       86 2023-04-24 20:31:27.000000 cnmfsns-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      964 2023-05-29 17:15:48.313333 cnmfsns-1.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 17:15:48.266443 cnmfsns-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 17:15:48.282086 cnmfsns-1.3.1/src/cnmfsns/
+-rw-rw-rw-   0        0        0      513 2023-05-12 18:06:16.000000 cnmfsns-1.3.1/src/cnmfsns/__init__.py
+-rw-rw-rw-   0        0        0    56223 2023-05-16 20:25:56.000000 cnmfsns-1.3.1/src/cnmfsns/cli.py
+-rw-rw-rw-   0        0        0    39682 2023-05-12 20:51:27.000000 cnmfsns-1.3.1/src/cnmfsns/cnmf.py
+-rw-rw-rw-   0        0        0    16061 2023-04-24 20:31:27.000000 cnmfsns-1.3.1/src/cnmfsns/colors.py
+-rw-rw-rw-   0        0        0     3257 2023-04-24 20:31:27.000000 cnmfsns-1.3.1/src/cnmfsns/config.py
+-rw-rw-rw-   0        0        0    35130 2023-05-29 17:09:43.000000 cnmfsns-1.3.1/src/cnmfsns/dataset.py
+-rw-rw-rw-   0        0        0    21163 2023-05-15 22:09:27.000000 cnmfsns-1.3.1/src/cnmfsns/integration.py
+-rw-rw-rw-   0        0        0    57617 2023-05-16 18:55:37.000000 cnmfsns-1.3.1/src/cnmfsns/plots.py
+-rw-rw-rw-   0        0        0    35301 2023-05-16 19:23:15.000000 cnmfsns-1.3.1/src/cnmfsns/sns.py
+-rw-rw-rw-   0        0        0     2767 2023-04-24 20:31:27.000000 cnmfsns-1.3.1/src/cnmfsns/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 17:15:48.313333 cnmfsns-1.3.1/src/cnmfsns.egg-info/
+-rw-rw-rw-   0        0        0     3982 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      472 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      177 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-29 17:15:48.000000 cnmfsns-1.3.1/src/cnmfsns.egg-info/top_level.txt
```

### Comparing `cnmfsns-1.3.0/LICENSE` & `cnmfsns-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.0/PKG-INFO` & `cnmfsns-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.3.0
+Version: 1.3.1
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,17 +16,17 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.3.0-blue)
+![version badge](https://img.shields.io/badge/version-1.3.1-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
-[![Conda Latest Release](https://anaconda.org/conda-forge/cnmfsns/badges/version.svg)](https://anaconda.org/anaconda/cnmfsns/)
+[![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
 
 **cNMF-SNS** (consensus Non-negative Matrix Factorization Solution Network Space) is a Python package enabling mosaic integration of bulk, single-cell, and
```

### Comparing `cnmfsns-1.3.0/README.md` & `cnmfsns-1.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -5,213 +5,213 @@
 00000040: 2070 6f77 6572 6675 6c20 6661 6374 6f72   powerful factor
 00000050: 697a 6174 696f 6e2d 6261 7365 6420 6d75  ization-based mu
 00000060: 6c74 692d 6f6d 6963 7320 696e 7465 6772  lti-omics integr
 00000070: 6174 696f 6e20 746f 6f6c 6b69 740d 0a0d  ation toolkit...
 00000080: 0a21 5b76 6572 7369 6f6e 2062 6164 6765  .![version badge
 00000090: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
 000000a0: 6965 6c64 732e 696f 2f62 6164 6765 2f76  ields.io/badge/v
-000000b0: 6572 7369 6f6e 2d31 2e33 2e30 2d62 6c75  ersion-1.3.0-blu
+000000b0: 6572 7369 6f6e 2d31 2e33 2e31 2d62 6c75  ersion-1.3.1-blu
 000000c0: 6529 0d0a 5b21 5b50 7950 4920 4c61 7465  e)..[![PyPI Late
 000000d0: 7374 2052 656c 6561 7365 5d28 6874 7470  st Release](http
 000000e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
 000000f0: 696f 2f70 7970 692f 762f 636e 6d66 736e  io/pypi/v/cnmfsn
 00000100: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
 00000110: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
 00000120: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b43  /cnmfsns/)..[![C
 00000130: 6f6e 6461 204c 6174 6573 7420 5265 6c65  onda Latest Rele
-00000140: 6173 655d 2868 7474 7073 3a2f 2f61 6e61  ase](https://ana
-00000150: 636f 6e64 612e 6f72 672f 636f 6e64 612d  conda.org/conda-
-00000160: 666f 7267 652f 636e 6d66 736e 732f 6261  forge/cnmfsns/ba
-00000170: 6467 6573 2f76 6572 7369 6f6e 2e73 7667  dges/version.svg
-00000180: 295d 2868 7474 7073 3a2f 2f61 6e61 636f  )](https://anaco
-00000190: 6e64 612e 6f72 672f 616e 6163 6f6e 6461  nda.org/anaconda
-000001a0: 2f63 6e6d 6673 6e73 2f29 0d0a 5b21 5b44  /cnmfsns/)..[![D
-000001b0: 6f63 756d 656e 7461 7469 6f6e 2073 7461  ocumentation sta
-000001c0: 7475 735d 2868 7474 7073 3a2f 2f72 6561  tus](https://rea
-000001d0: 6474 6865 646f 6373 2e6f 7267 2f70 726f  dthedocs.org/pro
-000001e0: 6a65 6374 732f 636e 6d66 2d73 6e73 2f62  jects/cnmf-sns/b
-000001f0: 6164 6765 2f3f 7665 7273 696f 6e3d 6c61  adge/?version=la
-00000200: 7465 7374 2673 7479 6c65 3d66 6c61 7429  test&style=flat)
-00000210: 5d28 290d 0a5b 215b 446f 776e 6c6f 6164  ]()..[![Download
-00000220: 735d 2868 7474 7073 3a2f 2f73 7461 7469  s](https://stati
-00000230: 632e 7065 7079 2e74 6563 682f 6261 6467  c.pepy.tech/badg
-00000240: 652f 636e 6d66 736e 7329 5d28 6874 7470  e/cnmfsns)](http
-00000250: 733a 2f2f 7065 7079 2e74 6563 682f 7072  s://pepy.tech/pr
-00000260: 6f6a 6563 742f 636e 6d66 736e 7329 0d0a  oject/cnmfsns)..
-00000270: 5b21 5b4c 6963 656e 7365 5d28 6874 7470  [![License](http
-00000280: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
-00000290: 696f 2f70 7970 692f 6c2f 636e 6d66 736e  io/pypi/l/cnmfsn
-000002a0: 732e 7376 6729 5d28 6874 7470 733a 2f2f  s.svg)](https://
-000002b0: 6769 7468 7562 2e63 6f6d 2f4d 6f72 7269  github.com/Morri
-000002c0: 7373 794c 6162 2f63 4e4d 462d 534e 532f  ssyLab/cNMF-SNS/
-000002d0: 626c 6f62 2f6d 6169 6e2f 4c49 4345 4e53  blob/main/LICENS
-000002e0: 4529 0d0a 0d0a 4175 7468 6f72 733a 205b  E)....Authors: [
-000002f0: 5465 6420 5665 7268 6579 5d28 6874 7470  Ted Verhey](http
-00000300: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f76  s://github.com/v
-00000310: 6572 6865 7974 6229 2c20 5b48 6565 776f  erheytb), [Heewo
-00000320: 6e20 5365 6f5d 2868 7474 7073 3a2f 2f67  n Seo](https://g
-00000330: 6974 6875 622e 636f 6d2f 6c6f 6f74 7069  ithub.com/lootpi
-00000340: 7a29 2c20 5b53 6f72 616e 6120 4d6f 7272  z), [Sorana Morr
-00000350: 6973 7379 5d28 6874 7470 733a 2f2f 6769  issy](https://gi
-00000360: 7468 7562 2e63 6f6d 2f61 6e63 6173 6f72  thub.com/ancasor
-00000370: 616e 6129 0d0a 0d0a 2a2a 634e 4d46 2d53  ana)....**cNMF-S
-00000380: 4e53 2a2a 2028 636f 6e73 656e 7375 7320  NS** (consensus 
-00000390: 4e6f 6e2d 6e65 6761 7469 7665 204d 6174  Non-negative Mat
-000003a0: 7269 7820 4661 6374 6f72 697a 6174 696f  rix Factorizatio
-000003b0: 6e20 536f 6c75 7469 6f6e 204e 6574 776f  n Solution Netwo
-000003c0: 726b 2053 7061 6365 2920 6973 2061 2050  rk Space) is a P
-000003d0: 7974 686f 6e20 7061 636b 6167 6520 656e  ython package en
-000003e0: 6162 6c69 6e67 206d 6f73 6169 6320 696e  abling mosaic in
-000003f0: 7465 6772 6174 696f 6e20 6f66 2062 756c  tegration of bul
-00000400: 6b2c 2073 696e 676c 652d 6365 6c6c 2c20  k, single-cell, 
-00000410: 616e 640d 0a73 7061 7469 616c 2065 7870  and..spatial exp
-00000420: 7265 7373 696f 6e20 6461 7461 2062 6574  ression data bet
-00000430: 7765 656e 2061 6e64 2077 6974 6869 6e20  ween and within 
-00000440: 6461 7461 7365 7473 2e20 4461 7461 7365  datasets. Datase
-00000450: 7473 2063 616e 2068 6176 6520 7061 7274  ts can have part
-00000460: 6961 6c6c 7920 6f76 6572 6c61 7070 696e  ially overlappin
-00000470: 6720 6665 6174 7572 6573 2028 6567 2e20  g features (eg. 
-00000480: 6765 6e65 7329 2061 7320 7765 6c6c 2061  genes) as well a
-00000490: 7320 6e6f 6e2d 6f76 6572 6c61 7070 696e  s non-overlappin
-000004a0: 6720 6665 6174 7572 6573 2e20 634e 4d46  g features. cNMF
-000004b0: 2070 726f 7669 6465 7320 6120 2a2a 726f   provides a **ro
-000004c0: 6275 7374 2c20 0d0a 756e 7375 7065 7276  bust, ..unsuperv
-000004d0: 6973 6564 2a2a 2064 6563 6f6e 766f 6c75  ised** deconvolu
-000004e0: 7469 6f6e 206f 6620 6561 6368 2064 6174  tion of each dat
-000004f0: 6173 6574 2069 6e74 6f20 6765 6e65 2065  aset into gene e
-00000500: 7870 7265 7373 696f 6e20 7072 6f67 7261  xpression progra
-00000510: 6d73 2028 4745 5073 292e 0d0a 2a2a 4e65  ms (GEPs)...**Ne
-00000520: 7477 6f72 6b2d 6261 7365 6420 696e 7465  twork-based inte
-00000530: 6772 6174 696f 6e2a 2a20 6f66 2047 4550  gration** of GEP
-00000540: 7320 656e 6162 6c65 7320 666c 6578 6962  s enables flexib
-00000550: 6c65 2069 6e74 6567 7261 7469 6f6e 206f  le integration o
-00000560: 6620 6d61 6e79 2064 6174 6173 6574 730d  f many datasets.
-00000570: 0a61 6372 6f73 7320 6173 7361 7973 2028  .across assays (
-00000580: 6567 2e20 5072 6f74 6569 6e2c 2052 4e41  eg. Protein, RNA
-00000590: 2d53 6571 2c20 7363 524e 412d 5365 712c  -Seq, scRNA-Seq,
-000005a0: 2073 7061 7469 616c 2065 7870 7265 7373   spatial express
-000005b0: 696f 6e29 2061 6e64 2070 6174 6965 6e74  ion) and patient
-000005c0: 2063 6f68 6f72 7473 2e0d 0a0d 0a43 6f6d   cohorts.....Com
-000005d0: 6d75 6e69 7469 6573 2077 6974 6820 4745  munities with GE
-000005e0: 5073 2066 726f 6d20 6d75 6c74 6970 6c65  Ps from multiple
-000005f0: 2064 6174 6173 6574 7320 6361 6e20 6265   datasets can be
-00000600: 2061 6e6e 6f74 6174 6564 2077 6974 6820   annotated with 
-00000610: 6461 7461 7365 742d 7370 6563 6966 6963  dataset-specific
-00000620: 0d0a 616e 6e6f 7461 7469 6f6e 7320 746f  ..annotations to
-00000630: 2066 6163 696c 6974 6174 6520 696e 7465   facilitate inte
-00000640: 7270 7265 7461 7469 6f6e 2e0d 0a0d 0a23  rpretation.....#
-00000650: 2320 e29a a14d 6169 6e20 4665 6174 7572  # ...Main Featur
-00000660: 6573 0d0a 0d0a 4865 7265 2061 7265 206a  es....Here are j
-00000670: 7573 7420 6120 6665 7720 6f66 2074 6865  ust a few of the
-00000680: 2074 6869 6e67 7320 7468 6174 2063 4e4d   things that cNM
-00000690: 462d 534e 5320 646f 6573 2077 656c 6c3a  F-SNS does well:
-000006a0: 0d0a 0d0a 2d20 4964 656e 7469 6669 6573  ....- Identifies
-000006b0: 2069 6e74 6572 7072 6574 6162 6c65 2c20   interpretable, 
-000006c0: 6164 6469 7469 7665 206e 6f6e 2d6e 6567  additive non-neg
-000006d0: 6174 6976 6520 6765 6e65 2065 7870 7265  ative gene expre
-000006e0: 7373 696f 6e20 7072 6f67 7261 6d73 0d0a  ssion programs..
-000006f0: 2d20 4d6f 7361 6963 2069 6e74 6567 7261  - Mosaic integra
-00000700: 7469 6f6e 2064 6f65 7320 6e6f 7420 7265  tion does not re
-00000710: 7175 6972 6520 7375 6273 6574 7469 6e67  quire subsetting
-00000720: 2066 6561 7475 7265 732f 6765 6e65 7320   features/genes 
-00000730: 746f 0d0a 2020 6120 7368 6172 6564 206f  to..  a shared o
-00000740: 7220 6f76 6572 6469 7370 6572 7365 6420  r overdispersed 
-00000750: 7375 6273 6574 0d0a 2d20 4964 6561 6c20  subset..- Ideal 
-00000760: 666f 7220 696e 6372 656d 656e 7461 6c20  for incremental 
-00000770: 696e 7465 6772 6174 696f 6e20 2861 6464  integration (add
-00000780: 696e 6720 6461 7461 7365 7473 206f 6e65  ing datasets one
-00000790: 2061 7420 6120 7469 6d65 2920 7369 6e63   at a time) sinc
-000007a0: 650d 0a20 2064 6563 6f6e 766f 6c75 7469  e..  deconvoluti
-000007b0: 6f6e 2069 7320 7065 7266 6f72 6d65 6420  on is performed 
-000007c0: 696e 6465 7065 6e64 656e 746c 7920 6f6e  independently on
-000007d0: 2065 6163 6820 6461 7461 7365 7420 6765   each dataset ge
-000007e0: 6e65 7261 7469 6e67 2069 6e76 6172 6961  nerating invaria
-000007f0: 6e74 2047 4550 730d 0a2d 2049 6e74 6567  nt GEPs..- Integ
-00000800: 7261 7469 6f6e 2064 6f65 7320 6e6f 7420  ration does not 
-00000810: 7265 7175 6972 6520 636f 6d70 6172 6162  require comparab
-00000820: 6c65 2064 6174 6120 7370 6172 7369 7479  le data sparsity
-00000830: 206f 7220 7365 7175 656e 6369 6e67 2064   or sequencing d
-00000840: 6570 7468 2028 7369 6e67 6c65 2d63 656c  epth (single-cel
-00000850: 6c2c 206d 6963 726f 6172 7261 792c 2062  l, microarray, b
-00000860: 756c 6b29 0d0a 2d20 5477 6f20 696e 7465  ulk)..- Two inte
-00000870: 7266 6163 6573 3a20 636f 6d6d 616e 642d  rfaces: command-
-00000880: 6c69 6e65 2069 6e74 6572 6661 6365 2066  line interface f
-00000890: 6f72 2072 6170 6964 2064 6174 6120 6578  or rapid data ex
-000008a0: 706c 6f72 6174 696f 6e20 616e 6420 7079  ploration and py
-000008b0: 7468 6f6e 0d0a 2020 696e 7465 7266 6163  thon..  interfac
-000008c0: 6520 666f 7220 6578 7465 6e73 6962 696c  e for extensibil
-000008d0: 6974 7920 616e 6420 666c 6578 6962 696c  ity and flexibil
-000008e0: 6974 790d 0a0d 0a23 2320 f09f 94a7 2049  ity....## .... I
-000008f0: 6e73 7461 6c6c 0d0a 0d0a 2323 2320 e298  nstall....### ..
-00000900: 81ef b88f 2050 7562 6c69 6320 5265 6c65  .... Public Rele
-00000910: 6173 650d 0a0d 0a49 6e73 7461 6c6c 2074  ase....Install t
-00000920: 6865 2070 6163 6b61 6765 2077 6974 6820  he package with 
-00000930: 636f 6e64 613a 0d0a 6060 6062 6173 680d  conda:..```bash.
-00000940: 0a63 6f6e 6461 2069 6e73 7461 6c6c 202d  .conda install -
-00000950: 6320 636f 6e64 612d 666f 7267 6520 636e  c conda-forge cn
-00000960: 6d66 736e 730d 0a60 6060 0d0a 0d0a 2323  mfsns..```....##
-00000970: 2320 e29c a820 4c61 7465 7374 2076 6572  # ... Latest ver
-00000980: 7369 6f6e 2066 726f 6d20 4769 7448 7562  sion from GitHub
-00000990: 0d0a 0d0a 4265 666f 7265 2069 6e73 7461  ....Before insta
-000009a0: 6c6c 696e 6720 634e 4d46 2d53 4e53 2075  lling cNMF-SNS u
-000009b0: 7369 6e67 2070 6970 2c20 6974 2069 7320  sing pip, it is 
-000009c0: 7265 636f 6d6d 656e 6465 6420 746f 2066  recommended to f
-000009d0: 6972 7374 2073 6574 2075 7020 6120 7365  irst set up a se
-000009e0: 7061 7261 7465 2063 6f6e 6461 2065 6e76  parate conda env
-000009f0: 6972 6f6e 6d65 6e74 2061 6e64 2068 6176  ironment and hav
-00000a00: 6520 636f 6e64 6120 6d61 6e61 6765 2061  e conda manage a
-00000a10: 7320 6d61 6e79 2064 6570 656e 6465 6e63  s many dependenc
-00000a20: 6965 7320 6173 2070 6f73 7369 626c 652e  ies as possible.
-00000a30: 0d0a 0d0a 6060 6062 6173 680d 0a63 6f6e  ....```bash..con
-00000a40: 6461 2063 7265 6174 6520 2d2d 6e61 6d65  da create --name
-00000a50: 2063 6e6d 6673 6e73 202d 6320 636f 6e64   cnmfsns -c cond
-00000a60: 612d 666f 7267 6520 7079 7468 6f6e 3d33  a-forge python=3
-00000a70: 2e31 3020 616e 6e64 6174 6120 7061 6e64  .10 anndata pand
-00000a80: 6173 206e 756d 7079 2073 6369 7079 206d  as numpy scipy m
-00000a90: 6174 706c 6f74 6c69 6220 7570 7365 7470  atplotlib upsetp
-00000aa0: 6c6f 7420 6874 7470 6c69 6232 2074 6f6d  lot httplib2 tom
-00000ab0: 6c69 2074 6f6d 6c69 2d77 2063 6c69 636b  li tomli-w click
-00000ac0: 2070 7967 7261 7068 7669 7a20 7079 7468   pygraphviz pyth
-00000ad0: 6f6e 2d69 6772 6170 6820 7365 6d61 6e74  on-igraph semant
-00000ae0: 6963 5f76 6572 7369 6f6e 2070 7979 616d  ic_version pyyam
-00000af0: 6c20 7363 696b 6974 2d6c 6561 726e 2066  l scikit-learn f
-00000b00: 6173 7463 6c75 7374 6572 2073 6361 6e70  astcluster scanp
-00000b10: 7920 7079 7961 6d6c 0d0a 636f 6e64 6120  y pyyaml..conda 
-00000b20: 6163 7469 7661 7465 2063 6e6d 6673 6e73  activate cnmfsns
-00000b30: 0d0a 7069 7020 696e 7374 616c 6c20 6769  ..pip install gi
-00000b40: 742b 6874 7470 733a 2f2f 6769 7468 7562  t+https://github
-00000b50: 2e63 6f6d 2f4d 6f72 7269 7373 794c 6162  .com/MorrissyLab
-00000b60: 2f63 4e4d 462d 534e 532e 6769 740d 0a60  /cNMF-SNS.git..`
-00000b70: 6060 0d0a 0d0a 2323 20f0 9f93 9620 446f  ``....## .... Do
-00000b80: 6375 6d65 6e74 6174 696f 6e0d 0a0d 0a23  cumentation....#
-00000b90: 2323 20f0 9f93 9320 5079 7468 6f6e 2069  ## .... Python i
-00000ba0: 6e74 6572 6661 6365 0d0a 0d0a 546f 2067  nterface....To g
-00000bb0: 6574 2073 7461 7274 6564 2c20 7361 6d70  et started, samp
-00000bc0: 6c65 2070 726f 7465 6f6d 6963 7320 6461  le proteomics da
-00000bd0: 7461 7365 7473 2061 6e64 2061 204a 7570  tasets and a Jup
-00000be0: 7974 6572 206e 6f74 6562 6f6f 6b20 7475  yter notebook tu
-00000bf0: 746f 7269 616c 2069 7320 6176 6169 6c61  torial is availa
-00000c00: 626c 6520 5b68 6572 655d 282f 7475 746f  ble [here](/tuto
-00000c10: 7269 616c 2f74 7574 6f72 6961 6c2e 6970  rial/tutorial.ip
-00000c20: 796e 6229 2e0d 0a0d 0a44 6574 6169 6c65  ynb).....Detaile
-00000c30: 6420 4150 4920 7265 6665 7265 6e63 6520  d API reference 
-00000c40: 6361 6e20 6265 2066 6f75 6e64 206f 6e20  can be found on 
-00000c50: 5b52 6561 6454 6865 446f 6373 5d28 6874  [ReadTheDocs](ht
-00000c60: 7470 733a 2f2f 636e 6d66 2d73 6e73 2e72  tps://cnmf-sns.r
-00000c70: 6561 6474 6865 646f 6373 2e69 6f2f 292e  eadthedocs.io/).
-00000c80: 0d0a 0d0a 0d0a 2323 2320 e28c a8ef b88f  ......### ......
-00000c90: 2043 6f6d 6d61 6e64 206c 696e 6520 696e   Command line in
-00000ca0: 7465 7266 6163 650d 0a0d 0a53 6565 2074  terface....See t
-00000cb0: 6865 205b 636f 6d6d 616e 6420 6c69 6e65  he [command line
-00000cc0: 2069 6e74 6572 6661 6365 2064 6f63 756d   interface docum
-00000cd0: 656e 7461 7469 6f6e 5d28 2f43 4c49 2e6d  entation](/CLI.m
-00000ce0: 6429 2e0d 0a0d 0a23 2320 f09f 92ad 2047  d).....## .... G
-00000cf0: 6574 7469 6e67 2048 656c 700d 0a0d 0a46  etting Help....F
-00000d00: 6f72 2065 7272 6f72 7320 6172 6973 696e  or errors arisin
-00000d10: 6720 6475 7269 6e67 2075 7365 206f 6620  g during use of 
-00000d20: 634e 4d46 2d53 4e53 2c20 6372 6561 7465  cNMF-SNS, create
-00000d30: 2061 6e64 2062 726f 7773 6520 6973 7375   and browse issu
-00000d40: 6573 2069 6e20 7468 6520 5b47 6974 4875  es in the [GitHu
-00000d50: 6220 2269 7373 7565 7322 2074 6162 5d28  b "issues" tab](
-00000d60: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-00000d70: 6f6d 2f4d 6f72 7269 7373 794c 6162 2f63  om/MorrissyLab/c
-00000d80: 4e4d 462d 534e 532f 6973 7375 6573 292e  NMF-SNS/issues).
+00000140: 6173 655d 2868 7474 7073 3a2f 2f69 6d67  ase](https://img
+00000150: 2e73 6869 656c 6473 2e69 6f2f 636f 6e64  .shields.io/cond
+00000160: 612f 766e 2f63 6f6e 6461 2d66 6f72 6765  a/vn/conda-forge
+00000170: 2f63 6e6d 6673 6e73 295d 2868 7474 7073  /cnmfsns)](https
+00000180: 3a2f 2f61 6e61 636f 6e64 612e 6f72 672f  ://anaconda.org/
+00000190: 636f 6e64 612d 666f 7267 652f 636e 6d66  conda-forge/cnmf
+000001a0: 736e 732f 290d 0a5b 215b 446f 6375 6d65  sns/)..[![Docume
+000001b0: 6e74 6174 696f 6e20 7374 6174 7573 5d28  ntation status](
+000001c0: 6874 7470 733a 2f2f 7265 6164 7468 6564  https://readthed
+000001d0: 6f63 732e 6f72 672f 7072 6f6a 6563 7473  ocs.org/projects
+000001e0: 2f63 6e6d 662d 736e 732f 6261 6467 652f  /cnmf-sns/badge/
+000001f0: 3f76 6572 7369 6f6e 3d6c 6174 6573 7426  ?version=latest&
+00000200: 7374 796c 653d 666c 6174 295d 2829 0d0a  style=flat)]()..
+00000210: 5b21 5b44 6f77 6e6c 6f61 6473 5d28 6874  [![Downloads](ht
+00000220: 7470 733a 2f2f 7374 6174 6963 2e70 6570  tps://static.pep
+00000230: 792e 7465 6368 2f62 6164 6765 2f63 6e6d  y.tech/badge/cnm
+00000240: 6673 6e73 295d 2868 7474 7073 3a2f 2f70  fsns)](https://p
+00000250: 6570 792e 7465 6368 2f70 726f 6a65 6374  epy.tech/project
+00000260: 2f63 6e6d 6673 6e73 290d 0a5b 215b 4c69  /cnmfsns)..[![Li
+00000270: 6365 6e73 655d 2868 7474 7073 3a2f 2f69  cense](https://i
+00000280: 6d67 2e73 6869 656c 6473 2e69 6f2f 7079  mg.shields.io/py
+00000290: 7069 2f6c 2f63 6e6d 6673 6e73 2e73 7667  pi/l/cnmfsns.svg
+000002a0: 295d 2868 7474 7073 3a2f 2f67 6974 6875  )](https://githu
+000002b0: 622e 636f 6d2f 4d6f 7272 6973 7379 4c61  b.com/MorrissyLa
+000002c0: 622f 634e 4d46 2d53 4e53 2f62 6c6f 622f  b/cNMF-SNS/blob/
+000002d0: 6d61 696e 2f4c 4943 454e 5345 290d 0a0d  main/LICENSE)...
+000002e0: 0a41 7574 686f 7273 3a20 5b54 6564 2056  .Authors: [Ted V
+000002f0: 6572 6865 795d 2868 7474 7073 3a2f 2f67  erhey](https://g
+00000300: 6974 6875 622e 636f 6d2f 7665 7268 6579  ithub.com/verhey
+00000310: 7462 292c 205b 4865 6577 6f6e 2053 656f  tb), [Heewon Seo
+00000320: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00000330: 2e63 6f6d 2f6c 6f6f 7470 697a 292c 205b  .com/lootpiz), [
+00000340: 536f 7261 6e61 204d 6f72 7269 7373 795d  Sorana Morrissy]
+00000350: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000360: 636f 6d2f 616e 6361 736f 7261 6e61 290d  com/ancasorana).
+00000370: 0a0d 0a2a 2a63 4e4d 462d 534e 532a 2a20  ...**cNMF-SNS** 
+00000380: 2863 6f6e 7365 6e73 7573 204e 6f6e 2d6e  (consensus Non-n
+00000390: 6567 6174 6976 6520 4d61 7472 6978 2046  egative Matrix F
+000003a0: 6163 746f 7269 7a61 7469 6f6e 2053 6f6c  actorization Sol
+000003b0: 7574 696f 6e20 4e65 7477 6f72 6b20 5370  ution Network Sp
+000003c0: 6163 6529 2069 7320 6120 5079 7468 6f6e  ace) is a Python
+000003d0: 2070 6163 6b61 6765 2065 6e61 626c 696e   package enablin
+000003e0: 6720 6d6f 7361 6963 2069 6e74 6567 7261  g mosaic integra
+000003f0: 7469 6f6e 206f 6620 6275 6c6b 2c20 7369  tion of bulk, si
+00000400: 6e67 6c65 2d63 656c 6c2c 2061 6e64 0d0a  ngle-cell, and..
+00000410: 7370 6174 6961 6c20 6578 7072 6573 7369  spatial expressi
+00000420: 6f6e 2064 6174 6120 6265 7477 6565 6e20  on data between 
+00000430: 616e 6420 7769 7468 696e 2064 6174 6173  and within datas
+00000440: 6574 732e 2044 6174 6173 6574 7320 6361  ets. Datasets ca
+00000450: 6e20 6861 7665 2070 6172 7469 616c 6c79  n have partially
+00000460: 206f 7665 726c 6170 7069 6e67 2066 6561   overlapping fea
+00000470: 7475 7265 7320 2865 672e 2067 656e 6573  tures (eg. genes
+00000480: 2920 6173 2077 656c 6c20 6173 206e 6f6e  ) as well as non
+00000490: 2d6f 7665 726c 6170 7069 6e67 2066 6561  -overlapping fea
+000004a0: 7475 7265 732e 2063 4e4d 4620 7072 6f76  tures. cNMF prov
+000004b0: 6964 6573 2061 202a 2a72 6f62 7573 742c  ides a **robust,
+000004c0: 200d 0a75 6e73 7570 6572 7669 7365 642a   ..unsupervised*
+000004d0: 2a20 6465 636f 6e76 6f6c 7574 696f 6e20  * deconvolution 
+000004e0: 6f66 2065 6163 6820 6461 7461 7365 7420  of each dataset 
+000004f0: 696e 746f 2067 656e 6520 6578 7072 6573  into gene expres
+00000500: 7369 6f6e 2070 726f 6772 616d 7320 2847  sion programs (G
+00000510: 4550 7329 2e0d 0a2a 2a4e 6574 776f 726b  EPs)...**Network
+00000520: 2d62 6173 6564 2069 6e74 6567 7261 7469  -based integrati
+00000530: 6f6e 2a2a 206f 6620 4745 5073 2065 6e61  on** of GEPs ena
+00000540: 626c 6573 2066 6c65 7869 626c 6520 696e  bles flexible in
+00000550: 7465 6772 6174 696f 6e20 6f66 206d 616e  tegration of man
+00000560: 7920 6461 7461 7365 7473 0d0a 6163 726f  y datasets..acro
+00000570: 7373 2061 7373 6179 7320 2865 672e 2050  ss assays (eg. P
+00000580: 726f 7465 696e 2c20 524e 412d 5365 712c  rotein, RNA-Seq,
+00000590: 2073 6352 4e41 2d53 6571 2c20 7370 6174   scRNA-Seq, spat
+000005a0: 6961 6c20 6578 7072 6573 7369 6f6e 2920  ial expression) 
+000005b0: 616e 6420 7061 7469 656e 7420 636f 686f  and patient coho
+000005c0: 7274 732e 0d0a 0d0a 436f 6d6d 756e 6974  rts.....Communit
+000005d0: 6965 7320 7769 7468 2047 4550 7320 6672  ies with GEPs fr
+000005e0: 6f6d 206d 756c 7469 706c 6520 6461 7461  om multiple data
+000005f0: 7365 7473 2063 616e 2062 6520 616e 6e6f  sets can be anno
+00000600: 7461 7465 6420 7769 7468 2064 6174 6173  tated with datas
+00000610: 6574 2d73 7065 6369 6669 630d 0a61 6e6e  et-specific..ann
+00000620: 6f74 6174 696f 6e73 2074 6f20 6661 6369  otations to faci
+00000630: 6c69 7461 7465 2069 6e74 6572 7072 6574  litate interpret
+00000640: 6174 696f 6e2e 0d0a 0d0a 2323 20e2 9aa1  ation.....## ...
+00000650: 4d61 696e 2046 6561 7475 7265 730d 0a0d  Main Features...
+00000660: 0a48 6572 6520 6172 6520 6a75 7374 2061  .Here are just a
+00000670: 2066 6577 206f 6620 7468 6520 7468 696e   few of the thin
+00000680: 6773 2074 6861 7420 634e 4d46 2d53 4e53  gs that cNMF-SNS
+00000690: 2064 6f65 7320 7765 6c6c 3a0d 0a0d 0a2d   does well:....-
+000006a0: 2049 6465 6e74 6966 6965 7320 696e 7465   Identifies inte
+000006b0: 7270 7265 7461 626c 652c 2061 6464 6974  rpretable, addit
+000006c0: 6976 6520 6e6f 6e2d 6e65 6761 7469 7665  ive non-negative
+000006d0: 2067 656e 6520 6578 7072 6573 7369 6f6e   gene expression
+000006e0: 2070 726f 6772 616d 730d 0a2d 204d 6f73   programs..- Mos
+000006f0: 6169 6320 696e 7465 6772 6174 696f 6e20  aic integration 
+00000700: 646f 6573 206e 6f74 2072 6571 7569 7265  does not require
+00000710: 2073 7562 7365 7474 696e 6720 6665 6174   subsetting feat
+00000720: 7572 6573 2f67 656e 6573 2074 6f0d 0a20  ures/genes to.. 
+00000730: 2061 2073 6861 7265 6420 6f72 206f 7665   a shared or ove
+00000740: 7264 6973 7065 7273 6564 2073 7562 7365  rdispersed subse
+00000750: 740d 0a2d 2049 6465 616c 2066 6f72 2069  t..- Ideal for i
+00000760: 6e63 7265 6d65 6e74 616c 2069 6e74 6567  ncremental integ
+00000770: 7261 7469 6f6e 2028 6164 6469 6e67 2064  ration (adding d
+00000780: 6174 6173 6574 7320 6f6e 6520 6174 2061  atasets one at a
+00000790: 2074 696d 6529 2073 696e 6365 0d0a 2020   time) since..  
+000007a0: 6465 636f 6e76 6f6c 7574 696f 6e20 6973  deconvolution is
+000007b0: 2070 6572 666f 726d 6564 2069 6e64 6570   performed indep
+000007c0: 656e 6465 6e74 6c79 206f 6e20 6561 6368  endently on each
+000007d0: 2064 6174 6173 6574 2067 656e 6572 6174   dataset generat
+000007e0: 696e 6720 696e 7661 7269 616e 7420 4745  ing invariant GE
+000007f0: 5073 0d0a 2d20 496e 7465 6772 6174 696f  Ps..- Integratio
+00000800: 6e20 646f 6573 206e 6f74 2072 6571 7569  n does not requi
+00000810: 7265 2063 6f6d 7061 7261 626c 6520 6461  re comparable da
+00000820: 7461 2073 7061 7273 6974 7920 6f72 2073  ta sparsity or s
+00000830: 6571 7565 6e63 696e 6720 6465 7074 6820  equencing depth 
+00000840: 2873 696e 676c 652d 6365 6c6c 2c20 6d69  (single-cell, mi
+00000850: 6372 6f61 7272 6179 2c20 6275 6c6b 290d  croarray, bulk).
+00000860: 0a2d 2054 776f 2069 6e74 6572 6661 6365  .- Two interface
+00000870: 733a 2063 6f6d 6d61 6e64 2d6c 696e 6520  s: command-line 
+00000880: 696e 7465 7266 6163 6520 666f 7220 7261  interface for ra
+00000890: 7069 6420 6461 7461 2065 7870 6c6f 7261  pid data explora
+000008a0: 7469 6f6e 2061 6e64 2070 7974 686f 6e0d  tion and python.
+000008b0: 0a20 2069 6e74 6572 6661 6365 2066 6f72  .  interface for
+000008c0: 2065 7874 656e 7369 6269 6c69 7479 2061   extensibility a
+000008d0: 6e64 2066 6c65 7869 6269 6c69 7479 0d0a  nd flexibility..
+000008e0: 0d0a 2323 20f0 9f94 a720 496e 7374 616c  ..## .... Instal
+000008f0: 6c0d 0a0d 0a23 2323 20e2 9881 efb8 8f20  l....### ...... 
+00000900: 5075 626c 6963 2052 656c 6561 7365 0d0a  Public Release..
+00000910: 0d0a 496e 7374 616c 6c20 7468 6520 7061  ..Install the pa
+00000920: 636b 6167 6520 7769 7468 2063 6f6e 6461  ckage with conda
+00000930: 3a0d 0a60 6060 6261 7368 0d0a 636f 6e64  :..```bash..cond
+00000940: 6120 696e 7374 616c 6c20 2d63 2063 6f6e  a install -c con
+00000950: 6461 2d66 6f72 6765 2063 6e6d 6673 6e73  da-forge cnmfsns
+00000960: 0d0a 6060 600d 0a0d 0a23 2323 20e2 9ca8  ..```....### ...
+00000970: 204c 6174 6573 7420 7665 7273 696f 6e20   Latest version 
+00000980: 6672 6f6d 2047 6974 4875 620d 0a0d 0a42  from GitHub....B
+00000990: 6566 6f72 6520 696e 7374 616c 6c69 6e67  efore installing
+000009a0: 2063 4e4d 462d 534e 5320 7573 696e 6720   cNMF-SNS using 
+000009b0: 7069 702c 2069 7420 6973 2072 6563 6f6d  pip, it is recom
+000009c0: 6d65 6e64 6564 2074 6f20 6669 7273 7420  mended to first 
+000009d0: 7365 7420 7570 2061 2073 6570 6172 6174  set up a separat
+000009e0: 6520 636f 6e64 6120 656e 7669 726f 6e6d  e conda environm
+000009f0: 656e 7420 616e 6420 6861 7665 2063 6f6e  ent and have con
+00000a00: 6461 206d 616e 6167 6520 6173 206d 616e  da manage as man
+00000a10: 7920 6465 7065 6e64 656e 6369 6573 2061  y dependencies a
+00000a20: 7320 706f 7373 6962 6c65 2e0d 0a0d 0a60  s possible.....`
+00000a30: 6060 6261 7368 0d0a 636f 6e64 6120 6372  ``bash..conda cr
+00000a40: 6561 7465 202d 2d6e 616d 6520 636e 6d66  eate --name cnmf
+00000a50: 736e 7320 2d63 2063 6f6e 6461 2d66 6f72  sns -c conda-for
+00000a60: 6765 2070 7974 686f 6e3d 332e 3130 2061  ge python=3.10 a
+00000a70: 6e6e 6461 7461 2070 616e 6461 7320 6e75  nndata pandas nu
+00000a80: 6d70 7920 7363 6970 7920 6d61 7470 6c6f  mpy scipy matplo
+00000a90: 746c 6962 2075 7073 6574 706c 6f74 2068  tlib upsetplot h
+00000aa0: 7474 706c 6962 3220 746f 6d6c 6920 746f  ttplib2 tomli to
+00000ab0: 6d6c 692d 7720 636c 6963 6b20 7079 6772  mli-w click pygr
+00000ac0: 6170 6876 697a 2070 7974 686f 6e2d 6967  aphviz python-ig
+00000ad0: 7261 7068 2073 656d 616e 7469 635f 7665  raph semantic_ve
+00000ae0: 7273 696f 6e20 7079 7961 6d6c 2073 6369  rsion pyyaml sci
+00000af0: 6b69 742d 6c65 6172 6e20 6661 7374 636c  kit-learn fastcl
+00000b00: 7573 7465 7220 7363 616e 7079 2070 7979  uster scanpy pyy
+00000b10: 616d 6c0d 0a63 6f6e 6461 2061 6374 6976  aml..conda activ
+00000b20: 6174 6520 636e 6d66 736e 730d 0a70 6970  ate cnmfsns..pip
+00000b30: 2069 6e73 7461 6c6c 2067 6974 2b68 7474   install git+htt
+00000b40: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000b50: 4d6f 7272 6973 7379 4c61 622f 634e 4d46  MorrissyLab/cNMF
+00000b60: 2d53 4e53 2e67 6974 0d0a 6060 600d 0a0d  -SNS.git..```...
+00000b70: 0a23 2320 f09f 9396 2044 6f63 756d 656e  .## .... Documen
+00000b80: 7461 7469 6f6e 0d0a 0d0a 2323 2320 f09f  tation....### ..
+00000b90: 9393 2050 7974 686f 6e20 696e 7465 7266  .. Python interf
+00000ba0: 6163 650d 0a0d 0a54 6f20 6765 7420 7374  ace....To get st
+00000bb0: 6172 7465 642c 2073 616d 706c 6520 7072  arted, sample pr
+00000bc0: 6f74 656f 6d69 6373 2064 6174 6173 6574  oteomics dataset
+00000bd0: 7320 616e 6420 6120 4a75 7079 7465 7220  s and a Jupyter 
+00000be0: 6e6f 7465 626f 6f6b 2074 7574 6f72 6961  notebook tutoria
+00000bf0: 6c20 6973 2061 7661 696c 6162 6c65 205b  l is available [
+00000c00: 6865 7265 5d28 2f74 7574 6f72 6961 6c2f  here](/tutorial/
+00000c10: 7475 746f 7269 616c 2e69 7079 6e62 292e  tutorial.ipynb).
+00000c20: 0d0a 0d0a 4465 7461 696c 6564 2041 5049  ....Detailed API
+00000c30: 2072 6566 6572 656e 6365 2063 616e 2062   reference can b
+00000c40: 6520 666f 756e 6420 6f6e 205b 5265 6164  e found on [Read
+00000c50: 5468 6544 6f63 735d 2868 7474 7073 3a2f  TheDocs](https:/
+00000c60: 2f63 6e6d 662d 736e 732e 7265 6164 7468  /cnmf-sns.readth
+00000c70: 6564 6f63 732e 696f 2f29 2e0d 0a0d 0a0d  edocs.io/)......
+00000c80: 0a23 2323 20e2 8ca8 efb8 8f20 436f 6d6d  .### ...... Comm
+00000c90: 616e 6420 6c69 6e65 2069 6e74 6572 6661  and line interfa
+00000ca0: 6365 0d0a 0d0a 5365 6520 7468 6520 5b63  ce....See the [c
+00000cb0: 6f6d 6d61 6e64 206c 696e 6520 696e 7465  ommand line inte
+00000cc0: 7266 6163 6520 646f 6375 6d65 6e74 6174  rface documentat
+00000cd0: 696f 6e5d 282f 434c 492e 6d64 292e 0d0a  ion](/CLI.md)...
+00000ce0: 0d0a 2323 20f0 9f92 ad20 4765 7474 696e  ..## .... Gettin
+00000cf0: 6720 4865 6c70 0d0a 0d0a 466f 7220 6572  g Help....For er
+00000d00: 726f 7273 2061 7269 7369 6e67 2064 7572  rors arising dur
+00000d10: 696e 6720 7573 6520 6f66 2063 4e4d 462d  ing use of cNMF-
+00000d20: 534e 532c 2063 7265 6174 6520 616e 6420  SNS, create and 
+00000d30: 6272 6f77 7365 2069 7373 7565 7320 696e  browse issues in
+00000d40: 2074 6865 205b 4769 7448 7562 2022 6973   the [GitHub "is
+00000d50: 7375 6573 2220 7461 625d 2868 7474 7073  sues" tab](https
+00000d60: 3a2f 2f67 6974 6875 622e 636f 6d2f 4d6f  ://github.com/Mo
+00000d70: 7272 6973 7379 4c61 622f 634e 4d46 2d53  rrissyLab/cNMF-S
+00000d80: 4e53 2f69 7373 7565 7329 2e              NS/issues).
```

### Comparing `cnmfsns-1.3.0/setup.cfg` & `cnmfsns-1.3.1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6e6d 6673 6e73 0d0a 7665 7273   = cnmfsns..vers
-00000020: 696f 6e20 3d20 312e 332e 300d 0a61 7574  ion = 1.3.0..aut
+00000020: 696f 6e20 3d20 312e 332e 310d 0a61 7574  ion = 1.3.1..aut
 00000030: 686f 7220 3d20 5465 6420 5665 7268 6579  hor = Ted Verhey
 00000040: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000050: 2074 6276 6572 6865 7940 7563 616c 6761   tbverhey@ucalga
 00000060: 7279 2e63 610d 0a64 6573 6372 6970 7469  ry.ca..descripti
 00000070: 6f6e 203d 2063 4e4d 4620 536f 6c75 7469  on = cNMF Soluti
 00000080: 6f6e 204e 6574 776f 726b 2053 7061 6365  on Network Space
 00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
```

### Comparing `cnmfsns-1.3.0/src/cnmfsns/__init__.py` & `cnmfsns-1.3.1/src/cnmfsns/__init__.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.0/src/cnmfsns/cli.py` & `cnmfsns-1.3.1/src/cnmfsns/cli.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.0/src/cnmfsns/cnmf.py` & `cnmfsns-1.3.1/src/cnmfsns/cnmf.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.0/src/cnmfsns/colors.py` & `cnmfsns-1.3.1/src/cnmfsns/colors.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.0/src/cnmfsns/config.py` & `cnmfsns-1.3.1/src/cnmfsns/config.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.0/src/cnmfsns/dataset.py` & `cnmfsns-1.3.1/src/cnmfsns/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,2100 +96,2101 @@
 000005f0: 7373 696f 6e20 6461 7461 2028 6164 6174  ssion data (adat
 00000600: 612e 5829 2229 0d0a 2020 2020 2020 2020  a.X)")..        
 00000610: 2020 2020 7261 6973 6520 5661 6c75 6545      raise ValueE
 00000620: 7272 6f72 2829 0d0a 2020 2020 2020 2020  rror()..        
 00000630: 0d0a 2020 2020 2020 2020 7365 6c66 2e70  ..        self.p
 00000640: 6174 6965 6e74 5f69 645f 636f 6c20 3d20  atient_id_col = 
 00000650: 7061 7469 656e 745f 6964 5f63 6f6c 0d0a  patient_id_col..
-00000660: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
-00000670: 7472 2861 6461 7461 2c20 2263 6e6d 6673  tr(adata, "cnmfs
-00000680: 6e73 5f76 6572 7369 6f6e 2229 2061 6e64  ns_version") and
-00000690: 2061 6461 7461 2e63 6e6d 6673 6e73 5f76   adata.cnmfsns_v
-000006a0: 6572 7369 6f6e 2069 7320 6e6f 7420 4e6f  ersion is not No
-000006b0: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-000006c0: 2073 656c 662e 6164 6174 6120 3d20 6164   self.adata = ad
-000006d0: 6174 610d 0a20 2020 2020 2020 2065 6c73  ata..        els
-000006e0: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
-000006f0: 2320 6368 6563 6b20 616e 6420 7570 6461  # check and upda
-00000700: 7465 206f 6c64 206f 7220 6578 7465 726e  te old or extern
-00000710: 616c 2068 3561 6420 6669 6c65 7320 666f  al h5ad files fo
-00000720: 7220 634e 4d46 2d53 4e53 2063 6f6d 706c  r cNMF-SNS compl
-00000730: 6961 6e63 650d 0a20 2020 200d 0a20 2020  iance..    ..   
-00000740: 2020 2020 2020 2020 2058 203d 2061 6461           X = ada
-00000750: 7461 2e74 6f5f 6466 2829 0d0a 2020 2020  ta.to_df()..    
-00000760: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00000770: 2020 2020 2020 6966 2061 6461 7461 2e69        if adata.i
-00000780: 7362 6163 6b65 643a 0d0a 2020 2020 2020  sbacked:..      
-00000790: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000007a0: 5275 6e74 696d 6545 7272 6f72 2822 6164  RuntimeError("ad
-000007b0: 6174 6120 6973 2061 2062 6163 6b65 6420  ata is a backed 
-000007c0: 416e 6e44 6174 6120 6f62 6a65 6374 2e20  AnnData object. 
-000007d0: 416e 6e44 6174 6120 6f62 6a65 6374 7320  AnnData objects 
-000007e0: 6f70 656e 6564 2069 6e20 6261 636b 6564  opened in backed
-000007f0: 206d 6f64 6520 6361 6e6e 6f74 2062 6520   mode cannot be 
-00000800: 6d69 6772 6174 6564 2e22 290d 0a0d 0a20  migrated.").... 
-00000810: 2020 2020 2020 2020 2020 2069 6620 6164             if ad
-00000820: 6174 612e 7261 7720 6973 204e 6f6e 653a  ata.raw is None:
-00000830: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000840: 2020 6973 5f6e 6f72 6d61 6c69 7a65 643d    is_normalized=
-00000850: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-00000860: 2020 2020 2020 2072 6177 203d 2061 6461         raw = ada
-00000870: 7461 2e74 6f5f 6466 2829 0d0a 2020 2020  ta.to_df()..    
-00000880: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-00000890: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000008a0: 6177 203d 2070 642e 4461 7461 4672 616d  aw = pd.DataFram
-000008b0: 6528 6164 6174 612e 7261 772e 582c 2069  e(adata.raw.X, i
-000008c0: 6e64 6578 3d58 2e69 6e64 6578 2c20 636f  ndex=X.index, co
-000008d0: 6c75 6d6e 733d 582e 636f 6c75 6d6e 7329  lumns=X.columns)
-000008e0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000008f0: 2020 636f 7272 6469 7374 203d 2058 2e63    corrdist = X.c
-00000900: 6f72 7277 6974 6828 7261 772c 2061 7869  orrwith(raw, axi
-00000910: 733d 3129 0d0a 2020 2020 2020 2020 2020  s=1)..          
-00000920: 2020 2020 2020 2320 6368 6563 6b73 2074        # checks t
-00000930: 6861 7420 616c 6c20 7361 6d70 6c65 7320  hat all samples 
-00000940: 6172 6520 7065 7266 6563 746c 7920 636f  are perfectly co
-00000950: 7272 656c 6174 6564 2062 6574 7765 656e  rrelated between
-00000960: 2063 6f75 6e74 7320 616e 6420 6e6f 726d   counts and norm
-00000970: 616c 697a 6564 2064 6174 610d 0a20 2020  alized data..   
-00000980: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00000990: 2828 636f 7272 6469 7374 202d 2031 292e  ((corrdist - 1).
-000009a0: 6162 7328 2920 3e20 3165 2d36 292e 616e  abs() > 1e-6).an
-000009b0: 7928 293a 0d0a 2020 2020 2020 2020 2020  y():..          
-000009c0: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
-000009d0: 672e 7761 726e 696e 6728 2243 6f75 6e74  g.warning("Count
-000009e0: 7320 616e 6420 6e6f 726d 616c 697a 6564  s and normalized
-000009f0: 2065 7870 7265 7373 696f 6e20 6d61 7472   expression matr
-00000a00: 6963 6573 2061 7265 206e 6f74 2070 6572  ices are not per
-00000a10: 6665 6374 6c79 2063 6f72 7265 6c61 7465  fectly correlate
-00000a20: 642e 2043 6f75 6e74 7320 6461 7461 2077  d. Counts data w
-00000a30: 696c 6c20 6265 2072 6574 6169 6e65 6420  ill be retained 
-00000a40: 696e 206d 6967 7261 7465 6420 6f62 6a65  in migrated obje
-00000a50: 6374 2e22 290d 0a20 2020 2020 2020 2020  ct.")..         
-00000a60: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-00000a70: 7420 666f 7263 655f 6d69 6772 6174 653a  t force_migrate:
-00000a80: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00000a90: 2020 2020 2020 2020 2020 6572 726f 726d            errorm
-00000aa0: 7367 203d 2022 436f 756c 6420 6e6f 7420  sg = "Could not 
-00000ab0: 6d69 6772 6174 6520 416e 6e44 6174 6120  migrate AnnData 
-00000ac0: 6f62 6a65 6374 2e22 0d0a 2020 2020 2020  object."..      
-00000ad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000ae0: 2020 6c6f 6767 696e 672e 6572 726f 7228    logging.error(
-00000af0: 6572 726f 726d 7367 290d 0a20 2020 2020  errormsg)..     
-00000b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000b10: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00000b20: 726f 7228 6572 726f 726d 7367 290d 0a20  ror(errormsg).. 
-00000b30: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00000b40: 2063 6865 636b 2066 6f72 2077 6865 7468   check for wheth
-00000b50: 6572 2075 7365 7220 6f72 6967 696e 616c  er user original
-00000b60: 6c79 2069 6e70 7574 206e 6f72 6d61 6c69  ly input normali
-00000b70: 7a65 6420 6f72 2063 6f75 6e74 7320 6461  zed or counts da
-00000b80: 7461 0d0a 2020 2020 2020 2020 2020 2020  ta..            
-00000b90: 2020 2020 6973 5f6e 6f72 6d61 6c69 7a65      is_normalize
-00000ba0: 6420 3d20 2828 5820 2d20 7261 7729 2e61  d = ((X - raw).a
-00000bb0: 6273 2829 203c 2031 652d 3629 2e61 6c6c  bs() < 1e-6).all
-00000bc0: 2829 2e61 6c6c 2829 0d0a 2020 2020 2020  ().all()..      
-00000bd0: 2020 2020 2020 2020 2020 585f 6973 5f74            X_is_t
-00000be0: 706d 203d 2028 2858 2e73 756d 2861 7869  pm = ((X.sum(axi
-00000bf0: 733d 3129 202d 2031 6536 292e 6162 7328  s=1) - 1e6).abs(
-00000c00: 2920 3e20 3165 3229 2e61 6e79 2829 0d0a  ) > 1e2).any()..
-00000c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000c20: 6966 2069 735f 6e6f 726d 616c 697a 6564  if is_normalized
-00000c30: 2061 6e64 206e 6f74 2058 5f69 735f 7470   and not X_is_tp
-00000c40: 6d3a 0d0a 2020 2020 2020 2020 2020 2020  m:..            
-00000c50: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-00000c60: 7761 726e 696e 6728 2241 6e6e 4461 7461  warning("AnnData
-00000c70: 206f 626a 6563 7420 636f 6e74 6169 6e73   object contains
-00000c80: 206e 6f6e 2d54 504d 206e 6f72 6d61 6c69   non-TPM normali
-00000c90: 7a65 6420 6461 7461 2e20 4e65 7720 416e  zed data. New An
-00000ca0: 6e44 6174 6120 6f62 6a65 6374 2077 696c  nData object wil
-00000cb0: 6c20 7265 7461 696e 2074 6865 2063 6f75  l retain the cou
-00000cc0: 6e74 2028 756e 6e6f 726d 616c 697a 6564  nt (unnormalized
-00000cd0: 2920 6461 7461 206f 6e6c 792e 2229 0d0a  ) data only.")..
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000cf0: 0d0a 2020 2020 2020 2020 2020 2020 6966  ..            if
-00000d00: 2022 6f64 6722 2069 6e20 6164 6174 612e   "odg" in adata.
-00000d10: 756e 7320 616e 6420 2267 656e 655f 7374  uns and "gene_st
-00000d20: 6174 7322 2069 6e20 6164 6174 612e 756e  ats" in adata.un
-00000d30: 735b 226f 6467 225d 3a0d 0a20 2020 2020  s["odg"]:..     
-00000d40: 2020 2020 2020 2020 2020 2067 656e 655f             gene_
-00000d50: 7374 6174 5f63 6f6c 756d 6e73 203d 2061  stat_columns = a
-00000d60: 6461 7461 2e75 6e73 5b22 6f64 6722 5d5b  data.uns["odg"][
-00000d70: 2267 656e 655f 7374 6174 7322 5d2e 636f  "gene_stats"].co
-00000d80: 6c75 6d6e 730d 0a20 2020 2020 2020 2020  lumns..         
-00000d90: 2020 2020 2020 2069 6620 6164 6174 612e         if adata.
-00000da0: 7661 722e 636f 6c75 6d6e 732e 6973 696e  var.columns.isin
-00000db0: 2867 656e 655f 7374 6174 5f63 6f6c 756d  (gene_stat_colum
-00000dc0: 6e73 292e 616e 7928 293a 0d0a 2020 2020  ns).any():..    
-00000dd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000de0: 6f76 6572 6c61 7070 696e 675f 636f 6c73  overlapping_cols
-00000df0: 203d 2061 6461 7461 2e76 6172 2e63 6f6c   = adata.var.col
-00000e00: 756d 6e73 2e69 7369 6e28 6765 6e65 5f73  umns.isin(gene_s
-00000e10: 7461 745f 636f 6c75 6d6e 7329 0d0a 2020  tat_columns)..  
-00000e20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000e30: 2020 6f76 6572 6c61 7070 696e 675f 636f    overlapping_co
-00000e40: 6c73 7472 203d 2022 2c20 222e 6a6f 696e  lstr = ", ".join
-00000e50: 286f 7665 726c 6170 7069 6e67 5f63 6f6c  (overlapping_col
-00000e60: 735b 6f76 6572 6c61 7070 696e 675f 636f  s[overlapping_co
-00000e70: 6c73 5d2e 696e 6465 782e 746f 5f6c 6973  ls].index.to_lis
-00000e80: 7428 2929 0d0a 2020 2020 2020 2020 2020  t())..          
-00000e90: 2020 2020 2020 2020 2020 6c6f 6767 696e            loggin
-00000ea0: 672e 7761 726e 696e 6728 6622 416e 6e44  g.warning(f"AnnD
-00000eb0: 6174 6120 6f62 6a65 6374 2063 6f6e 7461  ata object conta
-00000ec0: 696e 7320 634e 4d46 2067 656e 6520 7374  ins cNMF gene st
-00000ed0: 6174 7320 7768 6963 6820 7769 6c6c 206f  ats which will o
-00000ee0: 7665 7272 6964 6520 636f 6c75 6d6e 7320  verride columns 
-00000ef0: 696e 2061 6461 7461 2e76 6172 3a20 7b6f  in adata.var: {o
-00000f00: 7665 726c 6170 7069 6e67 5f63 6f6c 7374  verlapping_colst
-00000f10: 727d 2229 0d0a 2020 2020 2020 2020 2020  r}")..          
-00000f20: 2020 2020 2020 6164 6174 612e 7661 7220        adata.var 
-00000f30: 3d20 7064 2e6d 6572 6765 286c 6566 743d  = pd.merge(left=
-00000f40: 6164 6174 612e 7661 722c 2072 6967 6874  adata.var, right
-00000f50: 3d61 6461 7461 2e75 6e73 5b22 6f64 6722  =adata.uns["odg"
-00000f60: 5d5b 2267 656e 655f 7374 6174 7322 5d2c  ]["gene_stats"],
-00000f70: 2068 6f77 3d22 6c65 6674 222c 206c 6566   how="left", lef
-00000f80: 745f 696e 6465 783d 5472 7565 2c20 7269  t_index=True, ri
-00000f90: 6768 745f 696e 6465 783d 5472 7565 290d  ght_index=True).
-00000fa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000fb0: 2064 656c 2061 6461 7461 2e75 6e73 5b22   del adata.uns["
-00000fc0: 6f64 6722 5d5b 2267 656e 655f 7374 6174  odg"]["gene_stat
-00000fd0: 7322 5d0d 0a20 2020 2020 2020 2020 2020  s"]..           
-00000fe0: 200d 0a20 2020 2020 2020 2020 2020 2023   ..            #
-00000ff0: 2063 7265 6174 6520 6e65 7720 416e 6e44   create new AnnD
-00001000: 6174 6120 6f62 6a65 6374 0d0a 2020 2020  ata object..    
-00001010: 2020 2020 2020 2020 6e65 775f 6164 6174          new_adat
-00001020: 6120 3d20 6164 2e41 6e6e 4461 7461 2858  a = ad.AnnData(X
-00001030: 3d72 6177 2c20 6f62 733d 6164 6174 612e  =raw, obs=adata.
-00001040: 6f62 732c 2076 6172 3d61 6461 7461 2e76  obs, var=adata.v
-00001050: 6172 2c20 7661 726d 3d61 6461 7461 2e76  ar, varm=adata.v
-00001060: 6172 6d2c 206f 6273 6d3d 6164 6174 612e  arm, obsm=adata.
-00001070: 6f62 736d 2c20 756e 733d 6164 6174 612e  obsm, uns=adata.
-00001080: 756e 7329 0d0a 2020 2020 2020 2020 2020  uns)..          
-00001090: 2020 6966 2022 6869 7374 6f72 7922 206e    if "history" n
-000010a0: 6f74 2069 6e20 6e65 775f 6164 6174 612e  ot in new_adata.
-000010b0: 756e 733a 0d0a 2020 2020 2020 2020 2020  uns:..          
-000010c0: 2020 2020 2020 6e65 775f 6164 6174 612e        new_adata.
-000010d0: 756e 735b 2268 6973 746f 7279 225d 203d  uns["history"] =
-000010e0: 207b 7d0d 0a0d 0a20 2020 2020 2020 2020   {}....         
-000010f0: 2020 2023 2075 7064 6174 6520 6461 7461     # update data
-00001100: 7365 7420 6f62 6a65 6374 0d0a 2020 2020  set object..    
-00001110: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
-00001120: 7461 203d 206e 6577 5f61 6461 7461 0d0a  ta = new_adata..
-00001130: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001140: 2e69 735f 6e6f 726d 616c 697a 6564 203d  .is_normalized =
-00001150: 2069 735f 6e6f 726d 616c 697a 6564 0d0a   is_normalized..
-00001160: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00001170: 2e63 6e6d 6673 6e73 5f76 6572 7369 6f6e  .cnmfsns_version
-00001180: 203d 205f 5f76 6572 7369 6f6e 5f5f 0d0a   = __version__..
-00001190: 2020 2020 0d0a 2020 2020 4063 6c61 7373      ..    @class
-000011a0: 6d65 7468 6f64 0d0a 2020 2020 6465 6620  method..    def 
-000011b0: 6672 6f6d 5f64 6628 636c 732c 0d0a 2020  from_df(cls,..  
-000011c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000011d0: 6461 7461 3a20 7064 2e44 6174 6146 7261  data: pd.DataFra
-000011e0: 6d65 2c0d 0a20 2020 2020 2020 2020 2020  me,..           
-000011f0: 2020 2020 2020 2069 735f 6e6f 726d 616c         is_normal
-00001200: 697a 6564 3a20 626f 6f6c 2c0d 0a20 2020  ized: bool,..   
-00001210: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00001220: 7061 7273 6966 793a 2062 6f6f 6c20 3d20  parsify: bool = 
-00001230: 4661 6c73 652c 0d0a 2020 2020 2020 2020  False,..        
-00001240: 2020 2020 2020 2020 2020 6f62 733a 204f            obs: O
-00001250: 7074 696f 6e61 6c5b 7064 2e44 6174 6146  ptional[pd.DataF
-00001260: 7261 6d65 5d20 3d20 4e6f 6e65 2c0d 0a20  rame] = None,.. 
-00001270: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001280: 2076 6172 3a20 4f70 7469 6f6e 616c 5b70   var: Optional[p
-00001290: 642e 4461 7461 4672 616d 655d 203d 204e  d.DataFrame] = N
-000012a0: 6f6e 652c 0d0a 2020 2020 2020 2020 2020  one,..          
-000012b0: 2020 2020 2020 2020 7061 7469 656e 745f          patient_
-000012c0: 6964 5f63 6f6c 3a20 4f70 7469 6f6e 616c  id_col: Optional
-000012d0: 5b73 7472 5d20 3d20 4e6f 6e65 0d0a 2020  [str] = None..  
-000012e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000012f0: 293a 0d0a 2020 2020 2020 2020 2222 2243  ):..        """C
-00001300: 7265 6174 6573 2061 203a 636c 6173 733a  reates a :class:
-00001310: 607e 636e 6d66 736e 732e 6461 7461 7365  `~cnmfsns.datase
-00001320: 742e 4461 7461 7365 7460 206f 626a 6563  t.Dataset` objec
-00001330: 7420 6672 6f6d 2061 2070 616e 6461 7320  t from a pandas 
-00001340: 4461 7461 4672 616d 652e 0d0a 0d0a 2020  DataFrame.....  
-00001350: 2020 2020 2020 3a70 6172 616d 2064 6174        :param dat
-00001360: 613a 2041 6e20 6f62 7365 7276 6174 696f  a: An observatio
-00001370: 6e73 20c3 9720 7661 7269 6162 6c65 7320  ns .. variables 
-00001380: 6461 7461 0d0a 2020 2020 2020 2020 3a74  data..        :t
-00001390: 7970 6520 6461 7461 3a20 7064 2e44 6174  ype data: pd.Dat
-000013a0: 6146 7261 6d65 0d0a 2020 2020 2020 2020  aFrame..        
-000013b0: 3a70 6172 616d 2069 735f 6e6f 726d 616c  :param is_normal
-000013c0: 697a 6564 3a20 5370 6563 6966 7920 6966  ized: Specify if
-000013d0: 2064 6174 6120 6973 2061 6c72 6561 6479   data is already
-000013e0: 206e 6f72 6d61 6c69 7a65 6420 6f72 2077   normalized or w
-000013f0: 6865 7468 6572 206e 6f74 2e20 5261 7720  hether not. Raw 
-00001400: 6461 7461 2077 696c 6c20 6265 2054 504d  data will be TPM
-00001410: 206e 6f72 6d61 6c69 7a65 6420 7072 696f   normalized prio
-00001420: 7220 746f 206f 7665 7264 6973 7065 7273  r to overdispers
-00001430: 6564 2067 656e 6520 7365 6c65 6374 696f  ed gene selectio
-00001440: 6e2c 2077 6865 7265 6173 2061 6c72 6561  n, whereas alrea
-00001450: 6479 206e 6f72 6d61 6c69 7a65 6420 6461  dy normalized da
-00001460: 7461 2077 696c 6c20 6e6f 742e 0d0a 2020  ta will not...  
-00001470: 2020 2020 2020 3a74 7970 6520 6973 5f6e        :type is_n
-00001480: 6f72 6d61 6c69 7a65 643a 2062 6f6f 6c0d  ormalized: bool.
-00001490: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000014a0: 7370 6172 7369 6679 3a20 5374 6f72 6520  sparsify: Store 
-000014b0: 6461 7461 2061 7320 6120 7370 6172 7365  data as a sparse
-000014c0: 206d 6174 7269 782e 205b 4e6f 7465 2074   matrix. [Note t
-000014d0: 6861 7420 7468 6973 2066 6561 7475 7265  hat this feature
-000014e0: 2069 7320 6578 7065 7269 6d65 6e74 616c   is experimental
-000014f0: 5d2c 2064 6566 6175 6c74 7320 746f 2046  ], defaults to F
-00001500: 616c 7365 0d0a 2020 2020 2020 2020 3a74  alse..        :t
-00001510: 7970 6520 7370 6172 7369 6679 3a20 626f  ype sparsify: bo
-00001520: 6f6c 2c20 6f70 7469 6f6e 616c 0d0a 2020  ol, optional..  
-00001530: 2020 2020 2020 3a70 6172 616d 206f 6273        :param obs
-00001540: 3a20 416e 206f 6273 6572 7661 7469 6f6e  : An observation
-00001550: 7320 c397 206d 6574 6164 6174 6120 6d61  s .. metadata ma
-00001560: 7472 6978 2c20 6465 6661 756c 7473 2074  trix, defaults t
-00001570: 6f20 4e6f 6e65 0d0a 2020 2020 2020 2020  o None..        
-00001580: 3a74 7970 6520 6f62 733a 2060 7064 2e44  :type obs: `pd.D
-00001590: 6174 6146 7261 6d65 602c 206f 7074 696f  ataFrame`, optio
-000015a0: 6e61 6c0d 0a20 2020 2020 2020 203a 7061  nal..        :pa
-000015b0: 7261 6d20 7661 723a 2041 2076 6172 6961  ram var: A varia
-000015c0: 626c 6573 20c3 9720 6d65 7461 6461 7461  bles .. metadata
-000015d0: 206d 6174 7269 782c 2064 6566 6175 6c74   matrix, default
-000015e0: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
-000015f0: 2020 203a 7479 7065 2076 6172 3a20 6070     :type var: `p
-00001600: 642e 4461 7461 4672 616d 6560 2c20 6f70  d.DataFrame`, op
-00001610: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00001620: 3a70 6172 616d 2070 6174 6965 6e74 5f69  :param patient_i
-00001630: 645f 636f 6c3a 204e 616d 6520 6f66 206d  d_col: Name of m
-00001640: 6574 6164 6174 6120 6c61 7965 7220 7769  etadata layer wi
-00001650: 7468 2070 6174 6965 6e74 2049 4420 696e  th patient ID in
-00001660: 666f 726d 6174 696f 6e2c 2064 6566 6175  formation, defau
-00001670: 6c74 7320 746f 204e 6f6e 650d 0a20 2020  lts to None..   
-00001680: 2020 2020 203a 7479 7065 2070 6174 6965       :type patie
-00001690: 6e74 5f69 645f 636f 6c3a 2073 7472 2c20  nt_id_col: str, 
-000016a0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-000016b0: 2020 3a72 6574 7572 6e3a 204f 626a 6563    :return: Objec
-000016c0: 7420 7769 7468 2065 7870 7265 7373 696f  t with expressio
-000016d0: 6e20 616e 6420 6d65 7461 6461 7461 0d0a  n and metadata..
-000016e0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-000016f0: 3a63 6c61 7373 3a60 7e63 6e6d 6673 6e73  :class:`~cnmfsns
-00001700: 2e64 6174 6173 6574 2e44 6174 6173 6574  .dataset.Dataset
-00001710: 600d 0a20 2020 2020 2020 2022 2222 0d0a  `..        """..
-00001720: 2020 2020 2020 2020 6966 2076 6172 2069          if var i
-00001730: 7320 6e6f 7420 4e6f 6e65 3a0d 0a20 2020  s not None:..   
-00001740: 2020 2020 2020 2020 2076 6172 203d 2076           var = v
-00001750: 6172 2e72 6569 6e64 6578 2864 6174 612e  ar.reindex(data.
-00001760: 636f 6c75 6d6e 7329 0d0a 2020 2020 2020  columns)..      
-00001770: 2020 6966 2073 7061 7273 6966 793a 0d0a    if sparsify:..
-00001780: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00001790: 203d 2073 702e 6373 725f 6d61 7472 6978   = sp.csr_matrix
-000017a0: 2864 6174 612e 7661 6c75 6573 290d 0a20  (data.values).. 
-000017b0: 2020 2020 2020 2064 6174 6120 3d20 6461         data = da
-000017c0: 7461 2e61 7374 7970 6528 2266 6c6f 6174  ta.astype("float
-000017d0: 3332 2229 0d0a 2020 2020 2020 2020 756e  32")..        un
-000017e0: 7320 3d20 7b22 6869 7374 6f72 7922 3a20  s = {"history": 
-000017f0: 7b7d 2c20 226f 6467 223a 7b7d 7d0d 0a20  {}, "odg":{}}.. 
-00001800: 2020 2020 2020 2061 6461 7461 203d 2061         adata = a
-00001810: 642e 416e 6e44 6174 6128 583d 6461 7461  d.AnnData(X=data
-00001820: 2c20 7661 723d 7661 722c 2075 6e73 3d75  , var=var, uns=u
-00001830: 6e73 290d 0a20 2020 2020 2020 2064 6174  ns)..        dat
-00001840: 6173 6574 203d 2063 6c73 2861 6461 7461  aset = cls(adata
-00001850: 3d61 6461 7461 2c20 7061 7469 656e 745f  =adata, patient_
-00001860: 6964 5f63 6f6c 3d70 6174 6965 6e74 5f69  id_col=patient_i
-00001870: 645f 636f 6c29 0d0a 2020 2020 2020 2020  d_col)..        
-00001880: 6966 206f 6273 2069 7320 6e6f 7420 4e6f  if obs is not No
-00001890: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
-000018a0: 2064 6174 6173 6574 2e75 7064 6174 655f   dataset.update_
-000018b0: 6f62 7328 6f62 733d 6f62 7329 200d 0a20  obs(obs=obs) .. 
-000018c0: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-000018d0: 7461 7365 740d 0a20 2020 200d 0a20 2020  taset..    ..   
-000018e0: 2040 636c 6173 736d 6574 686f 640d 0a20   @classmethod.. 
-000018f0: 2020 2064 6566 2066 726f 6d5f 6835 6164     def from_h5ad
-00001900: 2863 6c73 2c0d 0a20 2020 2020 2020 2020  (cls,..         
-00001910: 2020 2020 2020 2020 2068 3561 645f 6669           h5ad_fi
-00001920: 6c65 3a20 7374 722c 0d0a 2020 2020 2020  le: str,..      
-00001930: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
-00001940: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
-00001950: 3d20 4e6f 6e65 2c0d 0a20 2020 2020 2020  = None,..       
-00001960: 2020 2020 2020 2020 2020 2070 6174 6965             patie
-00001970: 6e74 5f69 645f 636f 6c3a 204f 7074 696f  nt_id_col: Optio
-00001980: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
-00001990: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000019a0: 2020 2020 666f 7263 655f 6d69 6772 6174      force_migrat
-000019b0: 653d 4661 6c73 652c 2062 6163 6b65 643d  e=False, backed=
-000019c0: 4661 6c73 650d 0a20 2020 2020 2020 2020  False..         
-000019d0: 2020 2020 2020 2020 2029 3a0d 0a20 2020           ):..   
-000019e0: 2020 2020 2022 2222 4372 6561 7465 7320       """Creates 
-000019f0: 6120 3a63 6c61 7373 3a60 7e63 6e6d 6673  a :class:`~cnmfs
-00001a00: 6e73 2e64 6174 6173 6574 2e44 6174 6173  ns.dataset.Datas
-00001a10: 6574 6020 6f62 6a65 6374 2066 726f 6d20  et` object from 
-00001a20: 616e 2041 6e6e 4461 7461 2d63 6f6d 7061  an AnnData-compa
-00001a30: 7469 626c 6520 2e68 3561 6420 6669 6c65  tible .h5ad file
-00001a40: 2e0d 0a0d 0a20 2020 2020 2020 203a 7061  .....        :pa
-00001a50: 7261 6d20 6835 6164 5f66 696c 653a 2050  ram h5ad_file: P
-00001a60: 6174 6820 746f 202e 6835 6164 2066 696c  ath to .h5ad fil
-00001a70: 6520 7072 6f64 7563 6564 2062 7920 7363  e produced by sc
-00001a80: 616e 7079 2c20 416e 6e44 6174 612c 206f  anpy, AnnData, o
-00001a90: 7220 634e 4d46 2d53 4e53 0d0a 2020 2020  r cNMF-SNS..    
-00001aa0: 2020 2020 3a74 7970 6520 6835 6164 5f66      :type h5ad_f
-00001ab0: 696c 653a 2073 7472 0d0a 2020 2020 2020  ile: str..      
-00001ac0: 2020 3a70 6172 616d 2070 6174 6965 6e74    :param patient
-00001ad0: 5f69 645f 636f 6c3a 204e 616d 6520 6f66  _id_col: Name of
-00001ae0: 206d 6574 6164 6174 6120 6c61 7965 7220   metadata layer 
-00001af0: 7769 7468 2070 6174 6965 6e74 2049 4420  with patient ID 
-00001b00: 696e 666f 726d 6174 696f 6e2c 2064 6566  information, def
-00001b10: 6175 6c74 7320 746f 204e 6f6e 650d 0a20  aults to None.. 
-00001b20: 2020 2020 2020 203a 7479 7065 2070 6174         :type pat
-00001b30: 6965 6e74 5f69 645f 636f 6c3a 2073 7472  ient_id_col: str
-00001b40: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-00001b50: 2020 2020 3a70 6172 616d 2066 6f72 6365      :param force
-00001b60: 5f6d 6967 7261 7465 3a20 666f 7263 6573  _migrate: forces
-00001b70: 2063 6f6e 7665 7273 696f 6e20 6f66 2041   conversion of A
-00001b80: 6e6e 4461 7461 206f 626a 6563 7473 2065  nnData objects e
-00001b90: 7665 6e20 7768 656e 2061 6461 7461 2e58  ven when adata.X
-00001ba0: 2061 6e64 2061 6461 7461 2e72 6177 2e58   and adata.raw.X
-00001bb0: 2061 7265 206e 6f74 206c 696e 6561 726c   are not linearl
-00001bc0: 7920 7363 616c 6564 2072 656c 6174 6976  y scaled relativ
-00001bd0: 6520 746f 2065 6163 6820 6f74 6865 722c  e to each other,
-00001be0: 2064 6566 6175 6c74 7320 746f 2046 616c   defaults to Fal
-00001bf0: 7365 0d0a 2020 2020 2020 2020 3a74 7970  se..        :typ
-00001c00: 6520 666f 7263 655f 6d69 6772 6174 653a  e force_migrate:
-00001c10: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
-00001c20: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00001c30: 6261 636b 6564 3a20 5573 6520 6261 636b  backed: Use back
-00001c40: 6564 206d 6f64 6520 746f 206f 7065 6e20  ed mode to open 
-00001c50: 6835 6164 2066 696c 652e 2054 6869 7320  h5ad file. This 
-00001c60: 6361 6e20 7361 7665 206d 656d 6f72 7920  can save memory 
-00001c70: 7768 656e 2074 6865 2064 6174 6173 6574  when the dataset
-00001c80: 2069 7320 7665 7279 206c 6172 6765 2c20   is very large, 
-00001c90: 6275 7420 6973 206e 6f74 2063 6f6d 7061  but is not compa
-00001ca0: 7469 626c 6520 7769 7468 2068 3561 6420  tible with h5ad 
-00001cb0: 6669 6c65 7320 7072 6f64 7563 6564 206f  files produced o
-00001cc0: 7574 7369 6465 206f 6620 634e 4d46 2d53  utside of cNMF-S
-00001cd0: 4e53 2c20 6465 6661 756c 7473 2074 6f20  NS, defaults to 
-00001ce0: 4661 6c73 650d 0a20 2020 2020 2020 203a  False..        :
-00001cf0: 7479 7065 2062 6163 6b65 643a 2062 6f6f  type backed: boo
-00001d00: 6c2c 206f 7074 696f 6e61 6c0d 0a20 2020  l, optional..   
-00001d10: 2020 2020 203a 7265 7475 726e 3a20 4f62       :return: Ob
-00001d20: 6a65 6374 2077 6974 6820 6578 7072 6573  ject with expres
-00001d30: 7369 6f6e 2061 6e64 206d 6574 6164 6174  sion and metadat
-00001d40: 610d 0a20 2020 2020 2020 203a 7274 7970  a..        :rtyp
-00001d50: 653a 203a 636c 6173 733a 607e 636e 6d66  e: :class:`~cnmf
-00001d60: 736e 732e 6461 7461 7365 742e 4461 7461  sns.dataset.Data
-00001d70: 7365 7460 0d0a 2020 2020 2020 2020 2222  set`..        ""
-00001d80: 220d 0a20 2020 2020 2020 2061 6461 7461  "..        adata
-00001d90: 203d 2061 642e 7265 6164 5f68 3561 6428   = ad.read_h5ad(
-00001da0: 6835 6164 5f66 696c 652c 2062 6163 6b65  h5ad_file, backe
-00001db0: 643d 6261 636b 6564 290d 0a20 2020 2020  d=backed)..     
-00001dc0: 2020 2064 6174 6173 6574 203d 2044 6174     dataset = Dat
-00001dd0: 6173 6574 2861 6461 7461 3d61 6461 7461  aset(adata=adata
-00001de0: 2c20 7061 7469 656e 745f 6964 5f63 6f6c  , patient_id_col
-00001df0: 3d70 6174 6965 6e74 5f69 645f 636f 6c2c  =patient_id_col,
-00001e00: 2066 6f72 6365 5f6d 6967 7261 7465 3d66   force_migrate=f
-00001e10: 6f72 6365 5f6d 6967 7261 7465 290d 0a20  orce_migrate).. 
-00001e20: 2020 2020 2020 2072 6574 7572 6e20 6461         return da
-00001e30: 7461 7365 740d 0a20 2020 200d 0a20 2020  taset..    ..   
-00001e40: 2040 7072 6f70 6572 7479 0d0a 2020 2020   @property..    
-00001e50: 6465 6620 6973 5f6e 6f72 6d61 6c69 7a65  def is_normalize
-00001e60: 6428 7365 6c66 293a 0d0a 2020 2020 2020  d(self):..      
-00001e70: 2020 2222 224f 7574 7075 7473 2074 6865    """Outputs the
-00001e80: 206e 6f72 6d61 6c69 7a61 7469 6f6e 2073   normalization s
-00001e90: 7461 7475 7320 6f66 2074 6865 2064 6174  tatus of the dat
-00001ea0: 6173 6574 2e0d 0a0d 0a20 2020 2020 2020  aset.....       
-00001eb0: 203a 7265 7475 726e 3a20 5472 7565 2069   :return: True i
-00001ec0: 6620 6461 7461 7365 7420 636f 6e74 6169  f dataset contai
-00001ed0: 6e73 206e 6f72 6d61 6c69 7a65 6420 6461  ns normalized da
-00001ee0: 7461 2c20 4661 6c73 6520 6966 2069 7420  ta, False if it 
-00001ef0: 6973 2072 6177 2064 6174 612e 0d0a 2020  is raw data...  
-00001f00: 2020 2020 2020 3a72 7479 7065 3a20 626f        :rtype: bo
-00001f10: 6f6c 0d0a 2020 2020 2020 2020 2222 220d  ol..        """.
-00001f20: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00001f30: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
-00001f40: 6973 5f6e 6f72 6d61 6c69 7a65 6422 5d0d  is_normalized"].
-00001f50: 0a20 2020 200d 0a20 2020 2040 6973 5f6e  .    ..    @is_n
-00001f60: 6f72 6d61 6c69 7a65 642e 7365 7474 6572  ormalized.setter
-00001f70: 0d0a 2020 2020 6465 6620 6973 5f6e 6f72  ..    def is_nor
-00001f80: 6d61 6c69 7a65 6428 7365 6c66 2c20 7661  malized(self, va
-00001f90: 6c75 653a 2062 6f6f 6c29 3a0d 0a20 2020  lue: bool):..   
-00001fa0: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00001fb0: 756e 735b 2269 735f 6e6f 726d 616c 697a  uns["is_normaliz
-00001fc0: 6564 225d 203d 2076 616c 7565 0d0a 2020  ed"] = value..  
-00001fd0: 2020 2020 2020 0d0a 2020 2020 4070 726f        ..    @pro
-00001fe0: 7065 7274 790d 0a20 2020 2064 6566 2063  perty..    def c
-00001ff0: 6e6d 6673 6e73 5f76 6572 7369 6f6e 2873  nmfsns_version(s
-00002000: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
-00002010: 2222 634e 4d46 2d53 4e53 2076 6572 7369  ""cNMF-SNS versi
-00002020: 6f6e 2075 7365 6420 746f 2063 7265 6174  on used to creat
-00002030: 6520 7468 6520 6461 7461 7365 740d 0a0d  e the dataset...
-00002040: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00002050: 3a20 7665 7273 696f 6e0d 0a20 2020 2020  : version..     
-00002060: 2020 203a 7274 7970 653a 2073 7472 0d0a     :rtype: str..
-00002070: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00002080: 2020 2020 2069 6620 2263 6e6d 6673 6e73       if "cnmfsns
-00002090: 5f76 6572 7369 6f6e 2220 696e 2073 656c  _version" in sel
-000020a0: 662e 6164 6174 612e 756e 733a 0d0a 2020  f.adata.uns:..  
-000020b0: 2020 2020 2020 2020 2020 7665 7273 696f            versio
-000020c0: 6e20 3d20 7365 6c66 2e61 6461 7461 2e75  n = self.adata.u
-000020d0: 6e73 5b22 636e 6d66 736e 735f 7665 7273  ns["cnmfsns_vers
-000020e0: 696f 6e22 5d0d 0a20 2020 2020 2020 2065  ion"]..        e
-000020f0: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
-00002100: 2020 7665 7273 696f 6e20 3d20 4e6f 6e65    version = None
-00002110: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002120: 2076 6572 7369 6f6e 0d0a 2020 2020 2020   version..      
-00002130: 2020 0d0a 2020 2020 4070 726f 7065 7274    ..    @propert
-00002140: 790d 0a20 2020 2064 6566 2068 6173 5f63  y..    def has_c
-00002150: 6e6d 665f 7265 7375 6c74 7328 7365 6c66  nmf_results(self
-00002160: 293a 0d0a 2020 2020 2020 2020 2222 2254  ):..        """T
-00002170: 6573 7420 666f 7220 7765 6874 6865 7220  est for wehther 
-00002180: 4461 7461 7365 7420 636f 6e74 6169 6e73  Dataset contains
-00002190: 2063 4e4d 4620 7265 7375 6c74 7320 666f   cNMF results fo
-000021a0: 7220 7468 6520 6461 7461 7365 740d 0a0d  r the dataset...
-000021b0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000021c0: 3a20 5768 6574 6865 7220 636f 6d70 6c65  : Whether comple
-000021d0: 7465 2063 4e4d 4620 7265 7375 6c74 7320  te cNMF results 
-000021e0: 6172 6520 636f 6e74 6169 6e65 6420 666f  are contained fo
-000021f0: 7220 6174 206c 6561 7374 2031 2072 616e  r at least 1 ran
-00002200: 6b20 286b 290d 0a20 2020 2020 2020 203a  k (k)..        :
-00002210: 7274 7970 653a 2062 6f6f 6c0d 0a20 2020  rtype: bool..   
-00002220: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00002230: 2020 6d61 7472 6978 5f63 6865 636b 7320    matrix_checks 
-00002240: 3d20 5b0d 0a20 2020 2020 2020 2020 2020  = [..           
-00002250: 2022 636e 6d66 5f75 7361 6765 2220 696e   "cnmf_usage" in
-00002260: 2073 656c 662e 6164 6174 612e 6f62 736d   self.adata.obsm
-00002270: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
-00002280: 636e 6d66 5f67 6570 5f73 636f 7265 2220  cnmf_gep_score" 
-00002290: 696e 2073 656c 662e 6164 6174 612e 7661  in self.adata.va
-000022a0: 726d 2c0d 0a20 2020 2020 2020 2020 2020  rm,..           
-000022b0: 2022 636e 6d66 5f67 6570 5f74 706d 2220   "cnmf_gep_tpm" 
-000022c0: 696e 2073 656c 662e 6164 6174 612e 7661  in self.adata.va
-000022d0: 726d 2c0d 0a20 2020 2020 2020 2020 2020  rm,..           
-000022e0: 2022 636e 6d66 5f67 6570 5f72 6177 2220   "cnmf_gep_raw" 
-000022f0: 696e 2073 656c 662e 6164 6174 612e 7661  in self.adata.va
-00002300: 726d 2c0d 0a20 2020 2020 2020 2020 2020  rm,..           
-00002310: 2022 6b76 616c 7322 2069 6e20 7365 6c66   "kvals" in self
-00002320: 2e61 6461 7461 2e75 6e73 0d0a 2020 2020  .adata.uns..    
-00002330: 2020 2020 5d0d 0a20 2020 2020 2020 2072      ]..        r
-00002340: 6574 7572 6e20 616c 6c28 6d61 7472 6978  eturn all(matrix
-00002350: 5f63 6865 636b 7329 0d0a 2020 2020 2020  _checks)..      
-00002360: 2020 0d0a 2020 2020 4070 726f 7065 7274    ..    @propert
-00002370: 790d 0a20 2020 2064 6566 206f 7665 7264  y..    def overd
-00002380: 6973 7065 7273 6564 5f67 656e 6573 2873  ispersed_genes(s
-00002390: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
-000023a0: 2222 4f76 6572 6469 7370 6572 7365 6420  ""Overdispersed 
-000023b0: 6765 6e65 206c 6973 7420 7573 6564 2066  gene list used f
-000023c0: 6f72 2063 4e4d 460d 0a0d 0a20 2020 2020  or cNMF....     
-000023d0: 2020 203a 7265 7475 726e 3a20 6765 6e65     :return: gene
-000023e0: 206c 6973 740d 0a20 2020 2020 2020 203a   list..        :
-000023f0: 7274 7970 653a 206c 6973 740d 0a20 2020  rtype: list..   
-00002400: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00002410: 2020 7265 7475 726e 2073 656c 662e 6164    return self.ad
-00002420: 6174 612e 756e 735b 2267 656e 655f 6c69  ata.uns["gene_li
-00002430: 7374 225d 0d0a 0d0a 0d0a 2020 2020 4063  st"]......    @c
-00002440: 6e6d 6673 6e73 5f76 6572 7369 6f6e 2e73  nmfsns_version.s
-00002450: 6574 7465 720d 0a20 2020 2064 6566 2063  etter..    def c
-00002460: 6e6d 6673 6e73 5f76 6572 7369 6f6e 2873  nmfsns_version(s
-00002470: 656c 662c 2076 616c 7565 3a20 626f 6f6c  elf, value: bool
-00002480: 293a 0d0a 2020 2020 2020 2020 7365 6c66  ):..        self
-00002490: 2e61 6461 7461 2e75 6e73 5b22 636e 6d66  .adata.uns["cnmf
-000024a0: 736e 735f 7665 7273 696f 6e22 5d20 3d20  sns_version"] = 
-000024b0: 7661 6c75 650d 0a0d 0a20 2020 2020 2020  value....       
-000024c0: 200d 0a20 2020 2064 6566 2075 7064 6174   ..    def updat
-000024d0: 655f 6f62 7328 7365 6c66 2c20 6f62 7329  e_obs(self, obs)
-000024e0: 3a0d 0a20 2020 2020 2020 2022 2222 5570  :..        """Up
-000024f0: 6461 7465 2074 6865 206f 6273 6572 7661  date the observa
-00002500: 7469 6f6e 206d 6574 6164 6174 6120 7769  tion metadata wi
-00002510: 7468 2061 206e 6577 206d 6574 6164 6174  th a new metadat
-00002520: 6120 6d61 7472 6978 0d0a 0d0a 2020 2020  a matrix....    
-00002530: 2020 2020 3a70 6172 616d 206f 6273 3a20      :param obs: 
-00002540: 416e 206f 6273 6572 7661 7469 6f6e 7320  An observations 
-00002550: c397 206d 6574 6164 6174 6120 6d61 7472  .. metadata matr
-00002560: 6978 2c20 6465 6661 756c 7473 2074 6f20  ix, defaults to 
-00002570: 4e6f 6e65 0d0a 2020 2020 2020 2020 3a74  None..        :t
-00002580: 7970 6520 6f62 733a 2060 7064 2e44 6174  ype obs: `pd.Dat
-00002590: 6146 7261 6d65 602c 206f 7074 696f 6e61  aFrame`, optiona
-000025a0: 6c0d 0a20 2020 2020 2020 2022 2222 0d0a  l..        """..
-000025b0: 2020 2020 2020 2020 2320 636f 6e76 6572          # conver
-000025c0: 7420 276f 626a 6563 7427 2064 7479 7065  t 'object' dtype
-000025d0: 2074 6f20 6361 7465 676f 7269 6361 6c2c   to categorical,
-000025e0: 2063 6f6e 7665 7274 696e 6720 626f 6f6c   converting bool
-000025f0: 2076 616c 7565 7320 746f 2073 7472 696e   values to strin
-00002600: 6773 2061 7320 7468 6573 6520 6172 6520  gs as these are 
-00002610: 6e6f 7420 7375 7070 6f72 7465 6420 6279  not supported by
-00002620: 2041 6e6e 4461 7461 206f 6e2d 6469 736b   AnnData on-disk
-00002630: 2066 6f72 6d61 740d 0a20 2020 2020 2020   format..       
-00002640: 2066 6f72 2063 6f6c 2069 6e20 6f62 732e   for col in obs.
-00002650: 7365 6c65 6374 5f64 7479 7065 7328 696e  select_dtypes(in
-00002660: 636c 7564 653d 226f 626a 6563 7422 292e  clude="object").
-00002670: 636f 6c75 6d6e 733a 0d0a 2020 2020 2020  columns:..      
-00002680: 2020 2020 2020 6f62 735b 636f 6c5d 203d        obs[col] =
-00002690: 206f 6273 5b63 6f6c 5d2e 7265 706c 6163   obs[col].replac
-000026a0: 6528 7b54 7275 653a 2022 5472 7565 222c  e({True: "True",
-000026b0: 2046 616c 7365 3a20 2246 616c 7365 227d   False: "False"}
-000026c0: 292e 6173 7479 7065 2822 6361 7465 676f  ).astype("catego
-000026d0: 7279 2229 0d0a 2020 2020 2020 2020 6d69  ry")..        mi
-000026e0: 7373 696e 675f 7361 6d70 6c65 735f 696e  ssing_samples_in
-000026f0: 5f58 203d 206f 6273 2e69 6e64 6578 2e64  _X = obs.index.d
-00002700: 6966 6665 7265 6e63 6528 7365 6c66 2e61  ifference(self.a
-00002710: 6461 7461 2e6f 6273 2e69 6e64 6578 292e  data.obs.index).
-00002720: 6173 7479 7065 2873 7472 292e 746f 5f6c  astype(str).to_l
-00002730: 6973 7428 290d 0a20 2020 2020 2020 2069  ist()..        i
-00002740: 6620 6d69 7373 696e 675f 7361 6d70 6c65  f missing_sample
-00002750: 735f 696e 5f58 3a0d 0a20 2020 2020 2020  s_in_X:..       
-00002760: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
-00002770: 6e69 6e67 2822 5468 6520 666f 6c6c 6f77  ning("The follow
-00002780: 696e 6720 7361 6d70 6c65 7320 696e 2074  ing samples in t
-00002790: 6865 206d 6574 6164 6174 6120 7765 7265  he metadata were
-000027a0: 206e 6f74 2070 7265 7365 6e74 2069 6e20   not present in 
-000027b0: 7468 6520 6461 7461 2028 6061 6461 7461  the data (`adata
-000027c0: 2e58 6029 3a5c 6e20 202d 2022 202b 2022  .X`):\n  - " + "
-000027d0: 5c6e 2020 2d20 222e 6a6f 696e 286d 6973  \n  - ".join(mis
-000027e0: 7369 6e67 5f73 616d 706c 6573 5f69 6e5f  sing_samples_in_
-000027f0: 5829 290d 0a20 2020 2020 2020 206d 6973  X))..        mis
-00002800: 7369 6e67 5f73 616d 706c 6573 5f69 6e5f  sing_samples_in_
-00002810: 6d64 203d 2073 656c 662e 6164 6174 612e  md = self.adata.
-00002820: 6f62 732e 696e 6465 782e 6469 6666 6572  obs.index.differ
-00002830: 656e 6365 286f 6273 2e69 6e64 6578 292e  ence(obs.index).
-00002840: 6173 7479 7065 2873 7472 292e 746f 5f6c  astype(str).to_l
-00002850: 6973 7428 290d 0a20 2020 2020 2020 2069  ist()..        i
-00002860: 6620 6d69 7373 696e 675f 7361 6d70 6c65  f missing_sample
-00002870: 735f 696e 5f6d 643a 0d0a 2020 2020 2020  s_in_md:..      
-00002880: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
-00002890: 726e 696e 6728 2254 6865 2066 6f6c 6c6f  rning("The follo
-000028a0: 7769 6e67 2073 616d 706c 6573 2069 6e20  wing samples in 
-000028b0: 7468 6520 6461 7461 2028 6061 6461 7461  the data (`adata
-000028c0: 2e58 6029 2077 6572 6520 6162 7365 6e74  .X`) were absent
-000028d0: 2069 6e20 7468 6520 6d65 7461 6461 7461   in the metadata
-000028e0: 3a5c 6e20 202d 2022 202b 2022 5c6e 2020  :\n  - " + "\n  
-000028f0: 2d20 222e 6a6f 696e 286d 6973 7369 6e67  - ".join(missing
-00002900: 5f73 616d 706c 6573 5f69 6e5f 6d64 2929  _samples_in_md))
-00002910: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-00002920: 6461 7461 2e6f 6273 203d 206f 6273 2e72  data.obs = obs.r
-00002930: 6569 6e64 6578 2873 656c 662e 6164 6174  eindex(self.adat
-00002940: 612e 6f62 732e 696e 6465 7829 0d0a 2020  a.obs.index)..  
-00002950: 2020 0d0a 2020 2020 6465 6620 6765 745f    ..    def get_
-00002960: 6d65 7461 6461 7461 5f74 7970 655f 7375  metadata_type_su
-00002970: 6d6d 6172 7928 7365 6c66 293a 0d0a 2020  mmary(self):..  
-00002980: 2020 2020 2020 2222 2252 6574 7572 6e20        """Return 
-00002990: 6120 7072 696e 7461 626c 6520 7375 6d6d  a printable summ
-000029a0: 6172 7920 6f66 206d 6574 6164 6174 6120  ary of metadata 
-000029b0: 616e 6420 7661 6c75 6520 7479 7065 7320  and value types 
-000029c0: 666f 7220 6561 6368 206d 6574 6164 6174  for each metadat
-000029d0: 6120 6c61 7965 722e 0d0a 0d0a 2020 2020  a layer.....    
-000029e0: 2020 2020 3a72 6574 7572 6e3a 2053 756d      :return: Sum
-000029f0: 6d61 7279 206f 6620 6d65 7461 6461 7461  mary of metadata
-00002a00: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00002a10: 3a20 7374 720d 0a20 2020 2020 2020 2022  : str..        "
-00002a20: 2222 0d0a 2020 2020 2020 2020 6d73 6720  ""..        msg 
-00002a30: 3d20 2222 0d0a 2020 2020 2020 2020 666f  = ""..        fo
-00002a40: 7220 636f 6c20 696e 2073 656c 662e 6164  r col in self.ad
-00002a50: 6174 612e 6f62 732e 636f 6c75 6d6e 733a  ata.obs.columns:
-00002a60: 0d0a 2020 2020 2020 2020 2020 2020 6d73  ..            ms
-00002a70: 6720 2b3d 2022 2020 2020 436f 6c75 6d6e  g += "    Column
-00002a80: 3a20 2220 2b20 636f 6c20 2b20 225c 6e22  : " + col + "\n"
-00002a90: 0d0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
-00002aa0: 7220 7661 6c75 655f 7479 7065 2c20 636f  r value_type, co
-00002ab0: 756e 7420 696e 2073 656c 662e 6164 6174  unt in self.adat
-00002ac0: 612e 6f62 735b 636f 6c5d 2e64 726f 706e  a.obs[col].dropn
-00002ad0: 6128 292e 6d61 7028 7479 7065 292e 7661  a().map(type).va
-00002ae0: 6c75 655f 636f 756e 7473 2829 2e69 7465  lue_counts().ite
-00002af0: 6d73 2829 3a0d 0a20 2020 2020 2020 2020  ms():..         
-00002b00: 2020 2020 2020 206d 7367 202b 3d20 6622         msg += f"
-00002b10: 2020 2020 2020 2020 7b76 616c 7565 5f74          {value_t
-00002b20: 7970 657d 3a20 7b63 6f75 6e74 7d5c 6e22  ype}: {count}\n"
-00002b30: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-00002b40: 206d 7367 0d0a 2020 2020 0d0a 2020 2020   msg..    ..    
-00002b50: 6465 6620 7772 6974 655f 6835 6164 2873  def write_h5ad(s
-00002b60: 656c 662c 2066 696c 656e 616d 6529 3a0d  elf, filename):.
-00002b70: 0a20 2020 2020 2020 2022 2222 5772 6974  .        """Writ
-00002b80: 6520 6461 7461 7365 7420 746f 202e 6835  e dataset to .h5
-00002b90: 6164 2066 696c 652e 0d0a 0d0a 2020 2020  ad file.....    
-00002ba0: 2020 2020 3a70 6172 616d 2066 696c 656e      :param filen
-00002bb0: 616d 653a 2066 696c 6570 6174 680d 0a20  ame: filepath.. 
-00002bc0: 2020 2020 2020 203a 7479 7065 2066 696c         :type fil
-00002bd0: 656e 616d 653a 2073 7472 0d0a 2020 2020  ename: str..    
-00002be0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00002bf0: 2066 696c 656e 616d 6520 3d20 6f73 2e70   filename = os.p
-00002c00: 6174 682e 6162 7370 6174 6828 6669 6c65  ath.abspath(file
-00002c10: 6e61 6d65 290d 0a20 2020 2020 2020 206c  name)..        l
-00002c20: 6f67 6769 6e67 2e69 6e66 6f28 6622 5772  ogging.info(f"Wr
-00002c30: 6974 696e 6720 746f 207b 6669 6c65 6e61  iting to {filena
-00002c40: 6d65 7d22 290d 0a20 2020 2020 2020 2073  me}")..        s
-00002c50: 656c 662e 6164 6174 612e 7772 6974 655f  elf.adata.write_
-00002c60: 6835 6164 2866 696c 656e 616d 6529 0d0a  h5ad(filename)..
-00002c70: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
-00002c80: 696e 666f 2866 2244 6f6e 6522 290d 0a20  info(f"Done").. 
-00002c90: 2020 200d 0a20 2020 2064 6566 2074 6f5f     ..    def to_
-00002ca0: 6466 2873 656c 662c 206e 6f72 6d61 6c69  df(self, normali
-00002cb0: 7a65 643d 4661 6c73 6529 3a0d 0a20 2020  zed=False):..   
-00002cc0: 2020 2020 2022 2222 4765 7420 6461 7461       """Get data
-00002cd0: 206d 6174 7269 7820 6173 2061 2060 7064   matrix as a `pd
-00002ce0: 2e44 6174 6146 7261 6d65 600d 0a0d 0a20  .DataFrame`.... 
-00002cf0: 2020 2020 2020 203a 7061 7261 6d20 6e6f         :param no
-00002d00: 726d 616c 697a 6564 3a20 5365 7420 7472  rmalized: Set tr
-00002d10: 7565 2066 6f72 2054 504d 206e 6f72 6d61  ue for TPM norma
-00002d20: 6c69 7a65 6420 6f75 7470 7574 2c20 6465  lized output, de
-00002d30: 6661 756c 7473 2074 6f20 4661 6c73 650d  faults to False.
-00002d40: 0a20 2020 2020 2020 203a 7479 7065 206e  .        :type n
-00002d50: 6f72 6d61 6c69 7a65 643a 2062 6f6f 6c2c  ormalized: bool,
-00002d60: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00002d70: 2020 203a 7265 7475 726e 3a20 6f62 7365     :return: obse
-00002d80: 7276 6174 696f 6e73 20c3 9720 7661 7269  rvations .. vari
-00002d90: 6162 6c65 7320 6461 7461 206d 6174 7269  ables data matri
-00002da0: 780d 0a20 2020 2020 2020 203a 7274 7970  x..        :rtyp
-00002db0: 653a 2070 642e 4461 7461 4672 616d 650d  e: pd.DataFrame.
-00002dc0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00002dd0: 2020 2020 2020 6466 203d 2073 656c 662e        df = self.
-00002de0: 6164 6174 612e 746f 5f64 6628 290d 0a20  adata.to_df().. 
-00002df0: 2020 2020 2020 2069 6620 6e6f 726d 616c         if normal
-00002e00: 697a 6564 2061 6e64 206e 6f74 2073 656c  ized and not sel
-00002e10: 662e 6973 5f6e 6f72 6d61 6c69 7a65 643a  f.is_normalized:
-00002e20: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
-00002e30: 203d 2064 662e 6469 7628 6466 2e73 756d   = df.div(df.sum
-00002e40: 2861 7869 733d 3129 2c20 6178 6973 3d30  (axis=1), axis=0
-00002e50: 2920 2a20 3165 3620 2023 2054 504d 206e  ) * 1e6  # TPM n
-00002e60: 6f72 6d61 6c69 7a61 7469 6f6e 0d0a 2020  ormalization..  
-00002e70: 2020 2020 2020 7265 7475 726e 2064 660d        return df.
-00002e80: 0a20 2020 2020 2020 200d 0a20 2020 2064  .        ..    d
-00002e90: 6566 2072 656d 6f76 655f 756e 6661 6374  ef remove_unfact
-00002ea0: 6f72 697a 6162 6c65 5f67 656e 6573 2873  orizable_genes(s
-00002eb0: 656c 6629 3a0d 0a20 2020 2020 2020 2022  elf):..        "
-00002ec0: 2222 5265 6d6f 7665 7320 6765 6e65 7320  ""Removes genes 
-00002ed0: 7769 7468 206d 6973 7369 6e67 2076 616c  with missing val
-00002ee0: 7565 7320 6f72 207a 6572 6f20 7661 7269  ues or zero vari
-00002ef0: 616e 6365 2066 726f 6d20 7468 6520 6461  ance from the da
-00002f00: 7461 206d 6174 7269 782e 0d0a 2020 2020  ta matrix...    
-00002f10: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00002f20: 2064 6620 3d20 7365 6c66 2e74 6f5f 6466   df = self.to_df
-00002f30: 286e 6f72 6d61 6c69 7a65 643d 4661 6c73  (normalized=Fals
-00002f40: 6529 0d0a 2020 2020 2020 2020 2320 4368  e)..        # Ch
-00002f50: 6563 6b20 666f 7220 7661 7269 6162 6c65  eck for variable
-00002f60: 7320 7769 7468 206d 6973 7369 6e67 2076  s with missing v
-00002f70: 616c 7565 730d 0a20 2020 2020 2020 2067  alues..        g
-00002f80: 656e 6573 5f77 6974 685f 6d69 7373 696e  enes_with_missin
-00002f90: 6776 616c 7565 7320 3d20 6466 2e69 736e  gvalues = df.isn
-00002fa0: 756c 6c28 292e 616e 7928 290d 0a20 2020  ull().any()..   
-00002fb0: 2020 2020 200d 0a20 2020 2020 2020 2069       ..        i
-00002fc0: 6620 6765 6e65 735f 7769 7468 5f6d 6973  f genes_with_mis
-00002fd0: 7369 6e67 7661 6c75 6573 2e61 6e79 2829  singvalues.any()
-00002fe0: 3a0d 0a20 2020 2020 2020 2020 2020 206e  :..            n
-00002ff0: 5f6d 6973 7369 6e67 203d 2067 656e 6573  _missing = genes
-00003000: 5f77 6974 685f 6d69 7373 696e 6776 616c  _with_missingval
-00003010: 7565 732e 7375 6d28 290d 0a20 2020 2020  ues.sum()..     
-00003020: 2020 2020 2020 206c 6f67 6769 6e67 2e77         logging.w
-00003030: 6172 6e69 6e67 2866 227b 6e5f 6d69 7373  arning(f"{n_miss
-00003040: 696e 677d 206f 6620 7b73 656c 662e 6164  ing} of {self.ad
-00003050: 6174 612e 6e5f 7661 7273 7d20 7661 7269  ata.n_vars} vari
-00003060: 6162 6c65 7320 6172 6520 6d69 7373 696e  ables are missin
-00003070: 6720 7661 6c75 6573 2028 6061 6461 7461  g values (`adata
-00003080: 2e58 6029 2e22 290d 0a20 2020 2020 2020  .X`).")..       
-00003090: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
-000030a0: 6e69 6e67 2866 2253 7562 7365 7474 696e  ning(f"Subsettin
-000030b0: 6720 7661 7269 6162 6c65 7320 746f 2074  g variables to t
-000030c0: 686f 7365 2077 6974 6820 6e6f 206d 6973  hose with no mis
-000030d0: 7369 6e67 2076 616c 7565 732e 2229 0d0a  sing values.")..
-000030e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000030f0: 0d0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
-00003100: 6b20 666f 7220 6765 6e65 7320 7769 7468  k for genes with
-00003110: 207a 6572 6f20 7661 7269 616e 6365 0d0a   zero variance..
-00003120: 2020 2020 2020 2020 7a65 726f 7661 7267          zerovarg
-00003130: 656e 6573 203d 2028 6466 2e76 6172 2829  enes = (df.var()
-00003140: 203d 3d20 3029 0d0a 2020 2020 2020 2020   == 0)..        
-00003150: 6966 207a 6572 6f76 6172 6765 6e65 732e  if zerovargenes.
-00003160: 616e 7928 293a 0d0a 2020 2020 2020 2020  any():..        
-00003170: 2020 2020 6e5f 7a65 726f 7661 7220 3d20      n_zerovar = 
-00003180: 7a65 726f 7661 7267 656e 6573 2e73 756d  zerovargenes.sum
-00003190: 2829 0d0a 2020 2020 2020 2020 2020 2020  ()..            
-000031a0: 6c6f 6767 696e 672e 7761 726e 696e 6728  logging.warning(
-000031b0: 6622 7b6e 5f7a 6572 6f76 6172 7d20 6f66  f"{n_zerovar} of
-000031c0: 207b 7365 6c66 2e61 6461 7461 2e6e 5f76   {self.adata.n_v
-000031d0: 6172 737d 2076 6172 6961 626c 6573 2068  ars} variables h
-000031e0: 6176 6520 6120 7661 7269 616e 6365 206f  ave a variance o
-000031f0: 6620 7a65 726f 2069 6e20 636f 756e 7473  f zero in counts
-00003200: 2064 6174 6120 2860 6164 6174 612e 7261   data (`adata.ra
-00003210: 772e 5860 292e 2229 0d0a 2020 2020 2020  w.X`).")..      
-00003220: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
-00003230: 726e 696e 6728 6622 5375 6273 6574 7469  rning(f"Subsetti
-00003240: 6e67 2076 6172 6961 626c 6573 2074 6f20  ng variables to 
-00003250: 7468 6f73 6520 7769 7468 206e 6f6e 7a65  those with nonze
-00003260: 726f 2076 6172 6961 6e63 652e 2229 0d0a  ro variance.")..
-00003270: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00003280: 2020 6765 6e65 735f 746f 5f6b 6565 7020    genes_to_keep 
-00003290: 3d20 287e 6765 6e65 735f 7769 7468 5f6d  = (~genes_with_m
-000032a0: 6973 7369 6e67 7661 6c75 6573 2920 2620  issingvalues) & 
-000032b0: 287e 7a65 726f 7661 7267 656e 6573 290d  (~zerovargenes).
-000032c0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000032d0: 2020 2073 656c 662e 6164 6174 6120 3d20     self.adata = 
-000032e0: 7365 6c66 2e61 6461 7461 5b3a 2c67 656e  self.adata[:,gen
-000032f0: 6573 5f74 6f5f 6b65 6570 5d0d 0a0d 0a20  es_to_keep].... 
-00003300: 2020 2064 6566 2063 6f6d 7075 7465 5f67     def compute_g
-00003310: 656e 655f 7374 6174 7328 7365 6c66 2c20  ene_stats(self, 
-00003320: 6f64 675f 6465 6661 756c 745f 7370 6c69  odg_default_spli
-00003330: 6e65 5f64 6567 7265 653a 2069 6e74 203d  ne_degree: int =
-00003340: 2033 2c20 6f64 675f 6465 6661 756c 745f   3, odg_default_
-00003350: 646f 663a 2069 6e74 203d 2038 293a 0d0a  dof: int = 8):..
-00003360: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00003370: 2020 2020 2043 6f6d 7075 7465 7320 6765       Computes ge
-00003380: 6e65 2073 7461 7469 7374 6963 7320 616e  ne statistics an
-00003390: 6420 6669 7473 2074 776f 206d 6f64 656c  d fits two model
-000033a0: 7320 6f66 206d 6561 6e20 616e 6420 7661  s of mean and va
-000033b0: 7269 616e 6365 206f 6620 6765 6e65 7320  riance of genes 
-000033c0: 696e 2074 6865 2064 6174 6173 6574 2e20  in the dataset. 
-000033d0: 5468 6520 6669 7273 7420 6d65 7468 6f64  The first method
-000033e0: 2069 7320 7468 650d 0a20 2020 2020 2020   is the..       
-000033f0: 2067 656e 6572 616c 697a 6564 2061 6464   generalized add
-00003400: 6974 6976 6520 6d6f 6465 6c20 7769 7468  itive model with
-00003410: 2073 6d6f 6f74 6820 636f 6d70 6f6e 656e   smooth componen
-00003420: 7473 2028 422d 7370 6c69 6e65 7329 2074  ts (B-splines) t
-00003430: 6f20 6d6f 6465 6c20 7468 6520 7265 6c61  o model the rela
-00003440: 7469 6f6e 7368 6970 206f 6620 6d65 616e  tionship of mean
-00003450: 2061 6e64 2076 6172 6961 6e63 650d 0a20   and variance.. 
-00003460: 2020 2020 2020 2062 6574 7765 656e 2067         between g
-00003470: 656e 6573 2069 6e20 7468 6520 6461 7461  enes in the data
-00003480: 7365 742e 2049 7420 7072 6f64 7563 6573  set. It produces
-00003490: 2061 6e20 6f64 7363 6f72 6520 6d65 7472   an odscore metr
-000034a0: 6963 2066 6f72 206f 7665 7264 6973 7065  ic for overdispe
-000034b0: 7273 696f 6e2e 2054 6865 2073 6563 6f6e  rsion. The secon
-000034c0: 6420 6973 2074 6865 2063 6f75 6e74 2d73  d is the count-s
-000034d0: 7461 7469 7374 6963 730d 0a20 2020 2020  tatistics..     
-000034e0: 2020 206d 6574 686f 6420 666f 756e 6420     method found 
-000034f0: 696e 2074 6865 2063 4e4d 4620 7061 636b  in the cNMF pack
-00003500: 6167 652c 2077 6869 6368 2070 726f 6475  age, which produ
-00003510: 6365 7320 6120 6d6f 6469 6669 6564 2076  ces a modified v
-00003520: 2d73 636f 7265 206d 6574 7269 632e 2041  -score metric. A
-00003530: 6c6c 2067 656e 6520 7374 6174 6973 7469  ll gene statisti
-00003540: 6373 2061 7265 2073 746f 7265 6420 7769  cs are stored wi
-00003550: 7468 696e 2074 6865 0d0a 2020 2020 2020  thin the..      
-00003560: 2020 6461 7461 7365 7420 6f62 6a65 6374    dataset object
-00003570: 2061 6e64 2061 7265 2061 6363 6573 7369   and are accessi
-00003580: 626c 6520 7573 696e 6720 6064 6174 6173  ble using `datas
-00003590: 6574 2e61 6e6e 6461 7461 2e76 6172 602e  et.anndata.var`.
-000035a0: 0d0a 0d0a 2020 2020 2020 2020 3a70 6172  ....        :par
-000035b0: 616d 206f 6467 5f64 6566 6175 6c74 5f73  am odg_default_s
-000035c0: 706c 696e 655f 6465 6772 6565 3a20 422d  pline_degree: B-
-000035d0: 5370 6c69 6e65 2064 6567 7265 6520 666f  Spline degree fo
-000035e0: 7220 474c 4d2d 4741 4d20 6d6f 6465 6c6c  r GLM-GAM modell
-000035f0: 696e 6720 6f66 206d 6561 6e2d 7661 7269  ing of mean-vari
-00003600: 616e 6365 2072 656c 6174 696f 6e73 6869  ance relationshi
-00003610: 702c 2064 6566 6175 6c74 7320 746f 2033  p, defaults to 3
-00003620: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00003630: 6f64 675f 6465 6661 756c 745f 7370 6c69  odg_default_spli
-00003640: 6e65 5f64 6567 7265 653a 2069 6e74 2c20  ne_degree: int, 
-00003650: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
-00003660: 2020 3a70 6172 616d 206f 6467 5f64 6566    :param odg_def
-00003670: 6175 6c74 5f64 6f66 3a20 4465 6772 6565  ault_dof: Degree
-00003680: 7320 6f66 2066 7265 6564 6f6d 2066 6f72  s of freedom for
-00003690: 2047 4c4d 2d47 414d 206d 6f64 656c 6c69   GLM-GAM modelli
-000036a0: 6e67 206f 6620 6d65 616e 2d76 6172 616e  ng of mean-varan
-000036b0: 6365 2c20 6465 6661 756c 7473 2074 6f20  ce, defaults to 
-000036c0: 380d 0a20 2020 2020 2020 203a 7479 7065  8..        :type
-000036d0: 206f 6467 5f64 6566 6175 6c74 5f64 6f66   odg_default_dof
-000036e0: 3a20 696e 742c 206f 7074 696f 6e61 6c0d  : int, optional.
-000036f0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
-00003700: 2020 2020 2020 6461 7461 5f72 6177 203d        data_raw =
-00003710: 2073 656c 662e 746f 5f64 6628 290d 0a20   self.to_df().. 
-00003720: 2020 2020 2020 2064 6174 615f 6e6f 726d         data_norm
-00003730: 616c 697a 6564 203d 2073 656c 662e 746f  alized = self.to
-00003740: 5f64 6628 6e6f 726d 616c 697a 6564 3d54  _df(normalized=T
-00003750: 7275 6529 0d0a 2020 2020 2020 2020 0d0a  rue)..        ..
-00003760: 2020 2020 2020 2020 2320 6372 6561 7465          # create
-00003770: 2064 6174 6166 7261 6d65 206f 6620 7065   dataframe of pe
-00003780: 722d 6765 6e65 2073 7461 7469 7374 6963  r-gene statistic
-00003790: 730d 0a20 2020 2020 2020 2073 656c 662e  s..        self.
-000037a0: 6164 6174 612e 7661 725b 226d 6561 6e22  adata.var["mean"
-000037b0: 5d20 3d20 6461 7461 5f6e 6f72 6d61 6c69  ] = data_normali
-000037c0: 7a65 642e 6d65 616e 2829 0d0a 2020 2020  zed.mean()..    
-000037d0: 2020 2020 7365 6c66 2e61 6461 7461 2e76      self.adata.v
-000037e0: 6172 5b22 7261 6e6b 5f6d 6561 6e22 5d20  ar["rank_mean"] 
-000037f0: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
-00003800: 5b22 6d65 616e 225d 2e72 616e 6b28 290d  ["mean"].rank().
-00003810: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
-00003820: 6174 612e 7661 725b 2276 6172 6961 6e63  ata.var["varianc
-00003830: 6522 5d20 3d20 6461 7461 5f6e 6f72 6d61  e"] = data_norma
-00003840: 6c69 7a65 642e 7661 7228 290d 0a20 2020  lized.var()..   
-00003850: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00003860: 7661 725b 2273 6422 5d20 3d20 6461 7461  var["sd"] = data
-00003870: 5f6e 6f72 6d61 6c69 7a65 642e 7374 6428  _normalized.std(
-00003880: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00003890: 6164 6174 612e 7661 725b 226d 6973 7369  adata.var["missi
-000038a0: 6e67 6e65 7373 225d 203d 2064 6174 615f  ngness"] = data_
-000038b0: 6e6f 726d 616c 697a 6564 2e69 736e 756c  normalized.isnul
-000038c0: 6c28 292e 7375 6d28 2920 2f20 6461 7461  l().sum() / data
-000038d0: 5f6e 6f72 6d61 6c69 7a65 642e 7368 6170  _normalized.shap
-000038e0: 655b 305d 0d0a 2020 2020 2020 2020 7365  e[0]..        se
-000038f0: 6c66 2e61 6461 7461 2e76 6172 5b5b 226c  lf.adata.var[["l
-00003900: 6f67 5f6d 6561 6e22 2c20 226c 6f67 5f76  og_mean", "log_v
-00003910: 6172 6961 6e63 6522 5d5d 203d 206e 702e  ariance"]] = np.
-00003920: 6c6f 6731 3028 7365 6c66 2e61 6461 7461  log10(self.adata
-00003930: 2e76 6172 5b5b 226d 6561 6e22 2c20 2276  .var[["mean", "v
-00003940: 6172 6961 6e63 6522 5d5d 290d 0a20 2020  ariance"]])..   
-00003950: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
-00003960: 7661 725b 226d 6561 6e5f 636f 756e 7473  var["mean_counts
-00003970: 225d 203d 2064 6174 615f 7261 772e 6d65  "] = data_raw.me
-00003980: 616e 2829 0d0a 2020 2020 2020 2020 7365  an()..        se
-00003990: 6c66 2e61 6461 7461 2e76 6172 5b22 6f64  lf.adata.var["od
-000039a0: 7363 6f72 655f 6578 636c 7564 6564 225d  score_excluded"]
-000039b0: 203d 2028 2873 656c 662e 6164 6174 612e   = ((self.adata.
-000039c0: 7661 725b 226d 6973 7369 6e67 6e65 7373  var["missingness
-000039d0: 225d 203e 2030 2920 7c0d 0a20 2020 2020  "] > 0) |..     
-000039e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000660: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
+00000670: 2020 6966 2022 636e 6d66 736e 735f 7665    if "cnmfsns_ve
+00000680: 7273 696f 6e22 2069 6e20 6164 6174 612e  rsion" in adata.
+00000690: 756e 7320 616e 6420 6164 6174 612e 756e  uns and adata.un
+000006a0: 735b 2263 6e6d 6673 6e73 5f76 6572 7369  s["cnmfsns_versi
+000006b0: 6f6e 225d 2069 7320 6e6f 7420 4e6f 6e65  on"] is not None
+000006c0: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
+000006d0: 656c 662e 6164 6174 6120 3d20 6164 6174  elf.adata = adat
+000006e0: 610d 0a20 2020 2020 2020 2065 6c73 653a  a..        else:
+000006f0: 0d0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00000700: 6368 6563 6b20 616e 6420 7570 6461 7465  check and update
+00000710: 206f 6c64 206f 7220 6578 7465 726e 616c   old or external
+00000720: 2068 3561 6420 6669 6c65 7320 666f 7220   h5ad files for 
+00000730: 634e 4d46 2d53 4e53 2063 6f6d 706c 6961  cNMF-SNS complia
+00000740: 6e63 650d 0a20 2020 200d 0a20 2020 2020  nce..    ..     
+00000750: 2020 2020 2020 2058 203d 2061 6461 7461         X = adata
+00000760: 2e74 6f5f 6466 2829 0d0a 2020 2020 2020  .to_df()..      
+00000770: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00000780: 2020 2020 6966 2061 6461 7461 2e69 7362      if adata.isb
+00000790: 6163 6b65 643a 0d0a 2020 2020 2020 2020  acked:..        
+000007a0: 2020 2020 2020 2020 7261 6973 6520 5275          raise Ru
+000007b0: 6e74 696d 6545 7272 6f72 2822 6164 6174  ntimeError("adat
+000007c0: 6120 6973 2061 2062 6163 6b65 6420 416e  a is a backed An
+000007d0: 6e44 6174 6120 6f62 6a65 6374 2e20 416e  nData object. An
+000007e0: 6e44 6174 6120 6f62 6a65 6374 7320 6f70  nData objects op
+000007f0: 656e 6564 2069 6e20 6261 636b 6564 206d  ened in backed m
+00000800: 6f64 6520 6361 6e6e 6f74 2062 6520 6d69  ode cannot be mi
+00000810: 6772 6174 6564 2e22 290d 0a0d 0a20 2020  grated.")....   
+00000820: 2020 2020 2020 2020 2069 6620 6164 6174           if adat
+00000830: 612e 7261 7720 6973 204e 6f6e 653a 0d0a  a.raw is None:..
+00000840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000850: 6973 5f6e 6f72 6d61 6c69 7a65 643d 4661  is_normalized=Fa
+00000860: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+00000870: 2020 2020 2072 6177 203d 2061 6461 7461       raw = adata
+00000880: 2e74 6f5f 6466 2829 0d0a 2020 2020 2020  .to_df()..      
+00000890: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+000008a0: 2020 2020 2020 2020 2020 2020 2072 6177               raw
+000008b0: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
+000008c0: 6164 6174 612e 7261 772e 582c 2069 6e64  adata.raw.X, ind
+000008d0: 6578 3d58 2e69 6e64 6578 2c20 636f 6c75  ex=X.index, colu
+000008e0: 6d6e 733d 582e 636f 6c75 6d6e 7329 0d0a  mns=X.columns)..
+000008f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000900: 636f 7272 6469 7374 203d 2058 2e63 6f72  corrdist = X.cor
+00000910: 7277 6974 6828 7261 772c 2061 7869 733d  rwith(raw, axis=
+00000920: 3129 0d0a 2020 2020 2020 2020 2020 2020  1)..            
+00000930: 2020 2020 2320 6368 6563 6b73 2074 6861      # checks tha
+00000940: 7420 616c 6c20 7361 6d70 6c65 7320 6172  t all samples ar
+00000950: 6520 7065 7266 6563 746c 7920 636f 7272  e perfectly corr
+00000960: 656c 6174 6564 2062 6574 7765 656e 2063  elated between c
+00000970: 6f75 6e74 7320 616e 6420 6e6f 726d 616c  ounts and normal
+00000980: 697a 6564 2064 6174 610d 0a20 2020 2020  ized data..     
+00000990: 2020 2020 2020 2020 2020 2069 6620 2828             if ((
+000009a0: 636f 7272 6469 7374 202d 2031 292e 6162  corrdist - 1).ab
+000009b0: 7328 2920 3e20 3165 2d36 292e 616e 7928  s() > 1e-6).any(
+000009c0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
+000009d0: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+000009e0: 7761 726e 696e 6728 2243 6f75 6e74 7320  warning("Counts 
+000009f0: 616e 6420 6e6f 726d 616c 697a 6564 2065  and normalized e
+00000a00: 7870 7265 7373 696f 6e20 6d61 7472 6963  xpression matric
+00000a10: 6573 2061 7265 206e 6f74 2070 6572 6665  es are not perfe
+00000a20: 6374 6c79 2063 6f72 7265 6c61 7465 642e  ctly correlated.
+00000a30: 2043 6f75 6e74 7320 6461 7461 2077 696c   Counts data wil
+00000a40: 6c20 6265 2072 6574 6169 6e65 6420 696e  l be retained in
+00000a50: 206d 6967 7261 7465 6420 6f62 6a65 6374   migrated object
+00000a60: 2e22 290d 0a20 2020 2020 2020 2020 2020  .")..           
+00000a70: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+00000a80: 666f 7263 655f 6d69 6772 6174 653a 0d0a  force_migrate:..
+00000a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000aa0: 2020 2020 2020 2020 6572 726f 726d 7367          errormsg
+00000ab0: 203d 2022 436f 756c 6420 6e6f 7420 6d69   = "Could not mi
+00000ac0: 6772 6174 6520 416e 6e44 6174 6120 6f62  grate AnnData ob
+00000ad0: 6a65 6374 2e22 0d0a 2020 2020 2020 2020  ject."..        
+00000ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000af0: 6c6f 6767 696e 672e 6572 726f 7228 6572  logging.error(er
+00000b00: 726f 726d 7367 290d 0a20 2020 2020 2020  rormsg)..       
+00000b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000b20: 2072 6169 7365 2056 616c 7565 4572 726f   raise ValueErro
+00000b30: 7228 6572 726f 726d 7367 290d 0a20 2020  r(errormsg)..   
+00000b40: 2020 2020 2020 2020 2020 2020 2023 2063               # c
+00000b50: 6865 636b 2066 6f72 2077 6865 7468 6572  heck for whether
+00000b60: 2075 7365 7220 6f72 6967 696e 616c 6c79   user originally
+00000b70: 2069 6e70 7574 206e 6f72 6d61 6c69 7a65   input normalize
+00000b80: 6420 6f72 2063 6f75 6e74 7320 6461 7461  d or counts data
+00000b90: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000ba0: 2020 6973 5f6e 6f72 6d61 6c69 7a65 6420    is_normalized 
+00000bb0: 3d20 2828 5820 2d20 7261 7729 2e61 6273  = ((X - raw).abs
+00000bc0: 2829 203c 2031 652d 3629 2e61 6c6c 2829  () < 1e-6).all()
+00000bd0: 2e61 6c6c 2829 0d0a 2020 2020 2020 2020  .all()..        
+00000be0: 2020 2020 2020 2020 585f 6973 5f74 706d          X_is_tpm
+00000bf0: 203d 2028 2858 2e73 756d 2861 7869 733d   = ((X.sum(axis=
+00000c00: 3129 202d 2031 6536 292e 6162 7328 2920  1) - 1e6).abs() 
+00000c10: 3e20 3165 3229 2e61 6e79 2829 0d0a 2020  > 1e2).any()..  
+00000c20: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00000c30: 2069 735f 6e6f 726d 616c 697a 6564 2061   is_normalized a
+00000c40: 6e64 206e 6f74 2058 5f69 735f 7470 6d3a  nd not X_is_tpm:
+00000c50: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00000c60: 2020 2020 2020 6c6f 6767 696e 672e 7761        logging.wa
+00000c70: 726e 696e 6728 2241 6e6e 4461 7461 206f  rning("AnnData o
+00000c80: 626a 6563 7420 636f 6e74 6169 6e73 206e  bject contains n
+00000c90: 6f6e 2d54 504d 206e 6f72 6d61 6c69 7a65  on-TPM normalize
+00000ca0: 6420 6461 7461 2e20 4e65 7720 416e 6e44  d data. New AnnD
+00000cb0: 6174 6120 6f62 6a65 6374 2077 696c 6c20  ata object will 
+00000cc0: 7265 7461 696e 2074 6865 2063 6f75 6e74  retain the count
+00000cd0: 2028 756e 6e6f 726d 616c 697a 6564 2920   (unnormalized) 
+00000ce0: 6461 7461 206f 6e6c 792e 2229 0d0a 2020  data only.")..  
+00000cf0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00000d00: 2020 2020 2020 2020 2020 2020 6966 2022              if "
+00000d10: 6f64 6722 2069 6e20 6164 6174 612e 756e  odg" in adata.un
+00000d20: 7320 616e 6420 2267 656e 655f 7374 6174  s and "gene_stat
+00000d30: 7322 2069 6e20 6164 6174 612e 756e 735b  s" in adata.uns[
+00000d40: 226f 6467 225d 3a0d 0a20 2020 2020 2020  "odg"]:..       
+00000d50: 2020 2020 2020 2020 2067 656e 655f 7374           gene_st
+00000d60: 6174 5f63 6f6c 756d 6e73 203d 2061 6461  at_columns = ada
+00000d70: 7461 2e75 6e73 5b22 6f64 6722 5d5b 2267  ta.uns["odg"]["g
+00000d80: 656e 655f 7374 6174 7322 5d2e 636f 6c75  ene_stats"].colu
+00000d90: 6d6e 730d 0a20 2020 2020 2020 2020 2020  mns..           
+00000da0: 2020 2020 2069 6620 6164 6174 612e 7661       if adata.va
+00000db0: 722e 636f 6c75 6d6e 732e 6973 696e 2867  r.columns.isin(g
+00000dc0: 656e 655f 7374 6174 5f63 6f6c 756d 6e73  ene_stat_columns
+00000dd0: 292e 616e 7928 293a 0d0a 2020 2020 2020  ).any():..      
+00000de0: 2020 2020 2020 2020 2020 2020 2020 6f76                ov
+00000df0: 6572 6c61 7070 696e 675f 636f 6c73 203d  erlapping_cols =
+00000e00: 2061 6461 7461 2e76 6172 2e63 6f6c 756d   adata.var.colum
+00000e10: 6e73 2e69 7369 6e28 6765 6e65 5f73 7461  ns.isin(gene_sta
+00000e20: 745f 636f 6c75 6d6e 7329 0d0a 2020 2020  t_columns)..    
+00000e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000e40: 6f76 6572 6c61 7070 696e 675f 636f 6c73  overlapping_cols
+00000e50: 7472 203d 2022 2c20 222e 6a6f 696e 286f  tr = ", ".join(o
+00000e60: 7665 726c 6170 7069 6e67 5f63 6f6c 735b  verlapping_cols[
+00000e70: 6f76 6572 6c61 7070 696e 675f 636f 6c73  overlapping_cols
+00000e80: 5d2e 696e 6465 782e 746f 5f6c 6973 7428  ].index.to_list(
+00000e90: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+00000ea0: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+00000eb0: 7761 726e 696e 6728 6622 416e 6e44 6174  warning(f"AnnDat
+00000ec0: 6120 6f62 6a65 6374 2063 6f6e 7461 696e  a object contain
+00000ed0: 7320 634e 4d46 2067 656e 6520 7374 6174  s cNMF gene stat
+00000ee0: 7320 7768 6963 6820 7769 6c6c 206f 7665  s which will ove
+00000ef0: 7272 6964 6520 636f 6c75 6d6e 7320 696e  rride columns in
+00000f00: 2061 6461 7461 2e76 6172 3a20 7b6f 7665   adata.var: {ove
+00000f10: 726c 6170 7069 6e67 5f63 6f6c 7374 727d  rlapping_colstr}
+00000f20: 2229 0d0a 2020 2020 2020 2020 2020 2020  ")..            
+00000f30: 2020 2020 6164 6174 612e 7661 7220 3d20      adata.var = 
+00000f40: 7064 2e6d 6572 6765 286c 6566 743d 6164  pd.merge(left=ad
+00000f50: 6174 612e 7661 722c 2072 6967 6874 3d61  ata.var, right=a
+00000f60: 6461 7461 2e75 6e73 5b22 6f64 6722 5d5b  data.uns["odg"][
+00000f70: 2267 656e 655f 7374 6174 7322 5d2c 2068  "gene_stats"], h
+00000f80: 6f77 3d22 6c65 6674 222c 206c 6566 745f  ow="left", left_
+00000f90: 696e 6465 783d 5472 7565 2c20 7269 6768  index=True, righ
+00000fa0: 745f 696e 6465 783d 5472 7565 290d 0a20  t_index=True).. 
+00000fb0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00000fc0: 656c 2061 6461 7461 2e75 6e73 5b22 6f64  el adata.uns["od
+00000fd0: 6722 5d5b 2267 656e 655f 7374 6174 7322  g"]["gene_stats"
+00000fe0: 5d0d 0a20 2020 2020 2020 2020 2020 200d  ]..            .
+00000ff0: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+00001000: 7265 6174 6520 6e65 7720 416e 6e44 6174  reate new AnnDat
+00001010: 6120 6f62 6a65 6374 0d0a 2020 2020 2020  a object..      
+00001020: 2020 2020 2020 6e65 775f 6164 6174 6120        new_adata 
+00001030: 3d20 6164 2e41 6e6e 4461 7461 2858 3d72  = ad.AnnData(X=r
+00001040: 6177 2c20 6f62 733d 6164 6174 612e 6f62  aw, obs=adata.ob
+00001050: 732c 2076 6172 3d61 6461 7461 2e76 6172  s, var=adata.var
+00001060: 2c20 7661 726d 3d61 6461 7461 2e76 6172  , varm=adata.var
+00001070: 6d2c 206f 6273 6d3d 6164 6174 612e 6f62  m, obsm=adata.ob
+00001080: 736d 2c20 756e 733d 6164 6174 612e 756e  sm, uns=adata.un
+00001090: 7329 0d0a 2020 2020 2020 2020 2020 2020  s)..            
+000010a0: 6966 2022 6869 7374 6f72 7922 206e 6f74  if "history" not
+000010b0: 2069 6e20 6e65 775f 6164 6174 612e 756e   in new_adata.un
+000010c0: 733a 0d0a 2020 2020 2020 2020 2020 2020  s:..            
+000010d0: 2020 2020 6e65 775f 6164 6174 612e 756e      new_adata.un
+000010e0: 735b 2268 6973 746f 7279 225d 203d 207b  s["history"] = {
+000010f0: 7d0d 0a0d 0a20 2020 2020 2020 2020 2020  }....           
+00001100: 2023 2075 7064 6174 6520 6461 7461 7365   # update datase
+00001110: 7420 6f62 6a65 6374 0d0a 2020 2020 2020  t object..      
+00001120: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+00001130: 203d 206e 6577 5f61 6461 7461 0d0a 2020   = new_adata..  
+00001140: 2020 2020 2020 2020 2020 7365 6c66 2e69            self.i
+00001150: 735f 6e6f 726d 616c 697a 6564 203d 2069  s_normalized = i
+00001160: 735f 6e6f 726d 616c 697a 6564 0d0a 2020  s_normalized..  
+00001170: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00001180: 6e6d 6673 6e73 5f76 6572 7369 6f6e 203d  nmfsns_version =
+00001190: 205f 5f76 6572 7369 6f6e 5f5f 0d0a 2020   __version__..  
+000011a0: 2020 0d0a 2020 2020 4063 6c61 7373 6d65    ..    @classme
+000011b0: 7468 6f64 0d0a 2020 2020 6465 6620 6672  thod..    def fr
+000011c0: 6f6d 5f64 6628 636c 732c 0d0a 2020 2020  om_df(cls,..    
+000011d0: 2020 2020 2020 2020 2020 2020 2020 6461                da
+000011e0: 7461 3a20 7064 2e44 6174 6146 7261 6d65  ta: pd.DataFrame
+000011f0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00001200: 2020 2020 2069 735f 6e6f 726d 616c 697a       is_normaliz
+00001210: 6564 3a20 626f 6f6c 2c0d 0a20 2020 2020  ed: bool,..     
+00001220: 2020 2020 2020 2020 2020 2020 2073 7061               spa
+00001230: 7273 6966 793a 2062 6f6f 6c20 3d20 4661  rsify: bool = Fa
+00001240: 6c73 652c 0d0a 2020 2020 2020 2020 2020  lse,..          
+00001250: 2020 2020 2020 2020 6f62 733a 204f 7074          obs: Opt
+00001260: 696f 6e61 6c5b 7064 2e44 6174 6146 7261  ional[pd.DataFra
+00001270: 6d65 5d20 3d20 4e6f 6e65 2c0d 0a20 2020  me] = None,..   
+00001280: 2020 2020 2020 2020 2020 2020 2020 2076                 v
+00001290: 6172 3a20 4f70 7469 6f6e 616c 5b70 642e  ar: Optional[pd.
+000012a0: 4461 7461 4672 616d 655d 203d 204e 6f6e  DataFrame] = Non
+000012b0: 652c 0d0a 2020 2020 2020 2020 2020 2020  e,..            
+000012c0: 2020 2020 2020 7061 7469 656e 745f 6964        patient_id
+000012d0: 5f63 6f6c 3a20 4f70 7469 6f6e 616c 5b73  _col: Optional[s
+000012e0: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
+000012f0: 2020 2020 2020 2020 2020 2020 2020 293a                ):
+00001300: 0d0a 2020 2020 2020 2020 2222 2243 7265  ..        """Cre
+00001310: 6174 6573 2061 203a 636c 6173 733a 607e  ates a :class:`~
+00001320: 636e 6d66 736e 732e 6461 7461 7365 742e  cnmfsns.dataset.
+00001330: 4461 7461 7365 7460 206f 626a 6563 7420  Dataset` object 
+00001340: 6672 6f6d 2061 2070 616e 6461 7320 4461  from a pandas Da
+00001350: 7461 4672 616d 652e 0d0a 0d0a 2020 2020  taFrame.....    
+00001360: 2020 2020 3a70 6172 616d 2064 6174 613a      :param data:
+00001370: 2041 6e20 6f62 7365 7276 6174 696f 6e73   An observations
+00001380: 20c3 9720 7661 7269 6162 6c65 7320 6461   .. variables da
+00001390: 7461 0d0a 2020 2020 2020 2020 3a74 7970  ta..        :typ
+000013a0: 6520 6461 7461 3a20 7064 2e44 6174 6146  e data: pd.DataF
+000013b0: 7261 6d65 0d0a 2020 2020 2020 2020 3a70  rame..        :p
+000013c0: 6172 616d 2069 735f 6e6f 726d 616c 697a  aram is_normaliz
+000013d0: 6564 3a20 5370 6563 6966 7920 6966 2064  ed: Specify if d
+000013e0: 6174 6120 6973 2061 6c72 6561 6479 206e  ata is already n
+000013f0: 6f72 6d61 6c69 7a65 6420 6f72 2077 6865  ormalized or whe
+00001400: 7468 6572 206e 6f74 2e20 5261 7720 6461  ther not. Raw da
+00001410: 7461 2077 696c 6c20 6265 2054 504d 206e  ta will be TPM n
+00001420: 6f72 6d61 6c69 7a65 6420 7072 696f 7220  ormalized prior 
+00001430: 746f 206f 7665 7264 6973 7065 7273 6564  to overdispersed
+00001440: 2067 656e 6520 7365 6c65 6374 696f 6e2c   gene selection,
+00001450: 2077 6865 7265 6173 2061 6c72 6561 6479   whereas already
+00001460: 206e 6f72 6d61 6c69 7a65 6420 6461 7461   normalized data
+00001470: 2077 696c 6c20 6e6f 742e 0d0a 2020 2020   will not...    
+00001480: 2020 2020 3a74 7970 6520 6973 5f6e 6f72      :type is_nor
+00001490: 6d61 6c69 7a65 643a 2062 6f6f 6c0d 0a20  malized: bool.. 
+000014a0: 2020 2020 2020 203a 7061 7261 6d20 7370         :param sp
+000014b0: 6172 7369 6679 3a20 5374 6f72 6520 6461  arsify: Store da
+000014c0: 7461 2061 7320 6120 7370 6172 7365 206d  ta as a sparse m
+000014d0: 6174 7269 782e 205b 4e6f 7465 2074 6861  atrix. [Note tha
+000014e0: 7420 7468 6973 2066 6561 7475 7265 2069  t this feature i
+000014f0: 7320 6578 7065 7269 6d65 6e74 616c 5d2c  s experimental],
+00001500: 2064 6566 6175 6c74 7320 746f 2046 616c   defaults to Fal
+00001510: 7365 0d0a 2020 2020 2020 2020 3a74 7970  se..        :typ
+00001520: 6520 7370 6172 7369 6679 3a20 626f 6f6c  e sparsify: bool
+00001530: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00001540: 2020 2020 3a70 6172 616d 206f 6273 3a20      :param obs: 
+00001550: 416e 206f 6273 6572 7661 7469 6f6e 7320  An observations 
+00001560: c397 206d 6574 6164 6174 6120 6d61 7472  .. metadata matr
+00001570: 6978 2c20 6465 6661 756c 7473 2074 6f20  ix, defaults to 
+00001580: 4e6f 6e65 0d0a 2020 2020 2020 2020 3a74  None..        :t
+00001590: 7970 6520 6f62 733a 2060 7064 2e44 6174  ype obs: `pd.Dat
+000015a0: 6146 7261 6d65 602c 206f 7074 696f 6e61  aFrame`, optiona
+000015b0: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
+000015c0: 6d20 7661 723a 2041 2076 6172 6961 626c  m var: A variabl
+000015d0: 6573 20c3 9720 6d65 7461 6461 7461 206d  es .. metadata m
+000015e0: 6174 7269 782c 2064 6566 6175 6c74 7320  atrix, defaults 
+000015f0: 746f 204e 6f6e 650d 0a20 2020 2020 2020  to None..       
+00001600: 203a 7479 7065 2076 6172 3a20 6070 642e   :type var: `pd.
+00001610: 4461 7461 4672 616d 6560 2c20 6f70 7469  DataFrame`, opti
+00001620: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+00001630: 6172 616d 2070 6174 6965 6e74 5f69 645f  aram patient_id_
+00001640: 636f 6c3a 204e 616d 6520 6f66 206d 6574  col: Name of met
+00001650: 6164 6174 6120 6c61 7965 7220 7769 7468  adata layer with
+00001660: 2070 6174 6965 6e74 2049 4420 696e 666f   patient ID info
+00001670: 726d 6174 696f 6e2c 2064 6566 6175 6c74  rmation, default
+00001680: 7320 746f 204e 6f6e 650d 0a20 2020 2020  s to None..     
+00001690: 2020 203a 7479 7065 2070 6174 6965 6e74     :type patient
+000016a0: 5f69 645f 636f 6c3a 2073 7472 2c20 6f70  _id_col: str, op
+000016b0: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+000016c0: 3a72 6574 7572 6e3a 204f 626a 6563 7420  :return: Object 
+000016d0: 7769 7468 2065 7870 7265 7373 696f 6e20  with expression 
+000016e0: 616e 6420 6d65 7461 6461 7461 0d0a 2020  and metadata..  
+000016f0: 2020 2020 2020 3a72 7479 7065 3a20 3a63        :rtype: :c
+00001700: 6c61 7373 3a60 7e63 6e6d 6673 6e73 2e64  lass:`~cnmfsns.d
+00001710: 6174 6173 6574 2e44 6174 6173 6574 600d  ataset.Dataset`.
+00001720: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00001730: 2020 2020 2020 6966 2076 6172 2069 7320        if var is 
+00001740: 6e6f 7420 4e6f 6e65 3a0d 0a20 2020 2020  not None:..     
+00001750: 2020 2020 2020 2076 6172 203d 2076 6172         var = var
+00001760: 2e72 6569 6e64 6578 2864 6174 612e 636f  .reindex(data.co
+00001770: 6c75 6d6e 7329 0d0a 2020 2020 2020 2020  lumns)..        
+00001780: 6966 2073 7061 7273 6966 793a 0d0a 2020  if sparsify:..  
+00001790: 2020 2020 2020 2020 2020 6461 7461 203d            data =
+000017a0: 2073 702e 6373 725f 6d61 7472 6978 2864   sp.csr_matrix(d
+000017b0: 6174 612e 7661 6c75 6573 290d 0a20 2020  ata.values)..   
+000017c0: 2020 2020 2064 6174 6120 3d20 6461 7461       data = data
+000017d0: 2e61 7374 7970 6528 2266 6c6f 6174 3332  .astype("float32
+000017e0: 2229 0d0a 2020 2020 2020 2020 756e 7320  ")..        uns 
+000017f0: 3d20 7b22 6869 7374 6f72 7922 3a20 7b7d  = {"history": {}
+00001800: 2c20 226f 6467 223a 7b7d 7d0d 0a20 2020  , "odg":{}}..   
+00001810: 2020 2020 2061 6461 7461 203d 2061 642e       adata = ad.
+00001820: 416e 6e44 6174 6128 583d 6461 7461 2c20  AnnData(X=data, 
+00001830: 7661 723d 7661 722c 2075 6e73 3d75 6e73  var=var, uns=uns
+00001840: 290d 0a20 2020 2020 2020 2064 6174 6173  )..        datas
+00001850: 6574 203d 2063 6c73 2861 6461 7461 3d61  et = cls(adata=a
+00001860: 6461 7461 2c20 7061 7469 656e 745f 6964  data, patient_id
+00001870: 5f63 6f6c 3d70 6174 6965 6e74 5f69 645f  _col=patient_id_
+00001880: 636f 6c29 0d0a 2020 2020 2020 2020 6966  col)..        if
+00001890: 206f 6273 2069 7320 6e6f 7420 4e6f 6e65   obs is not None
+000018a0: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+000018b0: 6174 6173 6574 2e75 7064 6174 655f 6f62  ataset.update_ob
+000018c0: 7328 6f62 733d 6f62 7329 200d 0a20 2020  s(obs=obs) ..   
+000018d0: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
+000018e0: 7365 740d 0a20 2020 200d 0a20 2020 2040  set..    ..    @
+000018f0: 636c 6173 736d 6574 686f 640d 0a20 2020  classmethod..   
+00001900: 2064 6566 2066 726f 6d5f 6835 6164 2863   def from_h5ad(c
+00001910: 6c73 2c0d 0a20 2020 2020 2020 2020 2020  ls,..           
+00001920: 2020 2020 2020 2068 3561 645f 6669 6c65         h5ad_file
+00001930: 3a20 7374 722c 0d0a 2020 2020 2020 2020  : str,..        
+00001940: 2020 2020 2020 2020 2020 6e61 6d65 3a20            name: 
+00001950: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
+00001960: 4e6f 6e65 2c0d 0a20 2020 2020 2020 2020  None,..         
+00001970: 2020 2020 2020 2020 2070 6174 6965 6e74           patient
+00001980: 5f69 645f 636f 6c3a 204f 7074 696f 6e61  _id_col: Optiona
+00001990: 6c5b 7374 725d 203d 204e 6f6e 652c 0d0a  l[str] = None,..
+000019a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000019b0: 2020 666f 7263 655f 6d69 6772 6174 653d    force_migrate=
+000019c0: 4661 6c73 652c 2062 6163 6b65 643d 4661  False, backed=Fa
+000019d0: 6c73 650d 0a20 2020 2020 2020 2020 2020  lse..           
+000019e0: 2020 2020 2020 2029 3a0d 0a20 2020 2020         ):..     
+000019f0: 2020 2022 2222 4372 6561 7465 7320 6120     """Creates a 
+00001a00: 3a63 6c61 7373 3a60 7e63 6e6d 6673 6e73  :class:`~cnmfsns
+00001a10: 2e64 6174 6173 6574 2e44 6174 6173 6574  .dataset.Dataset
+00001a20: 6020 6f62 6a65 6374 2066 726f 6d20 616e  ` object from an
+00001a30: 2041 6e6e 4461 7461 2d63 6f6d 7061 7469   AnnData-compati
+00001a40: 626c 6520 2e68 3561 6420 6669 6c65 2e0d  ble .h5ad file..
+00001a50: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00001a60: 6d20 6835 6164 5f66 696c 653a 2050 6174  m h5ad_file: Pat
+00001a70: 6820 746f 202e 6835 6164 2066 696c 6520  h to .h5ad file 
+00001a80: 7072 6f64 7563 6564 2062 7920 7363 616e  produced by scan
+00001a90: 7079 2c20 416e 6e44 6174 612c 206f 7220  py, AnnData, or 
+00001aa0: 634e 4d46 2d53 4e53 0d0a 2020 2020 2020  cNMF-SNS..      
+00001ab0: 2020 3a74 7970 6520 6835 6164 5f66 696c    :type h5ad_fil
+00001ac0: 653a 2073 7472 0d0a 2020 2020 2020 2020  e: str..        
+00001ad0: 3a70 6172 616d 2070 6174 6965 6e74 5f69  :param patient_i
+00001ae0: 645f 636f 6c3a 204e 616d 6520 6f66 206d  d_col: Name of m
+00001af0: 6574 6164 6174 6120 6c61 7965 7220 7769  etadata layer wi
+00001b00: 7468 2070 6174 6965 6e74 2049 4420 696e  th patient ID in
+00001b10: 666f 726d 6174 696f 6e2c 2064 6566 6175  formation, defau
+00001b20: 6c74 7320 746f 204e 6f6e 650d 0a20 2020  lts to None..   
+00001b30: 2020 2020 203a 7479 7065 2070 6174 6965       :type patie
+00001b40: 6e74 5f69 645f 636f 6c3a 2073 7472 2c20  nt_id_col: str, 
+00001b50: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+00001b60: 2020 3a70 6172 616d 2066 6f72 6365 5f6d    :param force_m
+00001b70: 6967 7261 7465 3a20 666f 7263 6573 2063  igrate: forces c
+00001b80: 6f6e 7665 7273 696f 6e20 6f66 2041 6e6e  onversion of Ann
+00001b90: 4461 7461 206f 626a 6563 7473 2065 7665  Data objects eve
+00001ba0: 6e20 7768 656e 2061 6461 7461 2e58 2061  n when adata.X a
+00001bb0: 6e64 2061 6461 7461 2e72 6177 2e58 2061  nd adata.raw.X a
+00001bc0: 7265 206e 6f74 206c 696e 6561 726c 7920  re not linearly 
+00001bd0: 7363 616c 6564 2072 656c 6174 6976 6520  scaled relative 
+00001be0: 746f 2065 6163 6820 6f74 6865 722c 2064  to each other, d
+00001bf0: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+00001c00: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00001c10: 666f 7263 655f 6d69 6772 6174 653a 2062  force_migrate: b
+00001c20: 6f6f 6c2c 206f 7074 696f 6e61 6c0d 0a20  ool, optional.. 
+00001c30: 2020 2020 2020 203a 7061 7261 6d20 6261         :param ba
+00001c40: 636b 6564 3a20 5573 6520 6261 636b 6564  cked: Use backed
+00001c50: 206d 6f64 6520 746f 206f 7065 6e20 6835   mode to open h5
+00001c60: 6164 2066 696c 652e 2054 6869 7320 6361  ad file. This ca
+00001c70: 6e20 7361 7665 206d 656d 6f72 7920 7768  n save memory wh
+00001c80: 656e 2074 6865 2064 6174 6173 6574 2069  en the dataset i
+00001c90: 7320 7665 7279 206c 6172 6765 2c20 6275  s very large, bu
+00001ca0: 7420 6973 206e 6f74 2063 6f6d 7061 7469  t is not compati
+00001cb0: 626c 6520 7769 7468 2068 3561 6420 6669  ble with h5ad fi
+00001cc0: 6c65 7320 7072 6f64 7563 6564 206f 7574  les produced out
+00001cd0: 7369 6465 206f 6620 634e 4d46 2d53 4e53  side of cNMF-SNS
+00001ce0: 2c20 6465 6661 756c 7473 2074 6f20 4661  , defaults to Fa
+00001cf0: 6c73 650d 0a20 2020 2020 2020 203a 7479  lse..        :ty
+00001d00: 7065 2062 6163 6b65 643a 2062 6f6f 6c2c  pe backed: bool,
+00001d10: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00001d20: 2020 203a 7265 7475 726e 3a20 4f62 6a65     :return: Obje
+00001d30: 6374 2077 6974 6820 6578 7072 6573 7369  ct with expressi
+00001d40: 6f6e 2061 6e64 206d 6574 6164 6174 610d  on and metadata.
+00001d50: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00001d60: 203a 636c 6173 733a 607e 636e 6d66 736e   :class:`~cnmfsn
+00001d70: 732e 6461 7461 7365 742e 4461 7461 7365  s.dataset.Datase
+00001d80: 7460 0d0a 2020 2020 2020 2020 2222 220d  t`..        """.
+00001d90: 0a20 2020 2020 2020 2061 6461 7461 203d  .        adata =
+00001da0: 2061 642e 7265 6164 5f68 3561 6428 6835   ad.read_h5ad(h5
+00001db0: 6164 5f66 696c 652c 2062 6163 6b65 643d  ad_file, backed=
+00001dc0: 6261 636b 6564 290d 0a20 2020 2020 2020  backed)..       
+00001dd0: 2064 6174 6173 6574 203d 2044 6174 6173   dataset = Datas
+00001de0: 6574 2861 6461 7461 3d61 6461 7461 2c20  et(adata=adata, 
+00001df0: 7061 7469 656e 745f 6964 5f63 6f6c 3d70  patient_id_col=p
+00001e00: 6174 6965 6e74 5f69 645f 636f 6c2c 2066  atient_id_col, f
+00001e10: 6f72 6365 5f6d 6967 7261 7465 3d66 6f72  orce_migrate=for
+00001e20: 6365 5f6d 6967 7261 7465 290d 0a20 2020  ce_migrate)..   
+00001e30: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
+00001e40: 7365 740d 0a20 2020 200d 0a20 2020 2040  set..    ..    @
+00001e50: 7072 6f70 6572 7479 0d0a 2020 2020 6465  property..    de
+00001e60: 6620 6973 5f6e 6f72 6d61 6c69 7a65 6428  f is_normalized(
+00001e70: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00001e80: 2222 224f 7574 7075 7473 2074 6865 206e  """Outputs the n
+00001e90: 6f72 6d61 6c69 7a61 7469 6f6e 2073 7461  ormalization sta
+00001ea0: 7475 7320 6f66 2074 6865 2064 6174 6173  tus of the datas
+00001eb0: 6574 2e0d 0a0d 0a20 2020 2020 2020 203a  et.....        :
+00001ec0: 7265 7475 726e 3a20 5472 7565 2069 6620  return: True if 
+00001ed0: 6461 7461 7365 7420 636f 6e74 6169 6e73  dataset contains
+00001ee0: 206e 6f72 6d61 6c69 7a65 6420 6461 7461   normalized data
+00001ef0: 2c20 4661 6c73 6520 6966 2069 7420 6973  , False if it is
+00001f00: 2072 6177 2064 6174 612e 0d0a 2020 2020   raw data...    
+00001f10: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
+00001f20: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00001f30: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00001f40: 6c66 2e61 6461 7461 2e75 6e73 5b22 6973  lf.adata.uns["is
+00001f50: 5f6e 6f72 6d61 6c69 7a65 6422 5d0d 0a20  _normalized"].. 
+00001f60: 2020 200d 0a20 2020 2040 6973 5f6e 6f72     ..    @is_nor
+00001f70: 6d61 6c69 7a65 642e 7365 7474 6572 0d0a  malized.setter..
+00001f80: 2020 2020 6465 6620 6973 5f6e 6f72 6d61      def is_norma
+00001f90: 6c69 7a65 6428 7365 6c66 2c20 7661 6c75  lized(self, valu
+00001fa0: 653a 2062 6f6f 6c29 3a0d 0a20 2020 2020  e: bool):..     
+00001fb0: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
+00001fc0: 735b 2269 735f 6e6f 726d 616c 697a 6564  s["is_normalized
+00001fd0: 225d 203d 2076 616c 7565 0d0a 2020 2020  "] = value..    
+00001fe0: 2020 2020 0d0a 2020 2020 4070 726f 7065      ..    @prope
+00001ff0: 7274 790d 0a20 2020 2064 6566 2063 6e6d  rty..    def cnm
+00002000: 6673 6e73 5f76 6572 7369 6f6e 2873 656c  fsns_version(sel
+00002010: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
+00002020: 634e 4d46 2d53 4e53 2076 6572 7369 6f6e  cNMF-SNS version
+00002030: 2075 7365 6420 746f 2063 7265 6174 6520   used to create 
+00002040: 7468 6520 6461 7461 7365 740d 0a0d 0a20  the dataset.... 
+00002050: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+00002060: 7665 7273 696f 6e0d 0a20 2020 2020 2020  version..       
+00002070: 203a 7274 7970 653a 2073 7472 0d0a 2020   :rtype: str..  
+00002080: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00002090: 2020 2069 6620 2263 6e6d 6673 6e73 5f76     if "cnmfsns_v
+000020a0: 6572 7369 6f6e 2220 696e 2073 656c 662e  ersion" in self.
+000020b0: 6164 6174 612e 756e 733a 0d0a 2020 2020  adata.uns:..    
+000020c0: 2020 2020 2020 2020 7665 7273 696f 6e20          version 
+000020d0: 3d20 7365 6c66 2e61 6461 7461 2e75 6e73  = self.adata.uns
+000020e0: 5b22 636e 6d66 736e 735f 7665 7273 696f  ["cnmfsns_versio
+000020f0: 6e22 5d0d 0a20 2020 2020 2020 2065 6c73  n"]..        els
+00002100: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00002110: 7665 7273 696f 6e20 3d20 4e6f 6e65 0d0a  version = None..
+00002120: 2020 2020 2020 2020 7265 7475 726e 2076          return v
+00002130: 6572 7369 6f6e 0d0a 2020 2020 2020 2020  ersion..        
+00002140: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+00002150: 0a20 2020 2064 6566 2068 6173 5f63 6e6d  .    def has_cnm
+00002160: 665f 7265 7375 6c74 7328 7365 6c66 293a  f_results(self):
+00002170: 0d0a 2020 2020 2020 2020 2222 2254 6573  ..        """Tes
+00002180: 7420 666f 7220 7765 6874 6865 7220 4461  t for wehther Da
+00002190: 7461 7365 7420 636f 6e74 6169 6e73 2063  taset contains c
+000021a0: 4e4d 4620 7265 7375 6c74 7320 666f 7220  NMF results for 
+000021b0: 7468 6520 6461 7461 7365 740d 0a0d 0a20  the dataset.... 
+000021c0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
+000021d0: 5768 6574 6865 7220 636f 6d70 6c65 7465  Whether complete
+000021e0: 2063 4e4d 4620 7265 7375 6c74 7320 6172   cNMF results ar
+000021f0: 6520 636f 6e74 6169 6e65 6420 666f 7220  e contained for 
+00002200: 6174 206c 6561 7374 2031 2072 616e 6b20  at least 1 rank 
+00002210: 286b 290d 0a20 2020 2020 2020 203a 7274  (k)..        :rt
+00002220: 7970 653a 2062 6f6f 6c0d 0a20 2020 2020  ype: bool..     
+00002230: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00002240: 6d61 7472 6978 5f63 6865 636b 7320 3d20  matrix_checks = 
+00002250: 5b0d 0a20 2020 2020 2020 2020 2020 2022  [..            "
+00002260: 636e 6d66 5f75 7361 6765 2220 696e 2073  cnmf_usage" in s
+00002270: 656c 662e 6164 6174 612e 6f62 736d 2c0d  elf.adata.obsm,.
+00002280: 0a20 2020 2020 2020 2020 2020 2022 636e  .            "cn
+00002290: 6d66 5f67 6570 5f73 636f 7265 2220 696e  mf_gep_score" in
+000022a0: 2073 656c 662e 6164 6174 612e 7661 726d   self.adata.varm
+000022b0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+000022c0: 636e 6d66 5f67 6570 5f74 706d 2220 696e  cnmf_gep_tpm" in
+000022d0: 2073 656c 662e 6164 6174 612e 7661 726d   self.adata.varm
+000022e0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+000022f0: 636e 6d66 5f67 6570 5f72 6177 2220 696e  cnmf_gep_raw" in
+00002300: 2073 656c 662e 6164 6174 612e 7661 726d   self.adata.varm
+00002310: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00002320: 6b76 616c 7322 2069 6e20 7365 6c66 2e61  kvals" in self.a
+00002330: 6461 7461 2e75 6e73 0d0a 2020 2020 2020  data.uns..      
+00002340: 2020 5d0d 0a20 2020 2020 2020 2072 6574    ]..        ret
+00002350: 7572 6e20 616c 6c28 6d61 7472 6978 5f63  urn all(matrix_c
+00002360: 6865 636b 7329 0d0a 2020 2020 2020 2020  hecks)..        
+00002370: 0d0a 2020 2020 4070 726f 7065 7274 790d  ..    @property.
+00002380: 0a20 2020 2064 6566 206f 7665 7264 6973  .    def overdis
+00002390: 7065 7273 6564 5f67 656e 6573 2873 656c  persed_genes(sel
+000023a0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
+000023b0: 4f76 6572 6469 7370 6572 7365 6420 6765  Overdispersed ge
+000023c0: 6e65 206c 6973 7420 7573 6564 2066 6f72  ne list used for
+000023d0: 2063 4e4d 460d 0a0d 0a20 2020 2020 2020   cNMF....       
+000023e0: 203a 7265 7475 726e 3a20 6765 6e65 206c   :return: gene l
+000023f0: 6973 740d 0a20 2020 2020 2020 203a 7274  ist..        :rt
+00002400: 7970 653a 206c 6973 740d 0a20 2020 2020  ype: list..     
+00002410: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00002420: 7265 7475 726e 2073 656c 662e 6164 6174  return self.adat
+00002430: 612e 756e 735b 2267 656e 655f 6c69 7374  a.uns["gene_list
+00002440: 225d 0d0a 0d0a 0d0a 2020 2020 4063 6e6d  "]......    @cnm
+00002450: 6673 6e73 5f76 6572 7369 6f6e 2e73 6574  fsns_version.set
+00002460: 7465 720d 0a20 2020 2064 6566 2063 6e6d  ter..    def cnm
+00002470: 6673 6e73 5f76 6572 7369 6f6e 2873 656c  fsns_version(sel
+00002480: 662c 2076 616c 7565 3a20 626f 6f6c 293a  f, value: bool):
+00002490: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+000024a0: 6461 7461 2e75 6e73 5b22 636e 6d66 736e  data.uns["cnmfsn
+000024b0: 735f 7665 7273 696f 6e22 5d20 3d20 7661  s_version"] = va
+000024c0: 6c75 650d 0a0d 0a20 2020 2020 2020 200d  lue....        .
+000024d0: 0a20 2020 2064 6566 2075 7064 6174 655f  .    def update_
+000024e0: 6f62 7328 7365 6c66 2c20 6f62 7329 3a0d  obs(self, obs):.
+000024f0: 0a20 2020 2020 2020 2022 2222 5570 6461  .        """Upda
+00002500: 7465 2074 6865 206f 6273 6572 7661 7469  te the observati
+00002510: 6f6e 206d 6574 6164 6174 6120 7769 7468  on metadata with
+00002520: 2061 206e 6577 206d 6574 6164 6174 6120   a new metadata 
+00002530: 6d61 7472 6978 0d0a 0d0a 2020 2020 2020  matrix....      
+00002540: 2020 3a70 6172 616d 206f 6273 3a20 416e    :param obs: An
+00002550: 206f 6273 6572 7661 7469 6f6e 7320 c397   observations ..
+00002560: 206d 6574 6164 6174 6120 6d61 7472 6978   metadata matrix
+00002570: 2c20 6465 6661 756c 7473 2074 6f20 4e6f  , defaults to No
+00002580: 6e65 0d0a 2020 2020 2020 2020 3a74 7970  ne..        :typ
+00002590: 6520 6f62 733a 2060 7064 2e44 6174 6146  e obs: `pd.DataF
+000025a0: 7261 6d65 602c 206f 7074 696f 6e61 6c0d  rame`, optional.
+000025b0: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+000025c0: 2020 2020 2020 2320 636f 6e76 6572 7420        # convert 
+000025d0: 276f 626a 6563 7427 2064 7479 7065 2074  'object' dtype t
+000025e0: 6f20 6361 7465 676f 7269 6361 6c2c 2063  o categorical, c
+000025f0: 6f6e 7665 7274 696e 6720 626f 6f6c 2076  onverting bool v
+00002600: 616c 7565 7320 746f 2073 7472 696e 6773  alues to strings
+00002610: 2061 7320 7468 6573 6520 6172 6520 6e6f   as these are no
+00002620: 7420 7375 7070 6f72 7465 6420 6279 2041  t supported by A
+00002630: 6e6e 4461 7461 206f 6e2d 6469 736b 2066  nnData on-disk f
+00002640: 6f72 6d61 740d 0a20 2020 2020 2020 2066  ormat..        f
+00002650: 6f72 2063 6f6c 2069 6e20 6f62 732e 7365  or col in obs.se
+00002660: 6c65 6374 5f64 7479 7065 7328 696e 636c  lect_dtypes(incl
+00002670: 7564 653d 226f 626a 6563 7422 292e 636f  ude="object").co
+00002680: 6c75 6d6e 733a 0d0a 2020 2020 2020 2020  lumns:..        
+00002690: 2020 2020 6f62 735b 636f 6c5d 203d 206f      obs[col] = o
+000026a0: 6273 5b63 6f6c 5d2e 7265 706c 6163 6528  bs[col].replace(
+000026b0: 7b54 7275 653a 2022 5472 7565 222c 2046  {True: "True", F
+000026c0: 616c 7365 3a20 2246 616c 7365 227d 292e  alse: "False"}).
+000026d0: 6173 7479 7065 2822 6361 7465 676f 7279  astype("category
+000026e0: 2229 0d0a 2020 2020 2020 2020 6d69 7373  ")..        miss
+000026f0: 696e 675f 7361 6d70 6c65 735f 696e 5f58  ing_samples_in_X
+00002700: 203d 206f 6273 2e69 6e64 6578 2e64 6966   = obs.index.dif
+00002710: 6665 7265 6e63 6528 7365 6c66 2e61 6461  ference(self.ada
+00002720: 7461 2e6f 6273 2e69 6e64 6578 292e 6173  ta.obs.index).as
+00002730: 7479 7065 2873 7472 292e 746f 5f6c 6973  type(str).to_lis
+00002740: 7428 290d 0a20 2020 2020 2020 2069 6620  t()..        if 
+00002750: 6d69 7373 696e 675f 7361 6d70 6c65 735f  missing_samples_
+00002760: 696e 5f58 3a0d 0a20 2020 2020 2020 2020  in_X:..         
+00002770: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
+00002780: 6e67 2822 5468 6520 666f 6c6c 6f77 696e  ng("The followin
+00002790: 6720 7361 6d70 6c65 7320 696e 2074 6865  g samples in the
+000027a0: 206d 6574 6164 6174 6120 7765 7265 206e   metadata were n
+000027b0: 6f74 2070 7265 7365 6e74 2069 6e20 7468  ot present in th
+000027c0: 6520 6461 7461 2028 6061 6461 7461 2e58  e data (`adata.X
+000027d0: 6029 3a5c 6e20 202d 2022 202b 2022 5c6e  `):\n  - " + "\n
+000027e0: 2020 2d20 222e 6a6f 696e 286d 6973 7369    - ".join(missi
+000027f0: 6e67 5f73 616d 706c 6573 5f69 6e5f 5829  ng_samples_in_X)
+00002800: 290d 0a20 2020 2020 2020 206d 6973 7369  )..        missi
+00002810: 6e67 5f73 616d 706c 6573 5f69 6e5f 6d64  ng_samples_in_md
+00002820: 203d 2073 656c 662e 6164 6174 612e 6f62   = self.adata.ob
+00002830: 732e 696e 6465 782e 6469 6666 6572 656e  s.index.differen
+00002840: 6365 286f 6273 2e69 6e64 6578 292e 6173  ce(obs.index).as
+00002850: 7479 7065 2873 7472 292e 746f 5f6c 6973  type(str).to_lis
+00002860: 7428 290d 0a20 2020 2020 2020 2069 6620  t()..        if 
+00002870: 6d69 7373 696e 675f 7361 6d70 6c65 735f  missing_samples_
+00002880: 696e 5f6d 643a 0d0a 2020 2020 2020 2020  in_md:..        
+00002890: 2020 2020 6c6f 6767 696e 672e 7761 726e      logging.warn
+000028a0: 696e 6728 2254 6865 2066 6f6c 6c6f 7769  ing("The followi
+000028b0: 6e67 2073 616d 706c 6573 2069 6e20 7468  ng samples in th
+000028c0: 6520 6461 7461 2028 6061 6461 7461 2e58  e data (`adata.X
+000028d0: 6029 2077 6572 6520 6162 7365 6e74 2069  `) were absent i
+000028e0: 6e20 7468 6520 6d65 7461 6461 7461 3a5c  n the metadata:\
+000028f0: 6e20 202d 2022 202b 2022 5c6e 2020 2d20  n  - " + "\n  - 
+00002900: 222e 6a6f 696e 286d 6973 7369 6e67 5f73  ".join(missing_s
+00002910: 616d 706c 6573 5f69 6e5f 6d64 2929 0d0a  amples_in_md))..
+00002920: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+00002930: 7461 2e6f 6273 203d 206f 6273 2e72 6569  ta.obs = obs.rei
+00002940: 6e64 6578 2873 656c 662e 6164 6174 612e  ndex(self.adata.
+00002950: 6f62 732e 696e 6465 7829 0d0a 2020 2020  obs.index)..    
+00002960: 0d0a 2020 2020 6465 6620 6765 745f 6d65  ..    def get_me
+00002970: 7461 6461 7461 5f74 7970 655f 7375 6d6d  tadata_type_summ
+00002980: 6172 7928 7365 6c66 293a 0d0a 2020 2020  ary(self):..    
+00002990: 2020 2020 2222 2252 6574 7572 6e20 6120      """Return a 
+000029a0: 7072 696e 7461 626c 6520 7375 6d6d 6172  printable summar
+000029b0: 7920 6f66 206d 6574 6164 6174 6120 616e  y of metadata an
+000029c0: 6420 7661 6c75 6520 7479 7065 7320 666f  d value types fo
+000029d0: 7220 6561 6368 206d 6574 6164 6174 6120  r each metadata 
+000029e0: 6c61 7965 722e 0d0a 0d0a 2020 2020 2020  layer.....      
+000029f0: 2020 3a72 6574 7572 6e3a 2053 756d 6d61    :return: Summa
+00002a00: 7279 206f 6620 6d65 7461 6461 7461 0d0a  ry of metadata..
+00002a10: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00002a20: 7374 720d 0a20 2020 2020 2020 2022 2222  str..        """
+00002a30: 0d0a 2020 2020 2020 2020 6d73 6720 3d20  ..        msg = 
+00002a40: 2222 0d0a 2020 2020 2020 2020 666f 7220  ""..        for 
+00002a50: 636f 6c20 696e 2073 656c 662e 6164 6174  col in self.adat
+00002a60: 612e 6f62 732e 636f 6c75 6d6e 733a 0d0a  a.obs.columns:..
+00002a70: 2020 2020 2020 2020 2020 2020 6d73 6720              msg 
+00002a80: 2b3d 2022 2020 2020 436f 6c75 6d6e 3a20  += "    Column: 
+00002a90: 2220 2b20 636f 6c20 2b20 225c 6e22 0d0a  " + col + "\n"..
+00002aa0: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00002ab0: 7661 6c75 655f 7479 7065 2c20 636f 756e  value_type, coun
+00002ac0: 7420 696e 2073 656c 662e 6164 6174 612e  t in self.adata.
+00002ad0: 6f62 735b 636f 6c5d 2e64 726f 706e 6128  obs[col].dropna(
+00002ae0: 292e 6d61 7028 7479 7065 292e 7661 6c75  ).map(type).valu
+00002af0: 655f 636f 756e 7473 2829 2e69 7465 6d73  e_counts().items
+00002b00: 2829 3a0d 0a20 2020 2020 2020 2020 2020  ():..           
+00002b10: 2020 2020 206d 7367 202b 3d20 6622 2020       msg += f"  
+00002b20: 2020 2020 2020 7b76 616c 7565 5f74 7970        {value_typ
+00002b30: 657d 3a20 7b63 6f75 6e74 7d5c 6e22 0d0a  e}: {count}\n"..
+00002b40: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+00002b50: 7367 0d0a 2020 2020 0d0a 2020 2020 6465  sg..    ..    de
+00002b60: 6620 7772 6974 655f 6835 6164 2873 656c  f write_h5ad(sel
+00002b70: 662c 2066 696c 656e 616d 6529 3a0d 0a20  f, filename):.. 
+00002b80: 2020 2020 2020 2022 2222 5772 6974 6520         """Write 
+00002b90: 6461 7461 7365 7420 746f 202e 6835 6164  dataset to .h5ad
+00002ba0: 2066 696c 652e 0d0a 0d0a 2020 2020 2020   file.....      
+00002bb0: 2020 3a70 6172 616d 2066 696c 656e 616d    :param filenam
+00002bc0: 653a 2066 696c 6570 6174 680d 0a20 2020  e: filepath..   
+00002bd0: 2020 2020 203a 7479 7065 2066 696c 656e       :type filen
+00002be0: 616d 653a 2073 7472 0d0a 2020 2020 2020  ame: str..      
+00002bf0: 2020 2222 220d 0a20 2020 2020 2020 2066    """..        f
+00002c00: 696c 656e 616d 6520 3d20 6f73 2e70 6174  ilename = os.pat
+00002c10: 682e 6162 7370 6174 6828 6669 6c65 6e61  h.abspath(filena
+00002c20: 6d65 290d 0a20 2020 2020 2020 206c 6f67  me)..        log
+00002c30: 6769 6e67 2e69 6e66 6f28 6622 5772 6974  ging.info(f"Writ
+00002c40: 696e 6720 746f 207b 6669 6c65 6e61 6d65  ing to {filename
+00002c50: 7d22 290d 0a20 2020 2020 2020 2073 656c  }")..        sel
+00002c60: 662e 6164 6174 612e 7772 6974 655f 6835  f.adata.write_h5
+00002c70: 6164 2866 696c 656e 616d 6529 0d0a 2020  ad(filename)..  
+00002c80: 2020 2020 2020 6c6f 6767 696e 672e 696e        logging.in
+00002c90: 666f 2866 2244 6f6e 6522 290d 0a20 2020  fo(f"Done")..   
+00002ca0: 200d 0a20 2020 2064 6566 2074 6f5f 6466   ..    def to_df
+00002cb0: 2873 656c 662c 206e 6f72 6d61 6c69 7a65  (self, normalize
+00002cc0: 643d 4661 6c73 6529 3a0d 0a20 2020 2020  d=False):..     
+00002cd0: 2020 2022 2222 4765 7420 6461 7461 206d     """Get data m
+00002ce0: 6174 7269 7820 6173 2061 2060 7064 2e44  atrix as a `pd.D
+00002cf0: 6174 6146 7261 6d65 600d 0a0d 0a20 2020  ataFrame`....   
+00002d00: 2020 2020 203a 7061 7261 6d20 6e6f 726d       :param norm
+00002d10: 616c 697a 6564 3a20 5365 7420 7472 7565  alized: Set true
+00002d20: 2066 6f72 2054 504d 206e 6f72 6d61 6c69   for TPM normali
+00002d30: 7a65 6420 6f75 7470 7574 2c20 6465 6661  zed output, defa
+00002d40: 756c 7473 2074 6f20 4661 6c73 650d 0a20  ults to False.. 
+00002d50: 2020 2020 2020 203a 7479 7065 206e 6f72         :type nor
+00002d60: 6d61 6c69 7a65 643a 2062 6f6f 6c2c 206f  malized: bool, o
+00002d70: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00002d80: 203a 7265 7475 726e 3a20 6f62 7365 7276   :return: observ
+00002d90: 6174 696f 6e73 20c3 9720 7661 7269 6162  ations .. variab
+00002da0: 6c65 7320 6461 7461 206d 6174 7269 780d  les data matrix.
+00002db0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00002dc0: 2070 642e 4461 7461 4672 616d 650d 0a20   pd.DataFrame.. 
+00002dd0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00002de0: 2020 2020 6466 203d 2073 656c 662e 6164      df = self.ad
+00002df0: 6174 612e 746f 5f64 6628 290d 0a20 2020  ata.to_df()..   
+00002e00: 2020 2020 2069 6620 6e6f 726d 616c 697a       if normaliz
+00002e10: 6564 2061 6e64 206e 6f74 2073 656c 662e  ed and not self.
+00002e20: 6973 5f6e 6f72 6d61 6c69 7a65 643a 0d0a  is_normalized:..
+00002e30: 2020 2020 2020 2020 2020 2020 6466 203d              df =
+00002e40: 2064 662e 6469 7628 6466 2e73 756d 2861   df.div(df.sum(a
+00002e50: 7869 733d 3129 2c20 6178 6973 3d30 2920  xis=1), axis=0) 
+00002e60: 2a20 3165 3620 2023 2054 504d 206e 6f72  * 1e6  # TPM nor
+00002e70: 6d61 6c69 7a61 7469 6f6e 0d0a 2020 2020  malization..    
+00002e80: 2020 2020 7265 7475 726e 2064 660d 0a20      return df.. 
+00002e90: 2020 2020 2020 200d 0a20 2020 2064 6566         ..    def
+00002ea0: 2072 656d 6f76 655f 756e 6661 6374 6f72   remove_unfactor
+00002eb0: 697a 6162 6c65 5f67 656e 6573 2873 656c  izable_genes(sel
+00002ec0: 6629 3a0d 0a20 2020 2020 2020 2022 2222  f):..        """
+00002ed0: 5265 6d6f 7665 7320 6765 6e65 7320 7769  Removes genes wi
+00002ee0: 7468 206d 6973 7369 6e67 2076 616c 7565  th missing value
+00002ef0: 7320 6f72 207a 6572 6f20 7661 7269 616e  s or zero varian
+00002f00: 6365 2066 726f 6d20 7468 6520 6461 7461  ce from the data
+00002f10: 206d 6174 7269 782e 0d0a 2020 2020 2020   matrix...      
+00002f20: 2020 2222 220d 0a20 2020 2020 2020 2064    """..        d
+00002f30: 6620 3d20 7365 6c66 2e74 6f5f 6466 286e  f = self.to_df(n
+00002f40: 6f72 6d61 6c69 7a65 643d 4661 6c73 6529  ormalized=False)
+00002f50: 0d0a 2020 2020 2020 2020 2320 4368 6563  ..        # Chec
+00002f60: 6b20 666f 7220 7661 7269 6162 6c65 7320  k for variables 
+00002f70: 7769 7468 206d 6973 7369 6e67 2076 616c  with missing val
+00002f80: 7565 730d 0a20 2020 2020 2020 2067 656e  ues..        gen
+00002f90: 6573 5f77 6974 685f 6d69 7373 696e 6776  es_with_missingv
+00002fa0: 616c 7565 7320 3d20 6466 2e69 736e 756c  alues = df.isnul
+00002fb0: 6c28 292e 616e 7928 290d 0a20 2020 2020  l().any()..     
+00002fc0: 2020 200d 0a20 2020 2020 2020 2069 6620     ..        if 
+00002fd0: 6765 6e65 735f 7769 7468 5f6d 6973 7369  genes_with_missi
+00002fe0: 6e67 7661 6c75 6573 2e61 6e79 2829 3a0d  ngvalues.any():.
+00002ff0: 0a20 2020 2020 2020 2020 2020 206e 5f6d  .            n_m
+00003000: 6973 7369 6e67 203d 2067 656e 6573 5f77  issing = genes_w
+00003010: 6974 685f 6d69 7373 696e 6776 616c 7565  ith_missingvalue
+00003020: 732e 7375 6d28 290d 0a20 2020 2020 2020  s.sum()..       
+00003030: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
+00003040: 6e69 6e67 2866 227b 6e5f 6d69 7373 696e  ning(f"{n_missin
+00003050: 677d 206f 6620 7b73 656c 662e 6164 6174  g} of {self.adat
+00003060: 612e 6e5f 7661 7273 7d20 7661 7269 6162  a.n_vars} variab
+00003070: 6c65 7320 6172 6520 6d69 7373 696e 6720  les are missing 
+00003080: 7661 6c75 6573 2028 6061 6461 7461 2e58  values (`adata.X
+00003090: 6029 2e22 290d 0a20 2020 2020 2020 2020  `).")..         
+000030a0: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
+000030b0: 6e67 2866 2253 7562 7365 7474 696e 6720  ng(f"Subsetting 
+000030c0: 7661 7269 6162 6c65 7320 746f 2074 686f  variables to tho
+000030d0: 7365 2077 6974 6820 6e6f 206d 6973 7369  se with no missi
+000030e0: 6e67 2076 616c 7565 732e 2229 0d0a 2020  ng values.")..  
+000030f0: 2020 2020 2020 2020 2020 2020 2020 0d0a                ..
+00003100: 2020 2020 2020 2020 2320 4368 6563 6b20          # Check 
+00003110: 666f 7220 6765 6e65 7320 7769 7468 207a  for genes with z
+00003120: 6572 6f20 7661 7269 616e 6365 0d0a 2020  ero variance..  
+00003130: 2020 2020 2020 7a65 726f 7661 7267 656e        zerovargen
+00003140: 6573 203d 2028 6466 2e76 6172 2829 203d  es = (df.var() =
+00003150: 3d20 3029 0d0a 2020 2020 2020 2020 6966  = 0)..        if
+00003160: 207a 6572 6f76 6172 6765 6e65 732e 616e   zerovargenes.an
+00003170: 7928 293a 0d0a 2020 2020 2020 2020 2020  y():..          
+00003180: 2020 6e5f 7a65 726f 7661 7220 3d20 7a65    n_zerovar = ze
+00003190: 726f 7661 7267 656e 6573 2e73 756d 2829  rovargenes.sum()
+000031a0: 0d0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+000031b0: 6767 696e 672e 7761 726e 696e 6728 6622  gging.warning(f"
+000031c0: 7b6e 5f7a 6572 6f76 6172 7d20 6f66 207b  {n_zerovar} of {
+000031d0: 7365 6c66 2e61 6461 7461 2e6e 5f76 6172  self.adata.n_var
+000031e0: 737d 2076 6172 6961 626c 6573 2068 6176  s} variables hav
+000031f0: 6520 6120 7661 7269 616e 6365 206f 6620  e a variance of 
+00003200: 7a65 726f 2069 6e20 636f 756e 7473 2064  zero in counts d
+00003210: 6174 6120 2860 6164 6174 612e 7261 772e  ata (`adata.raw.
+00003220: 5860 292e 2229 0d0a 2020 2020 2020 2020  X`).")..        
+00003230: 2020 2020 6c6f 6767 696e 672e 7761 726e      logging.warn
+00003240: 696e 6728 6622 5375 6273 6574 7469 6e67  ing(f"Subsetting
+00003250: 2076 6172 6961 626c 6573 2074 6f20 7468   variables to th
+00003260: 6f73 6520 7769 7468 206e 6f6e 7a65 726f  ose with nonzero
+00003270: 2076 6172 6961 6e63 652e 2229 0d0a 2020   variance.")..  
+00003280: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00003290: 6765 6e65 735f 746f 5f6b 6565 7020 3d20  genes_to_keep = 
+000032a0: 287e 6765 6e65 735f 7769 7468 5f6d 6973  (~genes_with_mis
+000032b0: 7369 6e67 7661 6c75 6573 2920 2620 287e  singvalues) & (~
+000032c0: 7a65 726f 7661 7267 656e 6573 290d 0a20  zerovargenes).. 
+000032d0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+000032e0: 2073 656c 662e 6164 6174 6120 3d20 7365   self.adata = se
+000032f0: 6c66 2e61 6461 7461 5b3a 2c67 656e 6573  lf.adata[:,genes
+00003300: 5f74 6f5f 6b65 6570 5d0d 0a0d 0a20 2020  _to_keep]....   
+00003310: 2064 6566 2063 6f6d 7075 7465 5f67 656e   def compute_gen
+00003320: 655f 7374 6174 7328 7365 6c66 2c20 6f64  e_stats(self, od
+00003330: 675f 6465 6661 756c 745f 7370 6c69 6e65  g_default_spline
+00003340: 5f64 6567 7265 653a 2069 6e74 203d 2033  _degree: int = 3
+00003350: 2c20 6f64 675f 6465 6661 756c 745f 646f  , odg_default_do
+00003360: 663a 2069 6e74 203d 2038 293a 0d0a 2020  f: int = 8):..  
+00003370: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00003380: 2020 2043 6f6d 7075 7465 7320 6765 6e65     Computes gene
+00003390: 2073 7461 7469 7374 6963 7320 616e 6420   statistics and 
+000033a0: 6669 7473 2074 776f 206d 6f64 656c 7320  fits two models 
+000033b0: 6f66 206d 6561 6e20 616e 6420 7661 7269  of mean and vari
+000033c0: 616e 6365 206f 6620 6765 6e65 7320 696e  ance of genes in
+000033d0: 2074 6865 2064 6174 6173 6574 2e20 5468   the dataset. Th
+000033e0: 6520 6669 7273 7420 6d65 7468 6f64 2069  e first method i
+000033f0: 7320 7468 650d 0a20 2020 2020 2020 2067  s the..        g
+00003400: 656e 6572 616c 697a 6564 2061 6464 6974  eneralized addit
+00003410: 6976 6520 6d6f 6465 6c20 7769 7468 2073  ive model with s
+00003420: 6d6f 6f74 6820 636f 6d70 6f6e 656e 7473  mooth components
+00003430: 2028 422d 7370 6c69 6e65 7329 2074 6f20   (B-splines) to 
+00003440: 6d6f 6465 6c20 7468 6520 7265 6c61 7469  model the relati
+00003450: 6f6e 7368 6970 206f 6620 6d65 616e 2061  onship of mean a
+00003460: 6e64 2076 6172 6961 6e63 650d 0a20 2020  nd variance..   
+00003470: 2020 2020 2062 6574 7765 656e 2067 656e       between gen
+00003480: 6573 2069 6e20 7468 6520 6461 7461 7365  es in the datase
+00003490: 742e 2049 7420 7072 6f64 7563 6573 2061  t. It produces a
+000034a0: 6e20 6f64 7363 6f72 6520 6d65 7472 6963  n odscore metric
+000034b0: 2066 6f72 206f 7665 7264 6973 7065 7273   for overdispers
+000034c0: 696f 6e2e 2054 6865 2073 6563 6f6e 6420  ion. The second 
+000034d0: 6973 2074 6865 2063 6f75 6e74 2d73 7461  is the count-sta
+000034e0: 7469 7374 6963 730d 0a20 2020 2020 2020  tistics..       
+000034f0: 206d 6574 686f 6420 666f 756e 6420 696e   method found in
+00003500: 2074 6865 2063 4e4d 4620 7061 636b 6167   the cNMF packag
+00003510: 652c 2077 6869 6368 2070 726f 6475 6365  e, which produce
+00003520: 7320 6120 6d6f 6469 6669 6564 2076 2d73  s a modified v-s
+00003530: 636f 7265 206d 6574 7269 632e 2041 6c6c  core metric. All
+00003540: 2067 656e 6520 7374 6174 6973 7469 6373   gene statistics
+00003550: 2061 7265 2073 746f 7265 6420 7769 7468   are stored with
+00003560: 696e 2074 6865 0d0a 2020 2020 2020 2020  in the..        
+00003570: 6461 7461 7365 7420 6f62 6a65 6374 2061  dataset object a
+00003580: 6e64 2061 7265 2061 6363 6573 7369 626c  nd are accessibl
+00003590: 6520 7573 696e 6720 6064 6174 6173 6574  e using `dataset
+000035a0: 2e61 6e6e 6461 7461 2e76 6172 602e 0d0a  .anndata.var`...
+000035b0: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000035c0: 206f 6467 5f64 6566 6175 6c74 5f73 706c   odg_default_spl
+000035d0: 696e 655f 6465 6772 6565 3a20 422d 5370  ine_degree: B-Sp
+000035e0: 6c69 6e65 2064 6567 7265 6520 666f 7220  line degree for 
+000035f0: 474c 4d2d 4741 4d20 6d6f 6465 6c6c 696e  GLM-GAM modellin
+00003600: 6720 6f66 206d 6561 6e2d 7661 7269 616e  g of mean-varian
+00003610: 6365 2072 656c 6174 696f 6e73 6869 702c  ce relationship,
+00003620: 2064 6566 6175 6c74 7320 746f 2033 0d0a   defaults to 3..
+00003630: 2020 2020 2020 2020 3a74 7970 6520 6f64          :type od
+00003640: 675f 6465 6661 756c 745f 7370 6c69 6e65  g_default_spline
+00003650: 5f64 6567 7265 653a 2069 6e74 2c20 6f70  _degree: int, op
+00003660: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
+00003670: 3a70 6172 616d 206f 6467 5f64 6566 6175  :param odg_defau
+00003680: 6c74 5f64 6f66 3a20 4465 6772 6565 7320  lt_dof: Degrees 
+00003690: 6f66 2066 7265 6564 6f6d 2066 6f72 2047  of freedom for G
+000036a0: 4c4d 2d47 414d 206d 6f64 656c 6c69 6e67  LM-GAM modelling
+000036b0: 206f 6620 6d65 616e 2d76 6172 616e 6365   of mean-varance
+000036c0: 2c20 6465 6661 756c 7473 2074 6f20 380d  , defaults to 8.
+000036d0: 0a20 2020 2020 2020 203a 7479 7065 206f  .        :type o
+000036e0: 6467 5f64 6566 6175 6c74 5f64 6f66 3a20  dg_default_dof: 
+000036f0: 696e 742c 206f 7074 696f 6e61 6c0d 0a20  int, optional.. 
+00003700: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
+00003710: 2020 2020 6461 7461 5f72 6177 203d 2073      data_raw = s
+00003720: 656c 662e 746f 5f64 6628 290d 0a20 2020  elf.to_df()..   
+00003730: 2020 2020 2064 6174 615f 6e6f 726d 616c       data_normal
+00003740: 697a 6564 203d 2073 656c 662e 746f 5f64  ized = self.to_d
+00003750: 6628 6e6f 726d 616c 697a 6564 3d54 7275  f(normalized=Tru
+00003760: 6529 0d0a 2020 2020 2020 2020 0d0a 2020  e)..        ..  
+00003770: 2020 2020 2020 2320 6372 6561 7465 2064        # create d
+00003780: 6174 6166 7261 6d65 206f 6620 7065 722d  ataframe of per-
+00003790: 6765 6e65 2073 7461 7469 7374 6963 730d  gene statistics.
+000037a0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+000037b0: 6174 612e 7661 725b 226d 6561 6e22 5d20  ata.var["mean"] 
+000037c0: 3d20 6461 7461 5f6e 6f72 6d61 6c69 7a65  = data_normalize
+000037d0: 642e 6d65 616e 2829 0d0a 2020 2020 2020  d.mean()..      
+000037e0: 2020 7365 6c66 2e61 6461 7461 2e76 6172    self.adata.var
+000037f0: 5b22 7261 6e6b 5f6d 6561 6e22 5d20 3d20  ["rank_mean"] = 
+00003800: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
+00003810: 6d65 616e 225d 2e72 616e 6b28 290d 0a20  mean"].rank().. 
+00003820: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+00003830: 612e 7661 725b 2276 6172 6961 6e63 6522  a.var["variance"
+00003840: 5d20 3d20 6461 7461 5f6e 6f72 6d61 6c69  ] = data_normali
+00003850: 7a65 642e 7661 7228 290d 0a20 2020 2020  zed.var()..     
+00003860: 2020 2073 656c 662e 6164 6174 612e 7661     self.adata.va
+00003870: 725b 2273 6422 5d20 3d20 6461 7461 5f6e  r["sd"] = data_n
+00003880: 6f72 6d61 6c69 7a65 642e 7374 6428 290d  ormalized.std().
+00003890: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+000038a0: 6174 612e 7661 725b 226d 6973 7369 6e67  ata.var["missing
+000038b0: 6e65 7373 225d 203d 2064 6174 615f 6e6f  ness"] = data_no
+000038c0: 726d 616c 697a 6564 2e69 736e 756c 6c28  rmalized.isnull(
+000038d0: 292e 7375 6d28 2920 2f20 6461 7461 5f6e  ).sum() / data_n
+000038e0: 6f72 6d61 6c69 7a65 642e 7368 6170 655b  ormalized.shape[
+000038f0: 305d 0d0a 2020 2020 2020 2020 7365 6c66  0]..        self
+00003900: 2e61 6461 7461 2e76 6172 5b5b 226c 6f67  .adata.var[["log
+00003910: 5f6d 6561 6e22 2c20 226c 6f67 5f76 6172  _mean", "log_var
+00003920: 6961 6e63 6522 5d5d 203d 206e 702e 6c6f  iance"]] = np.lo
+00003930: 6731 3028 7365 6c66 2e61 6461 7461 2e76  g10(self.adata.v
+00003940: 6172 5b5b 226d 6561 6e22 2c20 2276 6172  ar[["mean", "var
+00003950: 6961 6e63 6522 5d5d 290d 0a20 2020 2020  iance"]])..     
+00003960: 2020 2073 656c 662e 6164 6174 612e 7661     self.adata.va
+00003970: 725b 226d 6561 6e5f 636f 756e 7473 225d  r["mean_counts"]
+00003980: 203d 2064 6174 615f 7261 772e 6d65 616e   = data_raw.mean
+00003990: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
+000039a0: 2e61 6461 7461 2e76 6172 5b22 6f64 7363  .adata.var["odsc
+000039b0: 6f72 655f 6578 636c 7564 6564 225d 203d  ore_excluded"] =
+000039c0: 2028 2873 656c 662e 6164 6174 612e 7661   ((self.adata.va
+000039d0: 725b 226d 6973 7369 6e67 6e65 7373 225d  r["missingness"]
+000039e0: 203e 2030 2920 7c0d 0a20 2020 2020 2020   > 0) |..       
 000039f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a00: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
-00003a10: 6174 612e 7661 725b 226c 6f67 5f6d 6561  ata.var["log_mea
-00003a20: 6e22 5d2e 6973 6e75 6c6c 2829 207c 0d0a  n"].isnull() |..
-00003a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a10: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+00003a20: 612e 7661 725b 226c 6f67 5f6d 6561 6e22  a.var["log_mean"
+00003a30: 5d2e 6973 6e75 6c6c 2829 207c 0d0a 2020  ].isnull() |..  
 00003a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003a50: 2020 2020 2020 2020 2020 2020 2020 2873                (s
-00003a60: 656c 662e 6164 6174 612e 7661 725b 226d  elf.adata.var["m
-00003a70: 6561 6e22 5d20 3d3d 2030 2920 7c0d 0a20  ean"] == 0) |.. 
-00003a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003a60: 2020 2020 2020 2020 2020 2020 2873 656c              (sel
+00003a70: 662e 6164 6174 612e 7661 725b 226d 6561  f.adata.var["mea
+00003a80: 6e22 5d20 3d3d 2030 2920 7c0d 0a20 2020  n"] == 0) |..   
 00003a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003aa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-00003ab0: 662e 6164 6174 612e 7661 725b 226c 6f67  f.adata.var["log
-00003ac0: 5f76 6172 6961 6e63 6522 5d2e 6973 6e75  _variance"].isnu
-00003ad0: 6c6c 2829 290d 0a0d 0a20 2020 2020 2020  ll())....       
-00003ae0: 2023 206d 6f64 656c 206d 6561 6e2d 7661   # model mean-va
-00003af0: 7269 616e 6365 2072 656c 6174 696f 6e73  riance relations
-00003b00: 6869 7020 7573 696e 6720 6765 6e65 7261  hip using genera
-00003b10: 6c69 7a65 6420 6164 6469 7469 7665 206d  lized additive m
-00003b20: 6f64 656c 2077 6974 6820 736d 6f6f 7468  odel with smooth
-00003b30: 2063 6f6d 706f 6e65 6e74 730d 0a20 2020   components..   
-00003b40: 2020 2020 2064 665f 6d6f 6465 6c20 3d20       df_model = 
-00003b50: 7365 6c66 2e61 6461 7461 2e76 6172 5b7e  self.adata.var[~
-00003b60: 7365 6c66 2e61 6461 7461 2e76 6172 5b22  self.adata.var["
-00003b70: 6f64 7363 6f72 655f 6578 636c 7564 6564  odscore_excluded
-00003b80: 225d 5d0d 0a20 2020 2020 2020 2062 7320  "]]..        bs 
-00003b90: 3d20 4253 706c 696e 6573 2864 665f 6d6f  = BSplines(df_mo
-00003ba0: 6465 6c5b 226d 6561 6e22 5d2c 2064 663d  del["mean"], df=
-00003bb0: 6f64 675f 6465 6661 756c 745f 646f 662c  odg_default_dof,
-00003bc0: 2064 6567 7265 653d 6f64 675f 6465 6661   degree=odg_defa
-00003bd0: 756c 745f 7370 6c69 6e65 5f64 6567 7265  ult_spline_degre
-00003be0: 6529 0d0a 2020 2020 2020 2020 6761 6d20  e)..        gam 
-00003bf0: 3d20 474c 4d47 616d 2e66 726f 6d5f 666f  = GLMGam.from_fo
-00003c00: 726d 756c 6128 226c 6f67 5f76 6172 6961  rmula("log_varia
-00003c10: 6e63 6520 7e20 6c6f 675f 6d65 616e 222c  nce ~ log_mean",
-00003c20: 2064 6174 613d 6466 5f6d 6f64 656c 2c20   data=df_model, 
-00003c30: 736d 6f6f 7468 6572 3d62 7329 2e66 6974  smoother=bs).fit
-00003c40: 2829 0d0a 2020 2020 2020 2020 7365 6c66  ()..        self
-00003c50: 2e61 6461 7461 2e76 6172 5b22 7265 7369  .adata.var["resi
-00003c60: 645f 6c6f 675f 7661 7269 616e 6365 225d  d_log_variance"]
-00003c70: 203d 2067 616d 2e72 6573 6964 5f72 6573   = gam.resid_res
-00003c80: 706f 6e73 650d 0a20 2020 2020 2020 2073  ponse..        s
-00003c90: 656c 662e 6164 6174 612e 7661 725b 226f  elf.adata.var["o
-00003ca0: 6473 636f 7265 225d 203d 206e 702e 7371  dscore"] = np.sq
-00003cb0: 7274 2831 3020 2a2a 2073 656c 662e 6164  rt(10 ** self.ad
-00003cc0: 6174 612e 7661 725b 2272 6573 6964 5f6c  ata.var["resid_l
-00003cd0: 6f67 5f76 6172 6961 6e63 6522 5d29 0d0a  og_variance"])..
-00003ce0: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
-00003cf0: 7461 2e76 6172 5b22 6761 6d5f 6669 7474  ta.var["gam_fitt
-00003d00: 6564 7661 6c75 6573 225d 203d 2067 616d  edvalues"] = gam
-00003d10: 2e66 6974 7465 6476 616c 7565 730d 0a0d  .fittedvalues...
-00003d20: 0a0d 0a20 2020 2020 2020 2023 206d 6f64  ...        # mod
-00003d30: 656c 206d 6561 6e2d 7661 7269 616e 6365  el mean-variance
-00003d40: 2072 656c 6174 696f 6e73 6869 7020 7573   relationship us
-00003d50: 696e 6720 634e 4d46 2773 206d 6574 686f  ing cNMF's metho
-00003d60: 6420 6261 7365 6420 6f6e 2076 2d73 636f  d based on v-sco
-00003d70: 7265 2061 6e64 206d 696e 696d 756d 2065  re and minimum e
-00003d80: 7870 7265 7373 696f 6e20 7468 7265 7368  xpression thresh
-00003d90: 6f6c 640d 0a20 2020 2020 2020 2076 7363  old..        vsc
-00003da0: 6f72 655f 7374 6174 7320 3d20 7064 2e44  ore_stats = pd.D
-00003db0: 6174 6146 7261 6d65 2863 6e6d 662e 6765  ataFrame(cnmf.ge
-00003dc0: 745f 6869 6768 7661 725f 6765 6e65 7328  t_highvar_genes(
-00003dd0: 696e 7075 745f 636f 756e 7473 3d64 6174  input_counts=dat
-00003de0: 615f 6e6f 726d 616c 697a 6564 2e76 616c  a_normalized.val
-00003df0: 7565 732c 206d 696e 696d 616c 5f6d 6561  ues, minimal_mea
-00003e00: 6e3d 3029 5b30 5d29 0d0a 2020 2020 2020  n=0)[0])..      
-00003e10: 2020 7673 636f 7265 5f73 7461 7473 2e69    vscore_stats.i
-00003e20: 6e64 6578 203d 2064 6174 615f 6e6f 726d  ndex = data_norm
-00003e30: 616c 697a 6564 2e63 6f6c 756d 6e73 0d0a  alized.columns..
-00003e40: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
-00003e50: 7461 2e76 6172 5b22 7673 636f 7265 225d  ta.var["vscore"]
-00003e60: 203d 2076 7363 6f72 655f 7374 6174 735b   = vscore_stats[
-00003e70: 2266 616e 6f5f 7261 7469 6f22 5d0d 0a20  "fano_ratio"].. 
-00003e80: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-00003e90: 612e 756e 735b 226f 6467 225d 5b22 6f64  a.uns["odg"]["od
-00003ea0: 675f 6465 6661 756c 745f 7370 6c69 6e65  g_default_spline
-00003eb0: 5f64 6567 7265 6522 5d20 3d20 6f64 675f  _degree"] = odg_
-00003ec0: 6465 6661 756c 745f 7370 6c69 6e65 5f64  default_spline_d
-00003ed0: 6567 7265 650d 0a20 2020 2020 2020 2073  egree..        s
-00003ee0: 656c 662e 6164 6174 612e 756e 735b 226f  elf.adata.uns["o
-00003ef0: 6467 225d 5b22 6f64 675f 6465 6661 756c  dg"]["odg_defaul
-00003f00: 745f 646f 6622 5d20 3d20 6f64 675f 6465  t_dof"] = odg_de
-00003f10: 6661 756c 745f 646f 660d 0a20 2020 2020  fault_dof..     
-00003f20: 2020 2073 656c 662e 6170 7065 6e64 5f74     self.append_t
-00003f30: 6f5f 6869 7374 6f72 7928 2247 656e 652d  o_history("Gene-
-00003f40: 6c65 7665 6c20 7374 6174 6973 7469 6373  level statistics
-00003f50: 2061 6e64 206f 7665 7264 6973 7065 7273   and overdispers
-00003f60: 696f 6e20 6d6f 6465 6c6c 696e 6720 636f  ion modelling co
-00003f70: 6d70 6c65 7465 642e 2229 0d0a 2020 2020  mpleted.")..    
-00003f80: 2020 2020 0d0a 2020 2020 6465 6620 7365      ..    def se
-00003f90: 6c65 6374 5f6f 7665 7264 6973 7065 7273  lect_overdispers
-00003fa0: 6564 5f67 656e 6573 5f66 726f 6d5f 6765  ed_genes_from_ge
-00003fb0: 6e65 6c69 7374 2873 656c 662c 2067 656e  nelist(self, gen
-00003fc0: 6573 3a20 436f 6c6c 6563 7469 6f6e 2c20  es: Collection, 
-00003fd0: 6d69 6e5f 6d65 616e 3d30 293a 0d0a 2020  min_mean=0):..  
-00003fe0: 2020 2020 2020 2222 2253 656c 6563 7420        """Select 
-00003ff0: 6f76 6572 6469 7370 6572 7365 6420 6765  overdispersed ge
-00004000: 6e65 732f 6665 6174 7572 6573 2075 7369  nes/features usi
-00004010: 6e67 2061 2063 7573 746f 6d20 6c69 7374  ng a custom list
-00004020: 2e20 4765 6e65 732f 6665 6174 7572 6573  . Genes/features
-00004030: 206e 6f74 2070 7265 7365 6e74 2069 6e20   not present in 
-00004040: 7468 6520 6461 7461 7365 7420 6172 6520  the dataset are 
-00004050: 6175 746f 6d61 7469 6361 6c6c 7920 6669  automatically fi
-00004060: 6c74 6572 6564 206f 7574 2e0d 0a0d 0a20  ltered out..... 
-00004070: 2020 2020 2020 203a 7061 7261 6d20 6765         :param ge
-00004080: 6e65 733a 2067 656e 6520 6c69 7374 0d0a  nes: gene list..
-00004090: 2020 2020 2020 2020 3a74 7970 6520 6765          :type ge
-000040a0: 6e65 733a 2043 6f6c 6c65 6374 696f 6e0d  nes: Collection.
-000040b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000040c0: 6d69 6e5f 6d65 616e 3a20 6d69 6e69 6d75  min_mean: minimu
-000040d0: 6d20 6765 6e65 2065 7870 7265 7373 696f  m gene expressio
-000040e0: 6e20 666f 7220 6765 6e65 7320 746f 2062  n for genes to b
-000040f0: 6520 636f 756e 7465 6420 6173 206f 7665  e counted as ove
-00004100: 7264 6973 7065 7273 6564 2c20 6465 6661  rdispersed, defa
-00004110: 756c 7473 2074 6f20 300d 0a20 2020 2020  ults to 0..     
-00004120: 2020 203a 7479 7065 206d 696e 5f6d 6561     :type min_mea
-00004130: 6e3a 2069 6e74 2c20 6f70 7469 6f6e 616c  n: int, optional
-00004140: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-00004150: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-00004160: 612e 7661 725b 2273 656c 6563 7465 6422  a.var["selected"
-00004170: 5d20 3d20 7365 6c66 2e61 6461 7461 2e76  ] = self.adata.v
-00004180: 6172 2e69 6e64 6578 2e69 7369 6e28 6765  ar.index.isin(ge
-00004190: 6e65 7329 2026 2073 656c 662e 6164 6174  nes) & self.adat
-000041a0: 612e 7661 725b 226d 6561 6e5f 636f 756e  a.var["mean_coun
-000041b0: 7473 225d 203e 3d20 6d69 6e5f 6d65 616e  ts"] >= min_mean
-000041c0: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
-000041d0: 6461 7461 2e75 6e73 5b22 6f64 6722 5d5b  data.uns["odg"][
-000041e0: 226f 7665 7264 6973 7065 7273 696f 6e5f  "overdispersion_
-000041f0: 6d65 7472 6963 225d 203d 2022 220d 0a20  metric"] = "".. 
-00004200: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-00004210: 612e 756e 735b 226f 6467 225d 5b22 6d69  a.uns["odg"]["mi
-00004220: 6e5f 6d65 616e 225d 203d 206d 696e 5f6d  n_mean"] = min_m
-00004230: 6561 6e0d 0a20 2020 2020 2020 2073 656c  ean..        sel
-00004240: 662e 6164 6174 612e 756e 735b 226f 6467  f.adata.uns["odg
-00004250: 225d 5b22 6d69 6e5f 7363 6f72 6522 5d20  "]["min_score"] 
-00004260: 3d20 2222 0d0a 2020 2020 2020 2020 7365  = ""..        se
-00004270: 6c66 2e61 6461 7461 2e75 6e73 5b22 6f64  lf.adata.uns["od
-00004280: 6722 5d5b 2274 6f70 5f6e 225d 203d 2022  g"]["top_n"] = "
-00004290: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-000042a0: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
-000042b0: 5b22 7175 616e 7469 6c65 225d 203d 2022  ["quantile"] = "
-000042c0: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
-000042d0: 6170 7065 6e64 5f74 6f5f 6869 7374 6f72  append_to_histor
-000042e0: 7928 224f 7665 7264 6973 7065 7273 6564  y("Overdispersed
-000042f0: 2067 656e 6573 2073 656c 6563 7465 6420   genes selected 
-00004300: 6672 6f6d 2063 7573 746f 6d20 6765 6e65  from custom gene
-00004310: 206c 6973 7422 290d 0a20 2020 2020 2020   list")..       
-00004320: 200d 0a20 2020 2064 6566 2073 656c 6563   ..    def selec
-00004330: 745f 6f76 6572 6469 7370 6572 7365 645f  t_overdispersed_
-00004340: 6765 6e65 7328 7365 6c66 2c0d 0a20 2020  genes(self,..   
-00004350: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ab0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003ac0: 6164 6174 612e 7661 725b 226c 6f67 5f76  adata.var["log_v
+00003ad0: 6172 6961 6e63 6522 5d2e 6973 6e75 6c6c  ariance"].isnull
+00003ae0: 2829 290d 0a0d 0a20 2020 2020 2020 2023  ())....        #
+00003af0: 206d 6f64 656c 206d 6561 6e2d 7661 7269   model mean-vari
+00003b00: 616e 6365 2072 656c 6174 696f 6e73 6869  ance relationshi
+00003b10: 7020 7573 696e 6720 6765 6e65 7261 6c69  p using generali
+00003b20: 7a65 6420 6164 6469 7469 7665 206d 6f64  zed additive mod
+00003b30: 656c 2077 6974 6820 736d 6f6f 7468 2063  el with smooth c
+00003b40: 6f6d 706f 6e65 6e74 730d 0a20 2020 2020  omponents..     
+00003b50: 2020 2064 665f 6d6f 6465 6c20 3d20 7365     df_model = se
+00003b60: 6c66 2e61 6461 7461 2e76 6172 5b7e 7365  lf.adata.var[~se
+00003b70: 6c66 2e61 6461 7461 2e76 6172 5b22 6f64  lf.adata.var["od
+00003b80: 7363 6f72 655f 6578 636c 7564 6564 225d  score_excluded"]
+00003b90: 5d0d 0a20 2020 2020 2020 2062 7320 3d20  ]..        bs = 
+00003ba0: 4253 706c 696e 6573 2864 665f 6d6f 6465  BSplines(df_mode
+00003bb0: 6c5b 226d 6561 6e22 5d2c 2064 663d 6f64  l["mean"], df=od
+00003bc0: 675f 6465 6661 756c 745f 646f 662c 2064  g_default_dof, d
+00003bd0: 6567 7265 653d 6f64 675f 6465 6661 756c  egree=odg_defaul
+00003be0: 745f 7370 6c69 6e65 5f64 6567 7265 6529  t_spline_degree)
+00003bf0: 0d0a 2020 2020 2020 2020 6761 6d20 3d20  ..        gam = 
+00003c00: 474c 4d47 616d 2e66 726f 6d5f 666f 726d  GLMGam.from_form
+00003c10: 756c 6128 226c 6f67 5f76 6172 6961 6e63  ula("log_varianc
+00003c20: 6520 7e20 6c6f 675f 6d65 616e 222c 2064  e ~ log_mean", d
+00003c30: 6174 613d 6466 5f6d 6f64 656c 2c20 736d  ata=df_model, sm
+00003c40: 6f6f 7468 6572 3d62 7329 2e66 6974 2829  oother=bs).fit()
+00003c50: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00003c60: 6461 7461 2e76 6172 5b22 7265 7369 645f  data.var["resid_
+00003c70: 6c6f 675f 7661 7269 616e 6365 225d 203d  log_variance"] =
+00003c80: 2067 616d 2e72 6573 6964 5f72 6573 706f   gam.resid_respo
+00003c90: 6e73 650d 0a20 2020 2020 2020 2073 656c  nse..        sel
+00003ca0: 662e 6164 6174 612e 7661 725b 226f 6473  f.adata.var["ods
+00003cb0: 636f 7265 225d 203d 206e 702e 7371 7274  core"] = np.sqrt
+00003cc0: 2831 3020 2a2a 2073 656c 662e 6164 6174  (10 ** self.adat
+00003cd0: 612e 7661 725b 2272 6573 6964 5f6c 6f67  a.var["resid_log
+00003ce0: 5f76 6172 6961 6e63 6522 5d29 0d0a 2020  _variance"])..  
+00003cf0: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+00003d00: 2e76 6172 5b22 6761 6d5f 6669 7474 6564  .var["gam_fitted
+00003d10: 7661 6c75 6573 225d 203d 2067 616d 2e66  values"] = gam.f
+00003d20: 6974 7465 6476 616c 7565 730d 0a0d 0a0d  ittedvalues.....
+00003d30: 0a20 2020 2020 2020 2023 206d 6f64 656c  .        # model
+00003d40: 206d 6561 6e2d 7661 7269 616e 6365 2072   mean-variance r
+00003d50: 656c 6174 696f 6e73 6869 7020 7573 696e  elationship usin
+00003d60: 6720 634e 4d46 2773 206d 6574 686f 6420  g cNMF's method 
+00003d70: 6261 7365 6420 6f6e 2076 2d73 636f 7265  based on v-score
+00003d80: 2061 6e64 206d 696e 696d 756d 2065 7870   and minimum exp
+00003d90: 7265 7373 696f 6e20 7468 7265 7368 6f6c  ression threshol
+00003da0: 640d 0a20 2020 2020 2020 2076 7363 6f72  d..        vscor
+00003db0: 655f 7374 6174 7320 3d20 7064 2e44 6174  e_stats = pd.Dat
+00003dc0: 6146 7261 6d65 2863 6e6d 662e 6765 745f  aFrame(cnmf.get_
+00003dd0: 6869 6768 7661 725f 6765 6e65 7328 696e  highvar_genes(in
+00003de0: 7075 745f 636f 756e 7473 3d64 6174 615f  put_counts=data_
+00003df0: 6e6f 726d 616c 697a 6564 2e76 616c 7565  normalized.value
+00003e00: 732c 206d 696e 696d 616c 5f6d 6561 6e3d  s, minimal_mean=
+00003e10: 3029 5b30 5d29 0d0a 2020 2020 2020 2020  0)[0])..        
+00003e20: 7673 636f 7265 5f73 7461 7473 2e69 6e64  vscore_stats.ind
+00003e30: 6578 203d 2064 6174 615f 6e6f 726d 616c  ex = data_normal
+00003e40: 697a 6564 2e63 6f6c 756d 6e73 0d0a 2020  ized.columns..  
+00003e50: 2020 2020 2020 7365 6c66 2e61 6461 7461        self.adata
+00003e60: 2e76 6172 5b22 7673 636f 7265 225d 203d  .var["vscore"] =
+00003e70: 2076 7363 6f72 655f 7374 6174 735b 2266   vscore_stats["f
+00003e80: 616e 6f5f 7261 7469 6f22 5d0d 0a20 2020  ano_ratio"]..   
+00003e90: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00003ea0: 756e 735b 226f 6467 225d 5b22 6f64 675f  uns["odg"]["odg_
+00003eb0: 6465 6661 756c 745f 7370 6c69 6e65 5f64  default_spline_d
+00003ec0: 6567 7265 6522 5d20 3d20 6f64 675f 6465  egree"] = odg_de
+00003ed0: 6661 756c 745f 7370 6c69 6e65 5f64 6567  fault_spline_deg
+00003ee0: 7265 650d 0a20 2020 2020 2020 2073 656c  ree..        sel
+00003ef0: 662e 6164 6174 612e 756e 735b 226f 6467  f.adata.uns["odg
+00003f00: 225d 5b22 6f64 675f 6465 6661 756c 745f  "]["odg_default_
+00003f10: 646f 6622 5d20 3d20 6f64 675f 6465 6661  dof"] = odg_defa
+00003f20: 756c 745f 646f 660d 0a20 2020 2020 2020  ult_dof..       
+00003f30: 2073 656c 662e 6170 7065 6e64 5f74 6f5f   self.append_to_
+00003f40: 6869 7374 6f72 7928 2247 656e 652d 6c65  history("Gene-le
+00003f50: 7665 6c20 7374 6174 6973 7469 6373 2061  vel statistics a
+00003f60: 6e64 206f 7665 7264 6973 7065 7273 696f  nd overdispersio
+00003f70: 6e20 6d6f 6465 6c6c 696e 6720 636f 6d70  n modelling comp
+00003f80: 6c65 7465 642e 2229 0d0a 2020 2020 2020  leted.")..      
+00003f90: 2020 0d0a 2020 2020 6465 6620 7365 6c65    ..    def sele
+00003fa0: 6374 5f6f 7665 7264 6973 7065 7273 6564  ct_overdispersed
+00003fb0: 5f67 656e 6573 5f66 726f 6d5f 6765 6e65  _genes_from_gene
+00003fc0: 6c69 7374 2873 656c 662c 2067 656e 6573  list(self, genes
+00003fd0: 3a20 436f 6c6c 6563 7469 6f6e 2c20 6d69  : Collection, mi
+00003fe0: 6e5f 6d65 616e 3d30 293a 0d0a 2020 2020  n_mean=0):..    
+00003ff0: 2020 2020 2222 2253 656c 6563 7420 6f76      """Select ov
+00004000: 6572 6469 7370 6572 7365 6420 6765 6e65  erdispersed gene
+00004010: 732f 6665 6174 7572 6573 2075 7369 6e67  s/features using
+00004020: 2061 2063 7573 746f 6d20 6c69 7374 2e20   a custom list. 
+00004030: 4765 6e65 732f 6665 6174 7572 6573 206e  Genes/features n
+00004040: 6f74 2070 7265 7365 6e74 2069 6e20 7468  ot present in th
+00004050: 6520 6461 7461 7365 7420 6172 6520 6175  e dataset are au
+00004060: 746f 6d61 7469 6361 6c6c 7920 6669 6c74  tomatically filt
+00004070: 6572 6564 206f 7574 2e0d 0a0d 0a20 2020  ered out.....   
+00004080: 2020 2020 203a 7061 7261 6d20 6765 6e65       :param gene
+00004090: 733a 2067 656e 6520 6c69 7374 0d0a 2020  s: gene list..  
+000040a0: 2020 2020 2020 3a74 7970 6520 6765 6e65        :type gene
+000040b0: 733a 2043 6f6c 6c65 6374 696f 6e0d 0a20  s: Collection.. 
+000040c0: 2020 2020 2020 203a 7061 7261 6d20 6d69         :param mi
+000040d0: 6e5f 6d65 616e 3a20 6d69 6e69 6d75 6d20  n_mean: minimum 
+000040e0: 6765 6e65 2065 7870 7265 7373 696f 6e20  gene expression 
+000040f0: 666f 7220 6765 6e65 7320 746f 2062 6520  for genes to be 
+00004100: 636f 756e 7465 6420 6173 206f 7665 7264  counted as overd
+00004110: 6973 7065 7273 6564 2c20 6465 6661 756c  ispersed, defaul
+00004120: 7473 2074 6f20 300d 0a20 2020 2020 2020  ts to 0..       
+00004130: 203a 7479 7065 206d 696e 5f6d 6561 6e3a   :type min_mean:
+00004140: 2069 6e74 2c20 6f70 7469 6f6e 616c 0d0a   int, optional..
+00004150: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00004160: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00004170: 7661 725b 2273 656c 6563 7465 6422 5d20  var["selected"] 
+00004180: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
+00004190: 2e69 6e64 6578 2e69 7369 6e28 6765 6e65  .index.isin(gene
+000041a0: 7329 2026 2073 656c 662e 6164 6174 612e  s) & self.adata.
+000041b0: 7661 725b 226d 6561 6e5f 636f 756e 7473  var["mean_counts
+000041c0: 225d 203e 3d20 6d69 6e5f 6d65 616e 0d0a  "] >= min_mean..
+000041d0: 2020 2020 2020 2020 7365 6c66 2e61 6461          self.ada
+000041e0: 7461 2e75 6e73 5b22 6f64 6722 5d5b 226f  ta.uns["odg"]["o
+000041f0: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
+00004200: 7472 6963 225d 203d 2022 220d 0a20 2020  tric"] = ""..   
+00004210: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00004220: 756e 735b 226f 6467 225d 5b22 6d69 6e5f  uns["odg"]["min_
+00004230: 6d65 616e 225d 203d 206d 696e 5f6d 6561  mean"] = min_mea
+00004240: 6e0d 0a20 2020 2020 2020 2073 656c 662e  n..        self.
+00004250: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
+00004260: 5b22 6d69 6e5f 7363 6f72 6522 5d20 3d20  ["min_score"] = 
+00004270: 2222 0d0a 2020 2020 2020 2020 7365 6c66  ""..        self
+00004280: 2e61 6461 7461 2e75 6e73 5b22 6f64 6722  .adata.uns["odg"
+00004290: 5d5b 2274 6f70 5f6e 225d 203d 2022 220d  ]["top_n"] = "".
+000042a0: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+000042b0: 6174 612e 756e 735b 226f 6467 225d 5b22  ata.uns["odg"]["
+000042c0: 7175 616e 7469 6c65 225d 203d 2022 220d  quantile"] = "".
+000042d0: 0a20 2020 2020 2020 2073 656c 662e 6170  .        self.ap
+000042e0: 7065 6e64 5f74 6f5f 6869 7374 6f72 7928  pend_to_history(
+000042f0: 224f 7665 7264 6973 7065 7273 6564 2067  "Overdispersed g
+00004300: 656e 6573 2073 656c 6563 7465 6420 6672  enes selected fr
+00004310: 6f6d 2063 7573 746f 6d20 6765 6e65 206c  om custom gene l
+00004320: 6973 7422 290d 0a20 2020 2020 2020 200d  ist")..        .
+00004330: 0a20 2020 2064 6566 2073 656c 6563 745f  .    def select_
+00004340: 6f76 6572 6469 7370 6572 7365 645f 6765  overdispersed_ge
+00004350: 6e65 7328 7365 6c66 2c0d 0a20 2020 2020  nes(self,..     
 00004360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004370: 6f76 6572 6469 7370 6572 7369 6f6e 5f6d  overdispersion_m
-00004380: 6574 7269 633a 2073 7472 203d 2022 6f64  etric: str = "od
-00004390: 7363 6f72 6522 2c0d 0a20 2020 2020 2020  score",..       
-000043a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043b0: 2020 2020 2020 2020 2020 2020 6d69 6e5f              min_
-000043c0: 6d65 616e 3a20 666c 6f61 7420 3d20 302c  mean: float = 0,
-000043d0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004370: 2020 2020 2020 2020 2020 2020 2020 6f76                ov
+00004380: 6572 6469 7370 6572 7369 6f6e 5f6d 6574  erdispersion_met
+00004390: 7269 633a 2073 7472 203d 2022 6f64 7363  ric: str = "odsc
+000043a0: 6f72 6522 2c0d 0a20 2020 2020 2020 2020  ore",..         
+000043b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043c0: 2020 2020 2020 2020 2020 6d69 6e5f 6d65            min_me
+000043d0: 616e 3a20 666c 6f61 7420 3d20 302c 0d0a  an: float = 0,..
 000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000043f0: 2020 2020 206d 696e 5f73 636f 7265 3a20       min_score: 
-00004400: 666c 6f61 7420 3d20 312e 302c 0d0a 2020  float = 1.0,..  
-00004410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004400: 2020 206d 696e 5f73 636f 7265 3a20 666c     min_score: fl
+00004410: 6f61 7420 3d20 312e 302c 0d0a 2020 2020  oat = 1.0,..    
 00004420: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004430: 2074 6f70 5f6e 3a20 696e 7420 3d20 4e6f   top_n: int = No
-00004440: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
-00004450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004460: 2020 2020 2020 2020 7175 616e 7469 6c65          quantile
-00004470: 3a20 666c 6f61 7420 3d20 4e6f 6e65 293a  : float = None):
-00004480: 0d0a 2020 2020 2020 2020 2222 2253 656c  ..        """Sel
-00004490: 6563 7420 6f76 6572 6469 7370 6572 7365  ect overdisperse
-000044a0: 6420 6765 6e65 732f 6665 6174 7572 6573  d genes/features
-000044b0: 2075 7369 6e67 2061 6e20 6f76 6572 6469   using an overdi
-000044c0: 7370 6572 7369 6f6e 206d 6574 7269 632e  spersion metric.
-000044d0: 204f 7074 696f 6e61 6c6c 7920 7365 7420   Optionally set 
-000044e0: 6120 6d69 6e69 6d75 6d20 6765 6e65 2065  a minimum gene e
-000044f0: 7870 7265 7373 696f 6e20 6c65 7665 6c2e  xpression level.
-00004500: 0d0a 2020 2020 2020 2020 5365 7420 6120  ..        Set a 
-00004510: 7468 7265 7368 6f6c 6420 7573 696e 6720  threshold using 
-00004520: 7468 6520 746f 7020 4e20 2827 746f 705f  the top N ('top_
-00004530: 6e27 292c 206d 696e 696d 756d 2073 636f  n'), minimum sco
-00004540: 7265 2028 276d 696e 5f73 636f 7265 2729  re ('min_score')
-00004550: 2c20 6f72 2070 726f 706f 7274 696f 6e20  , or proportion 
-00004560: 6f66 2066 6561 7475 7265 7320 2827 7175  of features ('qu
-00004570: 616e 7469 6c65 2729 206d 6574 686f 6473  antile') methods
-00004580: 2e0d 0a20 2020 2020 2020 204f 7665 7264  ...        Overd
-00004590: 6973 7065 7273 6564 2067 656e 6520 6c69  ispersed gene li
-000045a0: 7374 2069 7320 7361 7665 6420 696e 2074  st is saved in t
-000045b0: 6865 2044 6174 6173 6574 206f 626a 6563  he Dataset objec
-000045c0: 742e 0d0a 0d0a 2020 2020 2020 2020 3a70  t.....        :p
-000045d0: 6172 616d 206f 7665 7264 6973 7065 7273  aram overdispers
-000045e0: 696f 6e5f 6d65 7472 6963 3a20 226f 6473  ion_metric: "ods
-000045f0: 636f 7265 2220 6f72 2022 7673 636f 7265  core" or "vscore
-00004600: 222c 2064 6566 6175 6c74 7320 746f 2022  ", defaults to "
-00004610: 6f64 7363 6f72 6522 0d0a 2020 2020 2020  odscore"..      
-00004620: 2020 3a74 7970 6520 6f76 6572 6469 7370    :type overdisp
-00004630: 6572 7369 6f6e 5f6d 6574 7269 633a 2073  ersion_metric: s
-00004640: 7472 2c20 6f70 7469 6f6e 616c 0d0a 2020  tr, optional..  
-00004650: 2020 2020 2020 3a70 6172 616d 206d 696e        :param min
-00004660: 5f6d 6561 6e3a 206d 696e 696d 756d 2067  _mean: minimum g
-00004670: 656e 6520 6578 7072 6573 7369 6f6e 2066  ene expression f
-00004680: 6f72 2067 656e 6573 2074 6f20 6265 2063  or genes to be c
-00004690: 6f75 6e74 6564 2061 7320 6f76 6572 6469  ounted as overdi
-000046a0: 7370 6572 7365 642c 2064 6566 6175 6c74  spersed, default
-000046b0: 7320 746f 2030 0d0a 2020 2020 2020 2020  s to 0..        
-000046c0: 3a74 7970 6520 6d69 6e5f 6d65 616e 3a20  :type min_mean: 
-000046d0: 696e 742c 206f 7074 696f 6e61 6c0d 0a20  int, optional.. 
-000046e0: 2020 2020 2020 203a 7061 7261 6d20 6d69         :param mi
-000046f0: 6e5f 7363 6f72 653a 206d 696e 696d 756d  n_score: minimum
-00004700: 2073 636f 7265 2066 6f72 206f 7665 7264   score for overd
-00004710: 6973 7065 7273 696f 6e2c 2064 6566 6175  ispersion, defau
-00004720: 6c74 7320 746f 2031 2e30 0d0a 2020 2020  lts to 1.0..    
-00004730: 2020 2020 3a74 7970 6520 6d69 6e5f 7363      :type min_sc
-00004740: 6f72 653a 2066 6c6f 6174 2c20 6f70 7469  ore: float, opti
-00004750: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
-00004760: 6172 616d 2074 6f70 5f6e 3a20 4368 6f6f  aram top_n: Choo
-00004770: 7365 2074 6865 2074 6f70 204e 206d 6f73  se the top N mos
-00004780: 7420 6f76 6572 6469 7370 6572 7365 6420  t overdispersed 
-00004790: 6765 6e65 732c 2064 6566 6175 6c74 7320  genes, defaults 
-000047a0: 746f 204e 6f6e 650d 0a20 2020 2020 2020  to None..       
-000047b0: 203a 7479 7065 2074 6f70 5f6e 3a20 696e   :type top_n: in
-000047c0: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
-000047d0: 2020 2020 203a 7061 7261 6d20 7175 616e       :param quan
-000047e0: 7469 6c65 3a20 4368 6f6f 7365 2061 2071  tile: Choose a q
-000047f0: 7561 6e74 696c 6520 6f66 206f 7665 7264  uantile of overd
-00004800: 6973 7065 7273 696f 6e2e 2046 6f72 2065  ispersion. For e
-00004810: 7861 6d70 6c65 2c20 7468 6520 746f 7020  xample, the top 
-00004820: 3130 2520 6f66 206f 7665 7264 6973 7065  10% of overdispe
-00004830: 7273 6564 2067 656e 6573 2077 6f75 6c64  rsed genes would
-00004840: 2062 6520 302e 3130 2e20 4465 6661 756c   be 0.10. Defaul
-00004850: 7473 2074 6f20 4e6f 6e65 0d0a 2020 2020  ts to None..    
-00004860: 2020 2020 3a74 7970 6520 7175 616e 7469      :type quanti
-00004870: 6c65 3a20 666c 6f61 742c 206f 7074 696f  le: float, optio
-00004880: 6e61 6c0d 0a20 2020 2020 2020 203a 7261  nal..        :ra
-00004890: 6973 6573 2056 616c 7565 4572 726f 723a  ises ValueError:
-000048a0: 2045 7272 6f72 2069 6620 696e 7661 6c69   Error if invali
-000048b0: 6420 6f76 6572 6469 7370 6572 7369 6f6e  d overdispersion
-000048c0: 206d 6574 7269 6320 6973 2063 686f 7365   metric is chose
-000048d0: 6e2e 0d0a 2020 2020 2020 2020 2222 220d  n...        """.
-000048e0: 0a20 2020 2020 2020 200d 0a20 2020 2020  .        ..     
-000048f0: 2020 2069 6620 6f76 6572 6469 7370 6572     if overdisper
-00004900: 7369 6f6e 5f6d 6574 7269 6320 6e6f 7420  sion_metric not 
-00004910: 696e 2073 656c 662e 6164 6174 612e 7661  in self.adata.va
-00004920: 722e 636f 6c75 6d6e 733a 0d0a 2020 2020  r.columns:..    
-00004930: 2020 2020 2020 2020 6966 206f 7665 7264          if overd
-00004940: 6973 7065 7273 696f 6e5f 6d65 7472 6963  ispersion_metric
-00004950: 2069 6e20 2822 6f64 7363 6f72 6522 2c20   in ("odscore", 
-00004960: 2276 7363 6f72 6522 293a 0d0a 2020 2020  "vscore"):..    
-00004970: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-00004980: 6520 5661 6c75 6545 7272 6f72 280d 0a20  e ValueError(.. 
-00004990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049a0: 2020 2066 227b 6f76 6572 6469 7370 6572     f"{overdisper
-000049b0: 7369 6f6e 5f6d 6574 7269 637d 2068 6173  sion_metric} has
-000049c0: 206e 6f74 2062 6565 6e20 6361 6c63 756c   not been calcul
-000049d0: 6174 6564 2066 6f72 2074 6869 7320 6461  ated for this da
-000049e0: 7461 7365 742e 2022 0d0a 2020 2020 2020  taset. "..      
-000049f0: 2020 2020 2020 2020 2020 2020 2020 2245                "E
-00004a00: 6e73 7572 6520 7468 6174 2079 6f75 2063  nsure that you c
-00004a10: 616c 6c20 7468 6520 6044 6174 6173 6574  all the `Dataset
-00004a20: 2e63 6f6d 7075 7465 5f67 656e 655f 7374  .compute_gene_st
-00004a30: 6174 7328 2960 2066 6972 7374 2e22 0d0a  ats()` first."..
-00004a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a50: 2020 2020 290d 0a20 2020 2020 2020 2020      )..         
-00004a60: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
-00004a70: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00004a80: 5661 6c75 6545 7272 6f72 280d 0a20 2020  ValueError(..   
-00004a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004aa0: 2066 227b 6f76 6572 6469 7370 6572 7369   f"{overdispersi
-00004ab0: 6f6e 5f6d 6574 7269 637d 2069 7320 6e6f  on_metric} is no
-00004ac0: 7420 6120 7661 6c69 6420 6f76 6572 6469  t a valid overdi
-00004ad0: 7370 6572 7369 6f6e 206d 6574 7269 632e  spersion metric.
-00004ae0: 220d 0a20 2020 2020 2020 2020 2020 2020  "..             
-00004af0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-00004b00: 2020 0d0a 2020 2020 2020 2020 2320 7761    ..        # wa
-00004b10: 726e 2069 6620 6d75 6c74 6970 6c65 206d  rn if multiple m
-00004b20: 6574 686f 6473 2061 7265 2073 656c 6563  ethods are selec
-00004b30: 7465 640d 0a20 2020 2020 2020 2073 656c  ted..        sel
-00004b40: 6563 7465 645f 6d65 7468 6f64 7320 3d20  ected_methods = 
-00004b50: 5b5d 0d0a 2020 2020 2020 2020 6966 206d  []..        if m
-00004b60: 696e 5f73 636f 7265 2069 7320 6e6f 7420  in_score is not 
-00004b70: 4e6f 6e65 3a0d 0a20 2020 2020 2020 2020  None:..         
-00004b80: 2020 2073 656c 6563 7465 645f 6d65 7468     selected_meth
-00004b90: 6f64 732e 6170 7065 6e64 2822 6d69 6e5f  ods.append("min_
-00004ba0: 7363 6f72 6522 290d 0a20 2020 2020 2020  score")..       
-00004bb0: 2069 6620 746f 705f 6e20 6973 206e 6f74   if top_n is not
-00004bc0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00004bd0: 2020 2020 7365 6c65 6374 6564 5f6d 6574      selected_met
-00004be0: 686f 6473 2e61 7070 656e 6428 2274 6f70  hods.append("top
-00004bf0: 5f6e 2229 0d0a 2020 2020 2020 2020 6966  _n")..        if
-00004c00: 2071 7561 6e74 696c 6520 6973 206e 6f74   quantile is not
-00004c10: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00004c20: 2020 2020 7365 6c65 6374 6564 5f6d 6574      selected_met
-00004c30: 686f 6473 2e61 7070 656e 6428 2271 7561  hods.append("qua
-00004c40: 6e74 696c 6522 290d 0a20 2020 2020 2020  ntile")..       
-00004c50: 2069 6620 6c65 6e28 7365 6c65 6374 6564   if len(selected
-00004c60: 5f6d 6574 686f 6473 2920 3e20 313a 0d0a  _methods) > 1:..
-00004c70: 2020 2020 2020 2020 2020 2020 6d65 7468              meth
-00004c80: 6f64 7761 726e 7374 7220 3d20 222c 2022  odwarnstr = ", "
-00004c90: 2e6a 6f69 6e28 7365 6c65 6374 6564 5f6d  .join(selected_m
-00004ca0: 6574 686f 6473 290d 0a20 2020 2020 2020  ethods)..       
-00004cb0: 2020 2020 206c 6f67 6769 6e67 2e77 6172       logging.war
-00004cc0: 6e69 6e67 2866 224d 756c 7469 706c 6520  ning(f"Multiple 
-00004cd0: 636f 6e66 6c69 6374 696e 6720 6f76 6572  conflicting over
-00004ce0: 6469 7370 6572 7365 6420 6765 6e65 2073  dispersed gene s
-00004cf0: 656c 6563 7469 6f6e 2063 7269 7465 7269  election criteri
-00004d00: 6120 6861 7665 2062 6565 6e20 7365 6c65  a have been sele
-00004d10: 6374 6564 3a20 7b6d 6574 686f 6477 6172  cted: {methodwar
-00004d20: 6e73 7472 7d2e 2022 0d0a 2020 2020 2020  nstr}. "..      
-00004d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d40: 2020 2020 2020 224f 6e6c 7920 7468 6520        "Only the 
-00004d50: 696e 7465 7273 6563 7469 6f6e 206f 6620  intersection of 
-00004d60: 7468 6573 6520 6d65 7468 6f64 7320 7769  these methods wi
-00004d70: 6c6c 2062 6520 7365 6c65 6374 6564 2e22  ll be selected."
-00004d80: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00004d90: 2020 200d 0a20 2020 2020 2020 2023 206d     ..        # m
-00004da0: 696e 5f6d 6561 6e20 6669 6c74 6572 0d0a  in_mean filter..
-00004db0: 2020 2020 2020 2020 7365 6c65 6374 6564          selected
-00004dc0: 5f67 656e 6573 203d 2073 656c 662e 6164  _genes = self.ad
-00004dd0: 6174 612e 7661 725b 226d 6561 6e5f 636f  ata.var["mean_co
-00004de0: 756e 7473 225d 203e 3d20 6d69 6e5f 6d65  unts"] >= min_me
-00004df0: 616e 0d0a 2020 2020 2020 2020 2320 6d69  an..        # mi
-00004e00: 6e5f 7363 6f72 6520 6669 6c74 6572 0d0a  n_score filter..
-00004e10: 2020 2020 2020 2020 6966 206d 696e 5f73          if min_s
-00004e20: 636f 7265 2069 7320 6e6f 7420 4e6f 6e65  core is not None
-00004e30: 3a0d 0a20 2020 2020 2020 2020 2020 2073  :..            s
-00004e40: 656c 6563 7465 645f 6765 6e65 7320 3d20  elected_genes = 
-00004e50: 7365 6c65 6374 6564 5f67 656e 6573 2026  selected_genes &
-00004e60: 2028 7365 6c66 2e61 6461 7461 2e76 6172   (self.adata.var
-00004e70: 5b6f 7665 7264 6973 7065 7273 696f 6e5f  [overdispersion_
-00004e80: 6d65 7472 6963 5d20 3e3d 206d 696e 5f73  metric] >= min_s
-00004e90: 636f 7265 290d 0a20 2020 2020 2020 2023  core)..        #
-00004ea0: 2074 6f70 5f6e 2066 696c 7465 720d 0a20   top_n filter.. 
-00004eb0: 2020 2020 2020 2069 6620 746f 705f 6e20         if top_n 
-00004ec0: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00004ed0: 2020 2020 2020 2020 2020 6765 6e65 7320            genes 
-00004ee0: 3d20 7365 6c66 2e61 6461 7461 2e76 6172  = self.adata.var
-00004ef0: 5b6f 7665 7264 6973 7065 7273 696f 6e5f  [overdispersion_
-00004f00: 6d65 7472 6963 5d2e 736f 7274 5f76 616c  metric].sort_val
-00004f10: 7565 7328 6173 6365 6e64 696e 673d 4661  ues(ascending=Fa
-00004f20: 6c73 6529 2e68 6561 6428 696e 7428 746f  lse).head(int(to
-00004f30: 705f 6e29 292e 696e 6465 780d 0a20 2020  p_n)).index..   
-00004f40: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
-00004f50: 645f 6765 6e65 7320 3d20 7365 6c65 6374  d_genes = select
-00004f60: 6564 5f67 656e 6573 2026 2073 656c 662e  ed_genes & self.
-00004f70: 6164 6174 612e 7661 722e 696e 6465 782e  adata.var.index.
-00004f80: 6973 696e 2867 656e 6573 290d 0a20 2020  isin(genes)..   
-00004f90: 2020 2020 2023 2071 7561 6e74 696c 6520       # quantile 
-00004fa0: 6669 6c74 6572 0d0a 2020 2020 2020 2020  filter..        
-00004fb0: 6966 2071 7561 6e74 696c 6520 6973 206e  if quantile is n
-00004fc0: 6f74 204e 6f6e 653a 0d0a 2020 2020 2020  ot None:..      
-00004fd0: 2020 2020 2020 6e5f 746f 7461 6c5f 6765        n_total_ge
-00004fe0: 6e65 7320 3d20 7365 6c66 2e61 6461 7461  nes = self.adata
-00004ff0: 2e76 6172 5b6f 7665 7264 6973 7065 7273  .var[overdispers
-00005000: 696f 6e5f 6d65 7472 6963 5d2e 6e6f 746e  ion_metric].notn
-00005010: 756c 6c28 292e 7375 6d28 290d 0a20 2020  ull().sum()..   
-00005020: 2020 2020 2020 2020 2067 656e 6573 203d           genes =
-00005030: 2073 656c 662e 6164 6174 612e 7661 725b   self.adata.var[
-00005040: 6f76 6572 6469 7370 6572 7369 6f6e 5f6d  overdispersion_m
-00005050: 6574 7269 635d 2e73 6f72 745f 7661 6c75  etric].sort_valu
-00005060: 6573 2861 7363 656e 6469 6e67 3d46 616c  es(ascending=Fal
-00005070: 7365 292e 6865 6164 2869 6e74 2871 7561  se).head(int(qua
-00005080: 6e74 696c 6520 2a20 6e5f 746f 7461 6c5f  ntile * n_total_
-00005090: 6765 6e65 7329 292e 696e 6465 780d 0a20  genes)).index.. 
-000050a0: 2020 2020 2020 2020 2020 2073 656c 6563             selec
-000050b0: 7465 645f 6765 6e65 7320 3d20 7365 6c65  ted_genes = sele
-000050c0: 6374 6564 5f67 656e 6573 2026 2073 656c  cted_genes & sel
-000050d0: 662e 6164 6174 612e 7661 722e 696e 6465  f.adata.var.inde
-000050e0: 782e 6973 696e 2867 656e 6573 290d 0a0d  x.isin(genes)...
-000050f0: 0a20 2020 2020 2020 206e 5f73 656c 6563  .        n_selec
-00005100: 7465 645f 6765 6e65 7320 3d20 7365 6c65  ted_genes = sele
-00005110: 6374 6564 5f67 656e 6573 2e73 756d 2829  cted_genes.sum()
-00005120: 0d0a 2020 2020 2020 2020 6c6f 6767 696e  ..        loggin
-00005130: 672e 696e 666f 2866 227b 6e5f 7365 6c65  g.info(f"{n_sele
-00005140: 6374 6564 5f67 656e 6573 7d20 6765 6e65  cted_genes} gene
-00005150: 7320 7365 6c65 6374 6564 2066 6f72 2066  s selected for f
-00005160: 6163 746f 7269 7a61 7469 6f6e 2229 0d0a  actorization")..
-00005170: 2020 2020 2020 2020 0d0a 2020 2020 2020          ..      
-00005180: 2020 2320 6d61 6b65 2063 6861 6e67 6573    # make changes
-00005190: 2074 6f20 4461 7461 7365 7420 6f62 6a65   to Dataset obje
-000051a0: 6374 0d0a 2020 2020 2020 2020 7365 6c66  ct..        self
-000051b0: 2e61 6461 7461 2e76 6172 5b22 7365 6c65  .adata.var["sele
-000051c0: 6374 6564 225d 203d 2073 656c 6563 7465  cted"] = selecte
-000051d0: 645f 6765 6e65 730d 0a20 2020 2020 2020  d_genes..       
-000051e0: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-000051f0: 226f 6467 225d 5b22 6f76 6572 6469 7370  "odg"]["overdisp
-00005200: 6572 7369 6f6e 5f6d 6574 7269 6322 5d20  ersion_metric"] 
-00005210: 3d20 6f76 6572 6469 7370 6572 7369 6f6e  = overdispersion
-00005220: 5f6d 6574 7269 630d 0a20 2020 2020 2020  _metric..       
-00005230: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-00005240: 226f 6467 225d 5b22 6d69 6e5f 6d65 616e  "odg"]["min_mean
-00005250: 225d 203d 206d 696e 5f6d 6561 6e0d 0a20  "] = min_mean.. 
-00005260: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
-00005270: 612e 756e 735b 226f 6467 225d 5b22 6d69  a.uns["odg"]["mi
-00005280: 6e5f 7363 6f72 6522 5d20 3d20 6d69 6e5f  n_score"] = min_
-00005290: 7363 6f72 6520 6966 206d 696e 5f73 636f  score if min_sco
-000052a0: 7265 2069 7320 6e6f 7420 4e6f 6e65 2065  re is not None e
-000052b0: 6c73 6520 2222 0d0a 2020 2020 2020 2020  lse ""..        
-000052c0: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
-000052d0: 6f64 6722 5d5b 2274 6f70 5f6e 225d 203d  odg"]["top_n"] =
-000052e0: 2074 6f70 5f6e 2069 6620 746f 705f 6e20   top_n if top_n 
-000052f0: 6973 206e 6f74 204e 6f6e 6520 656c 7365  is not None else
-00005300: 2022 220d 0a20 2020 2020 2020 2073 656c   ""..        sel
-00005310: 662e 6164 6174 612e 756e 735b 226f 6467  f.adata.uns["odg
-00005320: 225d 5b22 7175 616e 7469 6c65 225d 203d  "]["quantile"] =
-00005330: 2071 7561 6e74 696c 6520 6966 2071 7561   quantile if qua
-00005340: 6e74 696c 6520 6973 206e 6f74 204e 6f6e  ntile is not Non
-00005350: 6520 656c 7365 2022 220d 0a20 2020 2020  e else ""..     
-00005360: 2020 2073 656c 662e 6170 7065 6e64 5f74     self.append_t
-00005370: 6f5f 6869 7374 6f72 7928 224f 7665 7264  o_history("Overd
-00005380: 6973 7065 7273 6564 2067 656e 6573 2073  ispersed genes s
-00005390: 656c 6563 7465 6422 290d 0a20 2020 200d  elected")..    .
-000053a0: 0a20 2020 2064 6566 2069 6e69 7469 616c  .    def initial
-000053b0: 697a 655f 636e 6d66 2873 656c 662c 2063  ize_cnmf(self, c
-000053c0: 6e6d 665f 6f75 7470 7574 5f64 6972 3a20  nmf_output_dir: 
-000053d0: 7374 722c 0d0a 2020 2020 2020 2020 2020  str,..          
-000053e0: 2020 2020 2020 2020 2020 2020 2020 636e                cn
-000053f0: 6d66 5f6e 616d 653a 2073 7472 2c0d 0a20  mf_name: str,.. 
-00005400: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005410: 2020 2020 2020 206b 7661 6c73 3a20 436f         kvals: Co
-00005420: 6c6c 6563 7469 6f6e 203d 2072 616e 6765  llection = range
-00005430: 2832 2c20 3631 292c 0d0a 2020 2020 2020  (2, 61),..      
-00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005450: 2020 6e5f 6974 6572 3a20 696e 7420 3d20    n_iter: int = 
-00005460: 3230 302c 0d0a 2020 2020 2020 2020 2020  200,..          
-00005470: 2020 2020 2020 2020 2020 2020 2020 6265                be
-00005480: 7461 5f6c 6f73 733a 2073 7472 203d 2022  ta_loss: str = "
-00005490: 6b75 6c6c 6261 636b 2d6c 6569 626c 6572  kullback-leibler
-000054a0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000054b0: 2020 2020 2020 2020 2020 2020 7365 6564              seed
-000054c0: 3a20 4f70 7469 6f6e 616c 5b69 6e74 5d20  : Optional[int] 
-000054d0: 3d20 4e6f 6e65 2920 2d3e 2063 6e6d 662e  = None) -> cnmf.
-000054e0: 634e 4d46 3a0d 0a20 2020 2020 2020 2022  cNMF:..        "
-000054f0: 2222 496e 6974 6961 6c69 7a65 2061 2063  ""Initialize a c
-00005500: 4e4d 4620 7275 6e20 666f 7220 7375 6273  NMF run for subs
-00005510: 6571 7565 6e74 2066 6163 746f 7269 7a61  equent factoriza
-00005520: 7469 6f6e 2e0d 0a0d 0a20 2020 2020 2020  tion.....       
-00005530: 203a 7061 7261 6d20 636e 6d66 5f6f 7574   :param cnmf_out
-00005540: 7075 745f 6469 723a 204f 7574 7075 7420  put_dir: Output 
-00005550: 6469 7265 6374 6f72 7920 666f 7220 634e  directory for cN
-00005560: 4d46 2072 6573 756c 7473 0d0a 2020 2020  MF results..    
-00005570: 2020 2020 3a74 7970 6520 636e 6d66 5f6f      :type cnmf_o
-00005580: 7574 7075 745f 6469 723a 2073 7472 0d0a  utput_dir: str..
-00005590: 2020 2020 2020 2020 3a70 6172 616d 2063          :param c
-000055a0: 6e6d 665f 6e61 6d65 3a20 4e61 6d65 206f  nmf_name: Name o
-000055b0: 6620 7468 6520 634e 4d46 2072 6573 756c  f the cNMF resul
-000055c0: 7473 2e20 4669 6c65 7320 7769 6c6c 2062  ts. Files will b
-000055d0: 6520 6f75 7470 7574 2074 6f20 5b63 6e6d  e output to [cnm
-000055e0: 665f 6f75 7470 7574 5f64 6972 5d2f 5b63  f_output_dir]/[c
-000055f0: 6e6d 665f 6e61 6d65 5d2f 0d0a 2020 2020  nmf_name]/..    
-00005600: 2020 2020 3a74 7970 6520 636e 6d66 5f6e      :type cnmf_n
-00005610: 616d 653a 2073 7472 0d0a 2020 2020 2020  ame: str..      
-00005620: 2020 3a70 6172 616d 206b 7661 6c73 3a20    :param kvals: 
-00005630: 5261 6e6b 7320 666f 7220 634e 4d46 2066  Ranks for cNMF f
-00005640: 6163 746f 7269 7a61 7469 6f6e 2c20 6465  actorization, de
-00005650: 6661 756c 7473 2074 6f20 7261 6e67 6528  faults to range(
-00005660: 322c 2036 3129 0d0a 2020 2020 2020 2020  2, 61)..        
-00005670: 3a74 7970 6520 6b76 616c 733a 2043 6f6c  :type kvals: Col
-00005680: 6c65 6374 696f 6e2c 206f 7074 696f 6e61  lection, optiona
-00005690: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
-000056a0: 6d20 6e5f 6974 6572 3a20 4e75 6d62 6572  m n_iter: Number
-000056b0: 206f 6620 6974 6572 6174 696f 6e73 2066   of iterations f
-000056c0: 726f 6d20 7768 6963 6820 746f 2062 7569  rom which to bui
-000056d0: 6c64 2061 2063 6f6e 7365 6e73 7573 2073  ld a consensus s
-000056e0: 6f6c 7574 696f 6e2c 2064 6566 6175 6c74  olution, default
-000056f0: 7320 746f 2032 3030 0d0a 2020 2020 2020  s to 200..      
-00005700: 2020 3a74 7970 6520 6e5f 6974 6572 3a20    :type n_iter: 
-00005710: 696e 742c 206f 7074 696f 6e61 6c0d 0a20  int, optional.. 
-00005720: 2020 2020 2020 203a 7061 7261 6d20 6265         :param be
-00005730: 7461 5f6c 6f73 733a 2062 6574 612d 6c6f  ta_loss: beta-lo
-00005740: 7373 2066 756e 6374 696f 6e2c 2065 6974  ss function, eit
-00005750: 6865 7220 226b 756c 6c62 6163 6b2d 6c65  her "kullback-le
-00005760: 6962 6c65 7222 206f 7220 2266 726f 6265  ibler" or "frobe
-00005770: 6e69 7573 222e 2044 6566 6175 6c74 7320  nius". Defaults 
-00005780: 746f 2022 6b75 6c6c 6261 636b 2d6c 6569  to "kullback-lei
-00005790: 626c 6572 220d 0a20 2020 2020 2020 203a  bler"..        :
-000057a0: 7479 7065 2062 6574 615f 6c6f 7373 3a20  type beta_loss: 
-000057b0: 7374 722c 206f 7074 696f 6e61 6c0d 0a20  str, optional.. 
-000057c0: 2020 2020 2020 203a 7061 7261 6d20 7365         :param se
-000057d0: 6564 3a20 5261 6e64 6f6d 2073 6565 6420  ed: Random seed 
-000057e0: 666f 7220 7265 7072 6f64 7563 6962 696c  for reproducibil
-000057f0: 6974 792c 2064 6566 6175 6c74 7320 746f  ity, defaults to
-00005800: 204e 6f6e 650d 0a20 2020 2020 2020 203a   None..        :
-00005810: 7479 7065 2073 6565 643a 204f 7074 696f  type seed: Optio
-00005820: 6e61 6c5b 696e 745d 2c20 6f70 7469 6f6e  nal[int], option
-00005830: 616c 0d0a 2020 2020 2020 2020 3a72 6574  al..        :ret
-00005840: 7572 6e3a 2063 4e4d 4620 6f62 6a65 6374  urn: cNMF object
-00005850: 0d0a 2020 2020 2020 2020 3a72 7479 7065  ..        :rtype
-00005860: 3a20 3a63 6c61 7373 3a60 636e 6d66 736e  : :class:`cnmfsn
-00005870: 732e 636e 6d66 2e63 4e4d 4660 0d0a 2020  s.cnmf.cNMF`..  
-00005880: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
-00005890: 2020 2063 6e6d 665f 6f62 6a20 3d20 636e     cnmf_obj = cn
-000058a0: 6d66 2e63 4e4d 4628 6f75 7470 7574 5f64  mf.cNMF(output_d
-000058b0: 6972 3d63 6e6d 665f 6f75 7470 7574 5f64  ir=cnmf_output_d
-000058c0: 6972 2c20 6e61 6d65 3d63 6e6d 665f 6e61  ir, name=cnmf_na
-000058d0: 6d65 290d 0a20 2020 2020 2020 200d 0a20  me)..        .. 
-000058e0: 2020 2020 2020 2023 2077 7269 7465 2054         # write T
-000058f0: 504d 2028 6e6f 726d 616c 697a 6564 2920  PM (normalized) 
-00005900: 6461 7461 0d0a 2020 2020 2020 2020 7470  data..        tp
-00005910: 6d20 3d20 6164 2e41 6e6e 4461 7461 2873  m = ad.AnnData(s
-00005920: 656c 662e 746f 5f64 6628 6e6f 726d 616c  elf.to_df(normal
-00005930: 697a 6564 3d54 7275 6529 290d 0a20 2020  ized=True))..   
-00005940: 2020 2020 2074 706d 2e77 7269 7465 5f68       tpm.write_h
-00005950: 3561 6428 636e 6d66 5f6f 626a 2e70 6174  5ad(cnmf_obj.pat
-00005960: 6873 5b22 7470 6d22 5d29 0d0a 0d0a 2020  hs["tpm"])....  
-00005970: 2020 2020 2020 6765 6e65 5f74 706d 5f6d        gene_tpm_m
-00005980: 6561 6e20 3d20 6e70 2e61 7272 6179 2874  ean = np.array(t
-00005990: 706d 2e58 2e6d 6561 6e28 6178 6973 3d30  pm.X.mean(axis=0
-000059a0: 2929 2e72 6573 6861 7065 282d 3129 0d0a  )).reshape(-1)..
-000059b0: 2020 2020 2020 2020 6765 6e65 5f74 706d          gene_tpm
-000059c0: 5f73 7464 6465 7620 3d20 6e70 2e61 7272  _stddev = np.arr
-000059d0: 6179 2874 706d 2e58 2e73 7464 2861 7869  ay(tpm.X.std(axi
-000059e0: 733d 302c 2064 646f 663d 3029 292e 7265  s=0, ddof=0)).re
-000059f0: 7368 6170 6528 2d31 290d 0a20 2020 2020  shape(-1)..     
-00005a00: 2020 2069 6e70 7574 5f74 706d 5f73 7461     input_tpm_sta
-00005a10: 7473 203d 2070 642e 4461 7461 4672 616d  ts = pd.DataFram
-00005a20: 6528 5b67 656e 655f 7470 6d5f 6d65 616e  e([gene_tpm_mean
-00005a30: 2c20 6765 6e65 5f74 706d 5f73 7464 6465  , gene_tpm_stdde
-00005a40: 765d 2c20 696e 6465 7820 3d20 5b27 5f5f  v], index = ['__
-00005a50: 6d65 616e 272c 2027 5f5f 7374 6427 5d29  mean', '__std'])
-00005a60: 2e54 0d0a 2020 2020 2020 2020 7574 696c  .T..        util
-00005a70: 732e 7361 7665 5f64 665f 746f 5f6e 707a  s.save_df_to_npz
-00005a80: 2869 6e70 7574 5f74 706d 5f73 7461 7473  (input_tpm_stats
-00005a90: 2c20 636e 6d66 5f6f 626a 2e70 6174 6873  , cnmf_obj.paths
-00005aa0: 5b27 7470 6d5f 7374 6174 7327 5d29 0d0a  ['tpm_stats'])..
-00005ab0: 2020 2020 2020 2020 6f76 6572 6469 7370          overdisp
-00005ac0: 6572 7365 645f 6765 6e65 7320 3d20 7365  ersed_genes = se
-00005ad0: 6c66 2e61 6461 7461 2e76 6172 5b22 7365  lf.adata.var["se
-00005ae0: 6c65 6374 6564 225d 5b73 656c 662e 6164  lected"][self.ad
-00005af0: 6174 612e 7661 725b 2273 656c 6563 7465  ata.var["selecte
-00005b00: 6422 5d5d 2e69 6e64 6578 0d0a 2020 2020  d"]].index..    
-00005b10: 2020 2020 6e6f 726d 5f63 6f75 6e74 7320      norm_counts 
-00005b20: 3d20 636e 6d66 5f6f 626a 2e67 6574 5f6e  = cnmf_obj.get_n
-00005b30: 6f72 6d5f 636f 756e 7473 2873 656c 662e  orm_counts(self.
-00005b40: 6164 6174 612c 2074 706d 2c20 6869 6768  adata, tpm, high
-00005b50: 5f76 6172 6961 6e63 655f 6765 6e65 735f  _variance_genes_
-00005b60: 6669 6c74 6572 3d6f 7665 7264 6973 7065  filter=overdispe
-00005b70: 7273 6564 5f67 656e 6573 290d 0a20 2020  rsed_genes)..   
-00005b80: 2020 2020 2069 6620 6e6f 726d 5f63 6f75       if norm_cou
-00005b90: 6e74 732e 582e 6474 7970 6520 213d 206e  nts.X.dtype != n
-00005ba0: 702e 666c 6f61 7436 343a 0d0a 2020 2020  p.float64:..    
-00005bb0: 2020 2020 2020 2020 6e6f 726d 5f63 6f75          norm_cou
-00005bc0: 6e74 732e 5820 3d20 6e6f 726d 5f63 6f75  nts.X = norm_cou
-00005bd0: 6e74 732e 582e 6173 7479 7065 286e 702e  nts.X.astype(np.
-00005be0: 666c 6f61 7436 3429 0d0a 2020 2020 2020  float64)..      
-00005bf0: 2020 636e 6d66 5f6f 626a 2e73 6176 655f    cnmf_obj.save_
-00005c00: 6e6f 726d 5f63 6f75 6e74 7328 6e6f 726d  norm_counts(norm
-00005c10: 5f63 6f75 6e74 7329 0d0a 0d0a 2020 2020  _counts)....    
-00005c20: 2020 2020 2320 7361 7665 2070 6172 616d      # save param
-00005c30: 6574 6572 7320 666f 7220 6661 6374 6f72  eters for factor
-00005c40: 697a 6174 696f 6e20 7374 6570 0d0a 2020  ization step..  
-00005c50: 2020 2020 2020 636e 6d66 5f6f 626a 2e73        cnmf_obj.s
-00005c60: 6176 655f 6e6d 665f 6974 6572 5f70 6172  ave_nmf_iter_par
-00005c70: 616d 7328 2a63 6e6d 665f 6f62 6a2e 6765  ams(*cnmf_obj.ge
-00005c80: 745f 6e6d 665f 6974 6572 5f70 6172 616d  t_nmf_iter_param
-00005c90: 7328 6b73 3d6b 7661 6c73 2c20 6e5f 6974  s(ks=kvals, n_it
-00005ca0: 6572 3d6e 5f69 7465 722c 2072 616e 646f  er=n_iter, rando
-00005cb0: 6d5f 7374 6174 655f 7365 6564 3d73 6565  m_state_seed=see
-00005cc0: 642c 2062 6574 615f 6c6f 7373 3d62 6574  d, beta_loss=bet
-00005cd0: 615f 6c6f 7373 2929 0d0a 0d0a 2020 2020  a_loss))....    
-00005ce0: 2020 2020 2320 7361 7665 2070 6172 616d      # save param
-00005cf0: 6574 6572 7320 696e 2041 6e6e 4461 7461  eters in AnnData
-00005d00: 206f 626a 6563 740d 0a20 2020 2020 2020   object..       
-00005d10: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
-00005d20: 2263 6e6d 6622 5d20 3d20 636e 6d66 5f6f  "cnmf"] = cnmf_o
-00005d30: 626a 2e67 6574 5f6e 6d66 5f69 7465 725f  bj.get_nmf_iter_
-00005d40: 7061 7261 6d73 286b 733d 6b76 616c 732c  params(ks=kvals,
-00005d50: 206e 5f69 7465 723d 6e5f 6974 6572 2c20   n_iter=n_iter, 
-00005d60: 7261 6e64 6f6d 5f73 7461 7465 5f73 6565  random_state_see
-00005d70: 643d 7365 6564 2c20 6265 7461 5f6c 6f73  d=seed, beta_los
-00005d80: 733d 6265 7461 5f6c 6f73 7329 5b31 5d20  s=beta_loss)[1] 
-00005d90: 2023 2064 6963 7420 6f66 2063 6e6d 6620   # dict of cnmf 
-00005da0: 7061 7261 6d65 7465 7273 0d0a 2020 2020  parameters..    
-00005db0: 2020 2020 0d0a 2020 2020 2020 2020 7365      ..        se
-00005dc0: 6c66 2e61 7070 656e 645f 746f 5f68 6973  lf.append_to_his
-00005dd0: 746f 7279 2866 2263 4e4d 4620 7061 7261  tory(f"cNMF para
-00005de0: 6d65 7465 7273 2061 6464 6564 2e20 634e  meters added. cN
-00005df0: 4d46 2069 6e70 7574 7320 696e 6974 6961  MF inputs initia
-00005e00: 6c69 7a65 6420 696e 207b 636e 6d66 5f6f  lized in {cnmf_o
-00005e10: 7574 7075 745f 6469 727d 2f7b 636e 6d66  utput_dir}/{cnmf
-00005e20: 5f6e 616d 657d 2229 0d0a 2020 2020 2020  _name}")..      
-00005e30: 2020 7265 7475 726e 2063 6e6d 665f 6f62    return cnmf_ob
-00005e40: 6a0d 0a20 2020 200d 0a20 2020 2064 6566  j..    ..    def
-00005e50: 2061 6464 5f63 6e6d 665f 7265 7375 6c74   add_cnmf_result
-00005e60: 7328 7365 6c66 2c20 636e 6d66 5f6f 7574  s(self, cnmf_out
-00005e70: 7075 745f 6469 722c 2063 6e6d 665f 6e61  put_dir, cnmf_na
-00005e80: 6d65 2c20 6c6f 6361 6c5f 6465 6e73 6974  me, local_densit
-00005e90: 795f 7468 7265 7368 6f6c 643a 2066 6c6f  y_threshold: flo
-00005ea0: 6174 203d 204e 6f6e 652c 206c 6f63 616c  at = None, local
-00005eb0: 5f6e 6569 6768 626f 7268 6f6f 645f 7369  _neighborhood_si
-00005ec0: 7a65 3a20 666c 6f61 7420 3d20 4e6f 6e65  ze: float = None
-00005ed0: 293a 0d0a 2020 2020 2020 2020 2222 220d  ):..        """.
-00005ee0: 0a20 2020 2020 2020 2041 6674 6572 2066  .        After f
-00005ef0: 6163 746f 7269 7a61 7469 6f6e 2c20 6164  actorization, ad
-00005f00: 6420 636f 6d70 6c65 7465 6420 634e 4d46  d completed cNMF
-00005f10: 2072 6573 756c 7473 2069 6e20 5b63 6e6d   results in [cnm
-00005f20: 665f 6f75 7470 7574 5f64 6972 5d2f 5b63  f_output_dir]/[c
-00005f30: 6e6d 665f 6e61 6d65 5d20 746f 2074 6865  nmf_name] to the
-00005f40: 2064 6174 6173 6574 206f 626a 6563 742e   dataset object.
-00005f50: 0d0a 0d0a 2020 2020 2020 2020 3a70 6172  ....        :par
-00005f60: 616d 2063 6e6d 665f 6f75 7470 7574 5f64  am cnmf_output_d
-00005f70: 6972 3a20 4f75 7470 7574 2064 6972 6563  ir: Output direc
-00005f80: 746f 7279 2066 6f72 2063 4e4d 4620 7265  tory for cNMF re
-00005f90: 7375 6c74 730d 0a20 2020 2020 2020 203a  sults..        :
-00005fa0: 7479 7065 2063 6e6d 665f 6f75 7470 7574  type cnmf_output
-00005fb0: 5f64 6972 3a20 7374 720d 0a20 2020 2020  _dir: str..     
-00005fc0: 2020 203a 7061 7261 6d20 636e 6d66 5f6e     :param cnmf_n
-00005fd0: 616d 653a 204e 616d 6520 6f66 2074 6865  ame: Name of the
-00005fe0: 2063 4e4d 4620 7265 7375 6c74 732e 2046   cNMF results. F
-00005ff0: 696c 6573 2077 696c 6c20 6265 206f 7574  iles will be out
-00006000: 7075 7420 746f 205b 636e 6d66 5f6f 7574  put to [cnmf_out
-00006010: 7075 745f 6469 725d 2f5b 636e 6d66 5f6e  put_dir]/[cnmf_n
-00006020: 616d 655d 2f0d 0a20 2020 2020 2020 203a  ame]/..        :
-00006030: 7479 7065 2063 6e6d 665f 6e61 6d65 3a20  type cnmf_name: 
-00006040: 7374 720d 0a20 2020 2020 2020 203a 7061  str..        :pa
-00006050: 7261 6d20 6c6f 6361 6c5f 6465 6e73 6974  ram local_densit
-00006060: 795f 7468 7265 7368 6f6c 643a 2054 6872  y_threshold: Thr
-00006070: 6573 686f 6c64 2066 6f72 2074 6865 206c  eshold for the l
-00006080: 6f63 616c 2064 656e 7369 7479 2066 696c  ocal density fil
-00006090: 7465 7269 6e67 2070 7269 6f72 2074 6f20  tering prior to 
-000060a0: 4745 5020 636f 6e73 656e 7375 732e 2041  GEP consensus. A
-000060b0: 6363 6570 7461 626c 6520 7468 7265 7368  cceptable thresh
-000060c0: 6f6c 6473 2061 7265 203e 2030 2061 6e64  olds are > 0 and
-000060d0: 203c 3d20 3220 2832 2e30 2069 7320 6e6f   <= 2 (2.0 is no
-000060e0: 2066 696c 7465 7269 6e67 292e 2044 6566   filtering). Def
-000060f0: 6175 6c74 7320 746f 204e 6f6e 652e 0d0a  aults to None...
-00006100: 2020 2020 2020 2020 3a74 7970 6520 6c6f          :type lo
-00006110: 6361 6c5f 6465 6e73 6974 795f 7468 7265  cal_density_thre
-00006120: 7368 6f6c 643a 2066 6c6f 6174 2c20 6f70  shold: float, op
-00006130: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00006140: 3a70 6172 616d 206c 6f63 616c 5f6e 6569  :param local_nei
-00006150: 6768 626f 7268 6f6f 645f 7369 7a65 3a20  ghborhood_size: 
-00006160: 4672 6163 7469 6f6e 206f 6620 7468 6520  Fraction of the 
-00006170: 6e75 6d62 6572 206f 6620 7265 706c 6963  number of replic
-00006180: 6174 6573 2074 6f20 7573 6520 6173 206e  ates to use as n
-00006190: 6561 7265 7374 206e 6569 6768 626f 7273  earest neighbors
-000061a0: 2066 6f72 206c 6f63 616c 2064 656e 7369   for local densi
-000061b0: 7479 2066 696c 7465 7269 6e67 2e20 4465  ty filtering. De
-000061c0: 6661 756c 7473 2074 6f20 4e6f 6e65 0d0a  faults to None..
-000061d0: 2020 2020 2020 2020 3a74 7970 6520 6c6f          :type lo
-000061e0: 6361 6c5f 6e65 6967 6862 6f72 686f 6f64  cal_neighborhood
-000061f0: 5f73 697a 653a 2066 6c6f 6174 2c20 6f70  _size: float, op
-00006200: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00006210: 2222 220d 0a20 2020 2020 2020 2073 656c  """..        sel
-00006220: 662e 6164 6174 612e 756e 735b 2263 6e6d  f.adata.uns["cnm
-00006230: 665f 6e61 6d65 225d 203d 2063 6e6d 665f  f_name"] = cnmf_
-00006240: 6e61 6d65 0d0a 0d0a 2020 2020 2020 2020  name....        
-00006250: 2320 696e 6665 7220 6672 6f6d 2066 696c  # infer from fil
-00006260: 656e 616d 6573 2077 6869 6368 206c 6f63  enames which loc
-00006270: 616c 2064 656e 7369 7479 2074 6872 6573  al density thres
-00006280: 686f 6c64 2077 6173 2075 7365 640d 0a20  hold was used.. 
-00006290: 2020 2020 2020 2073 656e 7365 645f 6c64         sensed_ld
-000062a0: 7473 203d 2073 6574 2829 0d0a 2020 2020  ts = set()..    
-000062b0: 2020 2020 666f 7220 666e 2069 6e20 676c      for fn in gl
-000062c0: 6f62 286f 732e 7061 7468 2e6a 6f69 6e28  ob(os.path.join(
-000062d0: 636e 6d66 5f6f 7574 7075 745f 6469 722c  cnmf_output_dir,
-000062e0: 2063 6e6d 665f 6e61 6d65 2c20 6622 7b63   cnmf_name, f"{c
-000062f0: 6e6d 665f 6e61 6d65 7d2a 2e2a 7370 6563  nmf_name}*.*spec
-00006300: 7472 612a 2e6b 5f2a 2229 293a 0d0a 2020  tra*.k_*")):..  
-00006310: 2020 2020 2020 2020 2020 6c64 745f 7374            ldt_st
-00006320: 7220 3d20 6f73 2e70 6174 682e 6261 7365  r = os.path.base
-00006330: 6e61 6d65 2866 6e29 2e73 706c 6974 2822  name(fn).split("
-00006340: 2e22 295b 2d33 5d0d 0a20 2020 2020 2020  .")[-3]..       
-00006350: 2020 2020 2074 7279 3a0d 0a20 2020 2020       try:..     
-00006360: 2020 2020 2020 2020 2020 206c 6474 203d             ldt =
-00006370: 2066 6c6f 6174 286c 6474 5f73 7472 2e72   float(ldt_str.r
-00006380: 6570 6c61 6365 2822 6474 5f22 2c20 2222  eplace("dt_", ""
-00006390: 292e 7265 706c 6163 6528 225f 222c 2022  ).replace("_", "
-000063a0: 2e22 2929 0d0a 2020 2020 2020 2020 2020  ."))..          
-000063b0: 2020 6578 6365 7074 2056 616c 7565 4572    except ValueEr
-000063c0: 726f 723a 0d0a 2020 2020 2020 2020 2020  ror:..          
-000063d0: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
-000063e0: 2020 2020 2020 2020 656c 7365 3a0d 0a20          else:.. 
-000063f0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00006400: 656e 7365 645f 6c64 7473 2e61 6464 2828  ensed_ldts.add((
-00006410: 6c64 745f 7374 722c 206c 6474 2929 0d0a  ldt_str, ldt))..
-00006420: 2020 2020 2020 2020 6966 206c 6f63 616c          if local
-00006430: 5f64 656e 7369 7479 5f74 6872 6573 686f  _density_thresho
-00006440: 6c64 2069 7320 4e6f 6e65 2061 6e64 206c  ld is None and l
-00006450: 656e 2873 656e 7365 645f 6c64 7473 2920  en(sensed_ldts) 
-00006460: 3d3d 2031 3a0d 0a20 2020 2020 2020 2020  == 1:..         
-00006470: 2020 206c 6474 5f73 7472 2c20 6c64 7420     ldt_str, ldt 
-00006480: 3d20 7365 6e73 6564 5f6c 6474 732e 706f  = sensed_ldts.po
-00006490: 7028 290d 0a20 2020 2020 2020 2065 6c69  p()..        eli
-000064a0: 6620 6c6f 6361 6c5f 6465 6e73 6974 795f  f local_density_
-000064b0: 7468 7265 7368 6f6c 6420 696e 2028 6c64  threshold in (ld
-000064c0: 745b 315d 2066 6f72 206c 6474 2069 6e20  t[1] for ldt in 
-000064d0: 7365 6e73 6564 5f6c 6474 7329 3a0d 0a20  sensed_ldts):.. 
-000064e0: 2020 2020 2020 2020 2020 206c 6474 5f73             ldt_s
-000064f0: 7472 2c20 6c64 7420 3d20 5b28 6c64 745f  tr, ldt = [(ldt_
-00006500: 7374 722c 206c 6474 2920 666f 7220 6c64  str, ldt) for ld
-00006510: 745f 7374 722c 206c 6474 2069 6e20 7365  t_str, ldt in se
-00006520: 6e73 6564 5f6c 6474 7320 6966 206c 6474  nsed_ldts if ldt
-00006530: 203d 3d20 6c6f 6361 6c5f 6465 6e73 6974   == local_densit
-00006540: 795f 7468 7265 7368 6f6c 645d 2e70 6f70  y_threshold].pop
-00006550: 2829 0d0a 2020 2020 2020 2020 656c 7365  ()..        else
-00006560: 3a0d 0a20 2020 2020 2020 2020 2020 206c  :..            l
-00006570: 6f67 6769 6e67 2e65 7272 6f72 2866 226c  ogging.error(f"l
-00006580: 6f63 616c 5f64 656e 7369 7479 5f74 6872  ocal_density_thr
-00006590: 6573 686f 6c64 206f 6620 7b6c 6f63 616c  eshold of {local
-000065a0: 5f64 656e 7369 7479 5f74 6872 6573 686f  _density_thresho
-000065b0: 6c64 7d20 646f 6573 206e 6f74 206d 6174  ld} does not mat
-000065c0: 6368 2077 6861 7420 6973 2069 6e20 7468  ch what is in th
-000065d0: 6520 634e 4d46 2072 6573 756c 7420 6469  e cNMF result di
-000065e0: 7265 6374 6f72 793a 207b 7365 6e73 6564  rectory: {sensed
-000065f0: 5f6c 6474 737d 2229 0d0a 2020 2020 2020  _ldts}")..      
-00006600: 2020 2020 2020 7379 732e 6578 6974 2831        sys.exit(1
-00006610: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-00006620: 6164 6174 612e 756e 735b 226c 6474 225d  adata.uns["ldt"]
-00006630: 203d 206c 6474 0d0a 2020 2020 2020 2020   = ldt..        
-00006640: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
-00006650: 6c6e 7322 5d20 3d20 6c6f 6361 6c5f 6e65  lns"] = local_ne
-00006660: 6967 6862 6f72 686f 6f64 5f73 697a 650d  ighborhood_size.
-00006670: 0a20 2020 2020 2020 2020 2020 200d 0a20  .            .. 
-00006680: 2020 2020 2020 2023 2049 6d70 6f72 7420         # Import 
-00006690: 4745 5073 0d0a 2020 2020 2020 2020 7265  GEPs..        re
-000066a0: 7375 6c74 5f74 7970 6573 203d 207b 0d0a  sult_types = {..
-000066b0: 2020 2020 2020 2020 2020 2020 2267 656e              "gen
-000066c0: 655f 7370 6563 7472 615f 7363 6f72 6522  e_spectra_score"
-000066d0: 3a20 2263 6e6d 665f 6765 705f 7363 6f72  : "cnmf_gep_scor
-000066e0: 6522 2c0d 0a20 2020 2020 2020 2020 2020  e",..           
-000066f0: 2022 6765 6e65 5f73 7065 6374 7261 5f74   "gene_spectra_t
-00006700: 706d 223a 2022 636e 6d66 5f67 6570 5f74  pm": "cnmf_gep_t
-00006710: 706d 222c 0d0a 2020 2020 2020 2020 2020  pm",..          
-00006720: 2020 2273 7065 6374 7261 223a 2022 636e    "spectra": "cn
-00006730: 6d66 5f67 6570 5f72 6177 220d 0a20 2020  mf_gep_raw"..   
-00006740: 2020 2020 2020 2020 207d 0d0a 2020 2020           }..    
-00006750: 2020 2020 666f 7220 6d61 7463 6873 7472      for matchstr
-00006760: 2c20 7265 7375 6c74 5f74 7970 6520 696e  , result_type in
-00006770: 2072 6573 756c 745f 7479 7065 732e 6974   result_types.it
-00006780: 656d 7328 293a 0d0a 2020 2020 2020 2020  ems():..        
-00006790: 2020 2020 6c6f 6767 696e 672e 696e 666f      logging.info
-000067a0: 2866 2249 6d70 6f72 7469 6e67 2047 4550  (f"Importing GEP
-000067b0: 733a 207b 6d61 7463 6873 7472 7d22 2920  s: {matchstr}") 
-000067c0: 200d 0a20 2020 2020 2020 2020 2020 206d   ..            m
-000067d0: 6574 615f 7720 3d20 5b5d 0d0a 2020 2020  eta_w = []..    
-000067e0: 2020 2020 2020 2020 666f 7220 666e 2069          for fn i
-000067f0: 6e20 676c 6f62 286f 732e 7061 7468 2e6a  n glob(os.path.j
-00006800: 6f69 6e28 636e 6d66 5f6f 7574 7075 745f  oin(cnmf_output_
-00006810: 6469 722c 2063 6e6d 665f 6e61 6d65 2c20  dir, cnmf_name, 
-00006820: 6622 7b63 6e6d 665f 6e61 6d65 7d2a 2e7b  f"{cnmf_name}*.{
-00006830: 6d61 7463 6873 7472 7d2e 6b5f 2a2e 7b6c  matchstr}.k_*.{l
-00006840: 6474 5f73 7472 7d2e 2a74 7874 2229 293a  dt_str}.*txt")):
-00006850: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00006860: 2020 6b20 3d20 696e 7428 6f73 2e70 6174    k = int(os.pat
-00006870: 682e 6261 7365 6e61 6d65 2866 6e29 2e72  h.basename(fn).r
-00006880: 656d 6f76 6570 7265 6669 7828 6622 7b63  emoveprefix(f"{c
-00006890: 6e6d 665f 6e61 6d65 7d2e 7b6d 6174 6368  nmf_name}.{match
-000068a0: 7374 727d 2e22 292e 7370 6c69 7428 222e  str}.").split(".
-000068b0: 2229 5b30 5d2e 7265 706c 6163 6528 226b  ")[0].replace("k
-000068c0: 5f22 2c20 2222 2929 0d0a 2020 2020 2020  _", ""))..      
-000068d0: 2020 2020 2020 2020 2020 7720 3d20 7064            w = pd
-000068e0: 2e72 6561 645f 7461 626c 6528 666e 2c20  .read_table(fn, 
-000068f0: 696e 6465 785f 636f 6c3d 3029 0d0a 2020  index_col=0)..  
-00006900: 2020 2020 2020 2020 2020 2020 2020 772e                w.
-00006910: 696e 6465 7820 3d20 7374 7228 6b29 202b  index = str(k) +
-00006920: 2022 2e22 202b 2077 2e69 6e64 6578 2e61   "." + w.index.a
-00006930: 7374 7970 6528 7374 7229 0d0a 2020 2020  stype(str)..    
-00006940: 2020 2020 2020 2020 2020 2020 6d65 7461              meta
-00006950: 5f77 2e61 7070 656e 6428 7729 0d0a 2020  _w.append(w)..  
-00006960: 2020 2020 2020 2020 2020 6d65 7461 5f77            meta_w
-00006970: 203d 2070 642e 636f 6e63 6174 286d 6574   = pd.concat(met
-00006980: 615f 772c 2061 7869 733d 3029 2e54 2e72  a_w, axis=0).T.r
-00006990: 6569 6e64 6578 2873 656c 662e 6164 6174  eindex(self.adat
-000069a0: 612e 7661 722e 696e 6465 7829 2e72 656e  a.var.index).ren
-000069b0: 616d 655f 6178 6973 285b 226b 2e67 6570  ame_axis(["k.gep
-000069c0: 225d 2c20 6178 6973 3d31 290d 0a20 2020  "], axis=1)..   
-000069d0: 2020 2020 2020 2020 2073 656c 662e 6164           self.ad
-000069e0: 6174 612e 7661 726d 5b72 6573 756c 745f  ata.varm[result_
-000069f0: 7479 7065 5d20 3d20 6d65 7461 5f77 0d0a  type] = meta_w..
-00006a00: 0d0a 2020 2020 2020 2020 2320 496d 706f  ..        # Impo
-00006a10: 7274 2055 7361 6765 730d 0a20 2020 2020  rt Usages..     
-00006a20: 2020 206c 6f67 6769 6e67 2e69 6e66 6f28     logging.info(
-00006a30: 6622 496d 706f 7274 696e 6720 5573 6167  f"Importing Usag
-00006a40: 6573 2229 2020 0d0a 2020 2020 2020 2020  es")  ..        
-00006a50: 7573 6167 6520 3d20 5b5d 0d0a 2020 2020  usage = []..    
-00006a60: 2020 2020 666f 7220 666e 2069 6e20 676c      for fn in gl
-00006a70: 6f62 286f 732e 7061 7468 2e6a 6f69 6e28  ob(os.path.join(
-00006a80: 636e 6d66 5f6f 7574 7075 745f 6469 722c  cnmf_output_dir,
-00006a90: 2063 6e6d 665f 6e61 6d65 2c20 6622 7b63   cnmf_name, f"{c
-00006aa0: 6e6d 665f 6e61 6d65 7d2a 2e75 7361 6765  nmf_name}*.usage
-00006ab0: 732e 6b5f 2a2e 7b6c 6474 5f73 7472 7d2e  s.k_*.{ldt_str}.
-00006ac0: 2a74 7874 2229 293a 0d0a 2020 2020 2020  *txt")):..      
-00006ad0: 2020 2020 2020 6b20 3d20 696e 7428 6f73        k = int(os
-00006ae0: 2e70 6174 682e 6261 7365 6e61 6d65 2866  .path.basename(f
-00006af0: 6e29 2e72 656d 6f76 6570 7265 6669 7828  n).removeprefix(
-00006b00: 6622 7b63 6e6d 665f 6e61 6d65 7d2e 7573  f"{cnmf_name}.us
-00006b10: 6167 6573 2e22 292e 7370 6c69 7428 222e  ages.").split(".
-00006b20: 2229 5b30 5d2e 7265 706c 6163 6528 226b  ")[0].replace("k
-00006b30: 5f22 2c20 2222 2929 0d0a 2020 2020 2020  _", ""))..      
-00006b40: 2020 2020 2020 6820 3d20 7064 2e72 6561        h = pd.rea
-00006b50: 645f 7461 626c 6528 666e 2c20 696e 6465  d_table(fn, inde
-00006b60: 785f 636f 6c3d 3029 0d0a 2020 2020 2020  x_col=0)..      
-00006b70: 2020 2020 2020 682e 636f 6c75 6d6e 7320        h.columns 
-00006b80: 3d20 7374 7228 6b29 202b 2022 2e22 202b  = str(k) + "." +
-00006b90: 2068 2e63 6f6c 756d 6e73 2e61 7374 7970   h.columns.astyp
-00006ba0: 6528 7374 7229 0d0a 2020 2020 2020 2020  e(str)..        
-00006bb0: 2020 2020 7573 6167 652e 6170 7065 6e64      usage.append
-00006bc0: 2868 290d 0a20 2020 2020 2020 2073 656c  (h)..        sel
-00006bd0: 662e 6164 6174 612e 6f62 736d 5b22 636e  f.adata.obsm["cn
-00006be0: 6d66 5f75 7361 6765 225d 203d 2070 642e  mf_usage"] = pd.
-00006bf0: 636f 6e63 6174 2875 7361 6765 2c20 6178  concat(usage, ax
-00006c00: 6973 3d31 292e 736f 7274 5f69 6e64 6578  is=1).sort_index
-00006c10: 2861 7869 733d 3129 2e72 656e 616d 655f  (axis=1).rename_
-00006c20: 6178 6973 285b 226b 2e67 6570 225d 2c20  axis(["k.gep"], 
-00006c30: 6178 6973 3d31 290d 0a20 2020 2020 2020  axis=1)..       
-00006c40: 200d 0a20 2020 2020 2020 2023 2049 6d70   ..        # Imp
-00006c50: 6f72 7420 6765 6e65 206c 6973 7420 7573  ort gene list us
-00006c60: 6564 2066 6f72 2066 6163 746f 7269 7a61  ed for factoriza
-00006c70: 7469 6f6e 0d0a 2020 2020 2020 2020 7769  tion..        wi
-00006c80: 7468 206f 7065 6e28 6f73 2e70 6174 682e  th open(os.path.
-00006c90: 6a6f 696e 2863 6e6d 665f 6f75 7470 7574  join(cnmf_output
-00006ca0: 5f64 6972 2c20 636e 6d66 5f6e 616d 652c  _dir, cnmf_name,
-00006cb0: 2066 227b 636e 6d66 5f6e 616d 657d 2e6f   f"{cnmf_name}.o
-00006cc0: 7665 7264 6973 7065 7273 6564 5f67 656e  verdispersed_gen
-00006cd0: 6573 2e74 7874 2229 2920 6173 2066 3a0d  es.txt")) as f:.
-00006ce0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00006cf0: 662e 6164 6174 612e 756e 735b 2267 656e  f.adata.uns["gen
-00006d00: 655f 6c69 7374 225d 203d 205b 6c69 6e65  e_list"] = [line
-00006d10: 2e73 7472 6970 2829 2066 6f72 206c 696e  .strip() for lin
-00006d20: 6520 696e 2066 2e72 6561 646c 696e 6573  e in f.readlines
-00006d30: 2829 5d0d 0a0d 0a20 2020 2020 2020 2023  ()]....        #
-00006d40: 2049 6d70 6f72 7420 4b2d 7365 6c65 6374   Import K-select
-00006d50: 696f 6e20 7374 6174 730d 0a20 2020 2020  ion stats..     
-00006d60: 2020 206b 7661 6c73 203d 2070 642e 4461     kvals = pd.Da
-00006d70: 7461 4672 616d 6528 2a2a 6e70 2e6c 6f61  taFrame(**np.loa
-00006d80: 6428 6f73 2e70 6174 682e 6a6f 696e 2863  d(os.path.join(c
-00006d90: 6e6d 665f 6f75 7470 7574 5f64 6972 2c20  nmf_output_dir, 
-00006da0: 636e 6d66 5f6e 616d 652c 2066 227b 636e  cnmf_name, f"{cn
-00006db0: 6d66 5f6e 616d 657d 2e6b 5f73 656c 6563  mf_name}.k_selec
-00006dc0: 7469 6f6e 5f73 7461 7473 2e64 662e 6e70  tion_stats.df.np
-00006dd0: 7a22 292c 2061 6c6c 6f77 5f70 6963 6b6c  z"), allow_pickl
-00006de0: 653d 5472 7565 2929 2e73 6574 5f69 6e64  e=True)).set_ind
-00006df0: 6578 2822 6b22 295b 5b22 7374 6162 696c  ex("k")[["stabil
-00006e00: 6974 7922 2c20 2270 7265 6469 6374 696f  ity", "predictio
-00006e10: 6e5f 6572 726f 7222 5d5d 0d0a 2020 2020  n_error"]]..    
-00006e20: 2020 2020 6b76 616c 732e 696e 6465 7820      kvals.index 
-00006e30: 3d20 6b76 616c 732e 696e 6465 782e 6173  = kvals.index.as
-00006e40: 7479 7065 2869 6e74 290d 0a20 2020 2020  type(int)..     
-00006e50: 2020 2073 656c 662e 6164 6174 612e 756e     self.adata.un
-00006e60: 735b 226b 7661 6c73 225d 203d 206b 7661  s["kvals"] = kva
-00006e70: 6c73 0d0a 2020 2020 2020 2020 7365 6c66  ls..        self
-00006e80: 2e61 7070 656e 645f 746f 5f68 6973 746f  .append_to_histo
-00006e90: 7279 2822 634e 4d46 2072 6573 756c 7473  ry("cNMF results
-00006ea0: 2061 6464 6564 2066 726f 6d20 6f75 7470   added from outp
-00006eb0: 7574 2064 6972 6563 746f 7279 207b 636e  ut directory {cn
-00006ec0: 6d66 5f6f 7574 7075 745f 6469 727d 2f7b  mf_output_dir}/{
-00006ed0: 636e 6d66 5f6e 616d 657d 2229 0d0a 0d0a  cnmf_name}")....
-00006ee0: 2020 2020 6465 6620 6765 745f 7573 6167      def get_usag
-00006ef0: 6573 2873 656c 662c 0d0a 2020 2020 2020  es(self,..      
-00006f00: 2020 2020 2020 2020 2020 2020 206b 3a20               k: 
-00006f10: 556e 696f 6e5b 696e 742c 2049 7465 7261  Union[int, Itera
-00006f20: 626c 655d 203d 204e 6f6e 652c 0d0a 2020  ble] = None,..  
-00006f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006f40: 2064 6973 6372 6574 697a 653a 2062 6f6f   discretize: boo
-00006f50: 6c20 3d20 4661 6c73 652c 0d0a 2020 2020  l = False,..    
-00006f60: 2020 2020 2020 2020 2020 2020 2020 206e                 n
-00006f70: 6f72 6d61 6c69 7a65 3a20 626f 6f6c 203d  ormalize: bool =
-00006f80: 2046 616c 7365 0d0a 2020 2020 2020 2020   False..        
-00006f90: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-00006fa0: 7064 2e44 6174 6146 7261 6d65 3a0d 0a20  pd.DataFrame:.. 
-00006fb0: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-00006fc0: 2020 2020 4361 6c63 756c 6174 6520 7573      Calculate us
-00006fd0: 6167 6520 6f66 2065 6163 6820 4745 5020  age of each GEP 
-00006fe0: 696e 2065 6163 6820 7361 6d70 6c65 2f6f  in each sample/o
-00006ff0: 6273 6572 7661 7469 6f6e 2e0d 0a0d 0a20  bservation..... 
-00007000: 2020 2020 2020 203a 7061 7261 6d20 6b3a         :param k:
-00007010: 2049 6620 616e 2069 6e74 6567 6572 206f   If an integer o
-00007020: 7220 6c69 7374 206f 6620 696e 7465 6765  r list of intege
-00007030: 7273 2c20 7265 7475 726e 7320 7573 6167  rs, returns usag
-00007040: 6573 206f 6e6c 7920 666f 7220 7370 6563  es only for spec
-00007050: 6966 6965 6420 7261 6e6b 732e 204f 7468  ified ranks. Oth
-00007060: 6572 7769 7365 2c20 7265 7475 726e 7320  erwise, returns 
-00007070: 7573 6167 6520 6f66 2061 6c6c 2047 4550  usage of all GEP
-00007080: 7320 6163 726f 7373 2072 616e 6b73 2e20  s across ranks. 
-00007090: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
-000070a0: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-000070b0: 6b3a 2069 6e74 2c20 6f70 7469 6f6e 616c  k: int, optional
-000070c0: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
-000070d0: 2064 6973 6372 6574 697a 653a 2044 6973   discretize: Dis
-000070e0: 6372 6574 697a 6573 2074 6865 2075 7361  cretizes the usa
-000070f0: 6765 206d 6174 7269 7820 7375 6368 2074  ge matrix such t
-00007100: 6861 7420 666f 7220 6561 6368 2076 616c  hat for each val
-00007110: 7565 206f 6620 6b2c 2065 6163 6820 7361  ue of k, each sa
-00007120: 6d70 6c65 2068 6173 2075 7361 6765 206f  mple has usage o
-00007130: 6620 6f6e 6c79 2031 2047 4550 2028 7468  f only 1 GEP (th
-00007140: 6520 6f6e 6520 7769 7468 2074 6865 206d  e one with the m
-00007150: 6178 696d 756d 2075 7361 6765 292e 2044  aximum usage). D
-00007160: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
-00007170: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
-00007180: 6469 7363 7265 7469 7a65 3a20 626f 6f6c  discretize: bool
-00007190: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
-000071a0: 2020 2020 3a70 6172 616d 206e 6f72 6d61      :param norma
-000071b0: 6c69 7a65 3a20 4e6f 726d 616c 697a 6520  lize: Normalize 
-000071c0: 7468 6520 4745 5020 7573 6167 6520 6d61  the GEP usage ma
-000071d0: 7472 6978 2073 7563 6820 7468 6174 2066  trix such that f
-000071e0: 6f72 2065 6163 6820 7661 6c75 6520 6f66  or each value of
-000071f0: 206b 2c20 7573 6167 6520 6f66 2061 6c6c   k, usage of all
-00007200: 2047 4550 7320 7375 6d73 2074 6f20 312e   GEPs sums to 1.
-00007210: 2044 6566 6175 6c74 7320 746f 2046 616c   Defaults to Fal
-00007220: 7365 0d0a 2020 2020 2020 2020 3a74 7970  se..        :typ
-00007230: 6520 6e6f 726d 616c 697a 653a 2062 6f6f  e normalize: boo
-00007240: 6c2c 206f 7074 696f 6e61 6c0d 0a20 2020  l, optional..   
-00007250: 2020 2020 203a 7265 7475 726e 3a20 6f62       :return: ob
-00007260: 7365 7276 6174 696f 6e20 c397 2047 4550  servation .. GEP
-00007270: 206d 6174 7269 780d 0a20 2020 2020 2020   matrix..       
-00007280: 203a 7274 7970 653a 2070 642e 4461 7461   :rtype: pd.Data
-00007290: 4672 616d 650d 0a20 2020 2020 2020 2022  Frame..        "
-000072a0: 2222 0d0a 2020 2020 2020 2020 6466 203d  ""..        df =
-000072b0: 2073 656c 662e 6164 6174 612e 6f62 736d   self.adata.obsm
-000072c0: 5b22 636e 6d66 5f75 7361 6765 225d 2e63  ["cnmf_usage"].c
-000072d0: 6f70 7928 290d 0a20 2020 2020 2020 2064  opy()..        d
-000072e0: 662e 636f 6c75 6d6e 7320 3d20 7064 2e4d  f.columns = pd.M
-000072f0: 756c 7469 496e 6465 782e 6672 6f6d 5f74  ultiIndex.from_t
-00007300: 7570 6c65 7328 6466 2e63 6f6c 756d 6e73  uples(df.columns
-00007310: 2e73 7472 2e73 706c 6974 2822 2e22 292e  .str.split(".").
-00007320: 746f 5f6c 6973 7428 2929 0d0a 2020 2020  to_list())..    
-00007330: 2020 2020 6466 2e63 6f6c 756d 6e73 203d      df.columns =
-00007340: 2064 662e 636f 6c75 6d6e 732e 7365 745f   df.columns.set_
-00007350: 6c65 7665 6c73 285b 6c2e 6173 7479 7065  levels([l.astype
-00007360: 2822 696e 7422 2920 666f 7220 6c20 696e  ("int") for l in
-00007370: 2064 662e 636f 6c75 6d6e 732e 6c65 7665   df.columns.leve
-00007380: 6c73 5d29 0d0a 2020 2020 2020 2020 6966  ls])..        if
-00007390: 206e 6f72 6d61 6c69 7a65 3a0d 0a20 2020   normalize:..   
-000073a0: 2020 2020 2020 2020 206e 6f72 6d61 6c69           normali
-000073b0: 7a65 6420 3d20 5b5d 0d0a 2020 2020 2020  zed = []..      
-000073c0: 2020 2020 2020 666f 7220 5f2c 2073 7562        for _, sub
-000073d0: 6466 2069 6e20 6466 2e67 726f 7570 6279  df in df.groupby
-000073e0: 2861 7869 733d 312c 206c 6576 656c 3d30  (axis=1, level=0
-000073f0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-00007400: 2020 2020 6e6f 726d 616c 697a 6564 2e61      normalized.a
-00007410: 7070 656e 6428 7375 6264 662e 6469 7628  ppend(subdf.div(
-00007420: 7375 6264 662e 7375 6d28 6178 6973 3d31  subdf.sum(axis=1
-00007430: 292c 2061 7869 733d 3029 290d 0a20 2020  ), axis=0))..   
-00007440: 2020 2020 2020 2020 2064 6620 3d20 7064           df = pd
-00007450: 2e63 6f6e 6361 7428 6e6f 726d 616c 697a  .concat(normaliz
-00007460: 6564 2c20 6178 6973 3d31 290d 0a20 2020  ed, axis=1)..   
-00007470: 2020 2020 2069 6620 6469 7363 7265 7469       if discreti
-00007480: 7a65 3a0d 0a20 2020 2020 2020 2020 2020  ze:..           
-00007490: 2064 6973 6372 6574 697a 6564 203d 205b   discretized = [
-000074a0: 5d0d 0a20 2020 2020 2020 2020 2020 2066  ]..            f
-000074b0: 6f72 205f 2c20 7375 6264 6620 696e 2064  or _, subdf in d
-000074c0: 662e 6772 6f75 7062 7928 6178 6973 3d31  f.groupby(axis=1
-000074d0: 2c20 6c65 7665 6c3d 3029 3a0d 0a20 2020  , level=0):..   
-000074e0: 2020 2020 2020 2020 2020 2020 2064 6973               dis
-000074f0: 6372 6574 697a 6564 2e61 7070 656e 6428  cretized.append(
-00007500: 7375 6264 662e 6571 2873 7562 6466 2e6d  subdf.eq(subdf.m
-00007510: 6178 2861 7869 733d 3129 2c20 6178 6973  ax(axis=1), axis
-00007520: 3d30 292e 6173 7479 7065 2869 6e74 2929  =0).astype(int))
-00007530: 0d0a 2020 2020 2020 2020 2020 2020 6466  ..            df
-00007540: 203d 2070 642e 636f 6e63 6174 2864 6973   = pd.concat(dis
-00007550: 6372 6574 697a 6564 2c20 6178 6973 3d31  cretized, axis=1
-00007560: 2920 2020 2020 2020 200d 0a20 2020 2020  )        ..     
-00007570: 2020 2069 6620 6b20 6973 206e 6f74 204e     if k is not N
-00007580: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
-00007590: 2020 6466 203d 2064 662e 6c6f 635b 3a2c    df = df.loc[:,
-000075a0: 206b 5d0d 0a20 2020 2020 2020 2064 6620   k]..        df 
-000075b0: 3d20 6466 2e73 6f72 745f 696e 6465 7828  = df.sort_index(
-000075c0: 6178 6973 3d30 292e 736f 7274 5f69 6e64  axis=0).sort_ind
-000075d0: 6578 2861 7869 733d 3129 2020 200d 0a20  ex(axis=1)   .. 
-000075e0: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
-000075f0: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00007600: 6765 745f 6765 7073 2873 656c 662c 0d0a  get_geps(self,..
-00007610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007620: 206b 3a20 556e 696f 6e5b 696e 742c 2049   k: Union[int, I
-00007630: 7465 7261 626c 655d 203d 204e 6f6e 652c  terable] = None,
-00007640: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007650: 2020 2074 7970 653d 2263 6e6d 665f 6765     type="cnmf_ge
-00007660: 705f 7363 6f72 6522 0d0a 2020 2020 2020  p_score"..      
-00007670: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-00007680: 7064 2e44 6174 6146 7261 6d65 3a0d 0a20  pd.DataFrame:.. 
-00007690: 2020 2020 2020 2022 2222 0d0a 2020 2020         """..    
-000076a0: 2020 2020 4765 7420 4745 5073 2e0d 0a0d      Get GEPs....
-000076b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000076c0: 6b3a 2049 6620 616e 2069 6e74 6567 6572  k: If an integer
-000076d0: 206f 7220 6c69 7374 206f 6620 696e 7465   or list of inte
-000076e0: 6765 7273 2c20 7265 7475 726e 7320 4745  gers, returns GE
-000076f0: 5073 206f 6e6c 7920 666f 7220 7370 6563  Ps only for spec
-00007700: 6966 6965 6420 7261 6e6b 732e 204f 7468  ified ranks. Oth
-00007710: 6572 7769 7365 2c20 7265 7475 726e 7320  erwise, returns 
-00007720: 4745 5073 2066 726f 6d20 616c 6c20 7261  GEPs from all ra
-00007730: 6e6b 732e 2044 6566 6175 6c74 7320 746f  nks. Defaults to
-00007740: 204e 6f6e 650d 0a20 2020 2020 2020 203a   None..        :
-00007750: 7479 7065 206b 3a20 556e 696f 6e5b 696e  type k: Union[in
-00007760: 742c 2049 7465 7261 626c 655d 2c20 6f70  t, Iterable], op
-00007770: 7469 6f6e 616c 0d0a 2020 2020 2020 2020  tional..        
-00007780: 3a70 6172 616d 2074 7970 653a 2022 636e  :param type: "cn
-00007790: 6d66 5f67 6570 5f73 636f 7265 2220 6f72  mf_gep_score" or
-000077a0: 2022 636e 6d66 5f67 6570 5f74 706d 222c   "cnmf_gep_tpm",
-000077b0: 2064 6566 6175 6c74 7320 746f 2022 636e   defaults to "cn
-000077c0: 6d66 5f67 6570 5f73 636f 7265 220d 0a20  mf_gep_score".. 
-000077d0: 2020 2020 2020 203a 7479 7065 2074 7970         :type typ
-000077e0: 653a 2073 7472 2c20 6f70 7469 6f6e 616c  e: str, optional
-000077f0: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
-00007800: 6e3a 2066 6561 7475 7265 7320 c397 2047  n: features .. G
-00007810: 4550 206d 6174 7269 780d 0a20 2020 2020  EP matrix..     
-00007820: 2020 203a 7274 7970 653a 2070 642e 4461     :rtype: pd.Da
-00007830: 7461 4672 616d 650d 0a20 2020 2020 2020  taFrame..       
-00007840: 2022 2222 0d0a 2020 2020 2020 2020 6466   """..        df
-00007850: 203d 2073 656c 662e 6164 6174 612e 7661   = self.adata.va
-00007860: 726d 5b74 7970 655d 2e63 6f70 7928 290d  rm[type].copy().
-00007870: 0a20 2020 2020 2020 2064 662e 636f 6c75  .        df.colu
-00007880: 6d6e 7320 3d20 7064 2e4d 756c 7469 496e  mns = pd.MultiIn
-00007890: 6465 782e 6672 6f6d 5f74 7570 6c65 7328  dex.from_tuples(
-000078a0: 6466 2e63 6f6c 756d 6e73 2e73 7472 2e73  df.columns.str.s
-000078b0: 706c 6974 2822 2e22 292e 746f 5f6c 6973  plit(".").to_lis
-000078c0: 7428 2929 0d0a 2020 2020 2020 2020 6466  t())..        df
-000078d0: 2e63 6f6c 756d 6e73 203d 2064 662e 636f  .columns = df.co
-000078e0: 6c75 6d6e 732e 7365 745f 6c65 7665 6c73  lumns.set_levels
-000078f0: 285b 6c2e 6173 7479 7065 2822 696e 7422  ([l.astype("int"
-00007900: 2920 666f 7220 6c20 696e 2064 662e 636f  ) for l in df.co
-00007910: 6c75 6d6e 732e 6c65 7665 6c73 5d29 0d0a  lumns.levels])..
-00007920: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00007930: 7461 6e63 6528 6b2c 2028 696e 742c 2049  tance(k, (int, I
-00007940: 7465 7261 626c 6529 293a 0d0a 2020 2020  terable)):..    
-00007950: 2020 2020 2020 2020 6466 203d 2064 662e          df = df.
-00007960: 6c6f 635b 3a2c 206b 5d0d 0a20 2020 2020  loc[:, k]..     
-00007970: 2020 2064 6620 3d20 6466 2e73 6f72 745f     df = df.sort_
-00007980: 696e 6465 7828 6178 6973 3d31 290d 0a20  index(axis=1).. 
-00007990: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
-000079a0: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-000079b0: 6765 745f 6d65 7461 6461 7461 5f64 6628  get_metadata_df(
-000079c0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-000079d0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000079e0: 6e63 6c75 6465 5f63 6174 6567 6f72 6963  nclude_categoric
-000079f0: 616c 3a20 626f 6f6c 203d 2054 7275 652c  al: bool = True,
-00007a00: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00007a10: 2020 2020 2020 2020 2020 696e 636c 7564            includ
-00007a20: 655f 6e75 6d65 7269 6361 6c3a 2062 6f6f  e_numerical: boo
-00007a30: 6c20 3d20 5472 7565 0d0a 2020 2020 2020  l = True..      
-00007a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007a50: 2020 2920 2d3e 2070 642e 4461 7461 4672    ) -> pd.DataFr
-00007a60: 616d 653a 0d0a 2020 2020 2020 2020 2222  ame:..        ""
-00007a70: 2247 6574 2073 616d 706c 652f 6f62 7365  "Get sample/obse
-00007a80: 7276 6174 696f 6e20 6d65 7461 6461 7461  rvation metadata
-00007a90: 2e0d 0a0d 0a20 2020 2020 2020 203a 7061  .....        :pa
-00007aa0: 7261 6d20 696e 636c 7564 655f 6361 7465  ram include_cate
-00007ab0: 676f 7269 6361 6c3a 2049 6e63 6c75 6465  gorical: Include
-00007ac0: 2063 6174 6567 6f72 6963 616c 206d 6574   categorical met
-00007ad0: 6164 6174 6120 6c61 7965 7273 2c20 6465  adata layers, de
-00007ae0: 6661 756c 7473 2074 6f20 5472 7565 0d0a  faults to True..
-00007af0: 2020 2020 2020 2020 3a74 7970 6520 696e          :type in
-00007b00: 636c 7564 655f 6361 7465 676f 7269 6361  clude_categorica
-00007b10: 6c3a 2062 6f6f 6c2c 206f 7074 696f 6e61  l: bool, optiona
-00007b20: 6c0d 0a20 2020 2020 2020 203a 7061 7261  l..        :para
-00007b30: 6d20 696e 636c 7564 655f 6e75 6d65 7269  m include_numeri
-00007b40: 6361 6c3a 2049 6e63 6c75 6465 206e 756d  cal: Include num
-00007b50: 6572 6963 616c 206d 6574 6164 6174 6120  erical metadata 
-00007b60: 6c61 7965 7273 2c20 6465 6661 756c 7473  layers, defaults
-00007b70: 2074 6f20 5472 7565 0d0a 2020 2020 2020   to True..      
-00007b80: 2020 3a74 7970 6520 696e 636c 7564 655f    :type include_
-00007b90: 6e75 6d65 7269 6361 6c3a 2062 6f6f 6c2c  numerical: bool,
-00007ba0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
-00007bb0: 2020 203a 7261 6973 6573 2056 616c 7565     :raises Value
-00007bc0: 4572 726f 723a 2045 7272 6f72 2069 6620  Error: Error if 
-00007bd0: 6d65 7461 6461 7461 2074 7970 6573 2061  metadata types a
-00007be0: 7265 206e 6f74 2072 6563 6f67 6e69 7a65  re not recognize
-00007bf0: 640d 0a20 2020 2020 2020 203a 7265 7475  d..        :retu
-00007c00: 726e 3a20 6f62 7365 7276 6174 696f 6e73  rn: observations
-00007c10: 20c3 9720 6d65 7461 6461 7461 206d 6174   .. metadata mat
-00007c20: 7269 780d 0a20 2020 2020 2020 203a 7274  rix..        :rt
-00007c30: 7970 653a 2070 642e 4461 7461 4672 616d  ype: pd.DataFram
-00007c40: 650d 0a20 2020 2020 2020 2022 2222 0d0a  e..        """..
-00007c50: 2020 2020 2020 2020 6474 7970 6573 203d          dtypes =
-00007c60: 205b 5d0d 0a20 2020 2020 2020 2069 6620   []..        if 
-00007c70: 696e 636c 7564 655f 6361 7465 676f 7269  include_categori
-00007c80: 6361 6c3a 0d0a 2020 2020 2020 2020 2020  cal:..          
-00007c90: 2020 6474 7970 6573 2e61 7070 656e 6428    dtypes.append(
-00007ca0: 2263 6174 6567 6f72 7922 290d 0a20 2020  "category")..   
-00007cb0: 2020 2020 2069 6620 696e 636c 7564 655f       if include_
-00007cc0: 6e75 6d65 7269 6361 6c3a 0d0a 2020 2020  numerical:..    
-00007cd0: 2020 2020 2020 2020 6474 7970 6573 202b          dtypes +
-00007ce0: 3d20 5b22 666c 6f61 7422 2c20 2269 6e74  = ["float", "int
-00007cf0: 225d 0d0a 2020 2020 2020 2020 756e 6578  "]..        unex
-00007d00: 706c 6169 6e65 645f 636f 6c73 203d 2073  plained_cols = s
-00007d10: 656c 662e 6164 6174 612e 6f62 732e 7365  elf.adata.obs.se
-00007d20: 6c65 6374 5f64 7479 7065 7328 6578 636c  lect_dtypes(excl
-00007d30: 7564 653d 2822 6361 7465 676f 7279 222c  ude=("category",
-00007d40: 2022 666c 6f61 7422 2c20 2269 6e74 2229   "float", "int")
-00007d50: 292e 636f 6c75 6d6e 730d 0a20 2020 2020  ).columns..     
-00007d60: 2020 2069 6620 6c65 6e28 756e 6578 706c     if len(unexpl
-00007d70: 6169 6e65 645f 636f 6c73 2920 3e20 303a  ained_cols) > 0:
-00007d80: 0d0a 2020 2020 2020 2020 2020 2020 756e  ..            un
-00007d90: 6578 706c 6169 6e65 645f 636f 6c5f 7374  explained_col_st
-00007da0: 7220 3d20 222c 2022 2e6a 6f69 6e28 756e  r = ", ".join(un
-00007db0: 6578 706c 6169 6e65 645f 636f 6c73 290d  explained_cols).
-00007dc0: 0a20 2020 2020 2020 2020 2020 2072 6169  .            rai
-00007dd0: 7365 2056 616c 7565 4572 726f 7228 6622  se ValueError(f"
-00007de0: 7b75 6e65 7870 6c61 696e 6564 5f63 6f6c  {unexplained_col
-00007df0: 5f73 7472 7d20 6d65 7461 6461 7461 2063  _str} metadata c
-00007e00: 6f6c 756d 6e73 2068 6176 6520 756e 7265  olumns have unre
-00007e10: 636f 676e 697a 6564 2064 7479 7065 732e  cognized dtypes.
-00007e20: 2229 0d0a 2020 2020 2020 2020 6466 203d  ")..        df =
-00007e30: 2073 656c 662e 6164 6174 612e 6f62 732e   self.adata.obs.
-00007e40: 7365 6c65 6374 5f64 7479 7065 7328 696e  select_dtypes(in
-00007e50: 636c 7564 653d 6474 7970 6573 290d 0a20  clude=dtypes).. 
-00007e60: 2020 2020 2020 2072 6574 7572 6e20 6466         return df
-00007e70: 0d0a 2020 2020 0d0a 2020 2020 6465 6620  ..    ..    def 
-00007e80: 6765 745f 6361 7465 676f 7279 5f6f 7665  get_category_ove
-00007e90: 7272 6570 7265 7365 6e74 6174 696f 6e28  rrepresentation(
-00007ea0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-00007eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007ec0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00007ed0: 6179 6572 3a20 7374 722c 0d0a 2020 2020  ayer: str,..    
-00007ee0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004430: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00004440: 6f70 5f6e 3a20 696e 7420 3d20 4e6f 6e65  op_n: int = None
+00004450: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
+00004460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004470: 2020 2020 2020 7175 616e 7469 6c65 3a20        quantile: 
+00004480: 666c 6f61 7420 3d20 4e6f 6e65 293a 0d0a  float = None):..
+00004490: 2020 2020 2020 2020 2222 2253 656c 6563          """Selec
+000044a0: 7420 6f76 6572 6469 7370 6572 7365 6420  t overdispersed 
+000044b0: 6765 6e65 732f 6665 6174 7572 6573 2075  genes/features u
+000044c0: 7369 6e67 2061 6e20 6f76 6572 6469 7370  sing an overdisp
+000044d0: 6572 7369 6f6e 206d 6574 7269 632e 204f  ersion metric. O
+000044e0: 7074 696f 6e61 6c6c 7920 7365 7420 6120  ptionally set a 
+000044f0: 6d69 6e69 6d75 6d20 6765 6e65 2065 7870  minimum gene exp
+00004500: 7265 7373 696f 6e20 6c65 7665 6c2e 0d0a  ression level...
+00004510: 2020 2020 2020 2020 5365 7420 6120 7468          Set a th
+00004520: 7265 7368 6f6c 6420 7573 696e 6720 7468  reshold using th
+00004530: 6520 746f 7020 4e20 2827 746f 705f 6e27  e top N ('top_n'
+00004540: 292c 206d 696e 696d 756d 2073 636f 7265  ), minimum score
+00004550: 2028 276d 696e 5f73 636f 7265 2729 2c20   ('min_score'), 
+00004560: 6f72 2070 726f 706f 7274 696f 6e20 6f66  or proportion of
+00004570: 2066 6561 7475 7265 7320 2827 7175 616e   features ('quan
+00004580: 7469 6c65 2729 206d 6574 686f 6473 2e0d  tile') methods..
+00004590: 0a20 2020 2020 2020 204f 7665 7264 6973  .        Overdis
+000045a0: 7065 7273 6564 2067 656e 6520 6c69 7374  persed gene list
+000045b0: 2069 7320 7361 7665 6420 696e 2074 6865   is saved in the
+000045c0: 2044 6174 6173 6574 206f 626a 6563 742e   Dataset object.
+000045d0: 0d0a 0d0a 2020 2020 2020 2020 3a70 6172  ....        :par
+000045e0: 616d 206f 7665 7264 6973 7065 7273 696f  am overdispersio
+000045f0: 6e5f 6d65 7472 6963 3a20 226f 6473 636f  n_metric: "odsco
+00004600: 7265 2220 6f72 2022 7673 636f 7265 222c  re" or "vscore",
+00004610: 2064 6566 6175 6c74 7320 746f 2022 6f64   defaults to "od
+00004620: 7363 6f72 6522 0d0a 2020 2020 2020 2020  score"..        
+00004630: 3a74 7970 6520 6f76 6572 6469 7370 6572  :type overdisper
+00004640: 7369 6f6e 5f6d 6574 7269 633a 2073 7472  sion_metric: str
+00004650: 2c20 6f70 7469 6f6e 616c 0d0a 2020 2020  , optional..    
+00004660: 2020 2020 3a70 6172 616d 206d 696e 5f6d      :param min_m
+00004670: 6561 6e3a 206d 696e 696d 756d 2067 656e  ean: minimum gen
+00004680: 6520 6578 7072 6573 7369 6f6e 2066 6f72  e expression for
+00004690: 2067 656e 6573 2074 6f20 6265 2063 6f75   genes to be cou
+000046a0: 6e74 6564 2061 7320 6f76 6572 6469 7370  nted as overdisp
+000046b0: 6572 7365 642c 2064 6566 6175 6c74 7320  ersed, defaults 
+000046c0: 746f 2030 0d0a 2020 2020 2020 2020 3a74  to 0..        :t
+000046d0: 7970 6520 6d69 6e5f 6d65 616e 3a20 696e  ype min_mean: in
+000046e0: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
+000046f0: 2020 2020 203a 7061 7261 6d20 6d69 6e5f       :param min_
+00004700: 7363 6f72 653a 206d 696e 696d 756d 2073  score: minimum s
+00004710: 636f 7265 2066 6f72 206f 7665 7264 6973  core for overdis
+00004720: 7065 7273 696f 6e2c 2064 6566 6175 6c74  persion, default
+00004730: 7320 746f 2031 2e30 0d0a 2020 2020 2020  s to 1.0..      
+00004740: 2020 3a74 7970 6520 6d69 6e5f 7363 6f72    :type min_scor
+00004750: 653a 2066 6c6f 6174 2c20 6f70 7469 6f6e  e: float, option
+00004760: 616c 0d0a 2020 2020 2020 2020 3a70 6172  al..        :par
+00004770: 616d 2074 6f70 5f6e 3a20 4368 6f6f 7365  am top_n: Choose
+00004780: 2074 6865 2074 6f70 204e 206d 6f73 7420   the top N most 
+00004790: 6f76 6572 6469 7370 6572 7365 6420 6765  overdispersed ge
+000047a0: 6e65 732c 2064 6566 6175 6c74 7320 746f  nes, defaults to
+000047b0: 204e 6f6e 650d 0a20 2020 2020 2020 203a   None..        :
+000047c0: 7479 7065 2074 6f70 5f6e 3a20 696e 742c  type top_n: int,
+000047d0: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+000047e0: 2020 203a 7061 7261 6d20 7175 616e 7469     :param quanti
+000047f0: 6c65 3a20 4368 6f6f 7365 2061 2071 7561  le: Choose a qua
+00004800: 6e74 696c 6520 6f66 206f 7665 7264 6973  ntile of overdis
+00004810: 7065 7273 696f 6e2e 2046 6f72 2065 7861  persion. For exa
+00004820: 6d70 6c65 2c20 7468 6520 746f 7020 3130  mple, the top 10
+00004830: 2520 6f66 206f 7665 7264 6973 7065 7273  % of overdispers
+00004840: 6564 2067 656e 6573 2077 6f75 6c64 2062  ed genes would b
+00004850: 6520 302e 3130 2e20 4465 6661 756c 7473  e 0.10. Defaults
+00004860: 2074 6f20 4e6f 6e65 0d0a 2020 2020 2020   to None..      
+00004870: 2020 3a74 7970 6520 7175 616e 7469 6c65    :type quantile
+00004880: 3a20 666c 6f61 742c 206f 7074 696f 6e61  : float, optiona
+00004890: 6c0d 0a20 2020 2020 2020 203a 7261 6973  l..        :rais
+000048a0: 6573 2056 616c 7565 4572 726f 723a 2045  es ValueError: E
+000048b0: 7272 6f72 2069 6620 696e 7661 6c69 6420  rror if invalid 
+000048c0: 6f76 6572 6469 7370 6572 7369 6f6e 206d  overdispersion m
+000048d0: 6574 7269 6320 6973 2063 686f 7365 6e2e  etric is chosen.
+000048e0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000048f0: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00004900: 2069 6620 6f76 6572 6469 7370 6572 7369   if overdispersi
+00004910: 6f6e 5f6d 6574 7269 6320 6e6f 7420 696e  on_metric not in
+00004920: 2073 656c 662e 6164 6174 612e 7661 722e   self.adata.var.
+00004930: 636f 6c75 6d6e 733a 0d0a 2020 2020 2020  columns:..      
+00004940: 2020 2020 2020 6966 206f 7665 7264 6973        if overdis
+00004950: 7065 7273 696f 6e5f 6d65 7472 6963 2069  persion_metric i
+00004960: 6e20 2822 6f64 7363 6f72 6522 2c20 2276  n ("odscore", "v
+00004970: 7363 6f72 6522 293a 0d0a 2020 2020 2020  score"):..      
+00004980: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+00004990: 5661 6c75 6545 7272 6f72 280d 0a20 2020  ValueError(..   
+000049a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000049b0: 2066 227b 6f76 6572 6469 7370 6572 7369   f"{overdispersi
+000049c0: 6f6e 5f6d 6574 7269 637d 2068 6173 206e  on_metric} has n
+000049d0: 6f74 2062 6565 6e20 6361 6c63 756c 6174  ot been calculat
+000049e0: 6564 2066 6f72 2074 6869 7320 6461 7461  ed for this data
+000049f0: 7365 742e 2022 0d0a 2020 2020 2020 2020  set. "..        
+00004a00: 2020 2020 2020 2020 2020 2020 2245 6e73              "Ens
+00004a10: 7572 6520 7468 6174 2079 6f75 2063 616c  ure that you cal
+00004a20: 6c20 7468 6520 6044 6174 6173 6574 2e63  l the `Dataset.c
+00004a30: 6f6d 7075 7465 5f67 656e 655f 7374 6174  ompute_gene_stat
+00004a40: 7328 2960 2066 6972 7374 2e22 0d0a 2020  s()` first."..  
+00004a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a60: 2020 290d 0a20 2020 2020 2020 2020 2020    )..           
+00004a70: 2065 6c73 653a 0d0a 2020 2020 2020 2020   else:..        
+00004a80: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
+00004a90: 6c75 6545 7272 6f72 280d 0a20 2020 2020  lueError(..     
+00004aa0: 2020 2020 2020 2020 2020 2020 2020 2066                 f
+00004ab0: 227b 6f76 6572 6469 7370 6572 7369 6f6e  "{overdispersion
+00004ac0: 5f6d 6574 7269 637d 2069 7320 6e6f 7420  _metric} is not 
+00004ad0: 6120 7661 6c69 6420 6f76 6572 6469 7370  a valid overdisp
+00004ae0: 6572 7369 6f6e 206d 6574 7269 632e 220d  ersion metric.".
+00004af0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004b00: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00004b10: 0d0a 2020 2020 2020 2020 2320 7761 726e  ..        # warn
+00004b20: 2069 6620 6d75 6c74 6970 6c65 206d 6574   if multiple met
+00004b30: 686f 6473 2061 7265 2073 656c 6563 7465  hods are selecte
+00004b40: 640d 0a20 2020 2020 2020 2073 656c 6563  d..        selec
+00004b50: 7465 645f 6d65 7468 6f64 7320 3d20 5b5d  ted_methods = []
+00004b60: 0d0a 2020 2020 2020 2020 6966 206d 696e  ..        if min
+00004b70: 5f73 636f 7265 2069 7320 6e6f 7420 4e6f  _score is not No
+00004b80: 6e65 3a0d 0a20 2020 2020 2020 2020 2020  ne:..           
+00004b90: 2073 656c 6563 7465 645f 6d65 7468 6f64   selected_method
+00004ba0: 732e 6170 7065 6e64 2822 6d69 6e5f 7363  s.append("min_sc
+00004bb0: 6f72 6522 290d 0a20 2020 2020 2020 2069  ore")..        i
+00004bc0: 6620 746f 705f 6e20 6973 206e 6f74 204e  f top_n is not N
+00004bd0: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00004be0: 2020 7365 6c65 6374 6564 5f6d 6574 686f    selected_metho
+00004bf0: 6473 2e61 7070 656e 6428 2274 6f70 5f6e  ds.append("top_n
+00004c00: 2229 0d0a 2020 2020 2020 2020 6966 2071  ")..        if q
+00004c10: 7561 6e74 696c 6520 6973 206e 6f74 204e  uantile is not N
+00004c20: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00004c30: 2020 7365 6c65 6374 6564 5f6d 6574 686f    selected_metho
+00004c40: 6473 2e61 7070 656e 6428 2271 7561 6e74  ds.append("quant
+00004c50: 696c 6522 290d 0a20 2020 2020 2020 2069  ile")..        i
+00004c60: 6620 6c65 6e28 7365 6c65 6374 6564 5f6d  f len(selected_m
+00004c70: 6574 686f 6473 2920 3e20 313a 0d0a 2020  ethods) > 1:..  
+00004c80: 2020 2020 2020 2020 2020 6d65 7468 6f64            method
+00004c90: 7761 726e 7374 7220 3d20 222c 2022 2e6a  warnstr = ", ".j
+00004ca0: 6f69 6e28 7365 6c65 6374 6564 5f6d 6574  oin(selected_met
+00004cb0: 686f 6473 290d 0a20 2020 2020 2020 2020  hods)..         
+00004cc0: 2020 206c 6f67 6769 6e67 2e77 6172 6e69     logging.warni
+00004cd0: 6e67 2866 224d 756c 7469 706c 6520 636f  ng(f"Multiple co
+00004ce0: 6e66 6c69 6374 696e 6720 6f76 6572 6469  nflicting overdi
+00004cf0: 7370 6572 7365 6420 6765 6e65 2073 656c  spersed gene sel
+00004d00: 6563 7469 6f6e 2063 7269 7465 7269 6120  ection criteria 
+00004d10: 6861 7665 2062 6565 6e20 7365 6c65 6374  have been select
+00004d20: 6564 3a20 7b6d 6574 686f 6477 6172 6e73  ed: {methodwarns
+00004d30: 7472 7d2e 2022 0d0a 2020 2020 2020 2020  tr}. "..        
+00004d40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d50: 2020 2020 224f 6e6c 7920 7468 6520 696e      "Only the in
+00004d60: 7465 7273 6563 7469 6f6e 206f 6620 7468  tersection of th
+00004d70: 6573 6520 6d65 7468 6f64 7320 7769 6c6c  ese methods will
+00004d80: 2062 6520 7365 6c65 6374 6564 2e22 290d   be selected.").
+00004d90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004da0: 200d 0a20 2020 2020 2020 2023 206d 696e   ..        # min
+00004db0: 5f6d 6561 6e20 6669 6c74 6572 0d0a 2020  _mean filter..  
+00004dc0: 2020 2020 2020 7365 6c65 6374 6564 5f67        selected_g
+00004dd0: 656e 6573 203d 2073 656c 662e 6164 6174  enes = self.adat
+00004de0: 612e 7661 725b 226d 6561 6e5f 636f 756e  a.var["mean_coun
+00004df0: 7473 225d 203e 3d20 6d69 6e5f 6d65 616e  ts"] >= min_mean
+00004e00: 0d0a 2020 2020 2020 2020 2320 6d69 6e5f  ..        # min_
+00004e10: 7363 6f72 6520 6669 6c74 6572 0d0a 2020  score filter..  
+00004e20: 2020 2020 2020 6966 206d 696e 5f73 636f        if min_sco
+00004e30: 7265 2069 7320 6e6f 7420 4e6f 6e65 3a0d  re is not None:.
+00004e40: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00004e50: 6563 7465 645f 6765 6e65 7320 3d20 7365  ected_genes = se
+00004e60: 6c65 6374 6564 5f67 656e 6573 2026 2028  lected_genes & (
+00004e70: 7365 6c66 2e61 6461 7461 2e76 6172 5b6f  self.adata.var[o
+00004e80: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
+00004e90: 7472 6963 5d20 3e3d 206d 696e 5f73 636f  tric] >= min_sco
+00004ea0: 7265 290d 0a20 2020 2020 2020 2023 2074  re)..        # t
+00004eb0: 6f70 5f6e 2066 696c 7465 720d 0a20 2020  op_n filter..   
+00004ec0: 2020 2020 2069 6620 746f 705f 6e20 6973       if top_n is
+00004ed0: 206e 6f74 204e 6f6e 653a 0d0a 2020 2020   not None:..    
+00004ee0: 2020 2020 2020 2020 6765 6e65 7320 3d20          genes = 
+00004ef0: 7365 6c66 2e61 6461 7461 2e76 6172 5b6f  self.adata.var[o
+00004f00: 7665 7264 6973 7065 7273 696f 6e5f 6d65  verdispersion_me
+00004f10: 7472 6963 5d2e 736f 7274 5f76 616c 7565  tric].sort_value
+00004f20: 7328 6173 6365 6e64 696e 673d 4661 6c73  s(ascending=Fals
+00004f30: 6529 2e68 6561 6428 696e 7428 746f 705f  e).head(int(top_
+00004f40: 6e29 292e 696e 6465 780d 0a20 2020 2020  n)).index..     
+00004f50: 2020 2020 2020 2073 656c 6563 7465 645f         selected_
+00004f60: 6765 6e65 7320 3d20 7365 6c65 6374 6564  genes = selected
+00004f70: 5f67 656e 6573 2026 2073 656c 662e 6164  _genes & self.ad
+00004f80: 6174 612e 7661 722e 696e 6465 782e 6973  ata.var.index.is
+00004f90: 696e 2867 656e 6573 290d 0a20 2020 2020  in(genes)..     
+00004fa0: 2020 2023 2071 7561 6e74 696c 6520 6669     # quantile fi
+00004fb0: 6c74 6572 0d0a 2020 2020 2020 2020 6966  lter..        if
+00004fc0: 2071 7561 6e74 696c 6520 6973 206e 6f74   quantile is not
+00004fd0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
+00004fe0: 2020 2020 6e5f 746f 7461 6c5f 6765 6e65      n_total_gene
+00004ff0: 7320 3d20 7365 6c66 2e61 6461 7461 2e76  s = self.adata.v
+00005000: 6172 5b6f 7665 7264 6973 7065 7273 696f  ar[overdispersio
+00005010: 6e5f 6d65 7472 6963 5d2e 6e6f 746e 756c  n_metric].notnul
+00005020: 6c28 292e 7375 6d28 290d 0a20 2020 2020  l().sum()..     
+00005030: 2020 2020 2020 2067 656e 6573 203d 2073         genes = s
+00005040: 656c 662e 6164 6174 612e 7661 725b 6f76  elf.adata.var[ov
+00005050: 6572 6469 7370 6572 7369 6f6e 5f6d 6574  erdispersion_met
+00005060: 7269 635d 2e73 6f72 745f 7661 6c75 6573  ric].sort_values
+00005070: 2861 7363 656e 6469 6e67 3d46 616c 7365  (ascending=False
+00005080: 292e 6865 6164 2869 6e74 2871 7561 6e74  ).head(int(quant
+00005090: 696c 6520 2a20 6e5f 746f 7461 6c5f 6765  ile * n_total_ge
+000050a0: 6e65 7329 292e 696e 6465 780d 0a20 2020  nes)).index..   
+000050b0: 2020 2020 2020 2020 2073 656c 6563 7465           selecte
+000050c0: 645f 6765 6e65 7320 3d20 7365 6c65 6374  d_genes = select
+000050d0: 6564 5f67 656e 6573 2026 2073 656c 662e  ed_genes & self.
+000050e0: 6164 6174 612e 7661 722e 696e 6465 782e  adata.var.index.
+000050f0: 6973 696e 2867 656e 6573 290d 0a0d 0a20  isin(genes).... 
+00005100: 2020 2020 2020 206e 5f73 656c 6563 7465         n_selecte
+00005110: 645f 6765 6e65 7320 3d20 7365 6c65 6374  d_genes = select
+00005120: 6564 5f67 656e 6573 2e73 756d 2829 0d0a  ed_genes.sum()..
+00005130: 2020 2020 2020 2020 6c6f 6767 696e 672e          logging.
+00005140: 696e 666f 2866 227b 6e5f 7365 6c65 6374  info(f"{n_select
+00005150: 6564 5f67 656e 6573 7d20 6765 6e65 7320  ed_genes} genes 
+00005160: 7365 6c65 6374 6564 2066 6f72 2066 6163  selected for fac
+00005170: 746f 7269 7a61 7469 6f6e 2229 0d0a 2020  torization")..  
+00005180: 2020 2020 2020 0d0a 2020 2020 2020 2020        ..        
+00005190: 2320 6d61 6b65 2063 6861 6e67 6573 2074  # make changes t
+000051a0: 6f20 4461 7461 7365 7420 6f62 6a65 6374  o Dataset object
+000051b0: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+000051c0: 6461 7461 2e76 6172 5b22 7365 6c65 6374  data.var["select
+000051d0: 6564 225d 203d 2073 656c 6563 7465 645f  ed"] = selected_
+000051e0: 6765 6e65 730d 0a20 2020 2020 2020 2073  genes..        s
+000051f0: 656c 662e 6164 6174 612e 756e 735b 226f  elf.adata.uns["o
+00005200: 6467 225d 5b22 6f76 6572 6469 7370 6572  dg"]["overdisper
+00005210: 7369 6f6e 5f6d 6574 7269 6322 5d20 3d20  sion_metric"] = 
+00005220: 6f76 6572 6469 7370 6572 7369 6f6e 5f6d  overdispersion_m
+00005230: 6574 7269 630d 0a20 2020 2020 2020 2073  etric..        s
+00005240: 656c 662e 6164 6174 612e 756e 735b 226f  elf.adata.uns["o
+00005250: 6467 225d 5b22 6d69 6e5f 6d65 616e 225d  dg"]["min_mean"]
+00005260: 203d 206d 696e 5f6d 6561 6e0d 0a20 2020   = min_mean..   
+00005270: 2020 2020 2073 656c 662e 6164 6174 612e       self.adata.
+00005280: 756e 735b 226f 6467 225d 5b22 6d69 6e5f  uns["odg"]["min_
+00005290: 7363 6f72 6522 5d20 3d20 6d69 6e5f 7363  score"] = min_sc
+000052a0: 6f72 6520 6966 206d 696e 5f73 636f 7265  ore if min_score
+000052b0: 2069 7320 6e6f 7420 4e6f 6e65 2065 6c73   is not None els
+000052c0: 6520 2222 0d0a 2020 2020 2020 2020 7365  e ""..        se
+000052d0: 6c66 2e61 6461 7461 2e75 6e73 5b22 6f64  lf.adata.uns["od
+000052e0: 6722 5d5b 2274 6f70 5f6e 225d 203d 2074  g"]["top_n"] = t
+000052f0: 6f70 5f6e 2069 6620 746f 705f 6e20 6973  op_n if top_n is
+00005300: 206e 6f74 204e 6f6e 6520 656c 7365 2022   not None else "
+00005310: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+00005320: 6164 6174 612e 756e 735b 226f 6467 225d  adata.uns["odg"]
+00005330: 5b22 7175 616e 7469 6c65 225d 203d 2071  ["quantile"] = q
+00005340: 7561 6e74 696c 6520 6966 2071 7561 6e74  uantile if quant
+00005350: 696c 6520 6973 206e 6f74 204e 6f6e 6520  ile is not None 
+00005360: 656c 7365 2022 220d 0a20 2020 2020 2020  else ""..       
+00005370: 2073 656c 662e 6170 7065 6e64 5f74 6f5f   self.append_to_
+00005380: 6869 7374 6f72 7928 224f 7665 7264 6973  history("Overdis
+00005390: 7065 7273 6564 2067 656e 6573 2073 656c  persed genes sel
+000053a0: 6563 7465 6422 290d 0a20 2020 200d 0a20  ected")..    .. 
+000053b0: 2020 2064 6566 2069 6e69 7469 616c 697a     def initializ
+000053c0: 655f 636e 6d66 2873 656c 662c 2063 6e6d  e_cnmf(self, cnm
+000053d0: 665f 6f75 7470 7574 5f64 6972 3a20 7374  f_output_dir: st
+000053e0: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+000053f0: 2020 2020 2020 2020 2020 2020 636e 6d66              cnmf
+00005400: 5f6e 616d 653a 2073 7472 2c0d 0a20 2020  _name: str,..   
+00005410: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005420: 2020 2020 206b 7661 6c73 3a20 436f 6c6c       kvals: Coll
+00005430: 6563 7469 6f6e 203d 2072 616e 6765 2832  ection = range(2
+00005440: 2c20 3631 292c 0d0a 2020 2020 2020 2020  , 61),..        
+00005450: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005460: 6e5f 6974 6572 3a20 696e 7420 3d20 3230  n_iter: int = 20
+00005470: 302c 0d0a 2020 2020 2020 2020 2020 2020  0,..            
+00005480: 2020 2020 2020 2020 2020 2020 6265 7461              beta
+00005490: 5f6c 6f73 733a 2073 7472 203d 2022 6b75  _loss: str = "ku
+000054a0: 6c6c 6261 636b 2d6c 6569 626c 6572 222c  llback-leibler",
+000054b0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000054c0: 2020 2020 2020 2020 2020 7365 6564 3a20            seed: 
+000054d0: 4f70 7469 6f6e 616c 5b69 6e74 5d20 3d20  Optional[int] = 
+000054e0: 4e6f 6e65 2920 2d3e 2063 6e6d 662e 634e  None) -> cnmf.cN
+000054f0: 4d46 3a0d 0a20 2020 2020 2020 2022 2222  MF:..        """
+00005500: 496e 6974 6961 6c69 7a65 2061 2063 4e4d  Initialize a cNM
+00005510: 4620 7275 6e20 666f 7220 7375 6273 6571  F run for subseq
+00005520: 7565 6e74 2066 6163 746f 7269 7a61 7469  uent factorizati
+00005530: 6f6e 2e0d 0a0d 0a20 2020 2020 2020 203a  on.....        :
+00005540: 7061 7261 6d20 636e 6d66 5f6f 7574 7075  param cnmf_outpu
+00005550: 745f 6469 723a 204f 7574 7075 7420 6469  t_dir: Output di
+00005560: 7265 6374 6f72 7920 666f 7220 634e 4d46  rectory for cNMF
+00005570: 2072 6573 756c 7473 0d0a 2020 2020 2020   results..      
+00005580: 2020 3a74 7970 6520 636e 6d66 5f6f 7574    :type cnmf_out
+00005590: 7075 745f 6469 723a 2073 7472 0d0a 2020  put_dir: str..  
+000055a0: 2020 2020 2020 3a70 6172 616d 2063 6e6d        :param cnm
+000055b0: 665f 6e61 6d65 3a20 4e61 6d65 206f 6620  f_name: Name of 
+000055c0: 7468 6520 634e 4d46 2072 6573 756c 7473  the cNMF results
+000055d0: 2e20 4669 6c65 7320 7769 6c6c 2062 6520  . Files will be 
+000055e0: 6f75 7470 7574 2074 6f20 5b63 6e6d 665f  output to [cnmf_
+000055f0: 6f75 7470 7574 5f64 6972 5d2f 5b63 6e6d  output_dir]/[cnm
+00005600: 665f 6e61 6d65 5d2f 0d0a 2020 2020 2020  f_name]/..      
+00005610: 2020 3a74 7970 6520 636e 6d66 5f6e 616d    :type cnmf_nam
+00005620: 653a 2073 7472 0d0a 2020 2020 2020 2020  e: str..        
+00005630: 3a70 6172 616d 206b 7661 6c73 3a20 5261  :param kvals: Ra
+00005640: 6e6b 7320 666f 7220 634e 4d46 2066 6163  nks for cNMF fac
+00005650: 746f 7269 7a61 7469 6f6e 2c20 6465 6661  torization, defa
+00005660: 756c 7473 2074 6f20 7261 6e67 6528 322c  ults to range(2,
+00005670: 2036 3129 0d0a 2020 2020 2020 2020 3a74   61)..        :t
+00005680: 7970 6520 6b76 616c 733a 2043 6f6c 6c65  ype kvals: Colle
+00005690: 6374 696f 6e2c 206f 7074 696f 6e61 6c0d  ction, optional.
+000056a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000056b0: 6e5f 6974 6572 3a20 4e75 6d62 6572 206f  n_iter: Number o
+000056c0: 6620 6974 6572 6174 696f 6e73 2066 726f  f iterations fro
+000056d0: 6d20 7768 6963 6820 746f 2062 7569 6c64  m which to build
+000056e0: 2061 2063 6f6e 7365 6e73 7573 2073 6f6c   a consensus sol
+000056f0: 7574 696f 6e2c 2064 6566 6175 6c74 7320  ution, defaults 
+00005700: 746f 2032 3030 0d0a 2020 2020 2020 2020  to 200..        
+00005710: 3a74 7970 6520 6e5f 6974 6572 3a20 696e  :type n_iter: in
+00005720: 742c 206f 7074 696f 6e61 6c0d 0a20 2020  t, optional..   
+00005730: 2020 2020 203a 7061 7261 6d20 6265 7461       :param beta
+00005740: 5f6c 6f73 733a 2062 6574 612d 6c6f 7373  _loss: beta-loss
+00005750: 2066 756e 6374 696f 6e2c 2065 6974 6865   function, eithe
+00005760: 7220 226b 756c 6c62 6163 6b2d 6c65 6962  r "kullback-leib
+00005770: 6c65 7222 206f 7220 2266 726f 6265 6e69  ler" or "frobeni
+00005780: 7573 222e 2044 6566 6175 6c74 7320 746f  us". Defaults to
+00005790: 2022 6b75 6c6c 6261 636b 2d6c 6569 626c   "kullback-leibl
+000057a0: 6572 220d 0a20 2020 2020 2020 203a 7479  er"..        :ty
+000057b0: 7065 2062 6574 615f 6c6f 7373 3a20 7374  pe beta_loss: st
+000057c0: 722c 206f 7074 696f 6e61 6c0d 0a20 2020  r, optional..   
+000057d0: 2020 2020 203a 7061 7261 6d20 7365 6564       :param seed
+000057e0: 3a20 5261 6e64 6f6d 2073 6565 6420 666f  : Random seed fo
+000057f0: 7220 7265 7072 6f64 7563 6962 696c 6974  r reproducibilit
+00005800: 792c 2064 6566 6175 6c74 7320 746f 204e  y, defaults to N
+00005810: 6f6e 650d 0a20 2020 2020 2020 203a 7479  one..        :ty
+00005820: 7065 2073 6565 643a 204f 7074 696f 6e61  pe seed: Optiona
+00005830: 6c5b 696e 745d 2c20 6f70 7469 6f6e 616c  l[int], optional
+00005840: 0d0a 2020 2020 2020 2020 3a72 6574 7572  ..        :retur
+00005850: 6e3a 2063 4e4d 4620 6f62 6a65 6374 0d0a  n: cNMF object..
+00005860: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00005870: 3a63 6c61 7373 3a60 636e 6d66 736e 732e  :class:`cnmfsns.
+00005880: 636e 6d66 2e63 4e4d 4660 0d0a 2020 2020  cnmf.cNMF`..    
+00005890: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
+000058a0: 2063 6e6d 665f 6f62 6a20 3d20 636e 6d66   cnmf_obj = cnmf
+000058b0: 2e63 4e4d 4628 6f75 7470 7574 5f64 6972  .cNMF(output_dir
+000058c0: 3d63 6e6d 665f 6f75 7470 7574 5f64 6972  =cnmf_output_dir
+000058d0: 2c20 6e61 6d65 3d63 6e6d 665f 6e61 6d65  , name=cnmf_name
+000058e0: 290d 0a20 2020 2020 2020 200d 0a20 2020  )..        ..   
+000058f0: 2020 2020 2023 2077 7269 7465 2054 504d       # write TPM
+00005900: 2028 6e6f 726d 616c 697a 6564 2920 6461   (normalized) da
+00005910: 7461 0d0a 2020 2020 2020 2020 7470 6d20  ta..        tpm 
+00005920: 3d20 6164 2e41 6e6e 4461 7461 2873 656c  = ad.AnnData(sel
+00005930: 662e 746f 5f64 6628 6e6f 726d 616c 697a  f.to_df(normaliz
+00005940: 6564 3d54 7275 6529 290d 0a20 2020 2020  ed=True))..     
+00005950: 2020 2074 706d 2e77 7269 7465 5f68 3561     tpm.write_h5a
+00005960: 6428 636e 6d66 5f6f 626a 2e70 6174 6873  d(cnmf_obj.paths
+00005970: 5b22 7470 6d22 5d29 0d0a 0d0a 2020 2020  ["tpm"])....    
+00005980: 2020 2020 6765 6e65 5f74 706d 5f6d 6561      gene_tpm_mea
+00005990: 6e20 3d20 6e70 2e61 7272 6179 2874 706d  n = np.array(tpm
+000059a0: 2e58 2e6d 6561 6e28 6178 6973 3d30 2929  .X.mean(axis=0))
+000059b0: 2e72 6573 6861 7065 282d 3129 0d0a 2020  .reshape(-1)..  
+000059c0: 2020 2020 2020 6765 6e65 5f74 706d 5f73        gene_tpm_s
+000059d0: 7464 6465 7620 3d20 6e70 2e61 7272 6179  tddev = np.array
+000059e0: 2874 706d 2e58 2e73 7464 2861 7869 733d  (tpm.X.std(axis=
+000059f0: 302c 2064 646f 663d 3029 292e 7265 7368  0, ddof=0)).resh
+00005a00: 6170 6528 2d31 290d 0a20 2020 2020 2020  ape(-1)..       
+00005a10: 2069 6e70 7574 5f74 706d 5f73 7461 7473   input_tpm_stats
+00005a20: 203d 2070 642e 4461 7461 4672 616d 6528   = pd.DataFrame(
+00005a30: 5b67 656e 655f 7470 6d5f 6d65 616e 2c20  [gene_tpm_mean, 
+00005a40: 6765 6e65 5f74 706d 5f73 7464 6465 765d  gene_tpm_stddev]
+00005a50: 2c20 696e 6465 7820 3d20 5b27 5f5f 6d65  , index = ['__me
+00005a60: 616e 272c 2027 5f5f 7374 6427 5d29 2e54  an', '__std']).T
+00005a70: 0d0a 2020 2020 2020 2020 7574 696c 732e  ..        utils.
+00005a80: 7361 7665 5f64 665f 746f 5f6e 707a 2869  save_df_to_npz(i
+00005a90: 6e70 7574 5f74 706d 5f73 7461 7473 2c20  nput_tpm_stats, 
+00005aa0: 636e 6d66 5f6f 626a 2e70 6174 6873 5b27  cnmf_obj.paths['
+00005ab0: 7470 6d5f 7374 6174 7327 5d29 0d0a 2020  tpm_stats'])..  
+00005ac0: 2020 2020 2020 6f76 6572 6469 7370 6572        overdisper
+00005ad0: 7365 645f 6765 6e65 7320 3d20 7365 6c66  sed_genes = self
+00005ae0: 2e61 6461 7461 2e76 6172 5b22 7365 6c65  .adata.var["sele
+00005af0: 6374 6564 225d 5b73 656c 662e 6164 6174  cted"][self.adat
+00005b00: 612e 7661 725b 2273 656c 6563 7465 6422  a.var["selected"
+00005b10: 5d5d 2e69 6e64 6578 0d0a 2020 2020 2020  ]].index..      
+00005b20: 2020 6e6f 726d 5f63 6f75 6e74 7320 3d20    norm_counts = 
+00005b30: 636e 6d66 5f6f 626a 2e67 6574 5f6e 6f72  cnmf_obj.get_nor
+00005b40: 6d5f 636f 756e 7473 2873 656c 662e 6164  m_counts(self.ad
+00005b50: 6174 612c 2074 706d 2c20 6869 6768 5f76  ata, tpm, high_v
+00005b60: 6172 6961 6e63 655f 6765 6e65 735f 6669  ariance_genes_fi
+00005b70: 6c74 6572 3d6f 7665 7264 6973 7065 7273  lter=overdispers
+00005b80: 6564 5f67 656e 6573 290d 0a20 2020 2020  ed_genes)..     
+00005b90: 2020 2069 6620 6e6f 726d 5f63 6f75 6e74     if norm_count
+00005ba0: 732e 582e 6474 7970 6520 213d 206e 702e  s.X.dtype != np.
+00005bb0: 666c 6f61 7436 343a 0d0a 2020 2020 2020  float64:..      
+00005bc0: 2020 2020 2020 6e6f 726d 5f63 6f75 6e74        norm_count
+00005bd0: 732e 5820 3d20 6e6f 726d 5f63 6f75 6e74  s.X = norm_count
+00005be0: 732e 582e 6173 7479 7065 286e 702e 666c  s.X.astype(np.fl
+00005bf0: 6f61 7436 3429 0d0a 2020 2020 2020 2020  oat64)..        
+00005c00: 636e 6d66 5f6f 626a 2e73 6176 655f 6e6f  cnmf_obj.save_no
+00005c10: 726d 5f63 6f75 6e74 7328 6e6f 726d 5f63  rm_counts(norm_c
+00005c20: 6f75 6e74 7329 0d0a 0d0a 2020 2020 2020  ounts)....      
+00005c30: 2020 2320 7361 7665 2070 6172 616d 6574    # save paramet
+00005c40: 6572 7320 666f 7220 6661 6374 6f72 697a  ers for factoriz
+00005c50: 6174 696f 6e20 7374 6570 0d0a 2020 2020  ation step..    
+00005c60: 2020 2020 636e 6d66 5f6f 626a 2e73 6176      cnmf_obj.sav
+00005c70: 655f 6e6d 665f 6974 6572 5f70 6172 616d  e_nmf_iter_param
+00005c80: 7328 2a63 6e6d 665f 6f62 6a2e 6765 745f  s(*cnmf_obj.get_
+00005c90: 6e6d 665f 6974 6572 5f70 6172 616d 7328  nmf_iter_params(
+00005ca0: 6b73 3d6b 7661 6c73 2c20 6e5f 6974 6572  ks=kvals, n_iter
+00005cb0: 3d6e 5f69 7465 722c 2072 616e 646f 6d5f  =n_iter, random_
+00005cc0: 7374 6174 655f 7365 6564 3d73 6565 642c  state_seed=seed,
+00005cd0: 2062 6574 615f 6c6f 7373 3d62 6574 615f   beta_loss=beta_
+00005ce0: 6c6f 7373 2929 0d0a 0d0a 2020 2020 2020  loss))....      
+00005cf0: 2020 2320 7361 7665 2070 6172 616d 6574    # save paramet
+00005d00: 6572 7320 696e 2041 6e6e 4461 7461 206f  ers in AnnData o
+00005d10: 626a 6563 740d 0a20 2020 2020 2020 2073  bject..        s
+00005d20: 656c 662e 6164 6174 612e 756e 735b 2263  elf.adata.uns["c
+00005d30: 6e6d 6622 5d20 3d20 636e 6d66 5f6f 626a  nmf"] = cnmf_obj
+00005d40: 2e67 6574 5f6e 6d66 5f69 7465 725f 7061  .get_nmf_iter_pa
+00005d50: 7261 6d73 286b 733d 6b76 616c 732c 206e  rams(ks=kvals, n
+00005d60: 5f69 7465 723d 6e5f 6974 6572 2c20 7261  _iter=n_iter, ra
+00005d70: 6e64 6f6d 5f73 7461 7465 5f73 6565 643d  ndom_state_seed=
+00005d80: 7365 6564 2c20 6265 7461 5f6c 6f73 733d  seed, beta_loss=
+00005d90: 6265 7461 5f6c 6f73 7329 5b31 5d20 2023  beta_loss)[1]  #
+00005da0: 2064 6963 7420 6f66 2063 6e6d 6620 7061   dict of cnmf pa
+00005db0: 7261 6d65 7465 7273 0d0a 2020 2020 2020  rameters..      
+00005dc0: 2020 0d0a 2020 2020 2020 2020 7365 6c66    ..        self
+00005dd0: 2e61 7070 656e 645f 746f 5f68 6973 746f  .append_to_histo
+00005de0: 7279 2866 2263 4e4d 4620 7061 7261 6d65  ry(f"cNMF parame
+00005df0: 7465 7273 2061 6464 6564 2e20 634e 4d46  ters added. cNMF
+00005e00: 2069 6e70 7574 7320 696e 6974 6961 6c69   inputs initiali
+00005e10: 7a65 6420 696e 207b 636e 6d66 5f6f 7574  zed in {cnmf_out
+00005e20: 7075 745f 6469 727d 2f7b 636e 6d66 5f6e  put_dir}/{cnmf_n
+00005e30: 616d 657d 2229 0d0a 2020 2020 2020 2020  ame}")..        
+00005e40: 7265 7475 726e 2063 6e6d 665f 6f62 6a0d  return cnmf_obj.
+00005e50: 0a20 2020 200d 0a20 2020 2064 6566 2061  .    ..    def a
+00005e60: 6464 5f63 6e6d 665f 7265 7375 6c74 7328  dd_cnmf_results(
+00005e70: 7365 6c66 2c20 636e 6d66 5f6f 7574 7075  self, cnmf_outpu
+00005e80: 745f 6469 722c 2063 6e6d 665f 6e61 6d65  t_dir, cnmf_name
+00005e90: 2c20 6c6f 6361 6c5f 6465 6e73 6974 795f  , local_density_
+00005ea0: 7468 7265 7368 6f6c 643a 2066 6c6f 6174  threshold: float
+00005eb0: 203d 204e 6f6e 652c 206c 6f63 616c 5f6e   = None, local_n
+00005ec0: 6569 6768 626f 7268 6f6f 645f 7369 7a65  eighborhood_size
+00005ed0: 3a20 666c 6f61 7420 3d20 4e6f 6e65 293a  : float = None):
+00005ee0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00005ef0: 2020 2020 2020 2041 6674 6572 2066 6163         After fac
+00005f00: 746f 7269 7a61 7469 6f6e 2c20 6164 6420  torization, add 
+00005f10: 636f 6d70 6c65 7465 6420 634e 4d46 2072  completed cNMF r
+00005f20: 6573 756c 7473 2069 6e20 5b63 6e6d 665f  esults in [cnmf_
+00005f30: 6f75 7470 7574 5f64 6972 5d2f 5b63 6e6d  output_dir]/[cnm
+00005f40: 665f 6e61 6d65 5d20 746f 2074 6865 2064  f_name] to the d
+00005f50: 6174 6173 6574 206f 626a 6563 742e 0d0a  ataset object...
+00005f60: 0d0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+00005f70: 2063 6e6d 665f 6f75 7470 7574 5f64 6972   cnmf_output_dir
+00005f80: 3a20 4f75 7470 7574 2064 6972 6563 746f  : Output directo
+00005f90: 7279 2066 6f72 2063 4e4d 4620 7265 7375  ry for cNMF resu
+00005fa0: 6c74 730d 0a20 2020 2020 2020 203a 7479  lts..        :ty
+00005fb0: 7065 2063 6e6d 665f 6f75 7470 7574 5f64  pe cnmf_output_d
+00005fc0: 6972 3a20 7374 720d 0a20 2020 2020 2020  ir: str..       
+00005fd0: 203a 7061 7261 6d20 636e 6d66 5f6e 616d   :param cnmf_nam
+00005fe0: 653a 204e 616d 6520 6f66 2074 6865 2063  e: Name of the c
+00005ff0: 4e4d 4620 7265 7375 6c74 732e 2046 696c  NMF results. Fil
+00006000: 6573 2077 696c 6c20 6265 206f 7574 7075  es will be outpu
+00006010: 7420 746f 205b 636e 6d66 5f6f 7574 7075  t to [cnmf_outpu
+00006020: 745f 6469 725d 2f5b 636e 6d66 5f6e 616d  t_dir]/[cnmf_nam
+00006030: 655d 2f0d 0a20 2020 2020 2020 203a 7479  e]/..        :ty
+00006040: 7065 2063 6e6d 665f 6e61 6d65 3a20 7374  pe cnmf_name: st
+00006050: 720d 0a20 2020 2020 2020 203a 7061 7261  r..        :para
+00006060: 6d20 6c6f 6361 6c5f 6465 6e73 6974 795f  m local_density_
+00006070: 7468 7265 7368 6f6c 643a 2054 6872 6573  threshold: Thres
+00006080: 686f 6c64 2066 6f72 2074 6865 206c 6f63  hold for the loc
+00006090: 616c 2064 656e 7369 7479 2066 696c 7465  al density filte
+000060a0: 7269 6e67 2070 7269 6f72 2074 6f20 4745  ring prior to GE
+000060b0: 5020 636f 6e73 656e 7375 732e 2041 6363  P consensus. Acc
+000060c0: 6570 7461 626c 6520 7468 7265 7368 6f6c  eptable threshol
+000060d0: 6473 2061 7265 203e 2030 2061 6e64 203c  ds are > 0 and <
+000060e0: 3d20 3220 2832 2e30 2069 7320 6e6f 2066  = 2 (2.0 is no f
+000060f0: 696c 7465 7269 6e67 292e 2044 6566 6175  iltering). Defau
+00006100: 6c74 7320 746f 204e 6f6e 652e 0d0a 2020  lts to None...  
+00006110: 2020 2020 2020 3a74 7970 6520 6c6f 6361        :type loca
+00006120: 6c5f 6465 6e73 6974 795f 7468 7265 7368  l_density_thresh
+00006130: 6f6c 643a 2066 6c6f 6174 2c20 6f70 7469  old: float, opti
+00006140: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+00006150: 6172 616d 206c 6f63 616c 5f6e 6569 6768  aram local_neigh
+00006160: 626f 7268 6f6f 645f 7369 7a65 3a20 4672  borhood_size: Fr
+00006170: 6163 7469 6f6e 206f 6620 7468 6520 6e75  action of the nu
+00006180: 6d62 6572 206f 6620 7265 706c 6963 6174  mber of replicat
+00006190: 6573 2074 6f20 7573 6520 6173 206e 6561  es to use as nea
+000061a0: 7265 7374 206e 6569 6768 626f 7273 2066  rest neighbors f
+000061b0: 6f72 206c 6f63 616c 2064 656e 7369 7479  or local density
+000061c0: 2066 696c 7465 7269 6e67 2e20 4465 6661   filtering. Defa
+000061d0: 756c 7473 2074 6f20 4e6f 6e65 0d0a 2020  ults to None..  
+000061e0: 2020 2020 2020 3a74 7970 6520 6c6f 6361        :type loca
+000061f0: 6c5f 6e65 6967 6862 6f72 686f 6f64 5f73  l_neighborhood_s
+00006200: 697a 653a 2066 6c6f 6174 2c20 6f70 7469  ize: float, opti
+00006210: 6f6e 616c 0d0a 2020 2020 2020 2020 2222  onal..        ""
+00006220: 220d 0a20 2020 2020 2020 2073 656c 662e  "..        self.
+00006230: 6164 6174 612e 756e 735b 2263 6e6d 665f  adata.uns["cnmf_
+00006240: 6e61 6d65 225d 203d 2063 6e6d 665f 6e61  name"] = cnmf_na
+00006250: 6d65 0d0a 0d0a 2020 2020 2020 2020 2320  me....        # 
+00006260: 696e 6665 7220 6672 6f6d 2066 696c 656e  infer from filen
+00006270: 616d 6573 2077 6869 6368 206c 6f63 616c  ames which local
+00006280: 2064 656e 7369 7479 2074 6872 6573 686f   density thresho
+00006290: 6c64 2077 6173 2075 7365 640d 0a20 2020  ld was used..   
+000062a0: 2020 2020 2073 656e 7365 645f 6c64 7473       sensed_ldts
+000062b0: 203d 2073 6574 2829 0d0a 2020 2020 2020   = set()..      
+000062c0: 2020 666f 7220 666e 2069 6e20 676c 6f62    for fn in glob
+000062d0: 286f 732e 7061 7468 2e6a 6f69 6e28 636e  (os.path.join(cn
+000062e0: 6d66 5f6f 7574 7075 745f 6469 722c 2063  mf_output_dir, c
+000062f0: 6e6d 665f 6e61 6d65 2c20 6622 7b63 6e6d  nmf_name, f"{cnm
+00006300: 665f 6e61 6d65 7d2a 2e2a 7370 6563 7472  f_name}*.*spectr
+00006310: 612a 2e6b 5f2a 2229 293a 0d0a 2020 2020  a*.k_*")):..    
+00006320: 2020 2020 2020 2020 6c64 745f 7374 7220          ldt_str 
+00006330: 3d20 6f73 2e70 6174 682e 6261 7365 6e61  = os.path.basena
+00006340: 6d65 2866 6e29 2e73 706c 6974 2822 2e22  me(fn).split("."
+00006350: 295b 2d33 5d0d 0a20 2020 2020 2020 2020  )[-3]..         
+00006360: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
+00006370: 2020 2020 2020 2020 206c 6474 203d 2066           ldt = f
+00006380: 6c6f 6174 286c 6474 5f73 7472 2e72 6570  loat(ldt_str.rep
+00006390: 6c61 6365 2822 6474 5f22 2c20 2222 292e  lace("dt_", "").
+000063a0: 7265 706c 6163 6528 225f 222c 2022 2e22  replace("_", "."
+000063b0: 2929 0d0a 2020 2020 2020 2020 2020 2020  ))..            
+000063c0: 6578 6365 7074 2056 616c 7565 4572 726f  except ValueErro
+000063d0: 723a 0d0a 2020 2020 2020 2020 2020 2020  r:..            
+000063e0: 2020 2020 7061 7373 0d0a 2020 2020 2020      pass..      
+000063f0: 2020 2020 2020 656c 7365 3a0d 0a20 2020        else:..   
+00006400: 2020 2020 2020 2020 2020 2020 2073 656e               sen
+00006410: 7365 645f 6c64 7473 2e61 6464 2828 6c64  sed_ldts.add((ld
+00006420: 745f 7374 722c 206c 6474 2929 0d0a 2020  t_str, ldt))..  
+00006430: 2020 2020 2020 6966 206c 6f63 616c 5f64        if local_d
+00006440: 656e 7369 7479 5f74 6872 6573 686f 6c64  ensity_threshold
+00006450: 2069 7320 4e6f 6e65 2061 6e64 206c 656e   is None and len
+00006460: 2873 656e 7365 645f 6c64 7473 2920 3d3d  (sensed_ldts) ==
+00006470: 2031 3a0d 0a20 2020 2020 2020 2020 2020   1:..           
+00006480: 206c 6474 5f73 7472 2c20 6c64 7420 3d20   ldt_str, ldt = 
+00006490: 7365 6e73 6564 5f6c 6474 732e 706f 7028  sensed_ldts.pop(
+000064a0: 290d 0a20 2020 2020 2020 2065 6c69 6620  )..        elif 
+000064b0: 6c6f 6361 6c5f 6465 6e73 6974 795f 7468  local_density_th
+000064c0: 7265 7368 6f6c 6420 696e 2028 6c64 745b  reshold in (ldt[
+000064d0: 315d 2066 6f72 206c 6474 2069 6e20 7365  1] for ldt in se
+000064e0: 6e73 6564 5f6c 6474 7329 3a0d 0a20 2020  nsed_ldts):..   
+000064f0: 2020 2020 2020 2020 206c 6474 5f73 7472           ldt_str
+00006500: 2c20 6c64 7420 3d20 5b28 6c64 745f 7374  , ldt = [(ldt_st
+00006510: 722c 206c 6474 2920 666f 7220 6c64 745f  r, ldt) for ldt_
+00006520: 7374 722c 206c 6474 2069 6e20 7365 6e73  str, ldt in sens
+00006530: 6564 5f6c 6474 7320 6966 206c 6474 203d  ed_ldts if ldt =
+00006540: 3d20 6c6f 6361 6c5f 6465 6e73 6974 795f  = local_density_
+00006550: 7468 7265 7368 6f6c 645d 2e70 6f70 2829  threshold].pop()
+00006560: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
+00006570: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00006580: 6769 6e67 2e65 7272 6f72 2866 226c 6f63  ging.error(f"loc
+00006590: 616c 5f64 656e 7369 7479 5f74 6872 6573  al_density_thres
+000065a0: 686f 6c64 206f 6620 7b6c 6f63 616c 5f64  hold of {local_d
+000065b0: 656e 7369 7479 5f74 6872 6573 686f 6c64  ensity_threshold
+000065c0: 7d20 646f 6573 206e 6f74 206d 6174 6368  } does not match
+000065d0: 2077 6861 7420 6973 2069 6e20 7468 6520   what is in the 
+000065e0: 634e 4d46 2072 6573 756c 7420 6469 7265  cNMF result dire
+000065f0: 6374 6f72 793a 207b 7365 6e73 6564 5f6c  ctory: {sensed_l
+00006600: 6474 737d 2229 0d0a 2020 2020 2020 2020  dts}")..        
+00006610: 2020 2020 7379 732e 6578 6974 2831 290d      sys.exit(1).
+00006620: 0a20 2020 2020 2020 2073 656c 662e 6164  .        self.ad
+00006630: 6174 612e 756e 735b 226c 6474 225d 203d  ata.uns["ldt"] =
+00006640: 206c 6474 0d0a 2020 2020 2020 2020 7365   ldt..        se
+00006650: 6c66 2e61 6461 7461 2e75 6e73 5b22 6c6e  lf.adata.uns["ln
+00006660: 7322 5d20 3d20 6c6f 6361 6c5f 6e65 6967  s"] = local_neig
+00006670: 6862 6f72 686f 6f64 5f73 697a 650d 0a20  hborhood_size.. 
+00006680: 2020 2020 2020 2020 2020 200d 0a20 2020             ..   
+00006690: 2020 2020 2023 2049 6d70 6f72 7420 4745       # Import GE
+000066a0: 5073 0d0a 2020 2020 2020 2020 7265 7375  Ps..        resu
+000066b0: 6c74 5f74 7970 6573 203d 207b 0d0a 2020  lt_types = {..  
+000066c0: 2020 2020 2020 2020 2020 2267 656e 655f            "gene_
+000066d0: 7370 6563 7472 615f 7363 6f72 6522 3a20  spectra_score": 
+000066e0: 2263 6e6d 665f 6765 705f 7363 6f72 6522  "cnmf_gep_score"
+000066f0: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00006700: 6765 6e65 5f73 7065 6374 7261 5f74 706d  gene_spectra_tpm
+00006710: 223a 2022 636e 6d66 5f67 6570 5f74 706d  ": "cnmf_gep_tpm
+00006720: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
+00006730: 2273 7065 6374 7261 223a 2022 636e 6d66  "spectra": "cnmf
+00006740: 5f67 6570 5f72 6177 220d 0a20 2020 2020  _gep_raw"..     
+00006750: 2020 2020 2020 207d 0d0a 2020 2020 2020         }..      
+00006760: 2020 666f 7220 6d61 7463 6873 7472 2c20    for matchstr, 
+00006770: 7265 7375 6c74 5f74 7970 6520 696e 2072  result_type in r
+00006780: 6573 756c 745f 7479 7065 732e 6974 656d  esult_types.item
+00006790: 7328 293a 0d0a 2020 2020 2020 2020 2020  s():..          
+000067a0: 2020 6c6f 6767 696e 672e 696e 666f 2866    logging.info(f
+000067b0: 2249 6d70 6f72 7469 6e67 2047 4550 733a  "Importing GEPs:
+000067c0: 207b 6d61 7463 6873 7472 7d22 2920 200d   {matchstr}")  .
+000067d0: 0a20 2020 2020 2020 2020 2020 206d 6574  .            met
+000067e0: 615f 7720 3d20 5b5d 0d0a 2020 2020 2020  a_w = []..      
+000067f0: 2020 2020 2020 666f 7220 666e 2069 6e20        for fn in 
+00006800: 676c 6f62 286f 732e 7061 7468 2e6a 6f69  glob(os.path.joi
+00006810: 6e28 636e 6d66 5f6f 7574 7075 745f 6469  n(cnmf_output_di
+00006820: 722c 2063 6e6d 665f 6e61 6d65 2c20 6622  r, cnmf_name, f"
+00006830: 7b63 6e6d 665f 6e61 6d65 7d2a 2e7b 6d61  {cnmf_name}*.{ma
+00006840: 7463 6873 7472 7d2e 6b5f 2a2e 7b6c 6474  tchstr}.k_*.{ldt
+00006850: 5f73 7472 7d2e 2a74 7874 2229 293a 0d0a  _str}.*txt")):..
+00006860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00006870: 6b20 3d20 696e 7428 6f73 2e70 6174 682e  k = int(os.path.
+00006880: 6261 7365 6e61 6d65 2866 6e29 2e72 656d  basename(fn).rem
+00006890: 6f76 6570 7265 6669 7828 6622 7b63 6e6d  oveprefix(f"{cnm
+000068a0: 665f 6e61 6d65 7d2e 7b6d 6174 6368 7374  f_name}.{matchst
+000068b0: 727d 2e22 292e 7370 6c69 7428 222e 2229  r}.").split(".")
+000068c0: 5b30 5d2e 7265 706c 6163 6528 226b 5f22  [0].replace("k_"
+000068d0: 2c20 2222 2929 0d0a 2020 2020 2020 2020  , ""))..        
+000068e0: 2020 2020 2020 2020 7720 3d20 7064 2e72          w = pd.r
+000068f0: 6561 645f 7461 626c 6528 666e 2c20 696e  ead_table(fn, in
+00006900: 6465 785f 636f 6c3d 3029 0d0a 2020 2020  dex_col=0)..    
+00006910: 2020 2020 2020 2020 2020 2020 772e 696e              w.in
+00006920: 6465 7820 3d20 7374 7228 6b29 202b 2022  dex = str(k) + "
+00006930: 2e22 202b 2077 2e69 6e64 6578 2e61 7374  ." + w.index.ast
+00006940: 7970 6528 7374 7229 0d0a 2020 2020 2020  ype(str)..      
+00006950: 2020 2020 2020 2020 2020 6d65 7461 5f77            meta_w
+00006960: 2e61 7070 656e 6428 7729 0d0a 2020 2020  .append(w)..    
+00006970: 2020 2020 2020 2020 6d65 7461 5f77 203d          meta_w =
+00006980: 2070 642e 636f 6e63 6174 286d 6574 615f   pd.concat(meta_
+00006990: 772c 2061 7869 733d 3029 2e54 2e72 6569  w, axis=0).T.rei
+000069a0: 6e64 6578 2873 656c 662e 6164 6174 612e  ndex(self.adata.
+000069b0: 7661 722e 696e 6465 7829 2e72 656e 616d  var.index).renam
+000069c0: 655f 6178 6973 285b 226b 2e67 6570 225d  e_axis(["k.gep"]
+000069d0: 2c20 6178 6973 3d31 290d 0a20 2020 2020  , axis=1)..     
+000069e0: 2020 2020 2020 2073 656c 662e 6164 6174         self.adat
+000069f0: 612e 7661 726d 5b72 6573 756c 745f 7479  a.varm[result_ty
+00006a00: 7065 5d20 3d20 6d65 7461 5f77 0d0a 0d0a  pe] = meta_w....
+00006a10: 2020 2020 2020 2020 2320 496d 706f 7274          # Import
+00006a20: 2055 7361 6765 730d 0a20 2020 2020 2020   Usages..       
+00006a30: 206c 6f67 6769 6e67 2e69 6e66 6f28 6622   logging.info(f"
+00006a40: 496d 706f 7274 696e 6720 5573 6167 6573  Importing Usages
+00006a50: 2229 2020 0d0a 2020 2020 2020 2020 7573  ")  ..        us
+00006a60: 6167 6520 3d20 5b5d 0d0a 2020 2020 2020  age = []..      
+00006a70: 2020 666f 7220 666e 2069 6e20 676c 6f62    for fn in glob
+00006a80: 286f 732e 7061 7468 2e6a 6f69 6e28 636e  (os.path.join(cn
+00006a90: 6d66 5f6f 7574 7075 745f 6469 722c 2063  mf_output_dir, c
+00006aa0: 6e6d 665f 6e61 6d65 2c20 6622 7b63 6e6d  nmf_name, f"{cnm
+00006ab0: 665f 6e61 6d65 7d2a 2e75 7361 6765 732e  f_name}*.usages.
+00006ac0: 6b5f 2a2e 7b6c 6474 5f73 7472 7d2e 2a74  k_*.{ldt_str}.*t
+00006ad0: 7874 2229 293a 0d0a 2020 2020 2020 2020  xt")):..        
+00006ae0: 2020 2020 6b20 3d20 696e 7428 6f73 2e70      k = int(os.p
+00006af0: 6174 682e 6261 7365 6e61 6d65 2866 6e29  ath.basename(fn)
+00006b00: 2e72 656d 6f76 6570 7265 6669 7828 6622  .removeprefix(f"
+00006b10: 7b63 6e6d 665f 6e61 6d65 7d2e 7573 6167  {cnmf_name}.usag
+00006b20: 6573 2e22 292e 7370 6c69 7428 222e 2229  es.").split(".")
+00006b30: 5b30 5d2e 7265 706c 6163 6528 226b 5f22  [0].replace("k_"
+00006b40: 2c20 2222 2929 0d0a 2020 2020 2020 2020  , ""))..        
+00006b50: 2020 2020 6820 3d20 7064 2e72 6561 645f      h = pd.read_
+00006b60: 7461 626c 6528 666e 2c20 696e 6465 785f  table(fn, index_
+00006b70: 636f 6c3d 3029 0d0a 2020 2020 2020 2020  col=0)..        
+00006b80: 2020 2020 682e 636f 6c75 6d6e 7320 3d20      h.columns = 
+00006b90: 7374 7228 6b29 202b 2022 2e22 202b 2068  str(k) + "." + h
+00006ba0: 2e63 6f6c 756d 6e73 2e61 7374 7970 6528  .columns.astype(
+00006bb0: 7374 7229 0d0a 2020 2020 2020 2020 2020  str)..          
+00006bc0: 2020 7573 6167 652e 6170 7065 6e64 2868    usage.append(h
+00006bd0: 290d 0a20 2020 2020 2020 2073 656c 662e  )..        self.
+00006be0: 6164 6174 612e 6f62 736d 5b22 636e 6d66  adata.obsm["cnmf
+00006bf0: 5f75 7361 6765 225d 203d 2070 642e 636f  _usage"] = pd.co
+00006c00: 6e63 6174 2875 7361 6765 2c20 6178 6973  ncat(usage, axis
+00006c10: 3d31 292e 736f 7274 5f69 6e64 6578 2861  =1).sort_index(a
+00006c20: 7869 733d 3129 2e72 656e 616d 655f 6178  xis=1).rename_ax
+00006c30: 6973 285b 226b 2e67 6570 225d 2c20 6178  is(["k.gep"], ax
+00006c40: 6973 3d31 290d 0a20 2020 2020 2020 200d  is=1)..        .
+00006c50: 0a20 2020 2020 2020 2023 2049 6d70 6f72  .        # Impor
+00006c60: 7420 6765 6e65 206c 6973 7420 7573 6564  t gene list used
+00006c70: 2066 6f72 2066 6163 746f 7269 7a61 7469   for factorizati
+00006c80: 6f6e 0d0a 2020 2020 2020 2020 7769 7468  on..        with
+00006c90: 206f 7065 6e28 6f73 2e70 6174 682e 6a6f   open(os.path.jo
+00006ca0: 696e 2863 6e6d 665f 6f75 7470 7574 5f64  in(cnmf_output_d
+00006cb0: 6972 2c20 636e 6d66 5f6e 616d 652c 2066  ir, cnmf_name, f
+00006cc0: 227b 636e 6d66 5f6e 616d 657d 2e6f 7665  "{cnmf_name}.ove
+00006cd0: 7264 6973 7065 7273 6564 5f67 656e 6573  rdispersed_genes
+00006ce0: 2e74 7874 2229 2920 6173 2066 3a0d 0a20  .txt")) as f:.. 
+00006cf0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006d00: 6164 6174 612e 756e 735b 2267 656e 655f  adata.uns["gene_
+00006d10: 6c69 7374 225d 203d 205b 6c69 6e65 2e73  list"] = [line.s
+00006d20: 7472 6970 2829 2066 6f72 206c 696e 6520  trip() for line 
+00006d30: 696e 2066 2e72 6561 646c 696e 6573 2829  in f.readlines()
+00006d40: 5d0d 0a0d 0a20 2020 2020 2020 2023 2049  ]....        # I
+00006d50: 6d70 6f72 7420 4b2d 7365 6c65 6374 696f  mport K-selectio
+00006d60: 6e20 7374 6174 730d 0a20 2020 2020 2020  n stats..       
+00006d70: 206b 7661 6c73 203d 2070 642e 4461 7461   kvals = pd.Data
+00006d80: 4672 616d 6528 2a2a 6e70 2e6c 6f61 6428  Frame(**np.load(
+00006d90: 6f73 2e70 6174 682e 6a6f 696e 2863 6e6d  os.path.join(cnm
+00006da0: 665f 6f75 7470 7574 5f64 6972 2c20 636e  f_output_dir, cn
+00006db0: 6d66 5f6e 616d 652c 2066 227b 636e 6d66  mf_name, f"{cnmf
+00006dc0: 5f6e 616d 657d 2e6b 5f73 656c 6563 7469  _name}.k_selecti
+00006dd0: 6f6e 5f73 7461 7473 2e64 662e 6e70 7a22  on_stats.df.npz"
+00006de0: 292c 2061 6c6c 6f77 5f70 6963 6b6c 653d  ), allow_pickle=
+00006df0: 5472 7565 2929 2e73 6574 5f69 6e64 6578  True)).set_index
+00006e00: 2822 6b22 295b 5b22 7374 6162 696c 6974  ("k")[["stabilit
+00006e10: 7922 2c20 2270 7265 6469 6374 696f 6e5f  y", "prediction_
+00006e20: 6572 726f 7222 5d5d 0d0a 2020 2020 2020  error"]]..      
+00006e30: 2020 6b76 616c 732e 696e 6465 7820 3d20    kvals.index = 
+00006e40: 6b76 616c 732e 696e 6465 782e 6173 7479  kvals.index.asty
+00006e50: 7065 2869 6e74 290d 0a20 2020 2020 2020  pe(int)..       
+00006e60: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+00006e70: 226b 7661 6c73 225d 203d 206b 7661 6c73  "kvals"] = kvals
+00006e80: 0d0a 2020 2020 2020 2020 7365 6c66 2e61  ..        self.a
+00006e90: 7070 656e 645f 746f 5f68 6973 746f 7279  ppend_to_history
+00006ea0: 2822 634e 4d46 2072 6573 756c 7473 2061  ("cNMF results a
+00006eb0: 6464 6564 2066 726f 6d20 6f75 7470 7574  dded from output
+00006ec0: 2064 6972 6563 746f 7279 207b 636e 6d66   directory {cnmf
+00006ed0: 5f6f 7574 7075 745f 6469 727d 2f7b 636e  _output_dir}/{cn
+00006ee0: 6d66 5f6e 616d 657d 2229 0d0a 0d0a 2020  mf_name}")....  
+00006ef0: 2020 6465 6620 6765 745f 7573 6167 6573    def get_usages
+00006f00: 2873 656c 662c 0d0a 2020 2020 2020 2020  (self,..        
+00006f10: 2020 2020 2020 2020 2020 206b 3a20 556e             k: Un
+00006f20: 696f 6e5b 696e 742c 2049 7465 7261 626c  ion[int, Iterabl
+00006f30: 655d 203d 204e 6f6e 652c 0d0a 2020 2020  e] = None,..    
+00006f40: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00006f50: 6973 6372 6574 697a 653a 2062 6f6f 6c20  iscretize: bool 
+00006f60: 3d20 4661 6c73 652c 0d0a 2020 2020 2020  = False,..      
+00006f70: 2020 2020 2020 2020 2020 2020 206e 6f72               nor
+00006f80: 6d61 6c69 7a65 3a20 626f 6f6c 203d 2046  malize: bool = F
+00006f90: 616c 7365 0d0a 2020 2020 2020 2020 2020  alse..          
+00006fa0: 2020 2020 2020 2020 2029 202d 3e20 7064           ) -> pd
+00006fb0: 2e44 6174 6146 7261 6d65 3a0d 0a20 2020  .DataFrame:..   
+00006fc0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00006fd0: 2020 4361 6c63 756c 6174 6520 7573 6167    Calculate usag
+00006fe0: 6520 6f66 2065 6163 6820 4745 5020 696e  e of each GEP in
+00006ff0: 2065 6163 6820 7361 6d70 6c65 2f6f 6273   each sample/obs
+00007000: 6572 7661 7469 6f6e 2e0d 0a0d 0a20 2020  ervation.....   
+00007010: 2020 2020 203a 7061 7261 6d20 6b3a 2049       :param k: I
+00007020: 6620 616e 2069 6e74 6567 6572 206f 7220  f an integer or 
+00007030: 6c69 7374 206f 6620 696e 7465 6765 7273  list of integers
+00007040: 2c20 7265 7475 726e 7320 7573 6167 6573  , returns usages
+00007050: 206f 6e6c 7920 666f 7220 7370 6563 6966   only for specif
+00007060: 6965 6420 7261 6e6b 732e 204f 7468 6572  ied ranks. Other
+00007070: 7769 7365 2c20 7265 7475 726e 7320 7573  wise, returns us
+00007080: 6167 6520 6f66 2061 6c6c 2047 4550 7320  age of all GEPs 
+00007090: 6163 726f 7373 2072 616e 6b73 2e20 4465  across ranks. De
+000070a0: 6661 756c 7473 2074 6f20 4e6f 6e65 0d0a  faults to None..
+000070b0: 2020 2020 2020 2020 3a74 7970 6520 6b3a          :type k:
+000070c0: 2069 6e74 2c20 6f70 7469 6f6e 616c 0d0a   int, optional..
+000070d0: 2020 2020 2020 2020 3a70 6172 616d 2064          :param d
+000070e0: 6973 6372 6574 697a 653a 2044 6973 6372  iscretize: Discr
+000070f0: 6574 697a 6573 2074 6865 2075 7361 6765  etizes the usage
+00007100: 206d 6174 7269 7820 7375 6368 2074 6861   matrix such tha
+00007110: 7420 666f 7220 6561 6368 2076 616c 7565  t for each value
+00007120: 206f 6620 6b2c 2065 6163 6820 7361 6d70   of k, each samp
+00007130: 6c65 2068 6173 2075 7361 6765 206f 6620  le has usage of 
+00007140: 6f6e 6c79 2031 2047 4550 2028 7468 6520  only 1 GEP (the 
+00007150: 6f6e 6520 7769 7468 2074 6865 206d 6178  one with the max
+00007160: 696d 756d 2075 7361 6765 292e 2044 6566  imum usage). Def
+00007170: 6175 6c74 7320 746f 2046 616c 7365 0d0a  aults to False..
+00007180: 2020 2020 2020 2020 3a74 7970 6520 6469          :type di
+00007190: 7363 7265 7469 7a65 3a20 626f 6f6c 2c20  scretize: bool, 
+000071a0: 6f70 7469 6f6e 616c 0d0a 2020 2020 2020  optional..      
+000071b0: 2020 3a70 6172 616d 206e 6f72 6d61 6c69    :param normali
+000071c0: 7a65 3a20 4e6f 726d 616c 697a 6520 7468  ze: Normalize th
+000071d0: 6520 4745 5020 7573 6167 6520 6d61 7472  e GEP usage matr
+000071e0: 6978 2073 7563 6820 7468 6174 2066 6f72  ix such that for
+000071f0: 2065 6163 6820 7661 6c75 6520 6f66 206b   each value of k
+00007200: 2c20 7573 6167 6520 6f66 2061 6c6c 2047  , usage of all G
+00007210: 4550 7320 7375 6d73 2074 6f20 312e 2044  EPs sums to 1. D
+00007220: 6566 6175 6c74 7320 746f 2046 616c 7365  efaults to False
+00007230: 0d0a 2020 2020 2020 2020 3a74 7970 6520  ..        :type 
+00007240: 6e6f 726d 616c 697a 653a 2062 6f6f 6c2c  normalize: bool,
+00007250: 206f 7074 696f 6e61 6c0d 0a20 2020 2020   optional..     
+00007260: 2020 203a 7265 7475 726e 3a20 6f62 7365     :return: obse
+00007270: 7276 6174 696f 6e20 c397 2047 4550 206d  rvation .. GEP m
+00007280: 6174 7269 780d 0a20 2020 2020 2020 203a  atrix..        :
+00007290: 7274 7970 653a 2070 642e 4461 7461 4672  rtype: pd.DataFr
+000072a0: 616d 650d 0a20 2020 2020 2020 2022 2222  ame..        """
+000072b0: 0d0a 2020 2020 2020 2020 6466 203d 2073  ..        df = s
+000072c0: 656c 662e 6164 6174 612e 6f62 736d 5b22  elf.adata.obsm["
+000072d0: 636e 6d66 5f75 7361 6765 225d 2e63 6f70  cnmf_usage"].cop
+000072e0: 7928 290d 0a20 2020 2020 2020 2064 662e  y()..        df.
+000072f0: 636f 6c75 6d6e 7320 3d20 7064 2e4d 756c  columns = pd.Mul
+00007300: 7469 496e 6465 782e 6672 6f6d 5f74 7570  tiIndex.from_tup
+00007310: 6c65 7328 6466 2e63 6f6c 756d 6e73 2e73  les(df.columns.s
+00007320: 7472 2e73 706c 6974 2822 2e22 292e 746f  tr.split(".").to
+00007330: 5f6c 6973 7428 2929 0d0a 2020 2020 2020  _list())..      
+00007340: 2020 6466 2e63 6f6c 756d 6e73 203d 2064    df.columns = d
+00007350: 662e 636f 6c75 6d6e 732e 7365 745f 6c65  f.columns.set_le
+00007360: 7665 6c73 285b 6c2e 6173 7479 7065 2822  vels([l.astype("
+00007370: 696e 7422 2920 666f 7220 6c20 696e 2064  int") for l in d
+00007380: 662e 636f 6c75 6d6e 732e 6c65 7665 6c73  f.columns.levels
+00007390: 5d29 0d0a 2020 2020 2020 2020 6966 206e  ])..        if n
+000073a0: 6f72 6d61 6c69 7a65 3a0d 0a20 2020 2020  ormalize:..     
+000073b0: 2020 2020 2020 206e 6f72 6d61 6c69 7a65         normalize
+000073c0: 6420 3d20 5b5d 0d0a 2020 2020 2020 2020  d = []..        
+000073d0: 2020 2020 666f 7220 5f2c 2073 7562 6466      for _, subdf
+000073e0: 2069 6e20 6466 2e67 726f 7570 6279 2861   in df.groupby(a
+000073f0: 7869 733d 312c 206c 6576 656c 3d30 293a  xis=1, level=0):
+00007400: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007410: 2020 6e6f 726d 616c 697a 6564 2e61 7070    normalized.app
+00007420: 656e 6428 7375 6264 662e 6469 7628 7375  end(subdf.div(su
+00007430: 6264 662e 7375 6d28 6178 6973 3d31 292c  bdf.sum(axis=1),
+00007440: 2061 7869 733d 3029 290d 0a20 2020 2020   axis=0))..     
+00007450: 2020 2020 2020 2064 6620 3d20 7064 2e63         df = pd.c
+00007460: 6f6e 6361 7428 6e6f 726d 616c 697a 6564  oncat(normalized
+00007470: 2c20 6178 6973 3d31 290d 0a20 2020 2020  , axis=1)..     
+00007480: 2020 2069 6620 6469 7363 7265 7469 7a65     if discretize
+00007490: 3a0d 0a20 2020 2020 2020 2020 2020 2064  :..            d
+000074a0: 6973 6372 6574 697a 6564 203d 205b 5d0d  iscretized = [].
+000074b0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+000074c0: 205f 2c20 7375 6264 6620 696e 2064 662e   _, subdf in df.
+000074d0: 6772 6f75 7062 7928 6178 6973 3d31 2c20  groupby(axis=1, 
+000074e0: 6c65 7665 6c3d 3029 3a0d 0a20 2020 2020  level=0):..     
+000074f0: 2020 2020 2020 2020 2020 2064 6973 6372             discr
+00007500: 6574 697a 6564 2e61 7070 656e 6428 7375  etized.append(su
+00007510: 6264 662e 6571 2873 7562 6466 2e6d 6178  bdf.eq(subdf.max
+00007520: 2861 7869 733d 3129 2c20 6178 6973 3d30  (axis=1), axis=0
+00007530: 292e 6173 7479 7065 2869 6e74 2929 0d0a  ).astype(int))..
+00007540: 2020 2020 2020 2020 2020 2020 6466 203d              df =
+00007550: 2070 642e 636f 6e63 6174 2864 6973 6372   pd.concat(discr
+00007560: 6574 697a 6564 2c20 6178 6973 3d31 2920  etized, axis=1) 
+00007570: 2020 2020 2020 200d 0a20 2020 2020 2020         ..       
+00007580: 2069 6620 6b20 6973 206e 6f74 204e 6f6e   if k is not Non
+00007590: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+000075a0: 6466 203d 2064 662e 6c6f 635b 3a2c 206b  df = df.loc[:, k
+000075b0: 5d0d 0a20 2020 2020 2020 2064 6620 3d20  ]..        df = 
+000075c0: 6466 2e73 6f72 745f 696e 6465 7828 6178  df.sort_index(ax
+000075d0: 6973 3d30 292e 736f 7274 5f69 6e64 6578  is=0).sort_index
+000075e0: 2861 7869 733d 3129 2020 200d 0a20 2020  (axis=1)   ..   
+000075f0: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
+00007600: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
+00007610: 745f 6765 7073 2873 656c 662c 0d0a 2020  t_geps(self,..  
+00007620: 2020 2020 2020 2020 2020 2020 2020 206b                 k
+00007630: 3a20 556e 696f 6e5b 696e 742c 2049 7465  : Union[int, Ite
+00007640: 7261 626c 655d 203d 204e 6f6e 652c 0d0a  rable] = None,..
+00007650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007660: 2074 7970 653d 2263 6e6d 665f 6765 705f   type="cnmf_gep_
+00007670: 7363 6f72 6522 0d0a 2020 2020 2020 2020  score"..        
+00007680: 2020 2020 2020 2020 2029 202d 3e20 7064           ) -> pd
+00007690: 2e44 6174 6146 7261 6d65 3a0d 0a20 2020  .DataFrame:..   
+000076a0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+000076b0: 2020 4765 7420 4745 5073 2e0d 0a0d 0a20    Get GEPs..... 
+000076c0: 2020 2020 2020 203a 7061 7261 6d20 6b3a         :param k:
+000076d0: 2049 6620 616e 2069 6e74 6567 6572 206f   If an integer o
+000076e0: 7220 6c69 7374 206f 6620 696e 7465 6765  r list of intege
+000076f0: 7273 2c20 7265 7475 726e 7320 4745 5073  rs, returns GEPs
+00007700: 206f 6e6c 7920 666f 7220 7370 6563 6966   only for specif
+00007710: 6965 6420 7261 6e6b 732e 204f 7468 6572  ied ranks. Other
+00007720: 7769 7365 2c20 7265 7475 726e 7320 4745  wise, returns GE
+00007730: 5073 2066 726f 6d20 616c 6c20 7261 6e6b  Ps from all rank
+00007740: 732e 2044 6566 6175 6c74 7320 746f 204e  s. Defaults to N
+00007750: 6f6e 650d 0a20 2020 2020 2020 203a 7479  one..        :ty
+00007760: 7065 206b 3a20 556e 696f 6e5b 696e 742c  pe k: Union[int,
+00007770: 2049 7465 7261 626c 655d 2c20 6f70 7469   Iterable], opti
+00007780: 6f6e 616c 0d0a 2020 2020 2020 2020 3a70  onal..        :p
+00007790: 6172 616d 2074 7970 653a 2022 636e 6d66  aram type: "cnmf
+000077a0: 5f67 6570 5f73 636f 7265 2220 6f72 2022  _gep_score" or "
+000077b0: 636e 6d66 5f67 6570 5f74 706d 222c 2064  cnmf_gep_tpm", d
+000077c0: 6566 6175 6c74 7320 746f 2022 636e 6d66  efaults to "cnmf
+000077d0: 5f67 6570 5f73 636f 7265 220d 0a20 2020  _gep_score"..   
+000077e0: 2020 2020 203a 7479 7065 2074 7970 653a       :type type:
+000077f0: 2073 7472 2c20 6f70 7469 6f6e 616c 0d0a   str, optional..
+00007800: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00007810: 2066 6561 7475 7265 7320 c397 2047 4550   features .. GEP
+00007820: 206d 6174 7269 780d 0a20 2020 2020 2020   matrix..       
+00007830: 203a 7274 7970 653a 2070 642e 4461 7461   :rtype: pd.Data
+00007840: 4672 616d 650d 0a20 2020 2020 2020 2022  Frame..        "
+00007850: 2222 0d0a 2020 2020 2020 2020 6466 203d  ""..        df =
+00007860: 2073 656c 662e 6164 6174 612e 7661 726d   self.adata.varm
+00007870: 5b74 7970 655d 2e63 6f70 7928 290d 0a20  [type].copy().. 
+00007880: 2020 2020 2020 2064 662e 636f 6c75 6d6e         df.column
+00007890: 7320 3d20 7064 2e4d 756c 7469 496e 6465  s = pd.MultiInde
+000078a0: 782e 6672 6f6d 5f74 7570 6c65 7328 6466  x.from_tuples(df
+000078b0: 2e63 6f6c 756d 6e73 2e73 7472 2e73 706c  .columns.str.spl
+000078c0: 6974 2822 2e22 292e 746f 5f6c 6973 7428  it(".").to_list(
+000078d0: 2929 0d0a 2020 2020 2020 2020 6466 2e63  ))..        df.c
+000078e0: 6f6c 756d 6e73 203d 2064 662e 636f 6c75  olumns = df.colu
+000078f0: 6d6e 732e 7365 745f 6c65 7665 6c73 285b  mns.set_levels([
+00007900: 6c2e 6173 7479 7065 2822 696e 7422 2920  l.astype("int") 
+00007910: 666f 7220 6c20 696e 2064 662e 636f 6c75  for l in df.colu
+00007920: 6d6e 732e 6c65 7665 6c73 5d29 0d0a 2020  mns.levels])..  
+00007930: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00007940: 6e63 6528 6b2c 2028 696e 742c 2049 7465  nce(k, (int, Ite
+00007950: 7261 626c 6529 293a 0d0a 2020 2020 2020  rable)):..      
+00007960: 2020 2020 2020 6466 203d 2064 662e 6c6f        df = df.lo
+00007970: 635b 3a2c 206b 5d0d 0a20 2020 2020 2020  c[:, k]..       
+00007980: 2064 6620 3d20 6466 2e73 6f72 745f 696e   df = df.sort_in
+00007990: 6465 7828 6178 6973 3d31 290d 0a20 2020  dex(axis=1)..   
+000079a0: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
+000079b0: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
+000079c0: 745f 6d65 7461 6461 7461 5f64 6628 7365  t_metadata_df(se
+000079d0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+000079e0: 2020 2020 2020 2020 2020 2020 2069 6e63               inc
+000079f0: 6c75 6465 5f63 6174 6567 6f72 6963 616c  lude_categorical
+00007a00: 3a20 626f 6f6c 203d 2054 7275 652c 0d0a  : bool = True,..
+00007a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a20: 2020 2020 2020 2020 696e 636c 7564 655f          include_
+00007a30: 6e75 6d65 7269 6361 6c3a 2062 6f6f 6c20  numerical: bool 
+00007a40: 3d20 5472 7565 0d0a 2020 2020 2020 2020  = True..        
+00007a50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007a60: 2920 2d3e 2070 642e 4461 7461 4672 616d  ) -> pd.DataFram
+00007a70: 653a 0d0a 2020 2020 2020 2020 2222 2247  e:..        """G
+00007a80: 6574 2073 616d 706c 652f 6f62 7365 7276  et sample/observ
+00007a90: 6174 696f 6e20 6d65 7461 6461 7461 2e0d  ation metadata..
+00007aa0: 0a0d 0a20 2020 2020 2020 203a 7061 7261  ...        :para
+00007ab0: 6d20 696e 636c 7564 655f 6361 7465 676f  m include_catego
+00007ac0: 7269 6361 6c3a 2049 6e63 6c75 6465 2063  rical: Include c
+00007ad0: 6174 6567 6f72 6963 616c 206d 6574 6164  ategorical metad
+00007ae0: 6174 6120 6c61 7965 7273 2c20 6465 6661  ata layers, defa
+00007af0: 756c 7473 2074 6f20 5472 7565 0d0a 2020  ults to True..  
+00007b00: 2020 2020 2020 3a74 7970 6520 696e 636c        :type incl
+00007b10: 7564 655f 6361 7465 676f 7269 6361 6c3a  ude_categorical:
+00007b20: 2062 6f6f 6c2c 206f 7074 696f 6e61 6c0d   bool, optional.
+00007b30: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00007b40: 696e 636c 7564 655f 6e75 6d65 7269 6361  include_numerica
+00007b50: 6c3a 2049 6e63 6c75 6465 206e 756d 6572  l: Include numer
+00007b60: 6963 616c 206d 6574 6164 6174 6120 6c61  ical metadata la
+00007b70: 7965 7273 2c20 6465 6661 756c 7473 2074  yers, defaults t
+00007b80: 6f20 5472 7565 0d0a 2020 2020 2020 2020  o True..        
+00007b90: 3a74 7970 6520 696e 636c 7564 655f 6e75  :type include_nu
+00007ba0: 6d65 7269 6361 6c3a 2062 6f6f 6c2c 206f  merical: bool, o
+00007bb0: 7074 696f 6e61 6c0d 0a20 2020 2020 2020  ptional..       
+00007bc0: 203a 7261 6973 6573 2056 616c 7565 4572   :raises ValueEr
+00007bd0: 726f 723a 2045 7272 6f72 2069 6620 6d65  ror: Error if me
+00007be0: 7461 6461 7461 2074 7970 6573 2061 7265  tadata types are
+00007bf0: 206e 6f74 2072 6563 6f67 6e69 7a65 640d   not recognized.
+00007c00: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+00007c10: 3a20 6f62 7365 7276 6174 696f 6e73 20c3  : observations .
+00007c20: 9720 6d65 7461 6461 7461 206d 6174 7269  . metadata matri
+00007c30: 780d 0a20 2020 2020 2020 203a 7274 7970  x..        :rtyp
+00007c40: 653a 2070 642e 4461 7461 4672 616d 650d  e: pd.DataFrame.
+00007c50: 0a20 2020 2020 2020 2022 2222 0d0a 2020  .        """..  
+00007c60: 2020 2020 2020 6474 7970 6573 203d 205b        dtypes = [
+00007c70: 5d0d 0a20 2020 2020 2020 2069 6620 696e  ]..        if in
+00007c80: 636c 7564 655f 6361 7465 676f 7269 6361  clude_categorica
+00007c90: 6c3a 0d0a 2020 2020 2020 2020 2020 2020  l:..            
+00007ca0: 6474 7970 6573 2e61 7070 656e 6428 2263  dtypes.append("c
+00007cb0: 6174 6567 6f72 7922 290d 0a20 2020 2020  ategory")..     
+00007cc0: 2020 2069 6620 696e 636c 7564 655f 6e75     if include_nu
+00007cd0: 6d65 7269 6361 6c3a 0d0a 2020 2020 2020  merical:..      
+00007ce0: 2020 2020 2020 6474 7970 6573 202b 3d20        dtypes += 
+00007cf0: 5b22 666c 6f61 7422 2c20 2269 6e74 225d  ["float", "int"]
+00007d00: 0d0a 2020 2020 2020 2020 756e 6578 706c  ..        unexpl
+00007d10: 6169 6e65 645f 636f 6c73 203d 2073 656c  ained_cols = sel
+00007d20: 662e 6164 6174 612e 6f62 732e 7365 6c65  f.adata.obs.sele
+00007d30: 6374 5f64 7479 7065 7328 6578 636c 7564  ct_dtypes(exclud
+00007d40: 653d 2822 6361 7465 676f 7279 222c 2022  e=("category", "
+00007d50: 666c 6f61 7422 2c20 2269 6e74 2229 292e  float", "int")).
+00007d60: 636f 6c75 6d6e 730d 0a20 2020 2020 2020  columns..       
+00007d70: 2069 6620 6c65 6e28 756e 6578 706c 6169   if len(unexplai
+00007d80: 6e65 645f 636f 6c73 2920 3e20 303a 0d0a  ned_cols) > 0:..
+00007d90: 2020 2020 2020 2020 2020 2020 756e 6578              unex
+00007da0: 706c 6169 6e65 645f 636f 6c5f 7374 7220  plained_col_str 
+00007db0: 3d20 222c 2022 2e6a 6f69 6e28 756e 6578  = ", ".join(unex
+00007dc0: 706c 6169 6e65 645f 636f 6c73 290d 0a20  plained_cols).. 
+00007dd0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
+00007de0: 2056 616c 7565 4572 726f 7228 6622 7b75   ValueError(f"{u
+00007df0: 6e65 7870 6c61 696e 6564 5f63 6f6c 5f73  nexplained_col_s
+00007e00: 7472 7d20 6d65 7461 6461 7461 2063 6f6c  tr} metadata col
+00007e10: 756d 6e73 2068 6176 6520 756e 7265 636f  umns have unreco
+00007e20: 676e 697a 6564 2064 7479 7065 732e 2229  gnized dtypes.")
+00007e30: 0d0a 2020 2020 2020 2020 6466 203d 2073  ..        df = s
+00007e40: 656c 662e 6164 6174 612e 6f62 732e 7365  elf.adata.obs.se
+00007e50: 6c65 6374 5f64 7479 7065 7328 696e 636c  lect_dtypes(incl
+00007e60: 7564 653d 6474 7970 6573 290d 0a20 2020  ude=dtypes)..   
+00007e70: 2020 2020 2072 6574 7572 6e20 6466 0d0a       return df..
+00007e80: 2020 2020 0d0a 2020 2020 6465 6620 6765      ..    def ge
+00007e90: 745f 6361 7465 676f 7279 5f6f 7665 7272  t_category_overr
+00007ea0: 6570 7265 7365 6e74 6174 696f 6e28 7365  epresentation(se
+00007eb0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+00007ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007ed0: 2020 2020 2020 2020 2020 2020 206c 6179               lay
+00007ee0: 6572 3a20 7374 722c 0d0a 2020 2020 2020  er: str,..      
 00007ef0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f00: 2020 2020 7472 756e 6361 7465 5f6e 6567      truncate_neg
-00007f10: 6174 6976 653a 2062 6f6f 6c20 3d20 5472  ative: bool = Tr
-00007f20: 7565 0d0a 2020 2020 2020 2020 2020 2020  ue..            
-00007f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007f40: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
-00007f50: 2070 642e 4461 7461 4672 616d 653a 0d0a   pd.DataFrame:..
-00007f60: 2020 2020 2020 2020 2222 2243 616c 6375          """Calcu
-00007f70: 6c61 7465 2050 6561 7273 6f6e 2072 6573  late Pearson res
-00007f80: 6964 7561 6c20 6f66 2063 6869 2d73 7175  idual of chi-squ
-00007f90: 6172 6564 2074 6573 742c 2061 7373 6f63  ared test, assoc
-00007fa0: 6961 7469 6e67 2047 4550 7320 666f 7220  iating GEPs for 
-00007fb0: 6561 6368 2072 616e 6b20 286b 2920 746f  each rank (k) to
-00007fc0: 2063 6174 6567 6f72 6965 7320 6f66 2073   categories of s
-00007fd0: 616d 706c 6573 2f6f 6273 6572 7661 7469  amples/observati
-00007fe0: 6f6e 732e 2042 7920 6465 6661 756c 742c  ons. By default,
-00007ff0: 2074 7275 6e63 6174 6573 206e 6567 6174   truncates negat
-00008000: 6976 6520 7661 6c75 6573 2e0d 0a0d 0a20  ive values..... 
-00008010: 2020 2020 2020 203a 7061 7261 6d20 6c61         :param la
-00008020: 7965 723a 206e 616d 6520 6f66 2063 6174  yer: name of cat
-00008030: 6567 6f72 6963 616c 2064 6174 6120 6c61  egorical data la
-00008040: 7965 720d 0a20 2020 2020 2020 203a 7479  yer..        :ty
-00008050: 7065 206c 6179 6572 3a20 7374 720d 0a20  pe layer: str.. 
-00008060: 2020 2020 2020 203a 7061 7261 6d20 7472         :param tr
-00008070: 756e 6361 7465 5f6e 6567 6174 6976 653a  uncate_negative:
-00008080: 2054 7275 6e63 6174 6520 6e65 6761 7469   Truncate negati
-00008090: 7665 2072 6573 6964 7561 6c73 2074 6f20  ve residuals to 
-000080a0: 302c 2064 6566 6175 6c74 7320 746f 2054  0, defaults to T
-000080b0: 7275 650d 0a20 2020 2020 2020 203a 7479  rue..        :ty
-000080c0: 7065 2074 7275 6e63 6174 655f 6e65 6761  pe truncate_nega
-000080d0: 7469 7665 3a20 626f 6f6c 2c20 6f70 7469  tive: bool, opti
-000080e0: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
-000080f0: 6574 7572 6e3a 2063 6174 6567 6f72 7920  eturn: category 
-00008100: c397 2047 4550 206d 6174 7269 7820 6f66  .. GEP matrix of
-00008110: 206f 7665 7272 6570 7265 7365 6e74 6174   overrepresentat
-00008120: 696f 6e20 7661 6c75 6573 0d0a 2020 2020  ion values..    
-00008130: 2020 2020 3a72 7479 7065 3a20 7064 2e44      :rtype: pd.D
-00008140: 6174 6146 7261 6d65 0d0a 2020 2020 2020  ataFrame..      
-00008150: 2020 2222 220d 0a20 2020 2020 2020 2075    """..        u
-00008160: 7361 6765 203d 2073 656c 662e 6765 745f  sage = self.get_
-00008170: 7573 6167 6573 2829 2e63 6f70 7928 290d  usages().copy().
-00008180: 0a20 2020 2020 2020 2073 616d 706c 655f  .        sample_
-00008190: 746f 5f63 6c61 7373 203d 2073 656c 662e  to_class = self.
-000081a0: 6765 745f 6d65 7461 6461 7461 5f64 6628  get_metadata_df(
-000081b0: 295b 6c61 7965 725d 0d0a 2020 2020 2020  )[layer]..      
-000081c0: 2020 7573 6167 652e 696e 6465 7820 3d20    usage.index = 
-000081d0: 7573 6167 652e 696e 6465 782e 6d61 7028  usage.index.map(
-000081e0: 7361 6d70 6c65 5f74 6f5f 636c 6173 7329  sample_to_class)
-000081f0: 0d0a 2020 2020 2020 2020 6f62 7365 7276  ..        observ
-00008200: 6564 203d 2075 7361 6765 2e67 726f 7570  ed = usage.group
-00008210: 6279 2861 7869 733d 302c 206c 6576 656c  by(axis=0, level
-00008220: 3d30 292e 7375 6d28 290d 0a20 2020 2020  =0).sum()..     
-00008230: 2020 2065 7870 6563 7465 6420 3d20 5b5d     expected = []
-00008240: 0d0a 2020 2020 2020 2020 666f 7220 6b2c  ..        for k,
-00008250: 206f 6273 5f6b 2069 6e20 6f62 7365 7276   obs_k in observ
-00008260: 6564 2e67 726f 7570 6279 2861 7869 733d  ed.groupby(axis=
-00008270: 312c 206c 6576 656c 3d31 293a 0d0a 2020  1, level=1):..  
-00008280: 2020 2020 2020 2020 2020 6578 705f 6b20            exp_k 
-00008290: 3d20 7064 2e44 6174 6146 7261 6d65 286f  = pd.DataFrame(o
-000082a0: 6273 5f6b 2e73 756d 2861 7869 733d 3129  bs_k.sum(axis=1)
-000082b0: 2920 4020 7064 2e44 6174 6146 7261 6d65  ) @ pd.DataFrame
-000082c0: 286f 6273 5f6b 2e73 756d 2861 7869 733d  (obs_k.sum(axis=
-000082d0: 3029 292e 5420 2f20 6f62 735f 6b2e 7375  0)).T / obs_k.su
-000082e0: 6d28 292e 7375 6d28 290d 0a20 2020 2020  m().sum()..     
-000082f0: 2020 2020 2020 2065 7870 6563 7465 642e         expected.
-00008300: 6170 7065 6e64 2865 7870 5f6b 290d 0a20  append(exp_k).. 
-00008310: 2020 2020 2020 2065 7870 6563 7465 6420         expected 
-00008320: 3d20 7064 2e63 6f6e 6361 7428 6578 7065  = pd.concat(expe
-00008330: 6374 6564 2c20 6178 6973 3d31 290d 0a20  cted, axis=1).. 
-00008340: 2020 2020 2020 2063 6869 7371 5f72 6573         chisq_res
-00008350: 6964 203d 2028 6f62 7365 7276 6564 202d  id = (observed -
-00008360: 2065 7870 6563 7465 6429 202f 206e 702e   expected) / np.
-00008370: 7371 7274 2865 7870 6563 7465 6429 2020  sqrt(expected)  
-00008380: 2320 7065 6172 736f 6e20 7265 7369 6475  # pearson residu
-00008390: 616c 206f 6620 6368 692d 7371 7561 7265  al of chi-square
-000083a0: 6420 7465 7374 206f 6620 636f 6e74 696e  d test of contin
-000083b0: 6765 6e63 7920 7461 626c 650d 0a20 2020  gency table..   
-000083c0: 2020 2020 2069 6620 7472 756e 6361 7465       if truncate
-000083d0: 5f6e 6567 6174 6976 653a 0d0a 2020 2020  _negative:..    
-000083e0: 2020 2020 2020 2020 6368 6973 715f 7265          chisq_re
-000083f0: 7369 6420 3d20 6368 6973 715f 7265 7369  sid = chisq_resi
-00008400: 642e 636c 6970 286c 6f77 6572 3d30 290d  d.clip(lower=0).
-00008410: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00008420: 6368 6973 715f 7265 7369 640d 0a20 2020  chisq_resid..   
-00008430: 200d 0a20 2020 2020 2020 200d 0a20 2020   ..        ..   
-00008440: 2064 6566 2067 6574 5f6d 6574 6164 6174   def get_metadat
-00008450: 615f 636f 7272 656c 6174 696f 6e28 7365  a_correlation(se
-00008460: 6c66 2c20 0d0a 2020 2020 2020 2020 2020  lf, ..          
-00008470: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008480: 2020 2020 2020 206c 6179 6572 3a20 7374         layer: st
-00008490: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-000084a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084b0: 2020 2020 206d 6574 686f 643a 2073 7472       method: str
-000084c0: 203d 2022 7065 6172 736f 6e22 0d0a 2020   = "pearson"..  
-000084d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000084e0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-000084f0: 202d 3e20 7064 2e53 6572 6965 733a 0d0a   -> pd.Series:..
-00008500: 2020 2020 2020 2020 2222 2243 616c 6375          """Calcu
-00008510: 6c61 7465 2050 6561 7273 6f6e 2063 6f72  late Pearson cor
-00008520: 7265 6c61 7469 6f6e 206f 6620 4745 5020  relation of GEP 
-00008530: 7573 6167 6520 746f 206e 756d 6572 6963  usage to numeric
-00008540: 616c 206d 6574 6164 6174 6120 6163 726f  al metadata acro
-00008550: 7373 2073 616d 706c 6573 2f6f 6273 6572  ss samples/obser
-00008560: 7661 7469 6f6e 732e 0d0a 0d0a 2020 2020  vations.....    
-00008570: 2020 2020 3a70 6172 616d 206c 6179 6572      :param layer
-00008580: 3a20 6e61 6d65 206f 6620 6e75 6d65 7269  : name of numeri
-00008590: 6361 6c20 6461 7461 206c 6179 6572 0d0a  cal data layer..
-000085a0: 2020 2020 2020 2020 3a74 7970 6520 6c61          :type la
-000085b0: 7965 723a 2073 7472 0d0a 2020 2020 2020  yer: str..      
-000085c0: 2020 3a70 6172 616d 206d 6574 686f 643a    :param method:
-000085d0: 2043 6f72 7265 6c61 7469 6f6e 206d 6574   Correlation met
-000085e0: 686f 643a 2022 7065 6172 736f 6e22 2c20  hod: "pearson", 
-000085f0: 2273 7065 6172 6d61 6e22 2c20 6f72 2022  "spearman", or "
-00008600: 6b65 6e64 616c 6c22 2e20 4465 6661 756c  kendall". Defaul
-00008610: 7473 2074 6f20 2270 6561 7273 6f6e 220d  ts to "pearson".
-00008620: 0a20 2020 2020 2020 203a 7479 7065 206d  .        :type m
-00008630: 6574 686f 643a 2073 7472 2c20 6f70 7469  ethod: str, opti
-00008640: 6f6e 616c 0d0a 2020 2020 2020 2020 3a72  onal..        :r
-00008650: 6574 7572 6e3a 2063 6f72 7265 6c61 7469  eturn: correlati
-00008660: 6f6e 206f 6620 4745 5020 746f 206d 6574  on of GEP to met
-00008670: 6164 6174 610d 0a20 2020 2020 2020 203a  adata..        :
-00008680: 7274 7970 653a 2070 642e 5365 7269 6573  rtype: pd.Series
-00008690: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
-000086a0: 2020 2020 2020 2075 7361 6765 203d 2073         usage = s
-000086b0: 656c 662e 6765 745f 7573 6167 6573 2829  elf.get_usages()
-000086c0: 2e63 6f70 7928 290d 0a20 2020 2020 2020  .copy()..       
-000086d0: 206d 6574 6164 6174 6120 3d20 7365 6c66   metadata = self
-000086e0: 2e67 6574 5f6d 6574 6164 6174 615f 6466  .get_metadata_df
-000086f0: 2829 5b6c 6179 6572 5d0d 0a20 2020 2020  ()[layer]..     
-00008700: 2020 206d 645f 636f 7272 203d 2075 7361     md_corr = usa
-00008710: 6765 2e63 6f72 7277 6974 6828 6d65 7461  ge.corrwith(meta
-00008720: 6461 7461 2c20 6d65 7468 6f64 3d6d 6574  data, method=met
-00008730: 686f 6429 0d0a 2020 2020 2020 2020 7265  hod)..        re
-00008740: 7475 726e 206d 645f 636f 7272 0d0a 2020  turn md_corr..  
-00008750: 2020 2020 2020 0d0a 2020 2020 6465 6620        ..    def 
-00008760: 6170 7065 6e64 5f74 6f5f 6869 7374 6f72  append_to_histor
-00008770: 7928 7365 6c66 2c20 656e 7472 7929 3a0d  y(self, entry):.
-00008780: 0a20 2020 2020 2020 2022 2222 4164 6420  .        """Add 
-00008790: 656e 7472 7920 746f 2044 6174 6173 6574  entry to Dataset
-000087a0: 2068 6973 746f 7279 2e0d 0a0d 0a20 2020   history.....   
-000087b0: 2020 2020 203a 7061 7261 6d20 656e 7472       :param entr
-000087c0: 793a 2044 6573 6372 6970 7469 6f6e 206f  y: Description o
-000087d0: 6620 6576 656e 7420 746f 2072 6563 6f72  f event to recor
-000087e0: 6420 696e 2074 6865 2068 6973 746f 7279  d in the history
-000087f0: 2e0d 0a20 2020 2020 2020 203a 7479 7065  ...        :type
-00008800: 2065 6e74 7279 3a20 7374 720d 0a20 2020   entry: str..   
-00008810: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00008820: 2020 7365 6c66 2e61 6461 7461 2e75 6e73    self.adata.uns
-00008830: 5b22 6869 7374 6f72 7922 5d5b 6461 7465  ["history"][date
-00008840: 7469 6d65 2e75 7463 6e6f 7728 292e 6973  time.utcnow().is
-00008850: 6f66 6f72 6d61 7428 295d 203d 2065 6e74  oformat()] = ent
-00008860: 7279 0d0a 2020 2020 2020 2020 0d0a 2020  ry..        ..  
-00008870: 2020 6465 6620 6765 745f 6869 7374 6f72    def get_histor
-00008880: 7928 7365 6c66 293a 0d0a 2020 2020 2020  y(self):..      
-00008890: 2020 2222 2252 6574 7572 6e73 2074 696d    """Returns tim
-000088a0: 6573 7461 6d70 6564 2068 6973 746f 7279  estamped history
-000088b0: 206f 6620 4461 7461 7365 7420 6f62 6a65   of Dataset obje
-000088c0: 6374 2e0d 0a0d 0a20 2020 2020 2020 203a  ct.....        :
-000088d0: 7265 7475 726e 3a20 6869 7374 6f72 790d  return: history.
-000088e0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-000088f0: 2064 6963 740d 0a20 2020 2020 2020 2022   dict..        "
-00008900: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00008910: 726e 2073 656c 662e 6164 6174 612e 756e  rn self.adata.un
-00008920: 735b 2268 6973 746f 7279 225d            s["history"]
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f10: 2020 7472 756e 6361 7465 5f6e 6567 6174    truncate_negat
+00007f20: 6976 653a 2062 6f6f 6c20 3d20 5472 7565  ive: bool = True
+00007f30: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00007f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007f50: 2020 2020 2020 2020 2020 2920 2d3e 2070            ) -> p
+00007f60: 642e 4461 7461 4672 616d 653a 0d0a 2020  d.DataFrame:..  
+00007f70: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+00007f80: 7465 2050 6561 7273 6f6e 2072 6573 6964  te Pearson resid
+00007f90: 7561 6c20 6f66 2063 6869 2d73 7175 6172  ual of chi-squar
+00007fa0: 6564 2074 6573 742c 2061 7373 6f63 6961  ed test, associa
+00007fb0: 7469 6e67 2047 4550 7320 666f 7220 6561  ting GEPs for ea
+00007fc0: 6368 2072 616e 6b20 286b 2920 746f 2063  ch rank (k) to c
+00007fd0: 6174 6567 6f72 6965 7320 6f66 2073 616d  ategories of sam
+00007fe0: 706c 6573 2f6f 6273 6572 7661 7469 6f6e  ples/observation
+00007ff0: 732e 2042 7920 6465 6661 756c 742c 2074  s. By default, t
+00008000: 7275 6e63 6174 6573 206e 6567 6174 6976  runcates negativ
+00008010: 6520 7661 6c75 6573 2e0d 0a0d 0a20 2020  e values.....   
+00008020: 2020 2020 203a 7061 7261 6d20 6c61 7965       :param laye
+00008030: 723a 206e 616d 6520 6f66 2063 6174 6567  r: name of categ
+00008040: 6f72 6963 616c 2064 6174 6120 6c61 7965  orical data laye
+00008050: 720d 0a20 2020 2020 2020 203a 7479 7065  r..        :type
+00008060: 206c 6179 6572 3a20 7374 720d 0a20 2020   layer: str..   
+00008070: 2020 2020 203a 7061 7261 6d20 7472 756e       :param trun
+00008080: 6361 7465 5f6e 6567 6174 6976 653a 2054  cate_negative: T
+00008090: 7275 6e63 6174 6520 6e65 6761 7469 7665  runcate negative
+000080a0: 2072 6573 6964 7561 6c73 2074 6f20 302c   residuals to 0,
+000080b0: 2064 6566 6175 6c74 7320 746f 2054 7275   defaults to Tru
+000080c0: 650d 0a20 2020 2020 2020 203a 7479 7065  e..        :type
+000080d0: 2074 7275 6e63 6174 655f 6e65 6761 7469   truncate_negati
+000080e0: 7665 3a20 626f 6f6c 2c20 6f70 7469 6f6e  ve: bool, option
+000080f0: 616c 0d0a 2020 2020 2020 2020 3a72 6574  al..        :ret
+00008100: 7572 6e3a 2063 6174 6567 6f72 7920 c397  urn: category ..
+00008110: 2047 4550 206d 6174 7269 7820 6f66 206f   GEP matrix of o
+00008120: 7665 7272 6570 7265 7365 6e74 6174 696f  verrepresentatio
+00008130: 6e20 7661 6c75 6573 0d0a 2020 2020 2020  n values..      
+00008140: 2020 3a72 7479 7065 3a20 7064 2e44 6174    :rtype: pd.Dat
+00008150: 6146 7261 6d65 0d0a 2020 2020 2020 2020  aFrame..        
+00008160: 2222 220d 0a20 2020 2020 2020 2075 7361  """..        usa
+00008170: 6765 203d 2073 656c 662e 6765 745f 7573  ge = self.get_us
+00008180: 6167 6573 2829 2e63 6f70 7928 290d 0a20  ages().copy().. 
+00008190: 2020 2020 2020 2073 616d 706c 655f 746f         sample_to
+000081a0: 5f63 6c61 7373 203d 2073 656c 662e 6765  _class = self.ge
+000081b0: 745f 6d65 7461 6461 7461 5f64 6628 295b  t_metadata_df()[
+000081c0: 6c61 7965 725d 0d0a 2020 2020 2020 2020  layer]..        
+000081d0: 7573 6167 652e 696e 6465 7820 3d20 7573  usage.index = us
+000081e0: 6167 652e 696e 6465 782e 6d61 7028 7361  age.index.map(sa
+000081f0: 6d70 6c65 5f74 6f5f 636c 6173 7329 0d0a  mple_to_class)..
+00008200: 2020 2020 2020 2020 6f62 7365 7276 6564          observed
+00008210: 203d 2075 7361 6765 2e67 726f 7570 6279   = usage.groupby
+00008220: 2861 7869 733d 302c 206c 6576 656c 3d30  (axis=0, level=0
+00008230: 292e 7375 6d28 290d 0a20 2020 2020 2020  ).sum()..       
+00008240: 2065 7870 6563 7465 6420 3d20 5b5d 0d0a   expected = []..
+00008250: 2020 2020 2020 2020 666f 7220 6b2c 206f          for k, o
+00008260: 6273 5f6b 2069 6e20 6f62 7365 7276 6564  bs_k in observed
+00008270: 2e67 726f 7570 6279 2861 7869 733d 312c  .groupby(axis=1,
+00008280: 206c 6576 656c 3d31 293a 0d0a 2020 2020   level=1):..    
+00008290: 2020 2020 2020 2020 6578 705f 6b20 3d20          exp_k = 
+000082a0: 7064 2e44 6174 6146 7261 6d65 286f 6273  pd.DataFrame(obs
+000082b0: 5f6b 2e73 756d 2861 7869 733d 3129 2920  _k.sum(axis=1)) 
+000082c0: 4020 7064 2e44 6174 6146 7261 6d65 286f  @ pd.DataFrame(o
+000082d0: 6273 5f6b 2e73 756d 2861 7869 733d 3029  bs_k.sum(axis=0)
+000082e0: 292e 5420 2f20 6f62 735f 6b2e 7375 6d28  ).T / obs_k.sum(
+000082f0: 292e 7375 6d28 290d 0a20 2020 2020 2020  ).sum()..       
+00008300: 2020 2020 2065 7870 6563 7465 642e 6170       expected.ap
+00008310: 7065 6e64 2865 7870 5f6b 290d 0a20 2020  pend(exp_k)..   
+00008320: 2020 2020 2065 7870 6563 7465 6420 3d20       expected = 
+00008330: 7064 2e63 6f6e 6361 7428 6578 7065 6374  pd.concat(expect
+00008340: 6564 2c20 6178 6973 3d31 290d 0a20 2020  ed, axis=1)..   
+00008350: 2020 2020 2063 6869 7371 5f72 6573 6964       chisq_resid
+00008360: 203d 2028 6f62 7365 7276 6564 202d 2065   = (observed - e
+00008370: 7870 6563 7465 6429 202f 206e 702e 7371  xpected) / np.sq
+00008380: 7274 2865 7870 6563 7465 6429 2020 2320  rt(expected)  # 
+00008390: 7065 6172 736f 6e20 7265 7369 6475 616c  pearson residual
+000083a0: 206f 6620 6368 692d 7371 7561 7265 6420   of chi-squared 
+000083b0: 7465 7374 206f 6620 636f 6e74 696e 6765  test of continge
+000083c0: 6e63 7920 7461 626c 650d 0a20 2020 2020  ncy table..     
+000083d0: 2020 2069 6620 7472 756e 6361 7465 5f6e     if truncate_n
+000083e0: 6567 6174 6976 653a 0d0a 2020 2020 2020  egative:..      
+000083f0: 2020 2020 2020 6368 6973 715f 7265 7369        chisq_resi
+00008400: 6420 3d20 6368 6973 715f 7265 7369 642e  d = chisq_resid.
+00008410: 636c 6970 286c 6f77 6572 3d30 290d 0a20  clip(lower=0).. 
+00008420: 2020 2020 2020 2072 6574 7572 6e20 6368         return ch
+00008430: 6973 715f 7265 7369 640d 0a20 2020 200d  isq_resid..    .
+00008440: 0a20 2020 2020 2020 200d 0a20 2020 2064  .        ..    d
+00008450: 6566 2067 6574 5f6d 6574 6164 6174 615f  ef get_metadata_
+00008460: 636f 7272 656c 6174 696f 6e28 7365 6c66  correlation(self
+00008470: 2c20 0d0a 2020 2020 2020 2020 2020 2020  , ..            
+00008480: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008490: 2020 2020 206c 6179 6572 3a20 7374 722c       layer: str,
+000084a0: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
+000084b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084c0: 2020 206d 6574 686f 643a 2073 7472 203d     method: str =
+000084d0: 2022 7065 6172 736f 6e22 0d0a 2020 2020   "pearson"..    
+000084e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000084f0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+00008500: 3e20 7064 2e53 6572 6965 733a 0d0a 2020  > pd.Series:..  
+00008510: 2020 2020 2020 2222 2243 616c 6375 6c61        """Calcula
+00008520: 7465 2050 6561 7273 6f6e 2063 6f72 7265  te Pearson corre
+00008530: 6c61 7469 6f6e 206f 6620 4745 5020 7573  lation of GEP us
+00008540: 6167 6520 746f 206e 756d 6572 6963 616c  age to numerical
+00008550: 206d 6574 6164 6174 6120 6163 726f 7373   metadata across
+00008560: 2073 616d 706c 6573 2f6f 6273 6572 7661   samples/observa
+00008570: 7469 6f6e 732e 0d0a 0d0a 2020 2020 2020  tions.....      
+00008580: 2020 3a70 6172 616d 206c 6179 6572 3a20    :param layer: 
+00008590: 6e61 6d65 206f 6620 6e75 6d65 7269 6361  name of numerica
+000085a0: 6c20 6461 7461 206c 6179 6572 0d0a 2020  l data layer..  
+000085b0: 2020 2020 2020 3a74 7970 6520 6c61 7965        :type laye
+000085c0: 723a 2073 7472 0d0a 2020 2020 2020 2020  r: str..        
+000085d0: 3a70 6172 616d 206d 6574 686f 643a 2043  :param method: C
+000085e0: 6f72 7265 6c61 7469 6f6e 206d 6574 686f  orrelation metho
+000085f0: 643a 2022 7065 6172 736f 6e22 2c20 2273  d: "pearson", "s
+00008600: 7065 6172 6d61 6e22 2c20 6f72 2022 6b65  pearman", or "ke
+00008610: 6e64 616c 6c22 2e20 4465 6661 756c 7473  ndall". Defaults
+00008620: 2074 6f20 2270 6561 7273 6f6e 220d 0a20   to "pearson".. 
+00008630: 2020 2020 2020 203a 7479 7065 206d 6574         :type met
+00008640: 686f 643a 2073 7472 2c20 6f70 7469 6f6e  hod: str, option
+00008650: 616c 0d0a 2020 2020 2020 2020 3a72 6574  al..        :ret
+00008660: 7572 6e3a 2063 6f72 7265 6c61 7469 6f6e  urn: correlation
+00008670: 206f 6620 4745 5020 746f 206d 6574 6164   of GEP to metad
+00008680: 6174 610d 0a20 2020 2020 2020 203a 7274  ata..        :rt
+00008690: 7970 653a 2070 642e 5365 7269 6573 0d0a  ype: pd.Series..
+000086a0: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+000086b0: 2020 2020 2075 7361 6765 203d 2073 656c       usage = sel
+000086c0: 662e 6765 745f 7573 6167 6573 2829 2e63  f.get_usages().c
+000086d0: 6f70 7928 290d 0a20 2020 2020 2020 206d  opy()..        m
+000086e0: 6574 6164 6174 6120 3d20 7365 6c66 2e67  etadata = self.g
+000086f0: 6574 5f6d 6574 6164 6174 615f 6466 2829  et_metadata_df()
+00008700: 5b6c 6179 6572 5d0d 0a20 2020 2020 2020  [layer]..       
+00008710: 206d 645f 636f 7272 203d 2075 7361 6765   md_corr = usage
+00008720: 2e63 6f72 7277 6974 6828 6d65 7461 6461  .corrwith(metada
+00008730: 7461 2c20 6d65 7468 6f64 3d6d 6574 686f  ta, method=metho
+00008740: 6429 0d0a 2020 2020 2020 2020 7265 7475  d)..        retu
+00008750: 726e 206d 645f 636f 7272 0d0a 2020 2020  rn md_corr..    
+00008760: 2020 2020 0d0a 2020 2020 6465 6620 6170      ..    def ap
+00008770: 7065 6e64 5f74 6f5f 6869 7374 6f72 7928  pend_to_history(
+00008780: 7365 6c66 2c20 656e 7472 7929 3a0d 0a20  self, entry):.. 
+00008790: 2020 2020 2020 2022 2222 4164 6420 656e         """Add en
+000087a0: 7472 7920 746f 2044 6174 6173 6574 2068  try to Dataset h
+000087b0: 6973 746f 7279 2e0d 0a0d 0a20 2020 2020  istory.....     
+000087c0: 2020 203a 7061 7261 6d20 656e 7472 793a     :param entry:
+000087d0: 2044 6573 6372 6970 7469 6f6e 206f 6620   Description of 
+000087e0: 6576 656e 7420 746f 2072 6563 6f72 6420  event to record 
+000087f0: 696e 2074 6865 2068 6973 746f 7279 2e0d  in the history..
+00008800: 0a20 2020 2020 2020 203a 7479 7065 2065  .        :type e
+00008810: 6e74 7279 3a20 7374 720d 0a20 2020 2020  ntry: str..     
+00008820: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00008830: 7365 6c66 2e61 6461 7461 2e75 6e73 5b22  self.adata.uns["
+00008840: 6869 7374 6f72 7922 5d5b 6461 7465 7469  history"][dateti
+00008850: 6d65 2e75 7463 6e6f 7728 292e 6973 6f66  me.utcnow().isof
+00008860: 6f72 6d61 7428 295d 203d 2065 6e74 7279  ormat()] = entry
+00008870: 0d0a 2020 2020 2020 2020 0d0a 2020 2020  ..        ..    
+00008880: 6465 6620 6765 745f 6869 7374 6f72 7928  def get_history(
+00008890: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+000088a0: 2222 2252 6574 7572 6e73 2074 696d 6573  """Returns times
+000088b0: 7461 6d70 6564 2068 6973 746f 7279 206f  tamped history o
+000088c0: 6620 4461 7461 7365 7420 6f62 6a65 6374  f Dataset object
+000088d0: 2e0d 0a0d 0a20 2020 2020 2020 203a 7265  .....        :re
+000088e0: 7475 726e 3a20 6869 7374 6f72 790d 0a20  turn: history.. 
+000088f0: 2020 2020 2020 203a 7274 7970 653a 2064         :rtype: d
+00008900: 6963 740d 0a20 2020 2020 2020 2022 2222  ict..        """
+00008910: 0d0a 2020 2020 2020 2020 7265 7475 726e  ..        return
+00008920: 2073 656c 662e 6164 6174 612e 756e 735b   self.adata.uns[
+00008930: 2268 6973 746f 7279 225d                 "history"]
```

### Comparing `cnmfsns-1.3.0/src/cnmfsns/integration.py` & `cnmfsns-1.3.1/src/cnmfsns/integration.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.0/src/cnmfsns/plots.py` & `cnmfsns-1.3.1/src/cnmfsns/plots.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.0/src/cnmfsns/sns.py` & `cnmfsns-1.3.1/src/cnmfsns/sns.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.0/src/cnmfsns/utils.py` & `cnmfsns-1.3.1/src/cnmfsns/utils.py`

 * *Files identical despite different names*

### Comparing `cnmfsns-1.3.0/src/cnmfsns.egg-info/PKG-INFO` & `cnmfsns-1.3.1/src/cnmfsns.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnmfsns
-Version: 1.3.0
+Version: 1.3.1
 Summary: cNMF Solution Network Space
 Home-page: https://github.com/MorrissyLab/cNMF-SNS
 Author: Ted Verhey
 Author-email: tbverhey@ucalgary.ca
 Project-URL: Bug Tracker, https://github.com/MorrissyLab/cNMF-SNS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -16,17 +16,17 @@
 
 ![cNMF-SNS logo](logo.png)
 
 -----------------
 
 # cNMF-SNS: powerful factorization-based multi-omics integration toolkit
 
-![version badge](https://img.shields.io/badge/version-1.3.0-blue)
+![version badge](https://img.shields.io/badge/version-1.3.1-blue)
 [![PyPI Latest Release](https://img.shields.io/pypi/v/cnmfsns.svg)](https://pypi.org/project/cnmfsns/)
-[![Conda Latest Release](https://anaconda.org/conda-forge/cnmfsns/badges/version.svg)](https://anaconda.org/anaconda/cnmfsns/)
+[![Conda Latest Release](https://img.shields.io/conda/vn/conda-forge/cnmfsns)](https://anaconda.org/conda-forge/cnmfsns/)
 [![Documentation status](https://readthedocs.org/projects/cnmf-sns/badge/?version=latest&style=flat)]()
 [![Downloads](https://static.pepy.tech/badge/cnmfsns)](https://pepy.tech/project/cnmfsns)
 [![License](https://img.shields.io/pypi/l/cnmfsns.svg)](https://github.com/MorrissyLab/cNMF-SNS/blob/main/LICENSE)
 
 Authors: [Ted Verhey](https://github.com/verheytb), [Heewon Seo](https://github.com/lootpiz), [Sorana Morrissy](https://github.com/ancasorana)
 
 **cNMF-SNS** (consensus Non-negative Matrix Factorization Solution Network Space) is a Python package enabling mosaic integration of bulk, single-cell, and
```


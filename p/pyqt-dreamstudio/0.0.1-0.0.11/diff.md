# Comparing `tmp/pyqt-dreamstudio-0.0.1.tar.gz` & `tmp/pyqt-dreamstudio-0.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqt-dreamstudio-0.0.1.tar", last modified: Mon May 29 04:59:57 2023, max compression
+gzip compressed data, was "pyqt-dreamstudio-0.0.11.tar", last modified: Mon May 29 05:19:20 2023, max compression
```

## Comparing `pyqt-dreamstudio-0.0.1.tar` & `pyqt-dreamstudio-0.0.11.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 04:59:57.261376 pyqt-dreamstudio-0.0.1/
--rw-rw-rw-   0        0        0     1086 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     2206 2023-05-29 04:59:57.260379 pyqt-dreamstudio-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1838 2023-05-29 04:53:48.000000 pyqt-dreamstudio-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 04:59:57.237436 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/
--rw-rw-rw-   0        0        0        0 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/__init__.py
--rw-rw-rw-   0        0        0     1558 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/currentImageView.py
--rw-rw-rw-   0        0        0     1706 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/explorerWidget.py
-drwxrwxrwx   0        0        0        0 2023-05-29 04:59:57.258381 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/ico/
--rw-rw-rw-   0        0        0        0 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/ico/__init__.py
--rw-rw-rw-   0        0        0     5066 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/imageListWidget.py
--rw-rw-rw-   0        0        0    18245 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/imageSqlite.py
--rw-rw-rw-   0        0        0    10980 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/imageStableDiffusionPage.py
--rw-rw-rw-   0        0        0     1444 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/inputDialog.py
--rw-rw-rw-   0        0        0     3814 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/leftSideBar.py
--rw-rw-rw-   0        0        0   232520 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/logo.png
--rw-rw-rw-   0        0        0     4908 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/main.py
--rw-rw-rw-   0        0        0     3270 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/notifier.py
--rw-rw-rw-   0        0        0      682 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/rightSideBar.py
--rw-rw-rw-   0        0        0     2854 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/searchBar.py
--rw-rw-rw-   0        0        0     5918 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/svgButton.py
--rw-rw-rw-   0        0        0      765 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/svgLabel.py
--rw-rw-rw-   0        0        0     4060 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/thumbnailView.py
--rw-rw-rw-   0        0        0     4884 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/toast.py
--rw-rw-rw-   0        0        0     1865 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/viewWidget.py
-drwxrwxrwx   0        0        0        0 2023-05-29 04:59:57.257384 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio.egg-info/
--rw-rw-rw-   0        0        0     2206 2023-05-29 04:59:56.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      829 2023-05-29 04:59:57.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 04:59:56.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-05-29 04:59:56.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-05-29 04:59:56.000000 pyqt-dreamstudio-0.0.1/pyqt_dreamstudio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 04:59:57.261376 pyqt-dreamstudio-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      861 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 05:19:20.351457 pyqt-dreamstudio-0.0.11/
+-rw-rw-rw-   0        0        0     1086 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/LICENSE
+-rw-rw-rw-   0        0        0     2544 2023-05-29 05:19:20.350460 pyqt-dreamstudio-0.0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     2162 2023-05-29 05:18:57.000000 pyqt-dreamstudio-0.0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 05:19:20.319542 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/
+-rw-rw-rw-   0        0        0        0 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/__init__.py
+-rw-rw-rw-   0        0        0     1558 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/currentImageView.py
+-rw-rw-rw-   0        0        0     1723 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/explorerWidget.py
+drwxrwxrwx   0        0        0        0 2023-05-29 05:19:20.348465 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/ico/
+-rw-rw-rw-   0        0        0        0 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/ico/__init__.py
+-rw-rw-rw-   0        0        0      712 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/ico/history.svg
+-rw-rw-rw-   0        0        0     1283 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/ico/setting.svg
+-rw-rw-rw-   0        0        0     5100 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageListWidget.py
+-rw-rw-rw-   0        0        0    18245 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageSqlite.py
+-rw-rw-rw-   0        0        0    11031 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageStableDiffusionPage.py
+-rw-rw-rw-   0        0        0     1444 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/inputDialog.py
+-rw-rw-rw-   0        0        0     3865 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/leftSideBar.py
+-rw-rw-rw-   0        0        0   232520 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/logo.png
+-rw-rw-rw-   0        0        0     4976 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/main.py
+-rw-rw-rw-   0        0        0     3270 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/notifier.py
+-rw-rw-rw-   0        0        0      699 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/rightSideBar.py
+-rw-rw-rw-   0        0        0     2854 2023-05-29 04:51:09.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/searchBar.py
+-rw-rw-rw-   0        0        0     5918 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/svgButton.py
+-rw-rw-rw-   0        0        0      765 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/svgLabel.py
+-rw-rw-rw-   0        0        0     4077 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/thumbnailView.py
+-rw-rw-rw-   0        0        0     4884 2023-05-29 04:49:18.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/toast.py
+-rw-rw-rw-   0        0        0     1899 2023-05-29 05:12:01.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/viewWidget.py
+drwxrwxrwx   0        0        0        0 2023-05-29 05:19:20.342482 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/
+-rw-rw-rw-   0        0        0     2544 2023-05-29 05:19:20.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      895 2023-05-29 05:19:20.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 05:19:20.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-29 05:19:20.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-05-29 05:19:20.000000 pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 05:19:20.351457 pyqt-dreamstudio-0.0.11/setup.cfg
+-rw-rw-rw-   0        0        0      879 2023-05-29 05:15:51.000000 pyqt-dreamstudio-0.0.11/setup.py
```

### Comparing `pyqt-dreamstudio-0.0.1/LICENSE` & `pyqt-dreamstudio-0.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.1/PKG-INFO` & `pyqt-dreamstudio-0.0.11/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,159 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2070 7971  : 2.1..Name: pyq
 00000020: 742d 6472 6561 6d73 7475 6469 6f0d 0a56  t-dreamstudio..V
-00000030: 6572 7369 6f6e 3a20 302e 302e 310d 0a53  ersion: 0.0.1..S
-00000040: 756d 6d61 7279 3a20 5573 696e 6720 4472  ummary: Using Dr
-00000050: 6561 6d53 7475 6469 6f20 4150 4920 696e  eamStudio API in
-00000060: 2050 7974 686f 6e20 6465 736b 746f 7020   Python desktop 
-00000070: 6170 706c 6963 6174 696f 6e0d 0a48 6f6d  application..Hom
-00000080: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
-00000090: 6769 7468 7562 2e63 6f6d 2f79 6a67 3330  github.com/yjg30
-000000a0: 3733 372f 7079 7174 2d64 7265 616d 7374  737/pyqt-dreamst
-000000b0: 7564 696f 2e67 6974 0d0a 4175 7468 6f72  udio.git..Author
-000000c0: 3a20 4a75 6e67 2047 7975 2059 6f6f 6e0d  : Jung Gyu Yoon.
-000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 2079  .Author-email: y
-000000e0: 6a67 3330 3733 3740 676d 6169 6c2e 636f  jg30737@gmail.co
-000000f0: 6d0d 0a4c 6963 656e 7365 3a20 4d49 540d  m..License: MIT.
-00000100: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00000110: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000120: 6d61 726b 646f 776e 0d0a 4c69 6365 6e73  markdown..Licens
-00000130: 652d 4669 6c65 3a20 4c49 4345 4e53 450d  e-File: LICENSE.
-00000140: 0a0d 0a0d 0a23 2070 7971 742d 6472 6561  .....# pyqt-drea
-00000150: 6d73 7475 6469 6f0d 0d0a 5573 696e 6720  mstudio...Using 
-00000160: 4472 6561 6d53 7475 6469 6f20 4150 4920  DreamStudio API 
-00000170: 696e 2050 7974 686f 6e20 6465 736b 746f  in Python deskto
-00000180: 7020 6170 706c 6963 6174 696f 6e0d 0d0a  p application...
-00000190: 0d0d 0a59 6f75 2063 616e 206d 616b 6520  ...You can make 
-000001a0: 6120 6275 6e63 6820 6f66 2069 6d61 6765  a bunch of image
-000001b0: 2077 6974 686f 7574 2069 6e73 7461 6c6c   without install
-000001c0: 696e 6720 6865 6176 7920 7265 736f 7572  ing heavy resour
-000001d0: 6365 7320 6c69 6b65 2043 5544 412c 2074  ces like CUDA, t
-000001e0: 6f72 6368 2c20 6574 632e 2042 7574 2069  orch, etc. But i
-000001f0: 7427 7320 6e6f 7420 6672 6565 2e0d 0d0a  t's not free....
-00000200: 0d0d 0a54 6869 7320 6973 2073 6570 6172  ...This is separ
-00000210: 6174 6564 2066 726f 6d20 3c61 2068 7265  ated from <a hre
-00000220: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000230: 622e 636f 6d2f 796a 6733 3037 3337 2f70  b.com/yjg30737/p
-00000240: 7971 742d 6f70 656e 6169 223e 7079 7174  yqt-openai">pyqt
-00000250: 2d6f 7065 6e61 693c 2f61 3e20 7061 636b  -openai</a> pack
-00000260: 6167 6520 746f 2070 656f 706c 6520 7768  age to people wh
-00000270: 6f20 6f6e 6c79 2077 616e 7473 2074 6f20  o only wants to 
-00000280: 7573 6520 7374 6162 6c65 2064 6966 6675  use stable diffu
-00000290: 7369 6f6e 2061 7069 0d0d 0a0d 0d0a 616e  sion api......an
-000002a0: 6420 7768 6f20 7761 6e74 7320 746f 2066  d who wants to f
-000002b0: 6f72 6b20 7468 6973 2074 6f20 6d61 6b65  ork this to make
-000002c0: 2074 6865 6972 2061 7070 2e0d 0d0a 0d0d   their app......
-000002d0: 0a23 2320 5072 6572 6571 7569 7369 7465  .## Prerequisite
-000002e0: 200d 0d0a 596f 7520 6861 7665 2074 6f20   ...You have to 
-000002f0: 6765 7420 7468 6520 4472 6561 6d53 7475  get the DreamStu
-00000300: 6469 6f20 6170 6920 6b65 7920 6672 6f6d  dio api key from
-00000310: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000320: 2f2f 706c 6174 666f 726d 2e73 7461 6269  //platform.stabi
-00000330: 6c69 7479 2e61 692f 646f 6373 2f67 6574  lity.ai/docs/get
-00000340: 7469 6e67 2d73 7461 7274 6564 2f61 7574  ting-started/aut
-00000350: 6865 6e74 6963 6174 696f 6e22 3e68 6572  hentication">her
-00000360: 653c 2f61 3e2e 0d0d 0a0d 0d0a 5573 696e  e</a>.......Usin
-00000370: 6720 4472 6561 6d53 7475 6469 6f20 6f72  g DreamStudio or
-00000380: 2074 6865 2041 5049 2072 6571 7569 7265   the API require
-00000390: 7320 6372 6564 6974 732e 2054 616b 6520  s credits. Take 
-000003a0: 6120 6c6f 6f6b 2061 7420 3c61 2068 7265  a look at <a hre
-000003b0: 663d 2268 7474 7073 3a2f 2f70 6c61 7466  f="https://platf
-000003c0: 6f72 6d2e 7374 6162 696c 6974 792e 6169  orm.stability.ai
-000003d0: 2f64 6f63 732f 6765 7474 696e 672d 7374  /docs/getting-st
-000003e0: 6172 7465 642f 6372 6564 6974 732d 616e  arted/credits-an
-000003f0: 642d 6269 6c6c 696e 6723 7364 786c 2d70  d-billing#sdxl-p
-00000400: 7269 6369 6e67 2d74 6162 6c65 223e 7072  ricing-table">pr
-00000410: 6963 696e 673c 2f61 3e20 6162 6f75 7420  icing</a> about 
-00000420: 7468 6973 2e0d 0d0a 0d0d 0a4d 616b 6520  this.......Make 
-00000430: 796f 7572 2069 6d61 6765 2069 6e20 3c61  your image in <a
-00000440: 2068 7265 663d 2268 7474 7073 3a2f 2f62   href="https://b
-00000450: 6574 612e 6472 6561 6d73 7475 6469 6f2e  eta.dreamstudio.
-00000460: 6169 2f67 656e 6572 6174 6522 3e68 6572  ai/generate">her
-00000470: 653c 2f61 3e20 6265 666f 7265 2064 6f69  e</a> before doi
-00000480: 6e67 2077 6974 6820 7468 6973 2061 7070  ng with this app
-00000490: 2e0d 0d0a 0d0d 0a23 2320 486f 7720 746f  .......## How to
-000004a0: 2049 6e73 7461 6c6c 0d0d 0a23 2323 2042   Install...### B
-000004b0: 7920 436c 6f6e 696e 6967 0d0d 0a31 2e20  y Cloninig...1. 
-000004c0: 6769 7420 636c 6f6e 6520 7e0d 0d0a 322e  git clone ~...2.
-000004d0: 2070 6970 2069 6e73 7461 6c6c 202d 7220   pip install -r 
-000004e0: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
-000004f0: 0d0d 0a33 2e20 7079 7468 6f6e 206d 6169  ...3. python mai
-00000500: 6e2e 7079 0d0d 0a23 2323 2042 7920 5069  n.py...### By Pi
-00000510: 700d 0d0a 7069 7020 696e 7374 616c 6c20  p...pip install 
-00000520: 7079 7174 5f64 7265 616d 7374 7564 696f  pyqt_dreamstudio
-00000530: 0d0d 0a0d 0d0a 2323 2048 6f77 2074 6f20  ......## How to 
-00000540: 5573 650d 0d0a 5468 6572 6520 6973 2074  Use...There is t
-00000550: 6865 206f 7074 696f 6e73 2074 6162 2061  he options tab a
-00000560: 7420 7468 6520 7269 6768 7420 7369 6465  t the right side
-00000570: 206f 6620 7468 6520 7769 6e64 6f77 2e20   of the window. 
-00000580: 0d0d 0a0d 0d0a 496e 7075 7420 796f 7572  ......Input your
-00000590: 2041 5049 206b 6579 2c20 6368 6f6f 7365   API key, choose
-000005a0: 2070 6172 616d 6574 6572 7320 796f 7520   parameters you 
-000005b0: 7761 6e74 2074 6f20 7365 742c 2077 7269  want to set, wri
-000005c0: 7465 2070 726f 706d 742c 2073 7562 6d69  te propmt, submi
-000005d0: 7420 6974 2c20 616e 6420 796f 7520 6361  t it, and you ca
-000005e0: 6e20 7365 6520 7468 6520 7265 7375 6c74  n see the result
-000005f0: 2061 7420 7468 6520 6c65 6674 2073 6964   at the left sid
-00000600: 6520 2877 6869 6368 206c 6f6f 6b73 206c  e (which looks l
-00000610: 696b 6520 6669 6c65 2065 7870 6c6f 7265  ike file explore
-00000620: 7229 2073 6f6f 6e20 656e 6f75 6768 2e0d  r) soon enough..
-00000630: 0d0a 0d0d 0a53 6565 2074 6865 203c 6120  .....See the <a 
-00000640: 6872 6566 3d22 6874 7470 733a 2f2f 706c  href="https://pl
-00000650: 6174 666f 726d 2e73 7461 6269 6c69 7479  atform.stability
-00000660: 2e61 692f 646f 6373 2f66 6561 7475 7265  .ai/docs/feature
-00000670: 732f 6170 692d 7061 7261 6d65 7465 7273  s/api-parameters
-00000680: 223e 7768 6f6c 6520 6578 706c 616e 6174  ">whole explanat
-00000690: 696f 6e3c 2f61 3e20 6162 6f75 7420 6576  ion</a> about ev
-000006a0: 6572 7920 6f70 7469 6f6e 7320 746f 206d  ery options to m
-000006b0: 616b 6520 6265 7474 6572 2069 6d61 6765  ake better image
-000006c0: 2e0d 0d0a 0d0d 0a41 6674 6572 2069 6d61  .......After ima
-000006d0: 6765 7320 676f 7420 6765 6e65 7261 7465  ges got generate
-000006e0: 642c 2079 6f75 2063 616e 2063 6f70 7920  d, you can copy 
-000006f0: 6f72 2064 6f77 6e6c 6f61 6420 616e 7920  or download any 
-00000700: 696d 6167 6573 2077 6865 6e20 796f 7520  images when you 
-00000710: 7075 7420 7468 6520 6d6f 7573 6520 6375  put the mouse cu
-00000720: 7273 6f72 206f 7665 7220 7468 656d 2e20  rsor over them. 
-00000730: 200d 0d0a 0d0d 0a23 2320 5265 7375 6c74   ......## Result
-00000740: 0d0d 0a21 5b69 6d61 6765 5d28 6874 7470  ...![image](http
-00000750: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
-00000760: 6a67 3330 3733 372f 7079 7174 2d64 7265  jg30737/pyqt-dre
-00000770: 616d 7374 7564 696f 2f61 7373 6574 732f  amstudio/assets/
-00000780: 3535 3037 3830 3433 2f38 3031 3031 6661  55078043/80101fa
-00000790: 662d 6662 3065 2d34 3365 322d 6163 6239  f-fb0e-43e2-acb9
-000007a0: 2d32 6366 3531 6139 6666 3362 3129 0d0d  -2cf51a9ff3b1)..
-000007b0: 0a0d 0d0a 2323 204e 6f74 650d 0d0a 4173  ....## Note...As
-000007c0: 2066 6172 2061 7320 6920 6b6e 6f77 2c20   far as i know, 
-000007d0: 5573 696e 6720 5374 6162 6c65 2044 6966  Using Stable Dif
-000007e0: 6675 7369 6f6e 2077 6974 6820 4150 4920  fusion with API 
-000007f0: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-00000800: 6469 7361 626c 6520 7361 6665 7479 2066  disable safety f
-00000810: 696c 7465 722e 2053 6861 6d65 2121 0d0d  ilter. Shame!!..
-00000820: 0a0d 0d0a 536f 2069 6620 796f 7520 7479  ....So if you ty
-00000830: 7065 2061 6e79 2077 6f72 6473 2077 6869  pe any words whi
-00000840: 6368 2069 7320 636f 6e73 6964 6572 6564  ch is considered
-00000850: 2061 7320 4e53 4657 2c20 746f 6173 7420   as NSFW, toast 
-00000860: 636f 6e74 6169 6e69 6e67 2065 7272 6f72  containing error
-00000870: 206d 6573 7361 6765 2077 696c 6c20 7368   message will sh
-00000880: 6f77 2075 700d 0d0a 0d0d 0a23 2320 4c69  ow up......## Li
-00000890: 6365 6e73 650d 0d0a 4d49 540d 0d0a       cense...MIT...
+00000030: 6572 7369 6f6e 3a20 302e 302e 3131 0d0a  ersion: 0.0.11..
+00000040: 5375 6d6d 6172 793a 2055 7369 6e67 2044  Summary: Using D
+00000050: 7265 616d 5374 7564 696f 2041 5049 2069  reamStudio API i
+00000060: 6e20 5079 7468 6f6e 2064 6573 6b74 6f70  n Python desktop
+00000070: 2061 7070 6c69 6361 7469 6f6e 0d0a 486f   application..Ho
+00000080: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+00000090: 2f67 6974 6875 622e 636f 6d2f 796a 6733  /github.com/yjg3
+000000a0: 3037 3337 2f70 7971 742d 6472 6561 6d73  0737/pyqt-dreams
+000000b0: 7475 6469 6f2e 6769 740d 0a41 7574 686f  tudio.git..Autho
+000000c0: 723a 204a 756e 6720 4779 7520 596f 6f6e  r: Jung Gyu Yoon
+000000d0: 0d0a 4175 7468 6f72 2d65 6d61 696c 3a20  ..Author-email: 
+000000e0: 796a 6733 3037 3337 4067 6d61 696c 2e63  yjg30737@gmail.c
+000000f0: 6f6d 0d0a 4c69 6365 6e73 653a 204d 4954  om..License: MIT
+00000100: 0d0a 4465 7363 7269 7074 696f 6e2d 436f  ..Description-Co
+00000110: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+00000120: 2f6d 6172 6b64 6f77 6e0d 0a4c 6963 656e  /markdown..Licen
+00000130: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+00000140: 0d0a 0d0a 0d0a 2320 7079 7174 2d64 7265  ......# pyqt-dre
+00000150: 616d 7374 7564 696f 0d0d 0a55 7369 6e67  amstudio...Using
+00000160: 2044 7265 616d 5374 7564 696f 2041 5049   DreamStudio API
+00000170: 2069 6e20 5079 7468 6f6e 2064 6573 6b74   in Python deskt
+00000180: 6f70 2061 7070 6c69 6361 7469 6f6e 0d0d  op application..
+00000190: 0a0d 0d0a 596f 7520 6361 6e20 6d61 6b65  ....You can make
+000001a0: 2061 2062 756e 6368 206f 6620 696d 6167   a bunch of imag
+000001b0: 6520 7769 7468 6f75 7420 696e 7374 616c  e without instal
+000001c0: 6c69 6e67 2068 6561 7679 2072 6573 6f75  ling heavy resou
+000001d0: 7263 6573 206c 696b 6520 4355 4441 2c20  rces like CUDA, 
+000001e0: 746f 7263 682c 2065 7463 2e20 4275 7420  torch, etc. But 
+000001f0: 6974 2773 206e 6f74 2066 7265 652e 0d0d  it's not free...
+00000200: 0a0d 0d0a 5468 6973 2069 7320 7365 7061  ....This is sepa
+00000210: 7261 7465 6420 6672 6f6d 203c 6120 6872  rated from <a hr
+00000220: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000230: 7562 2e63 6f6d 2f79 6a67 3330 3733 372f  ub.com/yjg30737/
+00000240: 7079 7174 2d6f 7065 6e61 6922 3e70 7971  pyqt-openai">pyq
+00000250: 742d 6f70 656e 6169 3c2f 613e 2070 6163  t-openai</a> pac
+00000260: 6b61 6765 2074 6f20 7065 6f70 6c65 2077  kage to people w
+00000270: 686f 206f 6e6c 7920 7761 6e74 7320 746f  ho only wants to
+00000280: 2075 7365 2073 7461 626c 6520 6469 6666   use stable diff
+00000290: 7573 696f 6e20 6170 690d 0d0a 0d0d 0a61  usion api......a
+000002a0: 6e64 2077 686f 2077 616e 7473 2074 6f20  nd who wants to 
+000002b0: 666f 726b 2074 6869 7320 746f 206d 616b  fork this to mak
+000002c0: 6520 7468 6569 7220 6170 702e 0d0d 0a0d  e their app.....
+000002d0: 0d0a 2323 2050 7265 7265 7175 6973 6974  ..## Prerequisit
+000002e0: 6520 0d0d 0a59 6f75 2068 6176 6520 746f  e ...You have to
+000002f0: 2067 6574 2074 6865 2044 7265 616d 5374   get the DreamSt
+00000300: 7564 696f 2061 7069 206b 6579 2066 726f  udio api key fro
+00000310: 6d20 3c61 2068 7265 663d 2268 7474 7073  m <a href="https
+00000320: 3a2f 2f70 6c61 7466 6f72 6d2e 7374 6162  ://platform.stab
+00000330: 696c 6974 792e 6169 2f64 6f63 732f 6765  ility.ai/docs/ge
+00000340: 7474 696e 672d 7374 6172 7465 642f 6175  tting-started/au
+00000350: 7468 656e 7469 6361 7469 6f6e 223e 6865  thentication">he
+00000360: 7265 3c2f 613e 2e0d 0d0a 0d0d 0a55 7369  re</a>.......Usi
+00000370: 6e67 2044 7265 616d 5374 7564 696f 206f  ng DreamStudio o
+00000380: 7220 7468 6520 4150 4920 7265 7175 6972  r the API requir
+00000390: 6573 2063 7265 6469 7473 2e20 5461 6b65  es credits. Take
+000003a0: 2061 206c 6f6f 6b20 6174 203c 6120 6872   a look at <a hr
+000003b0: 6566 3d22 6874 7470 733a 2f2f 706c 6174  ef="https://plat
+000003c0: 666f 726d 2e73 7461 6269 6c69 7479 2e61  form.stability.a
+000003d0: 692f 646f 6373 2f67 6574 7469 6e67 2d73  i/docs/getting-s
+000003e0: 7461 7274 6564 2f63 7265 6469 7473 2d61  tarted/credits-a
+000003f0: 6e64 2d62 696c 6c69 6e67 2373 6478 6c2d  nd-billing#sdxl-
+00000400: 7072 6963 696e 672d 7461 626c 6522 3e70  pricing-table">p
+00000410: 7269 6369 6e67 3c2f 613e 2061 626f 7574  ricing</a> about
+00000420: 2074 6869 732e 0d0d 0a0d 0d0a 4d61 6b65   this.......Make
+00000430: 2079 6f75 7220 696d 6167 6520 696e 203c   your image in <
+00000440: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000450: 6265 7461 2e64 7265 616d 7374 7564 696f  beta.dreamstudio
+00000460: 2e61 692f 6765 6e65 7261 7465 223e 6865  .ai/generate">he
+00000470: 7265 3c2f 613e 2062 6566 6f72 6520 646f  re</a> before do
+00000480: 696e 6720 7769 7468 2074 6869 7320 6170  ing with this ap
+00000490: 702e 0d0d 0a0d 0d0a 2323 2048 6f77 2074  p.......## How t
+000004a0: 6f20 496e 7374 616c 6c0d 0d0a 2323 2320  o Install...### 
+000004b0: 4279 2043 6c6f 6e69 6e69 670d 0d0a 312e  By Cloninig...1.
+000004c0: 2067 6974 2063 6c6f 6e65 207e 0d0d 0a32   git clone ~...2
+000004d0: 2e20 6364 2070 7971 742d 6472 6561 6d73  . cd pyqt-dreams
+000004e0: 7475 6469 6f0d 0d0a 332e 2070 6970 2069  tudio...3. pip i
+000004f0: 6e73 7461 6c6c 202d 7220 7265 7175 6972  nstall -r requir
+00000500: 656d 656e 7473 2e74 7874 0d0d 0a34 2e20  ements.txt...4. 
+00000510: 7079 7468 6f6e 2073 6574 7570 2e70 7920  python setup.py 
+00000520: 696e 7374 616c 6c0d 0d0a 352e 2063 6420  install...5. cd 
+00000530: 7079 7174 5f64 7265 616d 7374 7564 696f  pyqt_dreamstudio
+00000540: 0d0d 0a36 2e20 7079 7468 6f6e 206d 6169  ...6. python mai
+00000550: 6e2e 7079 0d0d 0a23 2323 2042 7920 7069  n.py...### By pi
+00000560: 700d 0d0a 312e 2070 6970 2069 6e73 7461  p...1. pip insta
+00000570: 6c6c 2070 7971 745f 6472 6561 6d73 7475  ll pyqt_dreamstu
+00000580: 6469 6f0d 0d0a 322e 200d 0d0a 6060 6070  dio...2. ...```p
+00000590: 7974 686f 6e0d 0d0a 6672 6f6d 2070 7971  ython...from pyq
+000005a0: 745f 6472 6561 6d73 7475 6469 6f2e 696d  t_dreamstudio.im
+000005b0: 6167 6547 656e 6572 6174 696e 6754 6f6f  ageGeneratingToo
+000005c0: 6c57 6964 6765 7420 696d 706f 7274 2049  lWidget import I
+000005d0: 6d61 6765 4765 6e65 7261 7469 6e67 546f  mageGeneratingTo
+000005e0: 6f6c 5769 6467 6574 0d0d 0a0d 0d0a 6966  olWidget......if
+000005f0: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00000600: 6d61 696e 5f5f 223a 0d0d 0a20 2020 2061  main__":...    a
+00000610: 7070 203d 2051 4170 706c 6963 6174 696f  pp = QApplicatio
+00000620: 6e28 7379 732e 6172 6776 290d 0d0a 2020  n(sys.argv)...  
+00000630: 2020 7720 3d20 496d 6167 6547 656e 6572    w = ImageGener
+00000640: 6174 696e 6754 6f6f 6c57 6964 6765 7428  atingToolWidget(
+00000650: 290d 0d0a 2020 2020 772e 7368 6f77 2829  )...    w.show()
+00000660: 0d0d 0a20 2020 2073 7973 2e65 7869 7428  ...    sys.exit(
+00000670: 6170 702e 6578 6563 5f28 2929 0d0d 0a60  app.exec_())...`
+00000680: 6060 0d0d 0a0d 0d0a 2323 2048 6f77 2074  ``......## How t
+00000690: 6f20 5573 650d 0d0a 5468 6572 6520 6973  o Use...There is
+000006a0: 2074 6865 206f 7074 696f 6e73 2074 6162   the options tab
+000006b0: 2061 7420 7468 6520 7269 6768 7420 7369   at the right si
+000006c0: 6465 206f 6620 7468 6520 7769 6e64 6f77  de of the window
+000006d0: 2e20 0d0d 0a0d 0d0a 496e 7075 7420 796f  . ......Input yo
+000006e0: 7572 2041 5049 206b 6579 2c20 6368 6f6f  ur API key, choo
+000006f0: 7365 2070 6172 616d 6574 6572 7320 796f  se parameters yo
+00000700: 7520 7761 6e74 2074 6f20 7365 742c 2077  u want to set, w
+00000710: 7269 7465 2070 726f 706d 742c 2073 7562  rite propmt, sub
+00000720: 6d69 7420 6974 2c20 616e 6420 796f 7520  mit it, and you 
+00000730: 6361 6e20 7365 6520 7468 6520 7265 7375  can see the resu
+00000740: 6c74 2061 7420 7468 6520 6c65 6674 2073  lt at the left s
+00000750: 6964 6520 2877 6869 6368 206c 6f6f 6b73  ide (which looks
+00000760: 206c 696b 6520 6669 6c65 2065 7870 6c6f   like file explo
+00000770: 7265 7229 2073 6f6f 6e20 656e 6f75 6768  rer) soon enough
+00000780: 2e0d 0d0a 0d0d 0a53 6565 2074 6865 203c  .......See the <
+00000790: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000007a0: 706c 6174 666f 726d 2e73 7461 6269 6c69  platform.stabili
+000007b0: 7479 2e61 692f 646f 6373 2f66 6561 7475  ty.ai/docs/featu
+000007c0: 7265 732f 6170 692d 7061 7261 6d65 7465  res/api-paramete
+000007d0: 7273 223e 7768 6f6c 6520 6578 706c 616e  rs">whole explan
+000007e0: 6174 696f 6e3c 2f61 3e20 6162 6f75 7420  ation</a> about 
+000007f0: 6576 6572 7920 6f70 7469 6f6e 7320 746f  every options to
+00000800: 206d 616b 6520 6265 7474 6572 2069 6d61   make better ima
+00000810: 6765 2e0d 0d0a 0d0d 0a41 6674 6572 2069  ge.......After i
+00000820: 6d61 6765 7320 676f 7420 6765 6e65 7261  mages got genera
+00000830: 7465 642c 2079 6f75 2063 616e 2063 6f70  ted, you can cop
+00000840: 7920 6f72 2064 6f77 6e6c 6f61 6420 616e  y or download an
+00000850: 7920 696d 6167 6573 2077 6865 6e20 796f  y images when yo
+00000860: 7520 7075 7420 7468 6520 6d6f 7573 6520  u put the mouse 
+00000870: 6375 7273 6f72 206f 7665 7220 7468 656d  cursor over them
+00000880: 2e20 200d 0d0a 0d0d 0a23 2320 5265 7375  .  ......## Resu
+00000890: 6c74 0d0d 0a21 5b69 6d61 6765 5d28 6874  lt...![image](ht
+000008a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000008b0: 2f79 6a67 3330 3733 372f 7079 7174 2d64  /yjg30737/pyqt-d
+000008c0: 7265 616d 7374 7564 696f 2f61 7373 6574  reamstudio/asset
+000008d0: 732f 3535 3037 3830 3433 2f38 3031 3031  s/55078043/80101
+000008e0: 6661 662d 6662 3065 2d34 3365 322d 6163  faf-fb0e-43e2-ac
+000008f0: 6239 2d32 6366 3531 6139 6666 3362 3129  b9-2cf51a9ff3b1)
+00000900: 0d0d 0a0d 0d0a 2323 204e 6f74 650d 0d0a  ......## Note...
+00000910: 4173 2066 6172 2061 7320 6920 6b6e 6f77  As far as i know
+00000920: 2c20 5573 696e 6720 5374 6162 6c65 2044  , Using Stable D
+00000930: 6966 6675 7369 6f6e 2077 6974 6820 4150  iffusion with AP
+00000940: 4920 646f 6573 6e27 7420 7375 7070 6f72  I doesn't suppor
+00000950: 7420 6469 7361 626c 6520 7361 6665 7479  t disable safety
+00000960: 2066 696c 7465 722e 2053 6861 6d65 2121   filter. Shame!!
+00000970: 0d0d 0a0d 0d0a 536f 2069 6620 796f 7520  ......So if you 
+00000980: 7479 7065 2061 6e79 2077 6f72 6473 2077  type any words w
+00000990: 6869 6368 2069 7320 636f 6e73 6964 6572  hich is consider
+000009a0: 6564 2061 7320 4e53 4657 2c20 746f 6173  ed as NSFW, toas
+000009b0: 7420 636f 6e74 6169 6e69 6e67 2065 7272  t containing err
+000009c0: 6f72 206d 6573 7361 6765 2077 696c 6c20  or message will 
+000009d0: 7368 6f77 2075 700d 0d0a 0d0d 0a23 2320  show up......## 
+000009e0: 4c69 6365 6e73 650d 0d0a 4d49 540d 0d0a  License...MIT...
```

### Comparing `pyqt-dreamstudio-0.0.1/README.md` & `pyqt-dreamstudio-0.0.11/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -49,67 +49,88 @@
 00000300: 2e64 7265 616d 7374 7564 696f 2e61 692f  .dreamstudio.ai/
 00000310: 6765 6e65 7261 7465 223e 6865 7265 3c2f  generate">here</
 00000320: 613e 2062 6566 6f72 6520 646f 696e 6720  a> before doing 
 00000330: 7769 7468 2074 6869 7320 6170 702e 0d0a  with this app...
 00000340: 0d0a 2323 2048 6f77 2074 6f20 496e 7374  ..## How to Inst
 00000350: 616c 6c0d 0a23 2323 2042 7920 436c 6f6e  all..### By Clon
 00000360: 696e 6967 0d0a 312e 2067 6974 2063 6c6f  inig..1. git clo
-00000370: 6e65 207e 0d0a 322e 2070 6970 2069 6e73  ne ~..2. pip ins
-00000380: 7461 6c6c 202d 7220 7265 7175 6972 656d  tall -r requirem
-00000390: 656e 7473 2e74 7874 0d0a 332e 2070 7974  ents.txt..3. pyt
-000003a0: 686f 6e20 6d61 696e 2e70 790d 0a23 2323  hon main.py..###
-000003b0: 2042 7920 5069 700d 0a70 6970 2069 6e73   By Pip..pip ins
-000003c0: 7461 6c6c 2070 7971 745f 6472 6561 6d73  tall pyqt_dreams
-000003d0: 7475 6469 6f0d 0a0d 0a23 2320 486f 7720  tudio....## How 
-000003e0: 746f 2055 7365 0d0a 5468 6572 6520 6973  to Use..There is
-000003f0: 2074 6865 206f 7074 696f 6e73 2074 6162   the options tab
-00000400: 2061 7420 7468 6520 7269 6768 7420 7369   at the right si
-00000410: 6465 206f 6620 7468 6520 7769 6e64 6f77  de of the window
-00000420: 2e20 0d0a 0d0a 496e 7075 7420 796f 7572  . ....Input your
-00000430: 2041 5049 206b 6579 2c20 6368 6f6f 7365   API key, choose
-00000440: 2070 6172 616d 6574 6572 7320 796f 7520   parameters you 
-00000450: 7761 6e74 2074 6f20 7365 742c 2077 7269  want to set, wri
-00000460: 7465 2070 726f 706d 742c 2073 7562 6d69  te propmt, submi
-00000470: 7420 6974 2c20 616e 6420 796f 7520 6361  t it, and you ca
-00000480: 6e20 7365 6520 7468 6520 7265 7375 6c74  n see the result
-00000490: 2061 7420 7468 6520 6c65 6674 2073 6964   at the left sid
-000004a0: 6520 2877 6869 6368 206c 6f6f 6b73 206c  e (which looks l
-000004b0: 696b 6520 6669 6c65 2065 7870 6c6f 7265  ike file explore
-000004c0: 7229 2073 6f6f 6e20 656e 6f75 6768 2e0d  r) soon enough..
-000004d0: 0a0d 0a53 6565 2074 6865 203c 6120 6872  ...See the <a hr
-000004e0: 6566 3d22 6874 7470 733a 2f2f 706c 6174  ef="https://plat
-000004f0: 666f 726d 2e73 7461 6269 6c69 7479 2e61  form.stability.a
-00000500: 692f 646f 6373 2f66 6561 7475 7265 732f  i/docs/features/
-00000510: 6170 692d 7061 7261 6d65 7465 7273 223e  api-parameters">
-00000520: 7768 6f6c 6520 6578 706c 616e 6174 696f  whole explanatio
-00000530: 6e3c 2f61 3e20 6162 6f75 7420 6576 6572  n</a> about ever
-00000540: 7920 6f70 7469 6f6e 7320 746f 206d 616b  y options to mak
-00000550: 6520 6265 7474 6572 2069 6d61 6765 2e0d  e better image..
-00000560: 0a0d 0a41 6674 6572 2069 6d61 6765 7320  ...After images 
-00000570: 676f 7420 6765 6e65 7261 7465 642c 2079  got generated, y
-00000580: 6f75 2063 616e 2063 6f70 7920 6f72 2064  ou can copy or d
-00000590: 6f77 6e6c 6f61 6420 616e 7920 696d 6167  ownload any imag
-000005a0: 6573 2077 6865 6e20 796f 7520 7075 7420  es when you put 
-000005b0: 7468 6520 6d6f 7573 6520 6375 7273 6f72  the mouse cursor
-000005c0: 206f 7665 7220 7468 656d 2e20 200d 0a0d   over them.  ...
-000005d0: 0a23 2320 5265 7375 6c74 0d0a 215b 696d  .## Result..![im
-000005e0: 6167 655d 2868 7474 7073 3a2f 2f67 6974  age](https://git
-000005f0: 6875 622e 636f 6d2f 796a 6733 3037 3337  hub.com/yjg30737
-00000600: 2f70 7971 742d 6472 6561 6d73 7475 6469  /pyqt-dreamstudi
-00000610: 6f2f 6173 7365 7473 2f35 3530 3738 3034  o/assets/5507804
-00000620: 332f 3830 3130 3166 6166 2d66 6230 652d  3/80101faf-fb0e-
-00000630: 3433 6532 2d61 6362 392d 3263 6635 3161  43e2-acb9-2cf51a
-00000640: 3966 6633 6231 290d 0a0d 0a23 2320 4e6f  9ff3b1)....## No
-00000650: 7465 0d0a 4173 2066 6172 2061 7320 6920  te..As far as i 
-00000660: 6b6e 6f77 2c20 5573 696e 6720 5374 6162  know, Using Stab
-00000670: 6c65 2044 6966 6675 7369 6f6e 2077 6974  le Diffusion wit
-00000680: 6820 4150 4920 646f 6573 6e27 7420 7375  h API doesn't su
-00000690: 7070 6f72 7420 6469 7361 626c 6520 7361  pport disable sa
-000006a0: 6665 7479 2066 696c 7465 722e 2053 6861  fety filter. Sha
-000006b0: 6d65 2121 0d0a 0d0a 536f 2069 6620 796f  me!!....So if yo
-000006c0: 7520 7479 7065 2061 6e79 2077 6f72 6473  u type any words
-000006d0: 2077 6869 6368 2069 7320 636f 6e73 6964   which is consid
-000006e0: 6572 6564 2061 7320 4e53 4657 2c20 746f  ered as NSFW, to
-000006f0: 6173 7420 636f 6e74 6169 6e69 6e67 2065  ast containing e
-00000700: 7272 6f72 206d 6573 7361 6765 2077 696c  rror message wil
-00000710: 6c20 7368 6f77 2075 700d 0a0d 0a23 2320  l show up....## 
-00000720: 4c69 6365 6e73 650d 0a4d 4954 0d0a       License..MIT..
+00000370: 6e65 207e 0d0a 322e 2063 6420 7079 7174  ne ~..2. cd pyqt
+00000380: 2d64 7265 616d 7374 7564 696f 0d0a 332e  -dreamstudio..3.
+00000390: 2070 6970 2069 6e73 7461 6c6c 202d 7220   pip install -r 
+000003a0: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
+000003b0: 0d0a 342e 2070 7974 686f 6e20 7365 7475  ..4. python setu
+000003c0: 702e 7079 2069 6e73 7461 6c6c 0d0a 352e  p.py install..5.
+000003d0: 2063 6420 7079 7174 5f64 7265 616d 7374   cd pyqt_dreamst
+000003e0: 7564 696f 0d0a 362e 2070 7974 686f 6e20  udio..6. python 
+000003f0: 6d61 696e 2e70 790d 0a23 2323 2042 7920  main.py..### By 
+00000400: 7069 700d 0a31 2e20 7069 7020 696e 7374  pip..1. pip inst
+00000410: 616c 6c20 7079 7174 5f64 7265 616d 7374  all pyqt_dreamst
+00000420: 7564 696f 0d0a 322e 200d 0a60 6060 7079  udio..2. ..```py
+00000430: 7468 6f6e 0d0a 6672 6f6d 2070 7971 745f  thon..from pyqt_
+00000440: 6472 6561 6d73 7475 6469 6f2e 696d 6167  dreamstudio.imag
+00000450: 6547 656e 6572 6174 696e 6754 6f6f 6c57  eGeneratingToolW
+00000460: 6964 6765 7420 696d 706f 7274 2049 6d61  idget import Ima
+00000470: 6765 4765 6e65 7261 7469 6e67 546f 6f6c  geGeneratingTool
+00000480: 5769 6467 6574 0d0a 0d0a 6966 205f 5f6e  Widget....if __n
+00000490: 616d 655f 5f20 3d3d 2022 5f5f 6d61 696e  ame__ == "__main
+000004a0: 5f5f 223a 0d0a 2020 2020 6170 7020 3d20  __":..    app = 
+000004b0: 5141 7070 6c69 6361 7469 6f6e 2873 7973  QApplication(sys
+000004c0: 2e61 7267 7629 0d0a 2020 2020 7720 3d20  .argv)..    w = 
+000004d0: 496d 6167 6547 656e 6572 6174 696e 6754  ImageGeneratingT
+000004e0: 6f6f 6c57 6964 6765 7428 290d 0a20 2020  oolWidget()..   
+000004f0: 2077 2e73 686f 7728 290d 0a20 2020 2073   w.show()..    s
+00000500: 7973 2e65 7869 7428 6170 702e 6578 6563  ys.exit(app.exec
+00000510: 5f28 2929 0d0a 6060 600d 0a0d 0a23 2320  _())..```....## 
+00000520: 486f 7720 746f 2055 7365 0d0a 5468 6572  How to Use..Ther
+00000530: 6520 6973 2074 6865 206f 7074 696f 6e73  e is the options
+00000540: 2074 6162 2061 7420 7468 6520 7269 6768   tab at the righ
+00000550: 7420 7369 6465 206f 6620 7468 6520 7769  t side of the wi
+00000560: 6e64 6f77 2e20 0d0a 0d0a 496e 7075 7420  ndow. ....Input 
+00000570: 796f 7572 2041 5049 206b 6579 2c20 6368  your API key, ch
+00000580: 6f6f 7365 2070 6172 616d 6574 6572 7320  oose parameters 
+00000590: 796f 7520 7761 6e74 2074 6f20 7365 742c  you want to set,
+000005a0: 2077 7269 7465 2070 726f 706d 742c 2073   write propmt, s
+000005b0: 7562 6d69 7420 6974 2c20 616e 6420 796f  ubmit it, and yo
+000005c0: 7520 6361 6e20 7365 6520 7468 6520 7265  u can see the re
+000005d0: 7375 6c74 2061 7420 7468 6520 6c65 6674  sult at the left
+000005e0: 2073 6964 6520 2877 6869 6368 206c 6f6f   side (which loo
+000005f0: 6b73 206c 696b 6520 6669 6c65 2065 7870  ks like file exp
+00000600: 6c6f 7265 7229 2073 6f6f 6e20 656e 6f75  lorer) soon enou
+00000610: 6768 2e0d 0a0d 0a53 6565 2074 6865 203c  gh.....See the <
+00000620: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000630: 706c 6174 666f 726d 2e73 7461 6269 6c69  platform.stabili
+00000640: 7479 2e61 692f 646f 6373 2f66 6561 7475  ty.ai/docs/featu
+00000650: 7265 732f 6170 692d 7061 7261 6d65 7465  res/api-paramete
+00000660: 7273 223e 7768 6f6c 6520 6578 706c 616e  rs">whole explan
+00000670: 6174 696f 6e3c 2f61 3e20 6162 6f75 7420  ation</a> about 
+00000680: 6576 6572 7920 6f70 7469 6f6e 7320 746f  every options to
+00000690: 206d 616b 6520 6265 7474 6572 2069 6d61   make better ima
+000006a0: 6765 2e0d 0a0d 0a41 6674 6572 2069 6d61  ge.....After ima
+000006b0: 6765 7320 676f 7420 6765 6e65 7261 7465  ges got generate
+000006c0: 642c 2079 6f75 2063 616e 2063 6f70 7920  d, you can copy 
+000006d0: 6f72 2064 6f77 6e6c 6f61 6420 616e 7920  or download any 
+000006e0: 696d 6167 6573 2077 6865 6e20 796f 7520  images when you 
+000006f0: 7075 7420 7468 6520 6d6f 7573 6520 6375  put the mouse cu
+00000700: 7273 6f72 206f 7665 7220 7468 656d 2e20  rsor over them. 
+00000710: 200d 0a0d 0a23 2320 5265 7375 6c74 0d0a   ....## Result..
+00000720: 215b 696d 6167 655d 2868 7474 7073 3a2f  ![image](https:/
+00000730: 2f67 6974 6875 622e 636f 6d2f 796a 6733  /github.com/yjg3
+00000740: 3037 3337 2f70 7971 742d 6472 6561 6d73  0737/pyqt-dreams
+00000750: 7475 6469 6f2f 6173 7365 7473 2f35 3530  tudio/assets/550
+00000760: 3738 3034 332f 3830 3130 3166 6166 2d66  78043/80101faf-f
+00000770: 6230 652d 3433 6532 2d61 6362 392d 3263  b0e-43e2-acb9-2c
+00000780: 6635 3161 3966 6633 6231 290d 0a0d 0a23  f51a9ff3b1)....#
+00000790: 2320 4e6f 7465 0d0a 4173 2066 6172 2061  # Note..As far a
+000007a0: 7320 6920 6b6e 6f77 2c20 5573 696e 6720  s i know, Using 
+000007b0: 5374 6162 6c65 2044 6966 6675 7369 6f6e  Stable Diffusion
+000007c0: 2077 6974 6820 4150 4920 646f 6573 6e27   with API doesn'
+000007d0: 7420 7375 7070 6f72 7420 6469 7361 626c  t support disabl
+000007e0: 6520 7361 6665 7479 2066 696c 7465 722e  e safety filter.
+000007f0: 2053 6861 6d65 2121 0d0a 0d0a 536f 2069   Shame!!....So i
+00000800: 6620 796f 7520 7479 7065 2061 6e79 2077  f you type any w
+00000810: 6f72 6473 2077 6869 6368 2069 7320 636f  ords which is co
+00000820: 6e73 6964 6572 6564 2061 7320 4e53 4657  nsidered as NSFW
+00000830: 2c20 746f 6173 7420 636f 6e74 6169 6e69  , toast containi
+00000840: 6e67 2065 7272 6f72 206d 6573 7361 6765  ng error message
+00000850: 2077 696c 6c20 7368 6f77 2075 700d 0a0d   will show up...
+00000860: 0a23 2320 4c69 6365 6e73 650d 0a4d 4954  .## License..MIT
+00000870: 0d0a                                     ..
```

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/currentImageView.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/currentImageView.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/explorerWidget.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/explorerWidget.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from qtpy.QtGui import QPixmap
 from qtpy.QtWidgets import QGridLayout, QWidget, QScrollArea, \
     QSizePolicy
 from qtpy.QtCore import Qt, Signal
 
-from thumbnailView import ThumbnailView
+from pyqt_dreamstudio.thumbnailView import ThumbnailView
 
 
 class ExplorerWidget(QScrollArea):
     clicked = Signal(QPixmap)
 
     def __init__(self):
         super().__init__()
```

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/imageListWidget.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageListWidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from datetime import datetime
 
 from qtpy.QtGui import QFont
 from qtpy.QtCore import Qt, Signal
 from qtpy.QtWidgets import QListWidget, QDialog, QListWidgetItem, QLabel, QHBoxLayout, QWidget, QApplication, QVBoxLayout
 
-from inputDialog import InputDialog
-from svgButton import SvgButton
+from pyqt_dreamstudio.inputDialog import InputDialog
+from pyqt_dreamstudio.svgButton import SvgButton
 
 
 class ImageItemWidget(QWidget):
     btnClicked = Signal(QListWidgetItem)
     imageUpdated = Signal(int, str)
 
     def __init__(self, text: str, item: QListWidgetItem, id):
```

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/imageSqlite.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageSqlite.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/imageStableDiffusionPage.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/imageStableDiffusionPage.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 
 import stability_sdk.interfaces.gooseai.generation.generation_pb2 as generation
 from qtpy.QtCore import Signal, QThread, QSettings
 from qtpy.QtWidgets import QWidget, QLineEdit, QVBoxLayout, QHBoxLayout, QGroupBox, QPushButton, QFormLayout, QSpinBox, QComboBox, \
     QLabel, QPlainTextEdit
 from stability_sdk import client
 
-from notifier import NotifierWidget
-from svgLabel import SvgLabel
+from pyqt_dreamstudio.notifier import NotifierWidget
+from pyqt_dreamstudio.svgLabel import SvgLabel
 
-from toast import Toast
+from pyqt_dreamstudio.toast import Toast
 
 os.environ['STABILITY_HOST'] = 'grpc.stability.ai:443'
 
 
 class StableDiffusionThread(QThread):
     replyGenerated = Signal(bytes)
     errorGenerated = Signal(str)
```

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/inputDialog.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/inputDialog.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/leftSideBar.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/leftSideBar.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import json
 
 from qtpy.QtCore import Signal
 from qtpy.QtWidgets import QWidget, QCheckBox, QListWidget, QVBoxLayout, QHBoxLayout, QSpacerItem, QSizePolicy, QListWidgetItem, \
     QLabel
 
-from imageListWidget import ImageListWidget
-from searchBar import SearchBar
-from svgButton import SvgButton
+from pyqt_dreamstudio.imageListWidget import ImageListWidget
+from pyqt_dreamstudio.searchBar import SearchBar
+from pyqt_dreamstudio.svgButton import SvgButton
 
 
 class LeftSideBar(QWidget):
     added = Signal()
     changed = Signal(QListWidgetItem)
     deleted = Signal(list)
     imageUpdated = Signal(int, str)
```

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/logo.png` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/logo.png`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/main.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import sys, os
 
 from qtpy.QtGui import QIcon, QGuiApplication, QFont
 from qtpy.QtWidgets import QApplication, QHBoxLayout, QVBoxLayout, QFrame, QWidget, QSplitter
 from qtpy.QtCore import Qt, Signal, QCoreApplication
 
-from leftSideBar import LeftSideBar
-from rightSideBar import RightSideBar
-from viewWidget import ViewWidget
-from svgButton import SvgButton
+from pyqt_dreamstudio.leftSideBar import LeftSideBar
+from pyqt_dreamstudio.rightSideBar import RightSideBar
+from pyqt_dreamstudio.viewWidget import ViewWidget
+from pyqt_dreamstudio.svgButton import SvgButton
 
 QApplication.setAttribute(Qt.AA_EnableHighDpiScaling)
 QCoreApplication.setAttribute(Qt.AA_UseHighDpiPixmaps)  # HighDPI support
 # qt version should be above 5.14
 if os.environ['QT_API'] == 'pyqt5' or os.environ['QT_API'] != 'pyside6':
     QGuiApplication.setHighDpiScaleFactorRoundingPolicy(Qt.HighDpiScaleFactorRoundingPolicy.PassThrough)
```

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/notifier.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/notifier.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/searchBar.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/searchBar.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/svgButton.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/svgButton.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/svgLabel.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/svgLabel.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/thumbnailView.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/thumbnailView.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import requests
 from qtpy.QtCore import Qt, QPointF, Signal
 from qtpy.QtGui import QPixmap, QColor, QBrush, QLinearGradient, QPainter
 from qtpy.QtWidgets import QGraphicsScene, QGraphicsPixmapItem, QGraphicsView, QApplication, QWidget, QHBoxLayout, \
     QFileDialog
 
-from svgButton import SvgButton
+from pyqt_dreamstudio.svgButton import SvgButton
 
 
 class ThumbnailView(QGraphicsView):
     clicked = Signal(QPixmap)
 
     def __init__(self):
         super().__init__()
```

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/toast.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/toast.py`

 * *Files identical despite different names*

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio/viewWidget.py` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio/viewWidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import requests
 
 from qtpy.QtGui import QFont, QPixmap
 from qtpy.QtWidgets import QWidget, QLabel, QGridLayout, QStackedWidget, QSplitter
 from qtpy.QtCore import Qt
 
-from explorerWidget import ExplorerWidget
-from thumbnailView import ThumbnailView
+from pyqt_dreamstudio.explorerWidget import ExplorerWidget
+from pyqt_dreamstudio.thumbnailView import ThumbnailView
 
 
 class ViewWidget(QWidget):
     def __init__(self):
         super().__init__()
         self.__initUi()
```

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio.egg-info/PKG-INFO` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,138 +1,159 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310d 0a4e 616d 653a 2070 7971  : 2.1..Name: pyq
 00000020: 742d 6472 6561 6d73 7475 6469 6f0d 0a56  t-dreamstudio..V
-00000030: 6572 7369 6f6e 3a20 302e 302e 310d 0a53  ersion: 0.0.1..S
-00000040: 756d 6d61 7279 3a20 5573 696e 6720 4472  ummary: Using Dr
-00000050: 6561 6d53 7475 6469 6f20 4150 4920 696e  eamStudio API in
-00000060: 2050 7974 686f 6e20 6465 736b 746f 7020   Python desktop 
-00000070: 6170 706c 6963 6174 696f 6e0d 0a48 6f6d  application..Hom
-00000080: 652d 7061 6765 3a20 6874 7470 733a 2f2f  e-page: https://
-00000090: 6769 7468 7562 2e63 6f6d 2f79 6a67 3330  github.com/yjg30
-000000a0: 3733 372f 7079 7174 2d64 7265 616d 7374  737/pyqt-dreamst
-000000b0: 7564 696f 2e67 6974 0d0a 4175 7468 6f72  udio.git..Author
-000000c0: 3a20 4a75 6e67 2047 7975 2059 6f6f 6e0d  : Jung Gyu Yoon.
-000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 2079  .Author-email: y
-000000e0: 6a67 3330 3733 3740 676d 6169 6c2e 636f  jg30737@gmail.co
-000000f0: 6d0d 0a4c 6963 656e 7365 3a20 4d49 540d  m..License: MIT.
-00000100: 0a44 6573 6372 6970 7469 6f6e 2d43 6f6e  .Description-Con
-00000110: 7465 6e74 2d54 7970 653a 2074 6578 742f  tent-Type: text/
-00000120: 6d61 726b 646f 776e 0d0a 4c69 6365 6e73  markdown..Licens
-00000130: 652d 4669 6c65 3a20 4c49 4345 4e53 450d  e-File: LICENSE.
-00000140: 0a0d 0a0d 0a23 2070 7971 742d 6472 6561  .....# pyqt-drea
-00000150: 6d73 7475 6469 6f0d 0d0a 5573 696e 6720  mstudio...Using 
-00000160: 4472 6561 6d53 7475 6469 6f20 4150 4920  DreamStudio API 
-00000170: 696e 2050 7974 686f 6e20 6465 736b 746f  in Python deskto
-00000180: 7020 6170 706c 6963 6174 696f 6e0d 0d0a  p application...
-00000190: 0d0d 0a59 6f75 2063 616e 206d 616b 6520  ...You can make 
-000001a0: 6120 6275 6e63 6820 6f66 2069 6d61 6765  a bunch of image
-000001b0: 2077 6974 686f 7574 2069 6e73 7461 6c6c   without install
-000001c0: 696e 6720 6865 6176 7920 7265 736f 7572  ing heavy resour
-000001d0: 6365 7320 6c69 6b65 2043 5544 412c 2074  ces like CUDA, t
-000001e0: 6f72 6368 2c20 6574 632e 2042 7574 2069  orch, etc. But i
-000001f0: 7427 7320 6e6f 7420 6672 6565 2e0d 0d0a  t's not free....
-00000200: 0d0d 0a54 6869 7320 6973 2073 6570 6172  ...This is separ
-00000210: 6174 6564 2066 726f 6d20 3c61 2068 7265  ated from <a hre
-00000220: 663d 2268 7474 7073 3a2f 2f67 6974 6875  f="https://githu
-00000230: 622e 636f 6d2f 796a 6733 3037 3337 2f70  b.com/yjg30737/p
-00000240: 7971 742d 6f70 656e 6169 223e 7079 7174  yqt-openai">pyqt
-00000250: 2d6f 7065 6e61 693c 2f61 3e20 7061 636b  -openai</a> pack
-00000260: 6167 6520 746f 2070 656f 706c 6520 7768  age to people wh
-00000270: 6f20 6f6e 6c79 2077 616e 7473 2074 6f20  o only wants to 
-00000280: 7573 6520 7374 6162 6c65 2064 6966 6675  use stable diffu
-00000290: 7369 6f6e 2061 7069 0d0d 0a0d 0d0a 616e  sion api......an
-000002a0: 6420 7768 6f20 7761 6e74 7320 746f 2066  d who wants to f
-000002b0: 6f72 6b20 7468 6973 2074 6f20 6d61 6b65  ork this to make
-000002c0: 2074 6865 6972 2061 7070 2e0d 0d0a 0d0d   their app......
-000002d0: 0a23 2320 5072 6572 6571 7569 7369 7465  .## Prerequisite
-000002e0: 200d 0d0a 596f 7520 6861 7665 2074 6f20   ...You have to 
-000002f0: 6765 7420 7468 6520 4472 6561 6d53 7475  get the DreamStu
-00000300: 6469 6f20 6170 6920 6b65 7920 6672 6f6d  dio api key from
-00000310: 203c 6120 6872 6566 3d22 6874 7470 733a   <a href="https:
-00000320: 2f2f 706c 6174 666f 726d 2e73 7461 6269  //platform.stabi
-00000330: 6c69 7479 2e61 692f 646f 6373 2f67 6574  lity.ai/docs/get
-00000340: 7469 6e67 2d73 7461 7274 6564 2f61 7574  ting-started/aut
-00000350: 6865 6e74 6963 6174 696f 6e22 3e68 6572  hentication">her
-00000360: 653c 2f61 3e2e 0d0d 0a0d 0d0a 5573 696e  e</a>.......Usin
-00000370: 6720 4472 6561 6d53 7475 6469 6f20 6f72  g DreamStudio or
-00000380: 2074 6865 2041 5049 2072 6571 7569 7265   the API require
-00000390: 7320 6372 6564 6974 732e 2054 616b 6520  s credits. Take 
-000003a0: 6120 6c6f 6f6b 2061 7420 3c61 2068 7265  a look at <a hre
-000003b0: 663d 2268 7474 7073 3a2f 2f70 6c61 7466  f="https://platf
-000003c0: 6f72 6d2e 7374 6162 696c 6974 792e 6169  orm.stability.ai
-000003d0: 2f64 6f63 732f 6765 7474 696e 672d 7374  /docs/getting-st
-000003e0: 6172 7465 642f 6372 6564 6974 732d 616e  arted/credits-an
-000003f0: 642d 6269 6c6c 696e 6723 7364 786c 2d70  d-billing#sdxl-p
-00000400: 7269 6369 6e67 2d74 6162 6c65 223e 7072  ricing-table">pr
-00000410: 6963 696e 673c 2f61 3e20 6162 6f75 7420  icing</a> about 
-00000420: 7468 6973 2e0d 0d0a 0d0d 0a4d 616b 6520  this.......Make 
-00000430: 796f 7572 2069 6d61 6765 2069 6e20 3c61  your image in <a
-00000440: 2068 7265 663d 2268 7474 7073 3a2f 2f62   href="https://b
-00000450: 6574 612e 6472 6561 6d73 7475 6469 6f2e  eta.dreamstudio.
-00000460: 6169 2f67 656e 6572 6174 6522 3e68 6572  ai/generate">her
-00000470: 653c 2f61 3e20 6265 666f 7265 2064 6f69  e</a> before doi
-00000480: 6e67 2077 6974 6820 7468 6973 2061 7070  ng with this app
-00000490: 2e0d 0d0a 0d0d 0a23 2320 486f 7720 746f  .......## How to
-000004a0: 2049 6e73 7461 6c6c 0d0d 0a23 2323 2042   Install...### B
-000004b0: 7920 436c 6f6e 696e 6967 0d0d 0a31 2e20  y Cloninig...1. 
-000004c0: 6769 7420 636c 6f6e 6520 7e0d 0d0a 322e  git clone ~...2.
-000004d0: 2070 6970 2069 6e73 7461 6c6c 202d 7220   pip install -r 
-000004e0: 7265 7175 6972 656d 656e 7473 2e74 7874  requirements.txt
-000004f0: 0d0d 0a33 2e20 7079 7468 6f6e 206d 6169  ...3. python mai
-00000500: 6e2e 7079 0d0d 0a23 2323 2042 7920 5069  n.py...### By Pi
-00000510: 700d 0d0a 7069 7020 696e 7374 616c 6c20  p...pip install 
-00000520: 7079 7174 5f64 7265 616d 7374 7564 696f  pyqt_dreamstudio
-00000530: 0d0d 0a0d 0d0a 2323 2048 6f77 2074 6f20  ......## How to 
-00000540: 5573 650d 0d0a 5468 6572 6520 6973 2074  Use...There is t
-00000550: 6865 206f 7074 696f 6e73 2074 6162 2061  he options tab a
-00000560: 7420 7468 6520 7269 6768 7420 7369 6465  t the right side
-00000570: 206f 6620 7468 6520 7769 6e64 6f77 2e20   of the window. 
-00000580: 0d0d 0a0d 0d0a 496e 7075 7420 796f 7572  ......Input your
-00000590: 2041 5049 206b 6579 2c20 6368 6f6f 7365   API key, choose
-000005a0: 2070 6172 616d 6574 6572 7320 796f 7520   parameters you 
-000005b0: 7761 6e74 2074 6f20 7365 742c 2077 7269  want to set, wri
-000005c0: 7465 2070 726f 706d 742c 2073 7562 6d69  te propmt, submi
-000005d0: 7420 6974 2c20 616e 6420 796f 7520 6361  t it, and you ca
-000005e0: 6e20 7365 6520 7468 6520 7265 7375 6c74  n see the result
-000005f0: 2061 7420 7468 6520 6c65 6674 2073 6964   at the left sid
-00000600: 6520 2877 6869 6368 206c 6f6f 6b73 206c  e (which looks l
-00000610: 696b 6520 6669 6c65 2065 7870 6c6f 7265  ike file explore
-00000620: 7229 2073 6f6f 6e20 656e 6f75 6768 2e0d  r) soon enough..
-00000630: 0d0a 0d0d 0a53 6565 2074 6865 203c 6120  .....See the <a 
-00000640: 6872 6566 3d22 6874 7470 733a 2f2f 706c  href="https://pl
-00000650: 6174 666f 726d 2e73 7461 6269 6c69 7479  atform.stability
-00000660: 2e61 692f 646f 6373 2f66 6561 7475 7265  .ai/docs/feature
-00000670: 732f 6170 692d 7061 7261 6d65 7465 7273  s/api-parameters
-00000680: 223e 7768 6f6c 6520 6578 706c 616e 6174  ">whole explanat
-00000690: 696f 6e3c 2f61 3e20 6162 6f75 7420 6576  ion</a> about ev
-000006a0: 6572 7920 6f70 7469 6f6e 7320 746f 206d  ery options to m
-000006b0: 616b 6520 6265 7474 6572 2069 6d61 6765  ake better image
-000006c0: 2e0d 0d0a 0d0d 0a41 6674 6572 2069 6d61  .......After ima
-000006d0: 6765 7320 676f 7420 6765 6e65 7261 7465  ges got generate
-000006e0: 642c 2079 6f75 2063 616e 2063 6f70 7920  d, you can copy 
-000006f0: 6f72 2064 6f77 6e6c 6f61 6420 616e 7920  or download any 
-00000700: 696d 6167 6573 2077 6865 6e20 796f 7520  images when you 
-00000710: 7075 7420 7468 6520 6d6f 7573 6520 6375  put the mouse cu
-00000720: 7273 6f72 206f 7665 7220 7468 656d 2e20  rsor over them. 
-00000730: 200d 0d0a 0d0d 0a23 2320 5265 7375 6c74   ......## Result
-00000740: 0d0d 0a21 5b69 6d61 6765 5d28 6874 7470  ...![image](http
-00000750: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f79  s://github.com/y
-00000760: 6a67 3330 3733 372f 7079 7174 2d64 7265  jg30737/pyqt-dre
-00000770: 616d 7374 7564 696f 2f61 7373 6574 732f  amstudio/assets/
-00000780: 3535 3037 3830 3433 2f38 3031 3031 6661  55078043/80101fa
-00000790: 662d 6662 3065 2d34 3365 322d 6163 6239  f-fb0e-43e2-acb9
-000007a0: 2d32 6366 3531 6139 6666 3362 3129 0d0d  -2cf51a9ff3b1)..
-000007b0: 0a0d 0d0a 2323 204e 6f74 650d 0d0a 4173  ....## Note...As
-000007c0: 2066 6172 2061 7320 6920 6b6e 6f77 2c20   far as i know, 
-000007d0: 5573 696e 6720 5374 6162 6c65 2044 6966  Using Stable Dif
-000007e0: 6675 7369 6f6e 2077 6974 6820 4150 4920  fusion with API 
-000007f0: 646f 6573 6e27 7420 7375 7070 6f72 7420  doesn't support 
-00000800: 6469 7361 626c 6520 7361 6665 7479 2066  disable safety f
-00000810: 696c 7465 722e 2053 6861 6d65 2121 0d0d  ilter. Shame!!..
-00000820: 0a0d 0d0a 536f 2069 6620 796f 7520 7479  ....So if you ty
-00000830: 7065 2061 6e79 2077 6f72 6473 2077 6869  pe any words whi
-00000840: 6368 2069 7320 636f 6e73 6964 6572 6564  ch is considered
-00000850: 2061 7320 4e53 4657 2c20 746f 6173 7420   as NSFW, toast 
-00000860: 636f 6e74 6169 6e69 6e67 2065 7272 6f72  containing error
-00000870: 206d 6573 7361 6765 2077 696c 6c20 7368   message will sh
-00000880: 6f77 2075 700d 0d0a 0d0d 0a23 2320 4c69  ow up......## Li
-00000890: 6365 6e73 650d 0d0a 4d49 540d 0d0a       cense...MIT...
+00000030: 6572 7369 6f6e 3a20 302e 302e 3131 0d0a  ersion: 0.0.11..
+00000040: 5375 6d6d 6172 793a 2055 7369 6e67 2044  Summary: Using D
+00000050: 7265 616d 5374 7564 696f 2041 5049 2069  reamStudio API i
+00000060: 6e20 5079 7468 6f6e 2064 6573 6b74 6f70  n Python desktop
+00000070: 2061 7070 6c69 6361 7469 6f6e 0d0a 486f   application..Ho
+00000080: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+00000090: 2f67 6974 6875 622e 636f 6d2f 796a 6733  /github.com/yjg3
+000000a0: 3037 3337 2f70 7971 742d 6472 6561 6d73  0737/pyqt-dreams
+000000b0: 7475 6469 6f2e 6769 740d 0a41 7574 686f  tudio.git..Autho
+000000c0: 723a 204a 756e 6720 4779 7520 596f 6f6e  r: Jung Gyu Yoon
+000000d0: 0d0a 4175 7468 6f72 2d65 6d61 696c 3a20  ..Author-email: 
+000000e0: 796a 6733 3037 3337 4067 6d61 696c 2e63  yjg30737@gmail.c
+000000f0: 6f6d 0d0a 4c69 6365 6e73 653a 204d 4954  om..License: MIT
+00000100: 0d0a 4465 7363 7269 7074 696f 6e2d 436f  ..Description-Co
+00000110: 6e74 656e 742d 5479 7065 3a20 7465 7874  ntent-Type: text
+00000120: 2f6d 6172 6b64 6f77 6e0d 0a4c 6963 656e  /markdown..Licen
+00000130: 7365 2d46 696c 653a 204c 4943 454e 5345  se-File: LICENSE
+00000140: 0d0a 0d0a 0d0a 2320 7079 7174 2d64 7265  ......# pyqt-dre
+00000150: 616d 7374 7564 696f 0d0d 0a55 7369 6e67  amstudio...Using
+00000160: 2044 7265 616d 5374 7564 696f 2041 5049   DreamStudio API
+00000170: 2069 6e20 5079 7468 6f6e 2064 6573 6b74   in Python deskt
+00000180: 6f70 2061 7070 6c69 6361 7469 6f6e 0d0d  op application..
+00000190: 0a0d 0d0a 596f 7520 6361 6e20 6d61 6b65  ....You can make
+000001a0: 2061 2062 756e 6368 206f 6620 696d 6167   a bunch of imag
+000001b0: 6520 7769 7468 6f75 7420 696e 7374 616c  e without instal
+000001c0: 6c69 6e67 2068 6561 7679 2072 6573 6f75  ling heavy resou
+000001d0: 7263 6573 206c 696b 6520 4355 4441 2c20  rces like CUDA, 
+000001e0: 746f 7263 682c 2065 7463 2e20 4275 7420  torch, etc. But 
+000001f0: 6974 2773 206e 6f74 2066 7265 652e 0d0d  it's not free...
+00000200: 0a0d 0d0a 5468 6973 2069 7320 7365 7061  ....This is sepa
+00000210: 7261 7465 6420 6672 6f6d 203c 6120 6872  rated from <a hr
+00000220: 6566 3d22 6874 7470 733a 2f2f 6769 7468  ef="https://gith
+00000230: 7562 2e63 6f6d 2f79 6a67 3330 3733 372f  ub.com/yjg30737/
+00000240: 7079 7174 2d6f 7065 6e61 6922 3e70 7971  pyqt-openai">pyq
+00000250: 742d 6f70 656e 6169 3c2f 613e 2070 6163  t-openai</a> pac
+00000260: 6b61 6765 2074 6f20 7065 6f70 6c65 2077  kage to people w
+00000270: 686f 206f 6e6c 7920 7761 6e74 7320 746f  ho only wants to
+00000280: 2075 7365 2073 7461 626c 6520 6469 6666   use stable diff
+00000290: 7573 696f 6e20 6170 690d 0d0a 0d0d 0a61  usion api......a
+000002a0: 6e64 2077 686f 2077 616e 7473 2074 6f20  nd who wants to 
+000002b0: 666f 726b 2074 6869 7320 746f 206d 616b  fork this to mak
+000002c0: 6520 7468 6569 7220 6170 702e 0d0d 0a0d  e their app.....
+000002d0: 0d0a 2323 2050 7265 7265 7175 6973 6974  ..## Prerequisit
+000002e0: 6520 0d0d 0a59 6f75 2068 6176 6520 746f  e ...You have to
+000002f0: 2067 6574 2074 6865 2044 7265 616d 5374   get the DreamSt
+00000300: 7564 696f 2061 7069 206b 6579 2066 726f  udio api key fro
+00000310: 6d20 3c61 2068 7265 663d 2268 7474 7073  m <a href="https
+00000320: 3a2f 2f70 6c61 7466 6f72 6d2e 7374 6162  ://platform.stab
+00000330: 696c 6974 792e 6169 2f64 6f63 732f 6765  ility.ai/docs/ge
+00000340: 7474 696e 672d 7374 6172 7465 642f 6175  tting-started/au
+00000350: 7468 656e 7469 6361 7469 6f6e 223e 6865  thentication">he
+00000360: 7265 3c2f 613e 2e0d 0d0a 0d0d 0a55 7369  re</a>.......Usi
+00000370: 6e67 2044 7265 616d 5374 7564 696f 206f  ng DreamStudio o
+00000380: 7220 7468 6520 4150 4920 7265 7175 6972  r the API requir
+00000390: 6573 2063 7265 6469 7473 2e20 5461 6b65  es credits. Take
+000003a0: 2061 206c 6f6f 6b20 6174 203c 6120 6872   a look at <a hr
+000003b0: 6566 3d22 6874 7470 733a 2f2f 706c 6174  ef="https://plat
+000003c0: 666f 726d 2e73 7461 6269 6c69 7479 2e61  form.stability.a
+000003d0: 692f 646f 6373 2f67 6574 7469 6e67 2d73  i/docs/getting-s
+000003e0: 7461 7274 6564 2f63 7265 6469 7473 2d61  tarted/credits-a
+000003f0: 6e64 2d62 696c 6c69 6e67 2373 6478 6c2d  nd-billing#sdxl-
+00000400: 7072 6963 696e 672d 7461 626c 6522 3e70  pricing-table">p
+00000410: 7269 6369 6e67 3c2f 613e 2061 626f 7574  ricing</a> about
+00000420: 2074 6869 732e 0d0d 0a0d 0d0a 4d61 6b65   this.......Make
+00000430: 2079 6f75 7220 696d 6167 6520 696e 203c   your image in <
+00000440: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00000450: 6265 7461 2e64 7265 616d 7374 7564 696f  beta.dreamstudio
+00000460: 2e61 692f 6765 6e65 7261 7465 223e 6865  .ai/generate">he
+00000470: 7265 3c2f 613e 2062 6566 6f72 6520 646f  re</a> before do
+00000480: 696e 6720 7769 7468 2074 6869 7320 6170  ing with this ap
+00000490: 702e 0d0d 0a0d 0d0a 2323 2048 6f77 2074  p.......## How t
+000004a0: 6f20 496e 7374 616c 6c0d 0d0a 2323 2320  o Install...### 
+000004b0: 4279 2043 6c6f 6e69 6e69 670d 0d0a 312e  By Cloninig...1.
+000004c0: 2067 6974 2063 6c6f 6e65 207e 0d0d 0a32   git clone ~...2
+000004d0: 2e20 6364 2070 7971 742d 6472 6561 6d73  . cd pyqt-dreams
+000004e0: 7475 6469 6f0d 0d0a 332e 2070 6970 2069  tudio...3. pip i
+000004f0: 6e73 7461 6c6c 202d 7220 7265 7175 6972  nstall -r requir
+00000500: 656d 656e 7473 2e74 7874 0d0d 0a34 2e20  ements.txt...4. 
+00000510: 7079 7468 6f6e 2073 6574 7570 2e70 7920  python setup.py 
+00000520: 696e 7374 616c 6c0d 0d0a 352e 2063 6420  install...5. cd 
+00000530: 7079 7174 5f64 7265 616d 7374 7564 696f  pyqt_dreamstudio
+00000540: 0d0d 0a36 2e20 7079 7468 6f6e 206d 6169  ...6. python mai
+00000550: 6e2e 7079 0d0d 0a23 2323 2042 7920 7069  n.py...### By pi
+00000560: 700d 0d0a 312e 2070 6970 2069 6e73 7461  p...1. pip insta
+00000570: 6c6c 2070 7971 745f 6472 6561 6d73 7475  ll pyqt_dreamstu
+00000580: 6469 6f0d 0d0a 322e 200d 0d0a 6060 6070  dio...2. ...```p
+00000590: 7974 686f 6e0d 0d0a 6672 6f6d 2070 7971  ython...from pyq
+000005a0: 745f 6472 6561 6d73 7475 6469 6f2e 696d  t_dreamstudio.im
+000005b0: 6167 6547 656e 6572 6174 696e 6754 6f6f  ageGeneratingToo
+000005c0: 6c57 6964 6765 7420 696d 706f 7274 2049  lWidget import I
+000005d0: 6d61 6765 4765 6e65 7261 7469 6e67 546f  mageGeneratingTo
+000005e0: 6f6c 5769 6467 6574 0d0d 0a0d 0d0a 6966  olWidget......if
+000005f0: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00000600: 6d61 696e 5f5f 223a 0d0d 0a20 2020 2061  main__":...    a
+00000610: 7070 203d 2051 4170 706c 6963 6174 696f  pp = QApplicatio
+00000620: 6e28 7379 732e 6172 6776 290d 0d0a 2020  n(sys.argv)...  
+00000630: 2020 7720 3d20 496d 6167 6547 656e 6572    w = ImageGener
+00000640: 6174 696e 6754 6f6f 6c57 6964 6765 7428  atingToolWidget(
+00000650: 290d 0d0a 2020 2020 772e 7368 6f77 2829  )...    w.show()
+00000660: 0d0d 0a20 2020 2073 7973 2e65 7869 7428  ...    sys.exit(
+00000670: 6170 702e 6578 6563 5f28 2929 0d0d 0a60  app.exec_())...`
+00000680: 6060 0d0d 0a0d 0d0a 2323 2048 6f77 2074  ``......## How t
+00000690: 6f20 5573 650d 0d0a 5468 6572 6520 6973  o Use...There is
+000006a0: 2074 6865 206f 7074 696f 6e73 2074 6162   the options tab
+000006b0: 2061 7420 7468 6520 7269 6768 7420 7369   at the right si
+000006c0: 6465 206f 6620 7468 6520 7769 6e64 6f77  de of the window
+000006d0: 2e20 0d0d 0a0d 0d0a 496e 7075 7420 796f  . ......Input yo
+000006e0: 7572 2041 5049 206b 6579 2c20 6368 6f6f  ur API key, choo
+000006f0: 7365 2070 6172 616d 6574 6572 7320 796f  se parameters yo
+00000700: 7520 7761 6e74 2074 6f20 7365 742c 2077  u want to set, w
+00000710: 7269 7465 2070 726f 706d 742c 2073 7562  rite propmt, sub
+00000720: 6d69 7420 6974 2c20 616e 6420 796f 7520  mit it, and you 
+00000730: 6361 6e20 7365 6520 7468 6520 7265 7375  can see the resu
+00000740: 6c74 2061 7420 7468 6520 6c65 6674 2073  lt at the left s
+00000750: 6964 6520 2877 6869 6368 206c 6f6f 6b73  ide (which looks
+00000760: 206c 696b 6520 6669 6c65 2065 7870 6c6f   like file explo
+00000770: 7265 7229 2073 6f6f 6e20 656e 6f75 6768  rer) soon enough
+00000780: 2e0d 0d0a 0d0d 0a53 6565 2074 6865 203c  .......See the <
+00000790: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000007a0: 706c 6174 666f 726d 2e73 7461 6269 6c69  platform.stabili
+000007b0: 7479 2e61 692f 646f 6373 2f66 6561 7475  ty.ai/docs/featu
+000007c0: 7265 732f 6170 692d 7061 7261 6d65 7465  res/api-paramete
+000007d0: 7273 223e 7768 6f6c 6520 6578 706c 616e  rs">whole explan
+000007e0: 6174 696f 6e3c 2f61 3e20 6162 6f75 7420  ation</a> about 
+000007f0: 6576 6572 7920 6f70 7469 6f6e 7320 746f  every options to
+00000800: 206d 616b 6520 6265 7474 6572 2069 6d61   make better ima
+00000810: 6765 2e0d 0d0a 0d0d 0a41 6674 6572 2069  ge.......After i
+00000820: 6d61 6765 7320 676f 7420 6765 6e65 7261  mages got genera
+00000830: 7465 642c 2079 6f75 2063 616e 2063 6f70  ted, you can cop
+00000840: 7920 6f72 2064 6f77 6e6c 6f61 6420 616e  y or download an
+00000850: 7920 696d 6167 6573 2077 6865 6e20 796f  y images when yo
+00000860: 7520 7075 7420 7468 6520 6d6f 7573 6520  u put the mouse 
+00000870: 6375 7273 6f72 206f 7665 7220 7468 656d  cursor over them
+00000880: 2e20 200d 0d0a 0d0d 0a23 2320 5265 7375  .  ......## Resu
+00000890: 6c74 0d0d 0a21 5b69 6d61 6765 5d28 6874  lt...![image](ht
+000008a0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000008b0: 2f79 6a67 3330 3733 372f 7079 7174 2d64  /yjg30737/pyqt-d
+000008c0: 7265 616d 7374 7564 696f 2f61 7373 6574  reamstudio/asset
+000008d0: 732f 3535 3037 3830 3433 2f38 3031 3031  s/55078043/80101
+000008e0: 6661 662d 6662 3065 2d34 3365 322d 6163  faf-fb0e-43e2-ac
+000008f0: 6239 2d32 6366 3531 6139 6666 3362 3129  b9-2cf51a9ff3b1)
+00000900: 0d0d 0a0d 0d0a 2323 204e 6f74 650d 0d0a  ......## Note...
+00000910: 4173 2066 6172 2061 7320 6920 6b6e 6f77  As far as i know
+00000920: 2c20 5573 696e 6720 5374 6162 6c65 2044  , Using Stable D
+00000930: 6966 6675 7369 6f6e 2077 6974 6820 4150  iffusion with AP
+00000940: 4920 646f 6573 6e27 7420 7375 7070 6f72  I doesn't suppor
+00000950: 7420 6469 7361 626c 6520 7361 6665 7479  t disable safety
+00000960: 2066 696c 7465 722e 2053 6861 6d65 2121   filter. Shame!!
+00000970: 0d0d 0a0d 0d0a 536f 2069 6620 796f 7520  ......So if you 
+00000980: 7479 7065 2061 6e79 2077 6f72 6473 2077  type any words w
+00000990: 6869 6368 2069 7320 636f 6e73 6964 6572  hich is consider
+000009a0: 6564 2061 7320 4e53 4657 2c20 746f 6173  ed as NSFW, toas
+000009b0: 7420 636f 6e74 6169 6e69 6e67 2065 7272  t containing err
+000009c0: 6f72 206d 6573 7361 6765 2077 696c 6c20  or message will 
+000009d0: 7368 6f77 2075 700d 0d0a 0d0d 0a23 2320  show up......## 
+000009e0: 4c69 6365 6e73 650d 0d0a 4d49 540d 0d0a  License...MIT...
```

### Comparing `pyqt-dreamstudio-0.0.1/pyqt_dreamstudio.egg-info/SOURCES.txt` & `pyqt-dreamstudio-0.0.11/pyqt_dreamstudio.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,8 +20,10 @@
 pyqt_dreamstudio/toast.py
 pyqt_dreamstudio/viewWidget.py
 pyqt_dreamstudio.egg-info/PKG-INFO
 pyqt_dreamstudio.egg-info/SOURCES.txt
 pyqt_dreamstudio.egg-info/dependency_links.txt
 pyqt_dreamstudio.egg-info/requires.txt
 pyqt_dreamstudio.egg-info/top_level.txt
-pyqt_dreamstudio/ico/__init__.py
+pyqt_dreamstudio/ico/__init__.py
+pyqt_dreamstudio/ico/history.svg
+pyqt_dreamstudio/ico/setting.svg
```

### Comparing `pyqt-dreamstudio-0.0.1/setup.py` & `pyqt-dreamstudio-0.0.11/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 setup(
     name='pyqt-dreamstudio',
-    version='0.0.1',
+    version='0.0.11',
     author='Jung Gyu Yoon',
     author_email='yjg30737@gmail.com',
     license='MIT',
     packages=find_packages(),
-    package_data={'pyqt_dreamstudio': ['logo.png'], 'ico': ['history.svg', 'setting.svg']},
+    package_data={'pyqt_dreamstudio': ['logo.png'], 'pyqt_dreamstudio.ico': ['history.svg', 'setting.svg']},
     description='Using DreamStudio API in Python desktop application',
     url='https://github.com/yjg30737/pyqt-dreamstudio.git',
     long_description_content_type='text/markdown',
     long_description=long_description,
     install_requires=[
         'PyQt5>=5.14',
         'PySide6',
```


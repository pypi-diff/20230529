# Comparing `tmp/act4e_mcdp-0.6.5-py3-none-any.whl.zip` & `tmp/act4e_mcdp-0.6.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 295918 bytes, number of entries: 16
--rw-r--r--  2.0 unx      424 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
+Zip file size: 295914 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      422 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
 -rw-r--r--  2.0 unx  1268167 b- defN 80-Jan-01 00:00 act4e_mcdp/autogen_packed_test_data.py
 -rw-r--r--  2.0 unx      571 b- defN 80-Jan-01 00:00 act4e_mcdp/download.py
 -rw-r--r--  2.0 unx    10779 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
 -rw-r--r--  2.0 unx     3281 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_dp.py
 -rw-r--r--  2.0 unx     4964 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_dp_queries.py
 -rw-r--r--  2.0 unx     3924 b- defN 80-Jan-01 00:00 act4e_mcdp/main_solve_mcdp.py
 -rw-r--r--  2.0 unx     4656 b- defN 80-Jan-01 00:00 act4e_mcdp/nameddps.py
 -rw-r--r--  2.0 unx     1790 b- defN 80-Jan-01 00:00 act4e_mcdp/posets.py
 -rw-r--r--  2.0 unx    11916 b- defN 80-Jan-01 00:00 act4e_mcdp/primitivedps.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 act4e_mcdp/py.typed
 -rw-r--r--  2.0 unx     7955 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
--rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.5.dist-info/WHEEL
--rw-r--r--  2.0 unx      225 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.5.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1310 b- defN 16-Jan-01 00:00 act4e_mcdp-0.6.5.dist-info/RECORD
-16 files, 1320411 bytes uncompressed, 293768 bytes compressed:  77.8%
+-rw-r--r--  2.0 unx      361 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx      225 b- defN 80-Jan-01 00:00 act4e_mcdp-0.6.6.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1310 b- defN 16-Jan-01 00:00 act4e_mcdp-0.6.6.dist-info/RECORD
+16 files, 1320409 bytes uncompressed, 293764 bytes compressed:  77.8%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: act4e_mcdp/py.typed
 Comment: 
 
 Filename: act4e_mcdp/solution_interface.py
 Comment: 
 
-Filename: act4e_mcdp-0.6.5.dist-info/METADATA
+Filename: act4e_mcdp-0.6.6.dist-info/METADATA
 Comment: 
 
-Filename: act4e_mcdp-0.6.5.dist-info/WHEEL
+Filename: act4e_mcdp-0.6.6.dist-info/WHEEL
 Comment: 
 
-Filename: act4e_mcdp-0.6.5.dist-info/entry_points.txt
+Filename: act4e_mcdp-0.6.6.dist-info/entry_points.txt
 Comment: 
 
-Filename: act4e_mcdp-0.6.5.dist-info/RECORD
+Filename: act4e_mcdp-0.6.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## act4e_mcdp/__init__.py

```diff
@@ -3,15 +3,15 @@
 coloredlogs.install(level="DEBUG")
 
 from logging import getLogger, DEBUG
 
 logger = getLogger(__name__)
 logger.setLevel(DEBUG)
 
-# __version__ = "0.2.1"
+__version__ = "0.6.6"
 
 from .loading import *
 from .main_solve_mcdp import *
 from .main_solve_dp import *
 from .solution_interface import *
 from .nameddps import *
 from .primitivedps import *
```

## Comparing `act4e_mcdp-0.6.5.dist-info/RECORD` & `act4e_mcdp-0.6.6.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-act4e_mcdp/__init__.py,sha256=GQsby_cbaGnIexdyFinnY6jVbCNIvaqBNwyEjsVvUjk,424
+act4e_mcdp/__init__.py,sha256=ydJHVaahecdLwpsp90HNLGAKSPh8W1sBkNNG9shkbPg,422
 act4e_mcdp/autogen_packed_test_data.py,sha256=P2HKZV9ybQgeYbiSq2xXehpuWS32O71adYsvu4TxdCE,1268167
 act4e_mcdp/download.py,sha256=fXm46ISIYvpFjouSMB0l0XLuJWw5CxZSpgi-fvmxMGA,571
 act4e_mcdp/loading.py,sha256=VbEkB6W13mueld_Sqn4PYyOLMhmVdWK2xzhqwRySm4Q,10779
 act4e_mcdp/main_solve_dp.py,sha256=qq6hdqu0LBLjK-1gJyayFhHsGFd0vvbHMgR4PVTWKYo,3281
 act4e_mcdp/main_solve_dp_queries.py,sha256=O305xUXgLAzHIg873k9v76BmFMVBS6YIJqh-u9xFq8Q,4964
 act4e_mcdp/main_solve_mcdp.py,sha256=zOAJhpY2S2E_P_c_UXkS4bMB40FxohF4iDMZlfRS-q0,3924
 act4e_mcdp/nameddps.py,sha256=knysGfVrbeilCg9gX4B7S-b8JcuwbfFJN-WMxgCBrXo,4656
 act4e_mcdp/posets.py,sha256=7iijB7waZd3nTyK-_eNBR6YZOWhcTUYtKqCm7irpFKE,1790
 act4e_mcdp/primitivedps.py,sha256=dfA15BwI43XJQMx6OLf2rTu31TWnHcnpIKUaDPxc3r0,11916
 act4e_mcdp/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 act4e_mcdp/solution_interface.py,sha256=ZXjfYHep9JNFukgCJfgs5smqrwazsXmkJU9Da4LIQsg,7955
-act4e_mcdp-0.6.5.dist-info/METADATA,sha256=6-BmNPh3rhMu7-fwHHNzwB7SQKnNqjC__dAWsB5ekTE,361
-act4e_mcdp-0.6.5.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-act4e_mcdp-0.6.5.dist-info/entry_points.txt,sha256=cFH3w3DzczOms0kJedGgJfIn3m4Ip6dqqlcFy5dRWWI,225
-act4e_mcdp-0.6.5.dist-info/RECORD,,
+act4e_mcdp-0.6.6.dist-info/METADATA,sha256=q8jgv2x1w4En3VNtRt3u7wioVXiDcZrUf5blGIVmdnI,361
+act4e_mcdp-0.6.6.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+act4e_mcdp-0.6.6.dist-info/entry_points.txt,sha256=cFH3w3DzczOms0kJedGgJfIn3m4Ip6dqqlcFy5dRWWI,225
+act4e_mcdp-0.6.6.dist-info/RECORD,,
```


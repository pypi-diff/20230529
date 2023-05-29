# Comparing `tmp/cloudtoken-2.1.6-py3-none-any.whl.zip` & `tmp/cloudtoken-2.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 52814 bytes, number of entries: 44
+Zip file size: 54229 bytes, number of entries: 44
 -rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cloudtoken/core/__init__.py
 -rw-r--r--  2.0 unx      126 b- defN 80-Jan-01 00:00 cloudtoken/core/__main__.py
 -rw-r--r--  2.0 unx     3938 b- defN 80-Jan-01 00:00 cloudtoken/core/abstract_classes.py
 -rw-r--r--  2.0 unx     3936 b- defN 80-Jan-01 00:00 cloudtoken/core/cli.py
 -rw-r--r--  2.0 unx     9715 b- defN 80-Jan-01 00:00 cloudtoken/core/core.py
 -rw-r--r--  2.0 unx     7817 b- defN 80-Jan-01 00:00 cloudtoken/core/daemon.py
 -rw-r--r--  2.0 unx      840 b- defN 80-Jan-01 00:00 cloudtoken/core/exceptions.py
@@ -34,13 +34,13 @@
 -rw-r--r--  2.0 unx     1211 b- defN 80-Jan-01 00:00 cloudtoken/plugins/okta/factors/push.py
 -rw-r--r--  2.0 unx      223 b- defN 80-Jan-01 00:00 cloudtoken/plugins/okta/factors/totp.py
 -rw-r--r--  2.0 unx     8693 b- defN 80-Jan-01 00:00 cloudtoken/plugins/okta/plugin.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 cloudtoken/plugins/saml/__init__.py
 -rw-r--r--  2.0 unx     9116 b- defN 80-Jan-01 00:00 cloudtoken/plugins/saml/plugin.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 cloudtoken/plugins/url_generator/__init__.py
 -rw-r--r--  2.0 unx     3663 b- defN 80-Jan-01 00:00 cloudtoken/plugins/url_generator/plugin.py
--rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 cloudtoken-2.1.6.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     1008 b- defN 80-Jan-01 00:00 cloudtoken-2.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cloudtoken-2.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 cloudtoken-2.1.6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     4115 b- defN 16-Jan-01 00:00 cloudtoken-2.1.6.dist-info/RECORD
-44 files, 154983 bytes uncompressed, 46038 bytes compressed:  70.3%
+-rw-r--r--  2.0 unx      560 b- defN 80-Jan-01 00:00 cloudtoken-2.1.7.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     3979 b- defN 80-Jan-01 00:00 cloudtoken-2.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cloudtoken-2.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 cloudtoken-2.1.7.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     4115 b- defN 16-Jan-01 00:00 cloudtoken-2.1.7.dist-info/RECORD
+44 files, 157954 bytes uncompressed, 47453 bytes compressed:  70.0%
```

## zipnote {}

```diff
@@ -111,23 +111,23 @@
 
 Filename: cloudtoken/plugins/url_generator/__init__.py
 Comment: 
 
 Filename: cloudtoken/plugins/url_generator/plugin.py
 Comment: 
 
-Filename: cloudtoken-2.1.6.dist-info/LICENSE.txt
+Filename: cloudtoken-2.1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: cloudtoken-2.1.6.dist-info/METADATA
+Filename: cloudtoken-2.1.7.dist-info/METADATA
 Comment: 
 
-Filename: cloudtoken-2.1.6.dist-info/WHEEL
+Filename: cloudtoken-2.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: cloudtoken-2.1.6.dist-info/entry_points.txt
+Filename: cloudtoken-2.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: cloudtoken-2.1.6.dist-info/RECORD
+Filename: cloudtoken-2.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cloudtoken/core/__init__.py

```diff
@@ -1,3 +1,3 @@
 # THIS FILE IS OVERWRITTEN BY sync_versions.py
-__version__ = "2.1.6"
+__version__ = "2.1.7"
```

## Comparing `cloudtoken-2.1.6.dist-info/LICENSE.txt` & `cloudtoken-2.1.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `cloudtoken-2.1.6.dist-info/RECORD` & `cloudtoken-2.1.7.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-cloudtoken/core/__init__.py,sha256=0pqj2wDcRLkdTrWjOw0bmekHKPWahGKhyyhBcalkGQI,73
+cloudtoken/core/__init__.py,sha256=Rp8mMtT1irneq1gBOFkwLjH3ugP52jzL2FDxHf-Oul4,73
 cloudtoken/core/__main__.py,sha256=rq3N-tTr2XIiITRpACY8tNbovFWxfRfvCQhzvo02XKs,126
 cloudtoken/core/abstract_classes.py,sha256=W2BD5ulQjLUURvsQ3BhVUPVMAFu10nEwQOHthoGS0uw,3938
 cloudtoken/core/cli.py,sha256=SVH28ao5RmiPg-nB6lOeVD8TJIf_8xLklIBSEdj8Rjw,3936
 cloudtoken/core/core.py,sha256=1YhXBsdop3aDTXf18fJlgSh-CvMwE7KOxLpud7_5dOw,9715
 cloudtoken/core/daemon.py,sha256=4v6iONQA8E_b3ujWR1QtfTJZ5Zh6JzIGtKAeDUgxIr8,7817
 cloudtoken/core/exceptions.py,sha256=ZZYiIEsuuGhmA1h-L8YiJLGNf2sboVwn2t44UxvG5S0,840
 cloudtoken/core/helper_classes.py,sha256=8v0gn8xYU3s_83BO7PW3SFSCKAOyyBD8KW-9BhO6dFk,322
@@ -33,12 +33,12 @@
 cloudtoken/plugins/okta/factors/push.py,sha256=R4hD4P8iiYwqr4KLX2mnK1zDvUc31i5W77kvTpw6eYY,1211
 cloudtoken/plugins/okta/factors/totp.py,sha256=m3E8ofTK_-cotHgefZsjqR_cUqyeqYAa2E-rCE-TwQk,223
 cloudtoken/plugins/okta/plugin.py,sha256=opOzN33Kc9E2q5JYx_s_mdf_Jii2Ns6HzTj7cmXAwpU,8693
 cloudtoken/plugins/saml/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cloudtoken/plugins/saml/plugin.py,sha256=XJWrFD17RGyPnvD-w31Ys5nZfMa7EE0493NtvOuLzvg,9116
 cloudtoken/plugins/url_generator/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cloudtoken/plugins/url_generator/plugin.py,sha256=Nc4EEN2kBytu3dlU3Mq5tza9EmSrdrU5tb_Jr-YCIKw,3663
-cloudtoken-2.1.6.dist-info/LICENSE.txt,sha256=CPMAOoxzsoQ99XIeHPg-85bC-DbzktyCKw79eoRj8Ds,560
-cloudtoken-2.1.6.dist-info/METADATA,sha256=zfaSij4NQmYEcHIy7VVUyySI8BRWbP4WpjipFv3t1CE,1008
-cloudtoken-2.1.6.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-cloudtoken-2.1.6.dist-info/entry_points.txt,sha256=2KarfdhhAiPZ6yTMDAtJCkTdtS7pheheoPGQMPxor8I,54
-cloudtoken-2.1.6.dist-info/RECORD,,
+cloudtoken-2.1.7.dist-info/LICENSE.txt,sha256=CPMAOoxzsoQ99XIeHPg-85bC-DbzktyCKw79eoRj8Ds,560
+cloudtoken-2.1.7.dist-info/METADATA,sha256=DYrm9puFr4D19FKUSZyoNG-Rvw1cOT_3d2ViWLtuVK0,3979
+cloudtoken-2.1.7.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+cloudtoken-2.1.7.dist-info/entry_points.txt,sha256=2KarfdhhAiPZ6yTMDAtJCkTdtS7pheheoPGQMPxor8I,54
+cloudtoken-2.1.7.dist-info/RECORD,,
```


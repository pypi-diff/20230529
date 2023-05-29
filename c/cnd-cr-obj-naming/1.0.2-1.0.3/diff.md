# Comparing `tmp/cnd_cr_obj_naming-1.0.2-py3-none-any.whl.zip` & `tmp/cnd_cr_obj_naming-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 3451 bytes, number of entries: 9
 -rw-rw-rw-  2.0 unx        5 b- defN 23-May-29 15:44 cr_obj_naming/VERSION
 -rw-r--r--  2.0 unx      187 b- defN 23-May-29 15:44 cr_obj_naming/__init__.py
 -rw-r--r--  2.0 unx      122 b- defN 23-May-29 15:44 cr_obj_naming/__version__.py
 -rw-r--r--  2.0 unx     1454 b- defN 23-May-29 15:44 cr_obj_naming/cnd_consul.py
 -rw-r--r--  2.0 unx     1456 b- defN 23-May-29 15:44 cr_obj_naming/obj_naming.py
--rw-r--r--  2.0 unx      758 b- defN 23-May-29 15:44 cnd_cr_obj_naming-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 15:44 cnd_cr_obj_naming-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 23-May-29 15:44 cnd_cr_obj_naming-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      745 b- defN 23-May-29 15:44 cnd_cr_obj_naming-1.0.2.dist-info/RECORD
+-rw-r--r--  2.0 unx      758 b- defN 23-May-29 15:44 cnd_cr_obj_naming-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 15:44 cnd_cr_obj_naming-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 23-May-29 15:44 cnd_cr_obj_naming-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      745 b- defN 23-May-29 15:44 cnd_cr_obj_naming-1.0.3.dist-info/RECORD
 9 files, 4833 bytes uncompressed, 2153 bytes compressed:  55.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: cr_obj_naming/cnd_consul.py
 Comment: 
 
 Filename: cr_obj_naming/obj_naming.py
 Comment: 
 
-Filename: cnd_cr_obj_naming-1.0.2.dist-info/METADATA
+Filename: cnd_cr_obj_naming-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: cnd_cr_obj_naming-1.0.2.dist-info/WHEEL
+Filename: cnd_cr_obj_naming-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: cnd_cr_obj_naming-1.0.2.dist-info/top_level.txt
+Filename: cnd_cr_obj_naming-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: cnd_cr_obj_naming-1.0.2.dist-info/RECORD
+Filename: cnd_cr_obj_naming-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cr_obj_naming/VERSION

```diff
@@ -1 +1 @@
-1.0.2
+1.0.3
```

## Comparing `cnd_cr_obj_naming-1.0.2.dist-info/METADATA` & `cnd_cr_obj_naming-1.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnd-cr-obj-naming
-Version: 1.0.2
+Version: 1.0.3
 Summary: Base for vro Custom Resource Object Naming
 Home-page: https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
 Author: Denis FABIEN
 Author-email: denis.fabien@changendevops.com
 License: MIT/X11
 Project-URL: Documentation, https://changendevops.com
 Project-URL: Source, https://gitlab.com/changendevops/cloudtools/cnd-cr-object.git
```

## Comparing `cnd_cr_obj_naming-1.0.2.dist-info/RECORD` & `cnd_cr_obj_naming-1.0.3.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-cr_obj_naming/VERSION,sha256=v-wuNFg62n5q8stzmT-3Wj9xR6bJQ-X_X1xClPxXe5A,5
+cr_obj_naming/VERSION,sha256=INLLCW0atBpBQCRtEvB79rjLdD_UgSK3JTLAPUTFwUo,5
 cr_obj_naming/__init__.py,sha256=1uv3gz09BL1cmYDLPne0PkqXcvqxLP9jy2DjeeyDCrA,187
 cr_obj_naming/__version__.py,sha256=ikxlExFPaHGK8AzUG9pDnI7Sm8GtkjdM12d5iJMRgik,122
 cr_obj_naming/cnd_consul.py,sha256=Y1651yLtYfWz6z-Cfz9hwXyplHkF8bS8fiOY7b_FaZ0,1454
 cr_obj_naming/obj_naming.py,sha256=-U-exAK7zbnDEKECyjWvhN5ErsmPBK47rybAlu4Qs_4,1456
-cnd_cr_obj_naming-1.0.2.dist-info/METADATA,sha256=TxVAVqKfu0xsXW4mC64oIy6V1r0MXFXVjpggwvxdCSw,758
-cnd_cr_obj_naming-1.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cnd_cr_obj_naming-1.0.2.dist-info/top_level.txt,sha256=IxheoHqwoyK8b3XMzAfOoe8Owc9qJeKmqwl2BTPOmBU,14
-cnd_cr_obj_naming-1.0.2.dist-info/RECORD,,
+cnd_cr_obj_naming-1.0.3.dist-info/METADATA,sha256=w6PjUPLWUpTvaCvVnAcl-KjxvOzW-UQpau8ogmqHPX0,758
+cnd_cr_obj_naming-1.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cnd_cr_obj_naming-1.0.3.dist-info/top_level.txt,sha256=IxheoHqwoyK8b3XMzAfOoe8Owc9qJeKmqwl2BTPOmBU,14
+cnd_cr_obj_naming-1.0.3.dist-info/RECORD,,
```


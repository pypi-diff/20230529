# Comparing `tmp/edaplore-0.3.6-py3-none-any.whl.zip` & `tmp/edaplore-0.3.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1354 bytes, number of entries: 5
--rw-r--r--  2.0 unx       33 b- defN 23-May-28 22:51 edaplore/__init__.py
--rw-r--r--  2.0 unx      488 b- defN 23-May-28 22:51 edaplore-0.3.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-28 22:51 edaplore-0.3.6.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-28 22:51 edaplore-0.3.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      375 b- defN 23-May-28 22:51 edaplore-0.3.6.dist-info/RECORD
-5 files, 997 bytes uncompressed, 648 bytes compressed:  35.0%
+Zip file size: 1356 bytes, number of entries: 5
+-rw-r--r--  2.0 unx       34 b- defN 23-May-28 22:53 edaplore/__init__.py
+-rw-r--r--  2.0 unx      488 b- defN 23-May-28 22:53 edaplore-0.3.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-28 22:53 edaplore-0.3.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-28 22:53 edaplore-0.3.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      375 b- defN 23-May-28 22:53 edaplore-0.3.7.dist-info/RECORD
+5 files, 998 bytes uncompressed, 650 bytes compressed:  34.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: edaplore/__init__.py
 Comment: 
 
-Filename: edaplore-0.3.6.dist-info/METADATA
+Filename: edaplore-0.3.7.dist-info/METADATA
 Comment: 
 
-Filename: edaplore-0.3.6.dist-info/WHEEL
+Filename: edaplore-0.3.7.dist-info/WHEEL
 Comment: 
 
-Filename: edaplore-0.3.6.dist-info/top_level.txt
+Filename: edaplore-0.3.7.dist-info/top_level.txt
 Comment: 
 
-Filename: edaplore-0.3.6.dist-info/RECORD
+Filename: edaplore-0.3.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edaplore/__init__.py

```diff
@@ -1 +1 @@
-from report.report import Report
+from .report.report import Report
```


# Comparing `tmp/revo-0.0.1-py3-none-any.whl.zip` & `tmp/revo-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,9 @@
-Zip file size: 1258 bytes, number of entries: 5
--rw-r--r--  2.0 unx       38 b- defN 23-May-29 07:25 src/__init__.py
--rw-r--r--  2.0 unx      316 b- defN 23-May-29 07:27 revo-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 07:27 revo-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-May-29 07:27 revo-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      354 b- defN 23-May-29 07:27 revo-0.0.1.dist-info/RECORD
-5 files, 804 bytes uncompressed, 594 bytes compressed:  26.1%
+Zip file size: 3688 bytes, number of entries: 7
+-rw-r--r--  2.0 unx       24 b- defN 23-May-29 11:26 revo/__init__.py
+-rw-r--r--  2.0 unx     4924 b- defN 23-May-29 11:25 revo/_revo.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-May-29 12:30 revo-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      541 b- defN 23-May-29 12:30 revo-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 12:30 revo-0.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-29 12:30 revo-0.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      510 b- defN 23-May-29 12:30 revo-0.1.0.dist-info/RECORD
+7 files, 7164 bytes uncompressed, 2788 bytes compressed:  61.1%
```

## zipnote {}

```diff
@@ -1,16 +1,22 @@
-Filename: src/__init__.py
+Filename: revo/__init__.py
 Comment: 
 
-Filename: revo-0.0.1.dist-info/METADATA
+Filename: revo/_revo.py
 Comment: 
 
-Filename: revo-0.0.1.dist-info/WHEEL
+Filename: revo-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: revo-0.0.1.dist-info/top_level.txt
+Filename: revo-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: revo-0.0.1.dist-info/RECORD
+Filename: revo-0.1.0.dist-info/WHEEL
+Comment: 
+
+Filename: revo-0.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: revo-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```


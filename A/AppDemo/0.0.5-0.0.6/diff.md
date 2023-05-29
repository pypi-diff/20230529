# Comparing `tmp/AppDemo-0.0.5-py3-none-any.whl.zip` & `tmp/AppDemo-0.0.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 2384 bytes, number of entries: 7
--rw-r--r--  2.0 unx      132 b- defN 23-May-29 03:51 app.py
+Zip file size: 2397 bytes, number of entries: 7
+-rw-r--r--  2.0 unx      132 b- defN 23-May-29 03:51 app/demo.py
 -rw-r--r--  2.0 unx       41 b- defN 23-May-29 05:51 app/hello_world.py
--rw-r--r--  2.0 unx     1055 b- defN 23-May-29 06:11 AppDemo-0.0.5.dist-info/LICENSE
--rw-r--r--  2.0 unx      362 b- defN 23-May-29 06:11 AppDemo-0.0.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 06:11 AppDemo-0.0.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-May-29 06:11 AppDemo-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      519 b- defN 23-May-29 06:11 AppDemo-0.0.5.dist-info/RECORD
-7 files, 2205 bytes uncompressed, 1464 bytes compressed:  33.6%
+-rw-r--r--  2.0 unx     1055 b- defN 23-May-29 06:20 AppDemo-0.0.6.dist-info/LICENSE
+-rw-r--r--  2.0 unx      362 b- defN 23-May-29 06:20 AppDemo-0.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 06:20 AppDemo-0.0.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-May-29 06:20 AppDemo-0.0.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      524 b- defN 23-May-29 06:20 AppDemo-0.0.6.dist-info/RECORD
+7 files, 2210 bytes uncompressed, 1467 bytes compressed:  33.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
-Filename: app.py
+Filename: app/demo.py
 Comment: 
 
 Filename: app/hello_world.py
 Comment: 
 
-Filename: AppDemo-0.0.5.dist-info/LICENSE
+Filename: AppDemo-0.0.6.dist-info/LICENSE
 Comment: 
 
-Filename: AppDemo-0.0.5.dist-info/METADATA
+Filename: AppDemo-0.0.6.dist-info/METADATA
 Comment: 
 
-Filename: AppDemo-0.0.5.dist-info/WHEEL
+Filename: AppDemo-0.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: AppDemo-0.0.5.dist-info/top_level.txt
+Filename: AppDemo-0.0.6.dist-info/top_level.txt
 Comment: 
 
-Filename: AppDemo-0.0.5.dist-info/RECORD
+Filename: AppDemo-0.0.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `AppDemo-0.0.5.dist-info/LICENSE` & `AppDemo-0.0.6.dist-info/LICENSE`

 * *Files identical despite different names*


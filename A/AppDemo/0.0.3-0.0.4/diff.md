# Comparing `tmp/AppDemo-0.0.3-py3-none-any.whl.zip` & `tmp/AppDemo-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 2179 bytes, number of entries: 6
+Zip file size: 2382 bytes, number of entries: 7
 -rw-r--r--  2.0 unx      132 b- defN 23-May-29 03:51 app.py
--rw-r--r--  2.0 unx     1055 b- defN 23-May-29 03:52 AppDemo-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx      362 b- defN 23-May-29 03:52 AppDemo-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-29 03:52 AppDemo-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 23-May-29 03:52 AppDemo-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      446 b- defN 23-May-29 03:52 AppDemo-0.0.3.dist-info/RECORD
-6 files, 2091 bytes uncompressed, 1371 bytes compressed:  34.4%
+-rw-r--r--  2.0 unx       41 b- defN 23-May-29 05:51 app/hello_world.py
+-rw-r--r--  2.0 unx     1055 b- defN 23-May-29 05:56 AppDemo-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx      362 b- defN 23-May-29 05:56 AppDemo-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 05:56 AppDemo-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 23-May-29 05:56 AppDemo-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      519 b- defN 23-May-29 05:56 AppDemo-0.0.4.dist-info/RECORD
+7 files, 2205 bytes uncompressed, 1462 bytes compressed:  33.7%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: app.py
 Comment: 
 
-Filename: AppDemo-0.0.3.dist-info/LICENSE
+Filename: app/hello_world.py
 Comment: 
 
-Filename: AppDemo-0.0.3.dist-info/METADATA
+Filename: AppDemo-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: AppDemo-0.0.3.dist-info/WHEEL
+Filename: AppDemo-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: AppDemo-0.0.3.dist-info/top_level.txt
+Filename: AppDemo-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: AppDemo-0.0.3.dist-info/RECORD
+Filename: AppDemo-0.0.4.dist-info/top_level.txt
+Comment: 
+
+Filename: AppDemo-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `AppDemo-0.0.3.dist-info/LICENSE` & `AppDemo-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*


# Comparing `tmp/mb_base-1.0.202305291037-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202305291038-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4365 bytes, number of entries: 9
+Zip file size: 4373 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
 -rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
--rw-rw-r--  2.0 unx     7554 b- defN 23-May-29 10:36 mb/plt/emb_viz.py
+-rw-rw-r--  2.0 unx     7580 b- defN 23-May-29 10:37 mb/plt/emb_viz.py
 -rw-rw-r--  2.0 unx       26 b- defN 23-May-25 00:31 mb/utils/__init__.py
--rw-rw-r--  2.0 unx      226 b- defN 23-May-29 10:37 mb_base-1.0.202305291037.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:37 mb_base-1.0.202305291037.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-29 10:37 mb_base-1.0.202305291037.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 10:37 mb_base-1.0.202305291037.dist-info/RECORD
-9 files, 9041 bytes uncompressed, 3123 bytes compressed:  65.5%
+-rw-rw-r--  2.0 unx      226 b- defN 23-May-29 10:38 mb_base-1.0.202305291038.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:38 mb_base-1.0.202305291038.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-29 10:38 mb_base-1.0.202305291038.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 10:38 mb_base-1.0.202305291038.dist-info/RECORD
+9 files, 9067 bytes uncompressed, 3131 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mb/plt/emb_viz.py
 Comment: 
 
 Filename: mb/utils/__init__.py
 Comment: 
 
-Filename: mb_base-1.0.202305291037.dist-info/METADATA
+Filename: mb_base-1.0.202305291038.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305291037.dist-info/WHEEL
+Filename: mb_base-1.0.202305291038.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305291037.dist-info/top_level.txt
+Filename: mb_base-1.0.202305291038.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305291037.dist-info/RECORD
+Filename: mb_base-1.0.202305291038.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb/plt/emb_viz.py

```diff
@@ -96,14 +96,15 @@
     
     if limit:
         df = df.sample(limit)
     
     assert emb_column in df.columns, 'Embedding column not found in dataframe'
     
     emb_data = np.concatenate(np.array(df[emb_column]))
+    print(emb_data.shape)
     emb_data = emb_data.reshape(-1,2) #change this for 3d
     if logger:
         logger.info('Embedding data shape {}'.format(str(emb_data.shape)))
     
     if target_column:
         target_data = list(df[target_column])
```


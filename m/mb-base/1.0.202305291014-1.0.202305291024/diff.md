# Comparing `tmp/mb_base-1.0.202305291014-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202305291024-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4249 bytes, number of entries: 9
+Zip file size: 4248 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
 -rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
--rw-rw-r--  2.0 unx     7206 b- defN 23-May-29 10:14 mb/plt/emb_viz.py
+-rw-rw-r--  2.0 unx     7210 b- defN 23-May-29 10:23 mb/plt/emb_viz.py
 -rw-rw-r--  2.0 unx       26 b- defN 23-May-25 00:31 mb/utils/__init__.py
--rw-rw-r--  2.0 unx      226 b- defN 23-May-29 10:14 mb_base-1.0.202305291014.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:14 mb_base-1.0.202305291014.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-29 10:14 mb_base-1.0.202305291014.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 10:14 mb_base-1.0.202305291014.dist-info/RECORD
-9 files, 8693 bytes uncompressed, 3007 bytes compressed:  65.4%
+-rw-rw-r--  2.0 unx      226 b- defN 23-May-29 10:24 mb_base-1.0.202305291024.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:24 mb_base-1.0.202305291024.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-29 10:24 mb_base-1.0.202305291024.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 10:24 mb_base-1.0.202305291024.dist-info/RECORD
+9 files, 8697 bytes uncompressed, 3006 bytes compressed:  65.4%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mb/plt/emb_viz.py
 Comment: 
 
 Filename: mb/utils/__init__.py
 Comment: 
 
-Filename: mb_base-1.0.202305291014.dist-info/METADATA
+Filename: mb_base-1.0.202305291024.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305291014.dist-info/WHEEL
+Filename: mb_base-1.0.202305291024.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305291014.dist-info/top_level.txt
+Filename: mb_base-1.0.202305291024.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305291014.dist-info/RECORD
+Filename: mb_base-1.0.202305291024.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb/plt/emb_viz.py

```diff
@@ -88,15 +88,15 @@
         None
     """
     
     if type(df) != pd.DataFrame:
         if logger:
             logger.info('Type of df :{}'.format(str(type(df))))
         df = pd.load_any_df(df)
-    emb_data = list(df[emb_column])
+    emb_data = np.array(df[emb_column])
     
     assert emb_column in df.columns, 'Embedding column not found in dataframe'
     
     if target_column:
         target_data = list(df[target_column])
         
     assert target_column==None or target_column in df.columns, 'Target column not found in dataframe'
```

## Comparing `mb_base-1.0.202305291014.dist-info/RECORD` & `mb_base-1.0.202305291024.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mb/numpy/__init__.py,sha256=paJ-HHrMmhCCBXA9GVOGoWUjB82J4sJ6bczyaL0xY2E,323
 mb/pandas/__init__.py,sha256=iiTr58Dv_spuo__mao6bJcooroxw3qW0nwZGA8RqPUo,49
 mb/plt/__init__.py,sha256=Ya4j8QIe5BCbMesMr1W8L9LP-FBy9LZbUow0XatJczA,54
-mb/plt/emb_viz.py,sha256=goG6q4NYwNgo6q_hDZkaTPK6M70JpfM83lt0AIZuqQo,7206
+mb/plt/emb_viz.py,sha256=lLfahr2b1qlRvPf7GricFsauAn_-AkMSZwIs4lI-M4s,7210
 mb/utils/__init__.py,sha256=d-IZbbU-gBC7zOXgiH5SqYVSP6XNaQ8da5153sNLSaY,26
-mb_base-1.0.202305291014.dist-info/METADATA,sha256=yT4pjgBzNRoT1KKEShXoWVKdiiOKsWV8U_LtnwjyKms,226
-mb_base-1.0.202305291014.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_base-1.0.202305291014.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
-mb_base-1.0.202305291014.dist-info/RECORD,,
+mb_base-1.0.202305291024.dist-info/METADATA,sha256=PuV2OCnzu0BSTZ1Zw4oc5mPbw2IQ7Xo-IxulPvy-ugc,226
+mb_base-1.0.202305291024.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_base-1.0.202305291024.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
+mb_base-1.0.202305291024.dist-info/RECORD,,
```


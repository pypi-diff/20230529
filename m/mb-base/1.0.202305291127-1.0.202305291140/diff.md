# Comparing `tmp/mb_base-1.0.202305291127-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202305291140-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4936 bytes, number of entries: 10
+Zip file size: 4976 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
 -rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
--rw-rw-r--  2.0 unx     7970 b- defN 23-May-29 11:02 mb/plt/emb_viz.py
+-rw-rw-r--  2.0 unx     8085 b- defN 23-May-29 11:40 mb/plt/emb_viz.py
 -rw-rw-r--  2.0 unx       65 b- defN 23-May-29 11:27 mb/utils/__init__.py
 -rw-rw-r--  2.0 unx      739 b- defN 23-May-29 11:18 mb/utils/pip_update.py
--rw-rw-r--  2.0 unx      291 b- defN 23-May-29 11:27 mb_base-1.0.202305291127.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 11:27 mb_base-1.0.202305291127.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-29 11:27 mb_base-1.0.202305291127.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      792 b- defN 23-May-29 11:27 mb_base-1.0.202305291127.dist-info/RECORD
-10 files, 10378 bytes uncompressed, 3574 bytes compressed:  65.6%
+-rw-rw-r--  2.0 unx      291 b- defN 23-May-29 11:40 mb_base-1.0.202305291140.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 11:40 mb_base-1.0.202305291140.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-29 11:40 mb_base-1.0.202305291140.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      792 b- defN 23-May-29 11:40 mb_base-1.0.202305291140.dist-info/RECORD
+10 files, 10493 bytes uncompressed, 3614 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: mb/utils/__init__.py
 Comment: 
 
 Filename: mb/utils/pip_update.py
 Comment: 
 
-Filename: mb_base-1.0.202305291127.dist-info/METADATA
+Filename: mb_base-1.0.202305291140.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305291127.dist-info/WHEEL
+Filename: mb_base-1.0.202305291140.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305291127.dist-info/top_level.txt
+Filename: mb_base-1.0.202305291140.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305291127.dist-info/RECORD
+Filename: mb_base-1.0.202305291140.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb/plt/emb_viz.py

```diff
@@ -46,15 +46,17 @@
         pca_emb = pca.fit_transform(list(df[emb]))
         if logger:
             logger.info('First PCA transform result : {}'.format(str(pca_emb[0])))
         temp_res = list(pca_emb)
     
     if emb_type=='tsne':
         tsne = TSNE(n_components=dim, verbose=1, perplexity=35, n_iter=250, **kwargs)
-        tsne_emb = tsne.fit_transform(list(df[emb]))
+        if type(df[emb].iloc[0]) is not np.ndarray:
+            df[emb] = df[emb].apply(lambda x: np.array(x))
+        tsne_emb = tsne.fit_transform(np.array(df[emb]))
         if logger:
             logger.info('First TSNE transform result : {}'.format(str(tsne_emb[0])))
         temp_res = list(tsne_emb)
     
     if emb_type=='umap':
         umap_emb = umap.UMAP(n_neighbors=dim, min_dist=0.3, metric='correlation',**kwargs).fit_transform(list(df[emb]))
         if logger:
```

## Comparing `mb_base-1.0.202305291127.dist-info/RECORD` & `mb_base-1.0.202305291140.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 mb/numpy/__init__.py,sha256=paJ-HHrMmhCCBXA9GVOGoWUjB82J4sJ6bczyaL0xY2E,323
 mb/pandas/__init__.py,sha256=iiTr58Dv_spuo__mao6bJcooroxw3qW0nwZGA8RqPUo,49
 mb/plt/__init__.py,sha256=Ya4j8QIe5BCbMesMr1W8L9LP-FBy9LZbUow0XatJczA,54
-mb/plt/emb_viz.py,sha256=W24rQmcMZs6ThWIcTOhy_qrcKqyT0Fl0cvi9yEcddbU,7970
+mb/plt/emb_viz.py,sha256=yElVtXWmjYfbrcZyURGKp0rqW48Zigx3pQIA8opDDpY,8085
 mb/utils/__init__.py,sha256=A9wwxJCd4Pezd_tO0opRpggIOxZayl84dBE14FXmiFk,65
 mb/utils/pip_update.py,sha256=XoQg7t9Jq9EnBGeQp0DA1rreP745fL0yJTki8h9teMQ,739
-mb_base-1.0.202305291127.dist-info/METADATA,sha256=UqBwK47Rhc8oOaI4bbSqRLagBltf6A8VmLmvR46j7xY,291
-mb_base-1.0.202305291127.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_base-1.0.202305291127.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
-mb_base-1.0.202305291127.dist-info/RECORD,,
+mb_base-1.0.202305291140.dist-info/METADATA,sha256=jcM6BNaGy0dSHCJT9gML69pnDjSWrnsiXWAptVBbFYk,291
+mb_base-1.0.202305291140.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_base-1.0.202305291140.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
+mb_base-1.0.202305291140.dist-info/RECORD,,
```


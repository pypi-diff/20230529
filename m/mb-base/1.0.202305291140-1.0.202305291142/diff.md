# Comparing `tmp/mb_base-1.0.202305291140-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202305291142-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4976 bytes, number of entries: 10
+Zip file size: 4963 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
 -rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
--rw-rw-r--  2.0 unx     8085 b- defN 23-May-29 11:40 mb/plt/emb_viz.py
+-rw-rw-r--  2.0 unx     8029 b- defN 23-May-29 11:42 mb/plt/emb_viz.py
 -rw-rw-r--  2.0 unx       65 b- defN 23-May-29 11:27 mb/utils/__init__.py
 -rw-rw-r--  2.0 unx      739 b- defN 23-May-29 11:18 mb/utils/pip_update.py
--rw-rw-r--  2.0 unx      291 b- defN 23-May-29 11:40 mb_base-1.0.202305291140.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 11:40 mb_base-1.0.202305291140.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-29 11:40 mb_base-1.0.202305291140.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      792 b- defN 23-May-29 11:40 mb_base-1.0.202305291140.dist-info/RECORD
-10 files, 10493 bytes uncompressed, 3614 bytes compressed:  65.6%
+-rw-rw-r--  2.0 unx      291 b- defN 23-May-29 11:42 mb_base-1.0.202305291142.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 11:42 mb_base-1.0.202305291142.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-29 11:42 mb_base-1.0.202305291142.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      792 b- defN 23-May-29 11:42 mb_base-1.0.202305291142.dist-info/RECORD
+10 files, 10437 bytes uncompressed, 3601 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: mb/utils/__init__.py
 Comment: 
 
 Filename: mb/utils/pip_update.py
 Comment: 
 
-Filename: mb_base-1.0.202305291140.dist-info/METADATA
+Filename: mb_base-1.0.202305291142.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305291140.dist-info/WHEEL
+Filename: mb_base-1.0.202305291142.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305291140.dist-info/top_level.txt
+Filename: mb_base-1.0.202305291142.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305291140.dist-info/RECORD
+Filename: mb_base-1.0.202305291142.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb/plt/emb_viz.py

```diff
@@ -46,16 +46,15 @@
         pca_emb = pca.fit_transform(list(df[emb]))
         if logger:
             logger.info('First PCA transform result : {}'.format(str(pca_emb[0])))
         temp_res = list(pca_emb)
     
     if emb_type=='tsne':
         tsne = TSNE(n_components=dim, verbose=1, perplexity=35, n_iter=250, **kwargs)
-        if type(df[emb].iloc[0]) is not np.ndarray:
-            df[emb] = df[emb].apply(lambda x: np.array(x))
+        df[emb] = df[emb].apply(lambda x: np.array(x))
         tsne_emb = tsne.fit_transform(np.array(df[emb]))
         if logger:
             logger.info('First TSNE transform result : {}'.format(str(tsne_emb[0])))
         temp_res = list(tsne_emb)
     
     if emb_type=='umap':
         umap_emb = umap.UMAP(n_neighbors=dim, min_dist=0.3, metric='correlation',**kwargs).fit_transform(list(df[emb]))
```


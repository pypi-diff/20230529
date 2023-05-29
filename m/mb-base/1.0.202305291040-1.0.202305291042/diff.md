# Comparing `tmp/mb_base-1.0.202305291040-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202305291042-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4371 bytes, number of entries: 9
+Zip file size: 4418 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
 -rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
--rw-rw-r--  2.0 unx     7553 b- defN 23-May-29 10:40 mb/plt/emb_viz.py
+-rw-rw-r--  2.0 unx     7708 b- defN 23-May-29 10:42 mb/plt/emb_viz.py
 -rw-rw-r--  2.0 unx       26 b- defN 23-May-25 00:31 mb/utils/__init__.py
--rw-rw-r--  2.0 unx      226 b- defN 23-May-29 10:40 mb_base-1.0.202305291040.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:40 mb_base-1.0.202305291040.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-29 10:40 mb_base-1.0.202305291040.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 10:40 mb_base-1.0.202305291040.dist-info/RECORD
-9 files, 9040 bytes uncompressed, 3129 bytes compressed:  65.4%
+-rw-rw-r--  2.0 unx      226 b- defN 23-May-29 10:42 mb_base-1.0.202305291042.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:42 mb_base-1.0.202305291042.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-29 10:42 mb_base-1.0.202305291042.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 10:42 mb_base-1.0.202305291042.dist-info/RECORD
+9 files, 9195 bytes uncompressed, 3176 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mb/plt/emb_viz.py
 Comment: 
 
 Filename: mb/utils/__init__.py
 Comment: 
 
-Filename: mb_base-1.0.202305291040.dist-info/METADATA
+Filename: mb_base-1.0.202305291042.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305291040.dist-info/WHEEL
+Filename: mb_base-1.0.202305291042.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305291040.dist-info/top_level.txt
+Filename: mb_base-1.0.202305291042.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305291040.dist-info/RECORD
+Filename: mb_base-1.0.202305291042.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb/plt/emb_viz.py

```diff
@@ -1,12 +1,13 @@
 ## file to view pca / umap / tsne embeddings in 2d or 3d with tf projector and plotly
 
 from mb import pandas as pd
 from sklearn.decomposition import PCA
 from sklearn.manifold import TSNE
+from sklearn.preprocessing import LabelEncoder
 import umap
 from matplotlib import pyplot as plt
 import tensorflow as tf
 import os
 import numpy as np
 
 __all__ = ['get_emb','viz_emb','generate_sprite_images']
@@ -102,14 +103,16 @@
     emb_data = np.concatenate(np.array(df[emb_column]))
     emb_data = emb_data.reshape(-1,2) #change this for 3d
     if logger:
         logger.info('Embedding data shape {}'.format(str(emb_data.shape)))
     
     if target_column:
         target_data = list(df[target_column])
+        if type(target_data[0]) == str:
+            target_data = LabelEncoder().fit_transform(target_data)
         
     assert target_column==None or target_column in df.columns, 'Target column not found in dataframe'
         
     # Visualize the embeddings using a scatter plot
     if viz_type=='plt' and target_column:
         plt.scatter(emb_data[:, 0], emb_data[:, 1], c=target_data, cmap='viridis')
         plt.show()
```


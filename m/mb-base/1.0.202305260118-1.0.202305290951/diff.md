# Comparing `tmp/mb_base-1.0.202305260118-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202305290951-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 3210 bytes, number of entries: 9
+Zip file size: 4227 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
 -rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
--rw-rw-r--  2.0 unx     3343 b- defN 23-May-26 01:17 mb/plt/emb_viz.py
+-rw-rw-r--  2.0 unx     7026 b- defN 23-May-29 09:50 mb/plt/emb_viz.py
 -rw-rw-r--  2.0 unx       26 b- defN 23-May-25 00:31 mb/utils/__init__.py
--rw-rw-r--  2.0 unx      226 b- defN 23-May-26 01:18 mb_base-1.0.202305260118.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-26 01:18 mb_base-1.0.202305260118.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-26 01:18 mb_base-1.0.202305260118.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      714 b- defN 23-May-26 01:18 mb_base-1.0.202305260118.dist-info/RECORD
-9 files, 4830 bytes uncompressed, 1968 bytes compressed:  59.3%
+-rw-rw-r--  2.0 unx      226 b- defN 23-May-29 09:51 mb_base-1.0.202305290951.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 09:51 mb_base-1.0.202305290951.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-29 09:51 mb_base-1.0.202305290951.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 09:51 mb_base-1.0.202305290951.dist-info/RECORD
+9 files, 8513 bytes uncompressed, 2985 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mb/plt/emb_viz.py
 Comment: 
 
 Filename: mb/utils/__init__.py
 Comment: 
 
-Filename: mb_base-1.0.202305260118.dist-info/METADATA
+Filename: mb_base-1.0.202305290951.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305260118.dist-info/WHEEL
+Filename: mb_base-1.0.202305290951.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305260118.dist-info/top_level.txt
+Filename: mb_base-1.0.202305290951.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305260118.dist-info/RECORD
+Filename: mb_base-1.0.202305290951.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb/plt/emb_viz.py

```diff
@@ -1,16 +1,19 @@
 ## file to view pca / umap / tsne embeddings in 2d or 3d with tf projector and plotly
 
 from mb import pandas as pd
 from sklearn.decomposition import PCA
 from sklearn.manifold import TSNE
 import umap
+from matplotlib import pyplot as plt
+import tensorflow as tf
+import os
+import numpy as np
 
-
-__all__ = ['get_emb','viz_emb']
+__all__ = ['get_emb','viz_emb','generate_sprite_images']
 
 
 def get_emb(df: pd.DataFrame, emb= 'embeddings', emb_type='umap', dim=2,keep_original_emb=False,file_save=None, logger=None,**kwargs):
     """
     Visualize embeddings in 2d or 3d with tf projector and plotly
 
     Args:
@@ -63,23 +66,113 @@
     if file_save:
         df.to_csv(file_save,index=False)
     else:
         df.to_csv('./emb_res.csv',index=False)
     
     return df
 
-def viz_emb(df: pd.DataFrame, emb_column='emb_res' , view_dim=2, viz_type ='plt', file_save=None, logger=None):
+def viz_emb(df: pd.DataFrame, emb_column='emb_res' , target_column='taxcode', viz_type ='plt',image_tb=None , file_save=None, logger=None):
     """
     Vizualize embeddings in 2d or 3d with tf projector and plotly
     
     Args:
         df (pd.DataFrame): dataframe containing embeddings. File location or DataFrame object.
         emb_column (str): name of embedding column
-        view_dim (int, optional): embedding dimension: 2 or 3 dim. Defaults to 2.
+        target_column (str): name of target column. It can be used to color the embeddings. Defaults to 'taxcode'. Can be None too.
         viz_type (str, optional): visualization type: 'plt' or 'tf'. Defaults to 'plt'.
+        image_tb (str, optional): image location column to be used in tensorboard projector if want to create with images. Defaults to None.
         file_save (str, optional): file location to save plot. If viz_type='tf', then it wont be saved. Defaults to None.
         logger (logger, optional): logger object. Defaults to None.
     Output:
         None
     """
     
+    if df is not pd.DataFrame:
+        df = pd.load_any_df(df)
+    emb_data = list(df[emb_column])
+    
+    assert emb_column in df.columns, 'Embedding column not found in dataframe'
+    
+    if target_column:
+        target_data = list(df[target_column])
+        
+    assert target_column==None or target_column in df.columns, 'Target column not found in dataframe'
+        
+    # Visualize the embeddings using a scatter plot
+    if viz_type=='plt' and target_column:
+        plt.scatter(emb_data[:, 0], emb_data[:, 1], c=target_data, cmap='Spectral')
+        plt.show()
+        if file_save:
+            plt.savefig(file_save)
+    elif viz_type=='plt' and target_column==None:
+        plt.scatter(emb_data[:, 0], emb_data[:, 1], cmap='Spectral')
+        plt.show()
+        if file_save:
+            plt.savefig(file_save)
+        
+    elif viz_type=='tf' and target_column:
+        
+        emb_data = np.array(emb_data)
+        np.savetxt('emb_res.tsv', emb_data, delimiter='\t')
+        
+        target_data.to_csv('labels.tsv',index=False,header=False,sep='\t')
+        
+        if image_tb is not None:
+            generate_sprite_images(df[image_tb], file_save=None, img_size=28 ,logger=None)
+            SPRITE_PATH = './sprite_image.png'
+        
+        ##check from here
+        log_dir = 'logs'
+        if not os.path.exists(log_dir):
+            os.makedirs(log_dir)
+        
+        from tensorboard.plugins import projector
+        
+        config = tf.summary_v1.ProjectorConfig()
+
+        embedding = config.embeddings.add()
+        embedding.tensor_path = 'emb_res.tsv'
+        embedding.metadata_path = 'labels.tsv'
+        embedding.sprite.image_path = 'sprite_image.png'
+        embedding.sprite.single_image_dim.extend([32, 32])
+
+        with open(os.path.join(log_dir, 'projector_config.pbtxt'), 'w') as f:
+            f.write(str(config))
+        
+        if logger:
+            logger.info('Saved sprite image to {}'.format(SPRITE_PATH))
+            logger.info('Run tensorboard --logdir={} to view embeddings'.format(log_dir))
+            logger.info('if on jupyter notebook, run below code to view embeddings in notebook')
+            logger.info('%load_ext tensorboard')
+            logger.info('%tensorboard --logdir={}'.format(log_dir))
+
+    
+def generate_sprite_images(img_paths, file_save=None, img_size= 28 ,logger=None):
+    """
+    Create a sprite image consisting of images
+
+    Args:
+        img_paths (list or pd.DataFrame): list of image paths
+        file_save (str, optional): file location to save sprite image. Defaults to None. Will save in current directory.
+        img_size (int, optional): image size. Defaults to 28.
+        logger (logger, optional): logger object. Defaults to None.
+    Output:
+        sprite_image (np.array): sprite image
+    """
+    
+    if img_paths is not list:
+        img_paths = list(img_paths)
+    
+    #create sprite image
+    images = [tf.io.read_file(img_path) for img_path in img_paths]
+    images = [tf.image.decode_image(img) for img in images]
+    images = [tf.image.resize(img, (img_size, img_size)) for img in images]
+    images = [img.numpy() for img in images]
+    sprite_image = np.concatenate(images, axis=1)
     
+    if file_save:
+        sprite_image.save(file_save)
+    else:
+        sprite_image.save('./sprite_image.png')
+        
+    return sprite_image
+
```


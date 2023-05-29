# Comparing `tmp/mb_base-1.0.202305291052-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202305291101-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4424 bytes, number of entries: 9
+Zip file size: 4437 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
 -rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
--rw-rw-r--  2.0 unx     7801 b- defN 23-May-29 10:52 mb/plt/emb_viz.py
+-rw-rw-r--  2.0 unx     8045 b- defN 23-May-29 11:01 mb/plt/emb_viz.py
 -rw-rw-r--  2.0 unx       26 b- defN 23-May-25 00:31 mb/utils/__init__.py
--rw-rw-r--  2.0 unx      226 b- defN 23-May-29 10:52 mb_base-1.0.202305291052.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:52 mb_base-1.0.202305291052.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-29 10:52 mb_base-1.0.202305291052.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 10:52 mb_base-1.0.202305291052.dist-info/RECORD
-9 files, 9288 bytes uncompressed, 3182 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx      226 b- defN 23-May-29 11:01 mb_base-1.0.202305291101.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 11:01 mb_base-1.0.202305291101.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-29 11:01 mb_base-1.0.202305291101.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 11:01 mb_base-1.0.202305291101.dist-info/RECORD
+9 files, 9532 bytes uncompressed, 3195 bytes compressed:  66.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mb/plt/emb_viz.py
 Comment: 
 
 Filename: mb/utils/__init__.py
 Comment: 
 
-Filename: mb_base-1.0.202305291052.dist-info/METADATA
+Filename: mb_base-1.0.202305291101.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305291052.dist-info/WHEEL
+Filename: mb_base-1.0.202305291101.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305291052.dist-info/top_level.txt
+Filename: mb_base-1.0.202305291101.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305291052.dist-info/RECORD
+Filename: mb_base-1.0.202305291101.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb/plt/emb_viz.py

```diff
@@ -3,14 +3,15 @@
 from mb import pandas as pd
 from sklearn.decomposition import PCA
 from sklearn.manifold import TSNE
 from sklearn.preprocessing import LabelEncoder
 import umap
 from matplotlib import pyplot as plt
 import tensorflow as tf
+from tensorboard.plugins import projector
 import os
 import numpy as np
 
 __all__ = ['get_emb','viz_emb','generate_sprite_images']
 
 
 def get_emb(df: pd.DataFrame, emb= 'embeddings', emb_type='umap', dim=2,keep_original_emb=False,file_save=None, logger=None,**kwargs):
@@ -126,43 +127,46 @@
         plt.scatter(emb_data[:, 0], emb_data[:, 1])
         plt.show()
         if file_save:
             plt.savefig(file_save)
 
     elif viz_type=='tf' and target_column:
         
+        ##check from here
+        log_dir = 'tp_logs'
+        if not os.path.exists(log_dir):
+            os.makedirs(log_dir)
+            
         emb_data = np.array(emb_data)
-        np.savetxt('emb_data_tf.tsv', emb_data, delimiter='\t')
+        loc_emb_data = os.path.join(log_dir,'emb_data_tf.tsv')
+        np.savetxt(loc_emb_data, emb_data, delimiter='\t')
         
         target_data = np.array(target_data)
-        np.savetxt('labels_tf.tsv',target_data,delimiter='\t')
+        loc_target_data = os.path.join(log_dir,'labels_tf.tsv')
+        np.savetxt(loc_target_data,target_data,delimiter='\t')
         
         if image_tb is not None:
-            generate_sprite_images(df[image_tb], file_save=None, img_size=28 ,logger=None)
-            SPRITE_PATH = './sprite_image.png'
-        
-        ##check from here
-        log_dir = 'logs'
-        if not os.path.exists(log_dir):
-            os.makedirs(log_dir)
+            loc_sprite_image = os.path.join(log_dir,'sprite_image.png')
+            generate_sprite_images(df[image_tb], file_save=loc_sprite_image, img_size=28 ,logger=None)        
         
         from tensorboard.plugins import projector
         
-        config = tf.summary.create_file_writer(log_dir)
+        config = projector.ProjectorConfig()
         embedding = config.embeddings.add()
-        embedding.tensor_path = 'emb_data_tf.tsv'
-        embedding.metadata_path = 'labels_tf.tsv'
-        embedding.sprite.image_path = 'sprite_image.png'
-        embedding.sprite.single_image_dim.extend([32, 32])
+        embedding.tensor_path = loc_emb_data
+        embedding.metadata_path = loc_target_data
+        if image_tb is not None:
+            embedding.sprite.image_path = loc_sprite_image
+            embedding.sprite.single_image_dim.extend([32, 32])
 
         with open(os.path.join(log_dir, 'projector_config.pbtxt'), 'w') as f:
             f.write(str(config))
         
         if logger:
-            logger.info('Saved sprite image to {}'.format(SPRITE_PATH))
+            logger.info('Saved sprite image to {}'.format(loc_sprite_image))
             logger.info('Run tensorboard --logdir={} to view embeddings'.format(log_dir))
             logger.info('if on jupyter notebook, run below code to view embeddings in notebook')
             logger.info('%load_ext tensorboard')
             logger.info('%tensorboard --logdir={}'.format(log_dir))
 
     
 def generate_sprite_images(img_paths, file_save=None, img_size= 28 ,logger=None):
```

## Comparing `mb_base-1.0.202305291052.dist-info/RECORD` & `mb_base-1.0.202305291101.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mb/numpy/__init__.py,sha256=paJ-HHrMmhCCBXA9GVOGoWUjB82J4sJ6bczyaL0xY2E,323
 mb/pandas/__init__.py,sha256=iiTr58Dv_spuo__mao6bJcooroxw3qW0nwZGA8RqPUo,49
 mb/plt/__init__.py,sha256=Ya4j8QIe5BCbMesMr1W8L9LP-FBy9LZbUow0XatJczA,54
-mb/plt/emb_viz.py,sha256=b5aKvln9w3Ky-8QVjO4woqPOZlltc6BpWNLMMPwN-mc,7801
+mb/plt/emb_viz.py,sha256=fx26RUmXigO0RJh9GWzVkqgvR0BuB7CAfiAx9_s4o0M,8045
 mb/utils/__init__.py,sha256=d-IZbbU-gBC7zOXgiH5SqYVSP6XNaQ8da5153sNLSaY,26
-mb_base-1.0.202305291052.dist-info/METADATA,sha256=50YZWeS-AGFgYRJpZEDBCQoGEhCvip-hgE0LnC5spJM,226
-mb_base-1.0.202305291052.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_base-1.0.202305291052.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
-mb_base-1.0.202305291052.dist-info/RECORD,,
+mb_base-1.0.202305291101.dist-info/METADATA,sha256=NWv2_0VDZyVbWLuwzRCYH0LUCA_ESr7_W21Y7Prjaew,226
+mb_base-1.0.202305291101.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_base-1.0.202305291101.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
+mb_base-1.0.202305291101.dist-info/RECORD,,
```


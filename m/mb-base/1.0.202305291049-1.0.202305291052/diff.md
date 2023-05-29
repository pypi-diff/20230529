# Comparing `tmp/mb_base-1.0.202305291049-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202305291052-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4428 bytes, number of entries: 9
+Zip file size: 4424 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
 -rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
--rw-rw-r--  2.0 unx     7795 b- defN 23-May-29 10:49 mb/plt/emb_viz.py
+-rw-rw-r--  2.0 unx     7801 b- defN 23-May-29 10:52 mb/plt/emb_viz.py
 -rw-rw-r--  2.0 unx       26 b- defN 23-May-25 00:31 mb/utils/__init__.py
--rw-rw-r--  2.0 unx      226 b- defN 23-May-29 10:49 mb_base-1.0.202305291049.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:49 mb_base-1.0.202305291049.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-29 10:49 mb_base-1.0.202305291049.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 10:49 mb_base-1.0.202305291049.dist-info/RECORD
-9 files, 9282 bytes uncompressed, 3186 bytes compressed:  65.7%
+-rw-rw-r--  2.0 unx      226 b- defN 23-May-29 10:52 mb_base-1.0.202305291052.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 10:52 mb_base-1.0.202305291052.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-29 10:52 mb_base-1.0.202305291052.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      714 b- defN 23-May-29 10:52 mb_base-1.0.202305291052.dist-info/RECORD
+9 files, 9288 bytes uncompressed, 3182 bytes compressed:  65.7%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: mb/plt/emb_viz.py
 Comment: 
 
 Filename: mb/utils/__init__.py
 Comment: 
 
-Filename: mb_base-1.0.202305291049.dist-info/METADATA
+Filename: mb_base-1.0.202305291052.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305291049.dist-info/WHEEL
+Filename: mb_base-1.0.202305291052.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305291049.dist-info/top_level.txt
+Filename: mb_base-1.0.202305291052.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305291049.dist-info/RECORD
+Filename: mb_base-1.0.202305291052.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb/plt/emb_viz.py

```diff
@@ -143,16 +143,15 @@
         ##check from here
         log_dir = 'logs'
         if not os.path.exists(log_dir):
             os.makedirs(log_dir)
         
         from tensorboard.plugins import projector
         
-        config = tf.summary_v1.ProjectorConfig()
-
+        config = tf.summary.create_file_writer(log_dir)
         embedding = config.embeddings.add()
         embedding.tensor_path = 'emb_data_tf.tsv'
         embedding.metadata_path = 'labels_tf.tsv'
         embedding.sprite.image_path = 'sprite_image.png'
         embedding.sprite.single_image_dim.extend([32, 32])
 
         with open(os.path.join(log_dir, 'projector_config.pbtxt'), 'w') as f:
```

## Comparing `mb_base-1.0.202305291049.dist-info/RECORD` & `mb_base-1.0.202305291052.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 mb/numpy/__init__.py,sha256=paJ-HHrMmhCCBXA9GVOGoWUjB82J4sJ6bczyaL0xY2E,323
 mb/pandas/__init__.py,sha256=iiTr58Dv_spuo__mao6bJcooroxw3qW0nwZGA8RqPUo,49
 mb/plt/__init__.py,sha256=Ya4j8QIe5BCbMesMr1W8L9LP-FBy9LZbUow0XatJczA,54
-mb/plt/emb_viz.py,sha256=E3cEVwf4ZsOsSdInuxGk28RDr6vzGK8FgBPr9gKuUgA,7795
+mb/plt/emb_viz.py,sha256=b5aKvln9w3Ky-8QVjO4woqPOZlltc6BpWNLMMPwN-mc,7801
 mb/utils/__init__.py,sha256=d-IZbbU-gBC7zOXgiH5SqYVSP6XNaQ8da5153sNLSaY,26
-mb_base-1.0.202305291049.dist-info/METADATA,sha256=GXQkwF-E5ZjHqre3cCgCPd7m9baxqp6Vg_oaf6I-M8E,226
-mb_base-1.0.202305291049.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_base-1.0.202305291049.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
-mb_base-1.0.202305291049.dist-info/RECORD,,
+mb_base-1.0.202305291052.dist-info/METADATA,sha256=50YZWeS-AGFgYRJpZEDBCQoGEhCvip-hgE0LnC5spJM,226
+mb_base-1.0.202305291052.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_base-1.0.202305291052.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
+mb_base-1.0.202305291052.dist-info/RECORD,,
```


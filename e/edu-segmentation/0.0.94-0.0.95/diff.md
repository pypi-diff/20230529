# Comparing `tmp/edu_segmentation-0.0.94-py3-none-any.whl.zip` & `tmp/edu_segmentation-0.0.95-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 50859 bytes, number of entries: 27
+Zip file size: 50860 bytes, number of entries: 27
 -rw-rw-rw-  2.0 fat     1885 b- defN 23-May-29 09:01 edu_segmentation/main.py
 -rw-rw-rw-  2.0 fat      325 b- defN 23-Apr-27 10:53 edu_segmentation/BARTTokenClassification/bart_tokenizer.py
 -rw-rw-rw-  2.0 fat      298 b- defN 23-Apr-27 10:53 edu_segmentation/BARTTokenClassification/config.py
 -rw-rw-rw-  2.0 fat     3930 b- defN 23-Apr-28 12:33 edu_segmentation/BARTTokenClassification/import_data_bart.py
 -rw-rw-rw-  2.0 fat    12186 b- defN 23-Apr-27 10:53 edu_segmentation/BARTTokenClassification/model.py
 -rw-rw-rw-  2.0 fat     4364 b- defN 23-Apr-28 16:04 edu_segmentation/BARTTokenClassification/run_segbot.py
 -rw-rw-rw-  2.0 fat     7480 b- defN 23-May-26 09:43 edu_segmentation/BARTTokenClassification/run_segbot_bart.py
@@ -18,12 +18,12 @@
 -rw-rw-rw-  2.0 fat    85404 b- defN 23-Apr-27 10:53 edu_segmentation/BERTTokenClassification/python38bert_modelling.py
 -rw-rw-rw-  2.0 fat     6168 b- defN 23-May-26 11:39 edu_segmentation/BERTTokenClassification/run_bert.py
 -rw-rw-rw-  2.0 fat     6410 b- defN 23-May-26 08:19 edu_segmentation/BERTTokenClassification/solver.py
 -rw-rw-rw-  2.0 fat     6979 b- defN 23-May-26 08:19 edu_segmentation/BERTTokenClassification/solver_postag.py
 -rw-rw-rw-  2.0 fat      537 b- defN 23-Apr-27 10:53 edu_segmentation/BERTTokenClassification/test_model.py
 -rw-rw-rw-  2.0 fat     1025 b- defN 23-May-26 08:20 edu_segmentation/BERTTokenClassification/train_model.py
 -rw-rw-rw-  2.0 fat     1315 b- defN 23-May-26 08:20 edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-rw-rw-  2.0 fat     2731 b- defN 23-May-29 10:23 edu_segmentation-0.0.94.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 10:23 edu_segmentation-0.0.94.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-29 10:23 edu_segmentation-0.0.94.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2949 b- defN 23-May-29 10:23 edu_segmentation-0.0.94.dist-info/RECORD
-27 files, 192683 bytes uncompressed, 45849 bytes compressed:  76.2%
+-rw-rw-rw-  2.0 fat     2731 b- defN 23-May-29 10:26 edu_segmentation-0.0.95.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 10:26 edu_segmentation-0.0.95.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-29 10:26 edu_segmentation-0.0.95.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2949 b- defN 23-May-29 10:26 edu_segmentation-0.0.95.dist-info/RECORD
+27 files, 192683 bytes uncompressed, 45850 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -63,20 +63,20 @@
 
 Filename: edu_segmentation/BERTTokenClassification/train_model.py
 Comment: 
 
 Filename: edu_segmentation/BERTTokenClassification/train_model_postag.py
 Comment: 
 
-Filename: edu_segmentation-0.0.94.dist-info/METADATA
+Filename: edu_segmentation-0.0.95.dist-info/METADATA
 Comment: 
 
-Filename: edu_segmentation-0.0.94.dist-info/WHEEL
+Filename: edu_segmentation-0.0.95.dist-info/WHEEL
 Comment: 
 
-Filename: edu_segmentation-0.0.94.dist-info/top_level.txt
+Filename: edu_segmentation-0.0.95.dist-info/top_level.txt
 Comment: 
 
-Filename: edu_segmentation-0.0.94.dist-info/RECORD
+Filename: edu_segmentation-0.0.95.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `edu_segmentation-0.0.94.dist-info/METADATA` & `edu_segmentation-0.0.95.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-segmentation
-Version: 0.0.94
+Version: 0.0.95
 Summary: To improve EDU segmentation performance using Segbot.
 Author: Your Name
 Author-email: you@example.com
 Requires-Dist: attrs (==23.1.0)
 Requires-Dist: bleach (==6.0.0)
 Requires-Dist: build (==0.10.0)
 Requires-Dist: CacheControl (==0.12.11)
```

## Comparing `edu_segmentation-0.0.94.dist-info/RECORD` & `edu_segmentation-0.0.95.dist-info/RECORD`

 * *Files 3% similar despite different names*

```diff
@@ -17,11 +17,11 @@
 edu_segmentation/BERTTokenClassification/python38bert_modelling.py,sha256=SdLYgE-Lb_jMfw4JeXFTCUqGLNCwFqsMePV6hug1ysU,85404
 edu_segmentation/BERTTokenClassification/run_bert.py,sha256=8fmBmxhrlwjf-bCkXdWst-UxJ_EwB15pK-VxsPXV0g4,6168
 edu_segmentation/BERTTokenClassification/solver.py,sha256=6VaR-uZoMNiOZh8hn9O9N0Dm9G8y0WOTrSOXjhX5g1I,6410
 edu_segmentation/BERTTokenClassification/solver_postag.py,sha256=R4tWfTUOhQXEnC38DXMFH_7jlqfXN65aymzqIUaQOqo,6979
 edu_segmentation/BERTTokenClassification/test_model.py,sha256=v5BbEMOWNbgAzQEQ2t-mKpLUE1lJ1mIDnZIBK27mxSE,537
 edu_segmentation/BERTTokenClassification/train_model.py,sha256=WpZnhOR-Zbo36wrkkctH8jczjZYTTSK75OaFGKDhyng,1025
 edu_segmentation/BERTTokenClassification/train_model_postag.py,sha256=MR_IPjwTucaPowlRH1M5qxyyfy2gisC4r7XKBUKbbag,1315
-edu_segmentation-0.0.94.dist-info/METADATA,sha256=gz4yccKcGWaON0TnYkVZDIzYXTf0q9vPa4wt_OnSC2c,2731
-edu_segmentation-0.0.94.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-edu_segmentation-0.0.94.dist-info/top_level.txt,sha256=Vg0ac0J5_9PTULod_LmMlCd9EquU-WBCknL1C_EczfI,17
-edu_segmentation-0.0.94.dist-info/RECORD,,
+edu_segmentation-0.0.95.dist-info/METADATA,sha256=CZj29AQoZzF-Hyv-Bg4yw0AAqDuY2zDQPo9_vWTV2Yw,2731
+edu_segmentation-0.0.95.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+edu_segmentation-0.0.95.dist-info/top_level.txt,sha256=Vg0ac0J5_9PTULod_LmMlCd9EquU-WBCknL1C_EczfI,17
+edu_segmentation-0.0.95.dist-info/RECORD,,
```


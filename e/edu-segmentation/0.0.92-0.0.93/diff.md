# Comparing `tmp/edu_segmentation-0.0.92-py3-none-any.whl.zip` & `tmp/edu_segmentation-0.0.93-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 50865 bytes, number of entries: 27
--rw-rw-rw-  2.0 fat     1883 b- defN 23-May-29 08:58 edu_segmentation/main.py
+Zip file size: 50861 bytes, number of entries: 27
+-rw-rw-rw-  2.0 fat     1885 b- defN 23-May-29 09:01 edu_segmentation/main.py
 -rw-rw-rw-  2.0 fat      325 b- defN 23-Apr-27 10:53 edu_segmentation/BARTTokenClassification/bart_tokenizer.py
 -rw-rw-rw-  2.0 fat      298 b- defN 23-Apr-27 10:53 edu_segmentation/BARTTokenClassification/config.py
 -rw-rw-rw-  2.0 fat     3930 b- defN 23-Apr-28 12:33 edu_segmentation/BARTTokenClassification/import_data_bart.py
 -rw-rw-rw-  2.0 fat    12186 b- defN 23-Apr-27 10:53 edu_segmentation/BARTTokenClassification/model.py
 -rw-rw-rw-  2.0 fat     4364 b- defN 23-Apr-28 16:04 edu_segmentation/BARTTokenClassification/run_segbot.py
 -rw-rw-rw-  2.0 fat     7480 b- defN 23-May-26 09:43 edu_segmentation/BARTTokenClassification/run_segbot_bart.py
 -rw-rw-rw-  2.0 fat     8974 b- defN 23-Apr-27 10:53 edu_segmentation/BARTTokenClassification/solver.py
@@ -18,12 +18,12 @@
 -rw-rw-rw-  2.0 fat    85404 b- defN 23-Apr-27 10:53 edu_segmentation/BERTTokenClassification/python38bert_modelling.py
 -rw-rw-rw-  2.0 fat     6168 b- defN 23-May-26 11:39 edu_segmentation/BERTTokenClassification/run_bert.py
 -rw-rw-rw-  2.0 fat     6410 b- defN 23-May-26 08:19 edu_segmentation/BERTTokenClassification/solver.py
 -rw-rw-rw-  2.0 fat     6979 b- defN 23-May-26 08:19 edu_segmentation/BERTTokenClassification/solver_postag.py
 -rw-rw-rw-  2.0 fat      537 b- defN 23-Apr-27 10:53 edu_segmentation/BERTTokenClassification/test_model.py
 -rw-rw-rw-  2.0 fat     1025 b- defN 23-May-26 08:20 edu_segmentation/BERTTokenClassification/train_model.py
 -rw-rw-rw-  2.0 fat     1315 b- defN 23-May-26 08:20 edu_segmentation/BERTTokenClassification/train_model_postag.py
--rw-rw-rw-  2.0 fat     2731 b- defN 23-May-29 08:59 edu_segmentation-0.0.92.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 08:59 edu_segmentation-0.0.92.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-29 08:59 edu_segmentation-0.0.92.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     2949 b- defN 23-May-29 08:59 edu_segmentation-0.0.92.dist-info/RECORD
-27 files, 192681 bytes uncompressed, 45855 bytes compressed:  76.2%
+-rw-rw-rw-  2.0 fat     2731 b- defN 23-May-29 09:02 edu_segmentation-0.0.93.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 09:02 edu_segmentation-0.0.93.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-29 09:02 edu_segmentation-0.0.93.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat     2949 b- defN 23-May-29 09:02 edu_segmentation-0.0.93.dist-info/RECORD
+27 files, 192683 bytes uncompressed, 45851 bytes compressed:  76.2%
```

## zipnote {}

```diff
@@ -63,20 +63,20 @@
 
 Filename: edu_segmentation/BERTTokenClassification/train_model.py
 Comment: 
 
 Filename: edu_segmentation/BERTTokenClassification/train_model_postag.py
 Comment: 
 
-Filename: edu_segmentation-0.0.92.dist-info/METADATA
+Filename: edu_segmentation-0.0.93.dist-info/METADATA
 Comment: 
 
-Filename: edu_segmentation-0.0.92.dist-info/WHEEL
+Filename: edu_segmentation-0.0.93.dist-info/WHEEL
 Comment: 
 
-Filename: edu_segmentation-0.0.92.dist-info/top_level.txt
+Filename: edu_segmentation-0.0.93.dist-info/top_level.txt
 Comment: 
 
-Filename: edu_segmentation-0.0.92.dist-info/RECORD
+Filename: edu_segmentation-0.0.93.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## edu_segmentation/main.py

```diff
@@ -12,19 +12,19 @@
     elif model == "bert_cased":
         segbot_model = run_segbot_bert_cased
 
     output = segbot_model(sent)
     results = []
     if granularity_level == "conjunction_words":
         for segment in output:
-            segment = segment.strip()
             index_str = segment[0].split(",")
             index_begin = index_str[0]            
             index_end = index_str[1]            
             word_str = segment[1]
+            word_str = word_str.strip()
             if word_str.startswith(tuple(conjunctions)):
                 splitted = word_str.split()
                 first_word = splitted[0]
                 remaining_words = " ".join(splitted[1:])
                 results.append([f'{index_begin}, {int(index_begin)+1}', first_word])
                 results.append([f'{int(index_begin)+2}, {index_end}', remaining_words])
             elif word_str.endswith(tuple(conjunctions)):
```

## Comparing `edu_segmentation-0.0.92.dist-info/METADATA` & `edu_segmentation-0.0.93.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edu-segmentation
-Version: 0.0.92
+Version: 0.0.93
 Summary: To improve EDU segmentation performance using Segbot.
 Author: Your Name
 Author-email: you@example.com
 Requires-Dist: attrs (==23.1.0)
 Requires-Dist: bleach (==6.0.0)
 Requires-Dist: build (==0.10.0)
 Requires-Dist: CacheControl (==0.12.11)
```

## Comparing `edu_segmentation-0.0.92.dist-info/RECORD` & `edu_segmentation-0.0.93.dist-info/RECORD`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-edu_segmentation/main.py,sha256=7l62fu0S6tXg88iiEgro_OU2-528JFiGSWqelaMTH-g,1883
+edu_segmentation/main.py,sha256=TaaG0G-gN1FwfzhlZuiU8xU5zueFR5imisge6OjyYYA,1885
 edu_segmentation/BARTTokenClassification/bart_tokenizer.py,sha256=UN45Y8kMUwmZk08HVti5B4u7TfPFibXlMpBfSmEz8fc,325
 edu_segmentation/BARTTokenClassification/config.py,sha256=t1GU5pSucv3rZ_shyBKoQ6MkSSLLIwlKnDj6AZFLLqs,298
 edu_segmentation/BARTTokenClassification/import_data_bart.py,sha256=n5QbY0LxtU_qIagbdWVL05KHlsG-f0T7oSDCi5VH2eU,3930
 edu_segmentation/BARTTokenClassification/model.py,sha256=I_LJ3XMKlji_q6PP5sXPcJq6-ESQ5VN4SVjyFOl4qvU,12186
 edu_segmentation/BARTTokenClassification/run_segbot.py,sha256=T4OGoffbsjNMhOMLvemijC2GULpo_U_X3uhcUa8zZpc,4364
 edu_segmentation/BARTTokenClassification/run_segbot_bart.py,sha256=QeJo-9M69LCcaiuLs54w_lR9zt2yt-bMRYYnkJPyDMA,7480
 edu_segmentation/BARTTokenClassification/solver.py,sha256=kPn_GytbW7f342NaDktpSPga78pU7DXN0jrrX0akvj4,8974
@@ -17,11 +17,11 @@
 edu_segmentation/BERTTokenClassification/python38bert_modelling.py,sha256=SdLYgE-Lb_jMfw4JeXFTCUqGLNCwFqsMePV6hug1ysU,85404
 edu_segmentation/BERTTokenClassification/run_bert.py,sha256=8fmBmxhrlwjf-bCkXdWst-UxJ_EwB15pK-VxsPXV0g4,6168
 edu_segmentation/BERTTokenClassification/solver.py,sha256=6VaR-uZoMNiOZh8hn9O9N0Dm9G8y0WOTrSOXjhX5g1I,6410
 edu_segmentation/BERTTokenClassification/solver_postag.py,sha256=R4tWfTUOhQXEnC38DXMFH_7jlqfXN65aymzqIUaQOqo,6979
 edu_segmentation/BERTTokenClassification/test_model.py,sha256=v5BbEMOWNbgAzQEQ2t-mKpLUE1lJ1mIDnZIBK27mxSE,537
 edu_segmentation/BERTTokenClassification/train_model.py,sha256=WpZnhOR-Zbo36wrkkctH8jczjZYTTSK75OaFGKDhyng,1025
 edu_segmentation/BERTTokenClassification/train_model_postag.py,sha256=MR_IPjwTucaPowlRH1M5qxyyfy2gisC4r7XKBUKbbag,1315
-edu_segmentation-0.0.92.dist-info/METADATA,sha256=Q9ZafaNDqIlLDTgDzC8zstd2Zcg7H7d8fGv6k7_-jZw,2731
-edu_segmentation-0.0.92.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-edu_segmentation-0.0.92.dist-info/top_level.txt,sha256=Vg0ac0J5_9PTULod_LmMlCd9EquU-WBCknL1C_EczfI,17
-edu_segmentation-0.0.92.dist-info/RECORD,,
+edu_segmentation-0.0.93.dist-info/METADATA,sha256=TgpY5MvdkaPGf1xZx4HIrhIHLKnrPmy4WymmX33kOnQ,2731
+edu_segmentation-0.0.93.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+edu_segmentation-0.0.93.dist-info/top_level.txt,sha256=Vg0ac0J5_9PTULod_LmMlCd9EquU-WBCknL1C_EczfI,17
+edu_segmentation-0.0.93.dist-info/RECORD,,
```


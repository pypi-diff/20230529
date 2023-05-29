# Comparing `tmp/ygModbus-0.0.2-py3-none-any.whl.zip` & `tmp/ygModbus-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 3655 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:11 ygModbus/__init__.py
+Zip file size: 4013 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:25 ygModbus/__init__.py
 -rw-rw-rw-  2.0 fat      278 b- defN 23-May-29 10:31 ygModbus/client.py
 -rw-rw-rw-  2.0 fat     4135 b- defN 23-May-29 11:11 ygModbus/server.py
--rw-rw-rw-  2.0 fat      601 b- defN 23-May-29 11:22 ygModbus-0.0.2.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:22 ygModbus-0.0.2.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-May-29 11:22 ygModbus-0.0.2.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:22 ygModbus-0.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      620 b- defN 23-May-29 11:22 ygModbus-0.0.2.dist-info/RECORD
-8 files, 5804 bytes uncompressed, 2567 bytes compressed:  55.8%
+-rw-rw-rw-  2.0 fat     1420 b- defN 23-May-29 11:26 ygModbus-0.0.3.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:26 ygModbus-0.0.3.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 23-May-29 11:26 ygModbus-0.0.3.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:26 ygModbus-0.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      621 b- defN 23-May-29 11:26 ygModbus-0.0.3.dist-info/RECORD
+8 files, 6624 bytes uncompressed, 2925 bytes compressed:  55.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: ygModbus/client.py
 Comment: 
 
 Filename: ygModbus/server.py
 Comment: 
 
-Filename: ygModbus-0.0.2.dist-info/METADATA
+Filename: ygModbus-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: ygModbus-0.0.2.dist-info/WHEEL
+Filename: ygModbus-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: ygModbus-0.0.2.dist-info/entry_points.txt
+Filename: ygModbus-0.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: ygModbus-0.0.2.dist-info/top_level.txt
+Filename: ygModbus-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: ygModbus-0.0.2.dist-info/RECORD
+Filename: ygModbus-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ygModbus/__init__.py

```diff
@@ -1 +1 @@
-__version__='0.0.2'
+__version__='0.0.3'
```

## Comparing `ygModbus-0.0.2.dist-info/RECORD` & `ygModbus-0.0.3.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-ygModbus/__init__.py,sha256=K3kV_Wytuyk886jujhc3R8PqeJ9BecJMTgVMlDjr5tA,19
+ygModbus/__init__.py,sha256=qlp5d6WrvsWpBMMTlS9u6vXJyf2cioGX8eRd6yXw4pA,19
 ygModbus/client.py,sha256=FVHG-BaiZzMZGYLLmbRispOxZMIFVurak7tiUyGYIiA,278
 ygModbus/server.py,sha256=OvsWvkl8wxc067HjRuKVDZtL5NUsNgtGcWb-eltUFAA,4135
-ygModbus-0.0.2.dist-info/METADATA,sha256=pFfNHBmyUcycn6cAwkHpBBl_TPBrlW9CUN7Ay3o3wzM,601
-ygModbus-0.0.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ygModbus-0.0.2.dist-info/entry_points.txt,sha256=RxlSVK5_r3N1pTsckChFnayhsyaObNe2QMirKYZcCnQ,50
-ygModbus-0.0.2.dist-info/top_level.txt,sha256=lxXp7DPRDnTB5sYaAnhBhgFvZ_6EIkq3NxhZ0liIFTo,9
-ygModbus-0.0.2.dist-info/RECORD,,
+ygModbus-0.0.3.dist-info/METADATA,sha256=BnBoXQrRv9o5o1QDvGovJ4Krqp17tUTm9LrAn6FyZ2c,1420
+ygModbus-0.0.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ygModbus-0.0.3.dist-info/entry_points.txt,sha256=RxlSVK5_r3N1pTsckChFnayhsyaObNe2QMirKYZcCnQ,50
+ygModbus-0.0.3.dist-info/top_level.txt,sha256=lxXp7DPRDnTB5sYaAnhBhgFvZ_6EIkq3NxhZ0liIFTo,9
+ygModbus-0.0.3.dist-info/RECORD,,
```


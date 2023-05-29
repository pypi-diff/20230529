# Comparing `tmp/ygModbus-0.0.8-py3-none-any.whl.zip` & `tmp/ygModbus-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4358 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:51 ygModbus/__init__.py
+Zip file size: 4356 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:53 ygModbus/__init__.py
 -rw-rw-rw-  2.0 fat      278 b- defN 23-May-29 10:31 ygModbus/client.py
--rw-rw-rw-  2.0 fat      369 b- defN 23-May-29 11:44 ygModbus/main.py
+-rw-rw-rw-  2.0 fat      369 b- defN 23-May-29 11:53 ygModbus/main.py
 -rw-rw-rw-  2.0 fat     4149 b- defN 23-May-29 11:44 ygModbus/server.py
--rw-rw-rw-  2.0 fat     1462 b- defN 23-May-29 11:51 ygModbus-0.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:51 ygModbus-0.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       48 b- defN 23-May-29 11:51 ygModbus-0.0.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:51 ygModbus-0.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      693 b- defN 23-May-29 11:51 ygModbus-0.0.8.dist-info/RECORD
-9 files, 7119 bytes uncompressed, 3162 bytes compressed:  55.6%
+-rw-rw-rw-  2.0 fat     1462 b- defN 23-May-29 11:53 ygModbus-0.0.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:53 ygModbus-0.0.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       43 b- defN 23-May-29 11:53 ygModbus-0.0.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:53 ygModbus-0.0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      693 b- defN 23-May-29 11:53 ygModbus-0.0.9.dist-info/RECORD
+9 files, 7114 bytes uncompressed, 3160 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: ygModbus/main.py
 Comment: 
 
 Filename: ygModbus/server.py
 Comment: 
 
-Filename: ygModbus-0.0.8.dist-info/METADATA
+Filename: ygModbus-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: ygModbus-0.0.8.dist-info/WHEEL
+Filename: ygModbus-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: ygModbus-0.0.8.dist-info/entry_points.txt
+Filename: ygModbus-0.0.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: ygModbus-0.0.8.dist-info/top_level.txt
+Filename: ygModbus-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: ygModbus-0.0.8.dist-info/RECORD
+Filename: ygModbus-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ygModbus/__init__.py

```diff
@@ -1 +1 @@
-__version__='0.0.8'
+__version__='0.0.9'
```

## Comparing `ygModbus-0.0.8.dist-info/METADATA` & `ygModbus-0.0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygModbus
-Version: 0.0.8
+Version: 0.0.9
 Summary: simple Modebus client and server test by response of random number
 Home-page: https://github.com/devggu/
 Author: devggu
 Author-email: pshnb123@gmail.com
 Keywords: modebus,pshn123,devggu,TCP,server,client
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `ygModbus-0.0.8.dist-info/RECORD` & `ygModbus-0.0.9.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-ygModbus/__init__.py,sha256=9_jSwg7P5SlFv0Ci2ZSYBcAbygp9XV2C8sryRO8tvko,19
+ygModbus/__init__.py,sha256=yYvgvA37XnvzMxLHz92xR3XDHUW-uAAMI18Q3lIm0r4,19
 ygModbus/client.py,sha256=FVHG-BaiZzMZGYLLmbRispOxZMIFVurak7tiUyGYIiA,278
 ygModbus/main.py,sha256=EztAHuwhuXIuvc__jJcicdjcSSCkRDFJmTKRMcVLYF4,369
 ygModbus/server.py,sha256=6OqQCxIJQoz5CeOM40Gu3GqZblPUxvUJ1TA0UXgoKo0,4149
-ygModbus-0.0.8.dist-info/METADATA,sha256=mS9ibxRthPI6E50PSGfpBVyusPtJZiqKCiZLhuCzzwo,1462
-ygModbus-0.0.8.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ygModbus-0.0.8.dist-info/entry_points.txt,sha256=Dc0NTrhOyLabNxiNsL2YmTrjgwqg6h75l0quzoZn64Q,48
-ygModbus-0.0.8.dist-info/top_level.txt,sha256=lxXp7DPRDnTB5sYaAnhBhgFvZ_6EIkq3NxhZ0liIFTo,9
-ygModbus-0.0.8.dist-info/RECORD,,
+ygModbus-0.0.9.dist-info/METADATA,sha256=m42s8mZUCJwIGjH7t65BRHqh_cX0lIM8pFScx6-ME5o,1462
+ygModbus-0.0.9.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ygModbus-0.0.9.dist-info/entry_points.txt,sha256=w6QbqELaVucwbt4PJekb4qqDf3E2HE7lihS7o4cpLuI,43
+ygModbus-0.0.9.dist-info/top_level.txt,sha256=lxXp7DPRDnTB5sYaAnhBhgFvZ_6EIkq3NxhZ0liIFTo,9
+ygModbus-0.0.9.dist-info/RECORD,,
```


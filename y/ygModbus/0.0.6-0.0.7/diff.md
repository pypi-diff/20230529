# Comparing `tmp/ygModbus-0.0.6-py3-none-any.whl.zip` & `tmp/ygModbus-0.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,11 @@
-Zip file size: 4013 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:41 ygModbus/__init__.py
+Zip file size: 4355 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:44 ygModbus/__init__.py
 -rw-rw-rw-  2.0 fat      278 b- defN 23-May-29 10:31 ygModbus/client.py
--rw-rw-rw-  2.0 fat     4135 b- defN 23-May-29 11:39 ygModbus/server.py
--rw-rw-rw-  2.0 fat     1420 b- defN 23-May-29 11:42 ygModbus-0.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:42 ygModbus-0.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-May-29 11:42 ygModbus-0.0.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:42 ygModbus-0.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      621 b- defN 23-May-29 11:42 ygModbus-0.0.6.dist-info/RECORD
-8 files, 6624 bytes uncompressed, 2925 bytes compressed:  55.8%
+-rw-rw-rw-  2.0 fat      369 b- defN 23-May-29 11:44 ygModbus/main.py
+-rw-rw-rw-  2.0 fat     4149 b- defN 23-May-29 11:44 ygModbus/server.py
+-rw-rw-rw-  2.0 fat     1420 b- defN 23-May-29 11:45 ygModbus-0.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:45 ygModbus-0.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       50 b- defN 23-May-29 11:45 ygModbus-0.0.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:45 ygModbus-0.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      693 b- defN 23-May-29 11:45 ygModbus-0.0.7.dist-info/RECORD
+9 files, 7079 bytes uncompressed, 3159 bytes compressed:  55.4%
```

## zipnote {}

```diff
@@ -1,25 +1,28 @@
 Filename: ygModbus/__init__.py
 Comment: 
 
 Filename: ygModbus/client.py
 Comment: 
 
+Filename: ygModbus/main.py
+Comment: 
+
 Filename: ygModbus/server.py
 Comment: 
 
-Filename: ygModbus-0.0.6.dist-info/METADATA
+Filename: ygModbus-0.0.7.dist-info/METADATA
 Comment: 
 
-Filename: ygModbus-0.0.6.dist-info/WHEEL
+Filename: ygModbus-0.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: ygModbus-0.0.6.dist-info/entry_points.txt
+Filename: ygModbus-0.0.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: ygModbus-0.0.6.dist-info/top_level.txt
+Filename: ygModbus-0.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: ygModbus-0.0.6.dist-info/RECORD
+Filename: ygModbus-0.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ygModbus/__init__.py

```diff
@@ -1 +1 @@
-__version__='0.0.6'
+__version__='0.0.7'
```

## ygModbus/server.py

```diff
@@ -95,19 +95,19 @@
 
 
 # if __name__ == "__main__":
 #     run_server()
 
 # run_server()
 
-if __name__ == "__main__":
-    parser = argparse.ArgumentParser(prog="ygModbus")
-    subparsers = parser.add_subparsers(dest="command")
+# if __name__ == "__main__":
+#     parser = argparse.ArgumentParser(prog="ygModbus")
+#     subparsers = parser.add_subparsers(dest="command")
 
-    runserver_parser = subparsers.add_parser("runserver", help="Run the server")
+#     runserver_parser = subparsers.add_parser("runserver", help="Run the server")
 
-    args = parser.parse_args()
+#     args = parser.parse_args()
 
-    if args.command == "runserver":
-        run_server()
+#     if args.command == "runserver":
+#         run_server()
```

## Comparing `ygModbus-0.0.6.dist-info/METADATA` & `ygModbus-0.0.7.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygModbus
-Version: 0.0.6
+Version: 0.0.7
 Summary: simple Modebus client and server test by response of random number
 Home-page: https://github.com/devggu/
 Author: devggu
 Author-email: pshnb123@gmail.com
 Keywords: modebus,pshn123,devggu,TCP,server,client
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `ygModbus-0.0.6.dist-info/RECORD` & `ygModbus-0.0.7.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-ygModbus/__init__.py,sha256=zzMTjJY407ibU6_ATOPO8KibRVB3tyW9yO0tRYzjTqw,19
+ygModbus/__init__.py,sha256=3Kn8sHWnxjlagph2LmftcF8JLlcMlmQIbU5t_jzgK3w,19
 ygModbus/client.py,sha256=FVHG-BaiZzMZGYLLmbRispOxZMIFVurak7tiUyGYIiA,278
-ygModbus/server.py,sha256=OvsWvkl8wxc067HjRuKVDZtL5NUsNgtGcWb-eltUFAA,4135
-ygModbus-0.0.6.dist-info/METADATA,sha256=W2pPVfb5UWo8W-5PMrraWkWqiCrutB-8jWNI3N1Cpmg,1420
-ygModbus-0.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-ygModbus-0.0.6.dist-info/entry_points.txt,sha256=RxlSVK5_r3N1pTsckChFnayhsyaObNe2QMirKYZcCnQ,50
-ygModbus-0.0.6.dist-info/top_level.txt,sha256=lxXp7DPRDnTB5sYaAnhBhgFvZ_6EIkq3NxhZ0liIFTo,9
-ygModbus-0.0.6.dist-info/RECORD,,
+ygModbus/main.py,sha256=EztAHuwhuXIuvc__jJcicdjcSSCkRDFJmTKRMcVLYF4,369
+ygModbus/server.py,sha256=6OqQCxIJQoz5CeOM40Gu3GqZblPUxvUJ1TA0UXgoKo0,4149
+ygModbus-0.0.7.dist-info/METADATA,sha256=b2Gt7N9m3G_yjoHD-wWNCCXrSiN4Pv1wOv_wkJScChk,1420
+ygModbus-0.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+ygModbus-0.0.7.dist-info/entry_points.txt,sha256=RxlSVK5_r3N1pTsckChFnayhsyaObNe2QMirKYZcCnQ,50
+ygModbus-0.0.7.dist-info/top_level.txt,sha256=lxXp7DPRDnTB5sYaAnhBhgFvZ_6EIkq3NxhZ0liIFTo,9
+ygModbus-0.0.7.dist-info/RECORD,,
```


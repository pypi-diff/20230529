# Comparing `tmp/ygModbus-0.0.3-py3-none-any.whl.zip` & `tmp/ygModbus-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4013 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:25 ygModbus/__init__.py
+Zip file size: 4022 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:32 ygModbus/__init__.py
 -rw-rw-rw-  2.0 fat      278 b- defN 23-May-29 10:31 ygModbus/client.py
--rw-rw-rw-  2.0 fat     4135 b- defN 23-May-29 11:11 ygModbus/server.py
--rw-rw-rw-  2.0 fat     1420 b- defN 23-May-29 11:26 ygModbus-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:26 ygModbus-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-May-29 11:26 ygModbus-0.0.3.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:26 ygModbus-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      621 b- defN 23-May-29 11:26 ygModbus-0.0.3.dist-info/RECORD
-8 files, 6624 bytes uncompressed, 2925 bytes compressed:  55.8%
+-rw-rw-rw-  2.0 fat     4149 b- defN 23-May-29 11:32 ygModbus/server.py
+-rw-rw-rw-  2.0 fat     1420 b- defN 23-May-29 11:33 ygModbus-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:33 ygModbus-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       60 b- defN 23-May-29 11:33 ygModbus-0.0.4.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:33 ygModbus-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      621 b- defN 23-May-29 11:33 ygModbus-0.0.4.dist-info/RECORD
+8 files, 6648 bytes uncompressed, 2934 bytes compressed:  55.9%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: ygModbus/client.py
 Comment: 
 
 Filename: ygModbus/server.py
 Comment: 
 
-Filename: ygModbus-0.0.3.dist-info/METADATA
+Filename: ygModbus-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: ygModbus-0.0.3.dist-info/WHEEL
+Filename: ygModbus-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: ygModbus-0.0.3.dist-info/entry_points.txt
+Filename: ygModbus-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ygModbus-0.0.3.dist-info/top_level.txt
+Filename: ygModbus-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ygModbus-0.0.3.dist-info/RECORD
+Filename: ygModbus-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ygModbus/__init__.py

```diff
@@ -1 +1 @@
-__version__='0.0.3'
+__version__='0.0.4'
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

## Comparing `ygModbus-0.0.3.dist-info/METADATA` & `ygModbus-0.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygModbus
-Version: 0.0.3
+Version: 0.0.4
 Summary: simple Modebus client and server test by response of random number
 Home-page: https://github.com/devggu/
 Author: devggu
 Author-email: pshnb123@gmail.com
 Keywords: modebus,pshn123,devggu,TCP,server,client
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```


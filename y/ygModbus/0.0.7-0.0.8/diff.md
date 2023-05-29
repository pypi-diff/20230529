# Comparing `tmp/ygModbus-0.0.7-py3-none-any.whl.zip` & `tmp/ygModbus-0.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 4355 bytes, number of entries: 9
--rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:44 ygModbus/__init__.py
+Zip file size: 4358 bytes, number of entries: 9
+-rw-rw-rw-  2.0 fat       19 b- defN 23-May-29 11:51 ygModbus/__init__.py
 -rw-rw-rw-  2.0 fat      278 b- defN 23-May-29 10:31 ygModbus/client.py
 -rw-rw-rw-  2.0 fat      369 b- defN 23-May-29 11:44 ygModbus/main.py
 -rw-rw-rw-  2.0 fat     4149 b- defN 23-May-29 11:44 ygModbus/server.py
--rw-rw-rw-  2.0 fat     1420 b- defN 23-May-29 11:45 ygModbus-0.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:45 ygModbus-0.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       50 b- defN 23-May-29 11:45 ygModbus-0.0.7.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:45 ygModbus-0.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      693 b- defN 23-May-29 11:45 ygModbus-0.0.7.dist-info/RECORD
-9 files, 7079 bytes uncompressed, 3159 bytes compressed:  55.4%
+-rw-rw-rw-  2.0 fat     1462 b- defN 23-May-29 11:51 ygModbus-0.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 11:51 ygModbus-0.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       48 b- defN 23-May-29 11:51 ygModbus-0.0.8.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        9 b- defN 23-May-29 11:51 ygModbus-0.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      693 b- defN 23-May-29 11:51 ygModbus-0.0.8.dist-info/RECORD
+9 files, 7119 bytes uncompressed, 3162 bytes compressed:  55.6%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: ygModbus/main.py
 Comment: 
 
 Filename: ygModbus/server.py
 Comment: 
 
-Filename: ygModbus-0.0.7.dist-info/METADATA
+Filename: ygModbus-0.0.8.dist-info/METADATA
 Comment: 
 
-Filename: ygModbus-0.0.7.dist-info/WHEEL
+Filename: ygModbus-0.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: ygModbus-0.0.7.dist-info/entry_points.txt
+Filename: ygModbus-0.0.8.dist-info/entry_points.txt
 Comment: 
 
-Filename: ygModbus-0.0.7.dist-info/top_level.txt
+Filename: ygModbus-0.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: ygModbus-0.0.7.dist-info/RECORD
+Filename: ygModbus-0.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ygModbus/__init__.py

```diff
@@ -1 +1 @@
-__version__='0.0.7'
+__version__='0.0.8'
```

## Comparing `ygModbus-0.0.7.dist-info/METADATA` & `ygModbus-0.0.8.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ygModbus
-Version: 0.0.7
+Version: 0.0.8
 Summary: simple Modebus client and server test by response of random number
 Home-page: https://github.com/devggu/
 Author: devggu
 Author-email: pshnb123@gmail.com
 Keywords: modebus,pshn123,devggu,TCP,server,client
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -18,22 +18,23 @@
 Requires-Dist: numpy
 
 # Modbus TCP simulator
 
 -set config in register_params.json
 
 ex)
-{
-    "40001":{"max_int":300, "min_int":100, "address":40001},
-    "40002":{"max_int":300, "min_int":20, "address":40002},
-    "40004":{"max_int":300, "min_int":20, "address":40004}
+<br>
+{<br>
+    "40001":{"max_int":300, "min_int":100, "address":40001},<br>
+    "40002":{"max_int":300, "min_int":20, "address":40002},<br>
+    "40004":{"max_int":300, "min_int":20, "address":40004}<br>
 }
 
 start simulating server by 'ygModBus runserver'
 
 ctrl+c for terminate server
 
-args:
-    ('-H', '--host', type=str, default='127.0.0.1', help='Host (default: 127.0.0.1)')
-    ('-p', '--port', type=int, default=502, help='TCP port (default: 502)')
-    ('-j', '--json', type=str, default='register_params.json', help='JSON file with register parameters (default: register_params.json)')
-    ('-i', '--interval', type=float, default=1.0, help='Interval in seconds for updating holding registers (default: 1.0)')
+args:<br>
+    ('-H', '--host', type=str, default='127.0.0.1', help='Host (default: 127.0.0.1)')<br>
+    ('-p', '--port', type=int, default=502, help='TCP port (default: 502)')<br>
+    ('-j', '--json', type=str, default='register_params.json', help='JSON file with register parameters (default: register_params.json)')<br>
+    ('-i', '--interval', type=float, default=1.0, help='Interval in seconds for updating holding registers (default: 1.0)')<br>
```


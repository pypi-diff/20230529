# Comparing `tmp/mb_base-1.0.202305291126-py3-none-any.whl.zip` & `tmp/mb_base-1.0.202305291127-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
 Zip file size: 4936 bytes, number of entries: 10
 -rw-rw-r--  2.0 unx      323 b- defN 23-May-25 00:28 mb/numpy/__init__.py
 -rw-rw-r--  2.0 unx       49 b- defN 23-May-25 00:31 mb/pandas/__init__.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-May-25 20:10 mb/plt/__init__.py
 -rw-rw-r--  2.0 unx     7970 b- defN 23-May-29 11:02 mb/plt/emb_viz.py
--rw-rw-r--  2.0 unx       66 b- defN 23-May-29 11:26 mb/utils/__init__.py
+-rw-rw-r--  2.0 unx       65 b- defN 23-May-29 11:27 mb/utils/__init__.py
 -rw-rw-r--  2.0 unx      739 b- defN 23-May-29 11:18 mb/utils/pip_update.py
--rw-rw-r--  2.0 unx      291 b- defN 23-May-29 11:26 mb_base-1.0.202305291126.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-29 11:26 mb_base-1.0.202305291126.dist-info/WHEEL
--rw-rw-r--  2.0 unx        3 b- defN 23-May-29 11:26 mb_base-1.0.202305291126.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      792 b- defN 23-May-29 11:26 mb_base-1.0.202305291126.dist-info/RECORD
-10 files, 10379 bytes uncompressed, 3574 bytes compressed:  65.6%
+-rw-rw-r--  2.0 unx      291 b- defN 23-May-29 11:27 mb_base-1.0.202305291127.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-29 11:27 mb_base-1.0.202305291127.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        3 b- defN 23-May-29 11:27 mb_base-1.0.202305291127.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      792 b- defN 23-May-29 11:27 mb_base-1.0.202305291127.dist-info/RECORD
+10 files, 10378 bytes uncompressed, 3574 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: mb/utils/__init__.py
 Comment: 
 
 Filename: mb/utils/pip_update.py
 Comment: 
 
-Filename: mb_base-1.0.202305291126.dist-info/METADATA
+Filename: mb_base-1.0.202305291127.dist-info/METADATA
 Comment: 
 
-Filename: mb_base-1.0.202305291126.dist-info/WHEEL
+Filename: mb_base-1.0.202305291127.dist-info/WHEEL
 Comment: 
 
-Filename: mb_base-1.0.202305291126.dist-info/top_level.txt
+Filename: mb_base-1.0.202305291127.dist-info/top_level.txt
 Comment: 
 
-Filename: mb_base-1.0.202305291126.dist-info/RECORD
+Filename: mb_base-1.0.202305291127.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mb/utils/__init__.py

```diff
@@ -1,2 +1,2 @@
 from mb_utils.src import *
-#from .pip_update import update_package
+from .pip_update import update_package
```

## Comparing `mb_base-1.0.202305291126.dist-info/RECORD` & `mb_base-1.0.202305291127.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 mb/numpy/__init__.py,sha256=paJ-HHrMmhCCBXA9GVOGoWUjB82J4sJ6bczyaL0xY2E,323
 mb/pandas/__init__.py,sha256=iiTr58Dv_spuo__mao6bJcooroxw3qW0nwZGA8RqPUo,49
 mb/plt/__init__.py,sha256=Ya4j8QIe5BCbMesMr1W8L9LP-FBy9LZbUow0XatJczA,54
 mb/plt/emb_viz.py,sha256=W24rQmcMZs6ThWIcTOhy_qrcKqyT0Fl0cvi9yEcddbU,7970
-mb/utils/__init__.py,sha256=k_f4LKzJ-_ZoHwOGblxghYWdiZjlgljDzHZWd-IoS58,66
+mb/utils/__init__.py,sha256=A9wwxJCd4Pezd_tO0opRpggIOxZayl84dBE14FXmiFk,65
 mb/utils/pip_update.py,sha256=XoQg7t9Jq9EnBGeQp0DA1rreP745fL0yJTki8h9teMQ,739
-mb_base-1.0.202305291126.dist-info/METADATA,sha256=d7zawlSZ2bQ3iw1GVG56RxTY2k702zehrYwxHXK4vrs,291
-mb_base-1.0.202305291126.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-mb_base-1.0.202305291126.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
-mb_base-1.0.202305291126.dist-info/RECORD,,
+mb_base-1.0.202305291127.dist-info/METADATA,sha256=UqBwK47Rhc8oOaI4bbSqRLagBltf6A8VmLmvR46j7xY,291
+mb_base-1.0.202305291127.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+mb_base-1.0.202305291127.dist-info/top_level.txt,sha256=2T5lqIVZs7HUr0KqUMPEaPF59QXcr0ErDy6K-J88ycM,3
+mb_base-1.0.202305291127.dist-info/RECORD,,
```


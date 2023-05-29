# Comparing `tmp/sqlite_hello-0.1.0a36-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_hello-0.1.0a37-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 8403 bytes, number of entries: 9
--rwxr-xr-x  2.0 unx    15784 b- defN 23-May-29 04:55 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      305 b- defN 23-May-29 04:55 sqlite_hello/__init__.py
--rwxr-xr-x  2.0 unx    15856 b- defN 23-May-29 04:55 sqlite_hello/hello0.so
--rwxr-xr-x  2.0 unx    15848 b- defN 23-May-29 04:55 sqlite_hello/hola0.so
--rw-r--r--  2.0 unx       80 b- defN 23-May-29 04:55 sqlite_hello/version.py
--rw-r--r--  2.0 unx      507 b- defN 23-May-29 04:55 sqlite_hello-0.1.0a36.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-May-29 04:55 sqlite_hello-0.1.0a36.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-May-29 04:55 sqlite_hello-0.1.0a36.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      741 b- defN 23-May-29 04:55 sqlite_hello-0.1.0a36.dist-info/RECORD
-9 files, 49244 bytes uncompressed, 7125 bytes compressed:  85.5%
+Zip file size: 8400 bytes, number of entries: 9
+-rwxr-xr-x  2.0 unx    15784 b- defN 23-May-29 05:14 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      305 b- defN 23-May-29 05:14 sqlite_hello/__init__.py
+-rwxr-xr-x  2.0 unx    15856 b- defN 23-May-29 05:14 sqlite_hello/hello0.so
+-rwxr-xr-x  2.0 unx    15848 b- defN 23-May-29 05:14 sqlite_hello/hola0.so
+-rw-r--r--  2.0 unx       80 b- defN 23-May-29 05:14 sqlite_hello/version.py
+-rw-r--r--  2.0 unx      507 b- defN 23-May-29 05:14 sqlite_hello-0.1.0a37.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-May-29 05:14 sqlite_hello-0.1.0a37.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-May-29 05:14 sqlite_hello-0.1.0a37.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      741 b- defN 23-May-29 05:14 sqlite_hello-0.1.0a37.dist-info/RECORD
+9 files, 49244 bytes uncompressed, 7122 bytes compressed:  85.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sqlite_hello/hola0.so
 Comment: 
 
 Filename: sqlite_hello/version.py
 Comment: 
 
-Filename: sqlite_hello-0.1.0a36.dist-info/METADATA
+Filename: sqlite_hello-0.1.0a37.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_hello-0.1.0a36.dist-info/WHEEL
+Filename: sqlite_hello-0.1.0a37.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_hello-0.1.0a36.dist-info/top_level.txt
+Filename: sqlite_hello-0.1.0a37.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_hello-0.1.0a36.dist-info/RECORD
+Filename: sqlite_hello-0.1.0a37.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## sqlite_hello/hello0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: fc16918e0d5c507fb0a17763c7107ca4ab10c18b
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: b7dc2348e2933fe244f9d22544ec53bf9ceb7977
```

### strings --all --bytes=8 {}

```diff
@@ -1,15 +1,15 @@
 __gmon_start__
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize
 sqlite3_api
 sqlite3_hello_init
 Hello, %s!
-v0.1.0-alpha.36
+v0.1.0-alpha.37
 hello_version
 GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.8061
 __do_global_dtors_aux_fini_array_entry
```

### readelf --wide --decompress --string-dump=.rodata {}

```diff
@@ -1,7 +1,7 @@
 
 String dump of section '.rodata':
   [     0]  Hello, %s!
-  [     b]  v0.1.0-alpha.36
+  [     b]  v0.1.0-alpha.37
   [    1b]  hello
   [    21]  hello_version
```

## sqlite_hello/hola0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 337aa2569d96632665dddfca43547240602891ec
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: d09e7828fb209a8836dfd7063fcb3e5f353e18e1
```

### strings --all --bytes=8 {}

```diff
@@ -1,15 +1,15 @@
 __gmon_start__
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize
 sqlite3_api
 sqlite3_hola_init
 Hola, %s!
-v0.1.0-alpha.36
+v0.1.0-alpha.37
 hola_version
 GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.8061
 __do_global_dtors_aux_fini_array_entry
```

### readelf --wide --decompress --string-dump=.rodata {}

```diff
@@ -1,7 +1,7 @@
 
 String dump of section '.rodata':
   [     2]  Hola, %s!
-  [     c]  v0.1.0-alpha.36
+  [     c]  v0.1.0-alpha.37
   [    1c]  hola
   [    21]  hola_version
```

## sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.36"
+__version__ = "0.1.0-alpha.37"
 __version_info__ = tuple(__version__.split("."))
```

## Comparing `sqlite_hello-0.1.0a36.dist-info/RECORD` & `sqlite_hello-0.1.0a37.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 noop.cpython-311-x86_64-linux-gnu.so,sha256=EYkwvM4rO5qdrRrumV09xH-JHgEZiTW5qhXN2rWNjJs,15784
 sqlite_hello/__init__.py,sha256=pcA3IBYCodi0pYnpMRWpFRZcLsiBjMrMdhPM0TLEzUM,305
-sqlite_hello/hello0.so,sha256=OzqpQHTzhxaEXcR2HM54CdOu-TK2MqzbbHQSm84Pi8o,15856
-sqlite_hello/hola0.so,sha256=qGpkIw8aPEN6gwNFgSsY-fKps0Y5aUM-wyHkWGtD1Sg,15848
-sqlite_hello/version.py,sha256=3_XKwwEFKKUTZTs-kitDDvDr0jR5LTSNnADLjAMoz94,80
-sqlite_hello-0.1.0a36.dist-info/METADATA,sha256=GIlIP3z5C_Q3Uu7PCX2U_pBUEwgaQ-AC-aMoZH-JnjM,507
-sqlite_hello-0.1.0a36.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
-sqlite_hello-0.1.0a36.dist-info/top_level.txt,sha256=KjVnaNCiS11UOKhSHnqZUwUFlrCeCQv89AtVw-JnynI,18
-sqlite_hello-0.1.0a36.dist-info/RECORD,,
+sqlite_hello/hello0.so,sha256=ZeKiAe_10t7kOmVzAO2ypZgqtaqDO6IdUqpTDo6gO6Y,15856
+sqlite_hello/hola0.so,sha256=8YhhUkJ_ET-nmQ5AqP1fBhNYNnyGnY2jtEa9cIbd5XU,15848
+sqlite_hello/version.py,sha256=8h0LuemAWtm8M-buiVGM8JoHQ7iPYNx-lAmf0AGSvNk,80
+sqlite_hello-0.1.0a37.dist-info/METADATA,sha256=O-DSMBBFkhlqQhDFs-JCnYttX7PxqqGW_FFroJcMPts,507
+sqlite_hello-0.1.0a37.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
+sqlite_hello-0.1.0a37.dist-info/top_level.txt,sha256=KjVnaNCiS11UOKhSHnqZUwUFlrCeCQv89AtVw-JnynI,18
+sqlite_hello-0.1.0a37.dist-info/RECORD,,
```


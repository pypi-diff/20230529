# Comparing `tmp/sqlite_hello-0.1.0a34-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_hello-0.1.0a35-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
 Zip file size: 8401 bytes, number of entries: 9
--rwxr-xr-x  2.0 unx    15784 b- defN 23-May-29 04:39 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      305 b- defN 23-May-29 04:38 sqlite_hello/__init__.py
--rwxr-xr-x  2.0 unx    15856 b- defN 23-May-29 04:38 sqlite_hello/hello0.so
--rwxr-xr-x  2.0 unx    15848 b- defN 23-May-29 04:38 sqlite_hello/hola0.so
--rw-r--r--  2.0 unx       80 b- defN 23-May-29 04:38 sqlite_hello/version.py
--rw-r--r--  2.0 unx      507 b- defN 23-May-29 04:39 sqlite_hello-0.1.0a34.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-May-29 04:39 sqlite_hello-0.1.0a34.dist-info/WHEEL
--rw-r--r--  2.0 unx       18 b- defN 23-May-29 04:39 sqlite_hello-0.1.0a34.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      741 b- defN 23-May-29 04:39 sqlite_hello-0.1.0a34.dist-info/RECORD
+-rwxr-xr-x  2.0 unx    15784 b- defN 23-May-29 04:50 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      305 b- defN 23-May-29 04:50 sqlite_hello/__init__.py
+-rwxr-xr-x  2.0 unx    15856 b- defN 23-May-29 04:50 sqlite_hello/hello0.so
+-rwxr-xr-x  2.0 unx    15848 b- defN 23-May-29 04:50 sqlite_hello/hola0.so
+-rw-r--r--  2.0 unx       80 b- defN 23-May-29 04:50 sqlite_hello/version.py
+-rw-r--r--  2.0 unx      507 b- defN 23-May-29 04:50 sqlite_hello-0.1.0a35.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-May-29 04:50 sqlite_hello-0.1.0a35.dist-info/WHEEL
+-rw-r--r--  2.0 unx       18 b- defN 23-May-29 04:50 sqlite_hello-0.1.0a35.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      741 b- defN 23-May-29 04:50 sqlite_hello-0.1.0a35.dist-info/RECORD
 9 files, 49244 bytes uncompressed, 7123 bytes compressed:  85.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sqlite_hello/hola0.so
 Comment: 
 
 Filename: sqlite_hello/version.py
 Comment: 
 
-Filename: sqlite_hello-0.1.0a34.dist-info/METADATA
+Filename: sqlite_hello-0.1.0a35.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_hello-0.1.0a34.dist-info/WHEEL
+Filename: sqlite_hello-0.1.0a35.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_hello-0.1.0a34.dist-info/top_level.txt
+Filename: sqlite_hello-0.1.0a35.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_hello-0.1.0a34.dist-info/RECORD
+Filename: sqlite_hello-0.1.0a35.dist-info/RECORD
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
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: d148a3f0a534d17aabd22adf30424c1977bb546e
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 0226258e0cf0ef00d26ff14ea9bbf4ea4b67d889
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
-v0.1.0-alpha.34
+v0.1.0-alpha.35
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
-  [     b]  v0.1.0-alpha.34
+  [     b]  v0.1.0-alpha.35
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
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 731459fefdac707bd6ed1d6ac750b0e6e4b82496
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 881cca49df843cb7fabc73e808d7235e0bf88a7d
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
-v0.1.0-alpha.34
+v0.1.0-alpha.35
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
-  [     c]  v0.1.0-alpha.34
+  [     c]  v0.1.0-alpha.35
   [    1c]  hola
   [    21]  hola_version
```

## sqlite_hello/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.0-alpha.34"
+__version__ = "0.1.0-alpha.35"
 __version_info__ = tuple(__version__.split("."))
```

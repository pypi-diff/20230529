# Comparing `tmp/gs_engine-0.22.0a20230528-py2.py3-none-macosx_11_0_x86_64.whl.zip` & `tmp/gs_engine-0.22.0a20230529-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 11905 bytes, number of entries: 9
--rw-rw-r--  2.0 unx      840 b- defN 23-May-28 21:09 gs_engine-0.22.0a20230528.dist-info/RECORD
--rw-r--r--  2.0 unx      140 b- defN 23-May-28 20:57 gs_engine-0.22.0a20230528.dist-info/WHEEL
--rw-r--r--  2.0 unx       19 b- defN 23-May-28 20:57 gs_engine-0.22.0a20230528.dist-info/top_level.txt
--rw-r--r--  2.0 unx    21664 b- defN 23-May-28 20:57 gs_engine-0.22.0a20230528.dist-info/METADATA
--rw-r--r--  2.0 unx      694 b- defN 23-May-28 19:08 graphscope_runtime/__init__.py
--rw-r--r--  2.0 unx     1573 b- defN 23-May-28 19:08 graphscope.runtime/conf/log4j2.xml
--rw-r--r--  2.0 unx      398 b- defN 23-May-28 19:08 graphscope.runtime/conf/executor.vineyard.properties
--rw-r--r--  2.0 unx      504 b- defN 23-May-28 19:08 graphscope.runtime/conf/frontend.vineyard.properties
--rw-r--r--  2.0 unx      204 b- defN 23-May-28 19:08 graphscope.runtime/conf/log4rs.yml
-9 files, 26036 bytes uncompressed, 10443 bytes compressed:  59.9%
+Zip file size: 11887 bytes, number of entries: 9
+-rw-r--r--  2.0 unx      398 b- defN 23-May-29 19:02 graphscope.runtime/conf/executor.vineyard.properties
+-rw-r--r--  2.0 unx      504 b- defN 23-May-29 19:02 graphscope.runtime/conf/frontend.vineyard.properties
+-rw-r--r--  2.0 unx     1573 b- defN 23-May-29 19:02 graphscope.runtime/conf/log4j2.xml
+-rw-r--r--  2.0 unx      204 b- defN 23-May-29 19:02 graphscope.runtime/conf/log4rs.yml
+-rw-r--r--  2.0 unx      694 b- defN 23-May-29 19:02 graphscope_runtime/__init__.py
+-rw-r--r--  2.0 unx    21664 b- defN 23-May-29 20:27 gs_engine-0.22.0a20230529.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-May-29 20:27 gs_engine-0.22.0a20230529.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 23-May-29 20:27 gs_engine-0.22.0a20230529.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      831 b- defN 23-May-29 20:27 gs_engine-0.22.0a20230529.dist-info/RECORD
+9 files, 25997 bytes uncompressed, 10425 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,28 +1,28 @@
-Filename: gs_engine-0.22.0a20230528.dist-info/RECORD
+Filename: graphscope.runtime/conf/executor.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.22.0a20230528.dist-info/WHEEL
+Filename: graphscope.runtime/conf/frontend.vineyard.properties
 Comment: 
 
-Filename: gs_engine-0.22.0a20230528.dist-info/top_level.txt
+Filename: graphscope.runtime/conf/log4j2.xml
 Comment: 
 
-Filename: gs_engine-0.22.0a20230528.dist-info/METADATA
+Filename: graphscope.runtime/conf/log4rs.yml
 Comment: 
 
 Filename: graphscope_runtime/__init__.py
 Comment: 
 
-Filename: graphscope.runtime/conf/log4j2.xml
+Filename: gs_engine-0.22.0a20230529.dist-info/METADATA
 Comment: 
 
-Filename: graphscope.runtime/conf/executor.vineyard.properties
+Filename: gs_engine-0.22.0a20230529.dist-info/WHEEL
 Comment: 
 
-Filename: graphscope.runtime/conf/frontend.vineyard.properties
+Filename: gs_engine-0.22.0a20230529.dist-info/top_level.txt
 Comment: 
 
-Filename: graphscope.runtime/conf/log4rs.yml
+Filename: gs_engine-0.22.0a20230529.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `gs_engine-0.22.0a20230528.dist-info/METADATA` & `gs_engine-0.22.0a20230529.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gs-engine
-Version: 0.22.0a20230528
+Version: 0.22.0a20230529
 Home-page: https://github.com/alibaba/GraphScope
 Author: GraphScope Team, Damo Academy
 Author-email: graphscope@alibaba-inc.com
 License: Apache License 2.0
 Keywords: GraphScope,Graph Computations
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```


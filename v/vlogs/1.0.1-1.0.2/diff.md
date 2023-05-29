# Comparing `tmp/vlogs-1.0.1.tar.gz` & `tmp/vlogs-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlogs-1.0.1.tar", max compression
+gzip compressed data, was "vlogs-1.0.2.tar", max compression
```

## Comparing `vlogs-1.0.1.tar` & `vlogs-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1045 2023-05-29 14:15:19.443787 vlogs-1.0.1/README.md
--rw-r--r--   0        0        0      342 2023-05-29 14:27:37.739031 vlogs-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-29 12:28:45.438951 vlogs-1.0.1/vlogs/__init__.py
--rw-r--r--   0        0        0       43 2023-05-29 12:42:40.212891 vlogs-1.0.1/vlogs/config.py
--rw-r--r--   0        0        0    11594 2023-05-29 14:26:39.114872 vlogs-1.0.1/vlogs/model.py
--rw-r--r--   0        0        0     2554 2023-05-29 14:26:29.465818 vlogs-1.0.1/vlogs/sdk.py
--rw-r--r--   0        0        0      804 2023-05-29 14:27:14.301584 vlogs-1.0.1/vlogs/service.py
--rw-r--r--   0        0        0      498 2023-05-29 12:44:44.073784 vlogs-1.0.1/vlogs/util.py
--rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 vlogs-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1222 2023-05-29 14:39:46.449093 vlogs-1.0.2/README.md
+-rw-r--r--   0        0        0      342 2023-05-29 14:46:25.579947 vlogs-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-29 12:28:45.438951 vlogs-1.0.2/vlogs/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-29 12:42:40.212891 vlogs-1.0.2/vlogs/config.py
+-rw-r--r--   0        0        0    11594 2023-05-29 14:26:39.114872 vlogs-1.0.2/vlogs/model.py
+-rw-r--r--   0        0        0     2554 2023-05-29 14:26:29.465818 vlogs-1.0.2/vlogs/sdk.py
+-rw-r--r--   0        0        0      804 2023-05-29 14:27:14.301584 vlogs-1.0.2/vlogs/service.py
+-rw-r--r--   0        0        0      500 2023-05-29 14:46:08.230314 vlogs-1.0.2/vlogs/util.py
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 vlogs-1.0.2/PKG-INFO
```

### Comparing `vlogs-1.0.1/README.md` & `vlogs-1.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,36 +12,40 @@
 ```
 
 ### Usages
 
 ```python
 from vlogs.sdk import VLogs, VLogsOptions
 from vlogs.model import Collector, CollectorType, CollectorSource
+import asyncio
 
-appId = "xx"
-apiKey = "vlogs_xx"
+appId = "72bd14c306a91fa8a590330e3898ddcc"
+apiKey = "vlogs_gX9WwSdKatMNdpUClLU0IfCx575tvdoeQ"
 
 # Create VLogs instance
 sdk = VLogs.create(
     VLogsOptions.builder()
     .apiKey(apiKey)
     .appId(appId)
     .build()
 )
 
-response = sdk.collect(
-    Collector.builder()
-    .type(CollectorType.Error)
-    .source(CollectorSource.Other)
-    .message("This is a test message")
-    .build()
-)
+async def main():
+    response = await sdk.collect(
+        Collector.builder()
+        .type(CollectorType.Error)
+        .source(CollectorSource.Other)
+        .message("This is a test message")
+        .build()
+    )
 
-print("Response: ", response)
+    print("Response: ", response)
 
+# Run the async function
+asyncio.run(main())
 ```
 
 ### Build, Install, and Test from Source
 
 ```shell
 make
 ```
```

### Comparing `vlogs-1.0.1/vlogs/model.py` & `vlogs-1.0.2/vlogs/model.py`

 * *Files identical despite different names*

### Comparing `vlogs-1.0.1/vlogs/sdk.py` & `vlogs-1.0.2/vlogs/sdk.py`

 * *Files identical despite different names*

### Comparing `vlogs-1.0.1/vlogs/service.py` & `vlogs-1.0.2/vlogs/service.py`

 * *Files identical despite different names*

### Comparing `vlogs-1.0.1/PKG-INFO` & `vlogs-1.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlogs
-Version: 1.0.1
+Version: 1.0.2
 Summary: CUBETIQ vLogs SDK for Python
 License: MIT
 Author: Sambo Chea
 Author-email: sombochea@cubetiqs.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -26,36 +26,40 @@
 ```
 
 ### Usages
 
 ```python
 from vlogs.sdk import VLogs, VLogsOptions
 from vlogs.model import Collector, CollectorType, CollectorSource
+import asyncio
 
-appId = "xx"
-apiKey = "vlogs_xx"
+appId = "72bd14c306a91fa8a590330e3898ddcc"
+apiKey = "vlogs_gX9WwSdKatMNdpUClLU0IfCx575tvdoeQ"
 
 # Create VLogs instance
 sdk = VLogs.create(
     VLogsOptions.builder()
     .apiKey(apiKey)
     .appId(appId)
     .build()
 )
 
-response = sdk.collect(
-    Collector.builder()
-    .type(CollectorType.Error)
-    .source(CollectorSource.Other)
-    .message("This is a test message")
-    .build()
-)
+async def main():
+    response = await sdk.collect(
+        Collector.builder()
+        .type(CollectorType.Error)
+        .source(CollectorSource.Other)
+        .message("This is a test message")
+        .build()
+    )
 
-print("Response: ", response)
+    print("Response: ", response)
 
+# Run the async function
+asyncio.run(main())
 ```
 
 ### Build, Install, and Test from Source
 
 ```shell
 make
 ```
```


# Comparing `tmp/aiogrpcclient-1.3.4-py3-none-any.whl.zip` & `tmp/aiogrpcclient-1.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3329 bytes, number of entries: 5
+Zip file size: 3340 bytes, number of entries: 5
 -rw-r--r--  2.0 unx       94 b- defN 22-Oct-25 09:23 aiogrpcclient/__init__.py
--rw-r--r--  2.0 unx     5495 b- defN 23-Apr-16 19:34 aiogrpcclient/base.py
-?rw-------  2.0 unx       91 b- defN 23-May-19 17:49 aiogrpcclient-1.3.4.dist-info/WHEEL
-?rw-------  2.0 unx      552 b- defN 23-May-19 17:49 aiogrpcclient-1.3.4.dist-info/METADATA
-?rw-------  2.0 unx      381 b- defN 23-May-19 17:49 aiogrpcclient-1.3.4.dist-info/RECORD
-5 files, 6613 bytes uncompressed, 2617 bytes compressed:  60.4%
+-rw-r--r--  2.0 unx     5529 b- defN 23-May-29 19:16 aiogrpcclient/base.py
+?rw-------  2.0 unx       91 b- defN 23-May-29 19:19 aiogrpcclient-1.3.5.dist-info/WHEEL
+?rw-------  2.0 unx      552 b- defN 23-May-29 19:19 aiogrpcclient-1.3.5.dist-info/METADATA
+?rw-------  2.0 unx      381 b- defN 23-May-29 19:19 aiogrpcclient-1.3.5.dist-info/RECORD
+5 files, 6647 bytes uncompressed, 2628 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: aiogrpcclient/__init__.py
 Comment: 
 
 Filename: aiogrpcclient/base.py
 Comment: 
 
-Filename: aiogrpcclient-1.3.4.dist-info/WHEEL
+Filename: aiogrpcclient-1.3.5.dist-info/WHEEL
 Comment: 
 
-Filename: aiogrpcclient-1.3.4.dist-info/METADATA
+Filename: aiogrpcclient-1.3.5.dist-info/METADATA
 Comment: 
 
-Filename: aiogrpcclient-1.3.4.dist-info/RECORD
+Filename: aiogrpcclient-1.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aiogrpcclient/base.py

```diff
@@ -3,15 +3,14 @@
 import json
 import logging
 import sys
 import typing
 from functools import wraps
 
 import grpc
-import termcolor
 import yaml
 from aiokit import AioThing
 from grpc import StatusCode
 from grpc.experimental.aio import insecure_channel
 from izihawa_utils.pb_to_json import MessageToDict
 from termcolor import colored
 
@@ -111,14 +110,15 @@
     def __init__(
         self,
         endpoint,
         max_retries: int = 2,
         retry_delay: float = 0.5,
         connection_timeout: float = None,
         max_message_length: int = 1024 * 1024 * 1024,
+        compression=None,
     ):
         super().__init__()
         if endpoint is None:
             raise RuntimeError(f'`endpoint` must be passed for {self.__class__.__name__} constructor')
         options = [
             ('grpc.dns_min_time_between_resolutions_ms', 1000),
             ('grpc.initial_reconnect_backoff_ms', 1000),
@@ -135,15 +135,15 @@
                     'maxBackoff': f'{retry_delay}s',
                     'backoffMultiplier': 1,
                     'retryableStatusCodes': list(map(lambda x: x.name, self.temporary_errors)),
                 }
             }]}))
         ]
         self.connection_timeout = connection_timeout
-        self.channel = insecure_channel(endpoint, options)
+        self.channel = insecure_channel(endpoint, options, compression=compression)
         self.stubs = {}
         for stub_name, stub_cls in self.stub_clses.items():
             self.stubs[stub_name] = stub_cls(self.channel)
 
     async def start(self):
         logging.getLogger('debug').debug({
             'action': 'start',
```

## Comparing `aiogrpcclient-1.3.4.dist-info/METADATA` & `aiogrpcclient-1.3.5.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiogrpcclient
-Version: 1.3.4
+Version: 1.3.5
 Author: Pasha Podolsky
 Author-email: ppodolsky@me.com
 Home-page: https://github.com/izihawa/aiogrpcclient
 License: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Requires-Dist: aiokit >= 1.2.2
```


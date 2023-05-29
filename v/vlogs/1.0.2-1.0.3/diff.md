# Comparing `tmp/vlogs-1.0.2.tar.gz` & `tmp/vlogs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlogs-1.0.2.tar", max compression
+gzip compressed data, was "vlogs-1.0.3.tar", max compression
```

## Comparing `vlogs-1.0.2.tar` & `vlogs-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1222 2023-05-29 14:39:46.449093 vlogs-1.0.2/README.md
--rw-r--r--   0        0        0      342 2023-05-29 14:46:25.579947 vlogs-1.0.2/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-29 12:28:45.438951 vlogs-1.0.2/vlogs/__init__.py
--rw-r--r--   0        0        0       43 2023-05-29 12:42:40.212891 vlogs-1.0.2/vlogs/config.py
--rw-r--r--   0        0        0    11594 2023-05-29 14:26:39.114872 vlogs-1.0.2/vlogs/model.py
--rw-r--r--   0        0        0     2554 2023-05-29 14:26:29.465818 vlogs-1.0.2/vlogs/sdk.py
--rw-r--r--   0        0        0      804 2023-05-29 14:27:14.301584 vlogs-1.0.2/vlogs/service.py
--rw-r--r--   0        0        0      500 2023-05-29 14:46:08.230314 vlogs-1.0.2/vlogs/util.py
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 vlogs-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1222 2023-05-29 14:39:46.449093 vlogs-1.0.3/README.md
+-rw-r--r--   0        0        0      342 2023-05-29 14:52:25.261682 vlogs-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-29 12:28:45.438951 vlogs-1.0.3/vlogs/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-29 12:42:40.212891 vlogs-1.0.3/vlogs/config.py
+-rw-r--r--   0        0        0    11646 2023-05-29 14:51:51.425511 vlogs-1.0.3/vlogs/model.py
+-rw-r--r--   0        0        0     2554 2023-05-29 14:51:12.793514 vlogs-1.0.3/vlogs/sdk.py
+-rw-r--r--   0        0        0      804 2023-05-29 14:27:14.301584 vlogs-1.0.3/vlogs/service.py
+-rw-r--r--   0        0        0      500 2023-05-29 14:46:08.230314 vlogs-1.0.3/vlogs/util.py
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 vlogs-1.0.3/PKG-INFO
```

### Comparing `vlogs-1.0.2/README.md` & `vlogs-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `vlogs-1.0.2/vlogs/model.py` & `vlogs-1.0.3/vlogs/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,15 +163,15 @@
     def __init__(self, name=None, version=None, versionCode=None, hostname=None, sender=None):
         self.name = name
         self.version = version
         self.versionCode = versionCode
         self.hostname = hostname
         self.sender = sender
 
-    def toMap(self):
+    def to_map(self):
         return {
             'name': self.name,
             'version': self.version,
             'version_code': self.versionCode,
             'hostname': self.hostname,
             'sender': self.sender
         }
@@ -216,24 +216,24 @@
             versionCode=self._versionCode,
             hostname=self._hostname,
             sender=self._sender
         )
 
 
 class Target:
-    def __init__(self, telegram=None, discord=None, sdkInfo=None):
+    def __init__(self, telegram: Telegram = None, discord: Discord = None, sdkInfo: SDKInfo = None):
         self.telegram = telegram
         self.discord = discord
         self.sdkInfo = sdkInfo
 
-    def toMap(self):
+    def to_map(self):
         return {
-            'telegram': self.telegram.toMap() if self.telegram else None,
-            'discord': self.discord.toMap() if self.discord else None,
-            'sdk_info': self.sdkInfo.toMap() if self.sdkInfo else None
+            'telegram': self.telegram.to_map() if self.telegram else None,
+            'discord': self.discord.to_map() if self.discord else None,
+            'sdk_info': self.sdkInfo.to_map() if self.sdkInfo else None
         }
 
     def merge(self, defaultTarget=None):
         if not defaultTarget:
             return
         self.telegram = self.telegram or defaultTarget.telegram
         self.discord = self.discord or defaultTarget.discord
@@ -273,64 +273,64 @@
         return self
 
     def build(self):
         return Target(telegram=self._telegram, discord=self._discord, sdkInfo=self._sdkInfo)
 
 
 class Collector:
-    def __init__(self, id=None, type=None, source=None, message=None, data=None, userAgent=None, timestamp=None, target=None, tags=None):
+    def __init__(self, id=None, type=None, source=None, message=None, data=None, useragent=None, timestamp=None, target=None, tags=None):
         self.id = id
         self.type = type
         self.source = source
         self.message = message
         self.data = data
-        self.userAgent = userAgent
+        self.useragent = useragent
         self.timestamp = timestamp
         self.target = target
         self.tags = tags
 
     def getId(self):
         if not self.id:
             self.id = generate_uuid()
         return self.id
 
-    def getTimestamp(self):
+    def get_timestamp(self):
         if not self.timestamp:
             self.timestamp = int(time.time() * 1000)
         return self.timestamp
 
-    def toMap(self):
+    def to_map(self):
         return {
             'id': self.getId(),
             'type': self.type,
             'source': self.source,
             'message': self.message,
             'data': self.data,
-            'user_agent': self.userAgent,
-            'timestamp': self.getTimestamp(),
-            'target': self.target.toMap() if self.target else None,
+            'user_agent': self.useragent,
+            'timestamp': self.get_timestamp(),
+            'target': self.target.to_map() if self.target else None,
             'tags': self.tags,
         }
 
     def toJson(self):
-        return json.dumps(self.toMap())
+        return json.dumps(self.to_map())
 
     @staticmethod
     def builder():
         return CollectorBuilder()
 
 
 class CollectorBuilder:
     def __init__(self):
         self._id = None
         self._type = None
         self._source = None
         self._message = None
         self._data = None
-        self._userAgent = None
+        self._useragent = None
         self._timestamp = None
         self._target = None
         self._tags = None
 
     def id(self, id):
         self._id = id
         return self
@@ -347,16 +347,16 @@
         self._message = message
         return self
 
     def data(self, data):
         self._data = data
         return self
 
-    def userAgent(self, userAgent):
-        self._userAgent = userAgent
+    def useragent(self, useragent):
+        self._useragent = useragent
         return self
 
     def timestamp(self, timestamp):
         self._timestamp = timestamp
         return self
 
     def target(self, target):
@@ -370,29 +370,29 @@
     def build(self):
         return Collector(
             id=self._id,
             type=self._type,
             source=self._source,
             message=self._message,
             data=self._data,
-            userAgent=self._userAgent,
+            useragent=self._useragent,
             timestamp=self._timestamp,
             target=self._target,
             tags=self._tags,
         )
 
 
 class CollectorResponse:
     def __init__(self, message=None, id=None):
         self.message = message
         self.id = id
 
 
 class VLogsOptions:
-    def __init__(self, url=None, appId=None, apiKey=None, connectionTimeout=None, testConnection=None, target=None):
+    def __init__(self, url=None, appId=None, apiKey=None, connectionTimeout=None, testConnection=None, target: Target=None):
         self.url = url
         self.appId = appId
         self.apiKey = apiKey
         self.connectionTimeout = connectionTimeout
         self.testConnection = testConnection
         self.target = target
```

### Comparing `vlogs-1.0.2/vlogs/sdk.py` & `vlogs-1.0.3/vlogs/sdk.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             if self._options.target:
                 request.target.merge(self._options.target)
 
         # Set SDK info to request
         request.target.sdk_info = sdk_info
 
         # Append user agent to request
-        request.userAgent = f'vlogs-python-sdk/{VLogs.VERSION}-{VLogs.VERSION_CODE} ({hostname})'
+        request.useragent = f'vlogs-python-sdk/{VLogs.VERSION}-{VLogs.VERSION_CODE} ({hostname})'
 
         response = await self._service.post(request.to_map(), headers, self._options.connectionTimeout or VLogs.DEFAULT_CONNECT_TIMEOUT)
         return response
 
     @staticmethod
     def create(options: VLogsOptions) -> 'VLogs':
         return VLogs(options)
```

### Comparing `vlogs-1.0.2/vlogs/service.py` & `vlogs-1.0.3/vlogs/service.py`

 * *Files identical despite different names*

### Comparing `vlogs-1.0.2/PKG-INFO` & `vlogs-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlogs
-Version: 1.0.2
+Version: 1.0.3
 Summary: CUBETIQ vLogs SDK for Python
 License: MIT
 Author: Sambo Chea
 Author-email: sombochea@cubetiqs.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


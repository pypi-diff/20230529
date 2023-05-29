# Comparing `tmp/vlogs-1.0.0.tar.gz` & `tmp/vlogs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlogs-1.0.0.tar", max compression
+gzip compressed data, was "vlogs-1.0.1.tar", max compression
```

## Comparing `vlogs-1.0.0.tar` & `vlogs-1.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1045 2023-05-29 14:15:19.443787 vlogs-1.0.0/README.md
--rw-r--r--   0        0        0      342 2023-05-29 12:27:53.734002 vlogs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-29 12:28:45.438951 vlogs-1.0.0/vlogs/__init__.py
--rw-r--r--   0        0        0       43 2023-05-29 12:42:40.212891 vlogs-1.0.0/vlogs/config.py
--rw-r--r--   0        0        0    11588 2023-05-29 14:01:43.619448 vlogs-1.0.0/vlogs/model.py
--rw-r--r--   0        0        0     2530 2023-05-29 14:02:52.795775 vlogs-1.0.0/vlogs/sdk.py
--rw-r--r--   0        0        0      792 2023-05-29 12:43:06.177074 vlogs-1.0.0/vlogs/service.py
--rw-r--r--   0        0        0      498 2023-05-29 12:44:44.073784 vlogs-1.0.0/vlogs/util.py
--rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 vlogs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1045 2023-05-29 14:15:19.443787 vlogs-1.0.1/README.md
+-rw-r--r--   0        0        0      342 2023-05-29 14:27:37.739031 vlogs-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-29 12:28:45.438951 vlogs-1.0.1/vlogs/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-29 12:42:40.212891 vlogs-1.0.1/vlogs/config.py
+-rw-r--r--   0        0        0    11594 2023-05-29 14:26:39.114872 vlogs-1.0.1/vlogs/model.py
+-rw-r--r--   0        0        0     2554 2023-05-29 14:26:29.465818 vlogs-1.0.1/vlogs/sdk.py
+-rw-r--r--   0        0        0      804 2023-05-29 14:27:14.301584 vlogs-1.0.1/vlogs/service.py
+-rw-r--r--   0        0        0      498 2023-05-29 12:44:44.073784 vlogs-1.0.1/vlogs/util.py
+-rw-r--r--   0        0        0     1473 1970-01-01 00:00:00.000000 vlogs-1.0.1/PKG-INFO
```

### Comparing `vlogs-1.0.0/README.md` & `vlogs-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `vlogs-1.0.0/vlogs/model.py` & `vlogs-1.0.1/vlogs/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 import time
-from util import generate_uuid
+from vlogs.util import generate_uuid
 
 
 class CollectorType:
     Error = "Error"
     Event = "Event"
     Metric = "Metric"
     Trace = "Trace"
```

### Comparing `vlogs-1.0.0/vlogs/sdk.py` & `vlogs-1.0.1/vlogs/sdk.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from model import Collector, CollectorResponse, SDKInfo, Target, VLogsOptions
-from service import VLogsService
-from util import get_system_hostname, get_system_username
-from config import BASE_URL
+from vlogs.model import Collector, CollectorResponse, SDKInfo, Target, VLogsOptions
+from vlogs.service import VLogsService
+from vlogs.util import get_system_hostname, get_system_username
+from vlogs.config import BASE_URL
 
 
 class VLogs:
     _logger = print
     NAME = 'vlogs'
     VERSION = '1.0.0'
     VERSION_CODE = '1'
```

### Comparing `vlogs-1.0.0/vlogs/service.py` & `vlogs-1.0.1/vlogs/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import requests
 
-from model import CollectorResponse
-from config import BASE_URL
+from vlogs.model import CollectorResponse
+from vlogs.config import BASE_URL
 
 
 class VLogsService:
     def __init__(self, base_url=BASE_URL):
         self.url = f"{base_url}/api/v1/collector"
 
     def post(self, body, headers=None, timeout=None):
```

### Comparing `vlogs-1.0.0/PKG-INFO` & `vlogs-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlogs
-Version: 1.0.0
+Version: 1.0.1
 Summary: CUBETIQ vLogs SDK for Python
 License: MIT
 Author: Sambo Chea
 Author-email: sombochea@cubetiqs.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


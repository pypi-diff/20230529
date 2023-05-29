# Comparing `tmp/vlogs-1.0.3.tar.gz` & `tmp/vlogs-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vlogs-1.0.3.tar", max compression
+gzip compressed data, was "vlogs-1.0.4.tar", max compression
```

## Comparing `vlogs-1.0.3.tar` & `vlogs-1.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1222 2023-05-29 14:39:46.449093 vlogs-1.0.3/README.md
--rw-r--r--   0        0        0      342 2023-05-29 14:52:25.261682 vlogs-1.0.3/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-29 12:28:45.438951 vlogs-1.0.3/vlogs/__init__.py
--rw-r--r--   0        0        0       43 2023-05-29 12:42:40.212891 vlogs-1.0.3/vlogs/config.py
--rw-r--r--   0        0        0    11646 2023-05-29 14:51:51.425511 vlogs-1.0.3/vlogs/model.py
--rw-r--r--   0        0        0     2554 2023-05-29 14:51:12.793514 vlogs-1.0.3/vlogs/sdk.py
--rw-r--r--   0        0        0      804 2023-05-29 14:27:14.301584 vlogs-1.0.3/vlogs/service.py
--rw-r--r--   0        0        0      500 2023-05-29 14:46:08.230314 vlogs-1.0.3/vlogs/util.py
--rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 vlogs-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1222 2023-05-29 14:39:46.449093 vlogs-1.0.4/README.md
+-rw-r--r--   0        0        0      342 2023-05-29 15:35:10.625758 vlogs-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-29 12:28:45.438951 vlogs-1.0.4/vlogs/__init__.py
+-rw-r--r--   0        0        0       43 2023-05-29 12:42:40.212891 vlogs-1.0.4/vlogs/config.py
+-rw-r--r--   0        0        0    11646 2023-05-29 14:51:51.425511 vlogs-1.0.4/vlogs/model.py
+-rw-r--r--   0        0        0     2554 2023-05-29 14:51:12.793514 vlogs-1.0.4/vlogs/sdk.py
+-rw-r--r--   0        0        0      733 2023-05-29 15:36:08.720409 vlogs-1.0.4/vlogs/service.py
+-rw-r--r--   0        0        0      500 2023-05-29 14:46:08.230314 vlogs-1.0.4/vlogs/util.py
+-rw-r--r--   0        0        0     1650 1970-01-01 00:00:00.000000 vlogs-1.0.4/PKG-INFO
```

### Comparing `vlogs-1.0.3/README.md` & `vlogs-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `vlogs-1.0.3/vlogs/model.py` & `vlogs-1.0.4/vlogs/model.py`

 * *Files identical despite different names*

### Comparing `vlogs-1.0.3/vlogs/sdk.py` & `vlogs-1.0.4/vlogs/sdk.py`

 * *Files identical despite different names*

### Comparing `vlogs-1.0.3/vlogs/service.py` & `vlogs-1.0.4/vlogs/service.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,23 +5,20 @@
 
 
 class VLogsService:
     def __init__(self, base_url=BASE_URL):
         self.url = f"{base_url}/api/v1/collector"
 
     def post(self, body, headers=None, timeout=None):
-        config = {
-            "method": "POST",
-            "url": self.url,
-            "data": body,
-            "headers": headers,
-            "timeout": timeout * 1000 if timeout else None,
-        }
-
-        response = requests.post(**config)
+        response = requests.post(
+            data=body,
+            url=self.url,
+            headers=headers,
+            timeout=timeout * 1000 if timeout else None,
+        )
 
         if response.status_code in [200, 201, 202]:
             return CollectorResponse(**response.json())
         else:
             raise Exception(
                 f"Failed to post data to vlogs server with status code: {response.status_code} and message: {response.text}"
             )
```

### Comparing `vlogs-1.0.3/PKG-INFO` & `vlogs-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vlogs
-Version: 1.0.3
+Version: 1.0.4
 Summary: CUBETIQ vLogs SDK for Python
 License: MIT
 Author: Sambo Chea
 Author-email: sombochea@cubetiqs.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/idbadapter-1.3.tar.gz` & `tmp/idbadapter-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.3.tar", last modified: Mon May 22 10:10:40 2023, max compression
+gzip compressed data, was "idbadapter-1.4.tar", last modified: Mon May 29 08:37:34 2023, max compression
```

## Comparing `idbadapter-1.3.tar` & `idbadapter-1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 10:10:40.402476 idbadapter-1.3/
--rw-rw-rw-   0        0        0    11558 2023-05-02 13:28:55.000000 idbadapter-1.3/LICENSE
--rw-rw-rw-   0        0        0      695 2023-05-22 10:10:40.402476 idbadapter-1.3/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-05 13:33:15.000000 idbadapter-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-22 10:10:40.385041 idbadapter-1.3/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-22 08:18:39.000000 idbadapter-1.3/idbadapter/__init__.py
--rw-rw-rw-   0        0        0     6806 2023-05-22 10:04:07.000000 idbadapter-1.3/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-05-22 10:10:40.401477 idbadapter-1.3/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      695 2023-05-22 10:10:40.000000 idbadapter-1.3/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-05-22 10:10:40.000000 idbadapter-1.3/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 10:10:40.000000 idbadapter-1.3/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-22 10:10:40.000000 idbadapter-1.3/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 10:10:40.000000 idbadapter-1.3/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-22 10:10:40.403476 idbadapter-1.3/setup.cfg
--rw-rw-rw-   0        0        0      987 2023-05-22 10:07:35.000000 idbadapter-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:37:34.591438 idbadapter-1.4/
+-rw-rw-rw-   0        0        0    11558 2023-05-02 13:28:55.000000 idbadapter-1.4/LICENSE
+-rw-rw-rw-   0        0        0      695 2023-05-29 08:37:34.592438 idbadapter-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-05 13:33:15.000000 idbadapter-1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 08:37:34.574439 idbadapter-1.4/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-22 08:18:39.000000 idbadapter-1.4/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0     7838 2023-05-29 08:29:56.000000 idbadapter-1.4/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-05-29 08:37:34.591438 idbadapter-1.4/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      695 2023-05-29 08:37:34.000000 idbadapter-1.4/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-05-29 08:37:34.000000 idbadapter-1.4/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 08:37:34.000000 idbadapter-1.4/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-29 08:37:34.000000 idbadapter-1.4/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-29 08:37:34.000000 idbadapter-1.4/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 08:37:34.593438 idbadapter-1.4/setup.cfg
+-rw-rw-rw-   0        0        0      987 2023-05-29 08:37:15.000000 idbadapter-1.4/setup.py
```

### Comparing `idbadapter-1.3/LICENSE` & `idbadapter-1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.3/PKG-INFO` & `idbadapter-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.3
+Version: 1.4
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.3/idbadapter/schedule_loader.py` & `idbadapter-1.4/idbadapter/schedule_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import requests
 import json
-import urllib.parse
+from urllib.parse import urljoin
 
 class Schedules:
     """Get schedules from database service
     """
     def __init__(self, url):
         """Constructor
         Args:
@@ -66,42 +66,68 @@
             self.objects = list({*self._get_objects_by_resource(), *self._get_objects_by_works()})
             
         if len(self.objects) == 0:
             raise Exception("Objects not found")
         
         return self
            
+    def get_works_names(self, work_type="all"):
+        queries = {
+            "all": "SELECT DISTINCT name FROM works",
+            "granulary": "SELECT DISTINCT name FROM basic_works",
+        }
+        if work_type not in queries:
+            raise ValueError(f"Incorrect work_type argument. {work_type}")
+        
+        data = json.dumps({"body": queries[work_type]})        
+        response = self.session.post(urljoin(self.url, "query/select"), data=data)
+        
+        return [k[0] for k in response.json()]
+        
+    def get_resources_names(self, res_type="all"):
+        queries = {
+            "all": "SELECT DISTINCT name FROM basic_resources",
+            "granulary": "SELECT DISTINCT name FROM basic_resources",
+        }
+        
+        if res_type not in queries:
+            raise ValueError(f"Incorrect res_type argument. {res_type}")
+        
+        data = json.dumps({"body": queries[res_type]})        
+        response = self.session.post(urljoin(self.url, "query/select"), data=data)
+        return [k[0] for k in response.json()]
+    
     def _get_works_ids_by_names(self, work_name_list):
         data = json.dumps(work_name_list)
-        response = self.session.post(urllib.parse.urljoin(self.url, "work/get_basic_works_ids"), data=data)
+        response = self.session.post(urljoin(self.url, "work/get_basic_works_ids"), data=data)
         if "detail" in response.json(): 
             return []
         return response.json()
     
     def _get_resource_ids_by_names(self, resource_names_list):
         if len(resource_names_list) == 0:
             return []
         data = json.dumps(resource_names_list)
-        response = self.session.post(urllib.parse.urljoin(self.url, "resource/get_basic_resource_ids"), data=data)
+        response = self.session.post(urljoin(self.url, "resource/get_basic_resource_ids"), data=data)
         if "detail" in response.json():
             return []
         return response.json()
     
     def _get_objects_by_resource(self):
         if len(self.resource_list) == 0:
             return []
         data = json.dumps(self.resource_list)
-        response = self.session.post(urllib.parse.urljoin(self.url, "resource/schedule_ids"), data=data)
+        response = self.session.post(urljoin(self.url, "resource/schedule_ids"), data=data)
         return response.json()
     
     def _get_objects_by_works(self):
         if len(self.works_list) == 0:
             return []
         data = json.dumps(self.works_list)
-        response = self.session.post(urllib.parse.urljoin(self.url, "work/schedule_ids"), data=data)
+        response = self.session.post(urljoin(self.url, "work/schedule_ids"), data=data)
         return response.json()
    
     def __iter__(self):
         return SchedulesIterator(self.objects, self.session, self.url, self.ceil_limit, self.objects_limit)
 
 
 class SchedulesIterator:
@@ -118,27 +144,27 @@
     def _select_works_from_db(self):
         data = json.dumps({
             "object_id": self.object_slice,
             "start_date": self.start_date,
             "max_work_statuses": self.ceil_limit
         })
 
-        response = self.session.post(urllib.parse.urljoin(self.url, "schedule/works_by_schedule"), data=data)
+        response = self.session.post(urljoin(self.url, "schedule/works_by_schedule"), data=data)
         works = response.json()
         df = pd.DataFrame(works)       
 
         return df
 
     def _select_resources_from_db(self, start_date, finish_date):
         data = json.dumps({
             "object_id": self.object_slice,
             "start_date": start_date,
             "finish_date": finish_date
         })
-        response = self.session.post(urllib.parse.urljoin(self.url, "schedule/resources_by_schedule"), data=data)
+        response = self.session.post(urljoin(self.url, "schedule/resources_by_schedule"), data=data)
         resources = response.json()
 
         df = pd.DataFrame(resources)
         
         return df
     
     def __next__(self):
```

### Comparing `idbadapter-1.3/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.4/idbadapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.3
+Version: 1.4
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.3/setup.py` & `idbadapter-1.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from distutils.core import setup
 
 version = '1.3'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.3',
+      version='1.4',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```


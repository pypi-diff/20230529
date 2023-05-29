# Comparing `tmp/shooju-3.8.8.tar.gz` & `tmp/shooju-3.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shooju-3.8.8.tar", last modified: Wed Jan 25 18:59:56 2023, max compression
+gzip compressed data, was "shooju-3.8.9.tar", last modified: Wed Mar  1 18:25:16 2023, max compression
```

## Comparing `shooju-3.8.8.tar` & `shooju-3.8.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 versh      (502) staff       (20)        0 2023-01-25 18:59:56.787685 shooju-3.8.8/
--rw-r--r--   0 versh      (502) staff       (20)     1022 2017-10-03 11:19:41.000000 shooju-3.8.8/LICENSE
--rw-r--r--   0 versh      (502) staff       (20)       21 2017-10-03 11:19:41.000000 shooju-3.8.8/MANIFEST.in
--rw-r--r--   0 versh      (502) staff       (20)    26678 2023-01-25 18:59:56.787542 shooju-3.8.8/PKG-INFO
--rw-r--r--   0 versh      (502) staff       (20)    21289 2023-01-25 18:53:58.000000 shooju-3.8.8/README.md
--rw-r--r--   0 versh      (502) staff       (20)       38 2023-01-25 18:59:56.787725 shooju-3.8.8/setup.cfg
--rw-r--r--   0 versh      (502) staff       (20)      888 2022-06-30 18:52:26.000000 shooju-3.8.8/setup.py
-drwxr-xr-x   0 versh      (502) staff       (20)        0 2023-01-25 18:59:56.785503 shooju-3.8.8/shooju/
--rw-r--r--   0 versh      (502) staff       (20)    82279 2023-01-25 18:53:58.000000 shooju-3.8.8/shooju/__init__.py
--rw-r--r--   0 versh      (502) staff       (20)     2909 2023-01-25 18:53:58.000000 shooju-3.8.8/shooju/common.py
-drwxr-xr-x   0 versh      (502) staff       (20)        0 2023-01-25 18:59:56.786844 shooju-3.8.8/shooju/hooks/
--rw-r--r--   0 versh      (502) staff       (20)        0 2022-06-30 18:52:26.000000 shooju-3.8.8/shooju/hooks/__init__.py
--rw-r--r--   0 versh      (502) staff       (20)     1551 2022-06-30 18:52:26.000000 shooju-3.8.8/shooju/hooks/base.py
--rw-r--r--   0 versh      (502) staff       (20)     5296 2022-06-30 18:52:26.000000 shooju-3.8.8/shooju/points_serializers.py
-drwxr-xr-x   0 versh      (502) staff       (20)        0 2023-01-25 18:59:56.787144 shooju-3.8.8/shooju/utils/
--rw-r--r--   0 versh      (502) staff       (20)        0 2019-07-24 09:42:22.000000 shooju-3.8.8/shooju/utils/__init__.py
--rw-r--r--   0 versh      (502) staff       (20)      805 2019-07-24 09:42:22.000000 shooju-3.8.8/shooju/utils/convert.py
-drwxr-xr-x   0 versh      (502) staff       (20)        0 2023-01-25 18:59:56.786615 shooju-3.8.8/shooju.egg-info/
--rw-r--r--   0 versh      (502) staff       (20)    26678 2023-01-25 18:59:56.000000 shooju-3.8.8/shooju.egg-info/PKG-INFO
--rw-r--r--   0 versh      (502) staff       (20)      376 2023-01-25 18:59:56.000000 shooju-3.8.8/shooju.egg-info/SOURCES.txt
--rw-r--r--   0 versh      (502) staff       (20)        1 2023-01-25 18:59:56.000000 shooju-3.8.8/shooju.egg-info/dependency_links.txt
--rw-r--r--   0 versh      (502) staff       (20)        2 2016-04-05 13:17:04.000000 shooju-3.8.8/shooju.egg-info/not-zip-safe
--rw-r--r--   0 versh      (502) staff       (20)       28 2023-01-25 18:59:56.000000 shooju-3.8.8/shooju.egg-info/requires.txt
--rw-r--r--   0 versh      (502) staff       (20)        7 2023-01-25 18:59:56.000000 shooju-3.8.8/shooju.egg-info/top_level.txt
+drwxr-xr-x   0 versh      (502) staff       (20)        0 2023-03-01 18:25:16.303604 shooju-3.8.9/
+-rw-r--r--   0 versh      (502) staff       (20)     1022 2017-10-03 11:19:41.000000 shooju-3.8.9/LICENSE
+-rw-r--r--   0 versh      (502) staff       (20)       21 2017-10-03 11:19:41.000000 shooju-3.8.9/MANIFEST.in
+-rw-r--r--   0 versh      (502) staff       (20)    26770 2023-03-01 18:25:16.303465 shooju-3.8.9/PKG-INFO
+-rw-r--r--   0 versh      (502) staff       (20)    21349 2023-03-01 18:24:51.000000 shooju-3.8.9/README.md
+-rw-r--r--   0 versh      (502) staff       (20)       38 2023-03-01 18:25:16.303643 shooju-3.8.9/setup.cfg
+-rw-r--r--   0 versh      (502) staff       (20)      888 2022-06-30 18:52:26.000000 shooju-3.8.9/setup.py
+drwxr-xr-x   0 versh      (502) staff       (20)        0 2023-03-01 18:25:16.301490 shooju-3.8.9/shooju/
+-rw-r--r--   0 versh      (502) staff       (20)    82818 2023-03-01 18:24:51.000000 shooju-3.8.9/shooju/__init__.py
+-rw-r--r--   0 versh      (502) staff       (20)     2909 2023-01-25 18:53:58.000000 shooju-3.8.9/shooju/common.py
+drwxr-xr-x   0 versh      (502) staff       (20)        0 2023-03-01 18:25:16.302621 shooju-3.8.9/shooju/hooks/
+-rw-r--r--   0 versh      (502) staff       (20)        0 2022-06-30 18:52:26.000000 shooju-3.8.9/shooju/hooks/__init__.py
+-rw-r--r--   0 versh      (502) staff       (20)     1551 2022-06-30 18:52:26.000000 shooju-3.8.9/shooju/hooks/base.py
+-rw-r--r--   0 versh      (502) staff       (20)     5296 2022-06-30 18:52:26.000000 shooju-3.8.9/shooju/points_serializers.py
+drwxr-xr-x   0 versh      (502) staff       (20)        0 2023-03-01 18:25:16.303052 shooju-3.8.9/shooju/utils/
+-rw-r--r--   0 versh      (502) staff       (20)        0 2019-07-24 09:42:22.000000 shooju-3.8.9/shooju/utils/__init__.py
+-rw-r--r--   0 versh      (502) staff       (20)      805 2019-07-24 09:42:22.000000 shooju-3.8.9/shooju/utils/convert.py
+drwxr-xr-x   0 versh      (502) staff       (20)        0 2023-03-01 18:25:16.302394 shooju-3.8.9/shooju.egg-info/
+-rw-r--r--   0 versh      (502) staff       (20)    26770 2023-03-01 18:25:16.000000 shooju-3.8.9/shooju.egg-info/PKG-INFO
+-rw-r--r--   0 versh      (502) staff       (20)      376 2023-03-01 18:25:16.000000 shooju-3.8.9/shooju.egg-info/SOURCES.txt
+-rw-r--r--   0 versh      (502) staff       (20)        1 2023-03-01 18:25:16.000000 shooju-3.8.9/shooju.egg-info/dependency_links.txt
+-rw-r--r--   0 versh      (502) staff       (20)        2 2016-04-05 13:17:04.000000 shooju-3.8.9/shooju.egg-info/not-zip-safe
+-rw-r--r--   0 versh      (502) staff       (20)       28 2023-03-01 18:25:16.000000 shooju-3.8.9/shooju.egg-info/requires.txt
+-rw-r--r--   0 versh      (502) staff       (20)        7 2023-03-01 18:25:16.000000 shooju-3.8.9/shooju.egg-info/top_level.txt
```

### Comparing `shooju-3.8.8/LICENSE` & `shooju-3.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `shooju-3.8.8/PKG-INFO` & `shooju-3.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shooju
-Version: 3.8.8
+Version: 3.8.9
 Summary: Official Shooju Client
 Home-page: http://shooju.com
 Author: Serge Aluker
 Author-email: serge@shooju.com
 License: MIT
 Description: # shooju
         
@@ -253,14 +253,18 @@
         To send url parameters, use the `params` argument:
         
             >>> conn.raw.get('/series', params={'series_id': r'user\series\s1'}
         
         
         ## Change log
         
+        **3.8.9**
+        
+        - `Connection.scroll` extra params improvements
+        
         **3.8.8**
         
         - Updated for compatibility with NumPy 1.24
         
         **3.8.7**
         
         - `Connection.scroll` improvements. Now returns a ScrollIterable object which has a `raw_response` property which can also be accessed during iteration
```

### Comparing `shooju-3.8.8/README.md` & `shooju-3.8.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -245,14 +245,18 @@
 To send url parameters, use the `params` argument:
 
     >>> conn.raw.get('/series', params={'series_id': r'user\series\s1'}
 
 
 ## Change log
 
+**3.8.9**
+
+- `Connection.scroll` extra params improvements
+
 **3.8.8**
 
 - Updated for compatibility with NumPy 1.24
 
 **3.8.7**
 
 - `Connection.scroll` improvements. Now returns a ScrollIterable object which has a `raw_response` property which can also be accessed during iteration
```

### Comparing `shooju-3.8.8/setup.py` & `shooju-3.8.9/setup.py`

 * *Files identical despite different names*

### Comparing `shooju-3.8.8/shooju/__init__.py` & `shooju-3.8.9/shooju/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from .hooks.base import Request, Response, BaseHook
 from .points_serializers import shooju_point, NANOSECONDS, Point, milli_tuple
 from .common import *
 import requests
 from itertools import cycle
 
-__version__ = '3.8.8'
+__version__ = '3.8.9'
 
 if NUMPY_INSTALLED:
     from .points_serializers import np_array
 
 if PANDAS_INSTALLED:
     from .points_serializers import pd_series, pd_series_localized
 
@@ -279,14 +279,17 @@
                                                                     scroll=scroll,
                                                                     batch_size=self._batch_size if scroll else None,
                                                                     sort=self._sort,
                                                                     deserialize_response_to_numpy=deserialize_response_to_numpy,
                                                                     url_params=self._extra_params,
                                                                     per_page=self._max_series if not scroll else None)
 
+            self._included_job = self.raw_response.get('included_job', False)
+            self._included_timestamp = self.raw_response.get('included_timestamp', False)
+
             if self._assert_under_max_series and\
                     self._max_series is not None and\
                     self._max_series < self.raw_response['total']:
                 raise ValueError(f'Expected <= {self._max_series} series, got {self.raw_response["total"]}')
 
             self._scroll_id = self.raw_response.get('scroll_id') if scroll else None
             self._series_left = min(self._max_series, self.raw_response['total']) \
@@ -294,35 +297,39 @@
 
         def __iter__(self):
             while self._series_left > 0:
                 if not self.raw_response['series']:
                     break
                 if not options.return_series_errors:
                     _check_bulk_api_errors(self.raw_response['series'])
-                for s in self._process_search_response(self.raw_response, self._serializer, self._series_left):
+                for s in self._process_search_response(self.raw_response, self._serializer, self._series_left,
+                                                       self._included_job, self._included_timestamp):
                     yield s
                 self._series_left -= len(self.raw_response['series'])
                 if self._series_left > 0:
                     self.raw_response = self._conn.shooju_api.scroll_series(self._scroll_id)
 
-        def _process_search_response(self, data, serializer, series_left):
+        def _process_search_response(self, data, serializer, series_left, included_job, included_timestamp):
             """
             Helper method to convert a api series search response to the module data structures
             :param data: api series response
             :param serializer: points serializer function; use one of shooju.points_serializers.*
             :param series_left: limit for this request
+            :param included_job: include historical job
+            :param included_timestamp: include historical timestamp
             :return: array of series objects
             :rtype: list
             """
             results = list()
             counter = 0
             for s in data['series']:
                 s.setdefault('fields', {})
                 if 'points' in s:
-                    s['points'] = serializer(s['points'], tz=self._conn._extract_series_tz(s))
+                    s['points'] = serializer(s['points'], tz=self._conn._extract_series_tz(s),
+                                             included_job=included_job, included_timestamp=included_timestamp)
                 results.append(s)
                 counter += 1
                 if counter == series_left:
                     break
             return results
 
     def scroll(self, query='', fields=None, df=None, dt=None, max_points=0,
```

### Comparing `shooju-3.8.8/shooju/common.py` & `shooju-3.8.9/shooju/common.py`

 * *Files identical despite different names*

### Comparing `shooju-3.8.8/shooju/hooks/base.py` & `shooju-3.8.9/shooju/hooks/base.py`

 * *Files identical despite different names*

### Comparing `shooju-3.8.8/shooju/points_serializers.py` & `shooju-3.8.9/shooju/points_serializers.py`

 * *Files identical despite different names*

### Comparing `shooju-3.8.8/shooju/utils/convert.py` & `shooju-3.8.9/shooju/utils/convert.py`

 * *Files identical despite different names*

### Comparing `shooju-3.8.8/shooju.egg-info/PKG-INFO` & `shooju-3.8.9/shooju.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shooju
-Version: 3.8.8
+Version: 3.8.9
 Summary: Official Shooju Client
 Home-page: http://shooju.com
 Author: Serge Aluker
 Author-email: serge@shooju.com
 License: MIT
 Description: # shooju
         
@@ -253,14 +253,18 @@
         To send url parameters, use the `params` argument:
         
             >>> conn.raw.get('/series', params={'series_id': r'user\series\s1'}
         
         
         ## Change log
         
+        **3.8.9**
+        
+        - `Connection.scroll` extra params improvements
+        
         **3.8.8**
         
         - Updated for compatibility with NumPy 1.24
         
         **3.8.7**
         
         - `Connection.scroll` improvements. Now returns a ScrollIterable object which has a `raw_response` property which can also be accessed during iteration
```


# Comparing `tmp/datatable-ajax-request-parser-1.0.2.tar.gz` & `tmp/datatable-ajax-request-parser-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatable-ajax-request-parser-1.0.2.tar", last modified: Mon May 29 07:15:33 2023, max compression
+gzip compressed data, was "datatable-ajax-request-parser-1.0.3.tar", last modified: Mon May 29 14:48:15 2023, max compression
```

## Comparing `datatable-ajax-request-parser-1.0.2.tar` & `datatable-ajax-request-parser-1.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 07:15:33.196290 datatable-ajax-request-parser-1.0.2/
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1067 2023-05-27 04:34:24.000000 datatable-ajax-request-parser-1.0.2/LICENCE
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 07:15:33.196351 datatable-ajax-request-parser-1.0.2/PKG-INFO
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5157 2023-05-29 07:14:50.000000 datatable-ajax-request-parser-1.0.2/README.md
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 07:15:33.195493 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/
--rw-r--r--   0 yapzhihon   (501) staff       (20)        0 2023-05-26 16:26:39.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/__init__.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)      946 2023-05-29 02:51:56.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/dataclasses.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     3801 2023-05-29 06:45:13.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/django_extension.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     2990 2023-05-27 04:18:44.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/parser.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5381 2023-05-29 06:45:13.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/test_django_extension.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     6750 2023-05-29 02:38:27.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/test_parser.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1035 2023-05-29 02:38:32.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/utils.py
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 07:15:33.196175 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 07:15:33.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/PKG-INFO
--rw-r--r--   0 yapzhihon   (501) staff       (20)      616 2023-05-29 07:15:33.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/SOURCES.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)        1 2023-05-29 07:15:33.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/dependency_links.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       24 2023-05-29 07:15:33.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/requires.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       30 2023-05-29 07:15:33.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/top_level.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       79 2023-05-29 07:15:33.196640 datatable-ajax-request-parser-1.0.2/setup.cfg
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1148 2023-05-29 07:15:17.000000 datatable-ajax-request-parser-1.0.2/setup.py
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 14:48:15.030539 datatable-ajax-request-parser-1.0.3/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1067 2023-05-27 04:34:24.000000 datatable-ajax-request-parser-1.0.3/LICENCE
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 14:48:15.030604 datatable-ajax-request-parser-1.0.3/PKG-INFO
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5157 2023-05-29 07:14:50.000000 datatable-ajax-request-parser-1.0.3/README.md
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 14:48:15.029792 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)        0 2023-05-26 16:26:39.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/__init__.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)      946 2023-05-29 02:51:56.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/dataclasses.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     3694 2023-05-29 14:29:57.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/django_extension.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     2990 2023-05-27 04:18:44.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/parser.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     6870 2023-05-29 14:28:30.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/test_django_extension.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     6750 2023-05-29 02:38:27.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/test_parser.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1035 2023-05-29 14:28:56.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/utils.py
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 14:48:15.030426 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 14:48:14.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/PKG-INFO
+-rw-r--r--   0 yapzhihon   (501) staff       (20)      616 2023-05-29 14:48:15.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)        1 2023-05-29 14:48:14.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       24 2023-05-29 14:48:14.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/requires.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       30 2023-05-29 14:48:14.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/top_level.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       79 2023-05-29 14:48:15.030919 datatable-ajax-request-parser-1.0.3/setup.cfg
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1148 2023-05-29 14:30:56.000000 datatable-ajax-request-parser-1.0.3/setup.py
```

### Comparing `datatable-ajax-request-parser-1.0.2/LICENCE` & `datatable-ajax-request-parser-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.2/PKG-INFO` & `datatable-ajax-request-parser-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-ajax-request-parser
-Version: 1.0.2
+Version: 1.0.3
 Summary: Helper function to parse ajax datatable request into usable dictionary
 Home-page: https://github.com/ziiiio/datatable_ajax_request_parser.git
 Author: Yap ZhiHon
 Author-email: y.zhihon@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `datatable-ajax-request-parser-1.0.2/README.md` & `datatable-ajax-request-parser-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/dataclasses.py` & `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/dataclasses.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/django_extension.py` & `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/django_extension.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,43 +41,41 @@
             if order.direction == 'desc':
                 db_column = '-' + db_column
 
             order_list.append(db_column)
 
         return order_list
 
-    def get_db_query_filter(self, mapping_dict: dict = None):
+    def get_db_query_filter(self, return_as_list_of_dicts: bool = False):
         filters = []
 
         for column in self.columns:
-            query_filter = Q()
-
-            if not column.searchable or (mapping_dict and column.data not in mapping_dict):
+            if not column.searchable:
                 continue
 
             col_name = column.data
 
             if self.search_regex:
-                query_filter |= Q(**{col_name + '__iregex': fr"{self.search_value}"})
+                filters.append({col_name + '__iregex': fr"{self.search_value}"})
             elif self.search_value:
-                query_filter |= Q(**{col_name + '__icontains': self.search_value})
+                filters.append({col_name + '__icontains': self.search_value})
 
             if not column.search_value:
-                filters.append(query_filter)
                 continue
 
             column_key = col_name + '__iregex' if column.search_is_regex else col_name + '__icontains'
 
-            query_filter |= Q(**{column_key: column.search_value})
+            filters.append({column_key: column.search_value})
 
-            filters.append(query_filter)
+        if return_as_list_of_dicts:
+            return filters
 
         final_query = Q()
         for _filter in filters:
-            final_query |= _filter
+            final_query |= Q(**_filter)
 
         return final_query
 
 
 @dataclass
 class DjangoDTResponse(DTResponse):
```

### Comparing `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/parser.py` & `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/parser.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/test_django_extension.py` & `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/test_django_extension.py`

 * *Files 18% similar despite different names*

```diff
@@ -71,14 +71,46 @@
                           Q(username__icontains='jjj') | \
                           Q(username__iregex='1234') | \
                           Q(type__icontains='jjj') | \
                           Q(type__icontains='hshs')
 
         assert_q_equal(result, expected_result)
 
+    def test_query_filter_get_dicts(self):
+        parsed_request = {
+            'draw': '1',
+            'columns': {
+                '0': {'data': 'hostname', 'name': '', 'searchable': 'true', 'orderable': 'true',
+                      'search': {'value': 'abc', 'regex': 'true'}},
+                '1': {'data': 'ip_address', 'name': '', 'searchable': 'true', 'orderable': 'true',
+                      'search': {'value': '', 'regex': 'false'}},
+                '2': {'data': 'username', 'name': '', 'searchable': 'true', 'orderable': 'true',
+                      'search': {'value': '1234', 'regex': 'true'}},
+                '3': {'data': 'type', 'name': '', 'searchable': 'true', 'orderable': 'true',
+                      'search': {'value': 'hshs', 'regex': 'false'}}
+            },
+            'order': {'0': {'column': '0', 'dir': 'asc'}},
+            'start': '0', 'length': '10',
+            'search': {'value': 'jjj', 'regex': 'false'},
+            '_': '1672804547475'
+        }
+
+        parsed_request = DjangoDTRequest(parsed_dict=parsed_request)
+
+        result = parsed_request.get_db_query_filter(return_as_list_of_dicts=True)
+
+        expected_result = [
+            {'hostname__icontains': 'jjj'}, {'hostname__iregex': 'abc'}, {'ip_address__icontains': 'jjj'},
+            {'username__icontains': 'jjj'}, {'username__iregex': '1234'}, {'type__icontains': 'jjj'},
+            {'type__icontains': 'hshs'}
+        ]
+
+        self.assertEqual(result, expected_result)
+
+
     def test_get_dt_response(self):
         parsed_request = get_django_datatable_query(self.sample_datatable_ajax_request)
 
         count_result = 12
         filter_result = [1, 2, 3, 4, 5]
         error = 'some error'
```

### Comparing `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/test_parser.py` & `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/utils.py` & `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/utils.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/PKG-INFO` & `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-ajax-request-parser
-Version: 1.0.2
+Version: 1.0.3
 Summary: Helper function to parse ajax datatable request into usable dictionary
 Home-page: https://github.com/ziiiio/datatable_ajax_request_parser.git
 Author: Yap ZhiHon
 Author-email: y.zhihon@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/SOURCES.txt` & `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.2/setup.py` & `datatable-ajax-request-parser-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="datatable-ajax-request-parser",
-    version="1.0.2",
+    version="1.0.3",
     description="Helper function to parse ajax datatable request into usable dictionary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yap ZhiHon",
     author_email="y.zhihon@gmail.com",
     url="https://github.com/ziiiio/datatable_ajax_request_parser.git",
     classifiers=[
```


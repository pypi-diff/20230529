# Comparing `tmp/datatable-ajax-request-parser-1.0.3.tar.gz` & `tmp/datatable-ajax-request-parser-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatable-ajax-request-parser-1.0.3.tar", last modified: Mon May 29 14:48:15 2023, max compression
+gzip compressed data, was "datatable-ajax-request-parser-1.0.4.tar", last modified: Mon May 29 15:30:56 2023, max compression
```

## Comparing `datatable-ajax-request-parser-1.0.3.tar` & `datatable-ajax-request-parser-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 14:48:15.030539 datatable-ajax-request-parser-1.0.3/
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1067 2023-05-27 04:34:24.000000 datatable-ajax-request-parser-1.0.3/LICENCE
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 14:48:15.030604 datatable-ajax-request-parser-1.0.3/PKG-INFO
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5157 2023-05-29 07:14:50.000000 datatable-ajax-request-parser-1.0.3/README.md
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 14:48:15.029792 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/
--rw-r--r--   0 yapzhihon   (501) staff       (20)        0 2023-05-26 16:26:39.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/__init__.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)      946 2023-05-29 02:51:56.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/dataclasses.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     3694 2023-05-29 14:29:57.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/django_extension.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     2990 2023-05-27 04:18:44.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/parser.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     6870 2023-05-29 14:28:30.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/test_django_extension.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     6750 2023-05-29 02:38:27.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/test_parser.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1035 2023-05-29 14:28:56.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/utils.py
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 14:48:15.030426 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 14:48:14.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/PKG-INFO
--rw-r--r--   0 yapzhihon   (501) staff       (20)      616 2023-05-29 14:48:15.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/SOURCES.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)        1 2023-05-29 14:48:14.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/dependency_links.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       24 2023-05-29 14:48:14.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/requires.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       30 2023-05-29 14:48:14.000000 datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/top_level.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       79 2023-05-29 14:48:15.030919 datatable-ajax-request-parser-1.0.3/setup.cfg
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1148 2023-05-29 14:30:56.000000 datatable-ajax-request-parser-1.0.3/setup.py
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 15:30:56.366571 datatable-ajax-request-parser-1.0.4/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1067 2023-05-27 04:34:24.000000 datatable-ajax-request-parser-1.0.4/LICENCE
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 15:30:56.366624 datatable-ajax-request-parser-1.0.4/PKG-INFO
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5157 2023-05-29 07:14:50.000000 datatable-ajax-request-parser-1.0.4/README.md
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 15:30:56.365864 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)        0 2023-05-26 16:26:39.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/__init__.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1096 2023-05-29 15:27:44.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/dataclasses.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     3591 2023-05-29 15:29:54.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/django_extension.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     2990 2023-05-27 04:18:44.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/parser.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     6043 2023-05-29 15:29:06.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/test_django_extension.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     6750 2023-05-29 02:38:27.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/test_parser.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1035 2023-05-29 14:28:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/utils.py
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 15:30:56.366463 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 15:30:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/PKG-INFO
+-rw-r--r--   0 yapzhihon   (501) staff       (20)      616 2023-05-29 15:30:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)        1 2023-05-29 15:30:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       24 2023-05-29 15:30:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/requires.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       30 2023-05-29 15:30:56.000000 datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/top_level.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       79 2023-05-29 15:30:56.366887 datatable-ajax-request-parser-1.0.4/setup.cfg
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1148 2023-05-29 15:30:37.000000 datatable-ajax-request-parser-1.0.4/setup.py
```

### Comparing `datatable-ajax-request-parser-1.0.3/LICENCE` & `datatable-ajax-request-parser-1.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.3/PKG-INFO` & `datatable-ajax-request-parser-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-ajax-request-parser
-Version: 1.0.3
+Version: 1.0.4
 Summary: Helper function to parse ajax datatable request into usable dictionary
 Home-page: https://github.com/ziiiio/datatable_ajax_request_parser.git
 Author: Yap ZhiHon
 Author-email: y.zhihon@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `datatable-ajax-request-parser-1.0.3/README.md` & `datatable-ajax-request-parser-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/dataclasses.py` & `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/dataclasses.py`

 * *Files 10% similar despite different names*

```diff
@@ -37,14 +37,20 @@
     start: int
     length: int
     search_value: str
     search_regex: bool
     columns: List[DTColumn]
     order: List[DTOrder]
 
+    def get_page_number(self) -> int:
+        return (self.start // self.length) + 1
+
+    def get_page_size(self) -> int:
+        return self.length
+
 
 @dataclass
 class DTResponse(DictHelperMixin):
     draw: int
     records_total: int
     records_filtered: int
     data: dict
```

### Comparing `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/django_extension.py` & `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/django_extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,26 +21,24 @@
         if parsed_dict:
             kwargs.update(add_typings_to_dict(parsed_dict))
 
         super().__init__(*args, **kwargs)
 
     # pass mapping dict in if you are not ordering based on the model
     # example: annotations, aggregations
-    def get_order_by(self, mapping_dict: dict = None):
+    def get_order_by(self):
         order_list = []
 
         for order in self.order:
             order_index = order.column
 
             if 0 > order_index or order_index >= len(self.columns):
                 continue
 
             db_column = self.columns[order_index].data
-            if mapping_dict and mapping_dict.get(db_column):
-                db_column = mapping_dict.get(db_column)
 
             if order.direction == 'desc':
                 db_column = '-' + db_column
 
             order_list.append(db_column)
 
         return order_list
@@ -99,21 +97,21 @@
                            error: str = None) -> DjangoDTResponse:
     draw = parsed_dt_query.draw
     offset = parsed_dt_query.start
     limit = parsed_dt_query.length
     order_by = parsed_dt_query.get_order_by()
     search = parsed_dt_query.get_db_query_filter()
 
+    total_count = model_class.objects.count()
     query_set = model_class.objects.filter(search).order_by(*order_by)
-
     query_set_count = query_set.count()
 
     filtered_set = query_set[offset:offset + limit]
 
     result = {
         "data": data_function(filtered_set),
-        "records_total": query_set_count,
+        "records_total": total_count,
         "records_filtered": query_set_count,
         "draw": draw,
         "error": error
     }
     return DjangoDTResponse(**result)
```

### Comparing `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/parser.py` & `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/parser.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/test_django_extension.py` & `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/test_django_extension.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,30 +24,15 @@
                                              'Bsearch%5D%5Bvalue%5D=&columns%5B2%5D%5Bsearch%5D%5Bregex%5D=false&' \
                                              'columns%5B3%5D%5Bdata%5D=type&columns%5B3%5D%5Bname%5D=&columns%5B3' \
                                              '%5D%5Bsearchable%5D=true&columns%5B3%5D%5Borderable%5D=true&columns' \
                                              '%5B3%5D%5Bsearch%5D%5Bvalue%5D=&columns%5B3%5D%5Bsearch%5D%5Bregex%' \
                                              '5D=false&order%5B0%5D%5Bcolumn%5D=0&order%5B0%5D%5Bdir%5D=asc&start' \
                                              '=0&length=10&search%5Bvalue%5D=&search%5Bregex%5D=false&_=1672804547475'
 
-    def test_get_order_by(self):
-        parsed_request = get_django_datatable_query(self.sample_datatable_ajax_request)
-
-        result = parsed_request.get_order_by()
-
-        self.assertEqual(result, ['hostname'])
-
-        parsed_request.order[0].direction = 'desc'
-
-        result = parsed_request.get_order_by()
-
-        self.assertEqual(result, ['-hostname'])
-
-    # @skip("Test will fail, but the function should return the expected result")
-    def test_query_filter(self):
-        parsed_request = {
+        self.parsed_request = {
             'draw': '1',
             'columns': {
                 '0': {'data': 'hostname', 'name': '', 'searchable': 'true', 'orderable': 'true',
                       'search': {'value': 'abc', 'regex': 'true'}},
                 '1': {'data': 'ip_address', 'name': '', 'searchable': 'true', 'orderable': 'true',
                       'search': {'value': '', 'regex': 'false'}},
                 '2': {'data': 'username', 'name': '', 'searchable': 'true', 'orderable': 'true',
@@ -57,48 +42,45 @@
             },
             'order': {'0': {'column': '0', 'dir': 'asc'}},
             'start': '0', 'length': '10',
             'search': {'value': 'jjj', 'regex': 'false'},
             '_': '1672804547475'
         }
 
-        parsed_request = DjangoDTRequest(parsed_dict=parsed_request)
+    def test_get_order_by(self):
+        parsed_request = get_django_datatable_query(self.sample_datatable_ajax_request)
+
+        result = parsed_request.get_order_by()
+
+        self.assertEqual(result, ['hostname'])
+
+        parsed_request.order[0].direction = 'desc'
+
+        result = parsed_request.get_order_by()
+
+        self.assertEqual(result, ['-hostname'])
+
+    # @skip("Test will fail, but the function should return the expected result")
+    def test_query_filter(self):
+        parsed_request = DjangoDTRequest(parsed_dict=self.parsed_request)
 
         result = parsed_request.get_db_query_filter()
 
         expected_result = Q(hostname__icontains='jjj') | \
                           Q(hostname__iregex='abc') | \
                           Q(ip_address__icontains='jjj') | \
                           Q(username__icontains='jjj') | \
                           Q(username__iregex='1234') | \
                           Q(type__icontains='jjj') | \
                           Q(type__icontains='hshs')
 
         assert_q_equal(result, expected_result)
 
     def test_query_filter_get_dicts(self):
-        parsed_request = {
-            'draw': '1',
-            'columns': {
-                '0': {'data': 'hostname', 'name': '', 'searchable': 'true', 'orderable': 'true',
-                      'search': {'value': 'abc', 'regex': 'true'}},
-                '1': {'data': 'ip_address', 'name': '', 'searchable': 'true', 'orderable': 'true',
-                      'search': {'value': '', 'regex': 'false'}},
-                '2': {'data': 'username', 'name': '', 'searchable': 'true', 'orderable': 'true',
-                      'search': {'value': '1234', 'regex': 'true'}},
-                '3': {'data': 'type', 'name': '', 'searchable': 'true', 'orderable': 'true',
-                      'search': {'value': 'hshs', 'regex': 'false'}}
-            },
-            'order': {'0': {'column': '0', 'dir': 'asc'}},
-            'start': '0', 'length': '10',
-            'search': {'value': 'jjj', 'regex': 'false'},
-            '_': '1672804547475'
-        }
-
-        parsed_request = DjangoDTRequest(parsed_dict=parsed_request)
+        parsed_request = DjangoDTRequest(parsed_dict=self.parsed_request)
 
         result = parsed_request.get_db_query_filter(return_as_list_of_dicts=True)
 
         expected_result = [
             {'hostname__icontains': 'jjj'}, {'hostname__iregex': 'abc'}, {'ip_address__icontains': 'jjj'},
             {'username__icontains': 'jjj'}, {'username__iregex': '1234'}, {'type__icontains': 'jjj'},
             {'type__icontains': 'hshs'}
@@ -107,38 +89,40 @@
         self.assertEqual(result, expected_result)
 
 
     def test_get_dt_response(self):
         parsed_request = get_django_datatable_query(self.sample_datatable_ajax_request)
 
         count_result = 12
+        total_result = 120
         filter_result = [1, 2, 3, 4, 5]
         error = 'some error'
 
         count_mock = mock.MagicMock()
         count_mock.__getitem__.return_value = filter_result
         count_mock.count.return_value = count_result
 
         order_mock = mock.Mock()
         order_mock.order_by.return_value = count_mock
 
-        filter_mock = mock.Mock()
-        filter_mock.filter.return_value = order_mock
+        filter_count_mock = mock.Mock()
+        filter_count_mock.filter.return_value = order_mock
+        filter_count_mock.count.return_value = total_result
 
         model_class_mock = mock.Mock()
-        model_class_mock.objects = filter_mock
+        model_class_mock.objects = filter_count_mock
 
         result = get_django_dt_response(parsed_request, model_class_mock, lambda x: x, error)
 
         results_transformed = result.convert_to_dt_response_dict()
 
         expected_result = {
             'data': filter_result,
-            'recordsTotal': count_result,
+            'recordsTotal': total_result,
             'recordsFiltered': count_result,
             'draw': parsed_request.draw,
             'error': error
         }
 
         self.assertEqual(expected_result, results_transformed)
-        filter_mock.filter.assert_called_with(parsed_request.get_db_query_filter())
+        filter_count_mock.filter.assert_called_with(parsed_request.get_db_query_filter())
         order_mock.order_by.assert_called_with(*parsed_request.get_order_by())
```

### Comparing `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/test_parser.py` & `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser/utils.py` & `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser/utils.py`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/PKG-INFO` & `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatable-ajax-request-parser
-Version: 1.0.3
+Version: 1.0.4
 Summary: Helper function to parse ajax datatable request into usable dictionary
 Home-page: https://github.com/ziiiio/datatable_ajax_request_parser.git
 Author: Yap ZhiHon
 Author-email: y.zhihon@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `datatable-ajax-request-parser-1.0.3/datatable_ajax_request_parser.egg-info/SOURCES.txt` & `datatable-ajax-request-parser-1.0.4/datatable_ajax_request_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatable-ajax-request-parser-1.0.3/setup.py` & `datatable-ajax-request-parser-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="datatable-ajax-request-parser",
-    version="1.0.3",
+    version="1.0.4",
     description="Helper function to parse ajax datatable request into usable dictionary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yap ZhiHon",
     author_email="y.zhihon@gmail.com",
     url="https://github.com/ziiiio/datatable_ajax_request_parser.git",
     classifiers=[
```


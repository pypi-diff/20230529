# Comparing `tmp/datatable_ajax_request_parser-1.0.0.tar.gz` & `tmp/datatable_ajax_request_parser-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatable_ajax_request_parser-1.0.0.tar", last modified: Sat May 27 04:40:13 2023, max compression
+gzip compressed data, was "datatable_ajax_request_parser-1.0.1.tar", last modified: Mon May 29 06:46:50 2023, max compression
```

## Comparing `datatable_ajax_request_parser-1.0.0.tar` & `datatable_ajax_request_parser-1.0.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-27 04:40:13.478684 datatable_ajax_request_parser-1.0.0/
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1067 2023-05-27 04:34:24.000000 datatable_ajax_request_parser-1.0.0/LICENCE
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5029 2023-05-27 04:40:13.478744 datatable_ajax_request_parser-1.0.0/PKG-INFO
--rw-r--r--   0 yapzhihon   (501) staff       (20)     4667 2023-05-27 04:30:10.000000 datatable_ajax_request_parser-1.0.0/README.md
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-27 04:40:13.477796 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/
--rw-r--r--   0 yapzhihon   (501) staff       (20)        0 2023-05-26 16:26:39.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/__init__.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)      805 2023-05-26 18:33:44.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/dataclasses.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     2533 2023-05-27 04:18:44.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/django_extension.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     2990 2023-05-27 04:18:44.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/parser.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     4271 2023-05-27 04:30:10.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/test_django_extension.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     6750 2023-05-27 02:48:20.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/test_parser.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1035 2023-05-27 04:12:23.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/utils.py
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-27 04:40:13.478576 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser.egg-info/
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5029 2023-05-27 04:40:13.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser.egg-info/PKG-INFO
--rw-r--r--   0 yapzhihon   (501) staff       (20)      616 2023-05-27 04:40:13.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser.egg-info/SOURCES.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)        1 2023-05-27 04:40:13.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser.egg-info/dependency_links.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       24 2023-05-27 04:40:13.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser.egg-info/requires.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       30 2023-05-27 04:40:13.000000 datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser.egg-info/top_level.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       79 2023-05-27 04:40:13.479036 datatable_ajax_request_parser-1.0.0/setup.cfg
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1077 2023-05-26 16:45:04.000000 datatable_ajax_request_parser-1.0.0/setup.py
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 06:46:50.132918 datatable_ajax_request_parser-1.0.1/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1067 2023-05-27 04:34:24.000000 datatable_ajax_request_parser-1.0.1/LICENCE
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5519 2023-05-29 06:46:50.133055 datatable_ajax_request_parser-1.0.1/PKG-INFO
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5157 2023-05-29 06:44:34.000000 datatable_ajax_request_parser-1.0.1/README.md
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 06:46:50.132001 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)        0 2023-05-26 16:26:39.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/__init__.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)      946 2023-05-29 02:51:56.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/dataclasses.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     3801 2023-05-29 06:45:13.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/django_extension.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     2990 2023-05-27 04:18:44.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/parser.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5381 2023-05-29 06:45:13.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/test_django_extension.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     6750 2023-05-29 02:38:27.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/test_parser.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1035 2023-05-29 02:38:32.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/utils.py
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 06:46:50.132723 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5519 2023-05-29 06:46:50.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/PKG-INFO
+-rw-r--r--   0 yapzhihon   (501) staff       (20)      616 2023-05-29 06:46:50.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)        1 2023-05-29 06:46:50.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       24 2023-05-29 06:46:50.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/requires.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       30 2023-05-29 06:46:50.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/top_level.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       79 2023-05-29 06:46:50.133542 datatable_ajax_request_parser-1.0.1/setup.cfg
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1077 2023-05-29 06:44:34.000000 datatable_ajax_request_parser-1.0.1/setup.py
```

### Comparing `datatable_ajax_request_parser-1.0.0/LICENCE` & `datatable_ajax_request_parser-1.0.1/LICENCE`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.0/PKG-INFO` & `datatable_ajax_request_parser-1.0.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: datatable_ajax_request_parser
-Version: 1.0.0
-Summary: Helper function to parse ajax datatable request into usable dictionary
-Author: Yap ZhiHon
-Author-email: y.zhihon@gmail.com
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-Provides-Extra: Django
-License-File: LICENCE
-
 # Python Ajax Datatable Request Parser
 
 This is a small package to help with parsing datatable requests
 
 
 ## Installation
 simply do a `pip install datatable_ajax_request_parser`
@@ -107,10 +95,24 @@
 
 ```python
 from datatable_ajax_request_parser.django_extension import DjangoDTRequest
 
 DjangoDTRequest(parsed_dict=parsed_request)
 ```
 
+If you need a response, there is a `DjangoDTResponse` helper class available to help parse into datatable-compliant format
+
+```python
+from datatable_ajax_request_parser.django_extension get_django_dt_response
+
+parsed_query = get_django_datatable_query(sample_url)
+get_django_dt_response(parsed_query, <your model class>, <your function to process the data>, <your error>)
+
+```
+
+
 ## Footnote
 
 Feel free to submit any PRs for improvements
+
+## Credits
+I did not write everything by myself, I thank Lim Yong Soon for providing much of the useful code.
```

### Comparing `datatable_ajax_request_parser-1.0.0/README.md` & `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: datatable-ajax-request-parser
+Version: 1.0.1
+Summary: Helper function to parse ajax datatable request into usable dictionary
+Author: Yap ZhiHon
+Author-email: y.zhihon@gmail.com
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+Provides-Extra: Django
+License-File: LICENCE
+
 # Python Ajax Datatable Request Parser
 
 This is a small package to help with parsing datatable requests
 
 
 ## Installation
 simply do a `pip install datatable_ajax_request_parser`
@@ -95,10 +107,24 @@
 
 ```python
 from datatable_ajax_request_parser.django_extension import DjangoDTRequest
 
 DjangoDTRequest(parsed_dict=parsed_request)
 ```
 
+If you need a response, there is a `DjangoDTResponse` helper class available to help parse into datatable-compliant format
+
+```python
+from datatable_ajax_request_parser.django_extension get_django_dt_response
+
+parsed_query = get_django_datatable_query(sample_url)
+get_django_dt_response(parsed_query, <your model class>, <your function to process the data>, <your error>)
+
+```
+
+
 ## Footnote
 
 Feel free to submit any PRs for improvements
+
+## Credits
+I did not write everything by myself, I thank Lim Yong Soon for providing much of the useful code.
```

### Comparing `datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/dataclasses.py` & `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/dataclasses.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,7 +36,16 @@
     draw: int
     start: int
     length: int
     search_value: str
     search_regex: bool
     columns: List[DTColumn]
     order: List[DTOrder]
+
+
+@dataclass
+class DTResponse(DictHelperMixin):
+    draw: int
+    records_total: int
+    records_filtered: int
+    data: dict
+    error: str
```

### Comparing `datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/parser.py` & `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/parser.py`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/test_django_extension.py` & `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/test_django_extension.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,18 @@
 from django.db.models import Q
 from django.test import TestCase
 
-from datatable_ajax_request_parser.django_extension import DjangoDTRequest, get_django_datatable_query
+from datatable_ajax_request_parser.django_extension import (
+    DjangoDTRequest, get_django_datatable_query,
+    get_django_dt_response
+)
 from datatable_ajax_request_parser.utils import assert_q_equal
 
+from unittest import mock
+
 
 class DjangoAjaxRequestTestCase(TestCase):
     def setUp(self):
         self.sample_datatable_ajax_request = 'http://somedomain/?draw=1&columns%5B0%5D%5Bdata%5D=hostname&columns' \
                                              '%5B0%5D%5Bname%5D=&columns%5B0%5D%5Bsearchable%5D=true&columns%5B0%' \
                                              '5D%5Borderable%5D=true&columns%5B0%5D%5Bsearch%5D%5Bvalue%5D=&colum' \
                                              'ns%5B0%5D%5Bsearch%5D%5Bregex%5D=false&columns%5B1%5D%5Bdata%5D=ip_' \
@@ -56,26 +61,52 @@
             '_': '1672804547475'
         }
 
         parsed_request = DjangoDTRequest(parsed_dict=parsed_request)
 
         result = parsed_request.get_db_query_filter()
 
-        # (OR: ('hostname__icontains', 'jjj'),
-        # ('hostname__iregex', 'abc'),
-        # ('ip_address__icontains', 'jjj'),
-        # ('username__icontains', 'jjj'),
-        # ('username__iregex', '1234'),
-        # ('type__icontains', 'jjj'),
-        # ('type__icontains', 'hshs'))
-
         expected_result = Q(hostname__icontains='jjj') | \
-            Q(hostname__iregex='abc') | \
-            Q(ip_address__icontains='jjj') | \
-            Q(username__icontains='jjj') | \
-            Q(username__iregex='1234') | \
-            Q(type__icontains='jjj') | \
-            Q(type__icontains='hshs')
+                          Q(hostname__iregex='abc') | \
+                          Q(ip_address__icontains='jjj') | \
+                          Q(username__icontains='jjj') | \
+                          Q(username__iregex='1234') | \
+                          Q(type__icontains='jjj') | \
+                          Q(type__icontains='hshs')
 
         assert_q_equal(result, expected_result)
 
+    def test_get_dt_response(self):
+        parsed_request = get_django_datatable_query(self.sample_datatable_ajax_request)
+
+        count_result = 12
+        filter_result = [1, 2, 3, 4, 5]
+        error = 'some error'
+
+        count_mock = mock.MagicMock()
+        count_mock.__getitem__.return_value = filter_result
+        count_mock.count.return_value = count_result
+
+        order_mock = mock.Mock()
+        order_mock.order_by.return_value = count_mock
+
+        filter_mock = mock.Mock()
+        filter_mock.filter.return_value = order_mock
+
+        model_class_mock = mock.Mock()
+        model_class_mock.objects = filter_mock
+
+        result = get_django_dt_response(parsed_request, model_class_mock, lambda x: x, error)
+
+        results_transformed = result.convert_to_dt_response_dict()
+
+        expected_result = {
+            'data': filter_result,
+            'recordsTotal': count_result,
+            'recordsFiltered': count_result,
+            'draw': parsed_request.draw,
+            'error': error
+        }
 
+        self.assertEqual(expected_result, results_transformed)
+        filter_mock.filter.assert_called_with(parsed_request.get_db_query_filter())
+        order_mock.order_by.assert_called_with(*parsed_request.get_order_by())
```

### Comparing `datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/test_parser.py` & `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser/utils.py` & `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/utils.py`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser.egg-info/PKG-INFO` & `datatable_ajax_request_parser-1.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: datatable-ajax-request-parser
-Version: 1.0.0
+Name: datatable_ajax_request_parser
+Version: 1.0.1
 Summary: Helper function to parse ajax datatable request into usable dictionary
 Author: Yap ZhiHon
 Author-email: y.zhihon@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: Django
@@ -107,10 +107,24 @@
 
 ```python
 from datatable_ajax_request_parser.django_extension import DjangoDTRequest
 
 DjangoDTRequest(parsed_dict=parsed_request)
 ```
 
+If you need a response, there is a `DjangoDTResponse` helper class available to help parse into datatable-compliant format
+
+```python
+from datatable_ajax_request_parser.django_extension get_django_dt_response
+
+parsed_query = get_django_datatable_query(sample_url)
+get_django_dt_response(parsed_query, <your model class>, <your function to process the data>, <your error>)
+
+```
+
+
 ## Footnote
 
 Feel free to submit any PRs for improvements
+
+## Credits
+I did not write everything by myself, I thank Lim Yong Soon for providing much of the useful code.
```

### Comparing `datatable_ajax_request_parser-1.0.0/datatable_ajax_request_parser.egg-info/SOURCES.txt` & `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.0/setup.py` & `datatable_ajax_request_parser-1.0.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="datatable_ajax_request_parser",
-    version="1.0.0",
+    version="1.0.1",
     description="Helper function to parse ajax datatable request into usable dictionary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yap ZhiHon",
     author_email="y.zhihon@gmail.com",
     classifiers=[
         "Operating System :: OS Independent"
```


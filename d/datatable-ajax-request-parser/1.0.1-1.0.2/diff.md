# Comparing `tmp/datatable_ajax_request_parser-1.0.1.tar.gz` & `tmp/datatable-ajax-request-parser-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatable_ajax_request_parser-1.0.1.tar", last modified: Mon May 29 06:46:50 2023, max compression
+gzip compressed data, was "datatable-ajax-request-parser-1.0.2.tar", last modified: Mon May 29 07:15:33 2023, max compression
```

## Comparing `datatable_ajax_request_parser-1.0.1.tar` & `datatable-ajax-request-parser-1.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 06:46:50.132918 datatable_ajax_request_parser-1.0.1/
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1067 2023-05-27 04:34:24.000000 datatable_ajax_request_parser-1.0.1/LICENCE
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5519 2023-05-29 06:46:50.133055 datatable_ajax_request_parser-1.0.1/PKG-INFO
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5157 2023-05-29 06:44:34.000000 datatable_ajax_request_parser-1.0.1/README.md
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 06:46:50.132001 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/
--rw-r--r--   0 yapzhihon   (501) staff       (20)        0 2023-05-26 16:26:39.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/__init__.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)      946 2023-05-29 02:51:56.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/dataclasses.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     3801 2023-05-29 06:45:13.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/django_extension.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     2990 2023-05-27 04:18:44.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/parser.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5381 2023-05-29 06:45:13.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/test_django_extension.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     6750 2023-05-29 02:38:27.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/test_parser.py
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1035 2023-05-29 02:38:32.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/utils.py
-drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 06:46:50.132723 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/
--rw-r--r--   0 yapzhihon   (501) staff       (20)     5519 2023-05-29 06:46:50.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/PKG-INFO
--rw-r--r--   0 yapzhihon   (501) staff       (20)      616 2023-05-29 06:46:50.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/SOURCES.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)        1 2023-05-29 06:46:50.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/dependency_links.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       24 2023-05-29 06:46:50.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/requires.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       30 2023-05-29 06:46:50.000000 datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/top_level.txt
--rw-r--r--   0 yapzhihon   (501) staff       (20)       79 2023-05-29 06:46:50.133542 datatable_ajax_request_parser-1.0.1/setup.cfg
--rw-r--r--   0 yapzhihon   (501) staff       (20)     1077 2023-05-29 06:44:34.000000 datatable_ajax_request_parser-1.0.1/setup.py
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 07:15:33.196290 datatable-ajax-request-parser-1.0.2/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1067 2023-05-27 04:34:24.000000 datatable-ajax-request-parser-1.0.2/LICENCE
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 07:15:33.196351 datatable-ajax-request-parser-1.0.2/PKG-INFO
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5157 2023-05-29 07:14:50.000000 datatable-ajax-request-parser-1.0.2/README.md
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 07:15:33.195493 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)        0 2023-05-26 16:26:39.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/__init__.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)      946 2023-05-29 02:51:56.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/dataclasses.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     3801 2023-05-29 06:45:13.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/django_extension.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     2990 2023-05-27 04:18:44.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/parser.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5381 2023-05-29 06:45:13.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/test_django_extension.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     6750 2023-05-29 02:38:27.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/test_parser.py
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1035 2023-05-29 02:38:32.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/utils.py
+drwxr-xr-x   0 yapzhihon   (501) staff       (20)        0 2023-05-29 07:15:33.196175 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     5590 2023-05-29 07:15:33.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/PKG-INFO
+-rw-r--r--   0 yapzhihon   (501) staff       (20)      616 2023-05-29 07:15:33.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)        1 2023-05-29 07:15:33.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       24 2023-05-29 07:15:33.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/requires.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       30 2023-05-29 07:15:33.000000 datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/top_level.txt
+-rw-r--r--   0 yapzhihon   (501) staff       (20)       79 2023-05-29 07:15:33.196640 datatable-ajax-request-parser-1.0.2/setup.cfg
+-rw-r--r--   0 yapzhihon   (501) staff       (20)     1148 2023-05-29 07:15:17.000000 datatable-ajax-request-parser-1.0.2/setup.py
```

### Comparing `datatable_ajax_request_parser-1.0.1/LICENCE` & `datatable-ajax-request-parser-1.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.1/PKG-INFO` & `datatable-ajax-request-parser-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
-Name: datatable_ajax_request_parser
-Version: 1.0.1
+Name: datatable-ajax-request-parser
+Version: 1.0.2
 Summary: Helper function to parse ajax datatable request into usable dictionary
+Home-page: https://github.com/ziiiio/datatable_ajax_request_parser.git
 Author: Yap ZhiHon
 Author-email: y.zhihon@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: Django
 License-File: LICENCE
 
 # Python Ajax Datatable Request Parser
 
 This is a small package to help with parsing datatable requests
 
 
 ## Installation
-simply do a `pip install datatable_ajax_request_parser`
+simply do a `pip install datatable-ajax-request-parser`
 
 
 ## How to use
 
 ```python
 
 from datatable_ajax_request_parser.parser import DTRequest, parse_datatable_raw_request_query
```

### Comparing `datatable_ajax_request_parser-1.0.1/README.md` & `datatable-ajax-request-parser-1.0.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Python Ajax Datatable Request Parser
 
 This is a small package to help with parsing datatable requests
 
 
 ## Installation
-simply do a `pip install datatable_ajax_request_parser`
+simply do a `pip install datatable-ajax-request-parser`
 
 
 ## How to use
 
 ```python
 
 from datatable_ajax_request_parser.parser import DTRequest, parse_datatable_raw_request_query
```

### Comparing `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/dataclasses.py` & `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/dataclasses.py`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/django_extension.py` & `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/django_extension.py`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/parser.py` & `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/parser.py`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/test_django_extension.py` & `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/test_django_extension.py`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/test_parser.py` & `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/test_parser.py`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser/utils.py` & `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser/utils.py`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/PKG-INFO` & `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: datatable-ajax-request-parser
-Version: 1.0.1
+Version: 1.0.2
 Summary: Helper function to parse ajax datatable request into usable dictionary
+Home-page: https://github.com/ziiiio/datatable_ajax_request_parser.git
 Author: Yap ZhiHon
 Author-email: y.zhihon@gmail.com
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: Django
 License-File: LICENCE
 
 # Python Ajax Datatable Request Parser
 
 This is a small package to help with parsing datatable requests
 
 
 ## Installation
-simply do a `pip install datatable_ajax_request_parser`
+simply do a `pip install datatable-ajax-request-parser`
 
 
 ## How to use
 
 ```python
 
 from datatable_ajax_request_parser.parser import DTRequest, parse_datatable_raw_request_query
```

### Comparing `datatable_ajax_request_parser-1.0.1/datatable_ajax_request_parser.egg-info/SOURCES.txt` & `datatable-ajax-request-parser-1.0.2/datatable_ajax_request_parser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatable_ajax_request_parser-1.0.1/setup.py` & `datatable-ajax-request-parser-1.0.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,21 +11,22 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
-    name="datatable_ajax_request_parser",
-    version="1.0.1",
+    name="datatable-ajax-request-parser",
+    version="1.0.2",
     description="Helper function to parse ajax datatable request into usable dictionary",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Yap ZhiHon",
     author_email="y.zhihon@gmail.com",
+    url="https://github.com/ziiiio/datatable_ajax_request_parser.git",
     classifiers=[
         "Operating System :: OS Independent"
     ],
     packages=setuptools.find_packages(
         include=['datatable_ajax_request_parser', 'datatable_ajax_request_parser.*']
     ),
     include_package_data=True,
```


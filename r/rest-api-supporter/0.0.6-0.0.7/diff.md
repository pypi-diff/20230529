# Comparing `tmp/rest-api-supporter-0.0.6.tar.gz` & `tmp/rest-api-supporter-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rest-api-supporter-0.0.6.tar", last modified: Thu Apr 27 10:38:24 2023, max compression
+gzip compressed data, was "rest-api-supporter-0.0.7.tar", last modified: Mon May 29 10:01:30 2023, max compression
```

## Comparing `rest-api-supporter-0.0.6.tar` & `rest-api-supporter-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:38:24.185637 rest-api-supporter-0.0.6/
--rw-r--r--   0 root         (0) root         (0)      836 2023-04-27 10:38:24.185637 rest-api-supporter-0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      554 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:38:24.183636 rest-api-supporter-0.0.6/rest_api_supporter/
--rw-r--r--   0 root         (0) root         (0)       42 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/rest_api_supporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:38:24.184636 rest-api-supporter-0.0.6/rest_api_supporter/servers/
--rw-r--r--   0 root         (0) root         (0)       91 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/rest_api_supporter/servers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4267 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/rest_api_supporter/servers/flask_rest_api_server.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:38:24.185637 rest-api-supporter-0.0.6/rest_api_supporter/utils/
--rw-r--r--   0 root         (0) root         (0)      204 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/rest_api_supporter/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/rest_api_supporter/utils/base64_to_image.py
--rw-r--r--   0 root         (0) root         (0)      387 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/rest_api_supporter/utils/get.py
--rw-r--r--   0 root         (0) root         (0)      292 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/rest_api_supporter/utils/image_to_base64.py
--rw-r--r--   0 root         (0) root         (0)      502 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/rest_api_supporter/utils/post.py
--rw-r--r--   0 root         (0) root         (0)      220 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/rest_api_supporter/utils/query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 10:38:24.184636 rest-api-supporter-0.0.6/rest_api_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)      836 2023-04-27 10:38:23.000000 rest-api-supporter-0.0.6/rest_api_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      614 2023-04-27 10:38:24.000000 rest-api-supporter-0.0.6/rest_api_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 10:38:23.000000 rest-api-supporter-0.0.6/rest_api_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/rest_api_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       26 2023-04-27 10:38:23.000000 rest-api-supporter-0.0.6/rest_api_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-04-27 10:38:23.000000 rest-api-supporter-0.0.6/rest_api_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 10:38:24.185637 rest-api-supporter-0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      606 2023-04-27 10:36:17.000000 rest-api-supporter-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:01:30.909896 rest-api-supporter-0.0.7/
+-rw-r--r--   0 root         (0) root         (0)      821 2023-05-29 10:01:30.909896 rest-api-supporter-0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      557 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:01:30.906896 rest-api-supporter-0.0.7/rest_api_supporter/
+-rw-r--r--   0 root         (0) root         (0)       43 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:01:30.908896 rest-api-supporter-0.0.7/rest_api_supporter/servers/
+-rw-r--r--   0 root         (0) root         (0)       91 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter/servers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4267 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter/servers/flask_rest_api_server.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:01:30.909896 rest-api-supporter-0.0.7/rest_api_supporter/utils/
+-rw-r--r--   0 root         (0) root         (0)      157 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter/utils/base64_to_image.py
+-rw-r--r--   0 root         (0) root         (0)      387 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter/utils/get.py
+-rw-r--r--   0 root         (0) root         (0)      292 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter/utils/image_to_base64.py
+-rw-r--r--   0 root         (0) root         (0)      502 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter/utils/post.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 10:01:30.908896 rest-api-supporter-0.0.7/rest_api_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      821 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      580 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       26 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/rest_api_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 10:01:30.909896 rest-api-supporter-0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      606 2023-05-29 10:01:30.000000 rest-api-supporter-0.0.7/setup.py
```

### Comparing `rest-api-supporter-0.0.6/PKG-INFO` & `rest-api-supporter-0.0.7/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: rest-api-supporter
-Version: 0.0.6
+Version: 0.0.7
 Summary: Rest api supporter
 Home-page: https://github.com/automatethem/rest-api-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # rest-api-supporter
 
 https://pypi.org/project/rest-api-supporter/
 <pre>
 pip install rest-api-supporter
 </pre>
 
 Supported APIs  
 <pre>
 import rest_api_supporter
 
-rest_api_supporter.servers.FlaskRestAPIServer
+#rest_api_supporter.servers.FlaskRestAPIServer
 rest_api_supporter.utils.image_to_base64
 rest_api_supporter.utils.base64_to_image
 rest_api_supporter.utils.post
 rest_api_supporter.utils.get
 </pre>
 
-REST API example (flask)  
-https://github.com/automatethem/rest-api-supporter/blob/main/examples/blueprint_app.py  
+#REST API example (flask)  
+#https://github.com/automatethem/rest-api-supporter/blob/main/examples/blueprint_app.py  
 https://github.com/automatethem/rest-api-supporter/blob/main/examples/predict.py
```

### Comparing `rest-api-supporter-0.0.6/README.md` & `rest-api-supporter-0.0.7/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 pip install rest-api-supporter
 </pre>
 
 Supported APIs  
 <pre>
 import rest_api_supporter
 
-rest_api_supporter.servers.FlaskRestAPIServer
+#rest_api_supporter.servers.FlaskRestAPIServer
 rest_api_supporter.utils.image_to_base64
 rest_api_supporter.utils.base64_to_image
 rest_api_supporter.utils.post
 rest_api_supporter.utils.get
 </pre>
 
-REST API example (flask)  
-https://github.com/automatethem/rest-api-supporter/blob/main/examples/blueprint_app.py  
+#REST API example (flask)  
+#https://github.com/automatethem/rest-api-supporter/blob/main/examples/blueprint_app.py  
 https://github.com/automatethem/rest-api-supporter/blob/main/examples/predict.py
```

### Comparing `rest-api-supporter-0.0.6/rest_api_supporter/servers/flask_rest_api_server.py` & `rest-api-supporter-0.0.7/rest_api_supporter/servers/flask_rest_api_server.py`

 * *Files identical despite different names*

### Comparing `rest-api-supporter-0.0.6/rest_api_supporter.egg-info/PKG-INFO` & `rest-api-supporter-0.0.7/rest_api_supporter.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: rest-api-supporter
-Version: 0.0.6
+Version: 0.0.7
 Summary: Rest api supporter
 Home-page: https://github.com/automatethem/rest-api-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # rest-api-supporter
 
 https://pypi.org/project/rest-api-supporter/
 <pre>
 pip install rest-api-supporter
 </pre>
 
 Supported APIs  
 <pre>
 import rest_api_supporter
 
-rest_api_supporter.servers.FlaskRestAPIServer
+#rest_api_supporter.servers.FlaskRestAPIServer
 rest_api_supporter.utils.image_to_base64
 rest_api_supporter.utils.base64_to_image
 rest_api_supporter.utils.post
 rest_api_supporter.utils.get
 </pre>
 
-REST API example (flask)  
-https://github.com/automatethem/rest-api-supporter/blob/main/examples/blueprint_app.py  
+#REST API example (flask)  
+#https://github.com/automatethem/rest-api-supporter/blob/main/examples/blueprint_app.py  
 https://github.com/automatethem/rest-api-supporter/blob/main/examples/predict.py
```

### Comparing `rest-api-supporter-0.0.6/rest_api_supporter.egg-info/SOURCES.txt` & `rest-api-supporter-0.0.7/rest_api_supporter.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -9,9 +9,8 @@
 rest_api_supporter.egg-info/top_level.txt
 rest_api_supporter/servers/__init__.py
 rest_api_supporter/servers/flask_rest_api_server.py
 rest_api_supporter/utils/__init__.py
 rest_api_supporter/utils/base64_to_image.py
 rest_api_supporter/utils/get.py
 rest_api_supporter/utils/image_to_base64.py
-rest_api_supporter/utils/post.py
-rest_api_supporter/utils/query.py
+rest_api_supporter/utils/post.py
```

### Comparing `rest-api-supporter-0.0.6/setup.py` & `rest-api-supporter-0.0.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='rest-api-supporter',
-	version='0.0.6',
+	version='0.0.7',
 	description='Rest api supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/rest-api-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```


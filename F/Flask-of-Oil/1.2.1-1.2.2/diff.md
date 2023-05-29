# Comparing `tmp/Flask-of-Oil-1.2.1.tar.gz` & `tmp/Flask-of-Oil-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Flask-of-Oil-1.2.1.tar", last modified: Mon May 29 11:27:11 2023, max compression
+gzip compressed data, was "Flask-of-Oil-1.2.2.tar", last modified: Mon May 29 11:35:49 2023, max compression
```

## Comparing `Flask-of-Oil-1.2.1.tar` & `Flask-of-Oil-1.2.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:27:11.770710 Flask-of-Oil-1.2.1/
-drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:27:11.763410 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/
--rw-r--r--   0 michal     (501) staff       (20)     1225 2023-05-29 11:27:11.000000 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/PKG-INFO
--rw-r--r--   0 michal     (501) staff       (20)      467 2023-05-29 11:27:11.000000 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/SOURCES.txt
--rw-r--r--   0 michal     (501) staff       (20)        1 2023-05-29 11:27:11.000000 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/dependency_links.txt
--rw-r--r--   0 michal     (501) staff       (20)       33 2023-05-29 11:27:11.000000 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/requires.txt
--rw-r--r--   0 michal     (501) staff       (20)       13 2023-05-29 11:27:11.000000 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/top_level.txt
--rw-r--r--   0 michal     (501) staff       (20)    11356 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.1/LICENSE.txt
--rw-r--r--   0 michal     (501) staff       (20)       72 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.1/MANIFEST.in
--rw-r--r--   0 michal     (501) staff       (20)     1225 2023-05-29 11:27:11.770843 Flask-of-Oil-1.2.1/PKG-INFO
--rw-r--r--   0 michal     (501) staff       (20)     8068 2023-05-29 11:22:08.000000 Flask-of-Oil-1.2.1/README.md
--rw-r--r--   0 michal     (501) staff       (20)      549 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.1/README.rst
-drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:27:11.767291 Flask-of-Oil-1.2.1/flask_of_oil/
--rw-r--r--   0 michal     (501) staff       (20)      232 2022-05-12 12:25:48.000000 Flask-of-Oil-1.2.1/flask_of_oil/__init__.py
--rw-r--r--   0 michal     (501) staff       (20)     5405 2023-05-29 11:18:50.000000 Flask-of-Oil-1.2.1/flask_of_oil/jwt_validator.py
--rw-r--r--   0 michal     (501) staff       (20)     7016 2022-08-26 14:27:53.000000 Flask-of-Oil-1.2.1/flask_of_oil/oauth_filter.py
--rw-r--r--   0 michal     (501) staff       (20)     5393 2022-08-26 11:30:52.000000 Flask-of-Oil-1.2.1/flask_of_oil/opaque_validator.py
--rw-r--r--   0 michal     (501) staff       (20)     1321 2022-08-12 12:06:11.000000 Flask-of-Oil-1.2.1/flask_of_oil/tools.py
--rw-r--r--   0 michal     (501) staff       (20)       80 2023-05-29 11:27:11.771305 Flask-of-Oil-1.2.1/setup.cfg
--rw-r--r--   0 michal     (501) staff       (20)      934 2023-05-29 11:18:54.000000 Flask-of-Oil-1.2.1/setup.py
-drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:27:11.770056 Flask-of-Oil-1.2.1/tests/
--rw-r--r--   0 michal     (501) staff       (20)    10182 2023-05-29 11:22:37.000000 Flask-of-Oil-1.2.1/tests/test_jwt_validator.py
--rw-r--r--   0 michal     (501) staff       (20)    12032 2023-05-29 11:18:50.000000 Flask-of-Oil-1.2.1/tests/test_oauth_filter.py
--rw-r--r--   0 michal     (501) staff       (20)     4981 2023-05-29 11:18:50.000000 Flask-of-Oil-1.2.1/tests/test_opaque_validator.py
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:35:49.729073 Flask-of-Oil-1.2.2/
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:35:49.723055 Flask-of-Oil-1.2.2/Flask_of_Oil.egg-info/
+-rw-r--r--   0 michal     (501) staff       (20)     1225 2023-05-29 11:35:49.000000 Flask-of-Oil-1.2.2/Flask_of_Oil.egg-info/PKG-INFO
+-rw-r--r--   0 michal     (501) staff       (20)      467 2023-05-29 11:35:49.000000 Flask-of-Oil-1.2.2/Flask_of_Oil.egg-info/SOURCES.txt
+-rw-r--r--   0 michal     (501) staff       (20)        1 2023-05-29 11:35:49.000000 Flask-of-Oil-1.2.2/Flask_of_Oil.egg-info/dependency_links.txt
+-rw-r--r--   0 michal     (501) staff       (20)       33 2023-05-29 11:35:49.000000 Flask-of-Oil-1.2.2/Flask_of_Oil.egg-info/requires.txt
+-rw-r--r--   0 michal     (501) staff       (20)       13 2023-05-29 11:35:49.000000 Flask-of-Oil-1.2.2/Flask_of_Oil.egg-info/top_level.txt
+-rw-r--r--   0 michal     (501) staff       (20)    11356 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.2/LICENSE.txt
+-rw-r--r--   0 michal     (501) staff       (20)       72 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.2/MANIFEST.in
+-rw-r--r--   0 michal     (501) staff       (20)     1225 2023-05-29 11:35:49.729204 Flask-of-Oil-1.2.2/PKG-INFO
+-rw-r--r--   0 michal     (501) staff       (20)     8068 2023-05-29 11:33:51.000000 Flask-of-Oil-1.2.2/README.md
+-rw-r--r--   0 michal     (501) staff       (20)      549 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.2/README.rst
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:35:49.726137 Flask-of-Oil-1.2.2/flask_of_oil/
+-rw-r--r--   0 michal     (501) staff       (20)      232 2022-05-12 12:25:48.000000 Flask-of-Oil-1.2.2/flask_of_oil/__init__.py
+-rw-r--r--   0 michal     (501) staff       (20)     5405 2023-05-29 11:18:50.000000 Flask-of-Oil-1.2.2/flask_of_oil/jwt_validator.py
+-rw-r--r--   0 michal     (501) staff       (20)     7016 2022-08-26 14:27:53.000000 Flask-of-Oil-1.2.2/flask_of_oil/oauth_filter.py
+-rw-r--r--   0 michal     (501) staff       (20)     5393 2022-08-26 11:30:52.000000 Flask-of-Oil-1.2.2/flask_of_oil/opaque_validator.py
+-rw-r--r--   0 michal     (501) staff       (20)     1321 2022-08-12 12:06:11.000000 Flask-of-Oil-1.2.2/flask_of_oil/tools.py
+-rw-r--r--   0 michal     (501) staff       (20)       80 2023-05-29 11:35:49.729599 Flask-of-Oil-1.2.2/setup.cfg
+-rw-r--r--   0 michal     (501) staff       (20)      934 2023-05-29 11:34:52.000000 Flask-of-Oil-1.2.2/setup.py
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:35:49.728076 Flask-of-Oil-1.2.2/tests/
+-rw-r--r--   0 michal     (501) staff       (20)    10182 2023-05-29 11:34:00.000000 Flask-of-Oil-1.2.2/tests/test_jwt_validator.py
+-rw-r--r--   0 michal     (501) staff       (20)    12032 2023-05-29 11:18:50.000000 Flask-of-Oil-1.2.2/tests/test_oauth_filter.py
+-rw-r--r--   0 michal     (501) staff       (20)     4981 2023-05-29 11:18:50.000000 Flask-of-Oil-1.2.2/tests/test_opaque_validator.py
```

### Comparing `Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/PKG-INFO` & `Flask-of-Oil-1.2.2/Flask_of_Oil.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-of-Oil
-Version: 1.2.1
+Version: 1.2.2
 Summary: Flask OAuth Filter - an OAuth Interceptor Logic
 Home-page: https://github.com/curity/flask-of-oil
 Author: Curity AB
 Author-email: info@curity.io
 License: Apache Software License
 Keywords: oauth,flask,introspection,access token,jwt,opaque
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-of-Oil-1.2.1/LICENSE.txt` & `Flask-of-Oil-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.1/PKG-INFO` & `Flask-of-Oil-1.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-of-Oil
-Version: 1.2.1
+Version: 1.2.2
 Summary: Flask OAuth Filter - an OAuth Interceptor Logic
 Home-page: https://github.com/curity/flask-of-oil
 Author: Curity AB
 Author-email: info@curity.io
 License: Apache Software License
 Keywords: oauth,flask,introspection,access token,jwt,opaque
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-of-Oil-1.2.1/README.md` & `Flask-of-Oil-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.1/README.rst` & `Flask-of-Oil-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.1/flask_of_oil/jwt_validator.py` & `Flask-of-Oil-1.2.2/flask_of_oil/jwt_validator.py`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.1/flask_of_oil/oauth_filter.py` & `Flask-of-Oil-1.2.2/flask_of_oil/oauth_filter.py`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.1/flask_of_oil/opaque_validator.py` & `Flask-of-Oil-1.2.2/flask_of_oil/opaque_validator.py`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.1/flask_of_oil/tools.py` & `Flask-of-Oil-1.2.2/flask_of_oil/tools.py`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.1/setup.py` & `Flask-of-Oil-1.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='Flask-of-Oil',
     packages=['flask_of_oil'],
-    version='1.2.1',
+    version='1.2.2',
     license='Apache Software License',
     description='Flask OAuth Filter - an OAuth Interceptor Logic',
     long_description=open('README.rst').read(),
     author='Curity AB',
     author_email='info@curity.io',
     url='https://github.com/curity/flask-of-oil',
     keywords=['oauth', 'flask', 'introspection', 'access token', 'jwt', 'opaque'],
```

### Comparing `Flask-of-Oil-1.2.1/tests/test_jwt_validator.py` & `Flask-of-Oil-1.2.2/tests/test_jwt_validator.py`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.1/tests/test_oauth_filter.py` & `Flask-of-Oil-1.2.2/tests/test_oauth_filter.py`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.1/tests/test_opaque_validator.py` & `Flask-of-Oil-1.2.2/tests/test_opaque_validator.py`

 * *Files identical despite different names*


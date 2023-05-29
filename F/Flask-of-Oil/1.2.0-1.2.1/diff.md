# Comparing `tmp/Flask-of-Oil-1.2.0.tar.gz` & `tmp/Flask-of-Oil-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/michal/projects/github/flask-of-oil/dist/tmppd7x3lcc/Flask-of-Oil-1.2.0.tar", last modified: Thu May 12 12:36:34 2022, max compression
+gzip compressed data, was "Flask-of-Oil-1.2.1.tar", last modified: Mon May 29 11:27:11 2023, max compression
```

## Comparing `Flask-of-Oil-1.2.0.tar` & `Flask-of-Oil-1.2.1.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 michal     (501) staff       (20)        0 2022-05-12 12:36:34.435224 Flask-of-Oil-1.2.0/
-drwxr-xr-x   0 michal     (501) staff       (20)        0 2022-05-12 12:36:34.431888 Flask-of-Oil-1.2.0/Flask_of_Oil.egg-info/
--rw-r--r--   0 michal     (501) staff       (20)     1225 2022-05-12 12:36:33.000000 Flask-of-Oil-1.2.0/Flask_of_Oil.egg-info/PKG-INFO
--rw-r--r--   0 michal     (501) staff       (20)      381 2022-05-12 12:36:34.000000 Flask-of-Oil-1.2.0/Flask_of_Oil.egg-info/SOURCES.txt
--rw-r--r--   0 michal     (501) staff       (20)        1 2022-05-12 12:36:34.000000 Flask-of-Oil-1.2.0/Flask_of_Oil.egg-info/dependency_links.txt
--rw-r--r--   0 michal     (501) staff       (20)       33 2022-05-12 12:36:34.000000 Flask-of-Oil-1.2.0/Flask_of_Oil.egg-info/requires.txt
--rw-r--r--   0 michal     (501) staff       (20)       13 2022-05-12 12:36:34.000000 Flask-of-Oil-1.2.0/Flask_of_Oil.egg-info/top_level.txt
--rw-r--r--   0 michal     (501) staff       (20)    11356 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.0/LICENSE.txt
--rw-r--r--   0 michal     (501) staff       (20)       72 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.0/MANIFEST.in
--rw-r--r--   0 michal     (501) staff       (20)     1225 2022-05-12 12:36:34.435464 Flask-of-Oil-1.2.0/PKG-INFO
--rw-r--r--   0 michal     (501) staff       (20)     7408 2022-05-12 12:25:48.000000 Flask-of-Oil-1.2.0/README.md
--rw-r--r--   0 michal     (501) staff       (20)      549 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.0/README.rst
-drwxr-xr-x   0 michal     (501) staff       (20)        0 2022-05-12 12:36:34.434549 Flask-of-Oil-1.2.0/flask_of_oil/
--rw-r--r--   0 michal     (501) staff       (20)      232 2022-05-12 12:25:48.000000 Flask-of-Oil-1.2.0/flask_of_oil/__init__.py
--rw-r--r--   0 michal     (501) staff       (20)     5445 2022-05-12 12:34:00.000000 Flask-of-Oil-1.2.0/flask_of_oil/jwt_validator.py
--rw-r--r--   0 michal     (501) staff       (20)     7016 2022-05-12 12:25:48.000000 Flask-of-Oil-1.2.0/flask_of_oil/oauth_filter.py
--rw-r--r--   0 michal     (501) staff       (20)     5393 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.0/flask_of_oil/opaque_validator.py
--rw-r--r--   0 michal     (501) staff       (20)     1371 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.0/flask_of_oil/tools.py
--rw-r--r--   0 michal     (501) staff       (20)       80 2022-05-12 12:36:34.436358 Flask-of-Oil-1.2.0/setup.cfg
--rw-r--r--   0 michal     (501) staff       (20)      934 2022-05-12 12:34:00.000000 Flask-of-Oil-1.2.0/setup.py
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:27:11.770710 Flask-of-Oil-1.2.1/
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:27:11.763410 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/
+-rw-r--r--   0 michal     (501) staff       (20)     1225 2023-05-29 11:27:11.000000 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/PKG-INFO
+-rw-r--r--   0 michal     (501) staff       (20)      467 2023-05-29 11:27:11.000000 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/SOURCES.txt
+-rw-r--r--   0 michal     (501) staff       (20)        1 2023-05-29 11:27:11.000000 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/dependency_links.txt
+-rw-r--r--   0 michal     (501) staff       (20)       33 2023-05-29 11:27:11.000000 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/requires.txt
+-rw-r--r--   0 michal     (501) staff       (20)       13 2023-05-29 11:27:11.000000 Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/top_level.txt
+-rw-r--r--   0 michal     (501) staff       (20)    11356 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.1/LICENSE.txt
+-rw-r--r--   0 michal     (501) staff       (20)       72 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.1/MANIFEST.in
+-rw-r--r--   0 michal     (501) staff       (20)     1225 2023-05-29 11:27:11.770843 Flask-of-Oil-1.2.1/PKG-INFO
+-rw-r--r--   0 michal     (501) staff       (20)     8068 2023-05-29 11:22:08.000000 Flask-of-Oil-1.2.1/README.md
+-rw-r--r--   0 michal     (501) staff       (20)      549 2021-05-06 08:22:15.000000 Flask-of-Oil-1.2.1/README.rst
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:27:11.767291 Flask-of-Oil-1.2.1/flask_of_oil/
+-rw-r--r--   0 michal     (501) staff       (20)      232 2022-05-12 12:25:48.000000 Flask-of-Oil-1.2.1/flask_of_oil/__init__.py
+-rw-r--r--   0 michal     (501) staff       (20)     5405 2023-05-29 11:18:50.000000 Flask-of-Oil-1.2.1/flask_of_oil/jwt_validator.py
+-rw-r--r--   0 michal     (501) staff       (20)     7016 2022-08-26 14:27:53.000000 Flask-of-Oil-1.2.1/flask_of_oil/oauth_filter.py
+-rw-r--r--   0 michal     (501) staff       (20)     5393 2022-08-26 11:30:52.000000 Flask-of-Oil-1.2.1/flask_of_oil/opaque_validator.py
+-rw-r--r--   0 michal     (501) staff       (20)     1321 2022-08-12 12:06:11.000000 Flask-of-Oil-1.2.1/flask_of_oil/tools.py
+-rw-r--r--   0 michal     (501) staff       (20)       80 2023-05-29 11:27:11.771305 Flask-of-Oil-1.2.1/setup.cfg
+-rw-r--r--   0 michal     (501) staff       (20)      934 2023-05-29 11:18:54.000000 Flask-of-Oil-1.2.1/setup.py
+drwxr-xr-x   0 michal     (501) staff       (20)        0 2023-05-29 11:27:11.770056 Flask-of-Oil-1.2.1/tests/
+-rw-r--r--   0 michal     (501) staff       (20)    10182 2023-05-29 11:22:37.000000 Flask-of-Oil-1.2.1/tests/test_jwt_validator.py
+-rw-r--r--   0 michal     (501) staff       (20)    12032 2023-05-29 11:18:50.000000 Flask-of-Oil-1.2.1/tests/test_oauth_filter.py
+-rw-r--r--   0 michal     (501) staff       (20)     4981 2023-05-29 11:18:50.000000 Flask-of-Oil-1.2.1/tests/test_opaque_validator.py
```

### Comparing `Flask-of-Oil-1.2.0/Flask_of_Oil.egg-info/PKG-INFO` & `Flask-of-Oil-1.2.1/Flask_of_Oil.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-of-Oil
-Version: 1.2.0
+Version: 1.2.1
 Summary: Flask OAuth Filter - an OAuth Interceptor Logic
 Home-page: https://github.com/curity/flask-of-oil
 Author: Curity AB
 Author-email: info@curity.io
 License: Apache Software License
 Keywords: oauth,flask,introspection,access token,jwt,opaque
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-of-Oil-1.2.0/LICENSE.txt` & `Flask-of-Oil-1.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.0/PKG-INFO` & `Flask-of-Oil-1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Flask-of-Oil
-Version: 1.2.0
+Version: 1.2.1
 Summary: Flask OAuth Filter - an OAuth Interceptor Logic
 Home-page: https://github.com/curity/flask-of-oil
 Author: Curity AB
 Author-email: info@curity.io
 License: Apache Software License
 Keywords: oauth,flask,introspection,access token,jwt,opaque
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `Flask-of-Oil-1.2.0/README.md` & `Flask-of-Oil-1.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -191,14 +191,44 @@
 @_app.errorhandler(403)
 def forbidden(error):
     return json.dumps({'error': "forbidden",
                        "error_description": "Access token is missing appropriate scopes"}), \
            403, {'Content-Type': 'application/json; charset=utf-8'}
 ```
 
+## Running the test suite
+
+You can run the test suite with the following command:
+
+```bash
+pytest --log-level=DEBUG
+```
+
+If you want to run tests from a concrete file, use this command:
+
+```bash
+pytest --log-level=DEBUG tests/test_jwt_validator.py
+```
+
+It's best to run the tests in a dedicated Python virtual environment. Follow these steps to create the environment, install all dependencies, then run the test suite:
+
+```bash
+python -m venv venv
+source venv/bin/activate
+pip install -r requirements.txt
+pytest --log-level=DEBUG tests/test_jwt_validator.py
+```
+
+When you're done with the tests, run:
+
+```bash
+deactivate
+```
+
+to exit the virtual environment.
 
 ## Questions and Support
 
 For questions and support, contact Curity AB:
 
 > Curity AB
 >
```

### Comparing `Flask-of-Oil-1.2.0/README.rst` & `Flask-of-Oil-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.0/flask_of_oil/jwt_validator.py` & `Flask-of-Oil-1.2.1/flask_of_oil/jwt_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,17 +112,15 @@
 
         if 'sub' not in payload:
             self.logger.debug("No subject in body, invalid token")
             return {"active": False}
 
         # Could be an empty scope, which may be allowed, so replace with empty string if not found
         if 'scope' not in payload:
-            scope = ""
-        else:
-            scope = payload['scope']
+            payload['scope'] = ""
 
         exp = payload['exp']
 
         d = datetime.utcnow()
         now = calendar.timegm(d.utctimetuple())
 
         if now >= exp:
```

### Comparing `Flask-of-Oil-1.2.0/flask_of_oil/oauth_filter.py` & `Flask-of-Oil-1.2.1/flask_of_oil/oauth_filter.py`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.0/flask_of_oil/opaque_validator.py` & `Flask-of-Oil-1.2.1/flask_of_oil/opaque_validator.py`

 * *Files identical despite different names*

### Comparing `Flask-of-Oil-1.2.0/flask_of_oil/tools.py` & `Flask-of-Oil-1.2.1/flask_of_oil/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,18 +16,16 @@
 
 import base64
 import random
 import string
 
 
 def base64_urldecode(string):
-    string.replace('-', '+')
-    string.replace('_', '/')
     string += '=' * (4 - (len(string) % 4))
-    return base64.b64decode(string)
+    return base64.urlsafe_b64decode(string)
 
 
 def decode_payload(token):
     if token and len(token.split('.')) == 3:
         token_part = token.split('.')[1]
         token_part += '=' * (4 - len(token_part) % 4)
         return base64.b64decode(token_part)
```

### Comparing `Flask-of-Oil-1.2.0/setup.py` & `Flask-of-Oil-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.core import setup
 
 setup(
     name='Flask-of-Oil',
     packages=['flask_of_oil'],
-    version='1.2.0',
+    version='1.2.1',
     license='Apache Software License',
     description='Flask OAuth Filter - an OAuth Interceptor Logic',
     long_description=open('README.rst').read(),
     author='Curity AB',
     author_email='info@curity.io',
     url='https://github.com/curity/flask-of-oil',
     keywords=['oauth', 'flask', 'introspection', 'access token', 'jwt', 'opaque'],
```


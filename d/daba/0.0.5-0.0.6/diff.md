# Comparing `tmp/daba-0.0.5.tar.gz` & `tmp/daba-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daba-0.0.5.tar", last modified: Sun May 28 21:47:47 2023, max compression
+gzip compressed data, was "daba-0.0.6.tar", last modified: Sun May 28 22:03:55 2023, max compression
```

## Comparing `daba-0.0.5.tar` & `daba-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 21:47:47.969518 daba-0.0.5/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)    35148 2023-05-26 00:11:19.000000 daba-0.0.5/LICENSE
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     3331 2023-05-28 21:47:47.969395 daba-0.0.5/PKG-INFO
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     2821 2023-05-28 15:17:32.000000 daba-0.0.5/README.md
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 21:47:47.968345 daba-0.0.5/daba/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     3800 2023-05-28 21:42:41.000000 daba-0.0.5/daba/Mongo.py
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 05:47:42.000000 daba-0.0.5/daba/__init__.py
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 21:47:47.968773 daba-0.0.5/daba.egg-info/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     3331 2023-05-28 21:47:47.000000 daba-0.0.5/daba.egg-info/PKG-INFO
--rw-r--r--   0 vishnuprakash   (501) staff       (20)      238 2023-05-28 21:47:47.000000 daba-0.0.5/daba.egg-info/SOURCES.txt
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        1 2023-05-28 21:47:47.000000 daba-0.0.5/daba.egg-info/dependency_links.txt
--rw-r--r--   0 vishnuprakash   (501) staff       (20)       11 2023-05-28 21:47:47.000000 daba-0.0.5/daba.egg-info/top_level.txt
--rw-r--r--   0 vishnuprakash   (501) staff       (20)       38 2023-05-28 21:47:47.969557 daba-0.0.5/setup.cfg
--rw-r--r--   0 vishnuprakash   (501) staff       (20)      735 2023-05-28 21:43:46.000000 daba-0.0.5/setup.py
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 21:47:47.968879 daba-0.0.5/tests/
-drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 21:47:47.969238 daba-0.0.5/tests/Database/
--rw-r--r--   0 vishnuprakash   (501) staff       (20)     6343 2023-05-28 08:07:40.000000 daba-0.0.5/tests/Database/Mongo.py
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:27.000000 daba-0.0.5/tests/Database/__init__.py
--rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:08.000000 daba-0.0.5/tests/__init__.py
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 22:03:55.622101 daba-0.0.6/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)    35148 2023-05-26 00:11:19.000000 daba-0.0.6/LICENSE
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     3331 2023-05-28 22:03:55.621978 daba-0.0.6/PKG-INFO
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     2821 2023-05-28 15:17:32.000000 daba-0.0.6/README.md
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 22:03:55.620797 daba-0.0.6/daba/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     3600 2023-05-28 22:03:35.000000 daba-0.0.6/daba/Mongo.py
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 05:47:42.000000 daba-0.0.6/daba/__init__.py
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 22:03:55.621329 daba-0.0.6/daba.egg-info/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     3331 2023-05-28 22:03:55.000000 daba-0.0.6/daba.egg-info/PKG-INFO
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)      238 2023-05-28 22:03:55.000000 daba-0.0.6/daba.egg-info/SOURCES.txt
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        1 2023-05-28 22:03:55.000000 daba-0.0.6/daba.egg-info/dependency_links.txt
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)       11 2023-05-28 22:03:55.000000 daba-0.0.6/daba.egg-info/top_level.txt
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)       38 2023-05-28 22:03:55.622144 daba-0.0.6/setup.cfg
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)      735 2023-05-28 21:59:16.000000 daba-0.0.6/setup.py
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 22:03:55.621455 daba-0.0.6/tests/
+drwxr-xr-x   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 22:03:55.621817 daba-0.0.6/tests/Database/
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)     6343 2023-05-28 08:07:40.000000 daba-0.0.6/tests/Database/Mongo.py
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:27.000000 daba-0.0.6/tests/Database/__init__.py
+-rw-r--r--   0 vishnuprakash   (501) staff       (20)        0 2023-05-28 06:09:08.000000 daba-0.0.6/tests/__init__.py
```

### Comparing `daba-0.0.5/LICENSE` & `daba-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `daba-0.0.5/PKG-INFO` & `daba-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daba
-Version: 0.0.5
+Version: 0.0.6
 Summary: daba by Klivolks.
 Home-page: https://github.com/klivolks/Database
 Author: Vishnu Prakash
 Author-email: vishnu@klivolks.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `daba-0.0.5/README.md` & `daba-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `daba-0.0.5/daba/Mongo.py` & `daba-0.0.6/daba/Mongo.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,24 +87,14 @@
 
     def count(self, condition=None):
         # Count the number of documents in the collection
         if condition is None:
             condition = {}
         return self.exec_operation(self.collection.count_documents, condition)
 
-
-    @contextmanager
-    def managed_db(self):
-        try:
-            yield
-        finally:
-            self.close_db()
-
     def exec_operation(self, operation, *args):
-        response = None
-        with self.managed_db():
-            try:
-                response = operation(*args)
-            except Exception as e:
-                self.logger.error(f"An error occurred: {e}")
-                raise
+        try:
+            response = operation(*args)
+        except Exception as e:
+            self.logger.error(f"An error occurred: {e}")
+            raise
         return response
```

### Comparing `daba-0.0.5/daba.egg-info/PKG-INFO` & `daba-0.0.6/daba.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daba
-Version: 0.0.5
+Version: 0.0.6
 Summary: daba by Klivolks.
 Home-page: https://github.com/klivolks/Database
 Author: Vishnu Prakash
 Author-email: vishnu@klivolks.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `daba-0.0.5/setup.py` & `daba-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='daba',
-    version='0.0.5',
+    version='0.0.6',
     description='daba by Klivolks.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Vishnu Prakash',
     author_email='vishnu@klivolks.com',
     url='https://github.com/klivolks/Database',
     packages=find_packages(),
```

### Comparing `daba-0.0.5/tests/Database/Mongo.py` & `daba-0.0.6/tests/Database/Mongo.py`

 * *Files identical despite different names*


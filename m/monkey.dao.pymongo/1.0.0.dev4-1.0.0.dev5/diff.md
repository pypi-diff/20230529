# Comparing `tmp/monkey.dao.pymongo-1.0.0.dev4.tar.gz` & `tmp/monkey.dao.pymongo-1.0.0.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monkey.dao.pymongo-1.0.0.dev4.tar", last modified: Sat Jan 28 10:02:01 2023, max compression
+gzip compressed data, was "monkey.dao.pymongo-1.0.0.dev5.tar", last modified: Mon May 29 06:18:55 2023, max compression
```

## Comparing `monkey.dao.pymongo-1.0.0.dev4.tar` & `monkey.dao.pymongo-1.0.0.dev5.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-01-28 10:02:01.295760 monkey.dao.pymongo-1.0.0.dev4/
--rw-rw-rw-   0        0        0    11556 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev4/LICENSE.txt
--rw-rw-rw-   0        0        0       60 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev4/MANIFEST.in
--rw-rw-rw-   0        0        0      961 2023-01-28 10:02:01.293739 monkey.dao.pymongo-1.0.0.dev4/PKG-INFO
--rw-rw-rw-   0        0        0      311 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev4/README.rst
-drwxrwxrwx   0        0        0        0 2023-01-28 10:02:01.223846 monkey.dao.pymongo-1.0.0.dev4/monkey/
--rw-rw-rw-   0        0        0      103 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev4/monkey/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-28 10:02:01.268946 monkey.dao.pymongo-1.0.0.dev4/monkey/dao/
--rw-rw-rw-   0        0        0      103 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev4/monkey/dao/__init__.py
-drwxrwxrwx   0        0        0        0 2023-01-28 10:02:01.289750 monkey.dao.pymongo-1.0.0.dev4/monkey/dao/pymongo/
--rw-rw-rw-   0        0        0       48 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev4/monkey/dao/pymongo/__init__.py
--rw-rw-rw-   0        0        0     9478 2023-01-28 10:01:16.000000 monkey.dao.pymongo-1.0.0.dev4/monkey/dao/pymongo/core.py
--rw-rw-rw-   0        0        0      415 2023-01-28 09:55:06.000000 monkey.dao.pymongo-1.0.0.dev4/monkey/dao/pymongo/utils.py
-drwxrwxrwx   0        0        0        0 2023-01-28 10:02:01.262003 monkey.dao.pymongo-1.0.0.dev4/monkey.dao.pymongo.egg-info/
--rw-rw-rw-   0        0        0      961 2023-01-28 10:02:01.000000 monkey.dao.pymongo-1.0.0.dev4/monkey.dao.pymongo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      397 2023-01-28 10:02:01.000000 monkey.dao.pymongo-1.0.0.dev4/monkey.dao.pymongo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-28 10:02:01.000000 monkey.dao.pymongo-1.0.0.dev4/monkey.dao.pymongo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-01-28 10:02:01.000000 monkey.dao.pymongo-1.0.0.dev4/monkey.dao.pymongo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-28 10:02:01.000000 monkey.dao.pymongo-1.0.0.dev4/monkey.dao.pymongo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       40 2023-01-28 10:01:16.000000 monkey.dao.pymongo-1.0.0.dev4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-01-28 10:02:01.295760 monkey.dao.pymongo-1.0.0.dev4/setup.cfg
--rw-rw-rw-   0        0        0     1313 2023-01-28 10:01:16.000000 monkey.dao.pymongo-1.0.0.dev4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 06:18:55.453594 monkey.dao.pymongo-1.0.0.dev5/
+-rw-rw-rw-   0        0        0    11556 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev5/LICENSE.txt
+-rw-rw-rw-   0        0        0       60 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev5/MANIFEST.in
+-rw-rw-rw-   0        0        0      961 2023-05-29 06:18:55.450602 monkey.dao.pymongo-1.0.0.dev5/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev5/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-29 06:18:55.400296 monkey.dao.pymongo-1.0.0.dev5/monkey/
+-rw-rw-rw-   0        0        0      103 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev5/monkey/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 06:18:55.431355 monkey.dao.pymongo-1.0.0.dev5/monkey/dao/
+-rw-rw-rw-   0        0        0      103 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev5/monkey/dao/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 06:18:55.442531 monkey.dao.pymongo-1.0.0.dev5/monkey/dao/pymongo/
+-rw-rw-rw-   0        0        0       48 2022-11-21 13:10:48.000000 monkey.dao.pymongo-1.0.0.dev5/monkey/dao/pymongo/__init__.py
+-rw-rw-rw-   0        0        0    10155 2023-05-29 06:09:39.000000 monkey.dao.pymongo-1.0.0.dev5/monkey/dao/pymongo/core.py
+-rw-rw-rw-   0        0        0      415 2023-01-28 09:55:06.000000 monkey.dao.pymongo-1.0.0.dev5/monkey/dao/pymongo/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 06:18:55.428397 monkey.dao.pymongo-1.0.0.dev5/monkey.dao.pymongo.egg-info/
+-rw-rw-rw-   0        0        0      961 2023-05-29 06:18:55.000000 monkey.dao.pymongo-1.0.0.dev5/monkey.dao.pymongo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      446 2023-05-29 06:18:55.000000 monkey.dao.pymongo-1.0.0.dev5/monkey.dao.pymongo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 06:18:55.000000 monkey.dao.pymongo-1.0.0.dev5/monkey.dao.pymongo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-29 06:18:55.000000 monkey.dao.pymongo-1.0.0.dev5/monkey.dao.pymongo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 06:18:55.000000 monkey.dao.pymongo-1.0.0.dev5/monkey.dao.pymongo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       40 2023-05-29 06:17:15.000000 monkey.dao.pymongo-1.0.0.dev5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 06:18:55.454593 monkey.dao.pymongo-1.0.0.dev5/setup.cfg
+-rw-rw-rw-   0        0        0     1313 2023-01-28 10:03:05.000000 monkey.dao.pymongo-1.0.0.dev5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 06:18:55.448605 monkey.dao.pymongo-1.0.0.dev5/tests/
+-rw-rw-rw-   0        0        0      586 2023-01-28 10:01:16.000000 monkey.dao.pymongo-1.0.0.dev5/tests/test_collections.py
+-rw-rw-rw-   0        0        0     1573 2023-01-28 10:01:16.000000 monkey.dao.pymongo-1.0.0.dev5/tests/test_datetime.py
```

### Comparing `monkey.dao.pymongo-1.0.0.dev4/LICENSE.txt` & `monkey.dao.pymongo-1.0.0.dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `monkey.dao.pymongo-1.0.0.dev4/PKG-INFO` & `monkey.dao.pymongo-1.0.0.dev5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkey.dao.pymongo
-Version: 1.0.0.dev4
+Version: 1.0.0.dev5
 Summary: Simple Data Access Object pattern implementation for MongoDB database.
 Home-page: https://bitbucket.org/monkey-python/monkey-dao-pymongo/
 Author: Xavier ROY
 Author-email: xavier@regbuddy.eu
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 1 - Planning
```

### Comparing `monkey.dao.pymongo-1.0.0.dev4/monkey/dao/pymongo/core.py` & `monkey.dao.pymongo-1.0.0.dev5/monkey/dao/pymongo/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,27 @@
         :param projection: a list of field names that should be returned in the result set or a dict specifying the
         fields to include or exclude.
         :return: the found document (if there is one)
         :raise: ObjectNotFoundError
         """
         return self.find_one_by_id(key, projection)
 
+    def find_one_by_seq_num(self, seq_num, projection=None):
+        """Finds a document by its sequence number
+        :param seq_num: id of the document
+        :param projection: a list of field names that should be returned in the result set or a dict specifying the
+        fields to include or exclude.
+        :return: the found document (if there is one)
+        :raise: ObjectNotFoundError
+        """
+        if self.seq_enabled:
+            return self.find_one({self.seq_num_field: seq_num}, projection)
+        else:
+            raise NotImplementedError(f'Sequence number is not enabled for {self.__class__}')
+
     def find(self, query=None, projection=None, skip=0, limit=0, sort=None):
         """Finds records matching the specified query
         :param query: the filter used to query the collection
         :param projection: a list of field names that should be returned in the result set or a dict specifying the
         fields to include or exclude.
         :param skip: the number of record to omit (from the start of the result set) when returning the results
         :param limit: the maximum number of records to return
@@ -174,15 +187,16 @@
         :return: id of the inserted document
         """
         document = {}
         if self.seq_enabled:
             document = {self.seq_num_field: self._get_next_seq_num()}
         document.update(data_set)
         try:
-            result: InsertOneResult = self.collection.insert_one(self._encode_dict(document))
+            encoded_doc = self._encode_dict(document)
+            result: InsertOneResult = self.collection.insert_one(encoded_doc)
             return result.inserted_id
         except PyMongoError as e:
             self.logger.error(f'Failed to insert new document with data: {document}')
             raise PersistenceError('Unexpected error', e)
 
     def _get_next_seq_num(self):
         """Gets the next sequence number value
```

### Comparing `monkey.dao.pymongo-1.0.0.dev4/monkey.dao.pymongo.egg-info/PKG-INFO` & `monkey.dao.pymongo-1.0.0.dev5/monkey.dao.pymongo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkey.dao.pymongo
-Version: 1.0.0.dev4
+Version: 1.0.0.dev5
 Summary: Simple Data Access Object pattern implementation for MongoDB database.
 Home-page: https://bitbucket.org/monkey-python/monkey-dao-pymongo/
 Author: Xavier ROY
 Author-email: xavier@regbuddy.eu
 License: Apache License, Version 2.0
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 1 - Planning
```

### Comparing `monkey.dao.pymongo-1.0.0.dev4/setup.py` & `monkey.dao.pymongo-1.0.0.dev5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import os
 from setuptools import setup, find_packages
 
 __name__ = 'monkey.dao.pymongo'
-__version__ = '1.0.0.dev4'
+__version__ = '1.0.0.dev5'
 __author__ = 'Xavier ROY'
 __author_email__ = 'xavier@regbuddy.eu'
 
 project_dir = os.path.dirname(os.path.realpath(__file__))
 requirement_file_path = project_dir + '/requirements.txt'
 requirements = []
 if os.path.isfile(requirement_file_path):
```


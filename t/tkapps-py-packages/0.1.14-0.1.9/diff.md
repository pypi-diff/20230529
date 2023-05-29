# Comparing `tmp/tkapps_py_packages-0.1.14.tar.gz` & `tmp/tkapps_py_packages-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkapps_py_packages-0.1.14.tar", last modified: Mon May 29 10:25:59 2023, max compression
+gzip compressed data, was "tkapps_py_packages-0.1.9.tar", last modified: Mon May 29 06:36:55 2023, max compression
```

## Comparing `tkapps_py_packages-0.1.14.tar` & `tkapps_py_packages-0.1.9.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 10:25:59.755720 tkapps_py_packages-0.1.14/
--rw-r--r--   0 gyanranjan   (502) staff       (20)     1074 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.14/LICENSE
--rw-r--r--   0 gyanranjan   (502) staff       (20)      853 2023-05-29 10:25:59.754651 tkapps_py_packages-0.1.14/PKG-INFO
--rw-r--r--   0 gyanranjan   (502) staff       (20)      316 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.14/README.md
--rw-r--r--   0 gyanranjan   (502) staff       (20)      657 2023-05-29 10:24:48.000000 tkapps_py_packages-0.1.14/pyproject.toml
--rw-r--r--   0 gyanranjan   (502) staff       (20)       38 2023-05-29 10:25:59.756023 tkapps_py_packages-0.1.14/setup.cfg
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 10:25:59.698845 tkapps_py_packages-0.1.14/src/
--rw-r--r--   0 gyanranjan   (502) staff       (20)        0 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.14/src/__init__.py
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 10:25:59.702698 tkapps_py_packages-0.1.14/src/pusher_notification/
--rw-r--r--   0 gyanranjan   (502) staff       (20)       34 2023-05-24 08:40:12.000000 tkapps_py_packages-0.1.14/src/pusher_notification/__init__.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     1356 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/pusher_notification/pusher_backend.py
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 10:25:59.710770 tkapps_py_packages-0.1.14/src/tkapps_py_packages.egg-info/
--rw-r--r--   0 gyanranjan   (502) staff       (20)      853 2023-05-29 10:25:59.000000 tkapps_py_packages-0.1.14/src/tkapps_py_packages.egg-info/PKG-INFO
--rw-r--r--   0 gyanranjan   (502) staff       (20)      772 2023-05-29 10:25:59.000000 tkapps_py_packages-0.1.14/src/tkapps_py_packages.egg-info/SOURCES.txt
--rw-r--r--   0 gyanranjan   (502) staff       (20)        1 2023-05-29 10:25:59.000000 tkapps_py_packages-0.1.14/src/tkapps_py_packages.egg-info/dependency_links.txt
--rw-r--r--   0 gyanranjan   (502) staff       (20)       15 2023-05-29 10:25:59.000000 tkapps_py_packages-0.1.14/src/tkapps_py_packages.egg-info/requires.txt
--rw-r--r--   0 gyanranjan   (502) staff       (20)       51 2023-05-29 10:25:59.000000 tkapps_py_packages-0.1.14/src/tkapps_py_packages.egg-info/top_level.txt
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 10:25:59.737405 tkapps_py_packages-0.1.14/src/tkaws/
--rw-r--r--   0 gyanranjan   (502) staff       (20)      332 2023-05-29 05:29:31.000000 tkapps_py_packages-0.1.14/src/tkaws/__init__.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     6526 2023-05-29 08:01:56.000000 tkapps_py_packages-0.1.14/src/tkaws/tkathena.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     6538 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/tkaws/tkdynamodb.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     6228 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/tkaws/tkelasticsearch.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     4086 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/tkaws/tkglue.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     2928 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/tkaws/tkkinesis.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     1844 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/tkaws/tklambda.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     7226 2023-05-29 09:24:05.000000 tkapps_py_packages-0.1.14/src/tkaws/tkmongo.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)    17787 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/tkaws/tks3.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     2390 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/tkaws/tkses.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     1095 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/tkaws/tksns.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     2629 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/tkaws/tksqs.py
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 10:25:59.741684 tkapps_py_packages-0.1.14/src/tkemail/
--rw-r--r--   0 gyanranjan   (502) staff       (20)       31 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.14/src/tkemail/__init__.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     3437 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.14/src/tkemail/tkemail.py
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 10:25:59.743631 tkapps_py_packages-0.1.14/src/tkteams/
--rw-r--r--   0 gyanranjan   (502) staff       (20)     8502 2023-05-29 10:24:28.000000 tkapps_py_packages-0.1.14/src/tkteams/__init__.py
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 10:25:59.752769 tkapps_py_packages-0.1.14/tests/
--rw-r--r--   0 gyanranjan   (502) staff       (20)        0 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.14/tests/test_tkdynamodb.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)      706 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.14/tests/test_tkemail.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)      194 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.14/tests/test_tks3.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     1115 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.14/tests/test_tkteams.py
+drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 06:36:55.632168 tkapps_py_packages-0.1.9/
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     1074 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.9/LICENSE
+-rw-r--r--   0 gyanranjan   (502) staff       (20)      852 2023-05-29 06:36:55.630848 tkapps_py_packages-0.1.9/PKG-INFO
+-rw-r--r--   0 gyanranjan   (502) staff       (20)      316 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.9/README.md
+-rw-r--r--   0 gyanranjan   (502) staff       (20)      608 2023-05-29 06:36:42.000000 tkapps_py_packages-0.1.9/pyproject.toml
+-rw-r--r--   0 gyanranjan   (502) staff       (20)       38 2023-05-29 06:36:55.632421 tkapps_py_packages-0.1.9/setup.cfg
+drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 06:36:55.573694 tkapps_py_packages-0.1.9/src/
+-rw-r--r--   0 gyanranjan   (502) staff       (20)        0 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.9/src/__init__.py
+drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 06:36:55.575682 tkapps_py_packages-0.1.9/src/pusher_notification/
+-rw-r--r--   0 gyanranjan   (502) staff       (20)       34 2023-05-24 08:40:12.000000 tkapps_py_packages-0.1.9/src/pusher_notification/__init__.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     1356 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/pusher_notification/pusher_backend.py
+drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 06:36:55.583212 tkapps_py_packages-0.1.9/src/tkapps_py_packages.egg-info/
+-rw-r--r--   0 gyanranjan   (502) staff       (20)      852 2023-05-29 06:36:55.000000 tkapps_py_packages-0.1.9/src/tkapps_py_packages.egg-info/PKG-INFO
+-rw-r--r--   0 gyanranjan   (502) staff       (20)      771 2023-05-29 06:36:55.000000 tkapps_py_packages-0.1.9/src/tkapps_py_packages.egg-info/SOURCES.txt
+-rw-r--r--   0 gyanranjan   (502) staff       (20)        1 2023-05-29 06:36:55.000000 tkapps_py_packages-0.1.9/src/tkapps_py_packages.egg-info/dependency_links.txt
+-rw-r--r--   0 gyanranjan   (502) staff       (20)       51 2023-05-29 06:36:55.000000 tkapps_py_packages-0.1.9/src/tkapps_py_packages.egg-info/top_level.txt
+drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 06:36:55.613187 tkapps_py_packages-0.1.9/src/tkaws/
+-rw-r--r--   0 gyanranjan   (502) staff       (20)      332 2023-05-29 05:29:31.000000 tkapps_py_packages-0.1.9/src/tkaws/__init__.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     6524 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tkathena.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     6538 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tkdynamodb.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     6228 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tkelasticsearch.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     4086 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tkglue.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     2928 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tkkinesis.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     1844 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tklambda.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     7830 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tkmongo.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)    17787 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tks3.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     2390 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tkses.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     1095 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tksns.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     2629 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkaws/tksqs.py
+drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 06:36:55.617590 tkapps_py_packages-0.1.9/src/tkemail/
+-rw-r--r--   0 gyanranjan   (502) staff       (20)       31 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.9/src/tkemail/__init__.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     3437 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkemail/tkemail.py
+drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 06:36:55.623229 tkapps_py_packages-0.1.9/src/tkteams/
+-rw-r--r--   0 gyanranjan   (502) staff       (20)       56 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.9/src/tkteams/__init__.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     6262 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.9/src/tkteams/message.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     2208 2023-05-29 06:30:56.000000 tkapps_py_packages-0.1.9/src/tkteams/teams.py
+drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 06:36:55.629552 tkapps_py_packages-0.1.9/tests/
+-rw-r--r--   0 gyanranjan   (502) staff       (20)        0 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.9/tests/test_tkdynamodb.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)      706 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.9/tests/test_tkemail.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)      194 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.9/tests/test_tks3.py
+-rw-r--r--   0 gyanranjan   (502) staff       (20)     1115 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.9/tests/test_tkteams.py
```

### Comparing `tkapps_py_packages-0.1.14/LICENSE` & `tkapps_py_packages-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/PKG-INFO` & `tkapps_py_packages-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkapps_py_packages
-Version: 0.1.14
+Version: 0.1.9
 Summary: A common package to be used across multiple projects
 Author-email: Gyan Ranjan <granjan@tekion.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tkapps_py_packages-0.1.14/pyproject.toml` & `tkapps_py_packages-0.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tkapps_py_packages"
-version = "0.1.14"
+version = "0.1.9"
 authors = [
   { name="Gyan Ranjan", email="granjan@tekion.com" },
 ]
 description = "A common package to be used across multiple projects"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = [
-    "pymongo",
-    "pusher",
-]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `tkapps_py_packages-0.1.14/src/pusher_notification/pusher_backend.py` & `tkapps_py_packages-0.1.9/src/pusher_notification/pusher_backend.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkapps_py_packages.egg-info/PKG-INFO` & `tkapps_py_packages-0.1.9/src/tkapps_py_packages.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkapps-py-packages
-Version: 0.1.14
+Version: 0.1.9
 Summary: A common package to be used across multiple projects
 Author-email: Gyan Ranjan <granjan@tekion.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tkapps_py_packages-0.1.14/src/tkapps_py_packages.egg-info/SOURCES.txt` & `tkapps_py_packages-0.1.9/src/tkapps_py_packages.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 src/__init__.py
 src/pusher_notification/__init__.py
 src/pusher_notification/pusher_backend.py
 src/tkapps_py_packages.egg-info/PKG-INFO
 src/tkapps_py_packages.egg-info/SOURCES.txt
 src/tkapps_py_packages.egg-info/dependency_links.txt
-src/tkapps_py_packages.egg-info/requires.txt
 src/tkapps_py_packages.egg-info/top_level.txt
 src/tkaws/__init__.py
 src/tkaws/tkathena.py
 src/tkaws/tkdynamodb.py
 src/tkaws/tkelasticsearch.py
 src/tkaws/tkglue.py
 src/tkaws/tkkinesis.py
@@ -20,11 +19,13 @@
 src/tkaws/tks3.py
 src/tkaws/tkses.py
 src/tkaws/tksns.py
 src/tkaws/tksqs.py
 src/tkemail/__init__.py
 src/tkemail/tkemail.py
 src/tkteams/__init__.py
+src/tkteams/message.py
+src/tkteams/teams.py
 tests/test_tkdynamodb.py
 tests/test_tkemail.py
 tests/test_tks3.py
 tests/test_tkteams.py
```

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tkathena.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkathena.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 import boto3
+from tks3 import Tks3
 
 
 class Tkathena:
     def __init__(self, region=None):
         """
         :param region: The region for AWS Athena
         """
@@ -114,26 +115,26 @@
             },
             ResultConfiguration={
                 'OutputLocation': output_location
             }
         )
         return response['QueryExecutionId']
 
-    # def get_output_location(self, output_path, database, query, report_name):
-    #     try:
-    #         execution_id = self.get_query_state(output_path, database, query)
-    #         if execution_id:
-    #             output_loc = output_path + "/" + str(execution_id) + ".csv"
-    #             final_path = output_path + "/" + str(report_name) + '.csv'
-    #             output_key = output_loc.split("//")[1]
-    #             final_key = final_path.split("//")[1]
-    #             Tks3().rename_s3_object(output_key, final_key)
-    #             return True
-    #     except Exception as err:
-    #         print(err)
+    def get_output_location(self, output_path, database, query, report_name):
+        try:
+            execution_id = self.get_query_state(output_path, database, query)
+            if execution_id:
+                output_loc = output_path + "/" + str(execution_id) + ".csv"
+                final_path = output_path + "/" + str(report_name) + '.csv'
+                output_key = output_loc.split("//")[1]
+                final_key = final_path.split("//")[1]
+                Tks3().rename_s3_object(output_key, final_key)
+                return True
+        except Exception as err:
+            print(err)
 
     def get_query_state(self, output_path, database, query):
         """
         param: output_path, database, query
         desc:from get query execution and execution_id the status is  printed.
         return: execution_id for success and false on failure
         """
```

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tkdynamodb.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkdynamodb.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tkelasticsearch.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkelasticsearch.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tkglue.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkglue.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tkkinesis.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkkinesis.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tklambda.py` & `tkapps_py_packages-0.1.9/src/tkaws/tklambda.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tkmongo.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkmongo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,38 @@
 import os
 from pymongo import MongoClient
 # from pandas import DataFrame
 from bson import json_util, BSON
 from bson import Binary, Code, ObjectId, Int64, Any
 import os, json
 import urllib.parse
-# from tklogs import Tkauditlogs
+from tklogs import Tkauditlogs
+
+# 13th March 2023 - Depreciated and to be removed in future after confirmation from saurav rawat.
+class NumberLong(int):
+    """Representation of the BSON int64 type.
+
+    This is necessary because every integral number is an :class:`int` in
+    Python 3. Small integral numbers are encoded to BSON int32 by default,
+    but Int64 numbers will always be encoded to BSON int64.
+
+    :Parameters:
+      - `value`: the numeric value to represent
+    """
+
+    __slots__ = ()
+
+    _type_marker = 18
+
+    def __getstate__(self) -> Any:
+        return {}
+
+    def __setstate__(self, state: Any) -> None:
+        pass
+
 
 class Tkmongo:
     def __init__(self, db_name=None):
         """
         :param dbname: The database name in mongo db.
         """
         if db_name is None:
@@ -39,30 +62,30 @@
         :param collection_name: The name of the collection in which the document will be inserted
         :param document: Document that will be inserted in the collection
         :param audit_log: Do we need audit Logs (False by default)
         :return:
         """
         if audit_log is True:
             old_document = self.fetch_document_by_id(collection_name, document['id'])
-            # Tkauditlogs().put_mongo_log(document, old_document, username='None')
+            Tkauditlogs().put_mongo_log(document, old_document, username='None')
         collection = self.get_collection(collection_name)
         return collection.insert_one(document)
 
 
     def update_document(self, collection_name, query, document, audit_log=False):
         """
         :param collection_name: The name of the collection in which the document will be inserted
         :param query: The Query to Update the Document
         :param document: The document which will be updated.
         :param audit_log: Do we need audit Logs (False by default)
         :return: Generic PyMongo response for "update_one"
         """
         if audit_log is True:
             old_document = self.fetch_document_by_id(collection_name, document['id'])
-            # Tkauditlogs().put_mongo_log(document, old_document, username=None)
+            Tkauditlogs().put_mongo_log(document, old_document, username=None)
         collection = self.get_collection(collection_name)
         return collection.update_one(query, document)
 
     def update_many_document(self, collection_name, query, document):
         """
         :param collection_name: The name of the collection in which the document will be inserted
         :param query: The Query to Update the Document
@@ -78,15 +101,15 @@
         :param query: The Query to Replace the Document
         :param document: The document which will be replaced.
         :param audit_log: Do we need audit Logs (False by default)
         :return: Generic PyMongo response for "replace_one"
         """
         if audit_log is True:
             old_document = self.fetch_document_by_id(collection_name, document['id'])
-            # Tkauditlogs().put_mongo_log(document, old_document, username=None)
+            Tkauditlogs().put_mongo_log(document, old_document, username=None)
         collection = self.get_collection(collection_name)
         return collection.replace_one(query, document)
 
     def insert_many_document(self, collection_name, documents):
         """
         :param collection_name: The name of the collection in which the document will be inserted
         :param documents: Document that will be inserted in the collection
```

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tks3.py` & `tkapps_py_packages-0.1.9/src/tkaws/tks3.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tkses.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkses.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tksns.py` & `tkapps_py_packages-0.1.9/src/tkaws/tksns.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkaws/tksqs.py` & `tkapps_py_packages-0.1.9/src/tkaws/tksqs.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkemail/tkemail.py` & `tkapps_py_packages-0.1.9/src/tkemail/tkemail.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/src/tkteams/__init__.py` & `tkapps_py_packages-0.1.9/src/tkteams/message.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,73 +1,9 @@
-import os
-import requests
-
-class Teams():
-    def __init__(self, webhook_url=None):
-        """
-        :param webhook_url: The Webhook url from the teams
-        """
-        if webhook_url is None:
-            try:
-                webhook_url = os.environ["WEBHOOK_URL"]
-            except Exception:
-                raise ValueError("WEBHOOK_URL is missing in both ENV Variable and constructor params.")
-        self.webhook_url = webhook_url
-        self.http_timeout = 60
-
-    def change_webhook(self, new_webhook):
-        """
-        :param new_webhook: the new webhook that will replace the older webhook
-        :return: none
-        """
-        self.webhook_url = new_webhook
-
-    def send_to_multiple_channels(self, webhooks_list, message):
-        """
-        :param webhooks_list: The list of webhooks where the message will be sent.
-        :param message: The message that will be posted across all the channels.
-        :return: None
-        """
-        for webhook_url in webhooks_list:
-            self.webhook_url = webhook_url
-            self.send_message(message)
-
-    def _validate_message(self, message):
-        """
-        :param message: The message that is to be sent to the teams channel should be of type Message
-        :return: Boolean
-        """
-        if type(message) != type(Message()):
-            raise ValueError("Object not of type Message")
-        if 'text' not in message.data:
-            raise ValueError("Message is empty!")
-        return True
-
-    def send_message(self, message):
-        """
-        :param message: The message that is to be sent to the teams channel should be of type Message
-        :return: Boolean (Status of message)
-        """
-        # self._validate_message(message)
-        headers = {"Content-Type": "application/json"}
-        r = requests.post(
-            self.webhook_url,
-            json=message.message,
-            headers=headers,
-            timeout=self.http_timeout,
-        )
-        self.last_http_response = r
-        if r.status_code == requests.codes.ok:  # pylint: disable=no-member
-            return True
-        else:
-            print(r.text)
-            raise r.raise_for_status()
-
-
-class Message():
+from teams import Teams
+class Message:
     def __init__(self, text=None):
         self.message = {"type": "message", "attachments": list()}
         self.message_data = dict()
         self.message_content = dict()
         self.message_data["contentType"] = "application/vnd.microsoft.card.adaptive"
         self.message_content["$schema"] = "http://adaptivecards.io/schemas/adaptive-card.json"
         self.message_content["version"] = "1.4"
@@ -132,16 +68,14 @@
 
     def mention_user(self, user_email, user_name=None):
         """
         :param user_email: User Email of the mentioned user
         :param user_name: Name of the mentioned user (this value should match in any of the text blocks)
         :return:
         """
-        if user_name is None:
-            user_name = user_email
         user_found = False
         for text_blocks in self.message_content['body']:
             if 'text' in text_blocks and user_name in text_blocks['text']:
                 user_found = True
                 text_blocks['text'] = text_blocks['text'].replace(user_name, f"<at>{user_name}</at>")
         if user_found is True:
             user_mention = {"type": "mention", "text": f"<at>{user_name}</at>", "mentioned": {"id": user_email, "name": user_name}}
@@ -216,15 +150,15 @@
     def print(self):
         """
         prints the entire message object for user to debug.
         """
         print(self.message)
 
 
-    def send(self, webhook=None):
+    def send(self):
         """
         :return: Response from Teams after sending the message
         """
-        response = Teams(webhook).send_message(self)
+        response = Teams().send_message(self.message)
         return response
```

### Comparing `tkapps_py_packages-0.1.14/tests/test_tkemail.py` & `tkapps_py_packages-0.1.9/tests/test_tkemail.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.14/tests/test_tkteams.py` & `tkapps_py_packages-0.1.9/tests/test_tkteams.py`

 * *Files identical despite different names*


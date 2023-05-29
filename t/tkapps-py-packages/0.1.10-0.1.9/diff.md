# Comparing `tmp/tkapps_py_packages-0.1.10.tar.gz` & `tmp/tkapps_py_packages-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkapps_py_packages-0.1.10.tar", last modified: Mon May 29 08:02:48 2023, max compression
+gzip compressed data, was "tkapps_py_packages-0.1.9.tar", last modified: Mon May 29 06:36:55 2023, max compression
```

## Comparing `tkapps_py_packages-0.1.10.tar` & `tkapps_py_packages-0.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 08:02:48.199906 tkapps_py_packages-0.1.10/
--rw-r--r--   0 gyanranjan   (502) staff       (20)     1074 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.10/LICENSE
--rw-r--r--   0 gyanranjan   (502) staff       (20)      853 2023-05-29 08:02:48.198928 tkapps_py_packages-0.1.10/PKG-INFO
--rw-r--r--   0 gyanranjan   (502) staff       (20)      316 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.10/README.md
--rw-r--r--   0 gyanranjan   (502) staff       (20)      609 2023-05-29 08:02:35.000000 tkapps_py_packages-0.1.10/pyproject.toml
--rw-r--r--   0 gyanranjan   (502) staff       (20)       38 2023-05-29 08:02:48.200154 tkapps_py_packages-0.1.10/setup.cfg
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 08:02:48.152797 tkapps_py_packages-0.1.10/src/
--rw-r--r--   0 gyanranjan   (502) staff       (20)        0 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.10/src/__init__.py
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 08:02:48.155752 tkapps_py_packages-0.1.10/src/pusher_notification/
--rw-r--r--   0 gyanranjan   (502) staff       (20)       34 2023-05-24 08:40:12.000000 tkapps_py_packages-0.1.10/src/pusher_notification/__init__.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     1356 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/pusher_notification/pusher_backend.py
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 08:02:48.161326 tkapps_py_packages-0.1.10/src/tkapps_py_packages.egg-info/
--rw-r--r--   0 gyanranjan   (502) staff       (20)      853 2023-05-29 08:02:48.000000 tkapps_py_packages-0.1.10/src/tkapps_py_packages.egg-info/PKG-INFO
--rw-r--r--   0 gyanranjan   (502) staff       (20)      771 2023-05-29 08:02:48.000000 tkapps_py_packages-0.1.10/src/tkapps_py_packages.egg-info/SOURCES.txt
--rw-r--r--   0 gyanranjan   (502) staff       (20)        1 2023-05-29 08:02:48.000000 tkapps_py_packages-0.1.10/src/tkapps_py_packages.egg-info/dependency_links.txt
--rw-r--r--   0 gyanranjan   (502) staff       (20)       51 2023-05-29 08:02:48.000000 tkapps_py_packages-0.1.10/src/tkapps_py_packages.egg-info/top_level.txt
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 08:02:48.181648 tkapps_py_packages-0.1.10/src/tkaws/
--rw-r--r--   0 gyanranjan   (502) staff       (20)      332 2023-05-29 05:29:31.000000 tkapps_py_packages-0.1.10/src/tkaws/__init__.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     6526 2023-05-29 08:01:56.000000 tkapps_py_packages-0.1.10/src/tkaws/tkathena.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     6538 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkaws/tkdynamodb.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     6228 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkaws/tkelasticsearch.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     4086 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkaws/tkglue.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     2928 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkaws/tkkinesis.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     1844 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkaws/tklambda.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     7830 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkaws/tkmongo.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)    17787 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkaws/tks3.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     2390 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkaws/tkses.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     1095 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkaws/tksns.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     2629 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkaws/tksqs.py
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 08:02:48.184342 tkapps_py_packages-0.1.10/src/tkemail/
--rw-r--r--   0 gyanranjan   (502) staff       (20)       31 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.10/src/tkemail/__init__.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     3437 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkemail/tkemail.py
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 08:02:48.189933 tkapps_py_packages-0.1.10/src/tkteams/
--rw-r--r--   0 gyanranjan   (502) staff       (20)       56 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.10/src/tkteams/__init__.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     6262 2023-05-29 06:32:36.000000 tkapps_py_packages-0.1.10/src/tkteams/message.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     2208 2023-05-29 06:30:56.000000 tkapps_py_packages-0.1.10/src/tkteams/teams.py
-drwxr-xr-x   0 gyanranjan   (502) staff       (20)        0 2023-05-29 08:02:48.197211 tkapps_py_packages-0.1.10/tests/
--rw-r--r--   0 gyanranjan   (502) staff       (20)        0 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.10/tests/test_tkdynamodb.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)      706 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.10/tests/test_tkemail.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)      194 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.10/tests/test_tks3.py
--rw-r--r--   0 gyanranjan   (502) staff       (20)     1115 2023-05-24 08:38:30.000000 tkapps_py_packages-0.1.10/tests/test_tkteams.py
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

### Comparing `tkapps_py_packages-0.1.10/LICENSE` & `tkapps_py_packages-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/PKG-INFO` & `tkapps_py_packages-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkapps_py_packages
-Version: 0.1.10
+Version: 0.1.9
 Summary: A common package to be used across multiple projects
 Author-email: Gyan Ranjan <granjan@tekion.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tkapps_py_packages-0.1.10/pyproject.toml` & `tkapps_py_packages-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tkapps_py_packages"
-version = "0.1.10"
+version = "0.1.9"
 authors = [
   { name="Gyan Ranjan", email="granjan@tekion.com" },
 ]
 description = "A common package to be used across multiple projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `tkapps_py_packages-0.1.10/src/pusher_notification/pusher_backend.py` & `tkapps_py_packages-0.1.9/src/pusher_notification/pusher_backend.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkapps_py_packages.egg-info/PKG-INFO` & `tkapps_py_packages-0.1.9/src/tkapps_py_packages.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkapps-py-packages
-Version: 0.1.10
+Version: 0.1.9
 Summary: A common package to be used across multiple projects
 Author-email: Gyan Ranjan <granjan@tekion.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tkapps_py_packages-0.1.10/src/tkapps_py_packages.egg-info/SOURCES.txt` & `tkapps_py_packages-0.1.9/src/tkapps_py_packages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tkathena.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkathena.py`

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

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tkdynamodb.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkdynamodb.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tkelasticsearch.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkelasticsearch.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tkglue.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkglue.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tkkinesis.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkkinesis.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tklambda.py` & `tkapps_py_packages-0.1.9/src/tkaws/tklambda.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tkmongo.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkmongo.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tks3.py` & `tkapps_py_packages-0.1.9/src/tkaws/tks3.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tkses.py` & `tkapps_py_packages-0.1.9/src/tkaws/tkses.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tksns.py` & `tkapps_py_packages-0.1.9/src/tkaws/tksns.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkaws/tksqs.py` & `tkapps_py_packages-0.1.9/src/tkaws/tksqs.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkemail/tkemail.py` & `tkapps_py_packages-0.1.9/src/tkemail/tkemail.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkteams/message.py` & `tkapps_py_packages-0.1.9/src/tkteams/message.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/src/tkteams/teams.py` & `tkapps_py_packages-0.1.9/src/tkteams/teams.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/tests/test_tkemail.py` & `tkapps_py_packages-0.1.9/tests/test_tkemail.py`

 * *Files identical despite different names*

### Comparing `tkapps_py_packages-0.1.10/tests/test_tkteams.py` & `tkapps_py_packages-0.1.9/tests/test_tkteams.py`

 * *Files identical despite different names*


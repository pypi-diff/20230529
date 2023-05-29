# Comparing `tmp/citros-23.19.1.tar.gz` & `tmp/citros-23.19.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.19.1.tar", last modified: Tue May  9 11:03:27 2023, max compression
+gzip compressed data, was "citros-23.19.2.tar", last modified: Wed May 17 07:41:11 2023, max compression
```

## Comparing `citros-23.19.1.tar` & `citros-23.19.2.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-09 11:03:09.000000 citros-23.19.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-09 11:03:27.239459 citros-23.19.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-09 11:03:09.000000 citros-23.19.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.235459 citros-23.19.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-05-09 11:03:09.000000 citros-23.19.1/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.235459 citros-23.19.1/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-09 11:03:09.000000 citros-23.19.1/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13315 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-09 11:03:09.000000 citros-23.19.1/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-09 11:03:09.000000 citros-23.19.1/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-05-09 11:03:09.000000 citros-23.19.1/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-09 11:03:09.000000 citros-23.19.1/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-09 11:03:09.000000 citros-23.19.1/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-09 11:03:09.000000 citros-23.19.1/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-09 11:03:09.000000 citros-23.19.1/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 11:03:09.000000 citros-23.19.1/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-05-09 11:03:09.000000 citros-23.19.1/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-09 11:03:09.000000 citros-23.19.1/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-09 11:03:09.000000 citros-23.19.1/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-09 11:03:09.000000 citros-23.19.1/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-09 11:03:09.000000 citros-23.19.1/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-09 11:03:27.000000 citros-23.19.1/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-09 11:03:27.000000 citros-23.19.1/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 11:03:27.000000 citros-23.19.1/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-09 11:03:27.000000 citros-23.19.1/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 11:03:27.000000 citros-23.19.1/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-09 11:03:09.000000 citros-23.19.1/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 11:03:27.239459 citros-23.19.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-09 11:03:09.000000 citros-23.19.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:27.239459 citros-23.19.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:09.000000 citros-23.19.1/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 11:03:09.000000 citros-23.19.1/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:41:11.725254 citros-23.19.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 07:40:53.000000 citros-23.19.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-17 07:41:11.725254 citros-23.19.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-17 07:40:53.000000 citros-23.19.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:41:11.717255 citros-23.19.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-05-17 07:40:53.000000 citros-23.19.2/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:41:11.721254 citros-23.19.2/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-17 07:40:53.000000 citros-23.19.2/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13412 2023-05-17 07:40:53.000000 citros-23.19.2/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-05-17 07:40:53.000000 citros-23.19.2/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-17 07:40:53.000000 citros-23.19.2/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-17 07:40:53.000000 citros-23.19.2/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-05-17 07:40:53.000000 citros-23.19.2/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9832 2023-05-17 07:40:53.000000 citros-23.19.2/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-17 07:40:53.000000 citros-23.19.2/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:41:11.721254 citros-23.19.2/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-17 07:40:53.000000 citros-23.19.2/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12075 2023-05-17 07:40:53.000000 citros-23.19.2/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:41:11.725254 citros-23.19.2/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-17 07:40:53.000000 citros-23.19.2/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-17 07:40:53.000000 citros-23.19.2/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-17 07:40:53.000000 citros-23.19.2/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:41:11.725254 citros-23.19.2/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-17 07:40:53.000000 citros-23.19.2/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-17 07:40:53.000000 citros-23.19.2/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11395 2023-05-17 07:40:53.000000 citros-23.19.2/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:41:11.725254 citros-23.19.2/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-17 07:40:53.000000 citros-23.19.2/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-17 07:40:53.000000 citros-23.19.2/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-17 07:40:53.000000 citros-23.19.2/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-17 07:40:53.000000 citros-23.19.2/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:41:11.721254 citros-23.19.2/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-17 07:41:11.000000 citros-23.19.2/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-17 07:41:11.000000 citros-23.19.2/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 07:41:11.000000 citros-23.19.2/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-17 07:41:11.000000 citros-23.19.2/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-17 07:41:11.000000 citros-23.19.2/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-17 07:40:53.000000 citros-23.19.2/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 07:41:11.725254 citros-23.19.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2038 2023-05-17 07:40:53.000000 citros-23.19.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 07:41:11.725254 citros-23.19.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:40:53.000000 citros-23.19.2/tests/test_parse_ros_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 07:40:53.000000 citros-23.19.2/tests/test_uplosd_to_server.py
```

### Comparing `citros-23.19.1/LICENSE` & `citros-23.19.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/PKG-INFO` & `citros-23.19.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.19.1
+Version: 23.19.2
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.19.1/README.md` & `citros-23.19.2/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/bin/citros` & `citros-23.19.2/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/__init__.py` & `citros-23.19.2/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/citros.py` & `citros-23.19.2/citros/citros.py`

 * *Files 0% similar despite different names*

```diff
@@ -233,15 +233,16 @@
             token = result["authenticate"]["jwt"]
         else:
             print("ERROR: failed to log in. resp: ", result)
             token = None
             return False
         
         try:
-            decoded = jwt.decode(token, options={"verify_signature": False})        
+            # bug fix. addede audience as it didnt work in some cases. 
+            decoded = jwt.decode(token, options={"verify_signature": False}, audience="postgraphile")        
             # print("decoded: ", decoded)
         except Exception as err:     
             print("ERROR: failed to log in. token: ", token) 
             self.log.exception(err)        
             traceback.print_exc()
             return False
```

### Comparing `citros-23.19.1/citros/citros_bag.py` & `citros-23.19.2/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/citros_batch.py` & `citros-23.19.2/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/citros_events.py` & `citros-23.19.2/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/citros_integration.py` & `citros-23.19.2/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/citros_params.py` & `citros-23.19.2/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/citros_utils.py` & `citros-23.19.2/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/launches/__init__.py` & `citros-23.19.2/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/launches/launch.py` & `citros-23.19.2/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/logger/__init__.py` & `citros-23.19.2/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/logger/logger.py` & `citros-23.19.2/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/logger/logger_pg_handler.py` & `citros-23.19.2/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/parsers/__init__.py` & `citros-23.19.2/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/parsers/parser_ros2.py` & `citros-23.19.2/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/rosbag/__init__.py` & `citros-23.19.2/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/rosbag/reader_base.py` & `citros-23.19.2/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/rosbag/reader_mcap.py` & `citros-23.19.2/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros/rosbag/reader_sqlite.py` & `citros-23.19.2/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/citros.egg-info/PKG-INFO` & `citros-23.19.2/citros.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.19.1
+Version: 23.19.2
 Summary: A cli entypoint for citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.19.1/citros.egg-info/SOURCES.txt` & `citros-23.19.2/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.19.1/setup.py` & `citros-23.19.2/setup.py`

 * *Files identical despite different names*


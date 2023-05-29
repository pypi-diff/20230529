# Comparing `tmp/syncanysql-0.1.4.tar.gz` & `tmp/syncanysql-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.1.4.tar", last modified: Fri May 26 10:44:08 2023, max compression
+gzip compressed data, was "syncanysql-0.1.5.tar", last modified: Mon May 29 10:04:48 2023, max compression
```

## Comparing `syncanysql-0.1.4.tar` & `syncanysql-0.1.5.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:08.178205 syncanysql-0.1.4/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-26 10:44:08.179206 syncanysql-0.1.4/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3018 2023-04-25 10:14:55.000000 syncanysql-0.1.4/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-26 10:44:08.189200 syncanysql-0.1.4/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2006 2023-05-26 07:22:02.000000 syncanysql-0.1.4/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:06.626398 syncanysql-0.1.4/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9167 2023-04-26 01:56:02.000000 syncanysql-0.1.4/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:07.190394 syncanysql-0.1.4/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1256 2023-05-26 03:51:27.000000 syncanysql-0.1.4/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6162 2023-05-23 08:35:54.000000 syncanysql-0.1.4/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      722 2023-05-26 03:56:52.000000 syncanysql-0.1.4/syncanysql/calculaters/env_variable_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:07.564024 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-05-17 08:58:39.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10197 2023-05-04 10:22:31.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6193 2023-04-24 06:11:11.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   171950 2023-05-26 07:01:52.000000 syncanysql-0.1.4/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12804 2023-05-08 04:32:02.000000 syncanysql-0.1.4/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.4/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8602 2023-05-26 04:09:39.000000 syncanysql-0.1.4/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3750 2023-04-26 01:56:02.000000 syncanysql-0.1.4/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.4/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6965 2023-04-27 09:10:45.000000 syncanysql-0.1.4/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:08.125182 syncanysql-0.1.4/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.4/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.4/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.4/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.4/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4258 2023-04-26 01:31:23.000000 syncanysql-0.1.4/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    20959 2023-05-18 08:15:36.000000 syncanysql-0.1.4/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2890 2023-05-08 04:04:28.000000 syncanysql-0.1.4/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.4/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.4/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      754 2023-05-08 04:04:28.000000 syncanysql-0.1.4/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-05-17 03:49:43.000000 syncanysql-0.1.4/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:06.924782 syncanysql-0.1.4/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.4/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      394 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:48.583557 syncanysql-0.1.5/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1063 2023-02-07 08:27:23.000000 syncanysql-0.1.5/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-29 10:04:48.584557 syncanysql-0.1.5/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3018 2023-04-25 10:14:55.000000 syncanysql-0.1.5/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-29 10:04:48.594529 syncanysql-0.1.5/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2007 2023-05-27 14:11:29.000000 syncanysql-0.1.5/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:47.148615 syncanysql-0.1.5/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9167 2023-04-26 01:56:02.000000 syncanysql-0.1.5/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:47.667528 syncanysql-0.1.5/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1319 2023-05-29 09:21:36.000000 syncanysql-0.1.5/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6842 2023-05-29 09:21:36.000000 syncanysql-0.1.5/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      722 2023-05-26 03:56:52.000000 syncanysql-0.1.5/syncanysql/calculaters/env_variable_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:48.047552 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      384 2023-05-29 03:23:56.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10475 2023-05-27 08:55:29.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2860 2023-05-29 05:03:18.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/logical_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6764 2023-05-29 05:01:09.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   177108 2023-05-29 09:59:09.000000 syncanysql-0.1.5/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    13459 2023-05-27 14:11:29.000000 syncanysql-0.1.5/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.5/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8633 2023-05-28 13:31:45.000000 syncanysql-0.1.5/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3750 2023-04-26 01:56:02.000000 syncanysql-0.1.5/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.5/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6965 2023-04-27 09:10:45.000000 syncanysql-0.1.5/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:48.536527 syncanysql-0.1.5/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.5/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.5/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.5/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.5/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4258 2023-04-26 01:31:23.000000 syncanysql-0.1.5/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    23474 2023-05-28 14:28:58.000000 syncanysql-0.1.5/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2890 2023-05-08 04:04:28.000000 syncanysql-0.1.5/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.5/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.5/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      754 2023-05-08 04:04:28.000000 syncanysql-0.1.5/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-05-27 07:49:00.000000 syncanysql-0.1.5/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:04:47.440030 syncanysql-0.1.5/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-29 10:04:45.000000 syncanysql-0.1.5/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-05-29 10:04:46.000000 syncanysql-0.1.5/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-29 10:04:45.000000 syncanysql-0.1.5/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-05-29 10:04:45.000000 syncanysql-0.1.5/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.5/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      395 2023-05-29 10:04:45.000000 syncanysql-0.1.5/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-05-29 10:04:45.000000 syncanysql-0.1.5/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.1.4/PKG-INFO` & `syncanysql-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.1.4/README.md` & `syncanysql-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/setup.py` & `syncanysql-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.1.4"
+version = "0.1.5"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -34,15 +34,15 @@
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
         "sqlglot>=11.5.5,<12",
-        "syncany>=0.2.9",
+        "syncany>=0.2.11",
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
         "pymysql": ['PyMySQL>=0.8.1'],
```

### Comparing `syncanysql-0.1.4/syncanysql/__init__.py` & `syncanysql-0.1.5/syncanysql/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/calculaters/__init__.py` & `syncanysql-0.1.5/syncanysql/calculaters/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     "mysql": MysqlCalculater,
     "aggregate_key": AggregateKeyCalculater,
     "aggregate_count": AggregateCountCalculater,
     "aggregate_sum": AggregateSumCalculater,
     "aggregate_max": AggregateMaxCalculater,
     "aggregate_min": AggregateMinCalculater,
     "aggregate_avg": AggregateAvgCalculater,
+    "aggregate_group_concat": AggregateGroupConcatCalculater,
 }
 CALCULATERS.update(SQL_CALCULATERS)
 
 
 def is_mysql_func(name):
     if MysqlCalculater.funcs is None:
         MysqlCalculater.find_func(name)
```

### Comparing `syncanysql-0.1.4/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.1.5/syncanysql/calculaters/aggregate_calculater.py`

 * *Files 5% similar despite different names*

```diff
@@ -173,7 +173,29 @@
         return {"count_value": state_value["count_value"] + data_value["count_value"],
                 "sum_value": state_value["sum_value"] + data_value["sum_value"]}
 
     def final_value(self, state_value):
         if state_value is None:
             return 0
         return state_value["sum_value"] / state_value["count_value"]
+
+
+class AggregateGroupConcatCalculater(StateAggregateCalculater):
+    def aggregate(self, state_value, data_value):
+        if data_value is None:
+            return state_value
+        if state_value is None:
+            return [str(data_value)]
+        state_value.append(str(data_value))
+        return state_value
+
+    def reduce(self, state_value, data_value):
+        if data_value is None:
+            return state_value
+        if state_value is None:
+            return data_value
+        return state_value + data_value
+
+    def final_value(self, state_value):
+        if not state_value:
+            return ""
+        return ",".join(state_value)
```

### Comparing `syncanysql-0.1.4/syncanysql/calculaters/env_variable_calculater.py` & `syncanysql-0.1.5/syncanysql/calculaters/env_variable_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.1.5/syncanysql/calculaters/mysql_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,15 +149,22 @@
     return dt.weekday() + 1
 
 def mysql_week(dt, mod=None):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
-    return int(dt.strftime("%U"))
+    return int(dt.strftime("%W" if str(mod) == "1" else "%U"))
+
+def mysql_yearweek(dt, mod=None):
+    if dt is None:
+        return None
+    if isinstance(dt, (int, float, str)):
+        dt = parse_datetime(str(dt), None, get_timezone())
+    return int(dt.strftime("%Y%W" if str(mod) == "1" else "%Y%U"))
 
 def mysql_dayofyear(dt):
     if dt is None:
         return None
     if isinstance(dt, (int, float, str)):
         dt = parse_datetime(str(dt), None, get_timezone())
     return int(dt.strftime("%j"))
```

### Comparing `syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/number_funcs.py` & `syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/number_funcs.py`

 * *Files 6% similar despite different names*

```diff
@@ -64,16 +64,36 @@
         except:
             return parse_number(x, True)
     return float(x)
 
 def ensure_number(x):
     if isinstance(x, (int, float)):
         return x
-    if isinstance(x, str) and "." in x:
-        return ensure_float(x)
+    if x is None:
+        raise ValueError('value is None')
+    if not x:
+        return 0
+    if x is True:
+        return 1
+    if isinstance(x, str):
+        if "." in x:
+            try:
+                return float(x)
+            except:
+                return ensure_float(x)
+        try:
+            return int(x)
+        except:
+            return ensure_int(x)
+    if isinstance(x, datetime.date):
+        if isinstance(x, datetime.datetime):
+            return int(x.strftime("%Y%m%d%H%M%S"))
+        return int(x.strftime("%Y%m%d"))
+    if isinstance(x, datetime.time):
+        return int(x.strftime("%H%M%S"))
     return ensure_int(x)
 
 def mysql_add(x, y):
     return ensure_number(x) + ensure_number(y)
 
 def mysql_sub(x, y):
     return ensure_number(x) - ensure_number(y)
```

### Comparing `syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.1.5/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/compiler.py` & `syncanysql-0.1.5/syncanysql/compiler.py`

 * *Files 1% similar despite different names*

```diff
@@ -417,29 +417,29 @@
                 config["aggregate"]["distinct_keys"].append(copy.deepcopy(column))
 
         where_expression = expression.args.get("where")
         if where_expression and isinstance(where_expression, sqlglot_expressions.Where):
             where_condition = self.compile_where_condition(where_expression.args["this"], config, arguments, primary_table, join_tables)
             if where_condition:
                 if not config["intercepts"]:
-                    config["intercepts"] = [["#const", True], ["#const", True]]
+                    config["intercepts"] = [["#const", 1], ["#const", 1]]
                 config["intercepts"][0] = where_condition
             self.parse_condition_typing_filter(expression, config, arguments)
 
         having_expression = expression.args.get("having")
         if having_expression:
             having_condition = self.compile_having_condition(having_expression.args["this"], config, arguments, primary_table)
             if config.get("aggregate") and config["aggregate"]["having_columns"]:
                 if len({True if having_column in config["aggregate"]["schema"] else False
                         for having_column in config["aggregate"]["having_columns"]}) != 1:
                     raise SyncanySqlCompileException(
                         'error having condition, cannot contain the values before and after the aggregate calculation at the same time, related sql "%s"'
                         % self.to_sql(expression))
             if not config["intercepts"]:
-                config["intercepts"] = [["#const", True], ["#const", True]]
+                config["intercepts"] = [["#const", 1], ["#const", 1]]
             config["intercepts"][1] = having_condition
 
         order_expression = expression.args.get("order")
         if order_expression:
             self.compile_order(order_expression.args["expressions"], config, arguments, primary_table)
 
         if expression.args.get("offset"):
@@ -658,19 +658,19 @@
                     def compile_having_column(left_having_expression, right_having_expression):
                         left_having_column = self.compile_calculate(left_having_expression, config, arguments,
                                                                     primary_table, column_join_tables, i - 1)
                         if isinstance(right_having_expression, list):
                             if len(right_having_expression) > 1:
                                 right_having_column = compile_having_column(right_having_expression[0],
                                                                             right_having_expression[1:])
-                                return ["#if", left_having_column, right_having_column, ["#const", False]]
+                                return ["#if", left_having_column, right_having_column, ["#const", 0]]
                             right_having_expression = right_having_expression[0]
                         right_having_column = self.compile_calculate(right_having_expression, config, arguments,
                                                                      primary_table, column_join_tables, i - 1)
-                        return ["#if", left_having_column, right_having_column, ["#const", False]]
+                        return ["#if", left_having_column, right_having_column, ["#const", 0]]
                     having_columns = compile_having_column(join_table["having_expressions"][0],
                                                            join_table["having_expressions"][1:])
                 column = [join_columns, join_db_table, having_columns, column] \
                     if join_columns else [join_db_table, having_columns, column]
             else:
                 column = [join_columns, join_db_table, column] if join_columns else [join_db_table, column]
 
@@ -688,22 +688,22 @@
     def compile_where_condition(self, expression, config, arguments, primary_table, join_tables, is_query_condition=True):
         if isinstance(expression, sqlglot_expressions.And):
             left_condition = self.compile_where_condition(expression.args.get("this"), config, arguments,
                                                           primary_table, join_tables, is_query_condition)
             right_condition = self.compile_where_condition(expression.args.get("expression"), config, arguments,
                                                            primary_table, join_tables, is_query_condition)
             if left_condition and right_condition:
-                return ["#if", left_condition, right_condition, ["#const", False]]
+                return ["#if", left_condition, right_condition, ["#const", 0]]
             return left_condition or right_condition or None
         if isinstance(expression, sqlglot_expressions.Or):
             left_condition = self.compile_where_condition(expression.args.get("this"), config, arguments, primary_table,
                                                           join_tables, False)
             right_condition = self.compile_where_condition(expression.args.get("expression"), config, arguments,
                                                            primary_table, join_tables, False)
-            return ["#if", left_condition, ["#const", True], right_condition]
+            return ["#if", left_condition, ["#const", 1], right_condition]
 
         def parse_calucate(calculate_expression):
             if not isinstance(config.get("schema"), dict):
                 return calculate_expression
             if self.is_column(calculate_expression, config, arguments):
                 calculate_name = "__where_condition_value_%d__" % id(calculate_expression)
                 self.compile_select_calculate_column(calculate_expression, config, arguments, primary_table,
@@ -795,72 +795,72 @@
         if isinstance(expression, sqlglot_expressions.EQ):
             is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
             if is_query_condition and is_query_column:
                 if condition_column["typing_name"] not in config["querys"]:
                     config["querys"][condition_column["typing_name"]] = {}
                 config["querys"][condition_column["typing_name"]]["=="] = right_calculater
                 return None
-            return ["@eq", left_calculater, right_calculater]
+            return ["@mysql::eq", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.NEQ):
             is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
             if is_query_condition and is_query_column:
                 if condition_column["typing_name"] not in config["querys"]:
                     config["querys"][condition_column["typing_name"]] = {}
                 config["querys"][condition_column["typing_name"]]["!="] = right_calculater
                 return None
-            return ["@neq", left_calculater, right_calculater]
+            return ["@mysql::neq", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.GT):
             is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
             if is_query_condition and is_query_column:
                 if condition_column["typing_name"] not in config["querys"]:
                     config["querys"][condition_column["typing_name"]] = {}
                 config["querys"][condition_column["typing_name"]][">"] = right_calculater
                 return None
-            return ["@gt", left_calculater, right_calculater]
+            return ["@mysql::gt", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.GTE):
             is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
             if is_query_condition and is_query_column:
                 if condition_column["typing_name"] not in config["querys"]:
                     config["querys"][condition_column["typing_name"]] = {}
                 config["querys"][condition_column["typing_name"]][">="] = right_calculater
                 return None
-            return ["@gte", left_calculater, right_calculater]
+            return ["@mysql::gte", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.LT):
             is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
             if is_query_condition and is_query_column:
                 if condition_column["typing_name"] not in config["querys"]:
                     config["querys"][condition_column["typing_name"]] = {}
                 config["querys"][condition_column["typing_name"]]["<"] = right_calculater
                 return None
-            return ["@lt", left_calculater, right_calculater]
+            return ["@mysql::lt", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.LTE):
             is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
             if is_query_condition and is_query_column:
                 if condition_column["typing_name"] not in config["querys"]:
                     config["querys"][condition_column["typing_name"]] = {}
                 config["querys"][condition_column["typing_name"]]["<="] = right_calculater
                 return None
-            return ["@lte", left_calculater, right_calculater]
+            return ["@mysql::lte", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.In):
             is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
             if is_query_condition and is_query_column:
                 if condition_column["typing_name"] not in config["querys"]:
                     config["querys"][condition_column["typing_name"]] = {}
                 config["querys"][condition_column["typing_name"]]["in"] = ["@convert_array", right_calculater]
                 return None
-            return ["@in", left_calculater, ["@convert_array", right_calculater]]
+            return ["@mysql::in", left_calculater, ["@convert_array", right_calculater]]
         elif isinstance(expression, sqlglot_expressions.Like):
             is_query_condition = False
             is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
             if not isinstance(right_calculater, list) or len(right_calculater) != 2 or right_calculater[0] != "#const":
                 raise SyncanySqlCompileException(
                     'error having condition, like condition value must be const, related sql "%s"'
                     % self.to_sql(expression))
             return ["#if", ["@re::match", right_calculater[1].replace("%", ".*").replace(".*.*", "%"), left_calculater],
-                    ["#const", True], ["#const", False]]
+                    ["#const", 1], ["#const", 0]]
         elif isinstance(expression, sqlglot_expressions.Paren):
             return self.compile_where_condition(expression.args.get("this"), config, arguments, primary_table, join_tables, False)
         else:
             return self.compile_calculate(parse_calucate(expression), config, arguments, primary_table, [])
 
     def compile_query_condition(self, expression, config, arguments, primary_table, typing_filters):
         if isinstance(expression, sqlglot_expressions.Select):
@@ -1130,14 +1130,16 @@
             return "@aggregate_sum::aggregate", "@aggregate_sum::reduce", None
         elif isinstance(expression, sqlglot_expressions.Min):
             return "@aggregate_min::aggregate", "@aggregate_min::reduce", None
         elif isinstance(expression, sqlglot_expressions.Max):
             return "@aggregate_max::aggregate", "@aggregate_max::reduce", None
         elif isinstance(expression, sqlglot_expressions.Avg):
             return "@aggregate_avg::aggregate", "@aggregate_avg::reduce", "@aggregate_avg::final_value"
+        elif isinstance(expression, sqlglot_expressions.GroupConcat):
+            return "@aggregate_group_concat::aggregate", "@aggregate_group_concat::reduce", "@aggregate_group_concat::final_value"
         elif isinstance(expression, sqlglot_expressions.Anonymous):
             calculater_name = expression.args["this"].lower()
             try:
                 aggregate_calculater = find_aggregate_calculater(calculater_name)
                 return ("@" + calculater_name + "::aggregate",
                         "@" + calculater_name + "::reduce",
                         ("@" + calculater_name + "::final_value" if hasattr(aggregate_calculater, "final_value") else None))
@@ -1252,25 +1254,16 @@
                 typing_filter = "datetime"
             elif to_type == sqlglot_expressions.DataType.TEXT_TYPES:
                 typing_filter = "str"
             else:
                 typing_filter = None
             value_column = self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
             if typing_filter:
-                return ["#if", ["#const", True], value_column, None, ":$.*|" + typing_filter]
+                return ["#if", ["#const", 1], value_column, None, ":$.*|" + typing_filter]
             return value_column
-        elif isinstance(expression, sqlglot_expressions.Binary):
-            func_name = expression.key.lower()
-            if isinstance(expression.args["expression"], sqlglot_expressions.Interval):
-                func_name = "date" + func_name
-            return [
-                ("@mysql::" + func_name) if is_mysql_func(func_name) else ("@" + func_name),
-                self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
-                self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index)
-            ]
         elif isinstance(expression, sqlglot_expressions.BitwiseNot):
             func_name = expression.key.lower()
             return [
                 ("@mysql::" + func_name) if is_mysql_func(func_name) else ("@" + func_name),
                 self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
             ]
         elif isinstance(expression, sqlglot_expressions.If):
@@ -1299,15 +1292,15 @@
                 value_column = parse_coalesce(expression.args.get("expressions"))
             else:
                 value_column = self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index)
             return ["#if", ["@is_null", condition_column], value_column, condition_column]
         elif isinstance(expression, sqlglot_expressions.Case):
             cases = {}
             cases["#case"] = self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index) \
-                                 if expression.args.get("this") else ["#const", True]
+                                 if expression.args.get("this") else ["#const", 1]
             if expression.args.get("ifs"):
                 for case_expression in expression.args["ifs"]:
                     if not isinstance(case_expression, sqlglot_expressions.If) or not self.is_const(case_expression.args["this"], config, arguments):
                         raise SyncanySqlCompileException('unknown calculate function, related sql "%s"' % self.to_sql(expression))
                     case_value = self.parse_const(case_expression.args["this"], config, arguments)["value"]
                     cases[(":" + str(case_value)) if isinstance(case_value, (int, float)) and not isinstance(case_value, bool) else case_value] = \
                         self.compile_calculate(case_expression.args["true"], config, arguments, primary_table, column_join_tables, join_index)
@@ -1338,18 +1331,15 @@
         elif isinstance(expression, sqlglot_expressions.Paren):
             return self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
         elif isinstance(expression, sqlglot_expressions.Between):
             return ["#make", {
                 "key_value": self.compile_calculate(expression.args["this"], config, arguments, primary_table, []),
                 "low_value": self.compile_calculate(expression.args["low"], config, arguments, primary_table, []),
                 "high_value": self.compile_calculate(expression.args["high"], config, arguments, primary_table, [])
-            }, [":@and", ["@gte", "$.key_value", "$.low_value"], ["@lte", "$.key_value", "$.high_value"]]]
-        elif isinstance(expression, sqlglot_expressions.Not):
-            return ["@not", self.compile_calculate(expression.args["this"], config, arguments, primary_table,
-                                                   column_join_tables, join_index)]
+            }, [":#if", ["@mysql::gte", "$.key_value", "$.low_value"], ["@mysql::lte", "$.key_value", "$.high_value"], ["#const", 0]]]
         elif self.is_column(expression, config, arguments):
             join_column = self.parse_column(expression, config, arguments)
             return self.compile_join_column_field(expression, config, arguments, primary_table, join_index, 
                                                   join_column, column_join_tables)
         elif isinstance(expression, sqlglot_expressions.Star):
             return "$.*"
         elif isinstance(expression, sqlglot_expressions.Tuple):
@@ -1358,43 +1348,89 @@
                 tuple_column.append(self.compile_calculate(tuple_expression, config, arguments, primary_table,
                                                    column_join_tables, join_index))
             return ["@convert_array", tuple_column]
         elif isinstance(expression, sqlglot_expressions.Interval):
             return ["#const", {"value": expression.args["this"].args["this"], "unit": expression.args["unit"].args["this"]}]
         elif self.is_const(expression, config, arguments):
             return self.compile_const(expression, config, arguments, self.parse_const(expression, config, arguments))
+        elif isinstance(expression, (sqlglot_expressions.Binary, sqlglot_expressions.Condition)):
+            if isinstance(expression, sqlglot_expressions.And):
+                return [
+                    "#if",
+                    self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
+                    self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index),
+                    ["#const", 0]
+                ]
+            if isinstance(expression, sqlglot_expressions.Or):
+                return [
+                    "#if",
+                    self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
+                    ["#const", 1],
+                    self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index)
+                ]
+            if isinstance(expression, sqlglot_expressions.Like):
+                return [
+                    "#if",
+                    [
+                        "@re::match",
+                        self.parse_const(expression.args["this"], config, arguments)["value"].replace("%", ".*").replace(".*.*", "%"),
+                        self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index)
+                    ],
+                    ["#const", 1], ["#const", 0]
+                ]
+
+            func_name = expression.key.lower()
+            if expression.args.get("expressions"):
+                return [
+                    ("@mysql::" + func_name) if is_mysql_func(func_name) else ("@" + func_name),
+                    self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
+                    ["#make", [self.compile_calculate(item_expression, config, arguments, primary_table, column_join_tables, join_index)
+                               for item_expression in expression.args["expressions"]]]
+                ]
+            if not expression.args.get("expression"):
+                return [
+                    ("@mysql::" + func_name) if is_mysql_func(func_name) else ("@" + func_name),
+                    self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index)
+                ]
+            if isinstance(expression.args["expression"], sqlglot_expressions.Interval):
+                func_name = "date" + func_name
+            return [
+                ("@mysql::" + func_name) if is_mysql_func(func_name) else ("@" + func_name),
+                self.compile_calculate(expression.args["this"], config, arguments, primary_table, column_join_tables, join_index),
+                self.compile_calculate(expression.args["expression"], config, arguments, primary_table, column_join_tables, join_index)
+            ]
         else:
             raise SyncanySqlCompileException('unknown calculate expression, related sql "%s"' % self.to_sql(expression))
 
     def compile_having_condition(self, expression, config, arguments, primary_table):
         if isinstance(expression, sqlglot_expressions.And):
             return [
                 "#if",
                 self.compile_having_condition(expression.args.get("this"), config, arguments, primary_table),
                 self.compile_having_condition(expression.args.get("expression"), config, arguments, primary_table),
-                ["#const", False]
+                ["#const", 0]
             ]
         if isinstance(expression, sqlglot_expressions.Or):
             return [
                 "#if",
                 self.compile_having_condition(expression.args.get("this"), config, arguments, primary_table),
-                ["#const", True],
+                ["#const", 1],
                 self.compile_having_condition(expression.args.get("expression"), config, arguments, primary_table)
             ]
 
         def parse(expression):
             left_column = None
             if "aggregate" not in config:
                 config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
             if expression.args.get("expressions"):
                 left_expression, right_expression = expression.args["this"], expression.args["expressions"]
             elif expression.args.get("query"):
                 left_expression, right_expression = expression.args["this"], expression.args["query"]
             else:
-                left_expression, right_expression = expression.args["this"], expression.args["expression"]
+                left_expression, right_expression = expression.args["this"], expression.args.get("expression")
             if self.is_column(left_expression, config, arguments):
                 left_column = self.parse_column(left_expression, config, arguments)
                 if isinstance(config["schema"], dict) and left_column["column_name"] not in config["schema"]:
                     raise SyncanySqlCompileException('unknown having condition column, column must be in the query result, related sql "%s"'
                                                      % self.to_sql(expression))
                 config["aggregate"]["having_columns"].add(left_column["column_name"])
                 left_calculater = self.compile_column(left_expression, config, arguments, left_column)
@@ -1406,14 +1442,16 @@
                     raise SyncanySqlCompileException('unknown having condition column, column must be in the query result, related sql "%s"'
                                                      % self.to_sql(expression))
                 for calculate_field in calculate_fields:
                     if calculate_field["column_name"] not in config["schema"]:
                         continue
                     config["aggregate"]["having_columns"].add(calculate_field["column_name"])
                 left_calculater = self.compile_calculate(left_expression, config, arguments, primary_table, [])
+            if not right_expression:
+                return left_calculater, None
 
             if isinstance(right_expression, list):
                 value_items = []
                 for value_expression_item in right_expression:
                     if not self.is_const(value_expression_item, config, arguments):
                         raise SyncanySqlCompileException('error having condition, array must be const value, related sql "%s"' % self.to_sql(expression))
                     value_items.append(self.parse_const(value_expression_item, config, arguments)["value"])
@@ -1441,44 +1479,50 @@
                 if calculate_field["column_name"] not in config["schema"]:
                     continue
                 config["aggregate"]["having_columns"].add(calculate_field["column_name"])
             return left_calculater, self.compile_calculate(right_expression, config, arguments, primary_table, [])
 
         if isinstance(expression, sqlglot_expressions.EQ):
             left_calculater, right_calculater = parse(expression)
-            return ["@eq", left_calculater, right_calculater]
+            return ["@mysql::eq", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.NEQ):
             left_calculater, right_calculater = parse(expression)
-            return ["@neq", left_calculater, right_calculater]
+            return ["@mysql::neq", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.GT):
             left_calculater, right_calculater = parse(expression)
-            return ["@gt", left_calculater, right_calculater]
+            return ["@mysql::gt", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.GTE):
             left_calculater, right_calculater = parse(expression)
-            return ["@gte", left_calculater, right_calculater]
+            return ["@mysql::gte", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.LT):
             left_calculater, right_calculater = parse(expression)
-            return ["@lt", left_calculater, right_calculater]
+            return ["@mysql::lt", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.LTE):
             left_calculater, right_calculater = parse(expression)
-            return ["@lte", left_calculater, right_calculater]
+            return ["@mysql::lte", left_calculater, right_calculater]
         elif isinstance(expression, sqlglot_expressions.In):
             left_calculater, right_calculater = parse(expression)
-            return ["@in", left_calculater, ["@convert_array", right_calculater]]
+            return ["@mysql::in", left_calculater, ["@convert_array", right_calculater]]
         elif isinstance(expression, sqlglot_expressions.Like):
             left_calculater, right_calculater = parse(expression)
             if not isinstance(right_calculater, list) or len(right_calculater) != 2 or right_calculater[0] != "#const":
                 raise SyncanySqlCompileException('error having condition, like condition value must be const, related sql "%s"'
                                                  % self.to_sql(expression))
             return ["#if", ["@re::match", right_calculater[1].replace("%", ".*").replace(".*.*", "%"), left_calculater],
-                    ["#const", True], ["#const", False]]
+                    ["#const", 1], ["#const", 0]]
         elif isinstance(expression, sqlglot_expressions.Paren):
             return self.compile_having_condition(expression.args.get("this"), config, arguments, primary_table)
         else:
-            return self.compile_calculate(expression, config, arguments, primary_table, [])
+            left_calculater, right_calculater = parse(expression)
+            func_name = expression.key.lower()
+            if expression.args.get("expression") and isinstance(expression.args["expression"], sqlglot_expressions.Interval):
+                func_name = "date" + func_name
+            if right_calculater is None:
+                return [("@mysql::" + func_name) if is_mysql_func(func_name) else ("@" + func_name), left_calculater]
+            return [("@mysql::" + func_name) if is_mysql_func(func_name) else ("@" + func_name), left_calculater, right_calculater]
 
     def compile_order(self, expression, config, arguments, primary_table):
         primary_sort_keys, sort_keys = [], []
         for order_expression in expression:
             if not self.is_column(order_expression.args["this"], config, arguments):
                 if isinstance(config["schema"], dict):
                     if str(order_expression.args["this"]) in config["schema"]:
@@ -1791,39 +1835,36 @@
         elif isinstance(expression, sqlglot_expressions.Paren):
             self.parse_calculate(expression.args["this"], config, arguments, primary_table, calculate_fields)
         elif self.is_column(expression, config, arguments):
             column = self.parse_column(expression, config, arguments)
             if not column["table_name"] or primary_table["table_name"] == column["table_name"]:
                 primary_table["columns"][column["column_name"]] = column
             calculate_fields.append(column)
-        elif isinstance(expression, (sqlglot_expressions.Select, sqlglot_expressions.Star, sqlglot_expressions.Interval,
-                                     sqlglot_expressions.DataType)):
+        elif isinstance(expression, (sqlglot_expressions.Select, sqlglot_expressions.Union, sqlglot_expressions.Subquery,
+                                     sqlglot_expressions.Star, sqlglot_expressions.Interval, sqlglot_expressions.DataType)):
             pass
         elif self.is_const(expression, config, arguments):
             pass
         else:
             if not isinstance(expression, sqlglot_expressions.Expression):
                 return
-            if expression.args.get("this"):
-                self.parse_calculate(expression.args["this"], config, arguments, primary_table, calculate_fields)
-            if expression.args.get("expression"):
-                self.parse_calculate(expression.args["expression"], config, arguments, primary_table, calculate_fields)
-            if expression.args.get("expressions") and isinstance(expression.args["expressions"], list):
-                for arg_expression in expression.args["expressions"]:
-                    self.parse_calculate(arg_expression, config, arguments, primary_table, calculate_fields)
-            for arg_type in expression.arg_types:
-                if arg_type in ("this", "expression", "expressions"):
-                    continue
-                if arg_type not in expression.args or not expression.args[arg_type]:
-                    continue
-                if isinstance(expression.args[arg_type], list):
-                    for arg_expression in expression.args.get(arg_type, []):
-                        self.parse_calculate(arg_expression, config, arguments, primary_table, calculate_fields)
+            for arg_expression in expression.args.values():
+                if isinstance(arg_expression, list):
+                    for item_arg_expression in expression.args["expressions"]:
+                        if not isinstance(item_arg_expression, sqlglot_expressions.Expression):
+                            continue
+                        if self.is_const(item_arg_expression, config, arguments):
+                            continue
+                        self.parse_calculate(item_arg_expression, config, arguments, primary_table, calculate_fields)
                 else:
-                    self.parse_calculate(expression.args[arg_type], config, arguments, primary_table, calculate_fields)
+                    if not isinstance(arg_expression, sqlglot_expressions.Expression):
+                        continue
+                    if self.is_const(arg_expression, config, arguments):
+                        continue
+                    self.parse_calculate(arg_expression, config, arguments, primary_table, calculate_fields)
 
     def parse_aggregate(self, expression, config, arguments, aggregate_expressions):
         if self.is_aggregate(expression, config, arguments):
             aggregate_expressions.append(expression)
         if not self.is_calculate(expression, config, arguments):
             return
         for _, child_expression in expression.args.items():
@@ -2122,21 +2163,26 @@
         if isinstance(expression, sqlglot_expressions.Neg):
             return not isinstance(expression.args["this"], sqlglot_expressions.Neg) and self.is_const(expression.args["this"], config, arguments)
         return isinstance(expression, (sqlglot_expressions.Literal, sqlglot_expressions.Boolean,
                                        sqlglot_expressions.Null, sqlglot_expressions.HexString, sqlglot_expressions.BitString,
                                        sqlglot_expressions.ByteString, sqlglot_expressions.Parameter))
 
     def is_calculate(self, expression, config, arguments):
-        return isinstance(expression, (sqlglot_expressions.Neg, sqlglot_expressions.Anonymous, sqlglot_expressions.Binary, sqlglot_expressions.Func,
-                                       sqlglot_expressions.Select, sqlglot_expressions.Subquery, sqlglot_expressions.Union, sqlglot_expressions.Between,
-                                       sqlglot_expressions.Not, sqlglot_expressions.BitwiseNot, sqlglot_expressions.Tuple))
+        if isinstance(expression, sqlglot_expressions.Condition):
+            return isinstance(expression, (sqlglot_expressions.EQ, sqlglot_expressions.NEQ, sqlglot_expressions.GT, sqlglot_expressions.GTE,
+                                           sqlglot_expressions.LT, sqlglot_expressions.LTE, sqlglot_expressions.In, sqlglot_expressions.Not,
+                                           sqlglot_expressions.Between, sqlglot_expressions.Like, sqlglot_expressions.Func,
+                                           sqlglot_expressions.Binary))
+        return isinstance(expression, (sqlglot_expressions.Neg, sqlglot_expressions.Binary, sqlglot_expressions.Select,
+                                       sqlglot_expressions.Subquery, sqlglot_expressions.Union,
+                                       sqlglot_expressions.BitwiseNot, sqlglot_expressions.Tuple))
 
     def is_aggregate(self, expression, config, arguments):
         if isinstance(expression, (sqlglot_expressions.Count, sqlglot_expressions.Sum, sqlglot_expressions.Max,
-                                       sqlglot_expressions.Min, sqlglot_expressions.Avg)):
+                                   sqlglot_expressions.Min, sqlglot_expressions.Avg, sqlglot_expressions.GroupConcat)):
             return True
         if isinstance(expression, sqlglot_expressions.Anonymous):
             calculater_name = expression.args["this"].lower()
             try:
                 find_aggregate_calculater(calculater_name)
             except CalculaterUnknownException:
                 return False
@@ -2423,76 +2469,98 @@
         if expression.args.get("group"):
             for group_expression in expression.args["group"].args["expressions"]:
                 self.parse_calculate(group_expression, config, arguments, primary_table, calculate_fields)
         if expression.args.get("order"):
             for order_expression in expression.args["order"].args["expressions"]:
                 self.parse_calculate(order_expression.args["this"], config, arguments, primary_table, calculate_fields)
         for calculate_field in calculate_fields:
-            sub_column = "%s as `%s`" % (str(calculate_field["expression"]), calculate_field["column_name"])
+            if not calculate_field["table_name"] and primary_table["table_name"] and primary_table["table_alias"]:
+                continue
+            if calculate_field["table_name"] and calculate_field["table_name"] != primary_table["table_name"]:
+                sub_column = "%s as `%s__%s`" % (str(calculate_field["expression"]),
+                                                 calculate_field["table_name"].replace(".", "__"),
+                                                 calculate_field["column_name"])
+            else:
+                sub_column = "%s as `%s`" % (str(calculate_field["expression"]), calculate_field["column_name"])
             if sub_column not in sub_columns:
                 sub_columns.append(sub_column)
         sub_sql.append(", ".join(sub_columns))
         sub_sql.append(str(expression.args["from"]))
         for join_expression in expression.args["joins"]:
             sub_sql.append(str(join_expression))
         if expression.args.get("where"):
             sub_sql.append(str(expression.args["where"]))
 
+        subquery_name = "__subquery_" + str(uuid.uuid1().int)
         sql = ["SELECT"]
         if expression.args.get("distinct"):
-            sql.append(str(expression.args["distinct"]))
-        sql.append(", ".join([str(self.optimize_rewrite_except_table(select_expression, config, arguments))
-                              for select_expression in expression.args["expressions"]]))
-        sql.append("FROM (%s) `__subquery_%s`" % (" ".join(sub_sql), str(uuid.uuid1().int)))
+            sql.append(str(self.optimize_rewrite_except_table(expression.args["distinct"],
+                                                              config, arguments, primary_table)))
+        select_sql = []
+        for select_expression in expression.args["expressions"]:
+            if isinstance(select_expression, sqlglot_expressions.Alias):
+                select_sql.append(str(self.optimize_rewrite_except_table(select_expression, config, arguments, primary_table)))
+                continue
+            if isinstance(select_expression, sqlglot_expressions.Column):
+                if isinstance(select_expression.args.get("this"), sqlglot_expressions.Star):
+                    if (subquery_name + ".*") not in select_sql:
+                        select_sql.insert(0, subquery_name + ".*")
+                    continue
+                select_column_name = self.parse_column(select_expression, config, arguments)["column_name"]
+            else:
+                select_column_name = str(select_expression)
+            select_sql.append("%s as `%s`" %
+                              (str(self.optimize_rewrite_except_table(select_expression, config, arguments, primary_table)),
+                               select_column_name))
+        sql.append(", ".join(select_sql))
+        sql.append("FROM (%s) `%s`" % (" ".join(sub_sql), subquery_name))
         if expression.args.get("group"):
-            sql.append(str(self.optimize_rewrite_except_table(expression.args["group"], config, arguments)))
+            sql.append(str(self.optimize_rewrite_except_table(expression.args["group"], config, arguments, primary_table)))
         if expression.args.get("having"):
             sql.append(str(expression.args["having"]))
         if expression.args.get("order"):
-            sql.append(str(self.optimize_rewrite_except_table(expression.args["order"], config, arguments)))
+            sql.append(str(self.optimize_rewrite_except_table(expression.args["order"], config, arguments, primary_table)))
         if expression.args.get("offset"):
             offset_expression, limit_expression = expression.args.get("limit"), expression.args.get("offset")
         else:
             offset_expression, limit_expression = None, expression.args.get("limit")
         if limit_expression:
             offset_value = max(int(offset_expression.args["expression"].args["this"]), 0) if offset_expression else 0
             limit_value = max(int(limit_expression.args["expression"].args["this"]), 1)
             sql.append(("LIMIT %d, %d" % (offset_value, limit_value)) if offset_value > 0 else ("LIMIT %d" % limit_value))
         return maybe_parse(" ".join(sql), dialect=CompilerDialect)
 
     def optimize_rewrite_parse_table(self, expression, config, arguments, table_expression):
-        table = {"table_name": None, "columns": {}}
+        table = {"table_name": None, "table_alias": None, "columns": {}}
         if isinstance(table_expression, sqlglot_expressions.Table):
-            table["table_name"] = self.parse_table(table_expression, config, arguments)["table_name"]
+            table.update(self.parse_table(table_expression, config, arguments))
         elif isinstance(table_expression, sqlglot_expressions.Subquery):
             if "alias" not in table_expression.args:
                 return table
-            table["table_name"] = table_expression.args["alias"].args["this"].name \
+            table["table_alias"] = table_expression.args["alias"].args["this"].name \
                 if table_expression.args.get("alias") else None
+            table["table_name"] = table["table_alias"]
         return table
 
     def optimize_rewrite_parse_condition(self, expression, config, arguments, primary_table, condition_expression,
                                          table_name, related_tables, on_expressions, const_expressions, calcuate_expressions):
         if isinstance(condition_expression, sqlglot_expressions.And):
             self.optimize_rewrite_parse_condition(expression, config, arguments, primary_table, condition_expression.args.get("this"),
                                                   table_name, related_tables, on_expressions, const_expressions, calcuate_expressions)
             self.optimize_rewrite_parse_condition(expression, config, arguments, primary_table, condition_expression.args.get("expression"),
                                                   table_name, related_tables, on_expressions, const_expressions, calcuate_expressions)
         elif isinstance(condition_expression, (sqlglot_expressions.EQ, sqlglot_expressions.NEQ, sqlglot_expressions.GT,
                                                sqlglot_expressions.GTE, sqlglot_expressions.LT, sqlglot_expressions.LTE,
                                                sqlglot_expressions.In)):
             if condition_expression.args.get("expressions"):
-                left_expression, right_expression = condition_expression.args["this"], condition_expression.args[
-                    "expressions"]
+                left_expression, right_expression = condition_expression.args["this"], condition_expression.args["expressions"]
             elif condition_expression.args.get("query"):
-                left_expression, right_expression = condition_expression.args["this"], condition_expression.args[
-                    "query"]
+                left_expression, right_expression = condition_expression.args["this"], condition_expression.args["query"]
             else:
-                left_expression, right_expression = condition_expression.args["this"], condition_expression.args[
-                    "expression"]
+                left_expression, right_expression = condition_expression.args["this"], condition_expression.args["expression"]
 
             condition_column, value_expression = None, left_expression
             if self.is_column(left_expression, config, arguments):
                 left_column = self.parse_column(left_expression, config, arguments)
                 if left_column["table_name"] == table_name:
                     condition_column, value_expression = left_column, right_expression
             if not condition_column and self.is_column(right_expression, config, arguments):
@@ -2512,19 +2580,23 @@
                 return
             on_expressions.append(condition_expression)
             for calculate_field in calculate_fields:
                 related_tables.add(calculate_field["table_name"])
         else:
             calcuate_expressions.append(condition_expression)
 
-    def optimize_rewrite_except_table(self, expression, config, arguments):
+    def optimize_rewrite_except_table(self, expression, config, arguments, primary_table):
         def parse_except_table(arg_expression):
             if not isinstance(arg_expression, sqlglot_expressions.Expression):
                 return arg_expression
             if isinstance(arg_expression, sqlglot_expressions.Column):
+                column = self.parse_column(arg_expression, config, arguments)
+                if column["table_name"] and column["table_name"] != primary_table["table_name"]:
+                    arg_expression.args["this"].args["this"] = "%s__%s" % (
+                        column["table_name"].replace(".", "__"), column["column_name"])
                 if arg_expression.args.get("db"):
                     arg_expression.args["db"] = None
                 if arg_expression.args.get("table"):
                     arg_expression.args["table"] = None
                 return arg_expression
             for child_arg_expression in arg_expression.args.values():
                 if isinstance(child_arg_expression, list):
```

### Comparing `syncanysql-0.1.4/syncanysql/config.py` & `syncanysql-0.1.5/syncanysql/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # -*- coding: utf-8 -*-
 # 2023/2/8
 # create by: snower
 
 import os
 import copy
 import re
+import sys
 import uuid
 import logging.config
 import json
 import pytz
 from syncany.taskers.core import CoreTasker
 from syncany.taskers.config import load_config
 from syncany.logger import get_logger
@@ -123,25 +124,36 @@
                 default_value = default_value[1:]
             args.append([arg_info[0], exps[arg_info[1]] if len(arg_info) >= 2 else "==", default_value])
             query = query.replace(arg, '%s')
         return query, args
 
     def load(self, custom_config=None):
         home_config_path, cwd_config_path = self.get_home(), os.path.abspath(os.getcwd())
+        if home_config_path not in sys.path:
+            sys.path.append(home_config_path)
         for filename in {os.path.join(home_config_path, "config.json"), os.path.join(home_config_path, "config.yaml"),
                          os.path.join(cwd_config_path, "config.json"), os.path.join(cwd_config_path, "config.yaml")}:
             if not os.path.exists(filename):
                 continue
             if "extends" not in self.config or not isinstance(self.config["extends"], list):
                 self.config["extends"] = []
             if filename not in self.config["extends"]:
                 self.config["extends"].append(filename)
         self.load_config()
         if custom_config and isinstance(custom_config, dict):
             self.merge_config(custom_config)
+        pypackage_paths = self.config.get("pypackage_paths")
+        if pypackage_paths:
+            if isinstance(pypackage_paths, str):
+                pypackage_paths = [pypackage_paths]
+            if isinstance(pypackage_paths, list):
+                for pypackage_path in pypackage_paths:
+                    if isinstance(pypackage_path, str) and os.path.exists(pypackage_path) \
+                            and os.path.isdir(pypackage_path) and pypackage_path not in sys.path:
+                        sys.path.append(pypackage_path)
 
         if "timezone" in self.config:
             timezone = self.config.get("timezone")
             set_timezone(pytz.timezone(timezone))
         if "databases" not in self.config:
             self.config["databases"] = []
         databases = {database["name"]: database for database in self.config["databases"]}
```

### Comparing `syncanysql-0.1.4/syncanysql/executor.py` & `syncanysql-0.1.5/syncanysql/executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # -*- coding: utf-8 -*-
 # 2023/2/13
 # create by: snower
+
 import datetime
 import os
 import sys
 import re
 import threading
 from collections import deque
 from syncany.filters import StringFilter
@@ -125,15 +126,16 @@
             lineno = sql.lineno
             sql = self.compile_variable(str(sql))
             raw_sqls = RAW_SQL_RE.findall(sql)
             for raw, raw_name, _, raw_sql, _ in raw_sqls:
                 raw_name_info = raw_name.split(".")
                 if len(raw_name_info) != 2:
                     raise SyncanySqlCompileException("raw sql name error: %s", raw)
-                raw_sql = "set @config.databases." + raw_name_info[0] + ".virtual_views." + raw_name_info[1] + "='''\n" + raw_sql.strip() + "\n'''"
+                raw_sql = "set @config.databases." + raw_name_info[0] + ".virtual_views." \
+                          + raw_name_info[1] + "='''\n" + raw_sql.strip() + "\n'''"
                 self.compile(name + "(" + str(lineno) + ")#set_virtual_view", raw_sql)
                 sql = sql.replace(raw, raw_name)
             self.compile(name + "(" + str(lineno) + ")", sql)
 
     def compile(self, name, sql):
         self._thread_local.current_executor = self
         config = self.session_config.get()
```

### Comparing `syncanysql-0.1.4/syncanysql/main.py` & `syncanysql-0.1.5/syncanysql/main.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/parser.py` & `syncanysql-0.1.5/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/prompt.py` & `syncanysql-0.1.5/syncanysql/prompt.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/taskers/delete.py` & `syncanysql-0.1.5/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/taskers/execute.py` & `syncanysql-0.1.5/syncanysql/taskers/execute.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/taskers/explain.py` & `syncanysql-0.1.5/syncanysql/taskers/explain.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/taskers/into.py` & `syncanysql-0.1.5/syncanysql/taskers/into.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/taskers/query.py` & `syncanysql-0.1.5/syncanysql/taskers/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # create by: snower
 
 import os
 import copy
 import time
 import traceback
 import uuid
+from collections import defaultdict
 from syncany.logger import get_logger
 from syncany.taskers.core import CoreTasker
 from syncany.hook import Hooker
 from syncany.taskers.tasker import _thread_local
 from syncany.main import TaskerYieldNext, warp_database_logging
 
 
@@ -45,47 +46,76 @@
 
     def finaled(self, tasker, e=None):
         if e is not None or self.batch_count <= 1:
             return
         self.tasker.run_reduce(self.executor, self.session_config, self.manager, self.arguments, False)
 
 
+class QueryTaskerTemporaryMemoryManager(object):
+    def __init__(self):
+        self.collections = defaultdict(int)
+
+    def add_collection(self, name):
+        if name not in self.collections:
+            self.collections[name] = 0
+
+    def use_collection(self, name):
+        self.collections[name] += 1
+
+    def unuse_collection(self, name):
+        if name not in self.collections:
+            return True
+        self.collections[name] -= 1
+        return self.collections[name] <= 0
+
+    def free_collection(self, name):
+        if name not in self.collections:
+            return True
+        if self.collections[name] > 0:
+            return False
+        self.collections.pop(name, None)
+        return True
+
+    def get_names(self):
+        return list(self.collections.keys())
+
+
 class QueryTasker(object):
-    def __init__(self, config, sql_expression=None):
+    def __init__(self, config, sql_expression=None, temporary_memory_manager=None):
         self.name = config.get("name", "")
         self.config = config
         self.sql_expression = sql_expression
         self.reduce_config = None
         self.tasker = None
         self.dependency_taskers = []
         self.arguments = None
         self.tasker_generator = None
         self.updaters = []
-        self.temporary_memory_collections = set([])
+        self.temporary_memory_manager = temporary_memory_manager or QueryTaskerTemporaryMemoryManager()
         self.run_start_time = 0
 
     def start(self, name, executor, session_config, manager, arguments):
         dependency_taskers, where_schema, aggregate = [], self.config.get("where_schema", None), self.config.pop("aggregate", None)
         if aggregate and aggregate.get("distinct_keys"):
             self.config, distinct_config = self.compile_distinct_config(where_schema, aggregate), self.config
             distinct_config["name"] = distinct_config["name"] + "#select@distinct"
-            distinct_tasker = QueryTasker(distinct_config)
+            distinct_tasker = QueryTasker(distinct_config, temporary_memory_manager=self.temporary_memory_manager)
             distinct_tasker.start(name, executor, session_config, manager, copy.deepcopy(arguments))
             dependency_taskers.append(distinct_tasker)
             arguments["@limit"] = 0
 
         for dependency_config in self.config.get("dependencys", []):
             kn, knl = (dependency_config["name"] + "@"), len(dependency_config["name"] + "@")
             dependency_arguments = {}
             for key, value in arguments.items():
                 if key[:knl] != kn:
                     continue
                 dependency_arguments[key[knl:]] = value
                 dependency_arguments.pop(key, None)
-            dependency_tasker = QueryTasker(dependency_config)
+            dependency_tasker = QueryTasker(dependency_config, temporary_memory_manager=self.temporary_memory_manager)
             dependency_tasker.start(name, executor, session_config, manager, dependency_arguments)
             dependency_taskers.append(dependency_tasker)
 
         where_schema = self.config.pop("where_schema", None)
         limit, batch = int(arguments.get("@limit", 0)), int(arguments.get("@batch", 0))
         require_reduce, reduce_intercept, sorted_limit = False, False, len(self.config.get("pipelines", [])) == 2
         if self.config.get("intercepts"):
@@ -341,17 +371,21 @@
             if isinstance(tasker.config["output"], str) and "&.--." in tasker.config["output"]:
                 compile_arguments["@insert_batch"] = 0
 
         tasker.compile(compile_arguments)
         if "@verbose" in compile_arguments and compile_arguments["@verbose"]:
             warp_database_logging(tasker)
 
+        if hasattr(tasker.loader, "name"):
+            if tasker.loader.name.startswith("--.__subquery_") or tasker.loader.name.startswith("--.__unionquery_"):
+                self.temporary_memory_manager.use_collection(tasker.loader.name)
+
         if hasattr(tasker.outputer, "name"):
             if tasker.outputer.name.startswith("--.__subquery_") or tasker.outputer.name.startswith("--.__unionquery_"):
-                self.temporary_memory_collections.add(tasker.outputer.name)
+                self.temporary_memory_manager.add_collection(tasker.outputer.name)
 
         loader_or_outputers = [tasker.loader, tasker.outputer] + list(tasker.join_loaders.values())
         for loader_or_outputer in loader_or_outputers:
             if not hasattr(loader_or_outputer, "name"):
                 continue
             info = loader_or_outputer.name.split(".")
             if len(info) <= 1:
@@ -379,41 +413,64 @@
                         yield value
                 except StopIteration as e:
                     exit_code = e.value
                     if exit_code is not None and exit_code != 0:
                         return exit_code
                     break
         except SystemError:
+            self.check_free_temporary_memory_collection(executor, tasker)
             tasker.close(False, "signal terminaled")
             get_logger().error("signal exited")
             return 130
         except KeyboardInterrupt:
+            self.check_free_temporary_memory_collection(executor, tasker)
             tasker.close(False, "user terminaled")
             get_logger().error("Crtl+C exited")
             return 130
         except Exception as e:
+            self.check_free_temporary_memory_collection(executor, tasker)
             tasker.close(False, "Error: " + repr(e), traceback.format_exc())
             get_logger().error("tasker %s error: %s\n%s", tasker.name, e, traceback.format_exc())
             return 1
         else:
+            self.check_free_temporary_memory_collection(executor, tasker)
             tasker.close()
         return 0
 
     def execute_updater(self, executor, session_config, manager):
         for updater in self.updaters:
             updater(executor, session_config, manager)
 
         for dependency_tasker in self.dependency_taskers:
             dependency_tasker.execute_updater(executor, session_config, manager)
 
     def get_temporary_memory_collections(self):
-        names = list(self.temporary_memory_collections)
+        names = self.temporary_memory_manager.get_names()
         for dependency_tasker in self.dependency_taskers:
             names.extend(dependency_tasker.get_temporary_memory_collections())
-        return names
+        return list(set(names))
+
+    def check_free_temporary_memory_collection(self, executor, tasker):
+        try:
+            if not hasattr(tasker.loader, "name"):
+                return
+            if not tasker.loader.name.startswith("--.__subquery_") and not tasker.loader.name.startswith("--.__unionquery_"):
+                return
+            if hasattr(tasker.outputer, "name") and tasker.loader.name == tasker.outputer.name:
+                return
+            name = tasker.loader.name
+            if self.temporary_memory_manager.unuse_collection(name):
+                database = tasker.databases.instance("--")
+                if executor.runners and database.is_streaming(name):
+                    return
+                delete = database.delete(name, ["id"])
+                delete.commit()
+                self.temporary_memory_manager.free_collection(name)
+        except:
+            pass
 
     def is_local_memory_database(self, config, name="--"):
         try:
             database_config = dict(**[database for database in config["databases"]
                                       if database["name"] == name][0])
             return database_config["driver"] == "memory"
         except (TypeError, KeyError, IndexError):
```

### Comparing `syncanysql-0.1.4/syncanysql/taskers/set.py` & `syncanysql-0.1.5/syncanysql/taskers/set.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/taskers/show.py` & `syncanysql-0.1.5/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/taskers/use.py` & `syncanysql-0.1.5/syncanysql/taskers/use.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql/utils.py` & `syncanysql-0.1.5/syncanysql/utils.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.4/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.1.5/syncanysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.4
+Version: 0.1.5
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.1.4/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.1.5/syncanysql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 syncanysql/__init__.py
 syncanysql/compiler.py
 syncanysql/config.py
 syncanysql/errors.py
@@ -21,14 +22,15 @@
 syncanysql/calculaters/__init__.py
 syncanysql/calculaters/aggregate_calculater.py
 syncanysql/calculaters/env_variable_calculater.py
 syncanysql/calculaters/mysql_calculater.py
 syncanysql/calculaters/mysql_funcs/__init__.py
 syncanysql/calculaters/mysql_funcs/datetime_funcs.py
 syncanysql/calculaters/mysql_funcs/json_funcs.py
+syncanysql/calculaters/mysql_funcs/logical_funcs.py
 syncanysql/calculaters/mysql_funcs/number_funcs.py
 syncanysql/calculaters/mysql_funcs/string_funcs.py
 syncanysql/taskers/__init__.py
 syncanysql/taskers/delete.py
 syncanysql/taskers/execute.py
 syncanysql/taskers/explain.py
 syncanysql/taskers/into.py
```


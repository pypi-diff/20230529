# Comparing `tmp/syncanyserver-0.0.2.tar.gz` & `tmp/syncanyserver-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanyserver-0.0.2.tar", last modified: Fri May 26 10:44:41 2023, max compression
+gzip compressed data, was "syncanyserver-0.0.3.tar", last modified: Mon May 29 10:05:27 2023, max compression
```

## Comparing `syncanyserver-0.0.2.tar` & `syncanyserver-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:41.128679 syncanyserver-0.0.2/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1084 2023-05-04 07:22:50.000000 syncanyserver-0.0.2/LICENSE
--rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-05-26 10:44:41.130679 syncanyserver-0.0.2/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)      215 2023-05-12 08:13:41.000000 syncanyserver-0.0.2/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-26 10:44:41.140679 syncanyserver-0.0.2/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2010 2023-05-26 07:24:05.000000 syncanyserver-0.0.2/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:40.750477 syncanyserver-0.0.2/syncanyserver/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      105 2023-05-17 03:50:23.000000 syncanyserver-0.0.2/syncanyserver/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4121 2023-05-12 08:47:17.000000 syncanyserver-0.0.2/syncanyserver/database.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2464 2023-05-26 07:20:59.000000 syncanyserver-0.0.2/syncanyserver/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    31204 2023-05-26 09:48:39.000000 syncanyserver-0.0.2/syncanyserver/server.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1868 2023-05-12 04:09:15.000000 syncanyserver-0.0.2/syncanyserver/table.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2325 2023-05-26 07:20:59.000000 syncanyserver-0.0.2/syncanyserver/user.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:41.076686 syncanyserver-0.0.2/syncanyserver.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-05-26 10:44:39.000000 syncanyserver-0.0.2/syncanyserver.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)      439 2023-05-26 10:44:40.000000 syncanyserver-0.0.2/syncanyserver.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-26 10:44:39.000000 syncanyserver-0.0.2/syncanyserver.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       60 2023-05-26 10:44:39.000000 syncanyserver-0.0.2/syncanyserver.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        2 2023-05-12 09:54:27.000000 syncanyserver-0.0.2/syncanyserver.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      363 2023-05-26 10:44:39.000000 syncanyserver-0.0.2/syncanyserver.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       14 2023-05-26 10:44:39.000000 syncanyserver-0.0.2/syncanyserver.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:05:27.562142 syncanyserver-0.0.3/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1084 2023-05-04 07:22:50.000000 syncanyserver-0.0.3/LICENSE
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-05-29 10:05:27.564115 syncanyserver-0.0.3/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      215 2023-05-12 08:13:41.000000 syncanyserver-0.0.3/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-29 10:05:27.574114 syncanyserver-0.0.3/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2010 2023-05-27 14:13:18.000000 syncanyserver-0.0.3/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:05:27.215169 syncanyserver-0.0.3/syncanyserver/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      105 2023-05-27 14:13:18.000000 syncanyserver-0.0.3/syncanyserver/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4121 2023-05-12 08:47:17.000000 syncanyserver-0.0.3/syncanyserver/database.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2464 2023-05-26 07:20:59.000000 syncanyserver-0.0.3/syncanyserver/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    31204 2023-05-26 09:48:39.000000 syncanyserver-0.0.3/syncanyserver/server.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1868 2023-05-12 04:09:15.000000 syncanyserver-0.0.3/syncanyserver/table.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2325 2023-05-26 07:20:59.000000 syncanyserver-0.0.3/syncanyserver/user.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-29 10:05:27.515717 syncanyserver-0.0.3/syncanyserver.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      885 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      439 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       60 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        2 2023-05-12 09:54:27.000000 syncanyserver-0.0.3/syncanyserver.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      363 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       14 2023-05-29 10:05:26.000000 syncanyserver-0.0.3/syncanyserver.egg-info/top_level.txt
```

### Comparing `syncanyserver-0.0.2/LICENSE` & `syncanyserver-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.2/PKG-INFO` & `syncanyserver-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanyserver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple and easy to use SQL scripts to build virtual database tables MySQL Server
 Home-page: https://github.com/snower/syncany-server
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany-server
```

### Comparing `syncanyserver-0.0.2/setup.py` & `syncanyserver-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.0.2"
+version = "0.0.3"
 
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
-        "syncanysql>=0.1.4",
+        "syncanysql>=0.1.5",
         "mysql-mimic>=2.2.3"
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
         "pymysql": ['PyMySQL>=0.8.1'],
         "openpyxl": ["openpyxl>=2.5.0"],
         "postgresql": ["psycopg2>=2.8.6"],
```

### Comparing `syncanyserver-0.0.2/syncanyserver/database.py` & `syncanyserver-0.0.3/syncanyserver/database.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.2/syncanyserver/main.py` & `syncanyserver-0.0.3/syncanyserver/main.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.2/syncanyserver/server.py` & `syncanyserver-0.0.3/syncanyserver/server.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.2/syncanyserver/table.py` & `syncanyserver-0.0.3/syncanyserver/table.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.2/syncanyserver/user.py` & `syncanyserver-0.0.3/syncanyserver/user.py`

 * *Files identical despite different names*

### Comparing `syncanyserver-0.0.2/syncanyserver.egg-info/PKG-INFO` & `syncanyserver-0.0.3/syncanyserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanyserver
-Version: 0.0.2
+Version: 0.0.3
 Summary: Simple and easy to use SQL scripts to build virtual database tables MySQL Server
 Home-page: https://github.com/snower/syncany-server
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # syncany-server
```


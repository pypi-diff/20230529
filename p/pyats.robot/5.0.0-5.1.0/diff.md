# Comparing `tmp/pyats.robot-5.0.0-py3-none-any.whl.zip` & `tmp/pyats.robot-5.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,18 @@
-Zip file size: 6190 bytes, number of entries: 8
--rw-r--r--  2.0 unx      534 b- defN 18-Oct-09 23:34 pyats.robot-5.0.0-py3.4-nspkg.pth
--rw-r--r--  2.0 unx      197 b- defN 18-Oct-09 21:59 pyats/robot/__init__.py
--rw-r--r--  2.0 unx    10921 b- defN 18-Oct-09 21:58 pyats/robot/pyATSRobot.py
--rw-r--r--  2.0 unx        6 b- defN 18-Oct-09 23:34 pyats.robot-5.0.0.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx        6 b- defN 18-Oct-09 23:34 pyats.robot-5.0.0.dist-info/top_level.txt
--rw-r--r--  2.0 unx       92 b- defN 18-Oct-09 23:34 pyats.robot-5.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx     2942 b- defN 18-Oct-09 23:34 pyats.robot-5.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx      676 b- defN 18-Oct-09 23:34 pyats.robot-5.0.0.dist-info/RECORD
-8 files, 15374 bytes uncompressed, 5010 bytes compressed:  67.4%
+Zip file size: 11043 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      534 b- defN 19-Jan-23 22:15 pyats.robot-5.1.0-py3.6-nspkg.pth
+-rw-r--r--  2.0 unx      197 b- defN 19-Jan-23 22:05 pyats/robot/__init__.py
+-rw-r--r--  2.0 unx    10921 b- defN 19-Jan-23 22:05 pyats/robot/pyATSRobot.py
+-rw-r--r--  2.0 unx       27 b- defN 19-Jan-23 22:05 pyats/robot/commands/__init__.py
+-rw-r--r--  2.0 unx     1314 b- defN 19-Jan-23 22:05 pyats/robot/commands/impl.py
+-rw-r--r--  2.0 unx     2486 b- defN 19-Jan-23 22:05 pyats/robot/commands/job.py
+-rw-r--r--  2.0 unx      184 b- defN 19-Jan-23 22:05 pyats/robot/runner/__init__.py
+-rw-r--r--  2.0 unx     1183 b- defN 19-Jan-23 22:05 pyats/robot/runner/harness.py
+-rw-r--r--  2.0 unx     3899 b- defN 19-Jan-23 22:05 pyats/robot/runner/listener.py
+-rw-r--r--  2.0 unx      689 b- defN 19-Jan-23 22:05 pyats/robot/runner/task.py
+-rw-r--r--  2.0 unx     2927 b- defN 19-Jan-23 22:15 pyats.robot-5.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 19-Jan-23 22:15 pyats.robot-5.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 19-Jan-23 22:15 pyats.robot-5.1.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        6 b- defN 19-Jan-23 22:15 pyats.robot-5.1.0.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        6 b- defN 19-Jan-23 22:15 pyats.robot-5.1.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1364 b- defN 19-Jan-23 22:15 pyats.robot-5.1.0.dist-info/RECORD
+16 files, 25896 bytes uncompressed, 8763 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,25 +1,49 @@
-Filename: pyats.robot-5.0.0-py3.4-nspkg.pth
+Filename: pyats.robot-5.1.0-py3.6-nspkg.pth
 Comment: 
 
 Filename: pyats/robot/__init__.py
 Comment: 
 
 Filename: pyats/robot/pyATSRobot.py
 Comment: 
 
-Filename: pyats.robot-5.0.0.dist-info/namespace_packages.txt
+Filename: pyats/robot/commands/__init__.py
 Comment: 
 
-Filename: pyats.robot-5.0.0.dist-info/top_level.txt
+Filename: pyats/robot/commands/impl.py
 Comment: 
 
-Filename: pyats.robot-5.0.0.dist-info/WHEEL
+Filename: pyats/robot/commands/job.py
 Comment: 
 
-Filename: pyats.robot-5.0.0.dist-info/METADATA
+Filename: pyats/robot/runner/__init__.py
 Comment: 
 
-Filename: pyats.robot-5.0.0.dist-info/RECORD
+Filename: pyats/robot/runner/harness.py
+Comment: 
+
+Filename: pyats/robot/runner/listener.py
+Comment: 
+
+Filename: pyats/robot/runner/task.py
+Comment: 
+
+Filename: pyats.robot-5.1.0.dist-info/METADATA
+Comment: 
+
+Filename: pyats.robot-5.1.0.dist-info/WHEEL
+Comment: 
+
+Filename: pyats.robot-5.1.0.dist-info/entry_points.txt
+Comment: 
+
+Filename: pyats.robot-5.1.0.dist-info/namespace_packages.txt
+Comment: 
+
+Filename: pyats.robot-5.1.0.dist-info/top_level.txt
+Comment: 
+
+Filename: pyats.robot-5.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyats/robot/__init__.py

```diff
@@ -1,5 +1,5 @@
 # metadata
-__version__ = '5.0.0'
+__version__ = '5.1.0'
 __author__ = 'Cisco Systems Inc.'
 __contact__ = ['pyats-support@cisco.com', 'pyats-support-ext@cisco.com']
 __copyright__ = 'Copyright (c) 2017, Cisco Systems Inc.'
```

## Comparing `pyats.robot-5.0.0-py3.4-nspkg.pth` & `pyats.robot-5.1.0-py3.6-nspkg.pth`

 * *Files identical despite different names*

## Comparing `pyats.robot-5.0.0.dist-info/METADATA` & `pyats.robot-5.1.0.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyats.robot
-Version: 5.0.0
+Version: 5.1.0
 Summary: pyATS Robot: Robot Module
 Home-page: https://developer.cisco.com/site/pyats/
 Author: Cisco Systems Inc.
 Author-email: pyats-support-ext@cisco.com
 License: Apache 2.0
 Keywords: pyats robot ces
 Platform: UNKNOWN
@@ -18,24 +18,23 @@
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Provides-Extra: dev
 Requires-Dist: robotframework
-Requires-Dist: pyats.aetest (<5.1.0,>=5.0.0)
-Requires-Dist: pyats.connections (<5.1.0,>=5.0.0)
+Requires-Dist: pyats.aetest (<5.2.0,>=5.1.0)
+Requires-Dist: pyats.connections (<5.2.0,>=5.1.0)
 Provides-Extra: dev
-Requires-Dist: coverage; extra == 'dev'
-Requires-Dist: restview; extra == 'dev'
-Requires-Dist: Sphinx; extra == 'dev'
-Requires-Dist: sphinxcontrib-napoleon; extra == 'dev'
-Requires-Dist: sphinx-rtd-theme; extra == 'dev'
+Requires-Dist: coverage ; extra == 'dev'
+Requires-Dist: restview ; extra == 'dev'
+Requires-Dist: Sphinx ; extra == 'dev'
+Requires-Dist: sphinxcontrib-napoleon ; extra == 'dev'
+Requires-Dist: sphinx-rtd-theme ; extra == 'dev'
 
 pyATS Robot Component
 =====================
 
 pyATS is an end-to-end testing ecosystem, specializing in data-driven and 
 reusable testing, and engineered to be suitable for Agile, rapid development 
 iterations. Extensible by design, pyATS enables developers start with small,
```


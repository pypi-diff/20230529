# Comparing `tmp/BehaviorPattern-0.0.3.tar.gz` & `tmp/BehaviorPattern-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BehaviorPattern-0.0.3.tar", last modified: Mon May 29 09:20:59 2023, max compression
+gzip compressed data, was "dist/BehaviorPattern-0.0.4.tar", last modified: Mon May 29 09:26:55 2023, max compression
```

## Comparing `BehaviorPattern-0.0.3.tar` & `BehaviorPattern-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern/
--rw-r--r--   0 tiger     (1000) tiger     (1000)    12311 2023-05-29 09:18:02.000000 BehaviorPattern-0.0.3/BehaviorPattern/BehaviorPattern.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:18:00.000000 BehaviorPattern-0.0.3/BehaviorPattern/__init__.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)      275 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/SOURCES.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/dependency_links.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       61 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/requires.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       16 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/top_level.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2850 2023-05-29 09:18:15.000000 BehaviorPattern-0.0.3/README.md
--rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/setup.cfg
--rw-r--r--   0 tiger     (1000) tiger     (1000)      810 2023-05-29 09:20:54.000000 BehaviorPattern-0.0.3/setup.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)    12311 2023-05-29 09:26:26.000000 BehaviorPattern-0.0.4/BehaviorPattern/BehaviorPattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:26:23.000000 BehaviorPattern-0.0.4/BehaviorPattern/__init__.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      275 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       43 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/requires.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       16 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/top_level.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2850 2023-05-29 09:26:39.000000 BehaviorPattern-0.0.4/README.md
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/setup.cfg
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     1815 2023-05-29 09:26:42.000000 BehaviorPattern-0.0.4/setup.py
```

### Comparing `BehaviorPattern-0.0.3/BehaviorPattern/BehaviorPattern.py` & `BehaviorPattern-0.0.4/BehaviorPattern/BehaviorPattern.py`

 * *Files identical despite different names*

### Comparing `BehaviorPattern-0.0.3/BehaviorPattern.egg-info/PKG-INFO` & `BehaviorPattern-0.0.4/BehaviorPattern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.3
+Version: 0.0.4
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `BehaviorPattern-0.0.3/PKG-INFO` & `BehaviorPattern-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.3
+Version: 0.0.4
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `BehaviorPattern-0.0.3/README.md` & `BehaviorPattern-0.0.4/README.md`

 * *Files identical despite different names*


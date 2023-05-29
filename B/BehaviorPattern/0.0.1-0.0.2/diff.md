# Comparing `tmp/BehaviorPattern-0.0.1.tar.gz` & `tmp/BehaviorPattern-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BehaviorPattern-0.0.1.tar", last modified: Mon May 29 08:31:43 2023, max compression
+gzip compressed data, was "dist/BehaviorPattern-0.0.2.tar", last modified: Mon May 29 09:00:28 2023, max compression
```

## Comparing `BehaviorPattern-0.0.1.tar` & `BehaviorPattern-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 08:31:43.000000 BehaviorPattern-0.0.1/
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 08:31:43.000000 BehaviorPattern-0.0.1/BehaviorPattern.egg-info/
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3167 2023-05-29 08:31:43.000000 BehaviorPattern-0.0.1/BehaviorPattern.egg-info/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)      212 2023-05-29 08:31:43.000000 BehaviorPattern-0.0.1/BehaviorPattern.egg-info/SOURCES.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 08:31:43.000000 BehaviorPattern-0.0.1/BehaviorPattern.egg-info/dependency_links.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       61 2023-05-29 08:31:43.000000 BehaviorPattern-0.0.1/BehaviorPattern.egg-info/requires.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 08:31:43.000000 BehaviorPattern-0.0.1/BehaviorPattern.egg-info/top_level.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3167 2023-05-29 08:31:43.000000 BehaviorPattern-0.0.1/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2844 2023-05-29 08:31:19.000000 BehaviorPattern-0.0.1/README.md
--rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 08:31:43.000000 BehaviorPattern-0.0.1/setup.cfg
--rw-r--r--   0 tiger     (1000) tiger     (1000)      707 2023-05-29 08:31:21.000000 BehaviorPattern-0.0.1/setup.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3167 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      212 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       43 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/requires.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/top_level.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3167 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2844 2023-05-29 09:00:13.000000 BehaviorPattern-0.0.2/README.md
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/setup.cfg
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     1640 2023-05-29 09:00:16.000000 BehaviorPattern-0.0.2/setup.py
```

### Comparing `BehaviorPattern-0.0.1/BehaviorPattern.egg-info/PKG-INFO` & `BehaviorPattern-0.0.2/BehaviorPattern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.1
+Version: 0.0.2
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `BehaviorPattern-0.0.1/PKG-INFO` & `BehaviorPattern-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.1
+Version: 0.0.2
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `BehaviorPattern-0.0.1/README.md` & `BehaviorPattern-0.0.2/README.md`

 * *Files identical despite different names*


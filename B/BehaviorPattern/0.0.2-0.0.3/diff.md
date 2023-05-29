# Comparing `tmp/BehaviorPattern-0.0.2.tar.gz` & `tmp/BehaviorPattern-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BehaviorPattern-0.0.2.tar", last modified: Mon May 29 09:00:28 2023, max compression
+gzip compressed data, was "dist/BehaviorPattern-0.0.3.tar", last modified: Mon May 29 09:20:59 2023, max compression
```

## Comparing `BehaviorPattern-0.0.2.tar` & `BehaviorPattern-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3167 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)      212 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/SOURCES.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/dependency_links.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       43 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/requires.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/BehaviorPattern.egg-info/top_level.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3167 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2844 2023-05-29 09:00:13.000000 BehaviorPattern-0.0.2/README.md
--rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 09:00:28.000000 BehaviorPattern-0.0.2/setup.cfg
--rw-r--r--   0 tiger     (1000) tiger     (1000)     1640 2023-05-29 09:00:16.000000 BehaviorPattern-0.0.2/setup.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)    12311 2023-05-29 09:18:02.000000 BehaviorPattern-0.0.3/BehaviorPattern/BehaviorPattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:18:00.000000 BehaviorPattern-0.0.3/BehaviorPattern/__init__.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      275 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       61 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/requires.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       16 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/BehaviorPattern.egg-info/top_level.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2850 2023-05-29 09:18:15.000000 BehaviorPattern-0.0.3/README.md
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 09:20:59.000000 BehaviorPattern-0.0.3/setup.cfg
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      810 2023-05-29 09:20:54.000000 BehaviorPattern-0.0.3/setup.py
```

### Comparing `BehaviorPattern-0.0.2/BehaviorPattern.egg-info/PKG-INFO` & `BehaviorPattern-0.0.3/BehaviorPattern.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.2
+Version: 0.0.3
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -92,15 +92,15 @@
 
 ## 贡献
 
 如果你发现任何bugs，请提交Issue或Pull Request进行更正
 
 ## 作者
 
-MyPackage由Chen Chen编写和维护。
+BehaviorPattern由Chen Chen编写和维护。
 
 ## 致谢
 
 感谢以下Python包的开发者：
 
 - numpy
 - pandas
```

### Comparing `BehaviorPattern-0.0.2/PKG-INFO` & `BehaviorPattern-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.2
+Version: 0.0.3
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -92,15 +92,15 @@
 
 ## 贡献
 
 如果你发现任何bugs，请提交Issue或Pull Request进行更正
 
 ## 作者
 
-MyPackage由Chen Chen编写和维护。
+BehaviorPattern由Chen Chen编写和维护。
 
 ## 致谢
 
 感谢以下Python包的开发者：
 
 - numpy
 - pandas
```

### Comparing `BehaviorPattern-0.0.2/README.md` & `BehaviorPattern-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -81,15 +81,15 @@
 
 ## 贡献
 
 如果你发现任何bugs，请提交Issue或Pull Request进行更正
 
 ## 作者
 
-MyPackage由Chen Chen编写和维护。
+BehaviorPattern由Chen Chen编写和维护。
 
 ## 致谢
 
 感谢以下Python包的开发者：
 
 - numpy
 - pandas
```


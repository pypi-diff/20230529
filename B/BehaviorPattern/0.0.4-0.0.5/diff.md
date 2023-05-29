# Comparing `tmp/BehaviorPattern-0.0.4.tar.gz` & `tmp/BehaviorPattern-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BehaviorPattern-0.0.4.tar", last modified: Mon May 29 09:26:55 2023, max compression
+gzip compressed data, was "dist/BehaviorPattern-0.0.5.tar", last modified: Mon May 29 09:45:49 2023, max compression
```

## Comparing `BehaviorPattern-0.0.4.tar` & `BehaviorPattern-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern/
--rw-r--r--   0 tiger     (1000) tiger     (1000)    12311 2023-05-29 09:26:26.000000 BehaviorPattern-0.0.4/BehaviorPattern/BehaviorPattern.py
--rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:26:23.000000 BehaviorPattern-0.0.4/BehaviorPattern/__init__.py
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)      275 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/SOURCES.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/dependency_links.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       43 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/requires.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       16 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/BehaviorPattern.egg-info/top_level.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2850 2023-05-29 09:26:39.000000 BehaviorPattern-0.0.4/README.md
--rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 09:26:55.000000 BehaviorPattern-0.0.4/setup.cfg
--rw-r--r--   0 tiger     (1000) tiger     (1000)     1815 2023-05-29 09:26:42.000000 BehaviorPattern-0.0.4/setup.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:45:49.000000 BehaviorPattern-0.0.5/
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:45:49.000000 BehaviorPattern-0.0.5/BehaviorPattern/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3121 2023-05-29 09:44:54.000000 BehaviorPattern-0.0.5/BehaviorPattern/CombinePattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     6892 2023-05-29 09:44:57.000000 BehaviorPattern-0.0.5/BehaviorPattern/ContinuePattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2759 2023-05-29 09:44:49.000000 BehaviorPattern-0.0.5/BehaviorPattern/DataClass.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3386 2023-05-29 09:45:00.000000 BehaviorPattern-0.0.5/BehaviorPattern/SequencePattern.py
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:44:45.000000 BehaviorPattern-0.0.5/BehaviorPattern/__init__.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 09:45:49.000000 BehaviorPattern-0.0.5/BehaviorPattern.egg-info/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 09:45:48.000000 BehaviorPattern-0.0.5/BehaviorPattern.egg-info/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      373 2023-05-29 09:45:49.000000 BehaviorPattern-0.0.5/BehaviorPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 09:45:48.000000 BehaviorPattern-0.0.5/BehaviorPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       43 2023-05-29 09:45:48.000000 BehaviorPattern-0.0.5/BehaviorPattern.egg-info/requires.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       16 2023-05-29 09:45:48.000000 BehaviorPattern-0.0.5/BehaviorPattern.egg-info/top_level.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3173 2023-05-29 09:45:49.000000 BehaviorPattern-0.0.5/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2850 2023-05-29 09:45:12.000000 BehaviorPattern-0.0.5/README.md
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 09:45:49.000000 BehaviorPattern-0.0.5/setup.cfg
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     1815 2023-05-29 09:45:17.000000 BehaviorPattern-0.0.5/setup.py
```

### Comparing `BehaviorPattern-0.0.4/BehaviorPattern.egg-info/PKG-INFO` & `BehaviorPattern-0.0.5/BehaviorPattern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.4
+Version: 0.0.5
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `BehaviorPattern-0.0.4/PKG-INFO` & `BehaviorPattern-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BehaviorPattern
-Version: 0.0.4
+Version: 0.0.5
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `BehaviorPattern-0.0.4/README.md` & `BehaviorPattern-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `BehaviorPattern-0.0.4/setup.py` & `BehaviorPattern-0.0.5/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     return [dependency for dependency in dependencies if dependency not in installed]
 
 # 如果存在未安装的依赖库，安装未安装的依赖库
 missing = get_missing_dependencies()
 if missing:
     setuptools.setup(
         name='BehaviorPattern',
-        version='0.0.4',
+        version='0.0.5',
         author='Chen Chen',
         author_email='cchen56@163.com',
         description='The tool is designed to mine behavior patterns',
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=setuptools.find_packages(),
         classifiers=[
@@ -40,15 +40,15 @@
         ],
         python_requires='>=3.6',
         install_requires=missing,
     )
 else:
     setuptools.setup(
         name='BehaviorPattern',
-        version='0.0.4',
+        version='0.0.5',
         author='Chen Chen',
         author_email='cchen56@163.com',
         description='The tool is designed to mine behavior patterns',
         long_description=long_description,
         long_description_content_type='text/markdown',
         packages=setuptools.find_packages(),
         classifiers=[
```


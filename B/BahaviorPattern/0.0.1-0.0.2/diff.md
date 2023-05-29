# Comparing `tmp/BahaviorPattern-0.0.1.tar.gz` & `tmp/BahaviorPattern-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BahaviorPattern-0.0.1.tar", last modified: Mon May 29 08:02:30 2023, max compression
+gzip compressed data, was "dist/BahaviorPattern-0.0.2.tar", last modified: Mon May 29 08:20:37 2023, max compression
```

## Comparing `BahaviorPattern-0.0.1.tar` & `BahaviorPattern-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 08:02:30.000000 BahaviorPattern-0.0.1/
-drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 08:02:30.000000 BahaviorPattern-0.0.1/BahaviorPattern.egg-info/
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3298 2023-05-29 08:02:30.000000 BahaviorPattern-0.0.1/BahaviorPattern.egg-info/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)      212 2023-05-29 08:02:30.000000 BahaviorPattern-0.0.1/BahaviorPattern.egg-info/SOURCES.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 08:02:30.000000 BahaviorPattern-0.0.1/BahaviorPattern.egg-info/dependency_links.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)       61 2023-05-29 08:02:30.000000 BahaviorPattern-0.0.1/BahaviorPattern.egg-info/requires.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 08:02:30.000000 BahaviorPattern-0.0.1/BahaviorPattern.egg-info/top_level.txt
--rw-r--r--   0 tiger     (1000) tiger     (1000)     3298 2023-05-29 08:02:30.000000 BahaviorPattern-0.0.1/PKG-INFO
--rw-r--r--   0 tiger     (1000) tiger     (1000)     2975 2023-05-29 08:01:27.000000 BahaviorPattern-0.0.1/README.md
--rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 08:02:30.000000 BahaviorPattern-0.0.1/setup.cfg
--rw-r--r--   0 tiger     (1000) tiger     (1000)      707 2023-05-29 08:01:43.000000 BahaviorPattern-0.0.1/setup.py
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 08:20:37.000000 BahaviorPattern-0.0.2/
+drwxr-xr-x   0 tiger     (1000) tiger     (1000)        0 2023-05-29 08:20:37.000000 BahaviorPattern-0.0.2/BahaviorPattern.egg-info/
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3167 2023-05-29 08:20:37.000000 BahaviorPattern-0.0.2/BahaviorPattern.egg-info/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      212 2023-05-29 08:20:37.000000 BahaviorPattern-0.0.2/BahaviorPattern.egg-info/SOURCES.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 08:20:37.000000 BahaviorPattern-0.0.2/BahaviorPattern.egg-info/dependency_links.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       61 2023-05-29 08:20:37.000000 BahaviorPattern-0.0.2/BahaviorPattern.egg-info/requires.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)        1 2023-05-29 08:20:37.000000 BahaviorPattern-0.0.2/BahaviorPattern.egg-info/top_level.txt
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     3167 2023-05-29 08:20:37.000000 BahaviorPattern-0.0.2/PKG-INFO
+-rw-r--r--   0 tiger     (1000) tiger     (1000)     2844 2023-05-29 08:19:45.000000 BahaviorPattern-0.0.2/README.md
+-rw-r--r--   0 tiger     (1000) tiger     (1000)       38 2023-05-29 08:20:37.000000 BahaviorPattern-0.0.2/setup.cfg
+-rw-r--r--   0 tiger     (1000) tiger     (1000)      707 2023-05-29 08:19:47.000000 BahaviorPattern-0.0.2/setup.py
```

### Comparing `BahaviorPattern-0.0.1/BahaviorPattern.egg-info/PKG-INFO` & `BahaviorPattern-0.0.2/BahaviorPattern.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BahaviorPattern
-Version: 0.0.1
+Version: 0.0.2
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -86,18 +86,14 @@
 - pandas
 - efficient_apriori
 - tqdm
 - prefixspan
 
 完整的依赖列表可以在setup.py中找到。
 
-## 开源许可
-
-MyPackage使用[MIT许可证](https://opensource.org/licenses/MIT)。请查看LICENSE文件获得更多信息。
-
 ## 贡献
 
 如果你发现任何bugs，请提交Issue或Pull Request进行更正
 
 ## 作者
 
 MyPackage由Chen Chen编写和维护。
```

### Comparing `BahaviorPattern-0.0.1/PKG-INFO` & `BahaviorPattern-0.0.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BahaviorPattern
-Version: 0.0.1
+Version: 0.0.2
 Summary: The tool is designed to mine behavior patterns
 Author: Chen Chen
 Author-email: cchen56@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -86,18 +86,14 @@
 - pandas
 - efficient_apriori
 - tqdm
 - prefixspan
 
 完整的依赖列表可以在setup.py中找到。
 
-## 开源许可
-
-MyPackage使用[MIT许可证](https://opensource.org/licenses/MIT)。请查看LICENSE文件获得更多信息。
-
 ## 贡献
 
 如果你发现任何bugs，请提交Issue或Pull Request进行更正
 
 ## 作者
 
 MyPackage由Chen Chen编写和维护。
```

### Comparing `BahaviorPattern-0.0.1/README.md` & `BahaviorPattern-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -75,18 +75,14 @@
 - pandas
 - efficient_apriori
 - tqdm
 - prefixspan
 
 完整的依赖列表可以在setup.py中找到。
 
-## 开源许可
-
-MyPackage使用[MIT许可证](https://opensource.org/licenses/MIT)。请查看LICENSE文件获得更多信息。
-
 ## 贡献
 
 如果你发现任何bugs，请提交Issue或Pull Request进行更正
 
 ## 作者
 
 MyPackage由Chen Chen编写和维护。
```

### Comparing `BahaviorPattern-0.0.1/setup.py` & `BahaviorPattern-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="BahaviorPattern",
-    version="0.0.1",
+    version="0.0.2",
     author="Chen Chen",
     author_email="cchen56@163.com",
     description="The tool is designed to mine behavior patterns",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```


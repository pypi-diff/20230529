# Comparing `tmp/ToolBox4Test-1.0.4.tar.gz` & `tmp/ToolBox4Test-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ToolBox4Test-1.0.4.tar", last modified: Mon May 29 13:56:34 2023, max compression
+gzip compressed data, was "dist\ToolBox4Test-1.0.5.tar", last modified: Mon May 29 14:27:10 2023, max compression
```

## Comparing `ToolBox4Test-1.0.4.tar` & `ToolBox4Test-1.0.5.tar`

### file list

```diff
@@ -1,35 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.132703 ToolBox4Test-1.0.4/
--rw-rw-rw-   0        0        0       91 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/.gitignore
--rw-rw-rw-   0        0        0     1085 2023-05-14 12:44:22.000000 ToolBox4Test-1.0.4/LICENSE
--rw-rw-rw-   0        0        0       43 2023-05-15 14:21:35.000000 ToolBox4Test-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1397 2023-05-29 13:56:34.132703 ToolBox4Test-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      891 2023-05-05 03:36:31.000000 ToolBox4Test-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.085838 ToolBox4Test-1.0.4/ToolBox4Test/
-drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.117081 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/
--rw-rw-rw-   0        0        0        0 2021-10-11 01:43:52.000000 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/__init__.py
--rw-rw-rw-   0        0        0    32883 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/adbShell.py
--rw-rw-rw-   0        0        0     8959 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/dataDriver.py
--rw-rw-rw-   0        0        0    15471 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/iterToolkit.py
--rw-rw-rw-   0        0        0    22733 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/toolkit.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.117081 ToolBox4Test-1.0.4/ToolBox4Test/CaseData/
--rw-rw-rw-   0        0        0      490 2023-05-05 03:35:53.000000 ToolBox4Test-1.0.4/ToolBox4Test/CaseData/__init__.py
--rw-rw-rw-   0        0        0    15311 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/CaseData/generateXmind.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.132703 ToolBox4Test-1.0.4/ToolBox4Test/Common/
--rw-rw-rw-   0        0        0        0 2021-10-11 01:39:57.000000 ToolBox4Test-1.0.4/ToolBox4Test/Common/__init__.py
--rw-rw-rw-   0        0        0    12085 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/Common/initConfig.py
--rw-rw-rw-   0        0        0    17348 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/Common/initRequest.py
--rw-rw-rw-   0        0        0    11329 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/Common/initRule.py
--rw-rw-rw-   0        0        0    15115 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/Common/initUIEnv.py
--rw-rw-rw-   0        0        0      659 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/__init__.py
--rw-rw-rw-   0        0        0     3165 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/ToolBox4Test/invokeFuncTrack.py
--rw-rw-rw-   0        0        0    25527 2023-05-16 14:24:49.000000 ToolBox4Test-1.0.4/ToolBox4Test/toolbox.py
-drwxrwxrwx   0        0        0        0 2023-05-29 13:56:34.101461 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/
--rw-rw-rw-   0        0        0     1397 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      793 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      174 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-29 13:56:33.000000 ToolBox4Test-1.0.4/ToolBox4Test.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      223 2023-05-15 14:48:08.000000 ToolBox4Test-1.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 13:56:34.132703 ToolBox4Test-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     3665 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:27:10.848165 ToolBox4Test-1.0.5/
+-rw-rw-rw-   0        0        0       91 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/.gitignore
+-rw-rw-rw-   0        0        0     1085 2023-05-14 12:44:22.000000 ToolBox4Test-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0       44 2023-05-29 14:25:13.000000 ToolBox4Test-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1397 2023-05-29 14:27:10.848165 ToolBox4Test-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      891 2023-05-05 03:36:31.000000 ToolBox4Test-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 14:27:10.801270 ToolBox4Test-1.0.5/ToolBox4Test/
+drwxrwxrwx   0        0        0        0 2023-05-29 14:27:10.832542 ToolBox4Test-1.0.5/ToolBox4Test/BaseUtility/
+-rw-rw-rw-   0        0        0        0 2021-10-11 01:43:52.000000 ToolBox4Test-1.0.5/ToolBox4Test/BaseUtility/__init__.py
+-rw-rw-rw-   0        0        0    32883 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/BaseUtility/adbShell.py
+-rw-rw-rw-   0        0        0     8959 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/BaseUtility/dataDriver.py
+-rw-rw-rw-   0        0        0    15471 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/BaseUtility/iterToolkit.py
+-rw-rw-rw-   0        0        0    22733 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/BaseUtility/toolkit.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:27:10.832542 ToolBox4Test-1.0.5/ToolBox4Test/CaseData/
+-rw-rw-rw-   0        0        0      490 2023-05-05 03:35:53.000000 ToolBox4Test-1.0.5/ToolBox4Test/CaseData/__init__.py
+-rw-rw-rw-   0        0        0    15311 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/CaseData/generateXmind.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:27:10.848165 ToolBox4Test-1.0.5/ToolBox4Test/Common/
+-rw-rw-rw-   0        0        0     1285 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/Common/Api_Template_Doc.yml
+-rw-rw-rw-   0        0        0     4309 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/Common/CMS_COMMON_ENUM.yml
+-rw-rw-rw-   0        0        0     6108 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/Common/CMS_Rules.yml
+-rw-rw-rw-   0        0        0        0 2021-10-11 01:39:57.000000 ToolBox4Test-1.0.5/ToolBox4Test/Common/__init__.py
+-rw-rw-rw-   0        0        0    12085 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/Common/initConfig.py
+-rw-rw-rw-   0        0        0    17348 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/Common/initRequest.py
+-rw-rw-rw-   0        0        0    11329 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/Common/initRule.py
+-rw-rw-rw-   0        0        0    15115 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/Common/initUIEnv.py
+-rw-rw-rw-   0        0        0      659 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/__init__.py
+-rw-rw-rw-   0        0        0     3165 2023-05-29 13:56:27.000000 ToolBox4Test-1.0.5/ToolBox4Test/invokeFuncTrack.py
+-rwxrwxrwx   0        0        0       25 2023-05-05 03:35:53.000000 ToolBox4Test-1.0.5/ToolBox4Test/toolbox.bat
+-rw-rw-rw-   0        0        0    25527 2023-05-16 14:24:49.000000 ToolBox4Test-1.0.5/ToolBox4Test/toolbox.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:27:10.816891 ToolBox4Test-1.0.5/ToolBox4Test.egg-info/
+-rw-rw-rw-   0        0        0     1397 2023-05-29 14:27:10.000000 ToolBox4Test-1.0.5/ToolBox4Test.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2023-05-29 14:27:10.000000 ToolBox4Test-1.0.5/ToolBox4Test.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 14:27:10.000000 ToolBox4Test-1.0.5/ToolBox4Test.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-05-29 14:27:10.000000 ToolBox4Test-1.0.5/ToolBox4Test.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      174 2023-05-29 14:27:10.000000 ToolBox4Test-1.0.5/ToolBox4Test.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 14:27:10.000000 ToolBox4Test-1.0.5/ToolBox4Test.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      223 2023-05-15 14:48:08.000000 ToolBox4Test-1.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 14:27:10.848165 ToolBox4Test-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     3665 2023-05-29 14:27:06.000000 ToolBox4Test-1.0.5/setup.py
```

### Comparing `ToolBox4Test-1.0.4/LICENSE` & `ToolBox4Test-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/PKG-INFO` & `ToolBox4Test-1.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolBox4Test
-Version: 1.0.4
+Version: 1.0.5
 Summary: TestToolbox 测试工具箱
 Home-page: https://gitlab.com/Gavinwhy/TestToolBox
 Author: Gavin
 Author-email: guowenwhy@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ToolBox4Test-1.0.4/README.md` & `ToolBox4Test-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/adbShell.py` & `ToolBox4Test-1.0.5/ToolBox4Test/BaseUtility/adbShell.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/dataDriver.py` & `ToolBox4Test-1.0.5/ToolBox4Test/BaseUtility/dataDriver.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/iterToolkit.py` & `ToolBox4Test-1.0.5/ToolBox4Test/BaseUtility/iterToolkit.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/BaseUtility/toolkit.py` & `ToolBox4Test-1.0.5/ToolBox4Test/BaseUtility/toolkit.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/CaseData/generateXmind.py` & `ToolBox4Test-1.0.5/ToolBox4Test/CaseData/generateXmind.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/Common/initConfig.py` & `ToolBox4Test-1.0.5/ToolBox4Test/Common/initConfig.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/Common/initRequest.py` & `ToolBox4Test-1.0.5/ToolBox4Test/Common/initRequest.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/Common/initRule.py` & `ToolBox4Test-1.0.5/ToolBox4Test/Common/initRule.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/Common/initUIEnv.py` & `ToolBox4Test-1.0.5/ToolBox4Test/Common/initUIEnv.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/__init__.py` & `ToolBox4Test-1.0.5/ToolBox4Test/__init__.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/invokeFuncTrack.py` & `ToolBox4Test-1.0.5/ToolBox4Test/invokeFuncTrack.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test/toolbox.py` & `ToolBox4Test-1.0.5/ToolBox4Test/toolbox.py`

 * *Files identical despite different names*

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test.egg-info/PKG-INFO` & `ToolBox4Test-1.0.5/ToolBox4Test.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ToolBox4Test
-Version: 1.0.4
+Version: 1.0.5
 Summary: TestToolbox 测试工具箱
 Home-page: https://gitlab.com/Gavinwhy/TestToolBox
 Author: Gavin
 Author-email: guowenwhy@foxmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ToolBox4Test-1.0.4/ToolBox4Test.egg-info/SOURCES.txt` & `ToolBox4Test-1.0.5/ToolBox4Test.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,26 +2,30 @@
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 ToolBox4Test/__init__.py
 ToolBox4Test/invokeFuncTrack.py
+ToolBox4Test/toolbox.bat
 ToolBox4Test/toolbox.py
 ToolBox4Test.egg-info/PKG-INFO
 ToolBox4Test.egg-info/SOURCES.txt
 ToolBox4Test.egg-info/dependency_links.txt
 ToolBox4Test.egg-info/entry_points.txt
 ToolBox4Test.egg-info/requires.txt
 ToolBox4Test.egg-info/top_level.txt
 ToolBox4Test/BaseUtility/__init__.py
 ToolBox4Test/BaseUtility/adbShell.py
 ToolBox4Test/BaseUtility/dataDriver.py
 ToolBox4Test/BaseUtility/iterToolkit.py
 ToolBox4Test/BaseUtility/toolkit.py
 ToolBox4Test/CaseData/__init__.py
 ToolBox4Test/CaseData/generateXmind.py
+ToolBox4Test/Common/Api_Template_Doc.yml
+ToolBox4Test/Common/CMS_COMMON_ENUM.yml
+ToolBox4Test/Common/CMS_Rules.yml
 ToolBox4Test/Common/__init__.py
 ToolBox4Test/Common/initConfig.py
 ToolBox4Test/Common/initRequest.py
 ToolBox4Test/Common/initRule.py
 ToolBox4Test/Common/initUIEnv.py
```

### Comparing `ToolBox4Test-1.0.4/setup.py` & `ToolBox4Test-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 @DateTime  : 2021/6/9 09:56
 @Contact   : guowenwhy@foxmail.com
 
 @Project   : ToolBox4Test
 @File      : setup.py
 @Describe  : TestToolbox 测试工具箱 | 辅助快速测试与验证
 ————————————————————
-@Version   : 1.0.1
+@Version   : 1.0.5
 """
 # update   : 0.1 调试
 # 1. python setup.py develop
-# 2. python setup.py sdist bdist_wheel
+# 2. python setup.py sdist upload -- dis
 # ————————————————————
 # update   : 05/14
-# 1. python setup.py sdist upload -- dis
+# 1. python setup.py sdist bdist_wheel
 # 2. twine upload dist/*
 # ————————————————————
 # update   :
 # 1.
 # 2.
 # ————————————————————
 
@@ -38,15 +38,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="ToolBox4Test",
-    version="1.0.4",
+    version="1.0.5",
     author="Gavin",
     author_email="guowenwhy@foxmail.com",
     description="TestToolbox 测试工具箱",
     long_description=long_description,
     long_description_content_type='text/markdown',
     
     # 项目主页
```


# Comparing `tmp/ats_case-0.8.0.tar.gz` & `tmp/ats_case-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.8.0.tar", last modified: Mon May 29 01:53:21 2023, max compression
+gzip compressed data, was "ats_case-0.8.1.tar", last modified: Mon May 29 02:27:05 2023, max compression
```

## Comparing `ats_case-0.8.0.tar` & `ats_case-0.8.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 01:53:21.392563 ats_case-0.8.0/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-05-29 01:53:21.390567 ats_case-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 01:53:21.018576 ats_case-0.8.0/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.0/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:53:21.218029 ats_case-0.8.0/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.0/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    18705 2023-05-22 07:49:46.000000 ats_case-0.8.0/ats_case/case/command.py
--rw-rw-rw-   0        0        0    11362 2023-05-29 01:51:13.000000 ats_case-0.8.0/ats_case/case/context.py
--rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.8.0/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.0/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:53:21.276872 ats_case-0.8.0/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.0/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.0/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.0/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:53:21.332722 ats_case-0.8.0/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.0/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.0/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.8.0/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:53:21.376605 ats_case-0.8.0/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.0/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.0/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-05-29 01:53:21.108324 ats_case-0.8.0/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-05-29 01:53:20.000000 ats_case-0.8.0/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-05-29 01:53:20.000000 ats_case-0.8.0/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 01:53:20.000000 ats_case-0.8.0/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-29 01:53:20.000000 ats_case-0.8.0/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 01:53:20.000000 ats_case-0.8.0/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 01:53:21.392563 ats_case-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      945 2023-05-29 01:51:53.000000 ats_case-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:27:05.236610 ats_case-0.8.1/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-05-29 02:27:05.234616 ats_case-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 02:27:04.752906 ats_case-0.8.1/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.8.1/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:27:05.045122 ats_case-0.8.1/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.8.1/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    18705 2023-05-22 07:49:46.000000 ats_case-0.8.1/ats_case/case/command.py
+-rw-rw-rw-   0        0        0    11367 2023-05-29 02:26:57.000000 ats_case-0.8.1/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     7500 2023-04-26 02:52:46.000000 ats_case-0.8.1/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5654 2023-05-22 01:21:46.000000 ats_case-0.8.1/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:27:05.124909 ats_case-0.8.1/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.8.1/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.8.1/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      790 2023-04-25 08:30:39.000000 ats_case-0.8.1/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:27:05.186743 ats_case-0.8.1/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.1/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-04-25 06:21:05.000000 ats_case-0.8.1/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     3611 2023-04-26 05:44:37.000000 ats_case-0.8.1/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:27:05.219654 ats_case-0.8.1/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.8.1/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2400 2023-05-29 01:45:03.000000 ats_case-0.8.1/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-05-29 02:27:04.875580 ats_case-0.8.1/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-05-29 02:27:03.000000 ats_case-0.8.1/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-05-29 02:27:04.000000 ats_case-0.8.1/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 02:27:03.000000 ats_case-0.8.1/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-05-29 02:27:03.000000 ats_case-0.8.1/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 02:27:03.000000 ats_case-0.8.1/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 02:27:05.236610 ats_case-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      945 2023-05-29 02:26:57.000000 ats_case-0.8.1/setup.py
```

### Comparing `ats_case-0.8.0/PKG-INFO` & `ats_case-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.8.0
+Version: 0.8.1
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.0/README.md` & `ats_case-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.0/ats_case/case/command.py` & `ats_case-0.8.1/ats_case/case/command.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.0/ats_case/case/context.py` & `ats_case-0.8.1/ats_case/case/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,15 +316,15 @@
 
         def acv_result(self):
             sc = fc = 0
             fs = []
             for s, result in self.acvs.items():
                 if str(result).find('不合格') >= 0:
                     fc += 1
-                    fs.append(s)
+                    fs.append(str(s))
                 else:
                     sc += 1
 
             msg = '步骤: {}步\r\n'.format(len(self._acvs))
             msg += '合格: {}步\r\n'.format(sc)
             msg += '不合格: {}步 - {}\r\n'.format(fc, ','.join(fs))
```

### Comparing `ats_case-0.8.0/ats_case/case/executor.py` & `ats_case-0.8.1/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.0/ats_case/case/translator.py` & `ats_case-0.8.1/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.0/ats_case/common/error.py` & `ats_case-0.8.1/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.0/ats_case/manage/core.py` & `ats_case-0.8.1/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.0/ats_case/manage/start.py` & `ats_case-0.8.1/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.0/ats_case/template/testcase_v1.tmp` & `ats_case-0.8.1/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.0/ats_case.egg-info/PKG-INFO` & `ats_case-0.8.1/ats_case.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.8.0
+Version: 0.8.1
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.8.0/ats_case.egg-info/SOURCES.txt` & `ats_case-0.8.1/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.8.0/setup.py` & `ats_case-0.8.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.8.0",
+    version="0.8.1",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```


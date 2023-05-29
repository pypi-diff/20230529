# Comparing `tmp/mathtranslate-2.3.1.tar.gz` & `tmp/mathtranslate-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathtranslate-2.3.1.tar", last modified: Sat May 20 06:50:08 2023, max compression
+gzip compressed data, was "mathtranslate-2.3.2.tar", last modified: Mon May 29 15:56:57 2023, max compression
```

## Comparing `mathtranslate-2.3.1.tar` & `mathtranslate-2.3.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/process_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/process_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencent.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/abstract_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/abstract_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/common_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/credential.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/exception/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/http/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/http/request.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/common/sign.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5040 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/translate_arxiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/translate_tex.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/upload_overleaf.py
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/mathtranslate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/mathtranslate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 06:50:08.000000 mathtranslate-2.3.1/mathtranslate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 06:50:08.353432 mathtranslate-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-20 06:49:53.000000 mathtranslate-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:56:57.618039 mathtranslate-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-29 15:56:57.618039 mathtranslate-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5060 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:56:57.614039 mathtranslate-2.3.2/mathtranslate/
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/process_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/process_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencent.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:56:57.614039 mathtranslate-2.3.2/mathtranslate/tencentcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:56:57.614039 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18688 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/common_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15693 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/credential.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:56:57.618039 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/exception/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:56:57.618039 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5006 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/http/request.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:56:57.618039 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/profile/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/common/sign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:56:57.618039 mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:56:57.618039 mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33836 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5350 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/translate_arxiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/translate_tex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/upload_overleaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/mathtranslate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:56:57.614039 mathtranslate-2.3.2/mathtranslate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5431 2023-05-29 15:56:57.000000 mathtranslate-2.3.2/mathtranslate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-29 15:56:57.000000 mathtranslate-2.3.2/mathtranslate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:56:57.000000 mathtranslate-2.3.2/mathtranslate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-29 15:56:57.000000 mathtranslate-2.3.2/mathtranslate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-29 15:56:57.000000 mathtranslate-2.3.2/mathtranslate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 15:56:57.000000 mathtranslate-2.3.2/mathtranslate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:56:57.618039 mathtranslate-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-29 15:56:39.000000 mathtranslate-2.3.2/setup.py
```

### Comparing `mathtranslate-2.3.1/LICENSE` & `mathtranslate-2.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/PKG-INFO` & `mathtranslate-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.3.1
+Version: 2.3.2
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.1 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.2 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.3.1/README.md` & `mathtranslate-2.3.2/README.md`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/cache.py` & `mathtranslate-2.3.2/mathtranslate/cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 def get_dirs():
     dirs = [os.path.join(ROOT_CACHE, dir) for dir in os.listdir(ROOT_CACHE)]
     return dirs
 
 
 def get_time(dir):
     timefile = os.path.join(dir, time_filename)
-    t = float(open(timefile).read())
+    t = float(open(timefile, encoding='utf-8').read())
     return t
 
 
 def write_time(dir):
     timefile = os.path.join(dir, time_filename)
     t = time.time()
-    print(t, file=open(timefile, "w"), end='')
+    print(t, file=open(timefile, "w", encoding='utf-8'), end='')
 
 
 def argmin(iterable):
     return min(enumerate(iterable), key=lambda x: x[1])[0]
 
 
 def remove_extra():
@@ -64,15 +64,15 @@
     os.makedirs(dir, exist_ok=True)
     write_time(dir)
 
 
 def load_paragraph(hash_key, hash_key_paragraph):
     filename = os.path.join(ROOT_CACHE, hash_key, hash_key_paragraph)
     if os.path.exists(filename):
-        return open(filename).read()
+        return open(filename, encoding='utf-8').read()
     else:
         return None
 
 
 def write_paragraph(hash_key, hash_key_paragraph, paragraph):
     filename = os.path.join(ROOT_CACHE, hash_key, hash_key_paragraph)
-    print(paragraph, file=open(filename, "w"), end='')
+    print(paragraph, file=open(filename, "w", encoding='utf-8'), end='')
```

### Comparing `mathtranslate-2.3.1/mathtranslate/config.py` & `mathtranslate-2.3.2/mathtranslate/config.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/encoding.py` & `mathtranslate-2.3.2/mathtranslate/encoding.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/process_file.py` & `mathtranslate-2.3.2/mathtranslate/process_file.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/process_latex.py` & `mathtranslate-2.3.2/mathtranslate/process_latex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/process_text.py` & `mathtranslate-2.3.2/mathtranslate/process_text.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencent.py` & `mathtranslate-2.3.2/mathtranslate/tencent.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/__init__.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/__init__.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/abstract_client.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/abstract_model.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/common_client.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/credential.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/exception/__init__.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/http/__init__.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/http/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/http/request.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/__init__.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/profile/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/client_profile.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/profile/http_profile.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/common/sign.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/__init__.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/__init__.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/v20180321/__init__.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/models.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py` & `mathtranslate-2.3.2/mathtranslate/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/translate.py` & `mathtranslate-2.3.2/mathtranslate/translate.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/translate_arxiv.py` & `mathtranslate-2.3.2/mathtranslate/translate_arxiv.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,39 +116,44 @@
 
     success = True
     cwd = os.getcwd()
     with tempfile.TemporaryDirectory() as temp_dir:
         print('temporary directory', temp_dir)
         os.chdir(temp_dir)
         try:
-            download_source(number, download_path)
-        except BaseException:
-            print('Cannot download source, maybe network issue or wrong link')
-            return False
-        if is_pdf(download_path):
-            # case 1
-            success = False
-        else:
-            content = gzip.decompress(open(download_path, "rb").read())
-            with open(download_path, "wb") as f:
-                f.write(content)
             try:
-                # case 4
-                with tarfile.open(download_path, mode='r') as f:
-                    f.extractall()
-                os.remove(download_path)
-            except tarfile.ReadError:
-                # case 2 or 3
-                print('This is a pure text file')
-                shutil.move(download_path, 'main.tex')
-            success = translate_dir('.', options)
-            if success:
-                # case 3
-                os.chdir(cwd)
-                zipdir(temp_dir, output_path)
+                download_source(number, download_path)
+            except BaseException:
+                print('Cannot download source, maybe network issue or wrong link')
+                return False
+            if is_pdf(download_path):
+                # case 1
+                success = False
+            else:
+                content = gzip.decompress(open(download_path, "rb").read())
+                with open(download_path, "wb") as f:
+                    f.write(content)
+                try:
+                    # case 4
+                    with tarfile.open(download_path, mode='r') as f:
+                        f.extractall()
+                    os.remove(download_path)
+                except tarfile.ReadError:
+                    # case 2 or 3
+                    print('This is a pure text file')
+                    shutil.move(download_path, 'main.tex')
+                success = translate_dir('.', options)
+                if success:
+                    # case 3
+                    os.chdir(cwd)
+                    zipdir(temp_dir, output_path)
+        except BaseException as e:
+            # first go back otherwise tempfile trying to delete the current directory that python is running in
+            os.chdir(cwd)
+            raise e
 
     if success:
         print('zip file is saved to', output_path)
         print('You can upload the zip file to overleaf to autocompile')
         return True
     else:
         print('Source code is not available for arxiv', number)
```

### Comparing `mathtranslate-2.3.1/mathtranslate/translate_tex.py` & `mathtranslate-2.3.2/mathtranslate/translate_tex.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/upload_overleaf.py` & `mathtranslate-2.3.2/mathtranslate/upload_overleaf.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate/utils.py` & `mathtranslate-2.3.2/mathtranslate/utils.py`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/mathtranslate.egg-info/PKG-INFO` & `mathtranslate-2.3.2/mathtranslate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathtranslate
-Version: 2.3.1
+Version: 2.3.2
 Summary: Translate math-heavy papers
 Home-page: https://github.com/SUSYUSTC/MathTranslate
 Author: MathTranslate developers
 Author-email: susyustc@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.1 Summary: Translate
+Metadata-Version: 2.1 Name: mathtranslate Version: 2.3.2 Summary: Translate
 math-heavy papers Home-page: https://github.com/SUSYUSTC/MathTranslate Author:
 MathTranslate developers Author-email: susyustc@gmail.com Classifier:
 Programming Language :: Python :: 3 Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown License-File: LICENSE #
 MathTranslate
      [https://img.shields.io/pypi/v/mathtranslate.svg?logo=pypi]  [https://
        img.shields.io/badge/license-Apache%202.0-yellow.svg?logo=apache]
```

### Comparing `mathtranslate-2.3.1/mathtranslate.egg-info/SOURCES.txt` & `mathtranslate-2.3.2/mathtranslate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mathtranslate-2.3.1/setup.py` & `mathtranslate-2.3.2/setup.py`

 * *Files identical despite different names*


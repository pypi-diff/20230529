# Comparing `tmp/revChatGPT-5.3.1.tar.gz` & `tmp/revChatGPT-5.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revChatGPT-5.3.1.tar", last modified: Sun May 28 11:46:07 2023, max compression
+gzip compressed data, was "revChatGPT-5.3.2.tar", last modified: Mon May 29 02:04:48 2023, max compression
```

## Comparing `revChatGPT-5.3.1.tar` & `revChatGPT-5.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.687970 revChatGPT-5.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-28 11:46:07.687970 revChatGPT-5.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 11:46:07.687970 revChatGPT-5.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.683970 revChatGPT-5.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.683970 revChatGPT-5.3.1/src/revChatGPT/
--rw-r--r--   0 runner    (1001) docker     (123)    53960 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/V1.py
--rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/V3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.687970 revChatGPT-5.3.1/src/revChatGPT/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/config/enable_internet.json
--rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/recipient.py
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/typings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/src/revChatGPT/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.683970 revChatGPT-5.3.1/src/revChatGPT.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7931 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/src/revChatGPT.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/src/revChatGPT.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/src/revChatGPT.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/src/revChatGPT.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 11:46:07.000000 revChatGPT-5.3.1/src/revChatGPT.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 11:46:07.687970 revChatGPT-5.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-28 11:45:38.000000 revChatGPT-5.3.1/tests/test_recipient.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:04:48.638136 revChatGPT-5.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-29 02:04:48.638136 revChatGPT-5.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-05-29 02:04:48.000000 revChatGPT-5.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 02:04:48.638136 revChatGPT-5.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:04:48.634136 revChatGPT-5.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:04:48.638136 revChatGPT-5.3.2/src/revChatGPT/
+-rw-r--r--   0 runner    (1001) docker     (123)    53887 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/src/revChatGPT/V1.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23208 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/src/revChatGPT/V3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/src/revChatGPT/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/src/revChatGPT/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:04:48.638136 revChatGPT-5.3.2/src/revChatGPT/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/src/revChatGPT/config/enable_internet.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/src/revChatGPT/recipient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/src/revChatGPT/typings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/src/revChatGPT/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:04:48.638136 revChatGPT-5.3.2/src/revChatGPT.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7961 2023-05-29 02:04:48.000000 revChatGPT-5.3.2/src/revChatGPT.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-05-29 02:04:48.000000 revChatGPT-5.3.2/src/revChatGPT.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:04:48.000000 revChatGPT-5.3.2/src/revChatGPT.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-29 02:04:48.000000 revChatGPT-5.3.2/src/revChatGPT.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 02:04:48.000000 revChatGPT-5.3.2/src/revChatGPT.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:04:48.638136 revChatGPT-5.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-29 02:04:08.000000 revChatGPT-5.3.2/tests/test_recipient.py
```

### Comparing `revChatGPT-5.3.1/LICENSE` & `revChatGPT-5.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.1/PKG-INFO` & `revChatGPT-5.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.3.1
+Version: 5.3.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
-English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md)
+English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md) - [한국어](./README_ko.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
```

### Comparing `revChatGPT-5.3.1/README.md` & `revChatGPT-5.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
-English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md)
+English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md) - [한국어](./README_ko.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
```

### Comparing `revChatGPT-5.3.1/setup.py` & `revChatGPT-5.3.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 if not PATH.exists():
     with open(DOCS_PATH, encoding="utf-8") as f1:
         with open(PATH, "w+", encoding="utf-8") as f2:
             f2.write(f1.read())
 
 setup(
     name="revChatGPT",
-    version="5.3.1",
+    version="5.3.2",
     description="ChatGPT is a reverse engineering of OpenAI's ChatGPT API",
     long_description=open(PATH, encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/acheong08/ChatGPT",
     project_urls={
         "Bug Report": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+",
         "Feature request": "https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+",
```

### Comparing `revChatGPT-5.3.1/src/revChatGPT/V1.py` & `revChatGPT-5.3.2/src/revChatGPT/V1.py`

 * *Files 2% similar despite different names*

```diff
@@ -682,23 +682,21 @@
 
         Args:
             response (_type_): _description_
 
         Raises:
             Error: _description_
         """
-        try:
-            response.raise_for_status()
-        except requests.exceptions.HTTPError as ex:
+        if response.status_code != 200:
             error = t.Error(
                 source="OpenAI",
                 message=response.text,
                 code=response.status_code,
             )
-            raise error from ex
+            raise error
 
     @logger(is_timed=True)
     def get_conversations(
         self,
         offset: int = 0,
         limit: int = 20,
         encoding: str | None = None,
```

### Comparing `revChatGPT-5.3.1/src/revChatGPT/V3.py` & `revChatGPT-5.3.2/src/revChatGPT/V3.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.1/src/revChatGPT/__init__.py` & `revChatGPT-5.3.2/src/revChatGPT/__init__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.1/src/revChatGPT/__main__.py` & `revChatGPT-5.3.2/src/revChatGPT/__main__.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.1/src/revChatGPT/config/enable_internet.json` & `revChatGPT-5.3.2/src/revChatGPT/config/enable_internet.json`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.1/src/revChatGPT/recipient.py` & `revChatGPT-5.3.2/src/revChatGPT/recipient.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.1/src/revChatGPT/typings.py` & `revChatGPT-5.3.2/src/revChatGPT/typings.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.1/src/revChatGPT/utils.py` & `revChatGPT-5.3.2/src/revChatGPT/utils.py`

 * *Files identical despite different names*

### Comparing `revChatGPT-5.3.1/src/revChatGPT.egg-info/PKG-INFO` & `revChatGPT-5.3.2/src/revChatGPT.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revChatGPT
-Version: 5.3.1
+Version: 5.3.2
 Summary: ChatGPT is a reverse engineering of OpenAI's ChatGPT API
 Home-page: https://github.com/acheong08/ChatGPT
 Author: Antonio Cheong
 Author-email: acheong@student.dalat.org
 License: GNU General Public License v2.0
 Project-URL: Bug Report, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=bug-report&template=bug_report.yml&title=%5BBug%5D%3A+
 Project-URL: Feature request, https://github.com/acheong08/ChatGPT/issues/new?assignees=&labels=enhancement&template=feature_request.yml&title=%5BFeature+Request%5D%3A+
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ChatGPT <img src="https://github.com/acheong08/ChatGPT/blob/main/logo.png?raw=true" width="15%"></img>
 
-English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md)
+English - [中文](./README_zh.md) - [Spanish](./README_sp.md) -  [日本語](./README_ja.md) - [한국어](./README_ko.md)
 
 [![PyPi](https://img.shields.io/pypi/v/revChatGPT.svg)](https://pypi.python.org/pypi/revChatGPT)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/revChatGPT)](https://pypi.python.org/pypi/revChatGPT)
 [![Downloads](https://static.pepy.tech/badge/revchatgpt)](https://pypi.python.org/pypi/revChatGPT)
 
 Reverse Engineered ChatGPT API by OpenAI. Extensible for chatbots etc.
```

### Comparing `revChatGPT-5.3.1/tests/test_recipient.py` & `revChatGPT-5.3.2/tests/test_recipient.py`

 * *Files identical despite different names*


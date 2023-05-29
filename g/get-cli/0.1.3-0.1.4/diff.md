# Comparing `tmp/get_cli-0.1.3.tar.gz` & `tmp/get_cli-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "get_cli-0.1.3.tar", max compression
+gzip compressed data, was "get_cli-0.1.4.tar", max compression
```

## Comparing `get_cli-0.1.3.tar` & `get_cli-0.1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1068 2023-03-21 09:45:17.540265 get_cli-0.1.3/LICENSE
--rw-r--r--   0        0        0     2122 2023-05-29 20:11:01.400002 get_cli-0.1.3/README.md
--rw-r--r--   0        0        0       47 2023-03-23 16:14:33.179468 get_cli-0.1.3/get_cli/__init__.py
--rw-r--r--   0        0        0      123 2023-03-23 13:04:57.484834 get_cli-0.1.3/get_cli/__main__.py
--rw-r--r--   0        0        0     1852 2023-03-23 13:22:39.258854 get_cli-0.1.3/get_cli/cli.py
--rw-r--r--   0        0        0      170 2023-03-22 20:54:11.558292 get_cli-0.1.3/get_cli/constants.py
--rw-r--r--   0        0        0     1645 2023-03-23 16:12:07.385824 get_cli-0.1.3/get_cli/controller.py
--rw-r--r--   0        0        0      310 2023-03-23 13:09:09.061781 get_cli-0.1.3/get_cli/main.py
--rw-r--r--   0        0        0     1177 2023-03-23 16:12:07.386244 get_cli-0.1.3/get_cli/service.py
--rw-r--r--   0        0        0     1837 2023-03-23 16:12:07.386631 get_cli-0.1.3/get_cli/storage.py
--rw-r--r--   0        0        0      520 2023-05-29 19:50:21.796455 get_cli-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 get_cli-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-21 09:45:17.540265 get_cli-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2122 2023-05-29 20:11:01.400002 get_cli-0.1.4/README.md
+-rw-r--r--   0        0        0       47 2023-05-29 20:17:19.743971 get_cli-0.1.4/get_cli/__init__.py
+-rw-r--r--   0        0        0      123 2023-03-23 13:04:57.484834 get_cli-0.1.4/get_cli/__main__.py
+-rw-r--r--   0        0        0     1852 2023-03-23 13:22:39.258854 get_cli-0.1.4/get_cli/cli.py
+-rw-r--r--   0        0        0      170 2023-03-22 20:54:11.558292 get_cli-0.1.4/get_cli/constants.py
+-rw-r--r--   0        0        0     1645 2023-03-23 16:12:07.385824 get_cli-0.1.4/get_cli/controller.py
+-rw-r--r--   0        0        0      310 2023-03-23 13:09:09.061781 get_cli-0.1.4/get_cli/main.py
+-rw-r--r--   0        0        0     1177 2023-03-23 16:12:07.386244 get_cli-0.1.4/get_cli/service.py
+-rw-r--r--   0        0        0     1837 2023-03-23 16:12:07.386631 get_cli-0.1.4/get_cli/storage.py
+-rw-r--r--   0        0        0      520 2023-05-29 20:17:27.111575 get_cli-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2907 1970-01-01 00:00:00.000000 get_cli-0.1.4/PKG-INFO
```

### Comparing `get_cli-0.1.3/LICENSE` & `get_cli-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `get_cli-0.1.3/README.md` & `get_cli-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `get_cli-0.1.3/get_cli/cli.py` & `get_cli-0.1.4/get_cli/cli.py`

 * *Files identical despite different names*

### Comparing `get_cli-0.1.3/get_cli/controller.py` & `get_cli-0.1.4/get_cli/controller.py`

 * *Files identical despite different names*

### Comparing `get_cli-0.1.3/get_cli/service.py` & `get_cli-0.1.4/get_cli/service.py`

 * *Files identical despite different names*

### Comparing `get_cli-0.1.3/get_cli/storage.py` & `get_cli-0.1.4/get_cli/storage.py`

 * *Files identical despite different names*

### Comparing `get_cli-0.1.3/pyproject.toml` & `get_cli-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "get-cli"
-version = "0.1.3"
+version = "0.1.4"
 description = "A simple unsafe cli tool to store and fetch data locally."
 license = "MIT"
 authors = ["noamtamir <noam.tamir@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/noamtamir/get-cli"
 
 [tool.poetry.dependencies]
```

### Comparing `get_cli-0.1.3/PKG-INFO` & `get_cli-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: get-cli
-Version: 0.1.3
+Version: 0.1.4
 Summary: A simple unsafe cli tool to store and fetch data locally.
 Home-page: https://github.com/noamtamir/get-cli
 License: MIT
 Author: noamtamir
 Author-email: noam.tamir@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


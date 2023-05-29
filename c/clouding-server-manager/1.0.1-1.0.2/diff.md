# Comparing `tmp/clouding_server_manager-1.0.1.tar.gz` & `tmp/clouding_server_manager-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clouding_server_manager-1.0.1.tar", max compression
+gzip compressed data, was "clouding_server_manager-1.0.2.tar", max compression
```

## Comparing `clouding_server_manager-1.0.1.tar` & `clouding_server_manager-1.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1065 2023-05-01 21:40:31.138645 clouding_server_manager-1.0.1/LICENSE
--rw-r--r--   0        0        0     6956 2023-05-26 10:29:34.188075 clouding_server_manager-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-25 23:26:38.831500 clouding_server_manager-1.0.1/clouding_server_manager/__init__.py
--rw-r--r--   0        0        0      590 2023-05-26 10:08:29.138115 clouding_server_manager-1.0.1/clouding_server_manager/__main__.py
--rw-r--r--   0        0        0     3998 2023-05-26 09:45:25.433435 clouding_server_manager-1.0.1/clouding_server_manager/commands.py
--rw-r--r--   0        0        0      782 2023-05-26 09:45:32.340190 clouding_server_manager-1.0.1/clouding_server_manager/constants.py
--rw-r--r--   0        0        0     7418 2023-05-26 09:45:23.540078 clouding_server_manager-1.0.1/clouding_server_manager/helpers.py
--rw-r--r--   0        0        0      851 2023-05-26 10:29:38.304795 clouding_server_manager-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7560 1970-01-01 00:00:00.000000 clouding_server_manager-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-01 21:40:31.138645 clouding_server_manager-1.0.2/LICENSE
+-rw-r--r--   0        0        0     6956 2023-05-26 10:29:34.188075 clouding_server_manager-1.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-25 23:26:38.831500 clouding_server_manager-1.0.2/clouding_server_manager/__init__.py
+-rw-r--r--   0        0        0      590 2023-05-26 10:08:29.138115 clouding_server_manager-1.0.2/clouding_server_manager/__main__.py
+-rw-r--r--   0        0        0     3998 2023-05-26 09:45:25.433435 clouding_server_manager-1.0.2/clouding_server_manager/commands.py
+-rw-r--r--   0        0        0      782 2023-05-26 09:45:32.340190 clouding_server_manager-1.0.2/clouding_server_manager/constants.py
+-rw-r--r--   0        0        0     7418 2023-05-26 09:45:23.540078 clouding_server_manager-1.0.2/clouding_server_manager/helpers.py
+-rw-r--r--   0        0        0      892 2023-05-29 12:16:13.284767 clouding_server_manager-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     7560 1970-01-01 00:00:00.000000 clouding_server_manager-1.0.2/PKG-INFO
```

### Comparing `clouding_server_manager-1.0.1/LICENSE` & `clouding_server_manager-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.1/README.md` & `clouding_server_manager-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.1/clouding_server_manager/__main__.py` & `clouding_server_manager-1.0.2/clouding_server_manager/__main__.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.1/clouding_server_manager/commands.py` & `clouding_server_manager-1.0.2/clouding_server_manager/commands.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.1/clouding_server_manager/constants.py` & `clouding_server_manager-1.0.2/clouding_server_manager/constants.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.1/clouding_server_manager/helpers.py` & `clouding_server_manager-1.0.2/clouding_server_manager/helpers.py`

 * *Files identical despite different names*

### Comparing `clouding_server_manager-1.0.1/pyproject.toml` & `clouding_server_manager-1.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [tool.poetry]
 name = "clouding-server-manager"
-version = "1.0.1"
+version = "1.0.2"
 description = "A Python project to easily manage Clouding servers from the command line."
 authors = ["dmarts05 <dmarts05@estudiantes.unileon.es>"]
 readme = "README.md"
 packages = [{include = "clouding_server_manager"}]
 
 [tool.poetry.scripts]
 clouding-sm = "clouding_server_manager.__main__:main"
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 requests = "^2.31.0"
 python-dotenv = "^1.0.0"
 click = "^8.1.3"
 
+[tool.poetry.group.dev]
+optional = true
+
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.3.2"
 black = "^23.3.0"
 flake8 = "^6.0.0"
 isort = "^5.12.0"
 mypy = "^1.3.0"
 types-requests = "^2.31.0.0"
```

### Comparing `clouding_server_manager-1.0.1/PKG-INFO` & `clouding_server_manager-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clouding-server-manager
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python project to easily manage Clouding servers from the command line.
 Author: dmarts05
 Author-email: dmarts05@estudiantes.unileon.es
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```


# Comparing `tmp/krakenpy-0.1.3.tar.gz` & `tmp/krakenpy-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakenpy-0.1.3.tar", max compression
+gzip compressed data, was "krakenpy-0.1.4.tar", max compression
```

## Comparing `krakenpy-0.1.3.tar` & `krakenpy-0.1.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      789 2023-05-29 10:49:53.300047 krakenpy-0.1.3/README.md
--rw-r--r--   0        0        0       86 2023-05-29 10:49:53.300692 krakenpy-0.1.3/krakenpy/__init__.py
--rw-r--r--   0        0        0      267 2023-05-28 15:41:35.959814 krakenpy-0.1.3/krakenpy/exceptions.py
--rw-r--r--   0        0        0     1429 2023-05-29 10:49:53.300935 krakenpy-0.1.3/krakenpy/payloads.py
--rw-r--r--   0        0        0      111 2023-05-28 14:45:32.763564 krakenpy-0.1.3/krakenpy/response.py
--rw-r--r--   0        0        0     3897 2023-05-29 10:49:53.301299 krakenpy-0.1.3/krakenpy/service.py
--rw-r--r--   0        0        0      883 2023-05-29 10:49:53.301515 krakenpy-0.1.3/krakenpy/utils.py
--rw-r--r--   0        0        0      854 2023-05-29 10:49:53.301784 krakenpy-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 krakenpy-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      789 2023-05-29 11:26:25.536152 krakenpy-0.1.4/README.md
+-rw-r--r--   0        0        0       86 2023-05-29 11:26:25.536152 krakenpy-0.1.4/krakenpy/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-29 11:26:25.536152 krakenpy-0.1.4/krakenpy/exceptions.py
+-rw-r--r--   0        0        0     1429 2023-05-29 11:26:25.536152 krakenpy-0.1.4/krakenpy/payloads.py
+-rw-r--r--   0        0        0      111 2023-05-29 11:26:25.536152 krakenpy-0.1.4/krakenpy/response.py
+-rw-r--r--   0        0        0     3897 2023-05-29 11:26:25.536152 krakenpy-0.1.4/krakenpy/service.py
+-rw-r--r--   0        0        0      883 2023-05-29 11:26:25.536152 krakenpy-0.1.4/krakenpy/utils.py
+-rw-r--r--   0        0        0      922 2023-05-29 11:26:25.536152 krakenpy-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 krakenpy-0.1.4/PKG-INFO
```

### Comparing `krakenpy-0.1.3/README.md` & `krakenpy-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `krakenpy-0.1.3/krakenpy/payloads.py` & `krakenpy-0.1.4/krakenpy/payloads.py`

 * *Files identical despite different names*

### Comparing `krakenpy-0.1.3/krakenpy/service.py` & `krakenpy-0.1.4/krakenpy/service.py`

 * *Files identical despite different names*

### Comparing `krakenpy-0.1.3/krakenpy/utils.py` & `krakenpy-0.1.4/krakenpy/utils.py`

 * *Files identical despite different names*

### Comparing `krakenpy-0.1.3/pyproject.toml` & `krakenpy-0.1.4/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krakenpy"
-version = "0.1.3"
+version = "0.1.4"
 description = "krakenpy is tool in which we integrated kraken crypto exchange API"
 authors = ["Sheikh Haris Zahid"]
 readme = "README.md"
 homepage = "https://github.com/Sheikhharis50/krakenpy"
 repository = "https://github.com/Sheikhharis50/krakenpy"
 classifiers = [
     "Development Status :: 1 - Planning",
@@ -19,11 +19,16 @@
 [tool.poetry.dependencies]
 python = "^3.10"
 krakenex = "^2.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.1"
 requests-mock = "^1.10.0"
+black = "^23.3.0"
+isort = "^5.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.isort]
+profile = "black"
```

### Comparing `krakenpy-0.1.3/PKG-INFO` & `krakenpy-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: krakenpy
-Version: 0.1.3
+Version: 0.1.4
 Summary: krakenpy is tool in which we integrated kraken crypto exchange API
 Home-page: https://github.com/Sheikhharis50/krakenpy
 Keywords: kraken,kraken-api,python,crypto
 Author: Sheikh Haris Zahid
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
```


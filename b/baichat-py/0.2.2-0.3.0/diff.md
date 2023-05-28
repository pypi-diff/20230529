# Comparing `tmp/baichat_py-0.2.2.tar.gz` & `tmp/baichat_py-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baichat_py-0.2.2.tar", max compression
+gzip compressed data, was "baichat_py-0.3.0.tar", max compression
```

## Comparing `baichat_py-0.2.2.tar` & `baichat_py-0.3.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1162 2023-05-24 19:17:37.396739 baichat_py-0.2.2/README.md
--rw-r--r--   0        0        0     5807 2023-05-24 19:17:37.397739 baichat_py-0.2.2/baichat_py/__init__.py
--rw-r--r--   0        0        0     1198 2023-05-24 19:17:37.398739 baichat_py-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2318 1970-01-01 00:00:00.000000 baichat_py-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      383 2023-05-28 21:57:26.827539 baichat_py-0.3.0/README.md
+-rw-r--r--   0        0        0     3303 2023-05-28 21:57:26.827539 baichat_py-0.3.0/baichat_py/__init__.py
+-rw-r--r--   0        0        0     1204 2023-05-28 21:58:18.399573 baichat_py-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 baichat_py-0.3.0/PKG-INFO
```

### Comparing `baichat_py-0.2.2/pyproject.toml` & `baichat_py-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "baichat-py"
-version = "0.2.2"
+version = "0.3.0"
 description = ""
 authors = ["0xMRTT <0xMRTT@proton.me>"]
 maintainers = ["0xMRTT <0xMRTT@proton.me>"]
 readme = "README.md"
 packages = [{include = "baichat_py"}]
 license = "GPL-3.0-or-later"
 homepage = "https://codeberg.org/Bavarder/baichat-py"
@@ -23,17 +23,16 @@
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://codeberg.org/Bavarder/baichat-py/issues"
 
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aiohttp = "^3.8.0"
-requests = "^2.29.0"
-
+fake-useragent = "^1.1.3"
+curl-cffi = "^0.5.6"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.source]]
 name = "codeberg"
```


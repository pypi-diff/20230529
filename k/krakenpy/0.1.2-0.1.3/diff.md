# Comparing `tmp/krakenpy-0.1.2.tar.gz` & `tmp/krakenpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "krakenpy-0.1.2.tar", max compression
+gzip compressed data, was "krakenpy-0.1.3.tar", max compression
```

## Comparing `krakenpy-0.1.2.tar` & `krakenpy-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      385 2023-05-29 07:29:26.565971 krakenpy-0.1.2/README.md
--rw-r--r--   0        0        0       87 2023-05-29 07:37:23.449910 krakenpy-0.1.2/krakenpy/__init__.py
--rw-r--r--   0        0        0      267 2023-05-28 15:41:35.959814 krakenpy-0.1.2/krakenpy/exceptions.py
--rw-r--r--   0        0        0     1019 2023-05-28 15:13:20.092650 krakenpy-0.1.2/krakenpy/payloads.py
--rw-r--r--   0        0        0      111 2023-05-28 14:45:32.763564 krakenpy-0.1.2/krakenpy/response.py
--rw-r--r--   0        0        0     2484 2023-05-29 07:19:27.539209 krakenpy-0.1.2/krakenpy/service.py
--rw-r--r--   0        0        0      306 2023-05-28 15:47:57.288600 krakenpy-0.1.2/krakenpy/utils.py
--rw-r--r--   0        0        0      854 2023-05-29 07:37:23.449892 krakenpy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1195 1970-01-01 00:00:00.000000 krakenpy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      789 2023-05-29 10:49:53.300047 krakenpy-0.1.3/README.md
+-rw-r--r--   0        0        0       86 2023-05-29 10:49:53.300692 krakenpy-0.1.3/krakenpy/__init__.py
+-rw-r--r--   0        0        0      267 2023-05-28 15:41:35.959814 krakenpy-0.1.3/krakenpy/exceptions.py
+-rw-r--r--   0        0        0     1429 2023-05-29 10:49:53.300935 krakenpy-0.1.3/krakenpy/payloads.py
+-rw-r--r--   0        0        0      111 2023-05-28 14:45:32.763564 krakenpy-0.1.3/krakenpy/response.py
+-rw-r--r--   0        0        0     3897 2023-05-29 10:49:53.301299 krakenpy-0.1.3/krakenpy/service.py
+-rw-r--r--   0        0        0      883 2023-05-29 10:49:53.301515 krakenpy-0.1.3/krakenpy/utils.py
+-rw-r--r--   0        0        0      854 2023-05-29 10:49:53.301784 krakenpy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 krakenpy-0.1.3/PKG-INFO
```

### Comparing `krakenpy-0.1.2/pyproject.toml` & `krakenpy-0.1.3/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "krakenpy"
-version = "0.1.2"
+version = "0.1.3"
 description = "krakenpy is tool in which we integrated kraken crypto exchange API"
 authors = ["Sheikh Haris Zahid"]
 readme = "README.md"
 homepage = "https://github.com/Sheikhharis50/krakenpy"
 repository = "https://github.com/Sheikhharis50/krakenpy"
 classifiers = [
     "Development Status :: 1 - Planning",
```


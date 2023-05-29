# Comparing `tmp/dgl_client-0.3.tar.gz` & `tmp/dgl_client-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgl_client-0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dgl_client-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dgl_client-0.3.tar` & `dgl_client-0.3.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       36 2023-05-26 06:08:29.040320 dgl_client-0.3/.gitignore
--rw-r--r--   0        0        0       69 2023-05-26 06:08:29.040320 dgl_client-0.3/README.md
--rw-r--r--   0        0        0       62 2023-05-29 11:33:58.648532 dgl_client-0.3/dgl_client/__init__.py
--rw-r--r--   0        0        0     6036 2023-05-29 11:24:12.508534 dgl_client-0.3/dgl_client/api_cli.py
--rw-r--r--   0        0        0     3928 2023-05-29 11:12:10.896537 dgl_client-0.3/dgl_client/main.py
--rw-r--r--   0        0        0        0 2023-05-26 06:08:29.040320 dgl_client-0.3/dgl_client/utils.py
--rw-r--r--   0        0        0      438 2023-05-26 06:08:29.040320 dgl_client-0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 06:08:29.040320 dgl_client-0.3/tests/__init__.py
--rw-r--r--   0        0        0      952 2023-05-29 11:23:50.236534 dgl_client-0.3/tests/create_token.py
--rw-r--r--   0        0        0     2074 2023-05-29 08:36:18.388573 dgl_client-0.3/tests/test_decode.py
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 dgl_client-0.3/PKG-INFO
+-rw-r--r--   0        0        0       36 2023-05-26 06:08:29.040320 dgl_client-0.3.1/.gitignore
+-rw-r--r--   0        0        0       69 2023-05-26 06:08:29.040320 dgl_client-0.3.1/README.md
+-rw-r--r--   0        0        0       64 2023-05-29 12:09:55.816524 dgl_client-0.3.1/dgl_client/__init__.py
+-rw-r--r--   0        0        0     6036 2023-05-29 11:24:12.508534 dgl_client-0.3.1/dgl_client/api_cli.py
+-rw-r--r--   0        0        0     3928 2023-05-29 11:12:10.896537 dgl_client-0.3.1/dgl_client/main.py
+-rw-r--r--   0        0        0        0 2023-05-26 06:08:29.040320 dgl_client-0.3.1/dgl_client/utils.py
+-rw-r--r--   0        0        0      441 2023-05-29 12:09:11.160524 dgl_client-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 06:08:29.040320 dgl_client-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0      952 2023-05-29 11:23:50.236534 dgl_client-0.3.1/tests/create_token.py
+-rw-r--r--   0        0        0     2074 2023-05-29 08:36:18.388573 dgl_client-0.3.1/tests/test_decode.py
+-rw-r--r--   0        0        0      296 1970-01-01 00:00:00.000000 dgl_client-0.3.1/PKG-INFO
```

### Comparing `dgl_client-0.3/dgl_client/api_cli.py` & `dgl_client-0.3.1/dgl_client/api_cli.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.3/dgl_client/main.py` & `dgl_client-0.3.1/dgl_client/main.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.3/tests/create_token.py` & `dgl_client-0.3.1/tests/create_token.py`

 * *Files identical despite different names*

### Comparing `dgl_client-0.3/tests/test_decode.py` & `dgl_client-0.3.1/tests/test_decode.py`

 * *Files identical despite different names*


# Comparing `tmp/file_io_cli_tddschn-1.1.1.tar.gz` & `tmp/file_io_cli_tddschn-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_io_cli_tddschn-1.1.1.tar", max compression
+gzip compressed data, was "file_io_cli_tddschn-1.1.2.tar", max compression
```

## Comparing `file_io_cli_tddschn-1.1.1.tar` & `file_io_cli_tddschn-1.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.1.1/LICENSE
--rw-r--r--   0        0        0     1084 2023-05-03 13:52:47.818681 file_io_cli_tddschn-1.1.1/LICENSE.txt
--rw-r--r--   0        0        0     3191 2023-05-29 10:57:54.277752 file_io_cli_tddschn-1.1.1/README.md
--rw-r--r--   0        0        0      147 2023-05-29 11:14:25.180666 file_io_cli_tddschn-1.1.1/file_io_cli_tddschn/__init__.py
--rw-r--r--   0        0        0    11701 2023-05-29 11:13:41.329372 file_io_cli_tddschn-1.1.1/file_io_cli_tddschn/cli.py
--rw-r--r--   0        0        0      321 2023-05-03 15:12:26.690529 file_io_cli_tddschn-1.1.1/file_io_cli_tddschn/config.py
--rw-r--r--   0        0        0      247 2023-05-29 11:13:36.261241 file_io_cli_tddschn-1.1.1/file_io_cli_tddschn/utils.py
--rw-r--r--   0        0        0     1168 2023-05-29 11:14:25.179595 file_io_cli_tddschn-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1084 2023-05-29 11:15:29.791564 file_io_cli_tddschn-1.1.2/LICENSE.txt
+-rw-r--r--   0        0        0     3191 2023-05-29 10:57:54.277752 file_io_cli_tddschn-1.1.2/README.md
+-rw-r--r--   0        0        0      147 2023-05-29 11:15:46.446979 file_io_cli_tddschn-1.1.2/file_io_cli_tddschn/__init__.py
+-rw-r--r--   0        0        0    11741 2023-05-29 11:14:47.400771 file_io_cli_tddschn-1.1.2/file_io_cli_tddschn/cli.py
+-rw-r--r--   0        0        0      321 2023-05-03 15:12:26.690529 file_io_cli_tddschn-1.1.2/file_io_cli_tddschn/config.py
+-rw-r--r--   0        0        0      247 2023-05-29 11:13:36.261241 file_io_cli_tddschn-1.1.2/file_io_cli_tddschn/utils.py
+-rw-r--r--   0        0        0     1168 2023-05-29 11:15:46.445162 file_io_cli_tddschn-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.1.2/PKG-INFO
```

### Comparing `file_io_cli_tddschn-1.1.1/LICENSE` & `file_io_cli_tddschn-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.1/LICENSE.txt` & `file_io_cli_tddschn-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.1/README.md` & `file_io_cli_tddschn-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.1/file_io_cli_tddschn/cli.py` & `file_io_cli_tddschn-1.1.2/file_io_cli_tddschn/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Copyright (c) 2018 Niklas Rosenstein
+# Copyright (c) 2023 Teddy Xinyuan Chen
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to
 # deal in the Software without restriction, including without limitation the
 # rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 # sell copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
```

### Comparing `file_io_cli_tddschn-1.1.1/pyproject.toml` & `file_io_cli_tddschn-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "file.io-cli-tddschn"
-version = "1.1.1"
+version = "1.1.2"
 description = "Command-line tool to upload files to https://file.io"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 # packages = [{ include = "file_io_cli.py" }]
 packages = [{ include = "file_io_cli_tddschn" }]
 homepage = "https://github.com/tddschn/file.io-cli-tddschn"
```

### Comparing `file_io_cli_tddschn-1.1.1/PKG-INFO` & `file_io_cli_tddschn-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-io-cli-tddschn
-Version: 1.1.1
+Version: 1.1.2
 Summary: Command-line tool to upload files to https://file.io
 Home-page: https://github.com/tddschn/file.io-cli-tddschn
 License: MIT
 Keywords: file.io,utility,uploader,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
```


# Comparing `tmp/file_io_cli_tddschn-1.1.2.tar.gz` & `tmp/file_io_cli_tddschn-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file_io_cli_tddschn-1.1.2.tar", max compression
+gzip compressed data, was "file_io_cli_tddschn-1.1.3.tar", max compression
```

## Comparing `file_io_cli_tddschn-1.1.2.tar` & `file_io_cli_tddschn-1.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.1.2/LICENSE
--rw-r--r--   0        0        0     1084 2023-05-29 11:15:29.791564 file_io_cli_tddschn-1.1.2/LICENSE.txt
--rw-r--r--   0        0        0     3191 2023-05-29 10:57:54.277752 file_io_cli_tddschn-1.1.2/README.md
--rw-r--r--   0        0        0      147 2023-05-29 11:15:46.446979 file_io_cli_tddschn-1.1.2/file_io_cli_tddschn/__init__.py
--rw-r--r--   0        0        0    11741 2023-05-29 11:14:47.400771 file_io_cli_tddschn-1.1.2/file_io_cli_tddschn/cli.py
--rw-r--r--   0        0        0      321 2023-05-03 15:12:26.690529 file_io_cli_tddschn-1.1.2/file_io_cli_tddschn/config.py
--rw-r--r--   0        0        0      247 2023-05-29 11:13:36.261241 file_io_cli_tddschn-1.1.2/file_io_cli_tddschn/utils.py
--rw-r--r--   0        0        0     1168 2023-05-29 11:15:46.445162 file_io_cli_tddschn-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1106 2023-05-03 14:09:29.309388 file_io_cli_tddschn-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1084 2023-05-29 11:15:29.791564 file_io_cli_tddschn-1.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     3342 2023-05-29 11:18:30.561155 file_io_cli_tddschn-1.1.3/README.md
+-rw-r--r--   0        0        0      147 2023-05-29 11:18:43.143047 file_io_cli_tddschn-1.1.3/file_io_cli_tddschn/__init__.py
+-rw-r--r--   0        0        0    11741 2023-05-29 11:14:47.400771 file_io_cli_tddschn-1.1.3/file_io_cli_tddschn/cli.py
+-rw-r--r--   0        0        0      321 2023-05-03 15:12:26.690529 file_io_cli_tddschn-1.1.3/file_io_cli_tddschn/config.py
+-rw-r--r--   0        0        0      247 2023-05-29 11:13:36.261241 file_io_cli_tddschn-1.1.3/file_io_cli_tddschn/utils.py
+-rw-r--r--   0        0        0     1168 2023-05-29 11:18:43.141656 file_io_cli_tddschn-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4148 1970-01-01 00:00:00.000000 file_io_cli_tddschn-1.1.3/PKG-INFO
```

### Comparing `file_io_cli_tddschn-1.1.2/LICENSE` & `file_io_cli_tddschn-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.2/LICENSE.txt` & `file_io_cli_tddschn-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.2/README.md` & `file_io_cli_tddschn-1.1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -117,14 +117,19 @@
 $ git clone https://github.com/tddschn/file.io-cli-tddschn.git
 $ cd file.io-cli-tddschn
 $ poetry install
 ```
 
 ### Changelog
 
+#### 1.1.2
+
+* Add -N, --num-threads option to upload files multiple times concurrently
+* Fix the uploaded file name when using relative path like `.`
+
 #### 1.0.5
 
 * Add -v, --verbose option to print server response in JSON
 * Use poetry for developing and packaging
 
 #### v1.0.4
```

### Comparing `file_io_cli_tddschn-1.1.2/file_io_cli_tddschn/cli.py` & `file_io_cli_tddschn-1.1.3/file_io_cli_tddschn/cli.py`

 * *Files identical despite different names*

### Comparing `file_io_cli_tddschn-1.1.2/pyproject.toml` & `file_io_cli_tddschn-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "file.io-cli-tddschn"
-version = "1.1.2"
+version = "1.1.3"
 description = "Command-line tool to upload files to https://file.io"
 authors = ["Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 # packages = [{ include = "file_io_cli.py" }]
 packages = [{ include = "file_io_cli_tddschn" }]
 homepage = "https://github.com/tddschn/file.io-cli-tddschn"
```

### Comparing `file_io_cli_tddschn-1.1.2/PKG-INFO` & `file_io_cli_tddschn-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-io-cli-tddschn
-Version: 1.1.2
+Version: 1.1.3
 Summary: Command-line tool to upload files to https://file.io
 Home-page: https://github.com/tddschn/file.io-cli-tddschn
 License: MIT
 Keywords: file.io,utility,uploader,CLI
 Author: Teddy Xinyuan Chen
 Author-email: 45612704+tddschn@users.noreply.github.com
 Requires-Python: >=3.11,<4.0
@@ -137,14 +137,19 @@
 $ git clone https://github.com/tddschn/file.io-cli-tddschn.git
 $ cd file.io-cli-tddschn
 $ poetry install
 ```
 
 ### Changelog
 
+#### 1.1.2
+
+* Add -N, --num-threads option to upload files multiple times concurrently
+* Fix the uploaded file name when using relative path like `.`
+
 #### 1.0.5
 
 * Add -v, --verbose option to print server response in JSON
 * Use poetry for developing and packaging
 
 #### v1.0.4
```


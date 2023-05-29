# Comparing `tmp/ssrs-0.1.1.tar.gz` & `tmp/ssrs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssrs-0.1.1.tar", max compression
+gzip compressed data, was "ssrs-0.1.2.tar", max compression
```

## Comparing `ssrs-0.1.1.tar` & `ssrs-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      601 2023-05-29 00:35:28.568475 ssrs-0.1.1/README.md
--rw-r--r--   0        0        0      974 2023-05-29 00:33:20.821785 ssrs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 23:36:23.863958 ssrs-0.1.1/src/ssrs/__init__.py
--rw-r--r--   0        0        0       62 2023-05-29 00:34:18.233342 ssrs-0.1.1/src/ssrs/__main__.py
--rwxr-xr-x   0        0        0     3184 2023-05-29 00:32:54.704382 ssrs-0.1.1/src/ssrs/ssrs.py
--rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 ssrs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      601 2023-05-29 00:35:28.568475 ssrs-0.1.2/README.md
+-rw-r--r--   0        0        0     1025 2023-05-29 01:14:49.448674 ssrs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 23:36:23.863958 ssrs-0.1.2/src/ssrs/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-29 00:34:18.233342 ssrs-0.1.2/src/ssrs/__main__.py
+-rwxr-xr-x   0        0        0     3184 2023-05-29 00:32:54.704382 ssrs-0.1.2/src/ssrs/ssrs.py
+-rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 ssrs-0.1.2/PKG-INFO
```

### Comparing `ssrs-0.1.1/README.md` & `ssrs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ssrs-0.1.1/pyproject.toml` & `ssrs-0.1.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "ssrs"
-version = "0.1.1"
-description = "Simple Scripting for Rust enables you to create \"scripts\", written in rust and \"interpret\" them, by using a shebang line. It's basically a way to run quick-and-dirty programs without having to setup a new crate."
+version = "0.1.2"
+description = "'Simple Scripting for Rust' enables you to run rust source files as scripts, from the command line, by prefixing them with a shebang line. It's useful because sometimes you just want to write a quick-and-dirty 'script', without having to creaate a new crate/package."
 authors = ["Bruno Fauth <149593@upf.br>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `ssrs-0.1.1/src/ssrs/ssrs.py` & `ssrs-0.1.2/src/ssrs/ssrs.py`

 * *Files identical despite different names*

### Comparing `ssrs-0.1.1/PKG-INFO` & `ssrs-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ssrs
-Version: 0.1.1
-Summary: Simple Scripting for Rust enables you to create "scripts", written in rust and "interpret" them, by using a shebang line. It's basically a way to run quick-and-dirty programs without having to setup a new crate.
+Version: 0.1.2
+Summary: 'Simple Scripting for Rust' enables you to run rust source files as scripts, from the command line, by prefixing them with a shebang line. It's useful because sometimes you just want to write a quick-and-dirty 'script', without having to creaate a new crate/package.
 Home-page: https://github.com/brunofauth/ssrs
 License: MIT
 Keywords: rust,scripting,shebang
 Author: Bruno Fauth
 Author-email: 149593@upf.br
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


# Comparing `tmp/ssrs-0.1.2.tar.gz` & `tmp/ssrs-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssrs-0.1.2.tar", max compression
+gzip compressed data, was "ssrs-0.1.3.tar", max compression
```

## Comparing `ssrs-0.1.2.tar` & `ssrs-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      601 2023-05-29 00:35:28.568475 ssrs-0.1.2/README.md
--rw-r--r--   0        0        0     1025 2023-05-29 01:14:49.448674 ssrs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 23:36:23.863958 ssrs-0.1.2/src/ssrs/__init__.py
--rw-r--r--   0        0        0       62 2023-05-29 00:34:18.233342 ssrs-0.1.2/src/ssrs/__main__.py
--rwxr-xr-x   0        0        0     3184 2023-05-29 00:32:54.704382 ssrs-0.1.2/src/ssrs/ssrs.py
--rw-r--r--   0        0        0     1601 1970-01-01 00:00:00.000000 ssrs-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      656 2023-05-29 01:44:00.289440 ssrs-0.1.3/README.md
+-rw-r--r--   0        0        0     1025 2023-05-29 01:43:19.775796 ssrs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 23:36:23.863958 ssrs-0.1.3/src/ssrs/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-29 00:34:18.233342 ssrs-0.1.3/src/ssrs/__main__.py
+-rwxr-xr-x   0        0        0     3184 2023-05-29 00:32:54.704382 ssrs-0.1.3/src/ssrs/ssrs.py
+-rw-r--r--   0        0        0     1656 1970-01-01 00:00:00.000000 ssrs-0.1.3/PKG-INFO
```

### Comparing `ssrs-0.1.2/README.md` & `ssrs-0.1.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -4,34 +4,36 @@
 line, by prefixing them with a shebang line. It's useful because sometimes you 
 just want to write a quick-and-dirty "script", without having to creaate a new 
 crate/package.
 
 
 # Installation
 
-## With `pip`
+## With `pipx`
 ```sh
-sudo pip install ssrs
+pipx install ssrs
 ```
 
-## With `pipx`
+## With `makepkg`
 ```sh
-pipx install ssrs
+git clone "https://github.com/brunofauth/ssrs"
+cd ssrs
+makepkg -cris
 ```
 
 # Usage
 
 ## From the Command Line
 ```sh
 ssrs-cli [ssrs-options] -- <script-file> [script-options]
 ```
 
 ## From Script Files
 ```rust
-#! /usr/bin/ssrs
+#! /usr/bin/env ssrs
 
 // your rust code here
 fn main() {
     println!("Hello World!");
 }
 ```
```

### Comparing `ssrs-0.1.2/pyproject.toml` & `ssrs-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssrs"
-version = "0.1.2"
+version = "0.1.3"
 description = "'Simple Scripting for Rust' enables you to run rust source files as scripts, from the command line, by prefixing them with a shebang line. It's useful because sometimes you just want to write a quick-and-dirty 'script', without having to creaate a new crate/package."
 authors = ["Bruno Fauth <149593@upf.br>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ssrs-0.1.2/src/ssrs/ssrs.py` & `ssrs-0.1.3/src/ssrs/ssrs.py`

 * *Files identical despite different names*

### Comparing `ssrs-0.1.2/PKG-INFO` & `ssrs-0.1.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssrs
-Version: 0.1.2
+Version: 0.1.3
 Summary: 'Simple Scripting for Rust' enables you to run rust source files as scripts, from the command line, by prefixing them with a shebang line. It's useful because sometimes you just want to write a quick-and-dirty 'script', without having to creaate a new crate/package.
 Home-page: https://github.com/brunofauth/ssrs
 License: MIT
 Keywords: rust,scripting,shebang
 Author: Bruno Fauth
 Author-email: 149593@upf.br
 Requires-Python: >=3.10,<4.0
@@ -25,34 +25,36 @@
 line, by prefixing them with a shebang line. It's useful because sometimes you 
 just want to write a quick-and-dirty "script", without having to creaate a new 
 crate/package.
 
 
 # Installation
 
-## With `pip`
+## With `pipx`
 ```sh
-sudo pip install ssrs
+pipx install ssrs
 ```
 
-## With `pipx`
+## With `makepkg`
 ```sh
-pipx install ssrs
+git clone "https://github.com/brunofauth/ssrs"
+cd ssrs
+makepkg -cris
 ```
 
 # Usage
 
 ## From the Command Line
 ```sh
 ssrs-cli [ssrs-options] -- <script-file> [script-options]
 ```
 
 ## From Script Files
 ```rust
-#! /usr/bin/ssrs
+#! /usr/bin/env ssrs
 
 // your rust code here
 fn main() {
     println!("Hello World!");
 }
 ```
```


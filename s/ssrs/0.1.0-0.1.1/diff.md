# Comparing `tmp/ssrs-0.1.0.tar.gz` & `tmp/ssrs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssrs-0.1.0.tar", max compression
+gzip compressed data, was "ssrs-0.1.1.tar", max compression
```

## Comparing `ssrs-0.1.0.tar` & `ssrs-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0      379 2023-05-28 23:01:09.302131 ssrs-0.1.0/README.md
--rw-r--r--   0        0        0      908 2023-05-28 23:46:32.454223 ssrs-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 23:36:23.863958 ssrs-0.1.0/src/ssrs/__init__.py
--rw-r--r--   0        0        0       66 2023-05-28 23:37:06.914411 ssrs-0.1.0/src/ssrs/__main__.py
--rwxr-xr-x   0        0        0     3053 2023-05-28 22:53:43.326673 ssrs-0.1.0/src/ssrs/ssrs.py
--rw-r--r--   0        0        0     1283 1970-01-01 00:00:00.000000 ssrs-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      601 2023-05-29 00:35:28.568475 ssrs-0.1.1/README.md
+-rw-r--r--   0        0        0      974 2023-05-29 00:33:20.821785 ssrs-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 23:36:23.863958 ssrs-0.1.1/src/ssrs/__init__.py
+-rw-r--r--   0        0        0       62 2023-05-29 00:34:18.233342 ssrs-0.1.1/src/ssrs/__main__.py
+-rwxr-xr-x   0        0        0     3184 2023-05-29 00:32:54.704382 ssrs-0.1.1/src/ssrs/ssrs.py
+-rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 ssrs-0.1.1/PKG-INFO
```

### Comparing `ssrs-0.1.0/pyproject.toml` & `ssrs-0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tool.poetry]
 name = "ssrs"
-version = "0.1.0"
+version = "0.1.1"
 description = "Simple Scripting for Rust enables you to create \"scripts\", written in rust and \"interpret\" them, by using a shebang line. It's basically a way to run quick-and-dirty programs without having to setup a new crate."
 authors = ["Bruno Fauth <149593@upf.br>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
+    "Programming Language :: Rust",
 ]
 keywords = ["rust", "scripting", "shebang"]
 repository = "https://github.com/brunofauth/ssrs"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/brunofauth/ssrs/issues"
 "Homepage" = "https://github.com/brunofauth/ssrs"
@@ -21,8 +22,10 @@
 python = "^3.10"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-ssrs = 'ssrs.ssrs:_main'
+ssrs = 'ssrs.ssrs:shebang'
+ssrs-cli = 'ssrs.ssrs:cli'
+
```

### Comparing `ssrs-0.1.0/src/ssrs/ssrs.py` & `ssrs-0.1.1/src/ssrs/ssrs.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from pathlib import Path
 import argparse as ap
 import os
 import shutil
 import subprocess as sp
 import enum
+import sys
 
 
 AnyPath = str | bytes | os.PathLike[str] | os.PathLike[bytes]
 
 
 def user_home() -> str:
     if os.name == "nt":
@@ -85,25 +86,29 @@
     script_name = file.with_suffix("").name
     try_init_crate(get_env_crate_path())
     shutil.copy2(file, get_scripts_path())
     build_script(script_name)
     run_script(script_name, script_args)
 
 
-def get_args() -> ap.Namespace:
+def get_args(source: list[str] | None = None) -> ap.Namespace:
     parser = ap.ArgumentParser(
         description="Use as a shebang line to run rust source file as scripts")
     parser.add_argument("input_file",
         help="The rust source file to run as a script")
     parser.add_argument("script_args", nargs='*',
         help="Arguments to be passed to the rust script")
 
-    return parser.parse_args()
+    return parser.parse_args(args=source)
 
 
-def _main() -> None:
+def cli() -> None:
     main(**vars(get_args()))
 
 
+def shebang() -> None:
+    main(**vars(get_args(source=["--"] + sys.argv[1:])))
+
+
 if __name__ == "__main__":
-    _main()
+    cli()
```

### Comparing `ssrs-0.1.0/PKG-INFO` & `ssrs-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,56 @@
 Metadata-Version: 2.1
 Name: ssrs
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple Scripting for Rust enables you to create "scripts", written in rust and "interpret" them, by using a shebang line. It's basically a way to run quick-and-dirty programs without having to setup a new crate.
 Home-page: https://github.com/brunofauth/ssrs
 License: MIT
 Keywords: rust,scripting,shebang
 Author: Bruno Fauth
 Author-email: 149593@upf.br
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Rust
 Project-URL: Bug Tracker, https://github.com/brunofauth/ssrs/issues
 Project-URL: Repository, https://github.com/brunofauth/ssrs
 Description-Content-Type: text/markdown
 
 # Description
 
 This program enables you to run rust source files as scripts, from the command 
 line, by prefixing them with a shebang line. It's useful because sometimes you 
 just want to write a quick-and-dirty "script", without having to creaate a new 
 crate/package.
 
 
+# Installation
+
+## With `pip`
+```sh
+sudo pip install ssrs
+```
+
+## With `pipx`
+```sh
+pipx install ssrs
+```
+
 # Usage
 
+## From the Command Line
+```sh
+ssrs-cli [ssrs-options] -- <script-file> [script-options]
+```
+
+## From Script Files
 ```rust
 #! /usr/bin/ssrs
 
 // your rust code here
 fn main() {
     println!("Hello World!");
 }
```


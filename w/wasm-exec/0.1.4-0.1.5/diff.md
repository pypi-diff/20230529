# Comparing `tmp/wasm_exec-0.1.4.tar.gz` & `tmp/wasm_exec-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasm_exec-0.1.4.tar", max compression
+gzip compressed data, was "wasm_exec-0.1.5.tar", max compression
```

## Comparing `wasm_exec-0.1.4.tar` & `wasm_exec-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-29 05:14:37.918375 wasm_exec-0.1.4/LICENSE
--rw-r--r--   0        0        0     3058 2023-05-29 05:14:37.918375 wasm_exec-0.1.4/README.md
--rw-r--r--   0        0        0      743 2023-05-29 05:14:37.918375 wasm_exec-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3519 2023-05-29 05:14:37.918375 wasm_exec-0.1.4/wasm_exec/__init__.py
--rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 wasm_exec-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-29 05:27:38.625179 wasm_exec-0.1.5/LICENSE
+-rw-r--r--   0        0        0     3058 2023-05-29 05:27:38.625179 wasm_exec-0.1.5/README.md
+-rw-r--r--   0        0        0      818 2023-05-29 05:27:38.625179 wasm_exec-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3519 2023-05-29 05:27:38.625179 wasm_exec-0.1.5/wasm_exec/__init__.py
+-rw-r--r--   0        0        0 20538911 2023-05-29 05:27:38.733183 wasm_exec-0.1.5/wasm_runtime/python-3.11.3.wasm
+-rw-r--r--   0        0        0      121 2023-05-29 05:27:38.733183 wasm_exec-0.1.5/wasm_runtime/python-3.11.3.wasm.sha256sum
+-rw-r--r--   0        0        0     1424 2023-05-29 05:27:38.733183 wasm_exec-0.1.5/wasm_runtime/wasm_runtime.py
+-rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 wasm_exec-0.1.5/PKG-INFO
```

### Comparing `wasm_exec-0.1.4/LICENSE` & `wasm_exec-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.4/README.md` & `wasm_exec-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.4/pyproject.toml` & `wasm_exec-0.1.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 [tool.poetry]
 name = "wasm-exec"
-version = "0.1.4"
+version = "0.1.5"
 description = "WASM-powered, sandboxed version of `exec()` for running dynamic code."
 authors = ["Justin Flick"]
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/jflick58/wasm_exec"
+packages = [
+    { include = "wasm_exec" },
+]
+include = ["wasm_runtime/*"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 wasmtime = "^9.0.0"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `wasm_exec-0.1.4/wasm_exec/__init__.py` & `wasm_exec-0.1.5/wasm_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.4/PKG-INFO` & `wasm_exec-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasm-exec
-Version: 0.1.4
+Version: 0.1.5
 Summary: WASM-powered, sandboxed version of `exec()` for running dynamic code.
 Home-page: https://www.github.com/jflick58/wasm_exec
 License: MIT
 Author: Justin Flick
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


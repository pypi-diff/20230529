# Comparing `tmp/wasm_exec-0.1.0.tar.gz` & `tmp/wasm_exec-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasm_exec-0.1.0.tar", max compression
+gzip compressed data, was "wasm_exec-0.1.1.tar", max compression
```

## Comparing `wasm_exec-0.1.0.tar` & `wasm_exec-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-29 03:57:34.894330 wasm_exec-0.1.0/LICENSE
--rw-r--r--   0        0        0     3054 2023-05-29 03:57:34.894330 wasm_exec-0.1.0/README.md
--rw-r--r--   0        0        0      779 2023-05-29 03:57:35.002332 wasm_exec-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3360 2023-05-29 03:57:35.002332 wasm_exec-0.1.0/wasm_exec/__init__.py
--rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 wasm_exec-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-29 04:15:58.628379 wasm_exec-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3209 2023-05-29 04:15:58.628379 wasm_exec-0.1.1/README.md
+-rw-r--r--   0        0        0 20538911 2023-05-29 04:15:58.748384 wasm_exec-0.1.1/bin/python-3.11.3.wasm
+-rw-r--r--   0        0        0      121 2023-05-29 04:15:58.748384 wasm_exec-0.1.1/bin/python-3.11.3.wasm.sha256sum
+-rw-r--r--   0        0        0     1424 2023-05-29 04:15:58.748384 wasm_exec-0.1.1/bin/wasm_runtime.py
+-rw-r--r--   0        0        0      812 2023-05-29 04:15:58.748384 wasm_exec-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3360 2023-05-29 04:15:58.748384 wasm_exec-0.1.1/wasm_exec/__init__.py
+-rw-r--r--   0        0        0     3907 1970-01-01 00:00:00.000000 wasm_exec-0.1.1/PKG-INFO
```

### Comparing `wasm_exec-0.1.0/LICENSE` & `wasm_exec-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.0/README.md` & `wasm_exec-0.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # wasm_exec
 Wasm-powered, sandboxed implementation of `exec()` for safely running dynamic Python code
 
 [![lint](https://github.com/jflick58/wasm_exec/actions/workflows/lint.yml/badge.svg)](https://github.com/jflick58/wasm_exec/actions/workflows/lint.yml)
 [![test](https://github.com/jflick58/wasm_exec/actions/workflows/test.yml/badge.svg)](https://github.com/jflick58/wasm_exec/actions/workflows/test.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/wasm-exec.svg)](https://badge.fury.io/py/wasm-exec)
 
 ## Install 
 
 ```pip install wasm_exec```
 
 ## Usage
 ```
@@ -18,15 +19,15 @@
 
 >> Hello World!
 ```
 
 ## How does this work? 
 
 - Arbitrary Python code is passed to the `wasm_exec` function 
-- A seperate Wasm-based Python interpreter is setup via wasmtime in a chroot jail
+- A seperate Wasm-based Python interpreter is setup via [wasmtime](https://github.com/bytecodealliance/wasmtime-py/tree/main) in a chroot jail
 - The arbitrary code is executed safely inside your isolated intepreter
 
 ## Why? 
 
 There are number of use-cases emerging that require arbitrary code execution, often code that is generate by LLMs (Large Language Models) like ChatGPT. This can enable some really cool functionality - like generative BI or website generation - but also introduce a massive security flaw if implemented via `eval() or exec()`. This is because arbitrary code can be executed using these methods. In a worst case scenario, `exec`'ing arbitrary code could enable some to `rm -rf /` your entire server! 
 
 This repo intends to provide a secure method of executing arbitrary Python code to empower LLM-based code generation. This was orignally intended to be a direct PR to [Langchain](https://github.com/hwchase17/langchain) but given that the problems with `exec()` extend to the entire Python ecosystem, it was decided that it would be better as a standalone package.
```

### Comparing `wasm_exec-0.1.0/pyproject.toml` & `wasm_exec-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "wasm-exec"
-version = "0.1.0"
+version = "0.1.1"
 description = "WASM-powered sandboxed version of `exec()` for running dynamic code."
 authors = ["Justin Flick"]
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/jflick58/wasm_exec"
 packages = [{include = "wasm_exec"}]
+include = ["bin/*", "README.md"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 wasmtime = "^9.0.0"
 
 [tool.poetry.group.test]
 optional = true
```

### Comparing `wasm_exec-0.1.0/wasm_exec/__init__.py` & `wasm_exec-0.1.1/wasm_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.0/PKG-INFO` & `wasm_exec-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasm-exec
-Version: 0.1.0
+Version: 0.1.1
 Summary: WASM-powered sandboxed version of `exec()` for running dynamic code.
 Home-page: https://www.github.com/jflick58/wasm_exec
 License: MIT
 Author: Justin Flick
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,15 @@
 
 # wasm_exec
 Wasm-powered, sandboxed implementation of `exec()` for safely running dynamic Python code
 
 [![lint](https://github.com/jflick58/wasm_exec/actions/workflows/lint.yml/badge.svg)](https://github.com/jflick58/wasm_exec/actions/workflows/lint.yml)
 [![test](https://github.com/jflick58/wasm_exec/actions/workflows/test.yml/badge.svg)](https://github.com/jflick58/wasm_exec/actions/workflows/test.yml)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![PyPI version](https://badge.fury.io/py/wasm-exec.svg)](https://badge.fury.io/py/wasm-exec)
 
 ## Install 
 
 ```pip install wasm_exec```
 
 ## Usage
 ```
@@ -36,15 +37,15 @@
 
 >> Hello World!
 ```
 
 ## How does this work? 
 
 - Arbitrary Python code is passed to the `wasm_exec` function 
-- A seperate Wasm-based Python interpreter is setup via wasmtime in a chroot jail
+- A seperate Wasm-based Python interpreter is setup via [wasmtime](https://github.com/bytecodealliance/wasmtime-py/tree/main) in a chroot jail
 - The arbitrary code is executed safely inside your isolated intepreter
 
 ## Why? 
 
 There are number of use-cases emerging that require arbitrary code execution, often code that is generate by LLMs (Large Language Models) like ChatGPT. This can enable some really cool functionality - like generative BI or website generation - but also introduce a massive security flaw if implemented via `eval() or exec()`. This is because arbitrary code can be executed using these methods. In a worst case scenario, `exec`'ing arbitrary code could enable some to `rm -rf /` your entire server! 
 
 This repo intends to provide a secure method of executing arbitrary Python code to empower LLM-based code generation. This was orignally intended to be a direct PR to [Langchain](https://github.com/hwchase17/langchain) but given that the problems with `exec()` extend to the entire Python ecosystem, it was decided that it would be better as a standalone package.
```


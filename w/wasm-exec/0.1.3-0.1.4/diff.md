# Comparing `tmp/wasm_exec-0.1.3.tar.gz` & `tmp/wasm_exec-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wasm_exec-0.1.3.tar", max compression
+gzip compressed data, was "wasm_exec-0.1.4.tar", max compression
```

## Comparing `wasm_exec-0.1.3.tar` & `wasm_exec-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-05-29 04:59:00.761112 wasm_exec-0.1.3/LICENSE
--rw-r--r--   0        0        0     3058 2023-05-29 04:59:00.761112 wasm_exec-0.1.3/README.md
--rw-r--r--   0        0        0      743 2023-05-29 04:59:00.761112 wasm_exec-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3360 2023-05-29 04:59:00.765112 wasm_exec-0.1.3/wasm_exec/__init__.py
--rw-r--r--   0        0        0 20538911 2023-05-29 04:59:00.881112 wasm_exec-0.1.3/wasm_exec/python-3.11.3.wasm
--rw-r--r--   0        0        0      121 2023-05-29 04:59:00.881112 wasm_exec-0.1.3/wasm_exec/python-3.11.3.wasm.sha256sum
--rw-r--r--   0        0        0     1424 2023-05-29 04:59:00.881112 wasm_exec-0.1.3/wasm_exec/wasm_runtime.py
--rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 wasm_exec-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-29 05:14:37.918375 wasm_exec-0.1.4/LICENSE
+-rw-r--r--   0        0        0     3058 2023-05-29 05:14:37.918375 wasm_exec-0.1.4/README.md
+-rw-r--r--   0        0        0      743 2023-05-29 05:14:37.918375 wasm_exec-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3519 2023-05-29 05:14:37.918375 wasm_exec-0.1.4/wasm_exec/__init__.py
+-rw-r--r--   0        0        0     3757 1970-01-01 00:00:00.000000 wasm_exec-0.1.4/PKG-INFO
```

### Comparing `wasm_exec-0.1.3/LICENSE` & `wasm_exec-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.3/README.md` & `wasm_exec-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `wasm_exec-0.1.3/pyproject.toml` & `wasm_exec-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wasm-exec"
-version = "0.1.3"
+version = "0.1.4"
 description = "WASM-powered, sandboxed version of `exec()` for running dynamic code."
 authors = ["Justin Flick"]
 license = "MIT"
 readme = "README.md"
 repository = "https://www.github.com/jflick58/wasm_exec"
 
 [tool.poetry.dependencies]
```

### Comparing `wasm_exec-0.1.3/wasm_exec/__init__.py` & `wasm_exec-0.1.4/wasm_exec/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,15 +51,20 @@
     engine_cfg = Config()
     engine_cfg.consume_fuel = use_fuel
     engine_cfg.cache = True
 
     linker = Linker(Engine(engine_cfg))
     linker.define_wasi()
 
-    python_module = Module.from_file(linker.engine, "bin/python-3.11.3.wasm")
+    runtime_path = runtime_path = os.path.abspath(
+        os.path.join(
+            os.path.dirname(__file__), "..", "wasm_runtime", "python-3.11.3.wasm"
+        )
+    )
+    python_module = Module.from_file(linker.engine, runtime_path)
 
     config = WasiConfig()
 
     config.argv = ("python", "-c", dedent(code))
     print(dedent(code))
 
     with tempfile.TemporaryDirectory() as chroot:
```

### Comparing `wasm_exec-0.1.3/PKG-INFO` & `wasm_exec-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wasm-exec
-Version: 0.1.3
+Version: 0.1.4
 Summary: WASM-powered, sandboxed version of `exec()` for running dynamic code.
 Home-page: https://www.github.com/jflick58/wasm_exec
 License: MIT
 Author: Justin Flick
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


# Comparing `tmp/umbral_pre-0.9.1.tar.gz` & `tmp/umbral_pre-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umbral_pre-0.9.1.tar", last modified: Sat Feb 18 01:33:11 2023, max compression
+gzip compressed data, was "umbral_pre-0.9.2.tar", last modified: Sun Feb 19 00:51:26 2023, max compression
```

## Comparing `umbral_pre-0.9.1.tar` & `umbral_pre-0.9.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 01:33:11.238469 umbral_pre-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-18 01:33:10.000000 umbral_pre-0.9.1/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-18 01:33:11.238469 umbral_pre-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 01:33:11.234468 umbral_pre-0.9.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 01:33:11.234468 umbral_pre-0.9.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/example/example.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-18 01:33:11.238469 umbral_pre-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 01:33:11.234468 umbral_pre-0.9.1/src/
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 01:33:11.238469 umbral_pre-0.9.1/umbral_pre/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/umbral_pre/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4972 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/umbral_pre/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-18 01:33:07.000000 umbral_pre-0.9.1/umbral_pre/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-18 01:33:11.238469 umbral_pre-0.9.1/umbral_pre.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-18 01:33:11.000000 umbral_pre-0.9.1/umbral_pre.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-18 01:33:11.000000 umbral_pre-0.9.1/umbral_pre.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 01:33:11.000000 umbral_pre-0.9.1/umbral_pre.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-18 01:33:11.000000 umbral_pre-0.9.1/umbral_pre.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-18 01:33:11.000000 umbral_pre-0.9.1/umbral_pre.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 00:51:26.214584 umbral_pre-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-02-19 00:51:25.000000 umbral_pre-0.9.2/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (123)    34916 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-19 00:51:26.214584 umbral_pre-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 00:51:26.210584 umbral_pre-0.9.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10239 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 00:51:26.210584 umbral_pre-0.9.2/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     3225 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/example/example.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-19 00:51:26.214584 umbral_pre-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 00:51:26.210584 umbral_pre-0.9.2/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 00:51:26.214584 umbral_pre-0.9.2/umbral_pre/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/umbral_pre/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/umbral_pre/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 00:51:22.000000 umbral_pre-0.9.2/umbral_pre/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 00:51:26.214584 umbral_pre-0.9.2/umbral_pre.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-02-19 00:51:26.000000 umbral_pre-0.9.2/umbral_pre.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-02-19 00:51:26.000000 umbral_pre-0.9.2/umbral_pre.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 00:51:26.000000 umbral_pre-0.9.2/umbral_pre.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 00:51:26.000000 umbral_pre-0.9.2/umbral_pre.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-19 00:51:26.000000 umbral_pre-0.9.2/umbral_pre.egg-info/top_level.txt
```

### Comparing `umbral_pre-0.9.1/LICENSE` & `umbral_pre-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `umbral_pre-0.9.1/PKG-INFO` & `umbral_pre-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umbral_pre
-Version: 0.9.1
+Version: 0.9.2
 Summary: Implementation of Umbral proxy reencryption algorithm
 Home-page: https://github.com/nucypher/rust-umbral/tree/master/umbral-pre-python
 Author: Bogdan Opanchuk
 Author-email: bogdan@opanchuk.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `umbral_pre-0.9.1/README.md` & `umbral_pre-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `umbral_pre-0.9.1/docs/Makefile` & `umbral_pre-0.9.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `umbral_pre-0.9.1/docs/conf.py` & `umbral_pre-0.9.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'umbral-pre'
 copyright = '2020, Bogdan Opanchuk'
 author = 'Bogdan Opanchuk'
 
 # The full version, including alpha/beta/rc tags
-release = '0.9.1'
+release = '0.9.2'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
```

### Comparing `umbral_pre-0.9.1/docs/index.rst` & `umbral_pre-0.9.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `umbral_pre-0.9.1/docs/make.bat` & `umbral_pre-0.9.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `umbral_pre-0.9.1/example/example.py` & `umbral_pre-0.9.2/example/example.py`

 * *Files identical despite different names*

### Comparing `umbral_pre-0.9.1/setup.py` & `umbral_pre-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="umbral_pre",
     description="Implementation of Umbral proxy reencryption algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version="0.9.1",
+    version="0.9.2",
     author="Bogdan Opanchuk",
     author_email="bogdan@opanchuk.net",
     url="https://github.com/nucypher/rust-umbral/tree/master/umbral-pre-python",
     rust_extensions=[RustExtension("umbral_pre._umbral", binding=Binding.PyO3)],
     packages=["umbral_pre"],
     package_data = {
         'umbral_pre': ['py.typed', '__init__.pyi'],
```

### Comparing `umbral_pre-0.9.1/src/lib.rs` & `umbral_pre-0.9.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `umbral_pre-0.9.1/umbral_pre/__init__.pyi` & `umbral_pre-0.9.2/umbral_pre/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     def to_be_bytes(self) -> bytes:
         ...
 
 
 class RecoverableSignature:
 
     @staticmethod
-    def from_be_bytes(data: bytes) -> Signature:
+    def from_be_bytes(data: bytes) -> RecoverableSignature:
         ...
 
     def to_be_bytes(self) -> bytes:
         ...
 
 
 class Capsule:
```

### Comparing `umbral_pre-0.9.1/umbral_pre.egg-info/PKG-INFO` & `umbral_pre-0.9.2/umbral_pre.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umbral-pre
-Version: 0.9.1
+Version: 0.9.2
 Summary: Implementation of Umbral proxy reencryption algorithm
 Home-page: https://github.com/nucypher/rust-umbral/tree/master/umbral-pre-python
 Author: Bogdan Opanchuk
 Author-email: bogdan@opanchuk.net
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```


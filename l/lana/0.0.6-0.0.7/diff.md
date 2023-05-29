# Comparing `tmp/lana-0.0.6.tar.gz` & `tmp/lana-0.0.7.tar.gz`

## Comparing `lana-0.0.6.tar` & `lana-0.0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.0.6/Cargo.toml
--rw-r--r--   0      501       20      709 2023-05-15 16:30:29.000000 lana-0.0.6/.gitignore
--rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.0.6/LICENSE
--rw-r--r--   0      501       20      412 2023-05-15 21:37:24.000000 lana-0.0.6/README.md
--rw-r--r--   0      501       20       71 2023-05-15 16:08:19.000000 lana-0.0.6/examples/example.py
--rw-r--r--   0      501       20       63 2023-05-16 07:53:35.000000 lana-0.0.6/lana/__init__.py
--rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.0.6/pyproject.toml
--rw-r--r--   0      501       20      490 2023-05-15 15:55:44.000000 lana-0.0.6/src/lib.rs
--rw-r--r--   0      501       20     7648 2023-05-16 07:54:29.000000 lana-0.0.6/Cargo.lock
--rw-r--r--   0        0        0      953 1970-01-01 00:00:00.000000 lana-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.0.7/Cargo.toml
+-rw-r--r--   0      501       20      709 2023-05-15 16:30:29.000000 lana-0.0.7/.gitignore
+-rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.0.7/LICENSE
+-rw-r--r--   0      501       20      382 2023-05-29 09:46:07.000000 lana-0.0.7/README.md
+-rw-r--r--   0      501       20       72 2023-05-29 10:02:57.000000 lana-0.0.7/examples/example.py
+-rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.0.7/lana/__init__.py
+-rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.0.7/pyproject.toml
+-rw-r--r--   0      501       20      626 2023-05-29 10:03:06.000000 lana-0.0.7/src/lib.rs
+-rw-r--r--   0      501       20     7648 2023-05-29 09:31:56.000000 lana-0.0.7/Cargo.lock
+-rw-r--r--   0        0        0      923 1970-01-01 00:00:00.000000 lana-0.0.7/PKG-INFO
```

### Comparing `lana-0.0.6/.gitignore` & `lana-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `lana-0.0.6/LICENSE` & `lana-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lana-0.0.6/pyproject.toml` & `lana-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lana-0.0.6/Cargo.lock` & `lana-0.0.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "lana"
-version = "0.0.6"
+version = "0.0.7"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.144"
```

### Comparing `lana-0.0.6/PKG-INFO` & `lana-0.0.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lana
-Version: 0.0.6
+Version: 0.0.7
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Linear Algebra experimental library
 Keywords: linear algebra
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
@@ -21,15 +21,15 @@
 (__,-'      ,'o"(            )>
    (       (__,-'            )
     `-'._.--._(             )
        |||  |||`-'._.--._.-'
                   |||  |||
 ```
 
-$\textit{\textbf{L}inear \textbf{A}lgebra for \textbf{n}octurnal and \textbf{a}dventurous data scientists}$
+**L**inear **a**lgebra for **n**octurnal and **a**dventurous data scientists.
 
 ## Install 
 
 ```console
 pip install lana
 ```
```


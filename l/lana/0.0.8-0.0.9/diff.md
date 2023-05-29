# Comparing `tmp/lana-0.0.8.tar.gz` & `tmp/lana-0.0.9.tar.gz`

## Comparing `lana-0.0.8.tar` & `lana-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,11 @@
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.0.8/Cargo.toml
--rw-r--r--   0      501       20      709 2023-05-15 16:30:29.000000 lana-0.0.8/.gitignore
--rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.0.8/LICENSE
--rw-r--r--   0      501       20      484 2023-05-29 10:10:32.000000 lana-0.0.8/README.md
--rw-r--r--   0      501       20       63 2023-05-29 10:08:25.000000 lana-0.0.8/examples/example.py
--rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.0.8/lana/__init__.py
--rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.0.8/pyproject.toml
--rw-r--r--   0      501       20      787 2023-05-29 10:20:29.000000 lana-0.0.8/src/lib.rs
--rw-r--r--   0      501       20     7648 2023-05-29 10:20:37.000000 lana-0.0.8/Cargo.lock
--rw-r--r--   0        0        0     1025 1970-01-01 00:00:00.000000 lana-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.0.9/Cargo.toml
+-rw-r--r--   0      501       20      709 2023-05-15 16:30:29.000000 lana-0.0.9/.gitignore
+-rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.0.9/LICENSE
+-rw-r--r--   0      501       20      501 2023-05-29 10:26:22.000000 lana-0.0.9/README.md
+-rw-r--r--   0      501       20      475 2023-05-29 10:54:53.000000 lana-0.0.9/build.py
+-rw-r--r--   0      501       20      117 2023-05-29 10:23:44.000000 lana-0.0.9/examples/example.py
+-rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.0.9/lana/__init__.py
+-rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.0.9/pyproject.toml
+-rw-r--r--   0      501       20      888 2023-05-29 10:44:24.000000 lana-0.0.9/src/lib.rs
+-rw-r--r--   0      501       20     7648 2023-05-29 10:30:23.000000 lana-0.0.9/Cargo.lock
+-rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 lana-0.0.9/PKG-INFO
```

### Comparing `lana-0.0.8/.gitignore` & `lana-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `lana-0.0.8/LICENSE` & `lana-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lana-0.0.8/pyproject.toml` & `lana-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lana-0.0.8/src/lib.rs` & `lana-0.0.9/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,19 @@
     #[staticmethod]
     pub fn zeros(dimensions: (usize, usize)) -> Self {
         let (rows, cols) = dimensions;
         let data: Vec<Vec<f64>> = vec![vec![0.0; cols]; rows];
         Matrix { data }
     }
 
+    #[staticmethod]
+    pub fn matrix(data: Vec<Vec<f64>>) -> Self {
+        Matrix { data } 
+    }
+
     #[getter]
     pub fn shape(&self) -> (usize, usize) {
         let rows = self.data.len();
         let cols = self.data[0].len();
         (rows, cols)
     }
```

### Comparing `lana-0.0.8/Cargo.lock` & `lana-0.0.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "lana"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.144"
```

### Comparing `lana-0.0.8/PKG-INFO` & `lana-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lana
-Version: 0.0.8
+Version: 0.0.9
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Linear Algebra experimental library
 Keywords: linear algebra
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
@@ -36,10 +36,11 @@
 ## Example 
 
 ```python
 from lana import Matrix
 
 mat = Matrix.zeros((3,3))
 mat.print()
+print(mat.shape)
 ```
```


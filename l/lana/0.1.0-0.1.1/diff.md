# Comparing `tmp/lana-0.1.0.tar.gz` & `tmp/lana-0.1.1.tar.gz`

## Comparing `lana-0.1.0.tar` & `lana-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.1.0/Cargo.toml
--rw-r--r--   0      501       20      709 2023-05-15 16:30:29.000000 lana-0.1.0/.gitignore
--rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.0/LICENSE
--rw-r--r--   0      501       20      719 2023-05-29 13:17:37.000000 lana-0.1.0/README.md
--rw-r--r--   0      501       20      475 2023-05-29 10:54:53.000000 lana-0.1.0/build.py
--rw-r--r--   0      501       20      298 2023-05-29 13:18:22.000000 lana-0.1.0/examples/example.py
--rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.1.0/lana/__init__.py
--rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.1.0/pyproject.toml
--rw-r--r--   0      501       20     1392 2023-05-29 13:47:06.000000 lana-0.1.0/src/lib.rs
--rw-r--r--   0      501       20      441 2023-05-29 13:25:42.000000 lana-0.1.0/test/test_matrix.py
--rw-r--r--   0      501       20     7648 2023-05-29 12:53:33.000000 lana-0.1.0/Cargo.lock
--rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 lana-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.1.1/Cargo.toml
+-rw-r--r--   0      501       20      719 2023-05-29 14:30:05.000000 lana-0.1.1/.gitignore
+-rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.1/LICENSE
+-rw-r--r--   0      501       20      688 2023-05-29 14:29:13.000000 lana-0.1.1/README.md
+-rw-r--r--   0      501       20      161 2023-05-29 14:29:22.000000 lana-0.1.1/examples/example.py
+-rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.1.1/lana/__init__.py
+-rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.1.1/pyproject.toml
+-rw-r--r--   0      501       20      164 2023-05-29 14:28:02.000000 lana-0.1.1/src/lib.rs
+-rw-r--r--   0      501       20     1150 2023-05-29 14:28:30.000000 lana-0.1.1/src/matrix.rs
+-rw-r--r--   0      501       20      441 2023-05-29 13:25:42.000000 lana-0.1.1/test/test_matrix.py
+-rw-r--r--   0      501       20     7648 2023-05-29 14:28:18.000000 lana-0.1.1/Cargo.lock
+-rw-r--r--   0        0        0     1229 1970-01-01 00:00:00.000000 lana-0.1.1/PKG-INFO
```

### Comparing `lana-0.1.0/.gitignore` & `lana-0.1.1/.gitignore`

 * *Files 2% similar despite different names*

```diff
@@ -69,8 +69,10 @@
 .vscode/
 
 # Pyenv
 .python-version
 
 .env/
 target/
-.github/
+.github/
+
+build.py
```

### Comparing `lana-0.1.0/LICENSE` & `lana-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lana-0.1.0/README.md` & `lana-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,20 +20,18 @@
 ```
 
 ## Example 
 
 ```python
 from lana import Matrix
 
-print("# zeros #")
-mat = Matrix.zeros((3,3))
-print(mat)
-print(f"shape: {mat.shape}, type: {type(mat)}")
+zeros = Matrix.zeros((3,3))
+print(zeros)
+print(f"shape: {zeros.shape}, type: {type(zeros)}")
 
-print("# matrix #")
 mat = Matrix.matrix([[1,2,3],[4,5,6]])
 print(mat)
 print(f"shape: {mat.shape}, type: {type(mat)}")
 for rows in mat.data:
     print(rows, type(rows))
 ```
```

### Comparing `lana-0.1.0/pyproject.toml` & `lana-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lana-0.1.0/src/lib.rs` & `lana-0.1.1/src/matrix.rs`

 * *Files 7% similar despite different names*

```diff
@@ -41,26 +41,12 @@
     #[getter]
     pub fn shape(&self) -> (usize, usize) {
         let rows = self.data.len();
         let cols = self.data[0].len();
         (rows, cols)
     }
 
-    // pub fn print(&self) {
-    //     for row in self.data.iter() {
-    //         println!("{:?}", row);
-    //     }
-    // }
-
     fn __repr__(&self) -> PyResult<String> {
         Ok(format!("{:?}", self.data))
     }
 
-}
-
-
-
-#[pymodule]
-fn lana(_py: Python, m: &PyModule) -> PyResult<()> {
-    m.add_class::<Matrix>()?;
-    Ok(())
 }
```

### Comparing `lana-0.1.0/Cargo.lock` & `lana-0.1.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "lana"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.144"
```

### Comparing `lana-0.1.0/PKG-INFO` & `lana-0.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lana
-Version: 0.1.0
+Version: 0.1.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Linear Algebra experimental library
 Keywords: linear algebra
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
@@ -34,20 +34,18 @@
 ```
 
 ## Example 
 
 ```python
 from lana import Matrix
 
-print("# zeros #")
-mat = Matrix.zeros((3,3))
-print(mat)
-print(f"shape: {mat.shape}, type: {type(mat)}")
+zeros = Matrix.zeros((3,3))
+print(zeros)
+print(f"shape: {zeros.shape}, type: {type(zeros)}")
 
-print("# matrix #")
 mat = Matrix.matrix([[1,2,3],[4,5,6]])
 print(mat)
 print(f"shape: {mat.shape}, type: {type(mat)}")
 for rows in mat.data:
     print(rows, type(rows))
 ```
```


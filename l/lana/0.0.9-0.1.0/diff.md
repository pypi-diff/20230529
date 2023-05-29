# Comparing `tmp/lana-0.0.9.tar.gz` & `tmp/lana-0.1.0.tar.gz`

## Comparing `lana-0.0.9.tar` & `lana-0.1.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.0.9/Cargo.toml
--rw-r--r--   0      501       20      709 2023-05-15 16:30:29.000000 lana-0.0.9/.gitignore
--rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.0.9/LICENSE
--rw-r--r--   0      501       20      501 2023-05-29 10:26:22.000000 lana-0.0.9/README.md
--rw-r--r--   0      501       20      475 2023-05-29 10:54:53.000000 lana-0.0.9/build.py
--rw-r--r--   0      501       20      117 2023-05-29 10:23:44.000000 lana-0.0.9/examples/example.py
--rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.0.9/lana/__init__.py
--rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.0.9/pyproject.toml
--rw-r--r--   0      501       20      888 2023-05-29 10:44:24.000000 lana-0.0.9/src/lib.rs
--rw-r--r--   0      501       20     7648 2023-05-29 10:30:23.000000 lana-0.0.9/Cargo.lock
--rw-r--r--   0        0        0     1042 1970-01-01 00:00:00.000000 lana-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0      280 1970-01-01 00:00:00.000000 lana-0.1.0/Cargo.toml
+-rw-r--r--   0      501       20      709 2023-05-15 16:30:29.000000 lana-0.1.0/.gitignore
+-rw-r--r--   0      501       20     1060 2023-05-15 16:24:44.000000 lana-0.1.0/LICENSE
+-rw-r--r--   0      501       20      719 2023-05-29 13:17:37.000000 lana-0.1.0/README.md
+-rw-r--r--   0      501       20      475 2023-05-29 10:54:53.000000 lana-0.1.0/build.py
+-rw-r--r--   0      501       20      298 2023-05-29 13:18:22.000000 lana-0.1.0/examples/example.py
+-rw-r--r--   0      501       20       53 2023-05-29 09:44:26.000000 lana-0.1.0/lana/__init__.py
+-rw-r--r--   0      501       20      635 2023-05-15 19:10:53.000000 lana-0.1.0/pyproject.toml
+-rw-r--r--   0      501       20     1392 2023-05-29 13:47:06.000000 lana-0.1.0/src/lib.rs
+-rw-r--r--   0      501       20      441 2023-05-29 13:25:42.000000 lana-0.1.0/test/test_matrix.py
+-rw-r--r--   0      501       20     7648 2023-05-29 12:53:33.000000 lana-0.1.0/Cargo.lock
+-rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 lana-0.1.0/PKG-INFO
```

### Comparing `lana-0.0.9/.gitignore` & `lana-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lana-0.0.9/LICENSE` & `lana-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lana-0.0.9/pyproject.toml` & `lana-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lana-0.0.9/src/lib.rs` & `lana-0.1.0/src/lib.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 use pyo3::prelude::*;
 
 #[pyclass]
+#[derive(Debug)]
 pub struct Matrix {
     #[pyo3(get, set)]
     data: Vec<Vec<f64>>,
 }
 
 
 #[pymethods]
@@ -14,35 +15,52 @@
     pub fn zeros(dimensions: (usize, usize)) -> Self {
         let (rows, cols) = dimensions;
         let data: Vec<Vec<f64>> = vec![vec![0.0; cols]; rows];
         Matrix { data }
     }
 
     #[staticmethod]
+    pub fn ones(dimensions: (usize, usize)) -> Self {
+        let (rows, cols) = dimensions;
+        let data: Vec<Vec<f64>> = vec![vec![1.0; cols]; rows];
+        Matrix { data }
+    }
+
+    #[staticmethod]
+    pub fn eye(size: usize) -> Self {
+        let data: Vec<Vec<f64>> = (0..size).map(|i| {
+            (0..size).map(|j| if i==j {1.0} else {0.0}).collect()
+        }).collect();
+        Matrix { data }
+    }
+
+    #[staticmethod]
     pub fn matrix(data: Vec<Vec<f64>>) -> Self {
         Matrix { data } 
     }
 
     #[getter]
     pub fn shape(&self) -> (usize, usize) {
         let rows = self.data.len();
         let cols = self.data[0].len();
         (rows, cols)
     }
 
-    pub fn print(&self) {
-        for row in &self.data {
-            for i in row {
-                print!("{} ", i);
-            }
-            println!();
-        }
+    // pub fn print(&self) {
+    //     for row in self.data.iter() {
+    //         println!("{:?}", row);
+    //     }
+    // }
+
+    fn __repr__(&self) -> PyResult<String> {
+        Ok(format!("{:?}", self.data))
     }
 
 }
 
 
+
 #[pymodule]
 fn lana(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add_class::<Matrix>()?;
     Ok(())
 }
```

### Comparing `lana-0.0.9/Cargo.lock` & `lana-0.1.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 name = "indoc"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "lana"
-version = "0.0.9"
+version = "0.1.0"
 dependencies = [
  "pyo3",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.144"
```

### Comparing `lana-0.0.9/PKG-INFO` & `lana-0.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lana
-Version: 0.0.9
+Version: 0.1.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Linear Algebra experimental library
 Keywords: linear algebra
 Author-email: Marco Salvalaggio <mar.salvalaggio@gmail.com>
@@ -34,13 +34,21 @@
 ```
 
 ## Example 
 
 ```python
 from lana import Matrix
 
+print("# zeros #")
 mat = Matrix.zeros((3,3))
-mat.print()
-print(mat.shape)
+print(mat)
+print(f"shape: {mat.shape}, type: {type(mat)}")
+
+print("# matrix #")
+mat = Matrix.matrix([[1,2,3],[4,5,6]])
+print(mat)
+print(f"shape: {mat.shape}, type: {type(mat)}")
+for rows in mat.data:
+    print(rows, type(rows))
 ```
```


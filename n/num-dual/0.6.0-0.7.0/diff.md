# Comparing `tmp/num_dual-0.6.0-cp37-abi3-win_amd64.whl.zip` & `tmp/num_dual-0.7.0-cp37-abi3-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 1851284 bytes, number of entries: 5
--rw-r--r--  4.6 unx     4747 b- defN 23-Jan-20 18:51 num_dual-0.6.0.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jan-20 18:51 num_dual-0.6.0.dist-info/WHEEL
--rw-r--r--  4.6 unx      115 b- defN 23-Jan-20 18:51 num_dual/__init__.py
--rwxr-xr-x  4.6 unx  7894016 b- defN 23-Jan-20 18:51 num_dual/num_dual.pyd
--rw-r--r--  4.6 unx      366 b- defN 23-Jan-20 18:51 num_dual-0.6.0.dist-info/RECORD
-5 files, 7899340 bytes uncompressed, 1850612 bytes compressed:  76.6%
+Zip file size: 2809603 bytes, number of entries: 5
+-rw-r--r--  4.6 unx     4762 b- defN 23-May-29 09:58 num_dual-0.7.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-May-29 09:58 num_dual-0.7.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx      115 b- defN 23-May-29 09:58 num_dual/__init__.py
+-rwxr-xr-x  4.6 unx  9679360 b- defN 23-May-29 09:58 num_dual/num_dual.pyd
+-rw-r--r--  4.6 unx      366 b- defN 23-May-29 09:58 num_dual-0.7.0.dist-info/RECORD
+5 files, 9684698 bytes uncompressed, 2808931 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
-Filename: num_dual-0.6.0.dist-info/METADATA
+Filename: num_dual-0.7.0.dist-info/METADATA
 Comment: 
 
-Filename: num_dual-0.6.0.dist-info/WHEEL
+Filename: num_dual-0.7.0.dist-info/WHEEL
 Comment: 
 
 Filename: num_dual/__init__.py
 Comment: 
 
 Filename: num_dual/num_dual.pyd
 Comment: 
 
-Filename: num_dual-0.6.0.dist-info/RECORD
+Filename: num_dual-0.7.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `num_dual-0.6.0.dist-info/METADATA` & `num_dual-0.7.0.dist-info/METADATA`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: num_dual
-Version: 0.6.0
+Name: num-dual
+Version: 0.7.0
 Summary: Generalized (hyper) dual numbers for the calculation of exact (partial) derivatives
 Keywords: mathematics,numerics,differentiation
 Home-Page: https://github.com/itt-ustutt/num-dual
 Author: Gernot Bauer <bauer@itt.uni-stuttgart.de>, Philipp Rehner <prehner@ethz.ch>
 Author-email: Gernot Bauer <bauer@itt.uni-stuttgart.de>, Philipp Rehner <prehner@ethz.ch>
 License: MIT OR Apache-2.0
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
@@ -37,59 +37,68 @@
 
 ### Rust
 
 Add this to your `Cargo.toml`:
 
 ```toml
 [dependencies]
-num-dual = "0.6"
+num-dual = "0.7"
 ```
 
 ## Example
 
 ### Python
 
 Compute the first and second derivative of a scalar-valued function.
 
 ```python
-from num_dual import derive2
+from num_dual import second_derivative
 import numpy as np
 
 def f(x):
     return np.exp(x) / np.sqrt(np.sin(x)**3 + np.cos(x)**3)
 
-x = derive2(1.5)
-result = f(x)
-print('f(x)    = {}'.format(result.value))
-print('df/dx   = {}'.format(result.first_derivative))
-print('d2f/dx2 = {}'.format(result.second_derivative))
+f, df, d2f = second_derivative(f, 1.5)
+
+print(f'f(x)    = {f}')
+print(f'df/dx   = {df}')
+print(f'd2f/dx2 = {d2f}')
 ```
 
 ### Rust
 This example defines a generic function that can be called using any (hyper) dual number and automatically calculates derivatives.
 ```rust
 use num_dual::*;
+
 fn f<D: DualNum<f64>>(x: D, y: D) -> D {
     x.powi(3) * y.powi(2)
 }
+
 fn main() {
     let (x, y) = (5.0, 4.0);
-    // Calculate a simple derivative
-    let x_dual = Dual64::from(x).derive();
+    // Calculate a simple derivative using dual numbers
+    let x_dual = Dual64::from(x).derivative();
     let y_dual = Dual64::from(y);
-    println!("{}", f(x_dual, y_dual));                      // 2000 + [1200]ε
+    println!("{}", f(x_dual, y_dual)); // 2000 + [1200]ε
+
+    // or use the provided function instead
+    let (_, df) = first_derivative(|x| f(x, y.into()), x);
+    println!("{df}"); // 1200
+
     // Calculate a gradient
-    let xy_dual_vec = StaticVec::new_vec([x,y]).map(DualVec64::<2>::from).derive();
-    println!("{}", f(xy_dual_vec[0], xy_dual_vec[1]).eps);  // [1200, 1000]
+    let (value, grad) = gradient(|v| f(v[0], v[1]), SMatrix::from([x, y]));
+    println!("{value} {grad}"); // 2000 [1200, 1000]
+
     // Calculate a Hessian
-    let xy_dual2 = StaticVec::new_vec([x,y]).map(Dual2Vec64::<2>::from).derive();
-    println!("{}", f(xy_dual2[0], xy_dual2[1]).v2);         // [[480, 600], [600, 250]]
+    let (_, _, hess) = hessian(|v| f(v[0], v[1]), SMatrix::from([x, y]));
+    println!("{hess}"); // [[480, 600], [600, 250]]
+
     // for x=cos(t) and y=sin(t) calculate the third derivative w.r.t. t
-    let t = Dual3_64::from(1.0).derive();
-    println!("{}", f(t.cos(), t.sin()).v3);                 // 7.358639755305733
+    let (_, _, _, d3f) = third_derivative(|t| f(t.cos(), t.sin()), 1.0);
+    println!("{d3f}"); // 7.358639755305733
 }
 ```
 
 ## Documentation
 
 - You can find the documentation of the rust crate [here](https://docs.rs/num-dual/).
 - The documentation of the python package can be found [here](https://itt-ustutt.github.io/num-dual/).
@@ -104,15 +113,15 @@
 ```
 Open `_build/html/index.html` in your browser.
 
 ## Further reading
 
 If you want to learn more about the topic of dual numbers and automatic differentiation, we have listed some useful resources for you here:
 
-- Initial paper about hyper-dual numbers: [Fike, J. and Alonso, 2011](https://arc.aiaa.org/doi/abs/10.2514/6.2011-886)
+- Initial paper about hyper-dual numbers: [Fike, J. and Alonso, J., 2011](https://arc.aiaa.org/doi/abs/10.2514/6.2011-886)
 - Website about all topics regarding automatic differentiation: [autodiff.org](http://www.autodiff.org/)
 - Our paper about dual numbers in equation of state modeling: [Rehner, P. and Bauer, G., 2021](https://www.frontiersin.org/article/10.3389/fceng.2021.758090)
 
 ## Cite us
 
 If you find `num-dual` useful for your own scientific studies, consider [citing our publication](https://www.frontiersin.org/article/10.3389/fceng.2021.758090) accompanying this library.
```


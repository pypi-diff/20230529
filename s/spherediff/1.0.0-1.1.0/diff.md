# Comparing `tmp/spherediff-1.0.0.tar.gz` & `tmp/spherediff-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spherediff-1.0.0.tar", last modified: Mon May 22 22:12:47 2023, max compression
+gzip compressed data, was "/home/kormos/spherediff/dist/.tmp-oulq8aci/spherediff-1.1.0.tar", last modified: Mon May 29 03:17:34 2023, max compression
```

## Comparing `spherediff-1.0.0.tar` & `spherediff-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-22 22:12:47.932046 spherediff-1.0.0/
--rw-r--r--   0 kormos    (1000) kormos    (1000)     1068 2023-05-22 22:12:37.000000 spherediff-1.0.0/LICENSE.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)     2906 2023-05-22 22:12:47.932046 spherediff-1.0.0/PKG-INFO
--rw-r--r--   0 kormos    (1000) kormos    (1000)     2410 2023-05-22 22:06:10.000000 spherediff-1.0.0/README.md
--rw-r--r--   0 kormos    (1000) kormos    (1000)      766 2023-05-22 22:00:57.000000 spherediff-1.0.0/pyproject.toml
--rw-r--r--   0 kormos    (1000) kormos    (1000)       38 2023-05-22 22:12:47.932046 spherediff-1.0.0/setup.cfg
--rw-r--r--   0 kormos    (1000) kormos    (1000)       50 2023-05-22 21:59:35.000000 spherediff-1.0.0/setup.py
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-22 22:12:47.922046 spherediff-1.0.0/src/
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-22 22:12:47.922046 spherediff-1.0.0/src/spherediff/
--rw-r--r--   0 kormos    (1000) kormos    (1000)        0 2023-05-08 23:09:07.000000 spherediff-1.0.0/src/spherediff/__init__.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     3450 2023-05-22 04:24:15.000000 spherediff-1.0.0/src/spherediff/coeffs.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     7195 2023-05-22 04:48:54.000000 spherediff-1.0.0/src/spherediff/kernel.py
--rwxr-xr-x   0 kormos    (1000) kormos    (1000)     1841 2023-05-22 04:24:19.000000 spherediff-1.0.0/src/spherediff/poly.py
--rw-r--r--   0 kormos    (1000) kormos    (1000)     2333 2023-05-22 05:54:25.000000 spherediff-1.0.0/src/spherediff/sample.py
-drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-22 22:12:47.932046 spherediff-1.0.0/src/spherediff.egg-info/
--rw-r--r--   0 kormos    (1000) kormos    (1000)     2906 2023-05-22 22:12:47.000000 spherediff-1.0.0/src/spherediff.egg-info/PKG-INFO
--rw-r--r--   0 kormos    (1000) kormos    (1000)      359 2023-05-22 22:12:47.000000 spherediff-1.0.0/src/spherediff.egg-info/SOURCES.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)        1 2023-05-22 22:12:47.000000 spherediff-1.0.0/src/spherediff.egg-info/dependency_links.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)       75 2023-05-22 22:12:47.000000 spherediff-1.0.0/src/spherediff.egg-info/requires.txt
--rw-r--r--   0 kormos    (1000) kormos    (1000)       11 2023-05-22 22:12:47.000000 spherediff-1.0.0/src/spherediff.egg-info/top_level.txt
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-29 03:17:34.875851 spherediff-1.1.0/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     1068 2023-05-22 22:12:37.000000 spherediff-1.1.0/LICENSE.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     2906 2023-05-29 03:17:34.875851 spherediff-1.1.0/PKG-INFO
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     2410 2023-05-22 22:06:10.000000 spherediff-1.1.0/README.md
+-rw-r--r--   0 kormos    (1000) kormos    (1000)      766 2023-05-29 03:16:18.000000 spherediff-1.1.0/pyproject.toml
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       38 2023-05-29 03:17:34.875851 spherediff-1.1.0/setup.cfg
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       50 2023-05-22 21:59:35.000000 spherediff-1.1.0/setup.py
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-29 03:17:34.875851 spherediff-1.1.0/src/
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-29 03:17:34.875851 spherediff-1.1.0/src/spherediff/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)        0 2023-05-08 23:09:07.000000 spherediff-1.1.0/src/spherediff/__init__.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     8087 2023-05-29 03:14:23.000000 spherediff-1.1.0/src/spherediff/coeffs.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)    11141 2023-05-29 03:14:23.000000 spherediff-1.1.0/src/spherediff/kernel.py
+-rwxr-xr-x   0 kormos    (1000) kormos    (1000)     4459 2023-05-29 03:14:23.000000 spherediff-1.1.0/src/spherediff/poly.py
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     2333 2023-05-22 05:54:25.000000 spherediff-1.1.0/src/spherediff/sample.py
+drwxr-xr-x   0 kormos    (1000) kormos    (1000)        0 2023-05-29 03:17:34.875851 spherediff-1.1.0/src/spherediff.egg-info/
+-rw-r--r--   0 kormos    (1000) kormos    (1000)     2906 2023-05-29 03:17:34.000000 spherediff-1.1.0/src/spherediff.egg-info/PKG-INFO
+-rw-r--r--   0 kormos    (1000) kormos    (1000)      359 2023-05-29 03:17:34.000000 spherediff-1.1.0/src/spherediff.egg-info/SOURCES.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)        1 2023-05-29 03:17:34.000000 spherediff-1.1.0/src/spherediff.egg-info/dependency_links.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       75 2023-05-29 03:17:34.000000 spherediff-1.1.0/src/spherediff.egg-info/requires.txt
+-rw-r--r--   0 kormos    (1000) kormos    (1000)       11 2023-05-29 03:17:34.000000 spherediff-1.1.0/src/spherediff.egg-info/top_level.txt
```

### Comparing `spherediff-1.0.0/LICENSE.txt` & `spherediff-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spherediff-1.0.0/PKG-INFO` & `spherediff-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherediff
-Version: 1.0.0
+Version: 1.1.0
 Summary: Sample from the diffusion kernel on any n-sphere
 Author-email: Rian Kormos <Rian.Kormos@ucsf.edu>
 Project-URL: Homepage, https://github.com/rckormos/SphereDiff
 Keywords: diffusion,hypersphere,sampling
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `spherediff-1.0.0/README.md` & `spherediff-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `spherediff-1.0.0/pyproject.toml` & `spherediff-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "spherediff"
-version = "1.0.0"
+version = "1.1.0"
 description = "Sample from the diffusion kernel on any n-sphere"
 readme = "README.md"
 authors = [{name = "Rian Kormos", email = "Rian.Kormos@ucsf.edu"}]
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License", 
     "Programming Language :: Python",
```

### Comparing `spherediff-1.0.0/src/spherediff/kernel.py` & `spherediff-1.1.0/src/spherediff/kernel.py`

 * *Files 22% similar despite different names*

```diff
@@ -68,18 +68,22 @@
         cdf += dcdf
         if np.abs(dpdf).max() < 1e-14 and np.abs(dcdf).max() < 1e-14:
             converged = True
         else:
             converged = False
         # update coeffs_l and coeffs_lp1 
         coeffs_lp2 = np.empty(len(coeffs_lp1) + 1)
+        prefactor = 2. ** ((n + 1) % 2)
         factor1 = (2 * l + n) / (2 * l + 4)
         factor2 = (l + n - 2) / (l + 2)
         coeffs_lp2[0] = factor1 * coeffs_lp1[1] - factor2 * coeffs_l[0]
-        for k in range(1, len(coeffs_lp2) - 2):
+        coeffs_lp2[1] = \
+            factor1 * (coeffs_lp1[2] + prefactor * coeffs_lp1[0]) - \
+            factor2 * coeffs_l[1]
+        for k in range(2, len(coeffs_lp2) - 2):
             coeffs_lp2[k] = \
                 factor1 * (coeffs_lp1[k + 1] + coeffs_lp1[k - 1]) - \
                 factor2 * coeffs_l[k]
         coeffs_lp2[-1] = factor1 * coeffs_lp1[-1]
         coeffs_lp2[-2] = factor1 * coeffs_lp1[-2]
         coeffs_l = coeffs_lp1
         coeffs_lp1 = coeffs_lp2
@@ -152,18 +156,22 @@
         mean += dmean
         if np.abs(dmean).max() < 1e-14:
             converged = True
         else:
             converged = False
         # update coeffs_l and coeffs_lp1 
         coeffs_lp2 = np.empty(len(coeffs_lp1) + 1)
+        prefactor = 2. ** ((n + 1) // 2)
         factor1 = (2 * l + n) / (2 * l + 4)
         factor2 = (l + n - 2) / (l + 2)
         coeffs_lp2[0] = factor1 * coeffs_lp1[1] - factor2 * coeffs_l[0]
-        for k in range(1, len(coeffs_lp2) - 2):
+        coeffs_lp2[1] = \
+            factor1 * (coeffs_lp1[2] + prefactor * coeffs_lp1[0]) - \
+            factor2 * coeffs_l[1]
+        for k in range(2, len(coeffs_lp2) - 2):
             coeffs_lp2[k] = \
                 factor1 * (coeffs_lp1[k + 1] + coeffs_lp1[k - 1]) - \
                 factor2 * coeffs_l[k]
         coeffs_lp2[-1] = factor1 * coeffs_lp1[-1]
         coeffs_lp2[-2] = factor1 * coeffs_lp1[-2]
         coeffs_l = coeffs_lp1
         coeffs_lp1 = coeffs_lp2
@@ -172,7 +180,95 @@
             (2 * l + n) / (l + 2) * gegenbauer_lp1_1 - \
             (l + n - 2) / (l + 2) * gegenbauer_l_1, \
             gegenbauer_lp1_1
         # update l and the squared normalization coefficient
         l += 1
         norm_square *= 2 * l / (2 * l + 2 * n - 6)
     return mean
+
+@nb.jit(nopython=True, cache=True)
+def raw_kernel(n, var, phi):
+    """Compute and differentiate the raw diffusion kernel on the (n-1)D sphere.
+
+       This kernel is a function of phi_{n-1}, the final polar angle in the 
+       hyperspherical coordinates of a sphere embedded in nD space. The 
+       volume element, sin^{n-2}(phi_{n-1}) is not included, hence the 
+       designation of the kernel as raw.
+
+    Parameters
+    ----------
+    n : int
+        The dimensionality of the space in which the spherical surface is 
+        embedded.
+    var : np.array [N]
+        Array of variance parameters for which to compute the raw diffusion 
+        kernel and its derivative at each angle phi.
+    phi : np.array [N]
+        Array of angles (in radians) at which to compute the raw diffusion 
+        kernel and its derivative.
+
+    Returns
+    -------
+    kernel : np.array [N]
+        The raw diffusion kernel on the (n-1)D sphere, evaluated at each 
+        angle phi.
+    kernel_deriv : np.array [N]
+        The derivative of the raw diffusion kernel on the (n-1)D sphere, 
+        evaluated at each angle phi.
+    """
+    norm_square = (2. / np.pi) ** (int(n - 3) % 2) * \
+                  2 ** (n - 3)
+    for j in range(n - 4, 0, -2):
+        norm_square *= j ** 2
+    for j in range(2 * n - 6, 0, -2):
+        norm_square /= j
+    kernel, kernel_deriv = np.zeros_like(phi), np.zeros_like(phi)
+    gegenbauer_l_1 = 1. # lth Gegenbauer polynomial evaluated at 1
+    gegenbauer_lp1_1 = n - 2 # l+1th Gegenbauer polynomial evaluated at 1
+    coeffs_l = np.array([1.])
+    coeffs_lp1 = np.array([0., n - 2])
+    converged, prev_converged = False, False
+    l = 0
+    while not (converged and prev_converged):
+        prev_converged = converged
+        dker, dker_deriv = np.zeros_like(phi), np.zeros_like(phi)
+        for k, coeff in enumerate(coeffs_l):
+            if not coeff:
+                continue
+            dker += coeff * np.cos(k * phi)
+            dker_deriv -= coeff * k * np.sin(k * phi)
+        exp_factor = np.exp(-0.5 * l * (l + n - 2) * var)
+        dker *= 0.5 * (2 * l + n - 2) * \
+                gegenbauer_l_1 * norm_square * exp_factor
+        dker_deriv *= 0.5 * (2 * l + n - 2) * \
+                      gegenbauer_l_1 * norm_square * exp_factor
+        kernel += dker
+        kernel_deriv += dker_deriv
+        if np.abs(dker).max() < 1e-14 and np.abs(dker_deriv).max() < 1e-14:
+            converged = True
+        else:
+            converged = False
+        # update coeffs_l and coeffs_lp1
+        coeffs_lp2 = np.empty(len(coeffs_lp1) + 1)
+        factor1 = (2 * l + n) / (2 * l + 4)
+        factor2 = (l + n - 2) / (l + 2)
+        coeffs_lp2[0] = factor1 * coeffs_lp1[1] - factor2 * coeffs_l[0]
+        coeffs_lp2[1] = \
+            factor1 * (coeffs_lp1[2] + 2. * coeffs_lp1[0]) - \
+            factor2 * coeffs_l[1]
+        for k in range(2, len(coeffs_lp2) - 2):
+            coeffs_lp2[k] = \
+                factor1 * (coeffs_lp1[k + 1] + coeffs_lp1[k - 1]) - \
+                factor2 * coeffs_l[k]
+        coeffs_lp2[-1] = factor1 * coeffs_lp1[-1]
+        coeffs_lp2[-2] = factor1 * coeffs_lp1[-2]
+        coeffs_l = coeffs_lp1
+        coeffs_lp1 = coeffs_lp2
+        # update gegenbauer_l_1 and gegenbauer_lp1_1
+        gegenbauer_lp1_1, gegenbauer_l_1 = \
+            (2 * l + n) / (l + 2) * gegenbauer_lp1_1 - \
+            (l + n - 2) / (l + 2) * gegenbauer_l_1, \
+            gegenbauer_lp1_1
+        # update l and the squared normalization coefficient
+        l += 1
+        norm_square *= 2 * l / (2 * l + 2 * n - 6)
+    return kernel, kernel_deriv
```

### Comparing `spherediff-1.0.0/src/spherediff/sample.py` & `spherediff-1.1.0/src/spherediff/sample.py`

 * *Files identical despite different names*

### Comparing `spherediff-1.0.0/src/spherediff.egg-info/PKG-INFO` & `spherediff-1.1.0/src/spherediff.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spherediff
-Version: 1.0.0
+Version: 1.1.0
 Summary: Sample from the diffusion kernel on any n-sphere
 Author-email: Rian Kormos <Rian.Kormos@ucsf.edu>
 Project-URL: Homepage, https://github.com/rckormos/SphereDiff
 Keywords: diffusion,hypersphere,sampling
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```


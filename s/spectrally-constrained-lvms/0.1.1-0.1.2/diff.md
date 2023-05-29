# Comparing `tmp/spectrally_constrained_lvms-0.1.1.tar.gz` & `tmp/spectrally_constrained_lvms-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrally_constrained_lvms-0.1.1.tar", max compression
+gzip compressed data, was "spectrally_constrained_lvms-0.1.2.tar", max compression
```

## Comparing `spectrally_constrained_lvms-0.1.1.tar` & `spectrally_constrained_lvms-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_constrained_lvms-0.1.1/LICENSE
--rw-r--r--   0        0        0     1777 2023-05-16 07:40:02.665593 spectrally_constrained_lvms-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1289 2023-05-13 20:02:18.006810 spectrally_constrained_lvms-0.1.1/README.md
--rw-r--r--   0        0        0     1212 2023-05-16 07:40:02.681793 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/__init__.py
--rw-r--r--   0        0        0    16084 2023-05-15 13:23:10.954638 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/cost_functions.py
--rw-r--r--   0        0        0    21547 2023-05-13 15:56:12.827004 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/helper_methods.py
--rw-r--r--   0        0        0    15121 2023-05-13 15:42:49.428404 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/negen_approx.py
--rw-r--r--   0        0        0    16446 2023-05-13 15:41:10.612996 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/spectral_constraint.py
--rw-r--r--   0        0        0    31979 2023-05-16 07:15:18.150362 spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/spectrally_constrained_model.py
--rw-r--r--   0        0        0     2635 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_constrained_lvms-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1747 2023-05-29 10:56:50.260003 spectrally_constrained_lvms-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     6955 2023-05-29 10:57:01.810232 spectrally_constrained_lvms-0.1.2/README.md
+-rw-r--r--   0        0        0     1184 2023-05-29 10:56:50.271514 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/__init__.py
+-rw-r--r--   0        0        0    32742 2023-05-26 12:13:55.514135 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/cost_functions.py
+-rw-r--r--   0        0        0    21405 2023-05-26 12:13:55.515128 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/helper_methods.py
+-rw-r--r--   0        0        0    13584 2023-05-26 12:13:55.515631 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/negen_approx.py
+-rw-r--r--   0        0        0    16775 2023-05-26 12:13:55.517156 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/spectral_constraint.py
+-rw-r--r--   0        0        0    52550 2023-05-26 12:13:55.518215 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/spectrally_constrained_model.py
+-rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.2/PKG-INFO
```

### Comparing `spectrally_constrained_lvms-0.1.1/LICENSE` & `spectrally_constrained_lvms-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.1/pyproject.toml` & `spectrally_constrained_lvms-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrally-constrained-LVMs"
-version = "0.1.1"
+version = "0.1.2"
 description = "An optimisation implementation of linear transforms with a spectral constraint."
 authors = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 maintainers = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/RyanBalshaw/spectrally-constrained-LVMs"
 repository = "https://github.com/RyanBalshaw/spectrally-constrained-LVMs"
@@ -30,18 +30,18 @@
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
 black = "^23.3.0"
 isort = "^5.12.0"
-interrogate = {extras = ["png"], version = "^1.5.0"}
 pytest = "^7.3.1"
 ruff = "^0.0.263"
 jupyterlab = "^3.6.3"
+interrogate = "^1.5.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 myst-parser = ">=0.16"
 sphinx = ">=4.0"
```

### Comparing `spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/__init__.py` & `spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 # Copyright 2023-present Ryan Balshaw
 """Spectrally-constrained-LVMs. Train linear LVMs with the addition
  of a spectral constraint with minimal effort."""
-from .cost_functions import negentropy_cost, sympy_cost, user_cost, variance_cost
+from .cost_functions import NegentropyCost, SympyCost, UserCost, VarianceCost
 from .helper_methods import (
-    Hankel_matrix,
-    batch_sampler,
-    data_processor,
-    deflation_orthogonalisation,
-    quasi_Newton,
+    BatchSampler,
+    DataProcessor,
+    DeflationOrthogonalisation,
+    QuasiNewton,
+    hankel_matrix,
 )
-from .negen_approx import cube_object, exp_object, logcosh_object, quad_object
-from .spectral_constraint import spectral_objective
-from .spectrally_constrained_model import linear_model
+from .negen_approx import CubeObject, ExpObject, LogcoshObject, QuadObject
+from .spectral_constraint import SpectralObjective
+from .spectrally_constrained_model import LinearModel
 
 __author__ = "Ryan Balshaw"
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __email__ = "ryanbalshaw81@gmail.com"
 __description__ = (
     "Train linear LVMs with the addition "
     "of a spectral constraint with minimal effort."
 )
 # __uri__ = "http://spectrally-constrained-lvms.readthedocs.io/"
 __all__ = [
-    "spectral_objective",
-    "negentropy_cost",
-    "sympy_cost",
-    "user_cost",
-    "variance_cost",
-    "Hankel_matrix",
-    "batch_sampler",
-    "data_processor",
-    "deflation_orthogonalisation",
-    "quasi_Newton",
-    "cube_object",
-    "exp_object",
-    "logcosh_object",
-    "quad_object",
-    "linear_model",
+    "SpectralObjective",
+    "NegentropyCost",
+    "SympyCost",
+    "UserCost",
+    "VarianceCost",
+    "hankel_matrix",
+    "LinearModel",
+    "BatchSampler",
+    "DataProcessor",
+    "DeflationOrthogonalisation",
+    "QuasiNewton",
+    "CubeObject",
+    "ExpObject",
+    "LogcoshObject",
+    "QuadObject",
 ]
```

### Comparing `spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/helper_methods.py` & `spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/helper_methods.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,34 +20,33 @@
 """
 
 import copy
 
 import numpy as np
 
 
-class data_processor(object):
+class DataProcessor(object):
     """
     A method that processes the data matrices.
 
     Methods
     -------
     initialise_preprocessing(X)
-        A method that initialises all of the processing attributes
+        A method that initialises all the processing attributes
         for the pre-processing (standardising with whitening). Solves
         for the whitening transform parameters.
 
     standardise_data(X)
         Standardises the columns of X to be zero-mean and unit-variance.
 
     preprocess_data(X)
         Transforms the X matrix to the whitened space (if required).
 
     unprocess_data(X)
-        Transforms a X matrix from the whitened space to the data space.
-
+        Transforms an X matrix from the whitened space to the data space.
     """
 
     def __init__(self, whiten: bool = True, var_PCA: float | None = None):
         """
         Parameters
         ----------
         whiten: bool
@@ -124,15 +123,15 @@
     def standardise_data(self, X):
         """
         A method that standardises the row of the data matrix X
 
         Parameters
         ----------
         X: ndarray
-            original feature matrix
+            The original feature matrix X.
 
         Returns
         -------
         X_standardised: ndarray
             Zero-mean, unit variance feature matrix.
         """
 
@@ -143,49 +142,49 @@
     def preprocess_data(self, X):
         """
         A method that pre-processes the data matrix X
 
         Parameters
         ----------
         X: ndarray
-            original feature matrix
+            The original feature matrix X.
 
         Returns
         -------
         X_whitened: ndarray
-            The whitened feature matrix
+            The whitened feature matrix.
         """
         X_standardised = self.standardise_data(X)
 
         X_whitened = (X_standardised @ self.latent_transform.T) @ self.Vh
         # X_whitened = np.dot(X_standardised, self.latent_transform.T)
 
         return X_whitened
 
     def unprocess_data(self, X):
         """
-        A method that unwhitens the whitened data matrix X
+        A method that un-whitens the whitened data matrix X
 
         Parameters
         ----------
         X: ndarray
             The whitened feature matrix
 
         Returns
         -------
         X_unwhitened: ndarray
-            The unwhitened feature matrix
+            The un-whitened feature matrix
         """
         X_unwhitened = np.dot(np.dot(X, self.recover_transform.T), self.Vh)
         # X_unwhitened = np.dot(X, self.recover_transform.T)
 
         return X_unwhitened
 
 
-class batch_sampler(object):
+class BatchSampler(object):
     """
     This is a simple iterator instance that can be called during runtime using:
 
     batch_sampler_inst = batch_sampler(batch_size, include_end=True)
     data_sampler = iter(batch_sampler_inst(X_preprocess, iter_idx=0))
 
     and then sampling in a loop or something like that:
@@ -195,15 +194,15 @@
     """
 
     def __init__(self, batch_size, random_sampler=True, include_end=False):
         """
         Parameters
         ----------
         batch_size: int
-            The batch size used by the sampler.
+                The batch size used by the sampler.
 
         random_sampler: bool
             A flag to specify whether the sampler runs by randomly selecting indices
             from the data (random_sampler=True) or if it loops through
             the data in sequence.
 
         include_end: bool
@@ -270,15 +269,15 @@
 
             self._max_iter = len(self._iter_range) - 1
 
         return self
 
     def __iter__(self):
         """
-        Initalises the iteration counter when iter() is applied to the sampler
+        Initialises the iteration counter when iter() is applied to the sampler
         instance.
 
         Returns
         -------
         self
         """
         self._iter_cnt = 0
@@ -312,15 +311,15 @@
 
         """
         if self._iter_cnt < self._max_iter:
             pass
 
         else:
             self._iter_cnt = 0
-            # raise StopIteration # I am breaking many Python laws.
+        # raise StopIteration # I am breaking many Python laws.
 
         # This code should be in the if statement
         if not self.random_sampler:
             idx_l = self._iter_range[self._iter_cnt]
             idx_u = self._iter_range[self._iter_cnt + 1]
             data_batch = np.take(
                 self._data, range(idx_l, idx_u, 1), axis=self._iter_idx
@@ -334,15 +333,15 @@
             )
 
         self._iter_cnt += 1
 
         return data_batch
 
 
-class quasi_Newton(object):
+class QuasiNewton(object):
     """
     This method implements different Hessian approximation strategies and
     performs the updates on each call.
 
     The included quasi-Newton methods are:
     - Symmetric rank one (SR1)
     - Davidson Fletcher Powell (DFP)
@@ -439,15 +438,15 @@
             I_mat = np.eye(grad_diff_k.shape[0])
 
             t1 = I_mat - grad_diff_k @ delta_params_k.T * gamma_k
             t2 = I_mat - delta_params_k @ grad_diff_k.T * gamma_k
             t3 = grad_diff_k @ grad_diff_k.T * gamma_k
 
             update_term = (
-                (t1) @ self.jacobian_mat_iter @ (t2) + t3 - self.jacobian_mat_iter
+                t1 @ self.jacobian_mat_iter @ t2 + t3 - self.jacobian_mat_iter
             )  # subtract to fix update rule below
 
         return update_term
 
     def boyden_fletcher_goldfarb_shanno(self, delta_params_k, grad_diff_k):
         """
         The BFGS update step
@@ -492,41 +491,30 @@
                 @ self.jacobian_mat_iter.T
             ) / (delta_params_k.T @ self.jacobian_mat_iter @ delta_params_k)
 
             update_term = t1 - t2
 
         return update_term
 
-    def initialise_jacobian(self, m):
+    def initialise_jacobian(self, n_features):
         """
         A method that initialises the Jacobian matrix.
         Assumes that
 
         Parameters
         ----------
-        m: int
+        n_features: int
             The dimensionality of the feature space.
 
-        Initialises
         -----------
         self.jacobian_mat_iter: ndarray
             The Hessian used during iteration.
         """
-        if self.use_inverse:
-            if self.jacobian_update_type == "bfgs":
-                self.jacobian_mat_iter = np.eye(m)
 
-            else:
-                self.jacobian_mat_iter = 0.1 * np.eye(m)
-        else:
-            if self.jacobian_update_type == "bfgs":
-                self.jacobian_mat_iter = np.eye(m)
-
-            else:
-                self.jacobian_mat_iter = 10 * np.eye(m)
+        self.jacobian_mat_iter = np.eye(n_features)
 
     def compute_update(self, gradient_vector):
         """
         A method used to compute the parameter update
         based on the gradient vector at time t.
 
         Parameters
@@ -577,29 +565,30 @@
             print(f"Update type ({self.jacobian_update_type}) not understood.")
             raise SystemExit
 
         self.jacobian_mat_iter += update_term
         self.iter_index += 1
 
 
-class deflation_orthogonalisation(object):
+class DeflationOrthogonalisation(object):
     """
     This method implements the Gram-Schmidt orthogonalisation
     process and some helper methods.
 
     Methods
     -------
     projection_operator(u, v)
-        words
+        This method computes the projection operator of v onto u.
 
     gram_schmidt_orthogonalisation(w, W, idx)
-        words
+        This method performs GS orthogonalisation. of w w.r.t the vectors in W up
+        to the W position.
 
     global_gso(W)
-        words
+        This method performs GSO sequentially for the rows in W.
 
     """
 
     @staticmethod
     def projection_operator(u, v):
         """
         Calculates projection of v onto u (equivalent to outer product map).
@@ -625,15 +614,16 @@
 
         Parameters
         ----------
         w: ndarray
             A Nx1 array that contains the vector we want to orthogonalise.
 
         W: ndarray
-            A MxN array that contains the vectors we want to orthogonalise w against.
+            A MxN array that contains the vectors we want to orthogonalise
+            w against.
 
         idx: int
             The upper index (cannot be zero) for the rows of W that
             we want to orthogonalise against.
 
         Returns
         -------
@@ -695,15 +685,15 @@
         # Iterate over the other vectors and orthogonalise against them
         for i in range(1, W.shape[0], 1):
             W_orth[i, :] = self.gram_schmidt_orthogonalisation(W[[i], :].T, W, i)[:, 0]
 
         return W_orth
 
 
-def Hankel_matrix(signal, Lw=512, Lsft=1):
+def hankel_matrix(signal, Lw=512, Lsft=1):
     """
     A method that performs hankelisation for the user.
 
     Parameters
     ----------
     signal: ndarray
         A (n,) shaped array that contains a time series of measurement values
```

### Comparing `spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/negen_approx.py` & `spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/negen_approx.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,130 +1,49 @@
 # Copyright 2023-present Ryan Balshaw
 """
 The negentropy approximation functions for the negentropy-based ICA methods.
 """
 import numpy as np
 
 
-class general_object(object):
-    """
-    An object that implements the first derivative, second derivative and
-    gamma functions of the XXXX (fill in here) function. These functions are used in the
-    negentropy calculation for negentropy-based ICA.
-
-    Methods
-    -------
-    function(u = float)
-        Return the function form of G(u) for the XXXX function
-
-    first_derivative(u = float)
-        Return the function form of the first derivative g(u) for the XXXX function
-
-    second_derivative(u = float)
-        Return the function form of the second derivative g'(u) for the XXXX function
-
-    gamma(u = float)
-        Return the function form of ratio g'(u)/g(u) for the XXXX function
-    """
-
-    def function(self, u: float):
-        """
-        This method implements the functional form of G(u)
-
-        Parameters
-        ----------
-        u: (float): The input value to be fed through G(u)
-
-        Returns
-        -------
-            float: The computation of G(u)
-        """
-
-        return None
-
-    def first_derivative(self, u: float):
-        """
-        This method implements the first derivative of G(.) for g(u)
-
-        Parameters
-        ----------
-        u: (float): The input value to be fed through g(u)
-
-        Returns
-        -------
-            float: The computation of g(u)
-        """
-
-        return None
-
-    def second_derivative(self, u: float):
-        """
-        This method implements the second derivative of G(.) for g'(u)
-
-        Parameters
-        ----------
-        u: (float): The input value to be fed through g'(u)
-
-        Returns
-        -------
-            float: The computation of g'(u)
-        """
-
-        return None
-
-    def gamma(self, u):
-        """
-        This method implements the ratio of the second derivative to
-        the first derivative (gamma(u) = g'(u) / g(u))
-
-        Parameters
-        ----------
-        u: (float): The input value to be fed through gamma(u)
-
-        Returns
-        -------
-            float: The computation of gamma(u)
-        """
-
-        return None
-
-
-class logcosh_object(object):
+class LogcoshObject(object):
     """
     An object that implements the first derivative, second derivative and
     gamma functions of the logcosh function. These functions are used in the
     negentropy approximation calculation for negentropy-based ICA.
 
     Methods
     -------
     function(u = float) -> 1/a1 * log((exp(a1 * u) + exp(-a1 * u)) / 2)
-        Return the function form of G(u) for the logcosh function
+            Return the function form of G(u) for the logcosh function
 
     first_derivative(u = float) -> tanh
-        Return the function form of the first derivative g(u) for the logcosh function
+            Return the function form of the first derivative g(u) for the logcosh
+            function
 
     second_derivative(u = float) -> 1 - tanh^2(u)
-        Return the function form of the second derivative g'(u) for the logcosh function
+            Return the function form of the second derivative g'(u) for the logcosh
+            function
 
     gamma(u = float)
-        Return the function form of ratio g'(u)/g(u) for the logcosh function
+            Return the function form of ratio g'(u)/g(u) for the logcosh function
     """
 
     def __init__(self, a1=None):
         """
 
         Parameters
         ----------
         a1: float
-            The a1 parameter for the  generalised logcosh function.
+                The a1 parameter for the  generalised logcosh function.
 
         Raises
         ------
         ValueError
-            If the a1 value is outside the recommended domain of [1, 2]
+                If the a1 value is outside the recommended domain of [1, 2]
         """
         if a1 is None:
             self.a1 = [1]  # [a1 = 1]
 
         else:
             if a1 < 1 or a1 > 2:
                 print(
@@ -136,39 +55,41 @@
 
     def function(self, u):
         """
         This method implements the functional form of G(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through G(u)
+        u: float
+                The input value to be fed through G(u)
 
         Returns
         -------
-            float: The computation of G(u)
+        The computation of G(u)
 
         """
 
         return (
             1
-            / (self.a1)
+            / self.a1
             * np.log((np.exp(self.a1 * u) + np.exp(-self.a1 * u)) / 2 + 1e-12)
         )  # 1e-12 for stability
 
     def first_derivative(self, u):
         """
         This method implements the first derivative of G(.) for g(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through g(u)
+        u: (float):
+                The input value to be fed through g(u)
 
         Returns
         -------
-            float: The computation of g(u)
+        The computation of g(u)
         """
         # au = self.a1 * u
         # e_au = np.exp(au)
         # e_n_au = np.exp(-au)
 
         return np.tanh(self.a1 * u)
         # (e_au - e_n_au) / (
@@ -176,36 +97,38 @@
 
     def second_derivative(self, u):
         """
         This method implements the second derivative of G(.) for g'(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through g'(u)
+        u: (float):
+                The input value to be fed through g'(u)
 
         Returns
         -------
-            float: The computation of g'(u)
+        The computation of g'(u)
         """
         d1 = self.first_derivative(self.a1 * u)
 
         return 1 - self.a1 * d1 * d1
 
     def gamma(self, u):
         """
         This method implements the ratio of the second derivative to
         the first derivative (gamma(u) = g'(u) / g(u))
 
         Parameters
         ----------
-        u: (float): The input value to be fed through gamma(u)
+        u: (float):
+                The input value to be fed through gamma(u)
 
         Returns
         -------
-            float: The computation of gamma(u)
+        The computation of gamma(u)
         """
         return self.second_derivative(u) / self.first_derivative(u)
 
     # I played around with finding the inverse distribution from the
     # transformed distribution.
     # Not useful here.
 
@@ -226,46 +149,46 @@
     #     numerator = e_p + e_2p * (e_2p - 1) ** (-1 / 2)
     #     denominator = e_p + np.sqrt(e_2p - 1)
     #     deriv = numerator / denominator
     #
     #     return np.array([-1, 1]) * deriv.reshape(-1, 1)
 
 
-class exp_object(object):
+class ExpObject(object):
     """
     An object that implements the first derivative, second derivative and
     gamma functions of the exp function. These functions are used in the
     negentropy approximation calculation for negentropy-based ICA.
 
     Methods
     -------
     function(u = float) -> -1/a2 * exp(-a2/2 * u^2)
-        Return the function form of G(u) for the exp function
+            Return the function form of G(u) for the exp function
 
     first_derivative(u = float) -> u * exp(-a2/2 * u^2)
-        Return the function form of the first derivative g(u) for the exp function
+            Return the function form of the first derivative g(u) for the exp function
 
     second_derivative(u = float) -> (1 - a2 * u^*2) * exp(-a2 / 2 * u^2)
-        Return the function form of the second derivative g'(u) for the exp function
+            Return the function form of the second derivative g'(u) for the exp function
 
     gamma(u = float) -> (1 - a2 * u^2) / u
-        Return the function form of ratio g'(u)/g(u) for the exp function
+            Return the function form of ratio g'(u)/g(u) for the exp function
     """
 
     def __init__(self, a2=None):
         """
         Parameters
         ----------
         a2: float - default: 1
-            The a2 parameter for the exp function.
+                The a2 parameter for the exp function.
 
         Raises
         ------
         ValueError
-            If the a2 value is outside the recommended domain of [0, 2]
+                If the a2 value is outside the recommended domain of [0, 2]
         """
         if a2 is None:
             self.a2 = [1]  # [a2 = 1]
 
         else:
             if a2 < 0 or a2 > 2:
                 print(
@@ -278,257 +201,289 @@
 
     def function(self, u):
         """
         This method implements the functional form of G(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through G(u)
+        u: (float):
+                The input value to be fed through G(u)
 
         Returns
         -------
-            float: The computation of G(u)
+        The computation of G(u)
         """
         return -1 / self.a2 * np.exp(-self.a2 / 2 * u**2)
 
     def first_derivative(self, u):
         """
         This method implements the first derivative of G(.) for g(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through g(u)
+        u: (float):
+                The input value to be fed through g(u)
 
         Returns
         -------
-            float: The computation of g(u)
+        The computation of g(u)
         """
         return u * np.exp(-self.a2 * u * u / 2)
 
     def second_derivative(self, u):
         """
         This method implements the second derivative of G(.) for g'(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through g'(u)
+        u: (float):
+                The input value to be fed through g'(u)
 
         Returns
         -------
-            float: The computation of g'(u)
+        The computation of g'(u)
         """
         return np.exp(-self.a2 * u * u / 2) * (1 - self.a2 * u * u)
 
     def gamma(self, u):
         """
         This method implements the ratio of the second derivative to
         the first derivative (gamma(u) = g'(u) / g(u))
 
         Parameters
         ----------
-        u: (float): The input value to be fed through gamma(u)
+        u: (float):
+                The input value to be fed through gamma(u)
 
         Returns
         -------
-            float: The computation of gamma(u)
+        The computation of gamma(u)
         """
         return (1 - self.a2 * u * u) / u
 
 
-class quad_object(object):
+class QuadObject(object):
     """
     An object that implements the first derivative, second derivative and
     gamma functions of the quad (u**4) function. These functions are used in the
     negentropy approximation calculation for negentropy-based ICA.
 
     Methods
     -------
     function(u = float) -> 1/4 u^4
-        Return the function form of G(u) for the quartic function
+            Return the function form of G(u) for the quartic function
 
     first_derivative(u = float) -> u^3
-        Return the function form of the first derivative g(u) for the quartic function
+            Return the function form of the first derivative g(u) for the quartic
+            function
 
     second_derivative(u = float) -> 3 u ^2
-        Return the function form of the second derivative g'(u) for the quartic function
+            Return the function form of the second derivative g'(u) for the quartic
+            function
 
     gamma(u = float) -> 3 / u
-        Return the function form of ratio g'(u)/g(u) for the quartic function
+            Return the function form of ratio g'(u)/g(u) for the quartic function
     """
 
-    def function(self, u):
+    @staticmethod
+    def function(u):
         """
         This method implements the functional form of G(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through G(u)
+        u: (float):
+                The input value to be fed through G(u)
 
         Returns
         -------
-            float: The computation of G(u)
+        The computation of G(u)
         """
         return 1 / 4 * u**4
 
-    def first_derivative(self, u):
+    @staticmethod
+    def first_derivative(u):
         """
         This method implements the first derivative of G(.) for g(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through g(u)
+        u: (float):
+                The input value to be fed through g(u)
 
         Returns
         -------
-            float: The computation of g(u)
+        The computation of g(u)
         """
         return u**3
 
-    def second_derivative(self, u):
+    @staticmethod
+    def second_derivative(u):
         """
         This method implements the second derivative of G(.) for g'(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through g'(u)
+        u: (float):
+                The input value to be fed through g'(u)
 
         Returns
         -------
-            float: The computation of g'(u)
+        The computation of g'(u)
         """
         return 3 * u**2
 
-    def gamma(self, u):
+    @staticmethod
+    def gamma(u):
         """
         This method implements the ratio of the second derivative to
         the first derivative (gamma(u) = g'(u) / g(u))
 
         Parameters
         ----------
-        u: (float): The input value to be fed through gamma(u)
+        u: (float):
+                The input value to be fed through gamma(u)
 
         Returns
         -------
-            float: The computation of gamma(u)
+        The computation of gamma(u)
         """
         return 3 / u
 
 
-class cube_object(object):
+class CubeObject(object):
     """
     An object that implements the first derivative, second derivative and
     gamma functions of the quad (u**4) function. These functions are used in the
     negentropy approximation calculation for negentropy-based ICA.
 
     Methods
     -------
     function(u = float) -> u^3
-        Return the function form of G(u) for the quartic function
+            Return the function form of G(u) for the cube function
 
     first_derivative(u = float) -> 3 u^2
-        Return the function form of the first derivative g(u) for the quartic function
+            Return the function form of the first derivative g(u) for the cube
+            function
 
     second_derivative(u = float) -> 6 u
-        Return the function form of the second derivative g'(u) for the quartic function
+            Return the function form of the second derivative g'(u) for the cube
+            function
 
     gamma(u = float) -> 2 / u
-        Return the function form of ratio g'(u)/g(u) for the quartic function
+            Return the function form of ratio g'(u)/g(u) for the cube function
     """
 
-    def function(self, u):
+    @staticmethod
+    def function(u):
         """
         This method implements the functional form of G(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through G(u)
+        u: (float):
+                The input value to be fed through G(u)
 
         Returns
         -------
-            float: The computation of G(u)
+        The computation of G(u)
         """
         return u**3
 
-    def first_derivative(self, u):
+    @staticmethod
+    def first_derivative(u):
         """
         This method implements the first derivative of G(.) for g(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through g(u)
+        u: (float):
+                The input value to be fed through g(u)
 
         Returns
         -------
-            float: The computation of g(u)
+        The computation of g(u)
         """
         return 3 * u**2
 
-    def second_derivative(self, u):
+    @staticmethod
+    def second_derivative(u):
         """
         This method implements the second derivative of G(.) for g'(u)
 
         Parameters
         ----------
-        u: (float): The input value to be fed through g'(u)
+        u: (float):
+                The input value to be fed through g'(u)
 
         Returns
         -------
-            float: The computation of g'(u)
+        The computation of g'(u)
         """
         return 6 * u
 
-    def gamma(self, u):
+    @staticmethod
+    def gamma(u):
         """
         This method implements the ratio of the second derivative to
         the first derivative (gamma(u) = g'(u) / g(u))
 
         Parameters
         ----------
-        u: (float): The input value to be fed through gamma(u)
+        u: (float):
+                The input value to be fed through gamma(u)
 
         Returns
         -------
-            float: The computation of gamma(u)
+                The computation of gamma(u)
         """
         return 2 / u
 
 
 def initialise_sources(
     source_name: str = "logcosh",
-    source_params: dict = {"source_name": "logcosh", "alpha": 1},
+    source_params: dict | None = None,
 ):
     """
     A function that takes in the source name and its associated parameters
     and returns the source instance and the E{G(nu)} value
     for a set number of samples (100 000 samples).
 
     Parameters
     ----------
     source_name: str
-        The name of the source that is to be used.
+            The name of the source that is to be used.
 
-    source_params: dict (default {"source_name":"logcosh", 'alpha':1})
-        The dictionary of parameters for the associated approximator.
+    source_params: dict | None (default None)
+            The dictionary of parameters for the associated approximator.
+            Format: {"alpha": alpha_val} where alpha_val is some float.
 
     Returns
     -------
+    source_instance:
+            The source instance that is to be used.
+
+    source_expecation: float
+            The evaluation of G(nu) for a set number of samples.
 
     """
+    if source_params is None:
+        source_params = {"alpha": 1}
 
     if source_name.lower() == "logcosh":
-        source_instance = logcosh_object(source_params["alpha"])
+        source_instance = LogcoshObject(source_params["alpha"])
 
     elif source_name.lower() == "exp":
-        source_instance = exp_object(source_params["alpha"])
+        source_instance = ExpObject(source_params["alpha"])
 
     elif source_name.lower() == "quad":
-        source_instance = quad_object()
+        source_instance = QuadObject()
 
     elif source_name.lower() == "cube":
-        source_instance = cube_object()
+        source_instance = CubeObject()
 
     else:
         print("Source name ({}) is unknown. Exiting the function.".format(source_name))
         raise SystemExit
 
     # Initialise expected value for G(nu) (for the negentropy-based ICA objective)
```

### Comparing `spectrally_constrained_lvms-0.1.1/spectrally_constrained_LVMs/spectral_constraint.py` & `spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/spectral_constraint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,93 +1,95 @@
 # Copyright 2023-present Ryan Balshaw
 """
 The spectral constraint method to be added to negentropy-based ICA approach.
 """
 import numpy as np
 
 
-class spectral_objective(object):
+class SpectralObjective(object):
     """
     An object that implements the spectral constraint objective.
 
     Methods
     -------
     dftmtx()
-        A method that returns the DFT matrix (unnormalised) by 1/sqrt(N).
+            A method that returns the DFT matrix (unnormalised) by 1/sqrt(N).
 
     decompose_DFT()
-        A method that decomposes the unnormalised DFT matrix into the real and
-        imaginary matrices R and I.
+            A method that decomposes the unnormalised DFT matrix into the real and
+            imaginary matrices R and I.
 
-    Haramard_product(A, x)
-        A method that computes the Haramard product for the matrix-vector product
-        v = A @ x. This returns v * v (elementwise product)
-
-    Haramard_derivative(A, x)
-        A method that computes the Haramard product derivative w.r.t the x
-        vector. d/dx(v * v) = 2 * diag(A @ x) @ A
+    Hadamard_product(A, x)
+            A method that computes the Hadamard product for the matrix-vector product
+            v = A @ x. This returns v * v (elementwise product)
+
+    Hadamard_derivative(A, x)
+            A method that computes the Hadamard product derivative w.r.t the x
+            vector. d/dx(v * v) = 2 * diag(A @ x) @ A
 
     check_w_want(w1)
-        This method checks whether the vector that we compare to (w1) is suitable.
-        It allows for either a Nx1 vector or a MxN matrix.
+            This method checks whether the vector that we compare to (w1) is suitable.
+            It allows for either a Nx1 vector or a MxN matrix.
 
     Xw(Re, Im, w)
-        This method computes the squared complex modulus of the Fourier
-        vector F(w). The returned vector is normalised by 1/N. It accounts for
-        the shape of w, to allow for a w to either be a Nx1 vector or a MxN matrix
-        for M vectors w.
+            This method computes the squared complex modulus of the Fourier
+            vector F(w). The returned vector is normalised by 1/N. It accounts for
+            the shape of w, to allow for a w to either be a Nx1 vector or a MxN matrix
+            for M vectors w.
 
     spectral_loss(w, w1)
-        This method returns the loss function for the spectral constraint.
-        It computes the dot product between the Fourier representation of w
-        and the Fourier representation/representations of the vector/vectors
-        in w1. The resulting shape of the loss is either a 1x1 vector or a
-        Mx1 vector (depending on whether w is a vector or matrix of vectors)
+            This method returns the loss function for the spectral constraint.
+            It computes the dot product between the Fourier representation of w
+            and the Fourier representation/representations of the vector/vectors
+            in w1. The resulting shape of the loss is either a 1x1 vector or a
+            Mx1 vector (depending on whether w is a vector or matrix of vectors)
 
     spectral_derivative(w, w1)
-        This method computes the first derivative (gradient) of the spectral loss
-        w.r.t the w parameters. It returns a Nx1 vector of parameters
-        or a NxM matrix of M gradient vectors.
+            This method computes the first derivative (gradient) of the spectral loss
+            w.r.t the w parameters. It returns a Nx1 vector of parameters
+            or a NxM matrix of M gradient vectors.
 
     spectral_hessian(w, w1)
-        This method computes the second derivative (Hessian) of the spectral loss
-        w.r.t the w parameters. it either returns a NxN vector of parameters
-        of a MxNxN matrix of M Hessians.
+            This method computes the second derivative (Hessian) of the spectral loss
+            w.r.t the w parameters. it either returns a NxN vector of parameters
+            of a MxNxN matrix of M Hessians.
     """
 
     def __init__(self, N, save_hessian_flag=True, inv_hessian_flag=True, verbose=False):
         """
         This method initialises the spectral constraint. It allows the user to
         define whether they wish to save the Hessian matrix in the instance,
         whether the inverse hessian is to be calculated and returned, and
         defines whether the print statements are used.
 
         Parameters
         ----------
         N: int | float
-            The dimensionality of the constraint domain.
+                The dimensionality of the constraint domain.
 
         save_hessian_flag: bool
-            A flag used to specify whether the hessian is saved locally in the
-            instance after it has been calculated.
+                A flag used to specify whether the hessian is saved locally in the
+                instance after it has been calculated.
 
         inv_hessian_flag: bool
-            A flag to specify whether the inverse hessian at computation time.
+                A flag to specify whether the inverse hessian at computation time.
 
         verbose: bool
-            A flag to control whether the print statements are used for the loss
-            function, derivative and the hessian.
+                A flag to control whether the print statements are used for the loss
+                function, derivative and the hessian.
 
+        Attributes
+        ----------
         R: ndarray
-            2D array of shape NxN contained data with 'float' type.
-            The real components of the unnormalised DFT matrix.
+                2D array of shape NxN contained data with 'float' type.
+                The real components of the unnormalised DFT matrix.
 
         I: ndarray
-            2D array of shape NxN contained data with 'float' type.
-            The imaginary components of the unnormalised DFT matrix.
+                2D array of shape NxN contained data with 'float' type.
+                The imaginary components of the unnormalised DFT matrix.
         """
         self.N = N
         self.save_hessian_flag = save_hessian_flag
         self.inv_hessian_flag = inv_hessian_flag
         self.verbose = verbose
 
         # Get R and I
@@ -96,16 +98,16 @@
     def dftmtx(self):
         """
         Computes the DFT matrix.
 
         Returns
         -------
         DFT_matrix: ndarray
-            A 2D array of shape NxN contained data with 'complex' type. This is the
-            unnormalised DFT matrix.
+                A 2D array of shape NxN contained data with 'complex' type. This is the
+                unnormalised DFT matrix.
         """
         # # Method 1:
         # scipy.linalg.dft(N)
 
         # # Method 2:
         # L = np.arange(0, N, 1) #0 to N-1
 
@@ -125,107 +127,107 @@
     def decompose_DFT(self):
         """
         Splits the complex DFT matrix into its real and imaginary components.
 
         Returns
         -------
         Re: ndarray
-            2D array of shape NxN contained data with 'float' type.
-            The real components of the unnormalised DFT matrix.
+                2D array of shape NxN contained data with 'float' type.
+                The real components of the unnormalised DFT matrix.
 
         Im: ndarray
-            2D array of shape NxN contained data with 'float' type.
-            The imaginary components of the unnormalised DFT matrix.
+                2D array of shape NxN contained data with 'float' type.
+                The imaginary components of the unnormalised DFT matrix.
         """
         D = self.dftmtx()
 
         Re = np.real(D)
         Im = np.imag(D)
 
         return Re, Im
 
     @staticmethod
-    def Haramard_product(A, x, vectorised_flag=False):
+    def Hadamard_product(A, x, vectorised_flag=False):
         """
-        A method that computes the Haramard product of v = A @ x.
+        A method that computes the Hadamard product of v = A @ x.
 
         Parameters
         ----------
         A: ndarray
-            The matrix component of v of 'float' type.
+                The matrix component of v of 'float' type.
 
         x: ndarray
-            The vector component of v of 'float' type. Shape is either Nx1 or
-            MxN
+                The vector component of v of 'float' type. Shape is either Nx1 or
+                MxN
 
         vectorised_flag: bool
-            A flag to specify whether x is a Nx1 vector or a MxN matrix.
-            This is important to control whether v = A @ x (false) or
-            v = x @ A.T (assuming that x is already transposed).
+                A flag to specify whether x is a Nx1 vector or a MxN matrix.
+                This is important to control whether v = A @ x (false) or
+                v = x @ A.T (assuming that x is already transposed).
 
         Returns
         -------
-            The elementwise product of v ʘ v.
+                The elementwise product of v ʘ v.
         """
         # Ax = A @ x
 
         if vectorised_flag:
             v = x @ A.T
 
         else:
             v = A @ x
 
-        return (v) ** 2  # (Ax) * (Ax) #
+        return v**2  # (Ax) * (Ax) #
 
     @staticmethod
-    def Haramard_derivative(A, x):
+    def Hadamard_derivative(A, x):
         """
-        A method that computes the derivative of Haramard product of
+        A method that computes the derivative of Hadamard product of
         v = A @ x w.r.t x.
 
         This method has no requirement for a vectorised_flag variable as it is
         only to be called on the Fourier representation of the vector w, not
         the vector/matrix w1 that it is compared to.
 
         Parameters
         ----------
         A: ndarray
-            The matrix component of v of 'float' type.
+                The matrix component of v of 'float' type.
 
         x: ndarray
-            The vector component of v of 'float' type. Shape is either Nx1 or
-            MxN
+                The vector component of v of 'float' type. Shape is either Nx1 or
+                MxN
 
         Returns
         -------
-            The elementwise derivative of v ʘ v w.r.t x.
+                The elementwise derivative of v ʘ v w.r.t x.
         """
         v = A @ x
 
         # Diagonalising is very slow! You can get the same output by just elementwise
         # multiplying A with the vector v.
 
-        return 2 * (v) * A  # 2 * np.diag(Ax[:, 0]) @ A
+        return 2 * v * A  # 2 * np.diag(Ax[:, 0]) @ A
 
     def check_w_want(self, w1):
         """
         A method that checks the shape of the vector w1.
 
         It is just used as a simple check to ensure that it matches the
         dimensionality of the problem
 
         Parameters
         ----------
         w1: npdarray
-            The vector of interest
+                The vector of interest
 
         Returns
         -------
         bool
-            If w1, in some way, matches the dimensionality, it passes.
+                If w1, in some way, matches the dimensionality, it passes.
         """
         if w1.shape[0] == self.N and w1.shape[1] == 1:  # A Nx1 vector
             return True
 
         elif w1.shape[0] >= 1 and w1.shape[1] == self.N:  # A MxN matrix
             return True
 
@@ -237,66 +239,66 @@
         This method computes the squared modulus of the Fourier representation of
         a vector or matrix w. Instead of using a vectorised_flag (haramard_product is
         a staticmethod), I can just use the shape of w directly.
 
         Parameters
         ----------
         Re: ndarray
-            2D array of shape NxN contained data with 'float' type.
+                2D array of shape NxN contained data with 'float' type.
 
         Im: ndarray
-            2D array of shape NxN contained data with 'float' type.
+                2D array of shape NxN contained data with 'float' type.
 
         w: nparray
-            2D array of shape Nx1 or MxN with 'float' type.
+                2D array of shape Nx1 or MxN with 'float' type.
 
         Returns
         -------
         spectral_representation: ndarray
-            The squared modulus of the Fourier transform of w. Shape is either
-            Nx1 or MxN (depends on shape of w).
+                The squared modulus of the Fourier transform of w. Shape is either
+                Nx1 or MxN (depends on shape of w).
         """
 
         if w.shape[1] == 1:
             vec_flag = False
 
         else:
             vec_flag = True
 
         spectral_representation = (
             1
             / self.N
             * (
-                self.Haramard_product(Re, w, vec_flag)
-                + self.Haramard_product(Im, w, vec_flag)
+                self.Hadamard_product(Re, w, vec_flag)
+                + self.Hadamard_product(Im, w, vec_flag)
             )
         )  # 1/N is included to satisfy Parseval's theorem (normalised)
 
         return spectral_representation
 
     def spectral_loss(self, w, w1):
         """
-        This method computes the spectral constrain loss function.
+        This method computes the spectral constraint loss function.
 
         Parameters
         ----------
         w: ndarray
-            The vector w that we wish to enforce is unique to the vector/vectors
-            in w1. Expected shape is Nx1.
+                The vector w that we wish to enforce is unique to the vector/vectors
+                in w1. Expected shape is Nx1.
 
         w1: ndarray
-            The vector/vectors that we wish to use to enforce that w is unique.
-            Expected shape is Nx1 or MxN.
+                The vector/vectors that we wish to use to enforce that w is unique.
+                Expected shape is Nx1 or MxN.
 
         Returns
         -------
         loss: float | ndarray
-            The dot product between the spectral representations of the w vector
-            and the vector/vectors in w1. It is either a scalar (if w1 is a vector)
-            or a Mx1 vector (if w1 is a MxN vector).
+                The dot product between the spectral representations of the w vector
+                and the vector/vectors in w1. It is either a scalar (if w1 is a vector)
+                or a Mx1 vector (if w1 is a MxN vector).
         """
 
         if self.verbose:
             print("Determining the loss function...")
 
         try:
             assert self.check_w_want(w1)
@@ -305,16 +307,14 @@
             print("W_want is the wrong shape!")
             raise SystemExit
 
         # Assume that w and w1 are column vectors
         # w = thing to optimise
         # w1 = goal
         # Calculate the loss
-
-        w.shape[0]
         # R, I = decompose_DFT(n)
 
         Xw_want = self.Xw(
             self.R, self.I, w1
         )  # np.convolve(w1[:, 0], w1[:, 0][::-1], mode = 'same').reshape(-1, 1))#
 
         # Xw_want = Xw_want * (Xw_want > 2 * np.std(Xw_want))
@@ -335,31 +335,33 @@
         """
         This method computes the first derivative of the spectral constraint
         loss function w.r.t w.
 
         Parameters
         ----------
         w: ndarray
-            The vector w that we wish to enforce is unique to the vector/vectors
-            in w1. Expected shape is Nx1.
+                The vector w that we wish to enforce is unique to the vector/vectors
+                in w1. Expected shape is Nx1.
 
         w1: ndarray
-            The vector/vectors that we wish to use to enforce that w is unique.
-            Expected shape is Nx1 or MxN.
+                The vector/vectors that we wish to use to enforce that w is unique.
+                Expected shape is Nx1 or MxN.
 
         Returns
         -------
         gradient: ndarray
-            The first derivative of the dot product between the spectral representations
-            of the w vector and the vector/vectors in w1. It is either a Nx1 vector
-            (if w1 is a vector) or a NxM matrix (if w1 is a MxN vector).
-
-            Note: I chose to use a NxM matrix for the latter as I know
-            each column represents a gradient vector as the constraint is applied
-            additively, so I can just sum over axis=1 to get a combined gradient vector.
+                The first derivative of the dot product between the spectral
+                representations of the w vector and the vector/vectors in w1.
+                It is either a Nx1 vector (if w1 is a vector) or a NxM matrix
+                (if w1 is a MxN vector).
+
+                Note: I chose to use a NxM matrix for the latter as I know
+                each column represents a gradient vector as the constraint is applied
+                additively, so I can just sum over axis=1 to get a combined gradient
+                vector.
         """
 
         if self.verbose:
             print("Determining the gradient...")
 
         try:
             assert self.check_w_want(w1)
@@ -374,18 +376,18 @@
         # Calculate the derivative
 
         Xw_want = self.Xw(
             self.R, self.I, w1
         )  # np.convolve(w1[:, 0], w1[:, 0][::-1], mode = 'same').reshape(-1, 1))#
         # Xw_want = Xw_want * (Xw_want > 2 * np.std(Xw_want))
 
-        term1 = self.Haramard_derivative(
+        term1 = self.Hadamard_derivative(
             self.R, w.reshape(-1, 1) if len(w.shape) == 1 else w
         )
-        term2 = self.Haramard_derivative(
+        term2 = self.Hadamard_derivative(
             self.I, w.reshape(-1, 1) if len(w.shape) == 1 else w
         )
 
         if w1.shape[1] == 1:
             gradient = (
                 (1 / self.N) * Xw_want.T @ (term1 + term2)
             )  # normalise by 1/N to account for term not included in (term1 + term2)
@@ -403,34 +405,34 @@
         """
         This method computes the second derivative of the spectral constraint
         loss function w.r.t w.
 
         Parameters
         ----------
         w: ndarray
-            The vector w that we wish to enforce is unique to the vector/vectors
-            in w1. Expected shape is Nx1.
+                The vector w that we wish to enforce is unique to the vector/vectors
+                in w1. Expected shape is Nx1.
 
         w1: ndarray
-            The vector/vectors that we wish to use to enforce that w is unique.
-            Expected shape is Nx1 or MxN.
+                The vector/vectors that we wish to use to enforce that w is unique.
+                Expected shape is Nx1 or MxN.
 
         Returns
         -------
         hessian: ndarray
-            The second derivative of the dot product between the spectral
-            representations of the w vector and the vector/vectors in w1.
-            It is either a NxN matrix (if w1 is a vector) or a MxNxN
-            matrix (if w1 is a MxN vector).
+                The second derivative of the dot product between the spectral
+                representations of the w vector and the vector/vectors in w1.
+                It is either a NxN matrix (if w1 is a vector) or a MxNxN
+                matrix (if w1 is a MxN vector).
 
         If save_hessian_flag is used during initialisation, it will first
         check to see if a Hessian exists.
 
         If inv_hessian_flag is used during initialisation, it will return
-         both the hessian and its inverse (NOT recommended).
+        both the hessian and its inverse (NOT recommended).
         """
 
         try:
             assert self.check_w_want(w1)
 
         except AssertionError:
             print("W_want is the wrong shape!")
@@ -464,18 +466,16 @@
 
                     dir_mat[c, :, :] = self.R[:, [c]] * self.R + self.I[:, [c]] * self.I
 
                 self.dir_mat = dir_mat
 
             if w1.shape[1] == 1:
                 hessian = (2 / self.N) * (
-                    np.tensordot(Xw_want.T, self.dir_mat, axes=([1], [1]))[
-                        0, :, :
-                    ]  # normalise by 2/N to account for term not included in (dir_mat)
-                )
+                    np.tensordot(Xw_want.T, self.dir_mat, axes=([1], [1]))[0, :, :]
+                )  # normalise by 2/N to account for term not included in (dir_mat)
 
             else:
                 hessian = (2 / self.N) * np.tensordot(
                     Xw_want, self.dir_mat, axes=([1], [1])
                 )  # normalise by 2/N to account for term not included in (dir_mat)
 
             # hessian = 2 * Xw_want.T @ dir_mat.transpose(1, 0, 2)
```


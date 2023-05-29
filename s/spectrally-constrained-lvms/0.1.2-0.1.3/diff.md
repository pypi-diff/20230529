# Comparing `tmp/spectrally_constrained_lvms-0.1.2.tar.gz` & `tmp/spectrally_constrained_lvms-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spectrally_constrained_lvms-0.1.2.tar", max compression
+gzip compressed data, was "spectrally_constrained_lvms-0.1.3.tar", max compression
```

## Comparing `spectrally_constrained_lvms-0.1.2.tar` & `spectrally_constrained_lvms-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_constrained_lvms-0.1.2/LICENSE
--rw-r--r--   0        0        0     1747 2023-05-29 10:56:50.260003 spectrally_constrained_lvms-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     6955 2023-05-29 10:57:01.810232 spectrally_constrained_lvms-0.1.2/README.md
--rw-r--r--   0        0        0     1184 2023-05-29 10:56:50.271514 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/__init__.py
--rw-r--r--   0        0        0    32742 2023-05-26 12:13:55.514135 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/cost_functions.py
--rw-r--r--   0        0        0    21405 2023-05-26 12:13:55.515128 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/helper_methods.py
--rw-r--r--   0        0        0    13584 2023-05-26 12:13:55.515631 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/negen_approx.py
--rw-r--r--   0        0        0    16775 2023-05-26 12:13:55.517156 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/spectral_constraint.py
--rw-r--r--   0        0        0    52550 2023-05-26 12:13:55.518215 spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/spectrally_constrained_model.py
--rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-04-28 07:39:34.154025 spectrally_constrained_lvms-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1747 2023-05-29 12:13:13.535204 spectrally_constrained_lvms-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     6955 2023-05-29 12:13:23.317568 spectrally_constrained_lvms-0.1.3/README.md
+-rw-r--r--   0        0        0     1184 2023-05-29 12:13:13.546738 spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/__init__.py
+-rw-r--r--   0        0        0    32459 2023-05-29 12:05:32.601314 spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/cost_functions.py
+-rw-r--r--   0        0        0    21405 2023-05-26 12:13:55.515128 spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/helper_methods.py
+-rw-r--r--   0        0        0    13584 2023-05-26 12:13:55.515631 spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/negen_approx.py
+-rw-r--r--   0        0        0    16775 2023-05-26 12:13:55.517156 spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/spectral_constraint.py
+-rw-r--r--   0        0        0    52550 2023-05-26 12:13:55.518215 spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/spectrally_constrained_model.py
+-rw-r--r--   0        0        0     8178 1970-01-01 00:00:00.000000 spectrally_constrained_lvms-0.1.3/PKG-INFO
```

### Comparing `spectrally_constrained_lvms-0.1.2/LICENSE` & `spectrally_constrained_lvms-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.2/pyproject.toml` & `spectrally_constrained_lvms-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spectrally-constrained-LVMs"
-version = "0.1.2"
+version = "0.1.3"
 description = "An optimisation implementation of linear transforms with a spectral constraint."
 authors = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 maintainers = ["Ryan Balshaw <ryanbalshaw81@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/RyanBalshaw/spectrally-constrained-LVMs"
 repository = "https://github.com/RyanBalshaw/spectrally-constrained-LVMs"
```

### Comparing `spectrally_constrained_lvms-0.1.2/README.md` & `spectrally_constrained_lvms-0.1.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ![GitHub license](https://img.shields.io/github/license/RyanBalshaw/spectrally-constrained-LVMs)
 ![GitHub last commit](https://img.shields.io/github/last-commit/RyanBalshaw/spectrally-constrained-LVMs)
 ![PyPI](https://img.shields.io/pypi/v/spectrally-constrained-lvms)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/spectrally-constrained-lvms?color=blueviolet)
 ![Read the Docs](https://img.shields.io/readthedocs/spectrally-constrained-lvms?color=informational)
 ![GitHub issues](https://img.shields.io/github/issues/RyanBalshaw/spectrally-constrained-LVMs?color=critical)
 
-*Current version:* 0.1.2
+*Current version:* 0.1.3
 
 Spectrally-constrained-LVMs is a Python-based package which facilitates the estimation of the linear latent variable model (LVM) parameters with a unique spectral constraint in single-channel time-series applications.
 
 ## Purpose
 LVMs are a statistical methodology which tries to capture the underlying structure in some observed data. This package caters to single channel time-series applications and provides a methodology to estimate the LVM parameters. The model parameters are encouraged to be diverse via a spectral constraint which enforces non-duplication of the spectral information captured by the latent sources.
 
 The purpose of this package is to provide a complete methodology that caters to a variety of LVM objective functions.
```

### Comparing `spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/__init__.py` & `spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     hankel_matrix,
 )
 from .negen_approx import CubeObject, ExpObject, LogcoshObject, QuadObject
 from .spectral_constraint import SpectralObjective
 from .spectrally_constrained_model import LinearModel
 
 __author__ = "Ryan Balshaw"
-__version__ = "0.1.2"
+__version__ = "0.1.3"
 __email__ = "ryanbalshaw81@gmail.com"
 __description__ = (
     "Train linear LVMs with the addition "
     "of a spectral constraint with minimal effort."
 )
 # __uri__ = "http://spectrally-constrained-lvms.readthedocs.io/"
 __all__ = [
```

### Comparing `spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/cost_functions.py` & `spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/cost_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,69 +18,69 @@
     """
     Base class for different formulations of the user
     cost function.
 
     Methods
     -------
     set_cost(cost_func)
-            This method takes in a cost_func variable and sets it as
-            an internal attribute self._cost.
+        This method takes in a cost_func variable and sets it as
+        an internal attribute self._cost.
 
     set_gradient(cost_gradient)
-            This method takes in a cost_gradient variable and sets it as
-            an internal attribute self._cost_gradient.
+        This method takes in a cost_gradient variable and sets it as
+        an internal attribute self._cost_gradient.
 
     set_hessian(cost_hessian)
-            This method takes in a cost_hessian variable and sets it as
-            an internal attribute self._cost_hessian.
+        This method takes in a cost_hessian variable and sets it as
+        an internal attribute self._cost_hessian.
 
     get_cost()
-            This method return the internal self._cost instance.
+        This method return the internal self._cost instance.
 
     get_gradient()
-            This method return the internal self._cost_gradient instance.
+        This method return the internal self._cost_gradient instance.
 
     get_hessian()
-            This method return the internal self._cost_hessian instance.
+        This method return the internal self._cost_hessian instance.
 
     check_gradient(X, w, y, step_size)
-            This method takes in an initial set of variables X, w, y, and a
-            finite difference step size. The function is used to check the
-            self._cost_gradient method using a central finite-difference
-            approach.
+        This method takes in an initial set of variables X, w, y, and a
+        finite difference step size. The function is used to check the
+        self._cost_gradient method using a central finite-difference
+        approach.
 
     check_hessian(X, w, y, step_size)
-            This method takes in an initial set of variables X, w, y, and a
-            finite difference step size. The function is used to check the
-            self._cost_hessian method using a central finite-difference
-            approach.
+        This method takes in an initial set of variables X, w, y, and a
+        finite difference step size. The function is used to check the
+        self._cost_hessian method using a central finite-difference
+        approach.
     """
 
     def __init__(self, verbose: bool = True):
         """
 
         Parameters
         ----------
         verbose : bool
-                A boolean flag to control any possible
-                print statements.
+            A boolean flag to control any possible
+            print statements.
         """
         self._cost = None
         self._cost_gradient = None
         self._cost_hessian = None
         self.verbose = verbose
 
     def set_cost(self, cost_func):
         """
         This method allows one to set their cost function.
 
         Parameters
         ----------
         cost_func : function
-                The users cost function.
+            The users cost function.
 
         Examples
         --------
         cost_func = lambda X, w, y: -1 * np.mean(y ** 2, axis=0)
 
         """
         self._cost = cost_func
@@ -88,32 +88,32 @@
     def set_gradient(self, cost_gradient):
         """
         This method allows one to set their gradient vector.
 
         Parameters
         ----------
         cost_gradient : function
-                The users gradient vector of the cost function.
+            The users gradient vector of the cost function.
 
         Examples
         --------
         cost_gradient = lambda X, w, y: -2 * np.mean(y * X, axis=0,
-                                                                        keepdims = True)
+            keepdims=True)
 
         """
         self._cost_gradient = cost_gradient
 
     def set_hessian(self, cost_hessian):
         """
         This method allows one to set their objective Hessian (optional).
 
         Parameters
         ----------
         cost_hessian : function
-                The users gradient vector of the cost function.
+            The users gradient vector of the cost function.
 
         Examples
         --------
         cost_hessian = lambda X, w, y: -2 /X.shape[0] * (X.T @ X)
 
         """
         self._cost_hessian = cost_hessian
@@ -162,37 +162,37 @@
         This method checks the self._cost_gradient function to determine
         whether the gradient implementation is correct based off the
         objective function.
 
         Parameters
         ----------
         X : ndarray
-                An array of size n_samples x n_features.
+            An array of size n_samples x n_features.
 
         w : ndarray
-                An column vector of size n_features x 1
+            An column vector of size n_features x 1
 
         y : ndarray
-                An column vector of size n_features x 1. Expected to be
-                equivalent to X @ w.
+            An column vector of size n_features x 1. Expected to be
+            equivalent to X @ w.
 
         step_size : float (default = 1e-4)
-                The finite difference step size.
+            The finite difference step size.
 
         Returns
         -------
         grad_current : ndarray
-                The gradient based off the internal self._cost_gradient instance.
+            The gradient based off the internal self._cost_gradient instance.
 
         grad_check : ndarray
-                The finite-difference approximation to the gradient
+            The finite-difference approximation to the gradient
 
         grad_norm : ndarray
-                The L2 norm between the analytical gradient and the finite difference
-                approximation.
+            The L2 norm between the analytical gradient and the finite difference
+            approximation.
 
         Note that this is a helper method. costClass operates as a base class,
         so you will find that methods such as self.cost() and self.cost_gradient()
         are accessed but never defined. I use a child class to define these methods.
         """
         # Finite difference gradient approximation (central difference)
 
@@ -228,37 +228,37 @@
         This method checks the self._cost_hessian function to determine
         whether the hessian implementation is correct based off the
         user-defined objective function.
 
         Parameters
         ----------
         X : ndarray
-                An array of size n_samples x n_features.
+            An array of size n_samples x n_features.
 
         w : ndarray
-                An column vector of size n_features x 1
+            An column vector of size n_features x 1
 
         y : ndarray
-                An column vector of size n_features x 1. Expected to be
-                equivalent to X @ w.
+            An column vector of size n_features x 1. Expected to be
+            equivalent to X @ w.
 
         step_size : float (default = 1e-4)
-                The finite difference step size.
+            The finite difference step size.
 
         Returns
         -------
         hess_current : ndarray
-                The hessian based off the internal self._cost_hessian instance.
+            The hessian based off the internal self._cost_hessian instance.
 
         hess_check : ndarray
-                The finite-difference approximation to the hessian.
+            The finite-difference approximation to the hessian.
 
         hess_norm : ndarray
-                The L2 norm (average of the row-wise L2 norm) between the analytical
-                hessian and the finite difference approximation.
+            The L2 norm (average of the row-wise L2 norm) between the analytical
+            hessian and the finite difference approximation.
 
         Note that this is a helper method. costClass operates as a base class,
         so you will find that methods such as self.cost() and self.cost_hessian()
         are accessed but never defined. I use a child class to define these methods.
         """
         # Finite difference Hessian approximation (central difference)
 
@@ -314,94 +314,94 @@
     Assumed function format from user: func(X, w, y) where X is a ndarray
     with shape (n_samples, n_features), w is a ndarray with shape (n_features, 1)
     and y is the linear transformation X @ w with shape (n_samples, 1).
 
     Methods
     -------
     cost(X, w, y)
-            This method accesses the internal self._cost instance attribute and
-            returns its output self._cost(X, w, y).
+        This method accesses the internal self._cost instance attribute and
+        returns its output self._cost(X, w, y).
 
     cost_gradient(X, w, y)
-            This method accesses the internal self._cost_gradient instance attribute and
-            returns its output self._cost_gradient(X, w, y).
+        This method accesses the internal self._cost_gradient instance attribute and
+        returns its output self._cost_gradient(X, w, y).
 
     cost_hessian(X, w, y)
-            This method accesses the internal self._cost_hessian instance attribute and
-            returns its output self._cost_hessian(X, w, y).
+        This method accesses the internal self._cost_hessian instance attribute and
+        returns its output self._cost_hessian(X, w, y).
     """
 
     def __init__(self, use_hessian: bool = True, verbose: bool = True):
         """
         Parameters
         ----------
         use_hessian : bool
-                A flag to control whether you use the Hessian or not.
-                This is useful in the parameter estimation step, as you may wish to just
-                perform steepest descent instead of using Newton's method.
+            A flag to control whether you use the Hessian or not.
+            This is useful in the parameter estimation step, as you may wish to just
+            perform steepest descent instead of using Newton's method.
         """
         super().__init__(verbose)
         self.use_hessian = use_hessian
 
     def cost(self, X, w, y):
         """
         A method that returns the cost function for the inputs.
 
         Parameters
         ----------
         X : ndarray
-                The feature matrix of size (n_samples, n_features)
+            The feature matrix of size (n_samples, n_features)
 
         w : ndarray
-                The transformation vector of size (n_features, 1)
+            The transformation vector of size (n_features, 1)
 
         y : ndarray
-                The transformed variable y = X @ w of size (n_samples, 1)
+            The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         cost function evalation of (X, w, y)
         """
         return self._cost(X, w, y)
 
     def cost_gradient(self, X, w, y):
         """
         A method that returns the cost function gradient for the inputs.
 
         Parameters
         ----------
         X : ndarray
-                The feature matrix of size (n_samples, n_features)
+            The feature matrix of size (n_samples, n_features)
 
         w : ndarray
-                The transformation vector of size (n_features, 1)
+            The transformation vector of size (n_features, 1)
 
         y : ndarray
-                The transformed variable y = X @ w of size (n_samples, 1)
+            The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         derivative function evalation of (X, w, y)
         """
         return self._cost_gradient(X, w, y)
 
     def cost_hessian(self, X, w, y):
         """
         A method that returns the Hessian function for the inputs.
 
         Parameters
         ----------
         X : ndarray
-                The feature matrix of size (n_samples, n_features)
+            The feature matrix of size (n_samples, n_features)
 
         w : ndarray
-                The transformation vector of size (n_features, 1)
+            The transformation vector of size (n_features, 1)
 
         y : ndarray
-                The transformed variable y = X @ w of size (n_samples, 1)
+            The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         Hessian function evalation of (X, w, y)
         """
         if self.use_hessian:
             return self._cost_hessian(X, w, y)
@@ -431,83 +431,83 @@
     and y is the linear transformation X @ w with shape (n_samples, 1).
 
     Note that while y is an input that is given for repeatability,
 
     Methods
     -------
     cost(X, w, y)
-            This method accesses the internal self._cost instance attribute and
-            returns its output self._cost(X, w, y).
+        This method accesses the internal self._cost instance attribute and
+        returns its output self._cost(X, w, y).
 
     cost_gradient(X, w, y)
-            This method accesses the internal self._cost_gradient instance attribute and
-            returns its output self._cost_gradient(X, w, y).
+        This method accesses the internal self._cost_gradient instance attribute and
+        returns its output self._cost_gradient(X, w, y).
 
     cost_hessian(X, w, y)
-            This method accesses the internal self._cost_hessian instance attribute and
-            returns its output self._cost_hessian(X, w, y).
+        This method accesses the internal self._cost_hessian instance attribute and
+        returns its output self._cost_hessian(X, w, y).
     """
 
     def __init__(
         self,
         n_samples: int,
         n_features: int,
         use_hessian: bool = False,
         verbose: bool = True,
     ):
         """
 
         Parameters
         ----------
         n_samples : int
-                The number of samples in X.
+            The number of samples in X.
 
         n_features : int
-                The number of features in X.
+            The number of features in X.
 
         use_hessian : bool (default = True)
-                A flag to specify whether the Hessian (2nd derivative) of the loss
-                function must be used. If use_hessian = False, the .cost_hessian()
-                method returns and identity matrix.
+            A flag to specify whether the Hessian (2nd derivative) of the loss
+            function must be used. If use_hessian = False, the .cost_hessian()
+            method returns and identity matrix.
 
         verbose : bool (default = True)
-                A flag to control the verbosity of different method calls.
+            A flag to control the verbosity of different method calls.
         """
         super().__init__(verbose)
         self.n_samples = n_samples
         self.n_features = n_features
         self.use_hessian = use_hessian
 
     def set_cost(self, cost_func):
         # overwrites the base method
         """
         This method allows one to set their cost function (overwrites default).
 
         Parameters
         ----------
         cost_func : function
-                The users cost function defined symbolically.
+            The users cost function defined symbolically.
 
         """
         self._sympy_cost = cost_func
 
     def get_model_parameters(self):
         """
 
         Returns
         -------
         X: sp.IndexedBase instance
-                An indexable SymPy matrix of size (n_samples, n_features)
+            An indexable SymPy matrix of size (n_samples, n_features)
 
         w:  sp.IndexedBase instance
-                An indexable SymPy matrix of size (n_features, 1)
+            An indexable SymPy matrix of size (n_features, 1)
 
         (i, j): tuple
-                A set of index variables that can be used to iterate over
-                the X and w sp.IndexedBase instances.
+            A set of index variables that can be used to iterate over
+            the X and w sp.IndexedBase instances.
 
         """
         i, j = sp.symbols("i j", cls=sp.Idx)
 
         self.w = sp.IndexedBase("w", shape=(self.n_features, 1))
         self.X = sp.IndexedBase("X", shape=(self.n_samples, self.n_features))
         self.y = sp.symbols("y")  # Placeholder variable
@@ -573,16 +573,16 @@
         """
         This method combines the implement_* methods into one call. The idea was to
         provide access to a set lambdification process through one instance call.
 
         Raises
         -------
         AttributeError
-                This is raised if the user's cost function has not been defined
-                within the instance.
+            This is raised if the user's cost function has not been defined
+            within the instance.
         """
         if hasattr(self, "_sympy_cost"):
             print("Calculating the sympy method components...")
 
             self.implement_cost()
             self.implement_first_derivative()
 
@@ -600,22 +600,22 @@
         """
         This method checks the shape of X to ensure it matches the pre-defined shape
         provided by the user.
 
         Parameters
         ----------
         X : ndarray
-                The input X matrix.
+            The input X matrix.
 
         Raises
         -------
         AssertionError
-                This is raised if the shape of X, given to and cost, cost_gradient or
-                cost_hessian call does not match the pre-defined shape given on instant
-                creation.
+            This is raised if the shape of X, given to and cost, cost_gradient or
+            cost_hessian call does not match the pre-defined shape given on instant
+            creation.
 
         """
         r, c = X.shape
         assert r == self.n_samples, print(
             f"Number of samples ({r}) in X  does not match the"
             f" expected value: {self.n_samples}."
         )
@@ -628,22 +628,22 @@
         """
         This method checks the shape of X to ensure it matches the pre-defined shape
         provided by the user.
 
         Parameters
         ----------
         w : ndarray
-                The input w vector.
+            The input w vector.
 
         Raises
         -------
         AssertionError
-                This is raised if the shape of X, given to and cost, cost_gradient or
-                cost_hessian call does not match the pre-defined shape given on instant
-                creation.
+            This is raised if the shape of X, given to and cost, cost_gradient or
+            cost_hessian call does not match the pre-defined shape given on instant
+            creation.
 
         """
         r, c = w.shape
         assert r == self.n_features, print(
             f"Number of samples ({r}) in w  does not match the"
             f" expected value: {self.n_features}."
         )
@@ -654,21 +654,21 @@
     def cost(self, X, w, y):
         """
         A method that returns the cost function for the inputs.
 
         Parameters
         ----------
         X : ndarray
-                The feature matrix of size (n_samples, n_features)
+            The feature matrix of size (n_samples, n_features)
 
         w : ndarray
-                The transformation vector of size (n_features, 1)
+            The transformation vector of size (n_features, 1)
 
         y : ndarray
-                The transformed variable y = X @ w of size (n_samples, 1)
+            The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         cost function evaluation of (X, w, y)
         """
         self._check_X(X)
         self._check_w(w)
@@ -681,42 +681,42 @@
     def cost_gradient(self, X, w, y):
         """
         A method that returns the cost function gradient for the inputs.
 
         Parameters
         ----------
         X : ndarray
-                The feature matrix of size (n_samples, n_features)
+            The feature matrix of size (n_samples, n_features)
 
         w : ndarray
-                The transformation vector of size (n_features, 1)
+            The transformation vector of size (n_features, 1)
 
         y : ndarray
-                The transformed variable y = X @ w of size (n_samples, 1)
+            The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         derivative function evaluation of (X, w, y)
         """
         return self._cost_gradient(X, w, y)
 
     def cost_hessian(self, X, w, y):
         """
         A method that returns the Hessian function for the inputs.
 
         Parameters
         ----------
         X : ndarray
-                The feature matrix of size (n_samples, n_features)
+            The feature matrix of size (n_samples, n_features)
 
         w : ndarray
-                The transformation vector of size (n_features, 1)
+            The transformation vector of size (n_features, 1)
 
         y : ndarray
-                The transformed variable y = X @ w of size (n_samples, 1)
+            The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         Hessian function evaluation of (X, w, y)
         """
         if self.use_hessian:
             return self._cost_hessian(X, w, y)
@@ -733,64 +733,69 @@
     Assumed function format: func(X, w, y) where X is a ndarray
     with shape (n_samples, n_features), w is a ndarray with shape (n_features, 1)
     and y is the linear transformation X @ w with shape (n_samples, 1).
 
     Methods
     -------
     cost(X, w, y)
-            This method calculates and returns the negentropy approximation
-            objective function.
+        This method calculates and returns the negentropy approximation
+        objective function.
 
     cost_gradient(X, w, y)
-            This method calculates and returns the gradient of the negentropy
-            approximation objective function.
+        This method calculates and returns the gradient of the negentropy
+        approximation objective function.
 
     cost_hessian(X, w, y)
-            This method calculates and returns the Hessian of the negentropy
-            approximation objective function.
+        This method calculates and returns the Hessian of the negentropy
+        approximation objective function.
     """
 
     def __init__(self, source_name: str, source_params: dict, verbose: bool = True):
         """
 
         Parameters
         ----------
         source_name : str
-                The name of the source function used for negentropy estimation.
-                Options: logcosh, exp, quad, cube
+            The name of the source function used for negentropy estimation.
+            Options: logcosh, exp, quad, cube
 
         source_params :  dict
-                A dictionary containing the source parameter {'alpha': 1}
+            A dictionary containing the source parameter {'alpha': 1}
 
         verbose : bool
-                Controls the verbosity of the instance.
+            Controls the verbosity of the instance.
         """
         super().__init__(verbose)
         self.source_name = source_name
         self.source_params = source_params  # dictionary of parameters
 
         # Initialise the source PDFs
         self.source_instance, self.source_expectation = initialise_sources(
             source_name, self.source_params
         )
 
+        # Enable compatability with CostClass
+        self.set_cost(self.cost)
+        self.set_gradient(self.cost_gradient)
+        self.set_hessian(self.cost_hessian)
+
     def cost(self, X, w, y):  # Important to negentropy-based ICA
         """
         Negentropy-estimate calculation for the objective function.
 
         Parameters
         ----------
         X : ndarray
-                The feature matrix of size (n_samples, n_features)
+            The feature matrix of size (n_samples, n_features)
 
         w : ndarray
-                The transformation vector of size (n_features, 1)
+            The transformation vector of size (n_features, 1)
 
         y : ndarray
-                The transformed variable y = X @ w of size (n_samples, 1)
+            The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         Negentropy cost in minimisation setting using (X, w, y)
 
         """
 
@@ -805,21 +810,21 @@
     def cost_gradient(self, X, w, y):
         """
         A method that returns the negentropy cost function gradient for the inputs.
 
         Parameters
         ----------
         X : ndarray
-                The feature matrix of size (n_samples, n_features)
+            The feature matrix of size (n_samples, n_features)
 
         w : ndarray
-                The transformation vector of size (n_features, 1)
+            The transformation vector of size (n_features, 1)
 
         y : ndarray
-                The transformed variable y = X @ w of size (n_samples, 1)
+            The transformed variable y = X @ w of size (n_samples, 1)
 
         Returns
         -------
         Derivative of the negetropy function evaluation using (X, w, y)
         """
         g_y = self.source_instance.first_derivative(y)
 
@@ -837,25 +842,25 @@
     def cost_hessian(self, X, w, y, approx_flag=True):
         """
         A method that returns the negentropy cost function Hessian for the inputs.
 
         Parameters
         ----------
         X : ndarray
-                The feature matrix of size (n_samples, n_features)
+            The feature matrix of size (n_samples, n_features)
 
         w : ndarray
-                The transformation vector of size (n_features, 1)
+            The transformation vector of size (n_features, 1)
 
         y : ndarray
-                The transformed variable y = X @ w of size (n_samples, 1)
+            The transformed variable y = X @ w of size (n_samples, 1)
 
         approx_flag : bool (default = True)
-                This flag specifies whether an approximation to the expectation in the
-                Hessian is used or not.
+            This flag specifies whether an approximation to the expectation in the
+            Hessian is used or not.
 
         Returns
         -------
         Hessian of the negentropy function evaluation using (X, w, y)
         """
         N, m = X.shape
 
@@ -890,45 +895,45 @@
 
         return jacobian
 
 
 class VarianceCost(UserCost):
     """
     This method implements the PCA variance maximisation objective. It inherits from
-    the user_cost class and simply implements the three necessary
+    the UserCost class and simply implements the three necessary components.
     """
 
     def __init__(self, use_hessian: bool = True, verbose: bool = True):
         """
         Defines the attributes for the user_cost class
 
         Parameters
         ----------
         use_hessian : bool
-                A flag to control whether you use the Hessian or not.
-                This is useful in the parameter estimation step, as you may wish to just
-                perform steepest descent instead of using Newton's method.
+            A flag to control whether you use the Hessian or not.
+            This is useful in the parameter estimation step, as you may wish to just
+            perform steepest descent instead of using Newton's method.
         """
         super().__init__(use_hessian, verbose)
 
         def loss(X, w, y):
             """
             The PCA variance maximisation cost function for an optimisation
             framework which performs minimisation.
 
             Parameters
             ----------
             X : ndarray
-                    The feature matrix of size (n_samples, n_features)
+                The feature matrix of size (n_samples, n_features)
 
             w : ndarray
-                            The transformation vector of size (n_features, 1)
+                The transformation vector of size (n_features, 1)
 
             y : ndarray
-                            The transformed variable y = X @ w of size (n_samples, 1)
+                The transformed variable y = X @ w of size (n_samples, 1)
 
             Returns
             -------
             Negative of latent variance.
             """
             return -1 * np.mean((X @ w) ** 2, axis=0)
 
@@ -936,21 +941,21 @@
             """
             The gradient of the PCA variance maximisation cost function for an
             optimisation framework which performs minimisation.
 
             Parameters
             ----------
             X : ndarray
-                    The feature matrix of size (n_samples, n_features)
+                The feature matrix of size (n_samples, n_features)
 
             w : ndarray
-                    The transformation vector of size (n_features, 1)
+                The transformation vector of size (n_features, 1)
 
             y : ndarray
-                    The transformed variable y = X @ w of size (n_samples, 1)
+                The transformed variable y = X @ w of size (n_samples, 1)
 
             Returns
             -------
             Gradient of the negative of latent variance.
             """
             return -2 * np.mean(y * X, axis=0, keepdims=True).T
 
@@ -958,63 +963,65 @@
             """
             The Hessian of the PCA variance maximisation cost function for an
             optimisation framework which performs minimisation.
 
             Parameters
             ----------
             X : ndarray
-                    The feature matrix of size (n_samples, n_features)
+                The feature matrix of size (n_samples, n_features)
 
             w : ndarray
-                    The transformation vector of size (n_features, 1)
+                The transformation vector of size (n_features, 1)
 
             y : ndarray
-                    The transformed variable y = X @ w of size (n_samples, 1)
+                The transformed variable y = X @ w of size (n_samples, 1)
 
             Returns
             -------
             Hessian of the negative of latent variance.
             """
             return -2 * np.cov(X, rowvar=False)
 
         self.set_cost(loss)
         self.set_gradient(grad)
         self.set_hessian(hess)
 
 
 # if __name__ == "__main__":
-# 	def l1_l2_norm(X, w, y):
-# 		N = X.shape[0]
-#
-# 		E1 = np.mean(np.abs(y), axis=0)
-# 		E2 = np.mean(y ** 2, axis=0)
+# def l1_l2_norm(X, w, y):
+# 	N = X.shape[0]
 #
-# 		return -1 * np.sqrt(N) * E1 / np.sqrt(E2)
+# 	E1 = np.mean(np.abs(y), axis=0)
+# 	E2 = np.mean(y ** 2, axis=0)
 #
+# 	return -1 * np.sqrt(N) * E1 / np.sqrt(E2)
 #
-# 	def l1_l2_grad(X, w, y):
-# 		N = X.shape[0]
 #
-# 		E1 = np.mean(np.abs(y), axis=0)
-# 		E2 = np.mean(y ** 2, axis=0)
+# def l1_l2_grad(X, w, y):
+# 	N = X.shape[0]
 #
-# 		p1 = np.mean(np.sign(y) * X, axis=0).T / np.sqrt(E2)
-# 		p2 = -1 * E1 / ((E2) ** (3 / 2)) * np.mean(y * X, axis=0).T
+# 	E1 = np.mean(np.abs(y), axis=0)
+# 	E2 = np.mean(y ** 2, axis=0)
 #
-# 		return -1 * np.sqrt(N) * (p1 + p2)
+# 	p1 = np.mean(np.sign(y) * X, axis=0).T / np.sqrt(E2)
+# 	p2 = -1 * E1 / ((E2) ** (3 / 2)) * np.mean(y * X, axis=0).T
 #
+# 	return -1 * np.sqrt(N) * (p1 + p2)
 #
-# 	def l1_l2_hessian(X, w, y):
-# 		pass
 #
+# def l1_l2_hessian(X, w, y):
+# 	pass
+
+
+# test_instance = user_cost(use_hessian=False)
+# test_instance = NegentropyCost(source_name='exp', source_params={'alpha': 1})
+
+# test_instance.set_cost(l1_l2_norm)
+# test_instance.set_gradient(l1_l2_grad)
 #
-# 	test_instance = user_cost(use_hessian=False)
-#
-# 	test_instance.set_cost(l1_l2_norm)
-# 	test_instance.set_gradient(l1_l2_grad)
-#
-# 	Lw = 256
-# 	X_ = np.random.randn(1000, Lw)
-# 	w_ = np.random.randn(Lw, 1)
-# 	y_ = X_ @ w_
+# Lw = 256
+# X_ = np.random.randn(1000, Lw)
+# w_ = np.random.randn(Lw, 1)
+# y_ = X_ @ w_
 #
-# 	grad_tup = test_instance.check_gradient(X_, w_, y_, 1e-4)
+# res_grad = test_instance.check_gradient(X_, w_, y_, 1e-4)
+# res_hess = test_instance.check_gradient(X_, w_, y_, 1e-4)
```

### Comparing `spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/helper_methods.py` & `spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/helper_methods.py`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/negen_approx.py` & `spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/negen_approx.py`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/spectral_constraint.py` & `spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/spectral_constraint.py`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.2/spectrally_constrained_LVMs/spectrally_constrained_model.py` & `spectrally_constrained_lvms-0.1.3/spectrally_constrained_LVMs/spectrally_constrained_model.py`

 * *Files identical despite different names*

### Comparing `spectrally_constrained_lvms-0.1.2/PKG-INFO` & `spectrally_constrained_lvms-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spectrally-constrained-lvms
-Version: 0.1.2
+Version: 0.1.3
 Summary: An optimisation implementation of linear transforms with a spectral constraint.
 Home-page: https://github.com/RyanBalshaw/spectrally-constrained-LVMs
 License: MIT
 Keywords: Linear LVMs,spectral constraint,PCA,ICA
 Author: Ryan Balshaw
 Author-email: ryanbalshaw81@gmail.com
 Maintainer: Ryan Balshaw
@@ -33,15 +33,15 @@
 ![GitHub license](https://img.shields.io/github/license/RyanBalshaw/spectrally-constrained-LVMs)
 ![GitHub last commit](https://img.shields.io/github/last-commit/RyanBalshaw/spectrally-constrained-LVMs)
 ![PyPI](https://img.shields.io/pypi/v/spectrally-constrained-lvms)
 ![PyPI - Wheel](https://img.shields.io/pypi/wheel/spectrally-constrained-lvms?color=blueviolet)
 ![Read the Docs](https://img.shields.io/readthedocs/spectrally-constrained-lvms?color=informational)
 ![GitHub issues](https://img.shields.io/github/issues/RyanBalshaw/spectrally-constrained-LVMs?color=critical)
 
-*Current version:* 0.1.2
+*Current version:* 0.1.3
 
 Spectrally-constrained-LVMs is a Python-based package which facilitates the estimation of the linear latent variable model (LVM) parameters with a unique spectral constraint in single-channel time-series applications.
 
 ## Purpose
 LVMs are a statistical methodology which tries to capture the underlying structure in some observed data. This package caters to single channel time-series applications and provides a methodology to estimate the LVM parameters. The model parameters are encouraged to be diverse via a spectral constraint which enforces non-duplication of the spectral information captured by the latent sources.
 
 The purpose of this package is to provide a complete methodology that caters to a variety of LVM objective functions.
```


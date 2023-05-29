# Comparing `tmp/invopt-0.0.4.tar.gz` & `tmp/invopt-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invopt-0.0.4.tar", last modified: Wed May 24 15:45:54 2023, max compression
+gzip compressed data, was "invopt-0.0.5.tar", last modified: Mon May 29 16:11:12 2023, max compression
```

## Comparing `invopt-0.0.4.tar` & `invopt-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 15:45:54.322594 invopt-0.0.4/
--rw-rw-rw-   0        0        0     1099 2023-05-01 20:52:18.000000 invopt-0.0.4/LICENSE.txt
--rw-rw-rw-   0        0        0     3944 2023-05-24 15:45:54.322594 invopt-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3354 2023-05-24 15:40:37.000000 invopt-0.0.4/README.md
--rw-rw-rw-   0        0        0      712 2023-05-24 09:24:06.000000 invopt-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 15:45:54.322594 invopt-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-24 15:45:54.290927 invopt-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 15:45:54.309587 invopt-0.0.4/src/invopt/
--rw-rw-rw-   0        0        0      388 2023-05-24 15:25:36.000000 invopt-0.0.4/src/invopt/__init__.py
--rw-rw-rw-   0        0        0    53495 2023-05-24 15:21:47.000000 invopt-0.0.4/src/invopt/main.py
-drwxrwxrwx   0        0        0        0 2023-05-24 15:45:54.322594 invopt-0.0.4/src/invopt.egg-info/
--rw-rw-rw-   0        0        0     3944 2023-05-24 15:45:54.000000 invopt-0.0.4/src/invopt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-05-24 15:45:54.000000 invopt-0.0.4/src/invopt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 15:45:54.000000 invopt-0.0.4/src/invopt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-24 15:45:54.000000 invopt-0.0.4/src/invopt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 15:45:54.000000 invopt-0.0.4/src/invopt.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 15:45:54.322594 invopt-0.0.4/tests/
--rw-rw-rw-   0        0        0     1681 2023-05-24 15:26:39.000000 invopt-0.0.4/tests/test_examples.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:11:12.618957 invopt-0.0.5/
+-rw-rw-rw-   0        0        0     1099 2023-05-01 20:52:18.000000 invopt-0.0.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     4244 2023-05-29 16:11:12.618957 invopt-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3654 2023-05-29 12:49:44.000000 invopt-0.0.5/README.md
+-rw-rw-rw-   0        0        0      712 2023-05-27 14:30:44.000000 invopt-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 16:11:12.634583 invopt-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 16:11:12.583800 invopt-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 16:11:12.588815 invopt-0.0.5/src/invopt/
+-rw-rw-rw-   0        0        0      518 2023-05-27 14:51:04.000000 invopt-0.0.5/src/invopt/__init__.py
+-rw-rw-rw-   0        0        0    59212 2023-05-29 15:50:10.000000 invopt-0.0.5/src/invopt/main.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:11:12.618957 invopt-0.0.5/src/invopt.egg-info/
+-rw-rw-rw-   0        0        0     4244 2023-05-29 16:11:12.000000 invopt-0.0.5/src/invopt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-29 16:11:12.000000 invopt-0.0.5/src/invopt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 16:11:12.000000 invopt-0.0.5/src/invopt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-29 16:11:12.000000 invopt-0.0.5/src/invopt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 16:11:12.000000 invopt-0.0.5/src/invopt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 16:11:12.618957 invopt-0.0.5/tests/
+-rw-rw-rw-   0        0        0     1974 2023-05-27 14:54:17.000000 invopt-0.0.5/tests/test_examples.py
```

### Comparing `invopt-0.0.4/LICENSE.txt` & `invopt-0.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `invopt-0.0.4/PKG-INFO` & `invopt-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invopt
-Version: 0.0.4
+Version: 0.0.5
 Summary: Inverse Optimization with Python
 Author-email: Pedro Zattoni Scroccaro <pedroszattoni@gmail.com>
 Project-URL: Homepage, https://github.com/pedroszattoni/invopt
 Project-URL: Bug Tracker, https://github.com/pedroszattoni/inverse-optimization/issues
 Keywords: inverse-optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,37 +12,44 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # InvOpt: Inverse Optimization with Python
 
-InvOpt is a Python package for solving Inverse Optimization (IO) problems. In IO problems, our goal is to model the behavior of an expert agent, which given an exogenous signal, returns a response action. The underlying assumption of IO is that to compute its response, the expert agent solves an optimization problem parametric in the exogenous signal. We assume to know the constraints imposed on the expert, but not its cost function. Therefore, our goal is to model the cost function being optimized by the expert, using examples of exogenous signals and corresponding expert response actions. More concretely, given a dataset $\mathcal{D} = \\{(\hat{s}_ i, \hat{x}_ i)\\}_ {i=1}^N$ of exogenous signals $\hat{s}_ i$ and the respective expert's response $\hat{x}_ i$, our goal is to find a cost vector $\theta \in \mathbb{R}^p$ such that the **Forward Optimization Problem (FOP)** with feature mapping $\phi$
-$$x_i \in \arg\min_ {x \in \mathbb{X}(\hat{s}_ i)} \ \theta^\top \phi(\hat{s}_ i,x)$$ reproduces (or in some sense approximates) the expert's action $\hat{x}_ i$. For a more detailed description of the IO problem and its modelling, please refer to [Zattoni Scroccaro et al. (2023)](https://arxiv.org/abs/2305.07730) and the references therein. 
+InvOpt is an open-source Python package for solving Inverse Optimization (IO) problems. In IO problems, our goal is to model the behavior of an expert agent, which given an exogenous signal, returns a response action. The underlying assumption of IO is that to compute its response, the expert agent solves an optimization problem parametric in an exogenous signal. We assume to know the constraints imposed on the expert, but not its cost function. Therefore, using examples of exogenous signals and corresponding expert response actions, our goal is to model the cost function being optimized by the expert. More concretely, given a dataset $\mathcal{D} = \\{(\hat{s}_ i, \hat{x}_ i)\\}_ {i=1}^N$ of exogenous signals $\hat{s}_ i$ and the respective expert's response $\hat{x}_ i$, feature mapping $\phi$, our goal is to find a cost vector $\theta \in \mathbb{R}^p$ such that a minimizer $x_ i$ of the **Forward Optimization Problem (FOP)**
+
+$$
+x_i \in \arg\min_ {x \in \mathbb{X}(\hat{s}_ i)} \ \langle \theta,\phi(\hat{s}_ i,x) \rangle
+$$
+
+reproduces (or in some sense approximates) the expert's action $\hat{x}_ i$. For a more detailed description of IO problems and their modeling, please refer to [Zattoni Scroccaro et al. (2023)](https://arxiv.org/abs/2305.07730) and the references therein. 
 
 ## Installation
 
 ```bash
 pip install invopt
 ```
-InvOpt depends on NumPy. Moreover, some of its functions also depend on gurobipy or cvxpy. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
+InvOpt depends on `numpy`. Moreover, some of its functions also depend on `gurobipy` or `cvxpy`. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
 
 ## Usage and examples
 
-The following functions are available in the InvOpt package to solving IO problems:
+The following functions are available in the InvOpt package:
 
-- [`discrete_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
+- [`discrete_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent): for FOPs with discrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
 - [`discrete`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete): for FOPs with dicrete decision spaces (e.g., binary).
+- [`continuous_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/continuous_linear): for continuous, linear FOPs.
+- [`continuous_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/continuous_quadratic): for continuous, quadratic FOPs.
 - [`mixed_integer_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
 - [`mixed_integer_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
 - [`FOM`](https://github.com/pedroszattoni/invopt/tree/main/examples/FOM): for general FOPs. Solves IO problem approximately using first-order methods.
 
 ## Contributing
 
-Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains a number of ideas to possibly improve the InvOpt package.
+Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains some ideas to possibly improve the InvOpt package.
 
 ## Citing
 If you use InvOpt for research, please cite our accompanying paper:
 
 ```bibtex
 @article{zattoniscroccaro2023learning,
   title={Learning in Inverse Optimization: Incenter Cost, Augmented Suboptimality Loss, and Algorithms},
```

### Comparing `invopt-0.0.4/README.md` & `invopt-0.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,40 @@
 
 # InvOpt: Inverse Optimization with Python
 
-InvOpt is a Python package for solving Inverse Optimization (IO) problems. In IO problems, our goal is to model the behavior of an expert agent, which given an exogenous signal, returns a response action. The underlying assumption of IO is that to compute its response, the expert agent solves an optimization problem parametric in the exogenous signal. We assume to know the constraints imposed on the expert, but not its cost function. Therefore, our goal is to model the cost function being optimized by the expert, using examples of exogenous signals and corresponding expert response actions. More concretely, given a dataset $\mathcal{D} = \\{(\hat{s}_ i, \hat{x}_ i)\\}_ {i=1}^N$ of exogenous signals $\hat{s}_ i$ and the respective expert's response $\hat{x}_ i$, our goal is to find a cost vector $\theta \in \mathbb{R}^p$ such that the **Forward Optimization Problem (FOP)** with feature mapping $\phi$
-$$x_i \in \arg\min_ {x \in \mathbb{X}(\hat{s}_ i)} \ \theta^\top \phi(\hat{s}_ i,x)$$ reproduces (or in some sense approximates) the expert's action $\hat{x}_ i$. For a more detailed description of the IO problem and its modelling, please refer to [Zattoni Scroccaro et al. (2023)](https://arxiv.org/abs/2305.07730) and the references therein. 
+InvOpt is an open-source Python package for solving Inverse Optimization (IO) problems. In IO problems, our goal is to model the behavior of an expert agent, which given an exogenous signal, returns a response action. The underlying assumption of IO is that to compute its response, the expert agent solves an optimization problem parametric in an exogenous signal. We assume to know the constraints imposed on the expert, but not its cost function. Therefore, using examples of exogenous signals and corresponding expert response actions, our goal is to model the cost function being optimized by the expert. More concretely, given a dataset $\mathcal{D} = \\{(\hat{s}_ i, \hat{x}_ i)\\}_ {i=1}^N$ of exogenous signals $\hat{s}_ i$ and the respective expert's response $\hat{x}_ i$, feature mapping $\phi$, our goal is to find a cost vector $\theta \in \mathbb{R}^p$ such that a minimizer $x_ i$ of the **Forward Optimization Problem (FOP)**
+
+$$
+x_i \in \arg\min_ {x \in \mathbb{X}(\hat{s}_ i)} \ \langle \theta,\phi(\hat{s}_ i,x) \rangle
+$$
+
+reproduces (or in some sense approximates) the expert's action $\hat{x}_ i$. For a more detailed description of IO problems and their modeling, please refer to [Zattoni Scroccaro et al. (2023)](https://arxiv.org/abs/2305.07730) and the references therein. 
 
 ## Installation
 
 ```bash
 pip install invopt
 ```
-InvOpt depends on NumPy. Moreover, some of its functions also depend on gurobipy or cvxpy. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
+InvOpt depends on `numpy`. Moreover, some of its functions also depend on `gurobipy` or `cvxpy`. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
 
 ## Usage and examples
 
-The following functions are available in the InvOpt package to solving IO problems:
+The following functions are available in the InvOpt package:
 
-- [`discrete_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
+- [`discrete_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent): for FOPs with discrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
 - [`discrete`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete): for FOPs with dicrete decision spaces (e.g., binary).
+- [`continuous_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/continuous_linear): for continuous, linear FOPs.
+- [`continuous_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/continuous_quadratic): for continuous, quadratic FOPs.
 - [`mixed_integer_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
 - [`mixed_integer_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
 - [`FOM`](https://github.com/pedroszattoni/invopt/tree/main/examples/FOM): for general FOPs. Solves IO problem approximately using first-order methods.
 
 ## Contributing
 
-Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains a number of ideas to possibly improve the InvOpt package.
+Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains some ideas to possibly improve the InvOpt package.
 
 ## Citing
 If you use InvOpt for research, please cite our accompanying paper:
 
 ```bibtex
 @article{zattoniscroccaro2023learning,
   title={Learning in Inverse Optimization: Incenter Cost, Augmented Suboptimality Loss, and Algorithms},
```

### Comparing `invopt-0.0.4/pyproject.toml` & `invopt-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "invopt"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Pedro Zattoni Scroccaro", email="pedroszattoni@gmail.com" },
 ]
 description = "Inverse Optimization with Python"
 readme = "README.md"
 keywords = ["inverse-optimization"]
 requires-python = ">=3.7"
```

### Comparing `invopt-0.0.4/src/invopt/main.py` & `invopt-0.0.5/src/invopt/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,17 +13,17 @@
     if Theta not in [None, 'nonnegative']:
         raise Exception('Invalid Theta. Accepted values are: None (default) '
                         'and \'nonnegative\'.')
 
 
 def check_decision_space(decision_space):
     """Check if decision_space is valid."""
-    if decision_space[0] != 'binary':
+    if decision_space != 'binary':
         raise Exception('Invalid decision space. Accepted values are: ' +
-                        ' tuple(\'binary\', n) (default).')
+                        '\'binary\'.')
 
 
 def check_regularizer(regularizer):
     """Check if regularizer is valid."""
     if regularizer not in ['L2_squared', 'L1']:
         raise Exception('Invalid regularizer. Accepted values are:' +
                         ' \'L2_squared\' (default) and \'L1\'.')
@@ -31,42 +31,39 @@
 
 def check_reg_parameter(reg_param):
     """Check if reg_param is valid."""
     if reg_param < 0:
         raise Exception('reg_param must be nonnegative.')
 
 
-def check_dist_func(dist_func, sub_loss):
-    """Check if dist_func is given when sub_loss=False."""
-    if (not sub_loss) and (dist_func is None):
-        raise Exception('dist_func required when sub_loss=False.')
-
-
-def warning_large_decision_space(decision_space):
+def warning_large_decision_space(decision_space, n):
     """Warn user if decision space is binary and high-dimensional."""
-    if (decision_space[0] == 'binary') and (decision_space[1] > 15):
-        warnings.warn('Attention! Using this IO method for models with binary '
+    if (decision_space == 'binary') and (n > 15):
+        warnings.warn('Attention! Using this function for FOPs with binary '
                       'decision variables requires solving an optimization '
                       'problem with potentially O(N*2^n) constraints, '
                       'where N is the number of training examples and n is '
                       'the dimension of the binary decision vector.')
 
 
-def warning_dist_func_sub_loss(dist_func, sub_loss):
-    """Warn user dist_func is not used when sub_loss=True."""
-    if sub_loss and (dist_func is not None):
-        warnings.warn('dist_func is not used when sub_loss=True.')
-
-
 def warning_theta_hat_reg_param(theta_hat, reg_param):
     """Warn user theta_hat is not used when reg_param=0."""
     if (theta_hat is not None) and (reg_param == 0):
         warnings.warn('theta_hat is not used when reg_param=0.')
 
 
+def warning_add_dist_func_y(add_dist_func_y):
+    """Warn user that add_dist_func_y increases the size of the problem."""
+    if add_dist_func_y:
+        warnings.warn('Setting add_dist_func_y=True increases the number of '
+                      'constraints of the IO problem by a factor of 2n, '
+                      'where n is the dimension of the continuous part of '
+                      'the decision vector.')
+
+
 def normalize(vec, norm):
     """
     Normalize nonzero array according to some norm.
 
     Parameters
     ----------
     vec : 1D ndarray
@@ -86,17 +83,17 @@
         vec = vec/norm_vec
     return vec
 
 
 def ASL(theta, dataset, FOP_aug, phi, dist_func,
         regularizer='L2_squared',
         reg_param=0,
-        theta_hat=0):
+        theta_hat=None):
     """
-    Evaluate augmented suboptimality loss.
+    Evaluate Augmented Suboptimality loss.
 
     Parameters
     ----------
     theta : 1D ndarray
         Cost vector.
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
@@ -114,17 +111,16 @@
         between them according to some distance metric.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     reg_param : float, optional
         Nonnegative regularization parameter. The default is 0.
     theta_hat : {1D ndarray, None}, optional
-        A priory belief or estimate of the true cost vector. When
-        theta_hat=None, it is defined as the vector of zeros. The default is
-        None.
+        A priory belief or estimate of the true cost vector theta. The default
+        is None.
 
     Raises
     ------
     Exception
         If invalid regularization parameter. If negative regularization
         parameter.
 
@@ -217,15 +213,15 @@
     scale_obj_diff : bool, optional
         When theta_true is given, scale objective value difference using
         theta_true. The default is True.
 
     Raises
     ------
     Exception
-        If theta_true is given but phi function is not.
+        If theta_true is given but the phi function is not.
 
     Returns
     -------
     results : {float, tuple(float, float, float)}
         Returns the average response difference. If true_theta is given, also
         returns the average objective value difference and cost vector
         difference as a tuple.
@@ -268,108 +264,91 @@
         results = (x_diff_avg, obj_diff_avg, theta_diff)
     else:
         results = x_diff_avg
 
     return results
 
 
-def discrete_consistent(dataset, decision_space, phi,
-                        X=None,
+def discrete_consistent(dataset, X, phi,
                         dist_func=None,
                         Theta=None,
                         regularizer='L2_squared',
                         theta_hat=None,
-                        feasibility=False,
                         verbose=False,
                         gurobi_params=None):
     """
-    Inverse optimization for discrete models with consistent data.
+    Inverse optimization for discrete FOPs with consistent data.
 
-    Uses incenter (default) or feasibility strategy. For more details, see
+    For more details, see
     https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
+    X : tuple(str, int, {callable, None})
+        Constraint set. Given a signal s and response x, X is a tuple
+        containing the type of the decision space, the size of the decision
+        space, and any extra constraints as an indicator function. For example,
+        if the decision vector is binary, with size n, and respects the
+        constraint Ax <= b., then X = ('binary', n, ind_func), where
+        ind_func(s, x) equals True if Ax <= b, and False otherwise. Notice that
+        A and b may be part of the signal s, which is why the indicator
+        function takes both s and x as inputs. If ind_func=None, it will be
+        defined as "def ind_func(s, x): return True".
     phi : callable
         Feature function. Given a signal s and response x, returns a 1D
         ndarray feature vector. Syntax: phi(s, x).
-    decision_space : {tuple('binary', n)}
-        Tuple containing type and dimension of the decision space.
-    X : {callable, None}, optional
-        Constraint set. Given a signal s and response x, returns True if x is a
-        feasible response, and False otherwise. It does not need to check for
-        the type of the decision variables contained in decision_space. For
-        example, if decision_space=('binary', n), X should not check if x is a
-        binary vector. Syntax: X(s, x). If None, it will be defined as
-        "def X(s, x): return True". The default is None.
     dist_func : {callable, None}, optional
-        Distance function. Given two responses x1 and x2, returns the distance
-        between them according to some distance metric. Not required when
-        using the feasibility strategy. Syntax: dist_func(x1, x2). The default
-        is None.
+        Distance penalization function. Given two responses x1 and x2, returns
+        the distance between them according to some distance metric. Syntax:
+        dist_func(x1, x2). The default is None.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     theta_hat : {1D ndarray, None}, optional
-        A priory belief or estimate of the true cost vector. The default is
-        None.
-    feasibility : bool, optional
-        If True, solve problem using the feasibility strategy. Namely, if
-        theta_hat=None, we search over the facets of the unit L-infinity sphere
-        until a feasible cost vector is found. If Theta='nonnegative', only
-        searches over the nonnegative facet of the L-1 sphere. If False, solve
-        the problem using the Incenter strategy. The default is False.
+        A priory belief or estimate of the true cost vector theta. The default
+        is None.
     verbose : bool, optional
         If True, print Gurobi's solver output. The default is False.
     gurobi_params : {list of tuple(str, value), None}, optional
         List of tuples with Gurobi's parameter name and value. For example,
         [('TimeLimit', 0.5), ('Method', 2)]. The default is None.
 
     Raises
     ------
     Exception
         If unsupported Theta, regularizer, or decision_space. If Gurobi does
-        not find an optimal solution. If feasibility=True and theta_hat is not
-        None. If feasibility=False, theta_hat is None and dist_func is None.
+        not find an optimal solution.
 
     Returns
     -------
     theta_opt : 1D ndarray
-        An optimal cost vector according to the chosen strategy.
+        An optimal cost vector.
 
     """
-    try:
-        import gurobipy as gp
-    except ImportError:
-        print("gurobipy is required for invopt's discrete_consistent " +
-              "function.")
+    import gurobipy as gp
+
+    decision_space, n, ind_func = X
 
     # Check if the inputs are valid
     check_Theta(Theta)
     check_decision_space(decision_space)
     check_regularizer(regularizer)
 
-    warning_large_decision_space(decision_space)
-
-    if (dist_func is None) and (not feasibility):
-        raise Exception('dist_func required when feasibility=False.')
+    warning_large_decision_space(decision_space, n)
 
-    if (dist_func is not None) and feasibility:
-        warnings.warn('dist_func not used when feasibility=True.')
-
-    if X is None:
-        def X(s, x): return True
+    if ind_func is None:
+        def ind_func(s, x): return True
 
     N = len(dataset)
 
-    # Sample signal and response to get dimension of the cost vector
+    # Sample a signal and response to get the dimension of the cost vector
     s_test, x_test = dataset[0]
     p = len(phi(s_test, x_test))
 
     # Initialize Gurobi model
     mdl = gp.Model()
     if not verbose:
         mdl.setParam('OutputFlag', 0)
@@ -381,29 +360,28 @@
 
     if Theta == 'nonnegative':
         mdl.addConstrs(theta[i] >= 0 for i in range(p))
 
     # Add constraints
     for i in range(N):
         s_hat, x_hat = dataset[i]
-        if decision_space[0] == 'binary':
-            n = decision_space[1]
+        if decision_space == 'binary':
             for k in range(2**n):
                 x = dec_to_bin(k, n)
-                if X(s_hat, x):
+                if ind_func(s_hat, x):
                     phi_1 = phi(s_hat, x)
                     phi_2 = phi(s_hat, x_hat)
-                    if feasibility:
+                    if dist_func is None:
                         dist = 0
                     else:
                         dist = dist_func(x_hat, x)
                     mdl.addConstr(gp.quicksum(theta[j]*(phi_1[j] - phi_2[j])
                                               for j in range(p)) >= dist)
 
-    if feasibility and (theta_hat is None):
+    if (dist_func is None) and (theta_hat is None):
         if Theta == 'nonnegative':
             mdl.addConstr(gp.quicksum(theta) == 1)
             mdl.optimize()
         else:
             # Search over facets of unit L-infinity sphere for a feasible
             # solution.
             for i in range(p):
@@ -438,578 +416,768 @@
                         f'= {mdl.status}. Set the flag verbose=True for more '
                         'details. The optimization problem will '
                         'always be infeasible if the data is not consistent.')
 
     return theta_opt
 
 
-def discrete(dataset, decision_space, phi,
-             X=None,
+def discrete(dataset, X, phi,
              dist_func=None,
              Theta=None,
              regularizer='L2_squared',
              reg_param=0,
              theta_hat=None,
-             sub_loss=False,
              verbose=False,
              gurobi_params=None):
     """
-    Inverse optimization for discrete models.
+    Inverse optimization for discrete FOPs.
 
     For more details, see
     https://github.com/pedroszattoni/invopt/tree/main/examples/discrete
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
+    X : tuple(str, int, {callable, None})
+        Constraint set. Given a signal s and response x, X is a tuple
+        containing the type of the decision space, the size of the decision
+        space, and any extra constraints as an indicator function. For example,
+        if the decision vector is binary, with size n, and respects the
+        constraint Ax <= b., then X = ('binary', n, ind_func), where
+        ind_func(s, x) equals True if Ax <= b, and False otherwise. Notice that
+        A and b may be part of the signal s, which is why the indicator
+        function takes both s and x as inputs. If ind_func=None, it will be
+        defined as "def ind_func(s, x): return True".
     phi : callable
         Feature function. Given a signal s and response x, returns a 1D
         ndarray feature vector. Syntax: phi(s, x).
-    decision_space : {tuple('binary', n)}
-        Tuple containing type and dimension of the decision space.
-    X : {callable, None}, optional
-        Constraint set. Given a signal s and response x, returns True if x is a
-        feasible response, and False otherwise. It does not need to check for
-        the type of the decision variables contained in decision_space. For
-        example, if decision_space=('binary', n), X should not check if x is a
-        binary vector. Syntax: X(s, x). If None, it will be defined as
-        "def X(s, x): return True". The default is None.
     dist_func : {callable, None}, optional
-        Distance function. Given two responses x1 and x2, returns the distance
-        between them according to some distance metric. Not required when
-        sub_loss=True. Syntax: dist_func(x1, x2). The default is None.
+        Distance penalization function. Given two responses x1 and x2, returns
+        the distance between them according to some distance metric. Syntax:
+        dist_func(x1, x2). The default is None.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     reg_param : float, optional
         Nonnegative regularization parameter. The default is 0.
     theta_hat : {1D ndarray, None}, optional
-        A priory belief or estimate of the true cost vector. When
-        theta_hat=None, it is defined as the vector of zeros. The default is
-        None.
-    sub_loss : bool, optional
-        If True, solve the problem using the Suboptimality loss. Namely,
-        searches over the facts of the unit L-infinity sphere for the cost
-        vector with the smallest loss. If Theta='nonnegative', only searches
-        over the nonnegative facet of the L-1 sphere. If False, solve the
-        problem using the Augmented Suboptimality loss. The default is False.
+        A priory belief or estimate of the true cost vector theta. The default
+        is None.
     verbose : bool, optional
         If True, print Gurobi's solver output. The default is False.
     gurobi_params : {list of tuple(str, value), None}, optional
         List of tuples with Gurobi's parameter name and value. For example,
         [('TimeLimit', 0.5), ('Method', 2)]. The default is None.
 
     Raises
     ------
     Exception
         If unsupported Theta, regularizer, or decision_space. If Gurobi does
-        not find an optimal solution. If sub_loss=False and dist_func is None.
+        not find an optimal solution.
 
     Returns
     -------
     theta_opt : 1D ndarray
-        An optimal cost vector according to the chosen strategy.
+        An optimal cost vector.
 
     """
-    _, n = decision_space
+    _, n, _ = X
 
     if theta_hat is None:
         theta_hat_mod = None
     else:
-        theta_hat_mod = (np.zeros((1, 1)), theta_hat)
+        theta_hat_mod = np.concatenate(([0], theta_hat))
 
     dataset_mod = []
     for data in dataset:
-        w_hat, z_hat = data
-        s_hat = (np.zeros((1, 1)), np.zeros((1, n)), np.array([0]), w_hat)
-        x_hat = (np.array([0]), z_hat)
-        dataset_mod.append((s_hat, x_hat))
+        s_hat, x_hat = data
+        s_hat_mod = (np.zeros((1, 1)),
+                     np.zeros((1, n)),
+                     np.array([0]),
+                     s_hat)
+        x_hat_mod = (np.array([0]), x_hat)
+        dataset_mod.append((s_hat_mod, x_hat_mod))
 
-    theta_opt_mod = mixed_integer_linear(dataset_mod, decision_space,
+    theta_opt_mod = mixed_integer_linear(dataset_mod, X,
                                          phi2=phi,
-                                         Z=X,
                                          dist_func_z=dist_func,
                                          Theta=Theta,
                                          regularizer=regularizer,
                                          reg_param=reg_param,
                                          theta_hat=theta_hat_mod,
-                                         sub_loss=sub_loss,
                                          verbose=verbose,
                                          gurobi_params=gurobi_params)
 
     theta_opt = theta_opt_mod[1:]
 
     return theta_opt
 
 
-def mixed_integer_linear(dataset, decision_space,
+def continuous_linear(dataset, phi1,
+                      add_dist_func_y=False,
+                      Theta=None,
+                      regularizer='L2_squared',
+                      reg_param=0,
+                      theta_hat=None,
+                      verbose=False,
+                      gurobi_params=None):
+    """
+    Inverse optimization for continuous linear FOPs.
+
+    For more details, see
+    https://github.com/pedroszattoni/invopt/tree/main/examples/continuous_linear
+
+    Parameters
+    ----------
+    dataset : list of tuples
+        List of tuples (s, x), where s is the signal and x is the response.
+    phi : callable
+        Feature function. Given a signal s and response x, returns a 1D
+        ndarray feature vector. Syntax: phi(s, x).
+    add_dist_func_y: bool, optional
+        If True, adds l-infinity distance penalization to the continuous part
+        or response vector. The default is 'None'.
+    Theta : {None, 'nonnegative'}, optional
+        Constraints on cost vector theta. The default is None.
+    regularizer : {'L2_squared', 'L1'}, optional
+        Type of regularization on cost vector theta. The default is
+        'L2_squared'.
+    reg_param : float, optional
+        Nonnegative regularization parameter. The default is 0.
+    theta_hat : {1D ndarray, None}, optional
+        A priory belief or estimate of the true cost vector theta=vec(Q). The
+        default is None.
+    verbose : bool, optional
+        If True, print Gurobi's solver output. The default is False.
+    gurobi_params : {list of tuple(str, value), None}, optional
+        List of tuples with Gurobi's parameter name and value. For example,
+        [('TimeLimit', 0.5), ('Method', 2)]. The default is None.
+
+    Raises
+    ------
+    Exception
+        If unsupported Theta or regularizer. If Gurobi does not find an optimal
+        solution.
+
+    Returns
+    -------
+    theta_opt : 1D ndarray
+        An optimal cost vector in the form theta = Q.flatten('F')
+
+    """
+    Z = ('binary', 0, None)
+
+    if theta_hat is None:
+        theta_hat_mod = None
+    else:
+        theta_hat_mod = np.concatenate((theta_hat, [0]))
+
+    dataset_mod = []
+    for data in dataset:
+        s_hat, x_hat = data
+        A, b, w = s_hat
+        s_hat_mod = (A, np.zeros((len(b), 1)), b, w)
+        x_hat_mod = (x_hat, np.array([0]))
+        dataset_mod.append((s_hat_mod, x_hat_mod))
+
+    def phi1_mod(w, z): return phi1(w)
+
+    theta_opt_mod = mixed_integer_linear(dataset_mod, Z,
+                                         add_dist_func_y=add_dist_func_y,
+                                         phi1=phi1_mod,
+                                         Theta=Theta,
+                                         regularizer=regularizer,
+                                         reg_param=reg_param,
+                                         theta_hat=theta_hat_mod,
+                                         verbose=verbose,
+                                         gurobi_params=gurobi_params)
+
+    theta_opt = theta_opt_mod[:-1]
+
+    return theta_opt
+
+
+def continuous_quadratic(dataset,
+                         phi1=None,
+                         add_dist_func_y=False,
+                         Theta=None,
+                         regularizer='L2_squared',
+                         reg_param=0,
+                         theta_hat=None,
+                         verbose=False):
+    """
+    Inverse optimization for continuous quadratic FOPs.
+
+    For more details, see
+    https://github.com/pedroszattoni/invopt/tree/main/examples/continuous_quadratic
+
+    Parameters
+    ----------
+    dataset : list of tuples
+        List of tuples (s, x), where s is the signal and x is the response.
+    phi1 : {callable, None}, optional
+        Feature function. Given w and response z, returns a 1D
+        ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
+        as "def phi1(w, z): return np.array([0])". The default is None.
+    add_dist_func_y: bool, optional
+        If True, adds l-infinity distance penalization to the continuous part
+        of the response vector. The default is 'None'.
+    Theta : {None, 'nonnegative'}, optional
+        Constraints on cost vector theta. The default is None.
+    regularizer : {'L2_squared', 'L1'}, optional
+        Type of regularization on cost vector theta. The default is
+        'L2_squared'.
+    reg_param : float, optional
+        Nonnegative regularization parameter. The default is 0.
+    theta_hat : {1D ndarray, None}, optional
+        A priory belief or estimate of the true cost vector
+        theta=(vec(Qyy), vec(Q)). The default is None.
+    verbose : bool, optional
+        If True, print the solver's output. The default is False.
+
+    Raises
+    ------
+    Exception
+        If unsupported Theta or regularizer. If Gurobi does not find an optimal
+        solution.
+
+    Returns
+    -------
+    theta_opt : 1D ndarray
+        An optimal cost vector in the form
+        theta = np.concatenate((Qyy.flatten('F'), Q.flatten('F')))
+
+    """
+    Z = ('binary', 0, None)
+
+    if theta_hat is None:
+        theta_hat_mod = None
+    else:
+        theta_hat_mod = np.concatenate((theta_hat, [0]))
+
+    dataset_mod = []
+    for data in dataset:
+        s_hat, x_hat = data
+        A, b, w = s_hat
+        s_hat_mod = (A, np.zeros((len(b), 1)), b, w)
+        x_hat_mod = (x_hat, np.array([0]))
+        dataset_mod.append((s_hat_mod, x_hat_mod))
+
+    def phi1_mod(w, z): return phi1(w)
+
+    theta_opt_mod = mixed_integer_quadratic(dataset_mod, Z,
+                                            phi1=phi1_mod,
+                                            add_dist_func_y=add_dist_func_y,
+                                            Theta=Theta,
+                                            regularizer=regularizer,
+                                            reg_param=reg_param,
+                                            theta_hat=theta_hat_mod,
+                                            verbose=verbose)
+    theta_opt = theta_opt_mod[:-1]
+
+    return theta_opt
+
+
+def mixed_integer_linear(dataset, Z,
                          phi1=None,
                          phi2=None,
-                         Z=None,
+                         add_dist_func_y=False,
                          dist_func_z=None,
                          Theta=None,
                          regularizer='L2_squared',
                          reg_param=0,
                          theta_hat=None,
-                         sub_loss=False,
                          verbose=False,
                          gurobi_params=None):
     """
-    Inverse optimization for linear models with mixed-integer feasible sets.
+    Inverse optimization for mixed-integer FOPs with linear continuous part.
 
     For more details, see
     https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_linear
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
-    decision_space : {tuple('binary', n)}
-        Tuple containing type and dimension of the decision space fo the
-        integer part of the decision vector.
-    Z : {callable, None}, optional
-        Constraint set of the integer part of the decision vector. Given a
-        signal s = (A, B, c, w) and response x = (y, z), returns True if z
-        (i.e., the integer part of x) is a feasible response, and False
-        otherwise. It does not need to check for the type of the decision
-        variables contained in decision_space. For example, if
-        decision_space=('binary', n), Z should not check if z is a binary
-        vector. Syntax: Z(w, z). If None, it will be defined as
-        "def Z(w, x): return True". The default is None.
+    Z : tuple(str, int, {callable, None})
+        Constraint set for the integer part of the decision vector. Given a
+        signal s = (A, B, c, w) and response x = (y, z), Z is a tuple
+        containing the type of the decision space, the size of the decision
+        space, and any extra constraints as an indicator function, all w.r.t.
+        the integer part or the decision vector, i.e., z. For example,
+        if z is binary, with size n, and respects the
+        constraint Dx <= e., then Z = ('binary', n, ind_func), where
+        ind_func(w, z) equals True if Dz <= e, and False otherwise. Notice that
+        D and e may be part of w, which is why the indicator function
+        takes both w and z as inputs. If ind_func=None, it will be defined as
+        "def ind_func(w, z): return True".
     phi1 : {callable, None}, optional
         Feature function. Given w and response z, returns a 1D
         ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
         as "def phi1(w, z): return np.array([0])". The default is None.
     phi2 : {callable, None}, optional
         Feature function. Given w and response z, returns a 1D
         ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
         as "def phi2(w, z): return np.array([0])". The default is None.
+    add_dist_func_y: bool, optional
+        If True, adds l-infinity distance penalization to the continuous part
+        of the response vector. The default is None.
     dist_func_z : {callable, None}, optional
-        Distance function. Given two responses x1=(y1,z1) and x2=(y2,z2),
-        returns the distance of their integer parts according to some distance
-        metric. Not required when sub_loss=True. Syntax: dist_func_z(z1, z2).
-        The default is None.
+        Distance penalization function. Given two responses x1=(y1,z1) and
+        x2=(y2,z2), returns the distance of their integer parts according to
+        some distance metric. Syntax: dist_func_z(z1, z2). The default is None.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     reg_param : float, optional
         Nonnegative regularization parameter. The default is 0.
-    theta_hat : {tuple(2D ndarray, 1D ndarray), None}, optional
+    theta_hat : {1D ndarray, None}, optional
         A priory belief or estimate of the true cost vector theta=(vec(Q), q).
-        Should be provided as a tuple (Q_hat, q_hat). When None, theta_hat is
-        defined as zeros. The default is None.
-    sub_loss : bool, optional
-        If True, solve the problem using the Suboptimality loss. Namely,
-        searches over the facts of the unit L-infinity sphere for the cost
-        vector with the smallest loss. If Theta='nonnegative', only searches
-        over the nonnegative facet of the L-1 sphere. If False, solve the
-        problem using the Augmented Suboptimality loss. The default is False.
+        The default is None.
     verbose : bool, optional
         If True, print Gurobi's solver output. The default is False.
     gurobi_params : {list of tuple(str, value), None}, optional
         List of tuples with Gurobi's parameter name and value. For example,
         [('TimeLimit', 0.5), ('Method', 2)]. The default is None.
 
     Raises
     ------
     Exception
         If unsupported Theta, regularizer, or decision_space. If Gurobi does
-        not find an optimal solution. If sub_loss=False and dist_func is None.
-        If neither phi1 nor phi2 are given.
+        not find an optimal solution. If neither phi1 nor phi2 are given.
 
     Returns
     -------
     theta_opt : 1D ndarray
-        An optimal cost vector according to the chosen strategy.
+        An optimal cost vector in the form
+        theta = np.concatenate((Q.flatten('F'), q))
 
     """
-    try:
-        import gurobipy as gp
-    except ImportError:
-        print("gurobipy is required for invopt's mixed_integer_linear " +
-              'function.')
+    import gurobipy as gp
+
+    decision_space, v, ind_func = Z
 
     # Check if the inputs are valid
     check_Theta(Theta)
     check_decision_space(decision_space)
     check_regularizer(regularizer)
     check_reg_parameter(reg_param)
-    check_dist_func(dist_func_z, sub_loss)
 
     # Warnings
-    warning_large_decision_space(decision_space)
-    warning_dist_func_sub_loss(dist_func_z, sub_loss)
+    warning_large_decision_space(decision_space, v)
     warning_theta_hat_reg_param(theta_hat, reg_param)
+    warning_add_dist_func_y(add_dist_func_y)
 
     if (phi1 is None) and (phi2 is None):
         raise Exception('Either phi1 or phi2 have to be given.')
 
     N = len(dataset)
 
-    if Z is None:
-        def Z(s, z): return True
+    if ind_func is None:
+        def ind_func(w, z): return True
 
+    # Check if phi1 or phi2 were not provided, which means the problem is
+    # purely discrete or continuous, respectively.
+    discrete_flag = False
+    continuous_flag = False
     if phi1 is None:
         def phi1(w, z): return np.array([0])
+        discrete_flag = True
     if phi2 is None:
         def phi2(w, z): return np.array([0])
+        continuous_flag = True
 
-    # Sample signal and response to get dimensions of problem
+    # Sample a signal and response to get the dimensions of the problem
     s_test, x_test = dataset[0]
     A_test, _, _, w_test = s_test
     y_test, z_test = x_test
-    u1 = len(phi1(w_test, z_test))
-    u2 = len(phi2(w_test, z_test))
-    m1, m2 = A_test.shape
+    m = len(phi1(w_test, z_test))
+    r = len(phi2(w_test, z_test))
+    t, u = A_test.shape
 
     # Initialize Gurobi model
     mdl = gp.Model()
     if not verbose:
         mdl.setParam('OutputFlag', 0)
     if gurobi_params is not None:
         for param, value in gurobi_params:
             mdl.setParam(param, value)
 
-    Q = mdl.addVars(m2, u1, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
-    q = mdl.addVars(u2, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
+    Q = mdl.addVars(u, m, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
+    q = mdl.addVars(r, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
     beta = mdl.addVars(N, vtype=gp.GRB.CONTINUOUS)
     sum_beta = (1/N)*gp.quicksum(beta)
 
+    if discrete_flag:
+        mdl.addConstrs(Q[i, j] == 0 for i in range(u) for j in range(m))
+    if continuous_flag:
+        mdl.addConstrs(q[i] == 0 for i in range(r))
+
     if Theta == 'nonnegative':
-        mdl.addConstrs(Q[i, j] >= 0 for i in range(m2) for j in range(u1))
-        mdl.addConstrs(q[i] >= 0 for i in range(u2))
+        mdl.addConstrs(Q[i, j] >= 0 for i in range(u) for j in range(m))
+        mdl.addConstrs(q[i] >= 0 for i in range(r))
 
     for i in range(N):
         s_hat, x_hat = dataset[i]
         y_hat, z_hat = x_hat
         A, B, c, w_hat = s_hat
-        if decision_space[0] == 'binary':
-            n = decision_space[1]
-            for k in range(2**n):
-                z = dec_to_bin(k, n)
-                if Z(w_hat, z):
-                    lamb = mdl.addVars(m1, vtype=gp.GRB.CONTINUOUS)
+        if decision_space == 'binary':
+            for k in range(2**v):
+                z = dec_to_bin(k, v)
+                if ind_func(w_hat, z):
+                    if dist_func_z is None:
+                        dist_z = 0
+                    else:
+                        dist_z = dist_func_z(z_hat, z)
 
-                    if sub_loss:
-                        dist = 0
+                    if add_dist_func_y:
+                        gamma_list = []
+                        for index in range(u):
+                            gamma = np.zeros(u)
+                            gamma[index] = 1
+                            gamma_list.append(gamma)
+                        for index in range(u):
+                            gamma = np.zeros(u)
+                            gamma[index] = -1
+                            gamma_list.append(gamma)
                     else:
-                        dist = dist_func_z(z_hat, z)
+                        gamma_list = [np.zeros(u)]
+
+                    for gamma in gamma_list:
+                        lamb = mdl.addVars(t, vtype=gp.GRB.CONTINUOUS)
 
-                    phi1_hat = phi1(w_hat, z_hat)
-                    phi2_hat = phi2(w_hat, z_hat)
-                    Qphi1 = [gp.quicksum(Q[i, j]*phi1_hat[j]
-                                         for j in range(u1))
-                             for i in range(m2)]
-                    yQphi1 = gp.quicksum(y_hat[j]*Qphi1[j] for j in range(m2))
-                    qphi2_hat = gp.quicksum(q[j]*phi2_hat[j]
-                                            for j in range(u2))
-                    theta_phi = yQphi1 + qphi2_hat
-
-                    Bz = B @ z
-                    lambcBz = gp.quicksum(lamb[j]*(c[j] - Bz[j])
-                                          for j in range(m1))
-                    ph2 = phi2(w_hat, z)
-                    qphi2 = gp.quicksum(q[j]*ph2[j] for j in range(u2))
-
-                    mdl.addConstr(theta_phi + lambcBz - qphi2 + dist
-                                  <= beta[i])
-
-                    ph1 = phi1(w_hat, z)
-                    mdl.addConstrs(gp.quicksum(Q[i, j]*ph1[j]
-                                               for j in range(u1))
-                                   + gp.quicksum(lamb[j]*A[j, i]
-                                                 for j in range(m1))
-                                   == 0 for i in range(m2))
+                        ph1_hat = phi1(w_hat, z_hat)
+                        ph2_hat = phi2(w_hat, z_hat)
+                        Qph1_hat = [gp.quicksum(Q[i, j]*ph1_hat[j]
+                                                for j in range(m))
+                                    for i in range(u)]
+                        yQph1_hat = gp.quicksum(y_hat[j]*Qph1_hat[j]
+                                                for j in range(u))
+                        qphi2_hat = gp.quicksum(q[j]*ph2_hat[j]
+                                                for j in range(r))
+                        theta_phi = yQph1_hat + qphi2_hat
+
+                        Bz = B @ z
+                        lambcBz = gp.quicksum(lamb[j]*(c[j] - Bz[j])
+                                              for j in range(t))
+                        ph2 = phi2(w_hat, z)
+                        qphi2 = gp.quicksum(q[j]*ph2[j] for j in range(r))
+
+                        gammay_hat = gp.quicksum(gamma[j]*y_hat[j]
+                                                 for j in range(u))
+                        mdl.addConstr(theta_phi + lambcBz - qphi2
+                                      + gammay_hat + dist_z <= beta[i])
+
+                        ph1 = phi1(w_hat, z)
+                        mdl.addConstrs(gp.quicksum(Q[i, j]*ph1[j]
+                                                   for j in range(m))
+                                       + gp.quicksum(lamb[j]*A[j, i]
+                                                     for j in range(t))
+                                       + gamma[i]
+                                       == 0 for i in range(u))
 
     if reg_param > 0:
         if theta_hat is None:
-            Q_hat = np.zeros((m2, u1))
-            q_hat = np.zeros(u2)
+            Q_hat = np.zeros((u, m))
+            q_hat = np.zeros(r)
         else:
-            Q_hat, q_hat = theta_hat
+            Q_hat = theta_hat[:-r].reshape((u, m))
+            q_hat = theta_hat[-r:]
 
         if regularizer == 'L2_squared':
-            Q_sum = gp.quicksum((Q[i, j] - Q_hat[i, j])**2 for i in range(m2)
-                                for j in range(u1))
-            q_sum = gp.quicksum((q[i] - q_hat[i])**2 for i in range(u2))
+            Q_sum = gp.quicksum((Q[i, j] - Q_hat[i, j])**2 for i in range(u)
+                                for j in range(m))
+            q_sum = gp.quicksum((q[i] - q_hat[i])**2 for i in range(r))
             reg_term = (reg_param/2)*(Q_sum + q_sum)
         elif regularizer == 'L1':
-            tQ = mdl.addVars(m2, u1, lb=-gp.GRB.INFINITY,
+            tQ = mdl.addVars(u, m, lb=-gp.GRB.INFINITY,
                              vtype=gp.GRB.CONTINUOUS)
-            tq = mdl.addVars(u2, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
+            tq = mdl.addVars(r, lb=-gp.GRB.INFINITY, vtype=gp.GRB.CONTINUOUS)
 
             reg_term = reg_param*(gp.quicksum(tQ) + gp.quicksum(tq))
 
             mdl.addConstrs(Q[i, j] - Q_hat[i, j] <= tQ[i, j]
-                           for i in range(m2) for j in range(u1))
+                           for i in range(u) for j in range(m))
             mdl.addConstrs(Q_hat[i, j] - Q[i, j] <= tQ[i, j]
-                           for i in range(m2) for j in range(u1))
-            mdl.addConstrs(q[i] - q_hat[i] <= tq[i] for i in range(u2))
-            mdl.addConstrs(q_hat[i] - q[i] <= tq[i] for i in range(u2))
+                           for i in range(u) for j in range(m))
+            mdl.addConstrs(q[i] - q_hat[i] <= tq[i] for i in range(r))
+            mdl.addConstrs(q_hat[i] - q[i] <= tq[i] for i in range(r))
     else:
         reg_term = 0
 
     mdl.setObjective(reg_term + sum_beta, gp.GRB.MINIMIZE)
 
-    # Check if norm equality constraint needs to be added to avoid the trivial
-    # solution theta=0
-    if sub_loss and ((reg_param == 0) or (theta_hat is None)):
+    # Check if the norm equality constraint needs to be added to avoid the
+    # trivial solution theta=0
+    if (((not add_dist_func_y) and (dist_func_z is None))
+            and ((reg_param == 0) or (theta_hat is None))):
         if Theta == 'nonnegative':
             mdl.addConstr(gp.quicksum(q) + gp.quicksum(Q) == 1)
             mdl.optimize()
 
             if mdl.status != 2:
                 raise Exception('Optimal solution not found. Gurobi status '
                                 f'code = {mdl.status}. Set the flag '
                                 'verbose=True for more details.')
 
-            Q_opt = np.array([[Q[i, j].X for i in range(m2)]
-                             for j in range(u1)])
-            q_opt = np.array([q[i].X for i in range(u2)])
+            Q_opt = np.array([[Q[i, j].X for i in range(u)]
+                             for j in range(m)])
+            q_opt = np.array([q[i].X for i in range(r)])
         else:
             # Search over facets of unit L-infinity sphere for the solution
             # with the lowest objective value.
             best_obj = np.inf
-            for i in range(u1):
+            for i in range(r):
                 for j in [-1, 1]:
                     cons = mdl.addConstr(q[i] == j)
                     mdl.optimize()
                     mdl.remove(cons)
                     # If an optimal solution was found
                     if mdl.status == 2:
                         obj_val = mdl.objVal
                         if obj_val < best_obj:
                             best_obj = obj_val
-                            Q_opt = np.array([[Q[i, j].X for i in range(m2)]
-                                              for j in range(u1)])
-                            q_opt = np.array([q[i].X for i in range(u2)])
-            for i in range(m2):
-                for k in range(u1):
+                            Q_opt = np.array([[Q[i, j].X for i in range(u)]
+                                              for j in range(m)])
+                            q_opt = np.array([q[i].X for i in range(r)])
+            for i in range(u):
+                for k in range(m):
                     for j in [-1, 1]:
                         cons = mdl.addConstr(Q[i, k] == j)
                         mdl.optimize()
                         mdl.remove(cons)
                         # If an optimal solution was found
                         if mdl.status == 2:
                             obj_val = mdl.objVal
                             if obj_val < best_obj:
                                 best_obj = obj_val
                                 Q_opt = np.array([[Q[i, j].X
-                                                   for i in range(m2)]
-                                                  for j in range(u1)])
-                                q_opt = np.array([q[i].X for i in range(u2)])
+                                                   for i in range(u)]
+                                                  for j in range(m)])
+                                q_opt = np.array([q[i].X for i in range(r)])
     else:
         mdl.optimize()
 
         if mdl.status != 2:
             raise Exception('Optimal solution not found. Gurobi status code '
                             f'= {mdl.status}. Set the flag verbose=True for '
                             'more details.')
 
-        Q_opt = np.array([[Q[i, j].X for i in range(m2)]
-                         for j in range(u1)])
-        q_opt = np.array([q[i].X for i in range(u2)])
+        Q_opt = np.array([[Q[i, j].X for i in range(u)]
+                         for j in range(m)])
+        q_opt = np.array([q[i].X for i in range(r)])
 
     theta_opt = np.concatenate((Q_opt.flatten('F'), q_opt))
     return theta_opt
 
 
-def mixed_integer_quadratic(dataset, decision_space,
+def mixed_integer_quadratic(dataset, Z,
                             phi1=None,
                             phi2=None,
-                            Z=None,
+                            add_dist_func_y=False,
                             dist_func_z=None,
                             Theta=None,
                             regularizer='L2_squared',
                             reg_param=0,
                             theta_hat=None,
-                            sub_loss=False,
-                            verbose=False,
-                            solver='mosek'):
+                            verbose=False):
     """
-    Inverse optimization for quadratic models with mixed-integer feasible sets.
+    Inverse optimization for mixed-integer FOPs with quadratic continuous part.
 
     For more details, see
     https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_quadratic
 
     Parameters
     ----------
     dataset : list of tuples
         List of tuples (s, x), where s is the signal and x is the response.
-    decision_space : {tuple('binary', n)}
-        Tuple containing type and dimension of the decision space.
-    Z : {callable, None}, optional
-        Constraint set of the integer part of the decision vector. Given a
-        signal s = (A, B, c, w) and response x = (y, z), returns True if z
-        (i.e., the integer part of x) is a feasible response, and False
-        otherwise. It does not need to check for the type of the decision
-        variables contained in decision_space. For example, if
-        decision_space=('binary', n), Z should not check if z is a binary
-        vector. Syntax: Z(w, z). If None, it will be defined as
-        "def Z(w, x): return True". The default is None.
+    Z : tuple(str, int, {callable, None})
+        Constraint set for the integer part of the decision vector. Given a
+        signal s = (A, B, c, w) and response x = (y, z), Z is a tuple
+        containing the type of the decision space, the size of the decision
+        space, and any extra constraints as an indicator function, all w.r.t.
+        the integer part or the decision vector, i.e., z. For example,
+        if z is binary, with size n, and respects the
+        constraint Dx <= e., then Z = ('binary', n, ind_func), where
+        ind_func(w, z) equals True if Dz <= e, and False otherwise. Notice that
+        D and e may be part of w, which is why the indicator function
+        takes both w and z as inputs. If ind_func=None, it will be defined as
+        "def ind_func(w, z): return True".
     phi1 : {callable, None}, optional
         Feature function. Given w and response z, returns a 1D
         ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
         as "def phi1(w, z): return np.array([0])". The default is None.
     phi2 : {callable, None}, optional
         Feature function. Given w and response z, returns a 1D
         ndarray feature vector. Syntax: phi1(w, z). If None, it will be defined
         as "def phi2(w, z): return np.array([0])". The default is None.
+    add_dist_func_y: bool, optional
+        If True, adds l-infinity distance penalization to the continuous part
+        of the response vector. The default is None.
     dist_func_z : {callable, None}, optional
-        Distance function. Given two responses x1=(y1,z1) and x2=(y2,z2),
-        returns the distance of their integer parts according to some distance
-        metric. Not required when sub_loss=True. Syntax: dist_func_z(z1, z2).
-        The default is None.
+        Distance penalization function. Given two responses x1=(y1,z1) and
+        x2=(y2,z2), returns the distance of their integer parts according to
+        some distance metric. Syntax: dist_func_z(z1, z2). The default is None.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     reg_param : float, optional
         Nonnegative regularization parameter. The default is 0.
-    theta_hat : {tuple(2D ndarray, 2D ndarray, 1D ndarray), None}, optional
+    theta_hat : {1D ndarray, None}, optional
         A priory belief or estimate of the true cost vector
-        theta=(vec(Qyy), vec(Q), q). Should be provided as a tuple
-        (Qyy_hat, Q_hat, q_hat). When None, theta_hat is defined as zeros. The
-        default is None.
-    sub_loss : bool, optional
-        If True, solve the problem using the Suboptimality loss. Namely,
-        searches over the facts of the unit L-infinity sphere for the cost
-        vector with the smallest loss. If Theta='nonnegative', only searches
-        over the nonnegative facet of the L-1 sphere. If False, solve the
-        problem using the Augmented Suboptimality loss. The default is False.
+        theta=(vec(Qyy), vec(Q), q). The default is None.
     verbose : bool, optional
-        If True, print solver's output. The default is False.
+        If True, print the solver's output. The default is False.
 
     Raises
     ------
     Exception
         If unsupported Theta, regularizer, or decision_space. If Gurobi does
-        not find an optimal solution. If sub_loss=False and dist_func is None.
+        not find an optimal solution.
 
     Returns
     -------
     theta_opt : 1D ndarray
-        An optimal cost vector according to the chosen strategy.
+        An optimal cost vector in the form theta =
+        np.concatenate((Qyy.flatten('F'), Q.flatten('F'), q.flatten('F')))
 
     """
-    try:
-        import cvxpy as cp
-    except ImportError:
-        print("cvxpy is required for invopt's mixed_integer_quadratic " +
-              "function.")
+    import cvxpy as cp
+
+    decision_space, v, ind_func = Z
 
     # Check if the inputs are valid
     check_Theta(Theta)
     check_decision_space(decision_space)
     check_regularizer(regularizer)
     check_reg_parameter(reg_param)
 
     # Warnings
-    warning_large_decision_space(decision_space)
-    warning_dist_func_sub_loss(dist_func_z, sub_loss)
+    warning_large_decision_space(decision_space, v)
     warning_theta_hat_reg_param(theta_hat, reg_param)
+    warning_add_dist_func_y(add_dist_func_y)
 
     N = len(dataset)
 
-    if Z is None:
-        def Z(s, z): return True
+    if ind_func is None:
+        def ind_func(w, z): return True
 
     if phi1 is None:
         def phi1(w, z): return np.array([0])
     if phi2 is None:
         def phi2(w, z): return np.array([0])
 
-    # Sample signal and response to get the the dimensions of the problem
+    # Sample a signal and response to get the dimensions of the problem
     s_test, x_test = dataset[0]
     A_test, _, _, w_test = s_test
     y_test, z_test = x_test
-    u1 = len(phi1(w_test, z_test))
-    u2 = len(phi2(w_test, z_test))
-    m1, m2 = A_test.shape
-
-    Qyy = cp.Variable((m2, m2), symmetric=True)
-    Q = cp.Variable((m2, u1))
-    q = cp.Variable((u2, 1))
+    m = len(phi1(w_test, z_test))
+    r = len(phi2(w_test, z_test))
+    t, u = A_test.shape
+
+    Qyy = cp.Variable((u, u), symmetric=True)
+    Q = cp.Variable((u, m))
+    q = cp.Variable((r, 1))
     beta = cp.Variable(N)
 
     constraints = []
 
     sum_beta = (1/N)*cp.sum(beta)
 
     if Theta == 'nonnegative':
         constraints += [Q >= 0, q >= 0]
 
     for i in range(N):
         s_hat, x_hat = dataset[i]
         y_hat, z_hat = x_hat
         A, B, c, w_hat = s_hat
-        if decision_space[0] == 'binary':
-            n = decision_space[1]
-            for k in range(2**n):
-                z = dec_to_bin(k, n)
-                if Z(w_hat, z):
-                    alpha = cp.Variable((1, 1))
-                    lamb = cp.Variable((m1, 1))
+        if decision_space == 'binary':
+            for k in range(2**v):
+                z = dec_to_bin(k, v)
+                if ind_func(w_hat, z):
+                    if dist_func_z is None:
+                        dist_z = 0
+                    else:
+                        dist_z = dist_func_z(z_hat, z)
 
-                    if sub_loss:
-                        dist = 0
+                    if add_dist_func_y:
+                        gamma_list = []
+                        for index in range(u):
+                            gamma = np.zeros(u)
+                            gamma[index] = 1
+                            gamma_list.append(gamma)
+                        for index in range(u):
+                            gamma = np.zeros(u)
+                            gamma[index] = -1
+                            gamma_list.append(gamma)
                     else:
-                        dist = dist_func_z(z_hat, z)
+                        gamma_list = [np.zeros(u)]
+
+                    for gamma in gamma_list:
+                        alpha = cp.Variable((1, 1))
+                        lamb = cp.Variable((t, 1))
 
-                    theta_phi_hat = (y_hat.T @ Qyy @ y_hat
-                                     + y_hat.T @ Q @ phi1(w_hat, z_hat)
-                                     + q.T @ phi2(w_hat, z_hat))
+                        theta_phi_hat = (y_hat.T @ Qyy @ y_hat
+                                         + y_hat.T @ Q @ phi1(w_hat, z_hat)
+                                         + q.T @ phi2(w_hat, z_hat))
 
-                    lambcBz = lamb.T @ (c - B @ z)
+                        lambcBz = lamb.T @ (c - B @ z)
 
-                    qphi2 = q.T @ phi2(w_hat, z)
+                        qphi2 = q.T @ phi2(w_hat, z)
 
-                    constraints += [theta_phi_hat + alpha + lambcBz - qphi2
-                                    <= beta[i] - dist]
+                        gammay_hat = gamma.T @ y_hat
 
-                    off_diag = Q @ phi1(w_hat, z).reshape((u1, 1)) + A.T @ lamb
-                    constraints += [cp.bmat([[Qyy, off_diag],
-                                             [off_diag.T, 4*alpha]]) >> 0]
-                    constraints += [lamb >= 0]
+                        constraints += [theta_phi_hat + alpha + lambcBz - qphi2
+                                        + gammay_hat + dist_z <= beta[i]]
+
+                        off_diag = (Q @ phi1(w_hat, z).reshape((m, 1))
+                                    + A.T @ lamb + gamma.reshape((u, 1)))
+                        constraints += [cp.bmat([[Qyy, off_diag],
+                                                 [off_diag.T, 4*alpha]]) >> 0]
+                        constraints += [lamb >= 0]
 
     if reg_param > 0:
         if theta_hat is None:
-            Qyy_hat = np.zeros((m2, m2))
-            Q_hat = np.zeros((m2, u1))
-            q_hat = np.zeros((u2, 1))
+            Qyy_hat = np.zeros((u, u))
+            Q_hat = np.zeros((u, m))
+            q_hat = np.zeros((r, 1))
         else:
-            Qyy_hat, Q_hat, q_hat = theta_hat
+            Qyy_hat = theta_hat[:u**2].reshape((u, u))
+            Q_hat = theta_hat[u**2:-r].reshape((u, m))
+            q_hat = theta_hat[-r:].reshape((r, 1))
 
         if regularizer == 'L2_squared':
             Qyy_sum = cp.sum_squares(Qyy - Qyy_hat)
             Q_sum = cp.sum_squares(Q - Q_hat)
             q_sum = cp.sum_squares(q - q_hat)
             reg_term = (reg_param/2)*(Qyy_sum + Q_sum + q_sum)
         elif regularizer == 'L1':
-            tQyy = cp.Variable((m2, m2), symmetric=True)
-            tQ = cp.Variable((m2, u1))
-            tq = cp.Variable((u2, 1))
+            tQyy = cp.Variable((u, u), symmetric=True)
+            tQ = cp.Variable((u, m))
+            tq = cp.Variable((r, 1))
             reg_term = reg_param*(cp.sum(tQyy) + cp.sum(tQ) + cp.sum(tq))
             constraints += [Qyy - Qyy_hat <= tQyy, Qyy_hat - Qyy <= tQyy]
             constraints += [Q - Q_hat <= tQ, Q_hat - Q <= tQ]
             constraints += [q - q_hat <= tq, q_hat - q <= tq]
     else:
         reg_term = 0
 
     obj = cp.Minimize(reg_term + sum_beta)
 
-    # Check if trace equality constraint needs to be added to avoid the trivial
-    # solution theta=0
-    if sub_loss and ((reg_param == 0) or (theta_hat is None)):
+    # Check if the trace equality constraint needs to be added to avoid the
+    # trivial solution theta=0
+    if (((not add_dist_func_y) and (dist_func_z is None))
+            and ((reg_param == 0) or (theta_hat is None))):
         constraints += [cp.trace(Qyy) == 1]
 
     prob = cp.Problem(obj, constraints)
     prob.solve(verbose=verbose)
 
     if prob.status != 'optimal':
         raise Exception('Optimal solution not found. CVXPY status code '
@@ -1058,15 +1226,15 @@
         (augmented) response. When using the Augmented Suboptimality loss,
         an augmented FOP should be used. Syntax: FOP(theta, s), or
         FOP(theta, s, x) for an augmented FOP.
     step_size : callable
         Step-size function. Takes as input the iteration counter t = 0,...,T-1
         and returns the step-size. Syntax: step_size(t).
     T : int
-        Number of iterations the algorithm is run.
+        The number of iterations for the algorithm.
     Theta : {None, 'nonnegative'}, optional
         Constraints on cost vector theta. The default is None.
     step : {'standard', 'exponentiated'}, optional
         Type of update step used for the first-order algorithm. If 'standard',
         uses standard "subgradient method" update steps:
         theta_{t+1} = theta_t - step_size(t)*subgradient. If 'exponentiated',
         uses exponentiated steps:
@@ -1074,16 +1242,15 @@
         'standard'.
     regularizer : {'L2_squared', 'L1'}, optional
         Type of regularization on cost vector theta. The default is
         'L2_squared'.
     reg_param : float, optional
         Nonnegative regularization parameter. The default is 0.
     theta_hat : {1D ndarray, None}, optional
-        A priory belief or estimate of the true cost vector. When
-        theta_hat=None, it is defined as the vector of zeros. The default is
+        A priory belief or estimate of the true cost vector. The default is
         None.
     batch_type : {float, 'reshuffled'}, optional
         If float, it is the fraction of the dataset used to compute stochastic
         subgradients of the loss function, where batch_type=b means use 10*b %
         of the data to compute (stochastic) subgradients. If
         batch_type='reshuffled', T is the number of epochs instead of the
         number of iterations. For each epoch, run the algorithm for N
@@ -1137,16 +1304,16 @@
     warning_theta_hat_reg_param(theta_hat, reg_param)
 
     if (step == 'exponentiated') and (regularizer != 'L1'):
         raise Exception('To use step = \'exponentiated\', '
                         'regularizer = \'L1\' is required.')
 
     if (step == 'exponentiated') and (theta_hat is not None):
-        raise Exception('To use step = \'exponentiated\', '
-                        'theta_hat = None is required.')
+        raise Exception('When step=\'exponentiated\', '
+                        'theta_hat must be None.')
 
     # Get the number of examples and dimension of the problem
     N = len(dataset)
     p = len(theta_0)
 
     if theta_hat is None:
         theta_hat = np.zeros(p)
@@ -1190,38 +1357,37 @@
             theta_avg = (1/(t+1))*theta_t + (t/(t+1))*theta_avg
         elif averaged == 2:
             theta_avg = (2/(t+2))*theta_t + (t/(t+2))*theta_avg
 
         if callback is not None:
             callback_list.append(callback(theta_avg))
 
-    # Check if callback_list is empty
+    # Check if the list callback_list is empty
     if callback_list:
         theta_T = callback_list
     else:
         theta_T = theta_avg
 
     return theta_T
 
 
 def gradient_regularizer(theta_t, regularizer, reg_param, theta_hat):
     """
-    Compute (sub)gradient of regularizer.
+    Compute (sub)gradient of the regularizer.
 
     Parameters
     ----------
     theta_t : 1D ndarray
         Vector where the gradient will be evaluated at.
     regularizer : {'L2_squared', 'L1'}
         Type of regularization on cost vector theta.
     reg_param : float
         Nonnegative regularization parameter..
     theta_hat : 1D ndarray
-        A priory belief or estimate of the true cost vector. When not None, the
-        cost vector returned will be the feasible vector closest to theta_hat.
+        A priory belief or estimate of the true cost vector.
 
     Returns
     -------
     reg_grad : 1D ndarray
         (Sub)gradient of the regularizer evaluated at theta_t.
 
     """
@@ -1267,15 +1433,15 @@
         (Sub)gradient of the regularizer evaluated at theta_t.
     loss_grad : 1D ndarray
         (Sub)gradient of the sum of losses evaluated at theta_t.
 
     """
     aux = 0
     for s_hat, x_hat in samples:
-        # Check if FOP is augmented
+        # Check if the FOP is augmented
         try:
             x_opt = FOP(theta_t, s_hat, x_hat)
         except TypeError:
             x_opt = FOP(theta_t, s_hat)
 
         aux += phi(s_hat, x_hat) - phi(s_hat, x_opt)
 
@@ -1343,15 +1509,15 @@
             theta_pos_t = np.clip(theta_t, 0, None)
             theta_neg_t = np.clip(theta_t, None, 0)
             theta_pos_t1 = np.multiply(theta_pos_t, np.exp(-eta_t*grad))
             theta_neg_t1 = np.multiply(theta_neg_t, np.exp(eta_t*grad))
             theta_t1 = theta_pos_t1 - theta_neg_t1
             norm_theta_t1 = np.sum(theta_pos_t1) + np.sum(theta_neg_t1)
 
-        # If outside the simplex, projec onto it
+        # If outside the simplex, project onto it
         if reg_param*norm_theta_t1 > 1:
             theta_t1 = theta_t1/(reg_param*norm_theta_t1)
 
     # Projection onto Theta
     if Theta == 'nonnegative':
         theta_t = np.clip(theta_t, 0, None)
```

### Comparing `invopt-0.0.4/src/invopt.egg-info/PKG-INFO` & `invopt-0.0.5/src/invopt.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invopt
-Version: 0.0.4
+Version: 0.0.5
 Summary: Inverse Optimization with Python
 Author-email: Pedro Zattoni Scroccaro <pedroszattoni@gmail.com>
 Project-URL: Homepage, https://github.com/pedroszattoni/invopt
 Project-URL: Bug Tracker, https://github.com/pedroszattoni/inverse-optimization/issues
 Keywords: inverse-optimization
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -12,37 +12,44 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 
 # InvOpt: Inverse Optimization with Python
 
-InvOpt is a Python package for solving Inverse Optimization (IO) problems. In IO problems, our goal is to model the behavior of an expert agent, which given an exogenous signal, returns a response action. The underlying assumption of IO is that to compute its response, the expert agent solves an optimization problem parametric in the exogenous signal. We assume to know the constraints imposed on the expert, but not its cost function. Therefore, our goal is to model the cost function being optimized by the expert, using examples of exogenous signals and corresponding expert response actions. More concretely, given a dataset $\mathcal{D} = \\{(\hat{s}_ i, \hat{x}_ i)\\}_ {i=1}^N$ of exogenous signals $\hat{s}_ i$ and the respective expert's response $\hat{x}_ i$, our goal is to find a cost vector $\theta \in \mathbb{R}^p$ such that the **Forward Optimization Problem (FOP)** with feature mapping $\phi$
-$$x_i \in \arg\min_ {x \in \mathbb{X}(\hat{s}_ i)} \ \theta^\top \phi(\hat{s}_ i,x)$$ reproduces (or in some sense approximates) the expert's action $\hat{x}_ i$. For a more detailed description of the IO problem and its modelling, please refer to [Zattoni Scroccaro et al. (2023)](https://arxiv.org/abs/2305.07730) and the references therein. 
+InvOpt is an open-source Python package for solving Inverse Optimization (IO) problems. In IO problems, our goal is to model the behavior of an expert agent, which given an exogenous signal, returns a response action. The underlying assumption of IO is that to compute its response, the expert agent solves an optimization problem parametric in an exogenous signal. We assume to know the constraints imposed on the expert, but not its cost function. Therefore, using examples of exogenous signals and corresponding expert response actions, our goal is to model the cost function being optimized by the expert. More concretely, given a dataset $\mathcal{D} = \\{(\hat{s}_ i, \hat{x}_ i)\\}_ {i=1}^N$ of exogenous signals $\hat{s}_ i$ and the respective expert's response $\hat{x}_ i$, feature mapping $\phi$, our goal is to find a cost vector $\theta \in \mathbb{R}^p$ such that a minimizer $x_ i$ of the **Forward Optimization Problem (FOP)**
+
+$$
+x_i \in \arg\min_ {x \in \mathbb{X}(\hat{s}_ i)} \ \langle \theta,\phi(\hat{s}_ i,x) \rangle
+$$
+
+reproduces (or in some sense approximates) the expert's action $\hat{x}_ i$. For a more detailed description of IO problems and their modeling, please refer to [Zattoni Scroccaro et al. (2023)](https://arxiv.org/abs/2305.07730) and the references therein. 
 
 ## Installation
 
 ```bash
 pip install invopt
 ```
-InvOpt depends on NumPy. Moreover, some of its functions also depend on gurobipy or cvxpy. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
+InvOpt depends on `numpy`. Moreover, some of its functions also depend on `gurobipy` or `cvxpy`. You can get a free academic license for Gurobi [here](https://www.gurobi.com/academia/academic-program-and-licenses/).
 
 ## Usage and examples
 
-The following functions are available in the InvOpt package to solving IO problems:
+The following functions are available in the InvOpt package:
 
-- [`discrete_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent): for FOPs with dicrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
+- [`discrete_consistent`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete_consistent): for FOPs with discrete decision spaces (e.g., binary), and when the dataset is consistent with some cost vector. Can be used to check if the data is consistent.
 - [`discrete`](https://github.com/pedroszattoni/invopt/tree/main/examples/discrete): for FOPs with dicrete decision spaces (e.g., binary).
+- [`continuous_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/continuous_linear): for continuous, linear FOPs.
+- [`continuous_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/continuous_quadratic): for continuous, quadratic FOPs.
 - [`mixed_integer_linear`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_linear): for FOPs with mixed-integer decision spaces and cost functions linear w.r.t. the continuous part of the decision variable.
 - [`mixed_integer_quadratic`](https://github.com/pedroszattoni/invopt/tree/main/examples/mixed_integer_quadratic): for FOPs with mixed-integer decision spaces and cost functions quadratic w.r.t. the continuous part of the decision variable.
 - [`FOM`](https://github.com/pedroszattoni/invopt/tree/main/examples/FOM): for general FOPs. Solves IO problem approximately using first-order methods.
 
 ## Contributing
 
-Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains a number of ideas to possibly improve the InvOpt package.
+Contributions, pull requests and suggestions are very much welcome. The  [TODO](https://github.com/pedroszattoni/invopt/blob/main/TODO.txt) file contains some ideas to possibly improve the InvOpt package.
 
 ## Citing
 If you use InvOpt for research, please cite our accompanying paper:
 
 ```bibtex
 @article{zattoniscroccaro2023learning,
   title={Learning in Inverse Optimization: Incenter Cost, Augmented Suboptimality Loss, and Algorithms},
```

### Comparing `invopt-0.0.4/tests/test_examples.py` & `invopt-0.0.5/tests/test_examples.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,14 +29,22 @@
         script_name = 'discrete_consistent\\binary_LP_consistent_data.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
     def test_binary_LP_inconsistent_data(self):
         script_name = 'discrete\\binary_LP_inconsistent_data.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
+    def test_LP(self):
+        script_name = 'continuous_linear\\LP.py'
+        self.assertTrue(test_script(path_to_examples, script_name))
+
+    def test_QP(self):
+        script_name = 'continuous_quadratic\\QP.py'
+        self.assertTrue(test_script(path_to_examples, script_name))
+
     def test_MILP(self):
         script_name = 'mixed_integer_linear\\MILP.py'
         self.assertTrue(test_script(path_to_examples, script_name))
 
     def test_MIQP(self):
         script_name = 'mixed_integer_quadratic\\MIQP.py'
         self.assertTrue(test_script(path_to_examples, script_name))
```


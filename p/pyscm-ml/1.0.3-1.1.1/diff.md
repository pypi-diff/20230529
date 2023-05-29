# Comparing `tmp/pyscm-ml-1.0.3.tar.gz` & `tmp/pyscm-ml-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyscm-ml-1.0.3.tar", last modified: Mon Jul 20 20:37:04 2020, max compression
+gzip compressed data, was "pyscm-ml-1.1.1.tar", last modified: Mon May 29 19:22:23 2023, max compression
```

## Comparing `pyscm-ml-1.0.3.tar` & `pyscm-ml-1.1.1.tar`

### file list

```diff
@@ -1,28 +1,25 @@
-drwxr-xr-x   0 alexandredrouin   (501) staff       (20)        0 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/
--rw-r--r--   0 alexandredrouin   (501) staff       (20)       25 2020-07-20 20:36:44.000000 pyscm-ml-1.0.3/MANIFEST.in
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     2213 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/PKG-INFO
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     1151 2020-07-20 20:28:54.000000 pyscm-ml-1.0.3/README.md
-drwxr-xr-x   0 alexandredrouin   (501) staff       (20)        0 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/cpp_extensions/
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     3775 2020-07-20 19:36:05.000000 pyscm-ml-1.0.3/cpp_extensions/best_utility.h
--rw-r--r--   0 alexandredrouin   (501) staff       (20)      690 2020-07-20 19:36:05.000000 pyscm-ml-1.0.3/cpp_extensions/double_utils.h
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     4279 2020-07-20 19:36:05.000000 pyscm-ml-1.0.3/cpp_extensions/solver.cpp
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     1198 2020-07-20 19:36:05.000000 pyscm-ml-1.0.3/cpp_extensions/solver.h
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     7698 2018-02-16 20:01:03.000000 pyscm-ml-1.0.3/cpp_extensions/utility_python_bindings.cpp
-drwxr-xr-x   0 alexandredrouin   (501) staff       (20)        0 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/pyscm/
--rw-r--r--   0 alexandredrouin   (501) staff       (20)      795 2018-02-16 20:01:03.000000 pyscm-ml-1.0.3/pyscm/__init__.py
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     2568 2018-02-16 20:01:03.000000 pyscm-ml-1.0.3/pyscm/model.py
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     3709 2018-02-16 20:01:03.000000 pyscm-ml-1.0.3/pyscm/rules.py
--rw-r--r--   0 alexandredrouin   (501) staff       (20)    11670 2020-07-20 19:36:10.000000 pyscm-ml-1.0.3/pyscm/scm.py
-drwxr-xr-x   0 alexandredrouin   (501) staff       (20)        0 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/pyscm/tests/
--rw-r--r--   0 alexandredrouin   (501) staff       (20)        0 2018-02-16 20:01:03.000000 pyscm-ml-1.0.3/pyscm/tests/__init__.py
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     1940 2018-02-16 20:01:03.000000 pyscm-ml-1.0.3/pyscm/tests/test_sklearn_compatibility.py
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     8320 2018-02-16 20:01:03.000000 pyscm-ml-1.0.3/pyscm/tests/test_utility.py
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     1437 2018-02-16 20:01:03.000000 pyscm-ml-1.0.3/pyscm/utils.py
-drwxr-xr-x   0 alexandredrouin   (501) staff       (20)        0 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/pyscm_ml.egg-info/
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     2213 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/pyscm_ml.egg-info/PKG-INFO
--rw-r--r--   0 alexandredrouin   (501) staff       (20)      512 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/pyscm_ml.egg-info/SOURCES.txt
--rw-r--r--   0 alexandredrouin   (501) staff       (20)        1 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/pyscm_ml.egg-info/dependency_links.txt
--rw-r--r--   0 alexandredrouin   (501) staff       (20)       29 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/pyscm_ml.egg-info/requires.txt
--rw-r--r--   0 alexandredrouin   (501) staff       (20)        6 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/pyscm_ml.egg-info/top_level.txt
--rw-r--r--   0 alexandredrouin   (501) staff       (20)       38 2020-07-20 20:37:04.000000 pyscm-ml-1.0.3/setup.cfg
--rw-r--r--   0 alexandredrouin   (501) staff       (20)     3012 2020-07-20 20:36:53.000000 pyscm-ml-1.0.3/setup.py
+drwxrwxr-x   0 thibaud   (1000) thibaud   (1000)        0 2023-05-29 19:22:23.401666 pyscm-ml-1.1.1/
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)    35121 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/LICENSE.md
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     1987 2023-05-29 19:22:23.401666 pyscm-ml-1.1.1/PKG-INFO
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     1199 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/README.md
+drwxrwxr-x   0 thibaud   (1000) thibaud   (1000)        0 2023-05-29 19:22:23.401666 pyscm-ml-1.1.1/cpp_extensions/
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     4279 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/cpp_extensions/solver.cpp
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     7698 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/cpp_extensions/utility_python_bindings.cpp
+drwxrwxr-x   0 thibaud   (1000) thibaud   (1000)        0 2023-05-29 19:22:23.401666 pyscm-ml-1.1.1/pyscm/
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)      796 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/pyscm/__init__.py
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     2563 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/pyscm/model.py
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     3751 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/pyscm/rules.py
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)    13214 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/pyscm/scm.py
+drwxrwxr-x   0 thibaud   (1000) thibaud   (1000)        0 2023-05-29 19:22:23.401666 pyscm-ml-1.1.1/pyscm/tests/
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)        0 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/pyscm/tests/__init__.py
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     2032 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/pyscm/tests/test_sklearn_compatibility.py
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     9215 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/pyscm/tests/test_utility.py
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     1552 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/pyscm/utils.py
+drwxrwxr-x   0 thibaud   (1000) thibaud   (1000)        0 2023-05-29 19:22:23.401666 pyscm-ml-1.1.1/pyscm_ml.egg-info/
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     1987 2023-05-29 19:22:23.000000 pyscm-ml-1.1.1/pyscm_ml.egg-info/PKG-INFO
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)      427 2023-05-29 19:22:23.000000 pyscm-ml-1.1.1/pyscm_ml.egg-info/SOURCES.txt
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)        1 2023-05-29 19:22:23.000000 pyscm-ml-1.1.1/pyscm_ml.egg-info/dependency_links.txt
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)       29 2023-05-29 19:22:23.000000 pyscm-ml-1.1.1/pyscm_ml.egg-info/requires.txt
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)        6 2023-05-29 19:22:23.000000 pyscm-ml-1.1.1/pyscm_ml.egg-info/top_level.txt
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)       38 2023-05-29 19:22:23.401666 pyscm-ml-1.1.1/setup.cfg
+-rw-rw-r--   0 thibaud   (1000) thibaud   (1000)     2915 2023-05-29 19:22:10.000000 pyscm-ml-1.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyscm-ml-1.0.3/PKG-INFO` & `pyscm-ml-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: pyscm-ml
-Version: 1.0.3
+Version: 1.1.1
 Summary: The Set Covering Machine algorithm
 Home-page: https://github.com/aldro61/pyscm
 Author: Alexandre Drouin
 Author-email: aldro61@gmail.com
 Maintainer: Alexandre Drouin
 Maintainer-email: aldro61@gmail.com
 License: GPL-3
-Description: [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
-        [![Build Status](https://travis-ci.org/aldro61/pyscm.svg?branch=master)](https://travis-ci.org/aldro61/pyscm)
-        [![DOI](https://zenodo.org/badge/17353131.svg)](https://zenodo.org/badge/latestdoi/17353131)
-        
-        
-        # pySCM
-        
-        A fast implementation of the Set Covering Machine algorithm using a dynamic programming algorithm to select the rules of greatest utility.
-        
-        Marchand, M., & Taylor, J. S. (2003). The set covering machine. Journal of Machine Learning Research, 3, 723–746.
-        
-        ![Alt text](https://github.com/aldro61/pyscm/raw/master/examples/decision_boundary.png)
-        
-        ## Installation
-        
-        ``` 
-        pip install pyscm-ml
-        ```
-        or
-        
-        ``` 
-        python setup.py install
-        ```
-        
-        ## Running tests
-        ```
-        python setup.py test
-        ```
-        
-        ## Contributors
-         * [Alexandre Drouin](http://graal.ift.ulaval.ca/adrouin) (package maintainer)
-         * [Francis Brochu](https://github.com/PhrankBrochu)
-         * [Gaël Letarte St-Pierre](https://github.com/gletarte)
-         * [Mazid Osseni](https://github.com/dizam92)
-         * [Pier-Luc Plante](https://github.com/plpla)
-         * [Thibaud Godon](https://github.com/thibgo)
-        
 Keywords: machine-learning classification set-covering-machine rule-based-models
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
+[![Build Status](https://travis-ci.org/aldro61/pyscm.svg?branch=master)](https://travis-ci.org/aldro61/pyscm)
+[![DOI](https://zenodo.org/badge/17353131.svg)](https://zenodo.org/badge/latestdoi/17353131)
+
+
+# pySCM
+
+A fast implementation of the Set Covering Machine algorithm using a dynamic programming algorithm to select the rules of greatest utility.
+
+Marchand, M., & Taylor, J. S. (2003). The set covering machine. Journal of Machine Learning Research, 3, 723–746.
+
+![Alt text](https://github.com/aldro61/pyscm/raw/master/examples/decision_boundary.png)
+
+## Installation
+
+``` 
+pip install pyscm-ml
+```
+or
+
+``` 
+python setup.py install
+```
+
+## Running tests
+```
+python setup.py test
+```
+
+## Contributors
+ * [Alexandre Drouin](http://graal.ift.ulaval.ca/adrouin) (package maintainer)
+ * [Baptiste Bauvin](https://github.com/babau1)
+ * [Francis Brochu](https://github.com/PhrankBrochu)
+ * [Gaël Letarte St-Pierre](https://github.com/gletarte)
+ * [Mazid Osseni](https://github.com/dizam92)
+ * [Pier-Luc Plante](https://github.com/plpla)
+ * [Thibaud Godon](https://github.com/thibgo)
+
+
```

### Comparing `pyscm-ml-1.0.3/README.md` & `pyscm-ml-1.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -25,12 +25,13 @@
 ## Running tests
 ```
 python setup.py test
 ```
 
 ## Contributors
  * [Alexandre Drouin](http://graal.ift.ulaval.ca/adrouin) (package maintainer)
+ * [Baptiste Bauvin](https://github.com/babau1)
  * [Francis Brochu](https://github.com/PhrankBrochu)
  * [Gaël Letarte St-Pierre](https://github.com/gletarte)
  * [Mazid Osseni](https://github.com/dizam92)
  * [Pier-Luc Plante](https://github.com/plpla)
  * [Thibaud Godon](https://github.com/thibgo)
```

### Comparing `pyscm-ml-1.0.3/cpp_extensions/solver.cpp` & `pyscm-ml-1.1.1/cpp_extensions/solver.cpp`

 * *Files identical despite different names*

### Comparing `pyscm-ml-1.0.3/cpp_extensions/utility_python_bindings.cpp` & `pyscm-ml-1.1.1/cpp_extensions/utility_python_bindings.cpp`

 * *Files identical despite different names*

### Comparing `pyscm-ml-1.0.3/pyscm/__init__.py` & `pyscm-ml-1.1.1/pyscm/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -12,8 +12,8 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
     along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 """
-from .scm import SetCoveringMachineClassifier
+from .scm import SetCoveringMachineClassifier
```

### Comparing `pyscm-ml-1.0.3/pyscm/model.py` & `pyscm-ml-1.1.1/pyscm/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,32 +58,33 @@
 
     def __len__(self):
         return len(self.rules)
 
     def __str__(self):
         return self._to_string()
 
+
 class ConjunctionModel(BaseModel):
     def predict(self, X):
-        predictions = np.ones(X.shape[0], np.bool)
+        predictions = np.ones(X.shape[0], bool)
         for a in self.rules:
             predictions = np.logical_and(predictions, a.classify(X))
         return predictions.astype(np.uint8)
 
     @property
     def type(self):
         return "conjunction"
 
     def __str__(self):
         return self._to_string(separator=" and ")
 
 
 class DisjunctionModel(BaseModel):
     def predict(self, X):
-        predictions = np.zeros(X.shape[0], np.bool)
+        predictions = np.zeros(X.shape[0], bool)
         for a in self.rules:
             predictions = np.logical_or(predictions, a.classify(X))
         return predictions.astype(np.uint8)
 
     @property
     def type(self):
         return "disjunction"
```

### Comparing `pyscm-ml-1.0.3/pyscm/rules.py` & `pyscm-ml-1.1.1/pyscm/rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 
 class BaseRule(object):
     """
     A rule mixin class
 
     """
+
     def __init__(self):
         super(BaseRule, self).__init__()
 
     def classify(self, X):
         """
         Classifies a set of examples using the rule.
 
@@ -75,14 +76,15 @@
         The index of the feature
     threshold: float
         The threshold at which the outcome of the rule changes
     kind: str, default="greater"
         The case in which the rule returns 1, either "greater" or "less_equal".
 
     """
+
     def __init__(self, feature_idx, threshold, kind="greater"):
         self.feature_idx = feature_idx
         self.threshold = threshold
         self.kind = kind
         super(DecisionStump, self).__init__()
 
     def classify(self, X):
@@ -112,12 +114,17 @@
 
         Returns:
         --------
         inverse: BaseRule
             A rule that is the inverse of self.
 
         """
-        return DecisionStump(feature_idx=self.feature_idx, threshold=self.threshold,
-                             kind="greater" if self.kind == "less_equal" else "less_equal")
+        return DecisionStump(
+            feature_idx=self.feature_idx,
+            threshold=self.threshold,
+            kind="greater" if self.kind == "less_equal" else "less_equal",
+        )
 
     def __str__(self):
-        return "X[{0:d}] {1!s} {2:.3f}".format(self.feature_idx, ">" if self.kind == "greater" else "<=", self.threshold)
+        return "X[{0:d}] {1!s} {2:.3f}".format(
+            self.feature_idx, ">" if self.kind == "greater" else "<=", self.threshold
+        )
```

### Comparing `pyscm-ml-1.0.3/pyscm/scm.py` & `pyscm-ml-1.1.1/pyscm/scm.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,33 +20,44 @@
 from six import iteritems
 
 import logging
 import numpy as np
 
 from sklearn.base import BaseEstimator, ClassifierMixin
 from sklearn.metrics import accuracy_score
-from sklearn.utils.validation import check_X_y, check_array, check_is_fitted,  check_random_state
+from sklearn.utils.validation import (
+    check_X_y,
+    check_array,
+    check_is_fitted,
+    check_random_state,
+)
 from warnings import warn
 
 from ._scm_utility import find_max as find_max_utility  # cpp extensions
 from .model import ConjunctionModel, DisjunctionModel
 from .rules import DecisionStump
 from .utils import _class_to_string
 
 
 class BaseSetCoveringMachine(BaseEstimator, ClassifierMixin):
-    def __init__(self, p=1.0, model_type="conjunction", max_rules=10, random_state=None):
+    def __init__(
+        self, p=1.0, model_type="conjunction", max_rules=10, random_state=None
+    ):
         self.p = p
         self.model_type = model_type
         self.max_rules = max_rules
         self.random_state = random_state
 
     def get_params(self, deep=True):
-        return {"p": self.p, "model_type": self.model_type, "max_rules": self.max_rules,
-                "random_state": self.random_state}
+        return {
+            "p": self.p,
+            "model_type": self.model_type,
+            "max_rules": self.max_rules,
+            "random_state": self.random_state,
+        }
 
     def set_params(self, **parameters):
         for parameter, value in iteritems(parameters):
             setattr(self, parameter, value)
         return self
 
     def fit(self, X, y, tiebreaker=None, iteration_callback=None, **fit_params):
@@ -100,73 +111,120 @@
                 if key[:9] == "utility__":
                     utility_function_additional_args[key[9:]] = value
 
         # Validate the input data
         logging.debug("Validating the input data")
         X, y = check_X_y(X, y)
         X = np.asarray(X, dtype=np.double)
-        self.classes_, y, total_n_ex_by_class = np.unique(y, return_inverse=True, return_counts=True)
+        self.classes_, y, total_n_ex_by_class = np.unique(
+            y, return_inverse=True, return_counts=True
+        )
         if len(self.classes_) != 2:
             raise ValueError("y must contain two unique classes.")
-        logging.debug("The data contains {0:d} examples. Negative class is {1!s} (n: {2:d}) and positive class is {3!s} (n: {4:d}).".format(len(y), self.classes_[0], total_n_ex_by_class[0], self.classes_[1], total_n_ex_by_class[1]))
+        logging.debug(
+            "The data contains {0:d} examples. Negative class is {1!s} (n: {2:d}) and positive class is {3!s} (n: {4:d}).".format(
+                len(y),
+                self.classes_[0],
+                total_n_ex_by_class[0],
+                self.classes_[1],
+                total_n_ex_by_class[1],
+            )
+        )
 
         # Invert the classes if we are learning a disjunction
         logging.debug("Preprocessing example labels")
         pos_ex_idx, neg_ex_idx = self._get_example_idx_by_class(y)
-        y = np.zeros(len(y), dtype=np.int)
+        y = np.zeros(len(y), dtype=int)
         y[pos_ex_idx] = 1
         y[neg_ex_idx] = 0
 
         # Presort all the features
         logging.debug("Presorting all features")
         X_argsort_by_feature_T = np.argsort(X, axis=0).T.copy()
 
         # Create an empty model
         logging.debug("Initializing empty model")
-        self.model_ = ConjunctionModel() if self.model_type == "conjunction" else DisjunctionModel()
+        self.model_ = (
+            ConjunctionModel()
+            if self.model_type == "conjunction"
+            else DisjunctionModel()
+        )
 
         logging.debug("Training start")
         remaining_example_idx = np.arange(len(y))
         remaining_negative_example_idx = neg_ex_idx
-        while len(remaining_negative_example_idx) > 0 and len(self.model_) < self.max_rules:
+        while (
+            len(remaining_negative_example_idx) > 0
+            and len(self.model_) < self.max_rules
+        ):
             logging.debug("Finding the optimal rule to add to the model")
-            opti_utility, \
-            opti_feat_idx, \
-            opti_threshold, \
-            opti_kind, \
-            opti_N, \
-            opti_P_bar = self._get_best_utility_rules(X.copy(), y.copy(), X_argsort_by_feature_T.copy(), remaining_example_idx.copy(),
-                                                      **utility_function_additional_args)
-
-            logging.debug("Tiebreaking. Found {0:d} optimal rules".format(len(opti_feat_idx)))
+            (
+                opti_utility,
+                opti_feat_idx,
+                opti_threshold,
+                opti_kind,
+                opti_N,
+                opti_P_bar,
+            ) = self._get_best_utility_rules(
+                X.copy(),
+                y.copy(),
+                X_argsort_by_feature_T.copy(),
+                remaining_example_idx.copy(),
+                **utility_function_additional_args
+            )
+
+            logging.debug(
+                "Tiebreaking. Found {0:d} optimal rules".format(len(opti_feat_idx))
+            )
             if len(opti_feat_idx) > 1:
                 if tiebreaker is None:
                     training_risk_decrease = 1.0 * opti_N - opti_P_bar
-                    keep_idx = np.where(training_risk_decrease == training_risk_decrease.max())[0][0]
+                    keep_idx = np.where(
+                        training_risk_decrease == training_risk_decrease.max()
+                    )[0][0]
                 else:
-                    keep_idx = tiebreaker(self.model_type, opti_feat_idx, opti_threshold, opti_kind)
+                    keep_idx = tiebreaker(
+                        self.model_type, opti_feat_idx, opti_threshold, opti_kind
+                    )
             else:
                 keep_idx = 0
-            stump = DecisionStump(feature_idx=opti_feat_idx[keep_idx], threshold=opti_threshold[keep_idx],
-                                  kind="greater" if opti_kind[keep_idx] == 0 else "less_equal")
+            stump = DecisionStump(
+                feature_idx=opti_feat_idx[keep_idx],
+                threshold=opti_threshold[keep_idx],
+                kind="greater" if opti_kind[keep_idx] == 0 else "less_equal",
+            )
 
             logging.debug("The best rule has utility {0:.3f}".format(opti_utility))
             self._add_attribute_to_model(stump)
 
-            logging.debug("Discarding all examples that the rule classifies as negative")
-            remaining_example_idx = remaining_example_idx[stump.classify(X[remaining_example_idx])]
-            remaining_negative_example_idx = remaining_negative_example_idx[stump.classify(X[remaining_negative_example_idx])]
-            logging.debug("There are {0:d} examples remaining ({1:d} negatives)".format(len(remaining_example_idx),
-                                                                              len(remaining_negative_example_idx)))
+            logging.debug(
+                "Discarding all examples that the rule classifies as negative"
+            )
+            remaining_example_idx = remaining_example_idx[
+                stump.classify(X[remaining_example_idx])
+            ]
+            remaining_negative_example_idx = remaining_negative_example_idx[
+                stump.classify(X[remaining_negative_example_idx])
+            ]
+            logging.debug(
+                "There are {0:d} examples remaining ({1:d} negatives)".format(
+                    len(remaining_example_idx), len(remaining_negative_example_idx)
+                )
+            )
 
             iteration_callback(self.model_)
 
         logging.debug("Training completed")
 
-        self.rule_importances_ = []  # TODO: implement rule importances (like its done in Kover)
+        logging.debug("Calculating rule importances")
+        # Definition: how often each rule outputs a value that causes the value of the model to be final
+        final_outcome = 0 if self.model_type == "conjunction" else 1
+        total_outcome = (self.model_.predict(X) == final_outcome).sum()  # n times the model outputs the final outcome
+        self.rule_importances_ = np.array([(r.classify(X) == final_outcome).sum() / total_outcome for r in self.model_.rules])  # contribution of each rule
+        logging.debug("Done.")
 
         return self
 
     def predict(self, X):
         """
         Predict class
 
@@ -196,21 +254,36 @@
 
         Returns:
         --------
         p : array of shape = [n_examples, 2]
             The class probabilities for each example. Classes are ordered by lexicographic order.
 
         """
-        warn("SetCoveringMachines do not support probabilistic predictions. The returned values will be zero or one.",
-             RuntimeWarning)
+        warn(
+            "SetCoveringMachines do not support probabilistic predictions. The returned values will be zero or one.",
+            RuntimeWarning,
+        )
         check_is_fitted(self, ["model_", "rule_importances_", "classes_"])
         X = check_array(X)
         pos_proba = self.classes_[self.model_.predict(X)]
         neg_proba = 1.0 - pos_proba
         return np.hstack((neg_proba.reshape(-1, 1), pos_proba.reshape(-1, 1)))
+    
+    @property
+    def rule_importances(self):
+        """
+        A measure of importance for each rule in the classifier based on how much it contributes to the final predictions.
+        
+        Returns:
+        --------
+        rule_importances: list of float
+            Importances of each rule, defined as defined in https://doi.org/10.1186/s12864-016-2889-6
+        """
+        check_is_fitted(self, ["model_", "rule_importances_", "classes_"])
+        return self.rule_importances_
 
     def score(self, X, y):
         """
         Predict classes of examples and measure accuracy
 
         Parameters:
         -----------
@@ -269,13 +342,17 @@
         The model type (conjunction or disjunction).
     max_rules: int, default=10
         The maximum number of rules in the model.
     random_state: int, np.random.RandomState or None, default=None
         The random state.
 
     """
-    def __init__(self, p=1.0, model_type=str("conjunction"), max_rules=10, random_state=None):
-        super(SetCoveringMachineClassifier, self).__init__(p=p, model_type=model_type, max_rules=max_rules,
-                                                           random_state=random_state)
+
+    def __init__(
+        self, p=1.0, model_type=str("conjunction"), max_rules=10, random_state=None
+    ):
+        super(SetCoveringMachineClassifier, self).__init__(
+            p=p, model_type=model_type, max_rules=max_rules, random_state=random_state
+        )
 
     def _get_best_utility_rules(self, X, y, X_argsort_by_feature_T, example_idx):
         return find_max_utility(self.p, X, y, X_argsort_by_feature_T, example_idx)
```

### Comparing `pyscm-ml-1.0.3/pyscm/tests/test_sklearn_compatibility.py` & `pyscm-ml-1.1.1/pyscm/tests/test_sklearn_compatibility.py`

 * *Files 22% similar despite different names*

```diff
@@ -7,49 +7,59 @@
 from sklearn.preprocessing import StandardScaler
 from unittest import TestCase
 
 from ..scm import SetCoveringMachineClassifier
 
 
 class SklearnCompatibilityTests(TestCase):
-
     def test_sklearn_grid_search(self):
         """
         Test compatibility with sklearn GridSearchCV function
 
         """
         rnd = np.random.RandomState(0)
-        X = np.random.rand(100,100)
+        X = np.random.rand(100, 100)
         y = np.random.randint(2, size=100)
 
-        scm_param_grid = {"p": [0.01, 0.1, 1, 10, 100],
-                          "max_rules": [1,2,3,4,5],
-                          "model_type": ["conjunction", "disjunction"],
-                          "random_state": [rnd]}
-        gscv = GridSearchCV(SetCoveringMachineClassifier(), scm_param_grid, n_jobs=1, cv=5)
+        scm_param_grid = {
+            "p": [0.01, 0.1, 1, 10, 100],
+            "max_rules": [1, 2, 3, 4, 5],
+            "model_type": ["conjunction", "disjunction"],
+            "random_state": [rnd],
+        }
+        gscv = GridSearchCV(
+            SetCoveringMachineClassifier(), scm_param_grid, n_jobs=1, cv=5
+        )
         try:
             gscv.fit(X, y)
         except Exception as e:
             self.fail("GridSearchCV.fit() raised " + e.message + " unexpectedly!")
 
-        gscv = GridSearchCV(SetCoveringMachineClassifier(), scm_param_grid, n_jobs=2, cv=5)
+        gscv = GridSearchCV(
+            SetCoveringMachineClassifier(), scm_param_grid, n_jobs=2, cv=5
+        )
         try:
             gscv.fit(X, y)
         except Exception as e:
-            self.fail("GridSearchCV.fit() raised "+e.message+" unexpectedly when running with 2 jobs!")
+            self.fail(
+                "GridSearchCV.fit() raised "
+                + e.message
+                + " unexpectedly when running with 2 jobs!"
+            )
 
     def test_sklearn_pipeline(self):
         """
         Test compatibility with sklearn pipelines
 
         """
         rnd = np.random.RandomState(0)
         X = np.random.rand(10, 10)
         y = np.random.randint(2, size=10)
 
-        scm = SetCoveringMachineClassifier(model_type="conjunction", p=0, max_rules=3, random_state=rnd)
-        pipeline = Pipeline([("Scale", StandardScaler()),
-                             ("SCM", scm)])
+        scm = SetCoveringMachineClassifier(
+            model_type="conjunction", p=0, max_rules=3, random_state=rnd
+        )
+        pipeline = Pipeline([("Scale", StandardScaler()), ("SCM", scm)])
         try:
             pipeline.fit(X, y)
         except Exception as e:
-            self.fail("Pipeline.fit() raised "+e.message+" unexpectedly!")
+            self.fail("Pipeline.fit() raised " + e.message + " unexpectedly!")
```

### Comparing `pyscm-ml-1.0.3/pyscm/tests/test_utility.py` & `pyscm-ml-1.1.1/pyscm/tests/test_utility.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,175 +33,243 @@
         """
         Dummy test #1
         """
         X = np.array([[1, 2, 2, 2, 3, 4]], dtype=np.double).reshape(-1, 1).copy()
         y = np.array([0, 1, 0, 1, 1, 1])
         p = 1
         Xas = np.argsort(X, axis=0).T.copy()
-        best_utility, best_feat_idx, \
-        best_thresholds, best_kinds, \
-        best_N, best_P_bar = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(1))
+        (
+            best_utility,
+            best_feat_idx,
+            best_thresholds,
+            best_kinds,
+            best_N,
+            best_P_bar,
+        ) = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(1))
         np.testing.assert_almost_equal(actual=best_utility, desired=1.0)
         np.testing.assert_almost_equal(actual=best_feat_idx, desired=[0])
         np.testing.assert_almost_equal(actual=best_thresholds, desired=[1])
         np.testing.assert_almost_equal(actual=best_kinds, desired=[0])
 
     def test_2(self):
         """
         Test that hyperparameter p works
         """
         X = np.array([[1, 2, 2, 2, 3, 4]], dtype=np.double).reshape(-1, 1).copy()
         y = np.array([0, 1, 0, 1, 1, 1])
         Xas = np.argsort(X, axis=0).T.copy()
         p = 0.5
-        best_utility, best_feat_idx, \
-        best_thresholds, best_kinds, \
-        best_N, best_P_bar = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(1))
+        (
+            best_utility,
+            best_feat_idx,
+            best_thresholds,
+            best_kinds,
+            best_N,
+            best_P_bar,
+        ) = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(1))
 
         np.testing.assert_almost_equal(actual=best_utility, desired=1.0)
         np.testing.assert_almost_equal(actual=best_feat_idx, desired=[0, 0])
         np.testing.assert_almost_equal(actual=best_thresholds, desired=[1, 2])
         np.testing.assert_almost_equal(actual=best_kinds, desired=[0, 0])
 
     def test_3(self):
         """
         Test that feature_weights works
         """
-        X = np.array([[1, 1],
-                      [1, 0]], dtype=np.double)
+        X = np.array([[1, 1], [1, 0]], dtype=np.double)
         y = np.array([0, 1])
         Xas = np.argsort(X, axis=0).T.copy()
         p = 1.0
 
         # Equal weights, feat 1 should be the best with utility 1
-        best_utility, best_feat_idx, \
-        best_thresholds, best_kinds, \
-        best_N, best_P_bar = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(X.shape[1]))
+        (
+            best_utility,
+            best_feat_idx,
+            best_thresholds,
+            best_kinds,
+            best_N,
+            best_P_bar,
+        ) = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(X.shape[1]))
         np.testing.assert_almost_equal(actual=best_utility, desired=1)
         np.testing.assert_almost_equal(actual=best_feat_idx, desired=[1])
 
         # Double weight for feat 1, should be the best with utility 2
-        best_utility, best_feat_idx, \
-        best_thresholds, best_kinds, \
-        best_N, best_P_bar = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.array([1.0, 2.0]))
+        (
+            best_utility,
+            best_feat_idx,
+            best_thresholds,
+            best_kinds,
+            best_N,
+            best_P_bar,
+        ) = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.array([1.0, 2.0]))
         np.testing.assert_almost_equal(actual=best_utility, desired=2)
         np.testing.assert_almost_equal(actual=best_feat_idx, desired=[1])
 
         # 10 times the weight for feat 1, should be the best with utility 10
-        best_utility, best_feat_idx, \
-        best_thresholds, best_kinds, \
-        best_N, best_P_bar = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.array([1.0, 10.0]))
+        (
+            best_utility,
+            best_feat_idx,
+            best_thresholds,
+            best_kinds,
+            best_N,
+            best_P_bar,
+        ) = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.array([1.0, 10.0]))
         np.testing.assert_almost_equal(actual=best_utility, desired=10)
         np.testing.assert_almost_equal(actual=best_feat_idx, desired=[1])
 
     def test_4(self):
         """
         Test that example_idx works
         """
-        X = np.array([[1, 1],
-                      [0, 0],
-                      [1, 0]], dtype=np.double)
+        X = np.array([[1, 1], [0, 0], [1, 0]], dtype=np.double)
         y = np.array([0, 1, 1])
         Xas = np.argsort(X, axis=0).T.copy()
         p = 1.0
 
         # If example 3 is included, the best feature is feat1
-        best_utility, best_feat_idx, \
-        best_thresholds, best_kinds, \
-        best_N, best_P_bar = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(X.shape[1]))
+        (
+            best_utility,
+            best_feat_idx,
+            best_thresholds,
+            best_kinds,
+            best_N,
+            best_P_bar,
+        ) = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(X.shape[1]))
         np.testing.assert_almost_equal(actual=best_feat_idx, desired=[1])
 
         # If example 3 is included, the best feature is feat1
-        best_utility, best_feat_idx, \
-        best_thresholds, best_kinds, \
-        best_N, best_P_bar = find_max(p, X, y, Xas, np.array([1, 2], dtype=np.int), np.ones(X.shape[1]))
+        (
+            best_utility,
+            best_feat_idx,
+            best_thresholds,
+            best_kinds,
+            best_N,
+            best_P_bar,
+        ) = find_max(p, X, y, Xas, np.array([1, 2], dtype=int), np.ones(X.shape[1]))
         np.testing.assert_almost_equal(actual=best_feat_idx, desired=[0, 1])
-        
+
     def test_5(self):
         """
         Test that solver return accurate equivalent rules
         """
-        X = np.array([[1, 1, 0.5, 1],
-                      [2, 1, 0.5, 1],
-                      [2, 1, 0.5, 1],
-                      [3, 1, 1.7, 0],
-                      [4, 1, 1.7, 0],
-                      [5, 1, 1.7, 0],
-                      [6, 1, 1.7, 0],
-                      [7, 1, 1.7, 0]], dtype=np.double)
+        X = np.array(
+            [
+                [1, 1, 0.5, 1],
+                [2, 1, 0.5, 1],
+                [2, 1, 0.5, 1],
+                [3, 1, 1.7, 0],
+                [4, 1, 1.7, 0],
+                [5, 1, 1.7, 0],
+                [6, 1, 1.7, 0],
+                [7, 1, 1.7, 0],
+            ],
+            dtype=np.double,
+        )
         y = np.array([0, 0, 0, 1, 1, 1, 1, 1])
         Xas = np.argsort(X, axis=0).T.copy()
         p = 1.0
 
-        best_utility, best_feat_idx, \
-        best_thresholds, best_kinds, \
-        best_N, best_P_bar = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(X.shape[1]))
+        (
+            best_utility,
+            best_feat_idx,
+            best_thresholds,
+            best_kinds,
+            best_N,
+            best_P_bar,
+        ) = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(X.shape[1]))
         np.testing.assert_almost_equal(actual=best_utility, desired=3.0)
         np.testing.assert_almost_equal(actual=best_feat_idx, desired=[0, 2, 3])
-        np.testing.assert_almost_equal(actual=best_thresholds, desired=[2., 0.5, 0.])
+        np.testing.assert_almost_equal(actual=best_thresholds, desired=[2.0, 0.5, 0.0])
         np.testing.assert_almost_equal(actual=best_kinds, desired=[0, 0, 1])
 
     def test_6(self):
         """
         Test that solver return accurate N and P_bar
         """
-        X = np.array([[0, 0.5, 0],
-                      [0, 1.7, 0],
-                      [1, 0.5, 0],
-                      [0, 1.7, 0],
-                      [1, 0.5, 0],
-                      [1, 1.7, 0],
-                      [1, 1.7, 0],
-                      [1, 1.7, 0]], dtype=np.double)
+        X = np.array(
+            [
+                [0, 0.5, 0],
+                [0, 1.7, 0],
+                [1, 0.5, 0],
+                [0, 1.7, 0],
+                [1, 0.5, 0],
+                [1, 1.7, 0],
+                [1, 1.7, 0],
+                [1, 1.7, 0],
+            ],
+            dtype=np.double,
+        )
         y = np.array([0, 0, 0, 1, 1, 1, 1, 1])
         Xas = np.argsort(X, axis=0).T.copy()
         p = 1.0
 
-        best_utility, best_feat_idx, \
-        best_thresholds, best_kinds, \
-        best_N, best_P_bar = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(X.shape[1]))
+        (
+            best_utility,
+            best_feat_idx,
+            best_thresholds,
+            best_kinds,
+            best_N,
+            best_P_bar,
+        ) = find_max(p, X, y, Xas, np.arange(X.shape[0]), np.ones(X.shape[1]))
         np.testing.assert_almost_equal(actual=best_N, desired=[2, 2])
         np.testing.assert_almost_equal(actual=best_P_bar, desired=[1, 1])
 
     def test_random_data(self):
         """
         Random testing
         """
-        n_tests = 10 #10000
+        n_tests = 10  # 10000
 
         # Using rounding generates cases with equal feature values for examples
         for n_decimals in range(3):
 
             # The more examples, the more likely we are to have equal feature values
             for n_examples in [10, 100, 1000]:
 
                 # Do this a few times for each configuration
                 for _ in range(n_tests):
-                    p = max(0, np.random.rand() * 100.)
-                    x = (np.random.rand(n_examples) * 5.).round(n_decimals).reshape(-1, 1).copy()
+                    p = max(0, np.random.rand() * 100.0)
+                    x = (
+                        (np.random.rand(n_examples) * 5.0)
+                        .round(n_decimals)
+                        .reshape(-1, 1)
+                        .copy()
+                    )
                     xas = np.argsort(x, axis=0).T.copy()
                     y = np.random.randint(0, 2, n_examples)
                     thresholds = np.unique(x)
 
                     # Use the solver to find the solution
-                    solver_best_utility, solver_best_feat_idx, solver_best_thresholds, solver_best_kinds, \
-                    solver_best_N, solver_best_P_bar= \
-                        find_max(p, x, y, xas, np.arange(n_examples))
+                    (
+                        solver_best_utility,
+                        solver_best_feat_idx,
+                        solver_best_thresholds,
+                        solver_best_kinds,
+                        solver_best_N,
+                        solver_best_P_bar,
+                    ) = find_max(p, x, y, xas, np.arange(n_examples))
 
                     # Less equal rule utilities
                     le_rule_utilities = []
                     for t in thresholds:
-                        rule_classifications = (x <= t).reshape(-1,)
+                        rule_classifications = (x <= t).reshape(
+                            -1,
+                        )
                         N = (~rule_classifications[y == 0]).sum()
                         P_bar = (~rule_classifications[y == 1]).sum()
                         le_rule_utilities.append(N - p * P_bar)
 
                     # Greater rule utilities
                     g_rule_utilities = []
                     for t in thresholds:
-                        rule_classifications = (x > t).reshape(-1,)
+                        rule_classifications = (x > t).reshape(
+                            -1,
+                        )
                         N = 1.0 * (~rule_classifications[y == 0]).sum()
                         P_bar = 1.0 * (~rule_classifications[y == 1]).sum()
                         g_rule_utilities.append(N - p * P_bar)
 
-                    np.testing.assert_almost_equal(actual=solver_best_utility, desired=max(max(le_rule_utilities),
-                                                                                           max(g_rule_utilities)))
+                    np.testing.assert_almost_equal(
+                        actual=solver_best_utility,
+                        desired=max(max(le_rule_utilities), max(g_rule_utilities)),
+                    )
```

### Comparing `pyscm-ml-1.0.3/pyscm/utils.py` & `pyscm-ml-1.1.1/pyscm/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -35,9 +35,19 @@
     string_rep: string
         A string representation of the class and its public attributes.
 
     Notes:
     -----
     Private attributes must be marked with a leading underscore.
     """
-    return instance.__class__.__name__ + "(" + ",".join(
-        [str(k) + "=" + str(v) for k, v in iteritems(instance.__dict__) if str(k[0]) != "_"]) + ")"
+    return (
+        instance.__class__.__name__
+        + "("
+        + ",".join(
+            [
+                str(k) + "=" + str(v)
+                for k, v in iteritems(instance.__dict__)
+                if str(k[0]) != "_"
+            ]
+        )
+        + ")"
+    )
```

### Comparing `pyscm-ml-1.0.3/pyscm_ml.egg-info/PKG-INFO` & `pyscm-ml-1.1.1/pyscm_ml.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,60 @@
 Metadata-Version: 2.1
 Name: pyscm-ml
-Version: 1.0.3
+Version: 1.1.1
 Summary: The Set Covering Machine algorithm
 Home-page: https://github.com/aldro61/pyscm
 Author: Alexandre Drouin
 Author-email: aldro61@gmail.com
 Maintainer: Alexandre Drouin
 Maintainer-email: aldro61@gmail.com
 License: GPL-3
-Description: [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
-        [![Build Status](https://travis-ci.org/aldro61/pyscm.svg?branch=master)](https://travis-ci.org/aldro61/pyscm)
-        [![DOI](https://zenodo.org/badge/17353131.svg)](https://zenodo.org/badge/latestdoi/17353131)
-        
-        
-        # pySCM
-        
-        A fast implementation of the Set Covering Machine algorithm using a dynamic programming algorithm to select the rules of greatest utility.
-        
-        Marchand, M., & Taylor, J. S. (2003). The set covering machine. Journal of Machine Learning Research, 3, 723–746.
-        
-        ![Alt text](https://github.com/aldro61/pyscm/raw/master/examples/decision_boundary.png)
-        
-        ## Installation
-        
-        ``` 
-        pip install pyscm-ml
-        ```
-        or
-        
-        ``` 
-        python setup.py install
-        ```
-        
-        ## Running tests
-        ```
-        python setup.py test
-        ```
-        
-        ## Contributors
-         * [Alexandre Drouin](http://graal.ift.ulaval.ca/adrouin) (package maintainer)
-         * [Francis Brochu](https://github.com/PhrankBrochu)
-         * [Gaël Letarte St-Pierre](https://github.com/gletarte)
-         * [Mazid Osseni](https://github.com/dizam92)
-         * [Pier-Luc Plante](https://github.com/plpla)
-         * [Thibaud Godon](https://github.com/thibgo)
-        
 Keywords: machine-learning classification set-covering-machine rule-based-models
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+[![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
+[![Build Status](https://travis-ci.org/aldro61/pyscm.svg?branch=master)](https://travis-ci.org/aldro61/pyscm)
+[![DOI](https://zenodo.org/badge/17353131.svg)](https://zenodo.org/badge/latestdoi/17353131)
+
+
+# pySCM
+
+A fast implementation of the Set Covering Machine algorithm using a dynamic programming algorithm to select the rules of greatest utility.
+
+Marchand, M., & Taylor, J. S. (2003). The set covering machine. Journal of Machine Learning Research, 3, 723–746.
+
+![Alt text](https://github.com/aldro61/pyscm/raw/master/examples/decision_boundary.png)
+
+## Installation
+
+``` 
+pip install pyscm-ml
+```
+or
+
+``` 
+python setup.py install
+```
+
+## Running tests
+```
+python setup.py test
+```
+
+## Contributors
+ * [Alexandre Drouin](http://graal.ift.ulaval.ca/adrouin) (package maintainer)
+ * [Baptiste Bauvin](https://github.com/babau1)
+ * [Francis Brochu](https://github.com/PhrankBrochu)
+ * [Gaël Letarte St-Pierre](https://github.com/gletarte)
+ * [Mazid Osseni](https://github.com/dizam92)
+ * [Pier-Luc Plante](https://github.com/plpla)
+ * [Thibaud Godon](https://github.com/thibgo)
+
+
```

### Comparing `pyscm-ml-1.0.3/setup.py` & `pyscm-ml-1.1.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,56 +31,52 @@
 # Required for the automatic installation of numpy
 class build_ext(_build_ext):
     def finalize_options(self):
         _build_ext.finalize_options(self)
         # Prevent numpy from thinking it is still in its setup process:
         __builtins__.__NUMPY_SETUP__ = False
         import numpy
+
         self.include_dirs.append(numpy.get_include())
 
 
-solver_module = Extension('pyscm._scm_utility',
-                          language="c++",
-                          sources=['cpp_extensions/utility_python_bindings.cpp',
-                                   'cpp_extensions/solver.cpp'],
-                          extra_compile_args=["-std=c++0x"] + os_compile_flags)
+solver_module = Extension(
+    "pyscm._scm_utility",
+    language="c++",
+    sources=["cpp_extensions/utility_python_bindings.cpp", "cpp_extensions/solver.cpp"],
+    extra_compile_args=["-std=c++0x"] + os_compile_flags,
+)
 
 dependencies = ["numpy", "scipy", "scikit-learn", "six"]
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyscm-ml",
-    version="1.0.3",
+    version="1.1.1",
     packages=find_packages(),
-
-    cmdclass={'build_ext': build_ext},
+    cmdclass={"build_ext": build_ext},
     setup_requires=dependencies,
     install_requires=dependencies,
-
     author="Alexandre Drouin",
     author_email="aldro61@gmail.com",
     maintainer="Alexandre Drouin",
     maintainer_email="aldro61@gmail.com",
     description="The Set Covering Machine algorithm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="GPL-3",
     keywords="machine-learning classification set-covering-machine rule-based-models",
     url="https://github.com/aldro61/pyscm",
-
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Programming Language :: Python",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
         "Intended Audience :: Science/Research",
-        "Topic :: Scientific/Engineering :: Artificial Intelligence"
+        "Topic :: Scientific/Engineering :: Artificial Intelligence",
     ],
-
-
     ext_modules=[solver_module],
-
-    test_suite='nose.collector',
-    tests_require=['nose']
+    test_suite="nose.collector",
+    tests_require=["nose"],
 )
```


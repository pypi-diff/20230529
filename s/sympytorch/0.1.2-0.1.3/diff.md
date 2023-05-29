# Comparing `tmp/sympytorch-0.1.2.tar.gz` & `tmp/sympytorch-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sympytorch-0.1.2.tar", last modified: Sun Apr 16 17:52:13 2023, max compression
+gzip compressed data, was "sympytorch-0.1.3.tar", last modified: Mon May 29 18:55:02 2023, max compression
```

## Comparing `sympytorch-0.1.2.tar` & `sympytorch-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-04-16 17:52:13.898434 sympytorch-0.1.2/
--rw-r--r--   0 kidger    (1000) kidger    (1000)    11357 2023-04-16 17:42:44.000000 sympytorch-0.1.2/LICENSE
--rw-r--r--   0 kidger    (1000) kidger    (1000)       28 2023-04-16 17:42:44.000000 sympytorch-0.1.2/MANIFEST.in
--rw-r--r--   0 kidger    (1000) kidger    (1000)     3227 2023-04-16 17:52:13.898434 sympytorch-0.1.2/PKG-INFO
--rw-r--r--   0 kidger    (1000) kidger    (1000)     2223 2023-04-16 17:42:44.000000 sympytorch-0.1.2/README.md
--rw-r--r--   0 kidger    (1000) kidger    (1000)       38 2023-04-16 17:52:13.898434 sympytorch-0.1.2/setup.cfg
--rw-r--r--   0 kidger    (1000) kidger    (1000)     2136 2023-04-16 17:42:44.000000 sympytorch-0.1.2/setup.py
-drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-04-16 17:52:13.896433 sympytorch-0.1.2/sympytorch/
--rw-r--r--   0 kidger    (1000) kidger    (1000)      101 2023-04-16 17:42:44.000000 sympytorch-0.1.2/sympytorch/__init__.py
--rw-r--r--   0 kidger    (1000) kidger    (1000)      851 2023-04-16 17:42:44.000000 sympytorch-0.1.2/sympytorch/hide_floats_m.py
--rw-r--r--   0 kidger    (1000) kidger    (1000)     6501 2023-04-16 17:50:40.000000 sympytorch-0.1.2/sympytorch/sympy_module.py
-drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-04-16 17:52:13.897434 sympytorch-0.1.2/sympytorch.egg-info/
--rw-r--r--   0 kidger    (1000) kidger    (1000)     3227 2023-04-16 17:52:13.000000 sympytorch-0.1.2/sympytorch.egg-info/PKG-INFO
--rw-r--r--   0 kidger    (1000) kidger    (1000)      318 2023-04-16 17:52:13.000000 sympytorch-0.1.2/sympytorch.egg-info/SOURCES.txt
--rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-04-16 17:52:13.000000 sympytorch-0.1.2/sympytorch.egg-info/dependency_links.txt
--rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-04-16 17:43:02.000000 sympytorch-0.1.2/sympytorch.egg-info/not-zip-safe
--rw-r--r--   0 kidger    (1000) kidger    (1000)       26 2023-04-16 17:52:13.000000 sympytorch-0.1.2/sympytorch.egg-info/requires.txt
--rw-r--r--   0 kidger    (1000) kidger    (1000)       11 2023-04-16 17:52:13.000000 sympytorch-0.1.2/sympytorch.egg-info/top_level.txt
+drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-05-29 18:55:02.025046 sympytorch-0.1.3/
+-rw-r--r--   0 kidger    (1000) kidger    (1000)    11357 2023-04-16 17:42:44.000000 sympytorch-0.1.3/LICENSE
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       28 2023-04-16 17:42:44.000000 sympytorch-0.1.3/MANIFEST.in
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     3227 2023-05-29 18:55:02.025046 sympytorch-0.1.3/PKG-INFO
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     2223 2023-04-16 17:42:44.000000 sympytorch-0.1.3/README.md
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       38 2023-05-29 18:55:02.025046 sympytorch-0.1.3/setup.cfg
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     2136 2023-04-16 17:42:44.000000 sympytorch-0.1.3/setup.py
+drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-05-29 18:55:02.024047 sympytorch-0.1.3/sympytorch/
+-rw-r--r--   0 kidger    (1000) kidger    (1000)      100 2023-05-29 18:54:33.000000 sympytorch-0.1.3/sympytorch/__init__.py
+-rw-r--r--   0 kidger    (1000) kidger    (1000)      851 2023-04-16 17:42:44.000000 sympytorch-0.1.3/sympytorch/hide_floats_m.py
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     6867 2023-05-29 18:54:10.000000 sympytorch-0.1.3/sympytorch/sympy_module.py
+drwxr-xr-x   0 kidger    (1000) kidger    (1000)        0 2023-05-29 18:55:02.025046 sympytorch-0.1.3/sympytorch.egg-info/
+-rw-r--r--   0 kidger    (1000) kidger    (1000)     3227 2023-05-29 18:55:01.000000 sympytorch-0.1.3/sympytorch.egg-info/PKG-INFO
+-rw-r--r--   0 kidger    (1000) kidger    (1000)      318 2023-05-29 18:55:01.000000 sympytorch-0.1.3/sympytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-05-29 18:55:01.000000 sympytorch-0.1.3/sympytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 kidger    (1000) kidger    (1000)        1 2023-04-16 17:43:02.000000 sympytorch-0.1.3/sympytorch.egg-info/not-zip-safe
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       26 2023-05-29 18:55:01.000000 sympytorch-0.1.3/sympytorch.egg-info/requires.txt
+-rw-r--r--   0 kidger    (1000) kidger    (1000)       11 2023-05-29 18:55:01.000000 sympytorch-0.1.3/sympytorch.egg-info/top_level.txt
```

### Comparing `sympytorch-0.1.2/LICENSE` & `sympytorch-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sympytorch-0.1.2/PKG-INFO` & `sympytorch-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympytorch
-Version: 0.1.2
+Version: 0.1.3
 Summary: Turning SymPy expressions into PyTorch modules.
 Home-page: https://github.com/patrick-kidger/sympytorch
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
```

### Comparing `sympytorch-0.1.2/README.md` & `sympytorch-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `sympytorch-0.1.2/setup.py` & `sympytorch-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `sympytorch-0.1.2/sympytorch/hide_floats_m.py` & `sympytorch-0.1.3/sympytorch/hide_floats_m.py`

 * *Files identical despite different names*

### Comparing `sympytorch-0.1.2/sympytorch/sympy_module.py` & `sympytorch-0.1.3/sympytorch/sympy_module.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,21 @@
     # Note: May raise error for integer matrices.
     sympy.Determinant: torch.det,
     sympy.core.numbers.ImaginaryUnit: _I,
     sympy.conjugate: torch.conj,
 
 }
 
+number_symbols = [cls for cls in sympy.NumberSymbol.__subclasses__()]
+
+def number_symbol_to_torch(symbol, *args):
+    return torch.tensor(float(symbol))
+
+_global_func_lookup.update({s: ft.partial(number_symbol_to_torch, s()) for s in number_symbols})
+
 
 class _Node(torch.nn.Module):
     def __init__(self, *, expr, _memodict, _func_lookup, **kwargs):
         super().__init__(**kwargs)
 
         self._sympy_func = expr.func
 
@@ -123,14 +130,16 @@
                 return sympy.S.Half
             else:
                 return self._sympy_func(self._numerator.item(), self._denominator.item())
         elif issubclass(self._sympy_func, sympy.Symbol):
             return self._sympy_func(self._name)
         elif issubclass(self._sympy_func, sympy.core.numbers.ImaginaryUnit):
             return sympy.I
+        elif issubclass(self._sympy_func, sympy.core.numbers.NumberSymbol):
+            return self._sympy_func()
         else:
             if issubclass(self._sympy_func, (sympy.Min, sympy.Max)):
                 evaluate = False
             else:
                 evaluate = True
             args = []
             for arg in self._args:
```

### Comparing `sympytorch-0.1.2/sympytorch.egg-info/PKG-INFO` & `sympytorch-0.1.3/sympytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sympytorch
-Version: 0.1.2
+Version: 0.1.3
 Summary: Turning SymPy expressions into PyTorch modules.
 Home-page: https://github.com/patrick-kidger/sympytorch
 Author: Patrick Kidger
 Author-email: contact@kidger.site
 Maintainer: Patrick Kidger
 Maintainer-email: contact@kidger.site
 License: Apache-2.0
```


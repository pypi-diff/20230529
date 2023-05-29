# Comparing `tmp/encomp-0.9.2.tar.gz` & `tmp/encomp-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encomp-0.9.2.tar", max compression
+gzip compressed data, was "encomp-0.9.3.tar", max compression
```

## Comparing `encomp-0.9.2.tar` & `encomp-0.9.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1072 2023-04-25 07:41:03.603957 encomp-0.9.2/LICENSE
--rw-r--r--   0        0        0    10441 2023-04-25 07:41:03.603957 encomp-0.9.2/README.md
--rw-r--r--   0        0        0       78 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/__init__.py
--rw-r--r--   0        0        0      710 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/constants.py
--rw-r--r--   0        0        0     1895 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/context.py
--rw-r--r--   0        0        0     1976 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/conversion.py
--rw-r--r--   0        0        0     4453 2023-03-12 08:05:11.060958 encomp-0.9.2/encomp/defs/constants.txt
--rw-r--r--   0        0        0    31139 2023-03-12 08:05:11.060958 encomp-0.9.2/encomp/defs/units.txt
--rw-r--r--   0        0        0    44819 2023-05-11 17:03:16.518616 encomp-0.9.2/encomp/fluids.py
--rw-r--r--   0        0        0    12415 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/gases.py
--rw-r--r--   0        0        0     7133 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/math.py
--rw-r--r--   0        0        0     5269 2023-04-25 08:07:46.797762 encomp-0.9.2/encomp/misc.py
--rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.2/encomp/py.typed
--rw-r--r--   0        0        0    14354 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/serialize.py
--rw-r--r--   0        0        0      416 2023-04-25 07:32:25.073969 encomp-0.9.2/encomp/session.py
--rw-r--r--   0        0        0     2645 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/settings.py
--rw-r--r--   0        0        0     2882 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/structures.py
--rw-r--r--   0        0        0    23410 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/sympy.py
--rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.2/encomp/tests/__init__.py
--rw-r--r--   0        0        0      197 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_constants.py
--rw-r--r--   0        0        0      904 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_context.py
--rw-r--r--   0        0        0      934 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_conversion.py
--rw-r--r--   0        0        0    10665 2023-05-11 17:03:39.366721 encomp-0.9.2/encomp/tests/test_fluids.py
--rw-r--r--   0        0        0     3065 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_fluids_types.py
--rw-r--r--   0        0        0     2542 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_function_signatures.py
--rw-r--r--   0        0        0     1103 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_gases.py
--rw-r--r--   0        0        0      189 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_math.py
--rw-r--r--   0        0        0     2066 2023-04-25 08:08:32.357986 encomp-0.9.2/encomp/tests/test_misc.py
--rw-r--r--   0        0        0     1544 2023-05-11 10:09:11.799816 encomp-0.9.2/encomp/tests/test_pandas.py
--rw-r--r--   0        0        0      777 2023-05-11 10:07:40.203132 encomp-0.9.2/encomp/tests/test_polars.py
--rw-r--r--   0        0        0     5478 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_quantity_combined.py
--rw-r--r--   0        0        0     1243 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_quantity_guard.py
--rw-r--r--   0        0        0     5200 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_quantity_inferred.py
--rw-r--r--   0        0        0      649 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_quantity_magnitude.py
--rw-r--r--   0        0        0    23222 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_quantity_types.py
--rw-r--r--   0        0        0     3453 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_serialize.py
--rw-r--r--   0        0        0      124 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_settings.py
--rw-r--r--   0        0        0     1768 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_structures.py
--rw-r--r--   0        0        0     1812 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_sympy.py
--rw-r--r--   0        0        0      929 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/tests/test_thermo.py
--rw-r--r--   0        0        0    36408 2023-05-11 11:02:54.448948 encomp-0.9.2/encomp/tests/test_units.py
--rw-r--r--   0        0        0     6402 2023-04-25 07:41:03.603957 encomp-0.9.2/encomp/thermo.py
--rw-r--r--   0        0        0    42726 2023-05-11 16:37:41.091538 encomp-0.9.2/encomp/units.py
--rw-r--r--   0        0        0    79885 2023-05-11 11:09:23.050144 encomp-0.9.2/encomp/units.pyi
--rw-r--r--   0        0        0    21664 2023-05-11 10:41:15.866326 encomp-0.9.2/encomp/utypes.py
--rw-r--r--   0        0        0     2973 2023-05-11 15:37:39.596907 encomp-0.9.2/pyproject.toml
--rw-r--r--   0        0        0    11685 1970-01-01 00:00:00.000000 encomp-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-04-25 07:41:03.603957 encomp-0.9.3/LICENSE
+-rw-r--r--   0        0        0    10441 2023-04-25 07:41:03.603957 encomp-0.9.3/README.md
+-rw-r--r--   0        0        0       78 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/__init__.py
+-rw-r--r--   0        0        0      710 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/constants.py
+-rw-r--r--   0        0        0     1895 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/context.py
+-rw-r--r--   0        0        0     1976 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/conversion.py
+-rw-r--r--   0        0        0     4453 2023-03-12 08:05:11.060958 encomp-0.9.3/encomp/defs/constants.txt
+-rw-r--r--   0        0        0    31139 2023-03-12 08:05:11.060958 encomp-0.9.3/encomp/defs/units.txt
+-rw-r--r--   0        0        0    44819 2023-05-11 17:03:16.518616 encomp-0.9.3/encomp/fluids.py
+-rw-r--r--   0        0        0    12415 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/gases.py
+-rw-r--r--   0        0        0     7133 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/math.py
+-rw-r--r--   0        0        0     5269 2023-04-25 08:07:46.797762 encomp-0.9.3/encomp/misc.py
+-rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.3/encomp/py.typed
+-rw-r--r--   0        0        0    14354 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/serialize.py
+-rw-r--r--   0        0        0      416 2023-04-25 07:32:25.073969 encomp-0.9.3/encomp/session.py
+-rw-r--r--   0        0        0     2645 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/settings.py
+-rw-r--r--   0        0        0     2882 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/structures.py
+-rw-r--r--   0        0        0    23410 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/sympy.py
+-rw-r--r--   0        0        0        0 2023-03-12 08:05:11.060958 encomp-0.9.3/encomp/tests/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_constants.py
+-rw-r--r--   0        0        0      904 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_context.py
+-rw-r--r--   0        0        0      934 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_conversion.py
+-rw-r--r--   0        0        0    10665 2023-05-11 17:03:39.366721 encomp-0.9.3/encomp/tests/test_fluids.py
+-rw-r--r--   0        0        0     3065 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_fluids_types.py
+-rw-r--r--   0        0        0     2542 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_function_signatures.py
+-rw-r--r--   0        0        0     1103 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_gases.py
+-rw-r--r--   0        0        0      189 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_math.py
+-rw-r--r--   0        0        0     2066 2023-04-25 08:08:32.357986 encomp-0.9.3/encomp/tests/test_misc.py
+-rw-r--r--   0        0        0     1544 2023-05-11 10:09:11.799816 encomp-0.9.3/encomp/tests/test_pandas.py
+-rw-r--r--   0        0        0      777 2023-05-11 10:07:40.203132 encomp-0.9.3/encomp/tests/test_polars.py
+-rw-r--r--   0        0        0     5478 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_quantity_combined.py
+-rw-r--r--   0        0        0     1243 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_quantity_guard.py
+-rw-r--r--   0        0        0     5200 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_quantity_inferred.py
+-rw-r--r--   0        0        0      649 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_quantity_magnitude.py
+-rw-r--r--   0        0        0    23222 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_quantity_types.py
+-rw-r--r--   0        0        0     3453 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_serialize.py
+-rw-r--r--   0        0        0      124 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_settings.py
+-rw-r--r--   0        0        0     1768 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_structures.py
+-rw-r--r--   0        0        0     1812 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_sympy.py
+-rw-r--r--   0        0        0      929 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/tests/test_thermo.py
+-rw-r--r--   0        0        0    36826 2023-05-29 06:48:33.865940 encomp-0.9.3/encomp/tests/test_units.py
+-rw-r--r--   0        0        0     6402 2023-04-25 07:41:03.603957 encomp-0.9.3/encomp/thermo.py
+-rw-r--r--   0        0        0    43840 2023-05-29 07:07:44.710271 encomp-0.9.3/encomp/units.py
+-rw-r--r--   0        0        0    79936 2023-05-29 07:00:53.820668 encomp-0.9.3/encomp/units.pyi
+-rw-r--r--   0        0        0    21664 2023-05-11 10:41:15.866326 encomp-0.9.3/encomp/utypes.py
+-rw-r--r--   0        0        0     2973 2023-05-29 06:45:28.449154 encomp-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0    11685 1970-01-01 00:00:00.000000 encomp-0.9.3/PKG-INFO
```

### Comparing `encomp-0.9.2/LICENSE` & `encomp-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/README.md` & `encomp-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/constants.py` & `encomp-0.9.3/encomp/constants.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/context.py` & `encomp-0.9.3/encomp/context.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/conversion.py` & `encomp-0.9.3/encomp/conversion.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/defs/constants.txt` & `encomp-0.9.3/encomp/defs/constants.txt`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/defs/units.txt` & `encomp-0.9.3/encomp/defs/units.txt`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/fluids.py` & `encomp-0.9.3/encomp/fluids.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/gases.py` & `encomp-0.9.3/encomp/gases.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/math.py` & `encomp-0.9.3/encomp/math.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/misc.py` & `encomp-0.9.3/encomp/misc.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/serialize.py` & `encomp-0.9.3/encomp/serialize.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/settings.py` & `encomp-0.9.3/encomp/settings.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/structures.py` & `encomp-0.9.3/encomp/structures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/sympy.py` & `encomp-0.9.3/encomp/sympy.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_context.py` & `encomp-0.9.3/encomp/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_conversion.py` & `encomp-0.9.3/encomp/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_fluids.py` & `encomp-0.9.3/encomp/tests/test_fluids.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_fluids_types.py` & `encomp-0.9.3/encomp/tests/test_fluids_types.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_function_signatures.py` & `encomp-0.9.3/encomp/tests/test_function_signatures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_gases.py` & `encomp-0.9.3/encomp/tests/test_gases.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_misc.py` & `encomp-0.9.3/encomp/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_pandas.py` & `encomp-0.9.3/encomp/tests/test_pandas.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_polars.py` & `encomp-0.9.3/encomp/tests/test_polars.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_quantity_combined.py` & `encomp-0.9.3/encomp/tests/test_quantity_combined.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_quantity_guard.py` & `encomp-0.9.3/encomp/tests/test_quantity_guard.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_quantity_inferred.py` & `encomp-0.9.3/encomp/tests/test_quantity_inferred.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_quantity_magnitude.py` & `encomp-0.9.3/encomp/tests/test_quantity_magnitude.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_quantity_types.py` & `encomp-0.9.3/encomp/tests/test_quantity_types.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_serialize.py` & `encomp-0.9.3/encomp/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_structures.py` & `encomp-0.9.3/encomp/tests/test_structures.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_sympy.py` & `encomp-0.9.3/encomp/tests/test_sympy.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_thermo.py` & `encomp-0.9.3/encomp/tests/test_thermo.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/tests/test_units.py` & `encomp-0.9.3/encomp/tests/test_units.py`

 * *Files 2% similar despite different names*

```diff
@@ -1332,7 +1332,24 @@
 
     assert isinstance(Q([1, 2, 3]).astype(np.ndarray).m, np.ndarray)
     assert isinstance(Q([1, 2, 3]).astype(pd.Series).m, pd.Series)
     assert isinstance(Q([1, 2, 3]).astype(pl.Series).m, pl.Series)
 
     assert Q([1, 2, 3]).astype(pd.Series, name="s1").m.name == "s1"
     assert Q([1, 2, 3]).astype(pl.Series, name="s1").m.name == "s1"
+
+
+def test_single_element_array_magnitude():
+    s1_list = [1.0]
+    s2_list = [1.0, 2.0]
+
+    Q(s1_list, "kg") * Q(s2_list, "m") / Q(s2_list, "kg")
+
+    s1_arr = np.array([1])
+    s2_arr = np.array([1, 2])
+
+    Q(s1_arr, "kg") * Q(s2_arr, "m") / Q(s2_arr, "kg")
+
+    s1_series = pd.Series([1], name="one")
+    s2_series = pd.Series([1, 2], name="two")
+
+    Q(s1_series, "kg") * Q(s2_series, "m") / Q(s2_series, "kg")
```

### Comparing `encomp-0.9.2/encomp/thermo.py` & `encomp-0.9.3/encomp/thermo.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/encomp/units.py` & `encomp-0.9.3/encomp/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 """
 
 
 from __future__ import annotations
 
 import copy
 import numbers
+import logging
 import re
 import warnings
 from types import UnionType
 from typing import Any, ClassVar, Generic, Iterable, Literal, TypeVar
 
 import numpy as np
 import pandas as pd
@@ -52,14 +53,16 @@
 if SETTINGS.ignore_ndarray_unit_stripped_warning:
     warnings.filterwarnings(
         "ignore",
         message="The unit of the quantity is stripped when downcasting to ndarray.",
     )
 
 
+_LOGGER = logging.getLogger(__name__)
+
 # custom errors inherit from pint.errors.DimensionalityError
 # (which inherits from TypeError)
 # this makes it possible to use
 # try:
 #     ...
 # except DimensionalityError:
 #     ...
@@ -681,14 +684,36 @@
 
                 raise DimensionalityTypeError(
                     f"Cannot convert {self.units} (dimensionality {current_name}) "
                     f"to {unit} (dimensionality {new_name})"
                 )
 
     def _call_subclass(self, *args) -> Quantity[DT, MT]:
+        # handle the edge case where a 1-element pd.Series is
+        # multiplied or divided by an N-element pd.Series
+
+        if "index" in self._original_magnitude_kwargs:
+            index = self._original_magnitude_kwargs["index"]
+
+            try:
+                magnitude_length = len(args[0])
+            except Exception:
+                magnitude_length = None
+
+            if magnitude_length is not None and magnitude_length != len(index):
+                _LOGGER.warning(
+                    f"Length of magnitude index {index} (length {len(index)}) does "
+                    f"not match length of {args[0]} (length {magnitude_length}), "
+                    "the index will be stripped. To avoid this warning, "
+                    "make sure to convert 1-element pd.Series to scalars before "
+                    "multiplying or dividing by another Quantity."
+                )
+
+                del self._original_magnitude_kwargs["index"]
+
         return self.subclass(
             *args,
             _mt_orig=self._original_magnitude_type,
             _mt_orig_kwargs=self._original_magnitude_kwargs,
         )
 
     def to_reduced_units(self) -> Quantity[DT, MT]:
@@ -1021,15 +1046,14 @@
 
             return np.zeros_like(is_equal).astype(bool)
 
         return is_equal and self.is_compatible_with(other)
 
     def __mul__(self, other):
         ret = super().__mul__(other)
-
         if self.dimensionless and isinstance(other, Quantity):
             return other.subclass(ret)
 
         return self._call_subclass(ret)
 
     def __rmul__(self, other):
         ret = super().__rmul__(other)
@@ -1153,14 +1177,18 @@
 
         return subcls(
             ret.m,
             ret.u,
         )
 
     @property
+    def is_scalar(self) -> bool:
+        return isinstance_types(self.m, (float, int))
+
+    @property
     def ndim(self) -> int:
         # compatibility with pandas broadcasting
         # if ndim == 0, pandas considers the object
         # a scalar and will fill array when assigning columns
         # this is similar to setting ureg.force_ndarray_like
         # except that it still allows for scalar magnitudes
```

### Comparing `encomp-0.9.2/encomp/units.pyi` & `encomp-0.9.3/encomp/units.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -164,14 +164,16 @@
     @property
     def m(self) -> MT: ...
     @property
     def u(self) -> Unit[DT]: ...
     @property
     def units(self) -> Unit[DT]: ...
     @property
+    def is_scalar(self) -> bool: ...
+    @property
     def ndim(self) -> int: ...
     def to_reduced_units(self) -> Quantity[DT, MT]: ...
     def to_base_units(self) -> Quantity[DT, MT]: ...
     def asdim(self, other: type[DT_] | Quantity[DT_, MT]) -> Quantity[DT_, MT]: ...
     def astype(self, magnitude_type: type[MT_], **kwargs: Any) -> Quantity[DT, MT_]: ...
     def to(self, unit: Unit[DT] | UnitsContainer | str | dict) -> Quantity[DT, MT]: ...
     def ito(self, unit: Unit[DT] | UnitsContainer | str) -> None: ...
```

### Comparing `encomp-0.9.2/encomp/utypes.py` & `encomp-0.9.3/encomp/utypes.py`

 * *Files identical despite different names*

### Comparing `encomp-0.9.2/pyproject.toml` & `encomp-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "encomp"
-version = "0.9.2"
+version = "0.9.3"
 description = "General-purpose library for engineering calculations"
 authors = ["William Laurén <lauren.william.a@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 packages = [{ include = "encomp" }]
 include = ["encomp/defs"]
```

### Comparing `encomp-0.9.2/PKG-INFO` & `encomp-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encomp
-Version: 0.9.2
+Version: 0.9.3
 Summary: General-purpose library for engineering calculations
 License: MIT
 Author: William Laurén
 Author-email: lauren.william.a@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


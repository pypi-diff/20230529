# Comparing `tmp/PyFinitDiff-0.3.4-py3-none-any.whl.zip` & `tmp/PyFinitDiff-0.3.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,20 @@
-Zip file size: 15894 bytes, number of entries: 16
--rw-r--r--  2.0 unx        0 b- defN 23-Apr-11 23:12 PyFinitDiff/__init__.py
--rw-r--r--  2.0 unx     3506 b- defN 23-Apr-11 23:12 PyFinitDiff/boundaries.py
--rw-r--r--  2.0 unx     8747 b- defN 23-Apr-11 23:12 PyFinitDiff/dense.py
--rw-r--r--  2.0 unx     6530 b- defN 23-Apr-11 23:12 PyFinitDiff/sparse1D.py
--rw-r--r--  2.0 unx     7968 b- defN 23-Apr-11 23:12 PyFinitDiff/sparse2D.py
--rw-r--r--  2.0 unx     8343 b- defN 23-Apr-11 23:12 PyFinitDiff/tools.py
--rw-r--r--  2.0 unx     3606 b- defN 23-Apr-11 23:12 PyFinitDiff/utils.py
--rw-r--r--  2.0 unx     1102 b- defN 23-Apr-11 23:12 PyFinitDiff/coefficients/__init__.py
--rw-r--r--  2.0 unx     1412 b- defN 23-Apr-11 23:12 PyFinitDiff/coefficients/backward.py
--rw-r--r--  2.0 unx     2254 b- defN 23-Apr-11 23:12 PyFinitDiff/coefficients/central.py
--rw-r--r--  2.0 unx     1396 b- defN 23-Apr-11 23:12 PyFinitDiff/coefficients/forward.py
--rw-r--r--  2.0 unx     1072 b- defN 23-Apr-11 23:13 PyFinitDiff-0.3.4.dist-info/LICENSE
--rw-r--r--  2.0 unx     3220 b- defN 23-Apr-11 23:13 PyFinitDiff-0.3.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-11 23:13 PyFinitDiff-0.3.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-11 23:13 PyFinitDiff-0.3.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1326 b- defN 23-Apr-11 23:13 PyFinitDiff-0.3.4.dist-info/RECORD
-16 files, 50586 bytes uncompressed, 13706 bytes compressed:  72.9%
+Zip file size: 16648 bytes, number of entries: 18
+-rw-r--r--  2.0 unx        0 b- defN 23-May-29 16:58 PyFinitDiff/__init__.py
+-rw-r--r--  2.0 unx     3506 b- defN 23-May-29 16:58 PyFinitDiff/boundaries.py
+-rw-r--r--  2.0 unx     8747 b- defN 23-May-29 16:58 PyFinitDiff/dense.py
+-rw-r--r--  2.0 unx     6532 b- defN 23-May-29 16:58 PyFinitDiff/sparse1D.py
+-rw-r--r--  2.0 unx     7970 b- defN 23-May-29 16:58 PyFinitDiff/sparse2D.py
+-rw-r--r--  2.0 unx     8343 b- defN 23-May-29 16:58 PyFinitDiff/triplet.py
+-rw-r--r--  2.0 unx     3608 b- defN 23-May-29 16:58 PyFinitDiff/utils.py
+-rw-r--r--  2.0 unx     1102 b- defN 23-May-29 16:58 PyFinitDiff/coefficients/__init__.py
+-rw-r--r--  2.0 unx     1412 b- defN 23-May-29 16:58 PyFinitDiff/coefficients/backward.py
+-rw-r--r--  2.0 unx     2254 b- defN 23-May-29 16:58 PyFinitDiff/coefficients/central.py
+-rw-r--r--  2.0 unx     1396 b- defN 23-May-29 16:58 PyFinitDiff/coefficients/forward.py
+-rw-r--r--  2.0 unx        0 b- defN 23-May-29 16:58 PyFinitDiff/tools/__init__.py
+-rw-r--r--  2.0 unx      906 b- defN 23-May-29 16:58 PyFinitDiff/tools/directories.py
+-rw-r--r--  2.0 unx     1072 b- defN 23-May-29 16:59 PyFinitDiff-0.3.5.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3220 b- defN 23-May-29 16:59 PyFinitDiff-0.3.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 16:59 PyFinitDiff-0.3.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-29 16:59 PyFinitDiff-0.3.5.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1499 b- defN 23-May-29 16:59 PyFinitDiff-0.3.5.dist-info/RECORD
+18 files, 51671 bytes uncompressed, 14182 bytes compressed:  72.6%
```

## zipnote {}

```diff
@@ -9,15 +9,15 @@
 
 Filename: PyFinitDiff/sparse1D.py
 Comment: 
 
 Filename: PyFinitDiff/sparse2D.py
 Comment: 
 
-Filename: PyFinitDiff/tools.py
+Filename: PyFinitDiff/triplet.py
 Comment: 
 
 Filename: PyFinitDiff/utils.py
 Comment: 
 
 Filename: PyFinitDiff/coefficients/__init__.py
 Comment: 
@@ -27,23 +27,29 @@
 
 Filename: PyFinitDiff/coefficients/central.py
 Comment: 
 
 Filename: PyFinitDiff/coefficients/forward.py
 Comment: 
 
-Filename: PyFinitDiff-0.3.4.dist-info/LICENSE
+Filename: PyFinitDiff/tools/__init__.py
 Comment: 
 
-Filename: PyFinitDiff-0.3.4.dist-info/METADATA
+Filename: PyFinitDiff/tools/directories.py
 Comment: 
 
-Filename: PyFinitDiff-0.3.4.dist-info/WHEEL
+Filename: PyFinitDiff-0.3.5.dist-info/LICENSE
 Comment: 
 
-Filename: PyFinitDiff-0.3.4.dist-info/top_level.txt
+Filename: PyFinitDiff-0.3.5.dist-info/METADATA
 Comment: 
 
-Filename: PyFinitDiff-0.3.4.dist-info/RECORD
+Filename: PyFinitDiff-0.3.5.dist-info/WHEEL
+Comment: 
+
+Filename: PyFinitDiff-0.3.5.dist-info/top_level.txt
+Comment: 
+
+Filename: PyFinitDiff-0.3.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## PyFinitDiff/sparse1D.py

```diff
@@ -1,12 +1,12 @@
 import numpy
 from dataclasses import dataclass, field
 from typing import Dict
 
-from PyFinitDiff.tools import Triplet
+from PyFinitDiff.triplet import Triplet
 from PyFinitDiff.coefficients import FinitCoefficients
 
 
 @dataclass
 class VariableDiagonal1d():
     """
     This class is a construction of diagonals element of the finit-difference method.
```

## PyFinitDiff/sparse2D.py

```diff
@@ -1,15 +1,15 @@
 # Built-in imports
 import numpy
 from dataclasses import dataclass
 
 
 # Local imports
 from PyFinitDiff.coefficients import FinitCoefficients
-from PyFinitDiff.tools import Triplet
+from PyFinitDiff.triplet import Triplet
 from PyFinitDiff.boundaries import Boundaries2D
 
 
 @dataclass
 class VariableDiagonal2d():
     """
     This class is a construction of diagonals element of the finit-difference method.
```

## PyFinitDiff/utils.py

```diff
@@ -1,13 +1,13 @@
 import matplotlib.pyplot as plt
 from collections.abc import Iterable
 import numpy
 import scipy
 
-from PyFinitDiff.tools import DiagonalTriplet
+from PyFinitDiff.triplet import DiagonalTriplet
 
 
 class NameSpace:
     def __init__(self, **kwargs):
         self.__dict__.update(kwargs)
```

## Comparing `PyFinitDiff/tools.py` & `PyFinitDiff/triplet.py`

 * *Files identical despite different names*

## Comparing `PyFinitDiff-0.3.4.dist-info/LICENSE` & `PyFinitDiff-0.3.5.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `PyFinitDiff-0.3.4.dist-info/METADATA` & `PyFinitDiff-0.3.5.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyFinitDiff
-Version: 0.3.4
+Version: 0.3.5
 Summary: A package finit-difference matrix generation.
 Home-page: https://github.com/MartinPdeS/PyFinitDiff
 Author: Martin Poinsinet de Sivry
 Author-email: Martin.poinsinet.de.sivry@gmail.com
 License: MIT
 Platform: unix
 Platform: linux
```

## Comparing `PyFinitDiff-0.3.4.dist-info/RECORD` & `PyFinitDiff-0.3.5.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 PyFinitDiff/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 PyFinitDiff/boundaries.py,sha256=Riz1yaSJAH468pfAEllpUTG8l6syvy5d2Mm7OSs80BQ,3506
 PyFinitDiff/dense.py,sha256=Jc2NzQfOiNzzWPWbSlEEIjKDEg-6nRsRsiG7tDKQCag,8747
-PyFinitDiff/sparse1D.py,sha256=l-Pgh1tJFhKCOxJTfY2Hk5H4JVEiZAjBi0MFpOuo07Q,6530
-PyFinitDiff/sparse2D.py,sha256=iWJxM_VWYbPNbm6NZWYaZxM_OUQXkGdQ40EVlqM2RJY,7968
-PyFinitDiff/tools.py,sha256=f7Bfn7YzyME13mfAiM5YkB4bjl0ThUsm3mbX1PbTwAk,8343
-PyFinitDiff/utils.py,sha256=S_VKMi4zHUq5JWeCdimoMr2wSozQ0LZn1vejrt-CzJU,3606
+PyFinitDiff/sparse1D.py,sha256=wQg1fB5tgK0eKDDr9DaBgXF2pSQldHjyfeKq6xwNJzg,6532
+PyFinitDiff/sparse2D.py,sha256=G5RPJEMwpANKwaODpGbzyzzgzUdBcOHWidb-Q33OCp4,7970
+PyFinitDiff/triplet.py,sha256=f7Bfn7YzyME13mfAiM5YkB4bjl0ThUsm3mbX1PbTwAk,8343
+PyFinitDiff/utils.py,sha256=nmyJgvPUvGe9TXoKZaScNyY88315xjEBtVf30SVh-5E,3608
 PyFinitDiff/coefficients/__init__.py,sha256=OtSx7OJ4HKMHgzbi6wJAT-rSCUjIA8BXcA-82GCSjgk,1102
 PyFinitDiff/coefficients/backward.py,sha256=na_PH1PwgAj6NwiOkiZlcQlR-IfT56OsQ7x0P4xNKsk,1412
 PyFinitDiff/coefficients/central.py,sha256=YItc5ii4sd8MHxJgS9_AK70cC5tLxtN2duOce0ESZOw,2254
 PyFinitDiff/coefficients/forward.py,sha256=5dxhUhSXsX-8OqdIuQmrnJ3jxGftIaMnL-H8kQ43-uo,1396
-PyFinitDiff-0.3.4.dist-info/LICENSE,sha256=U6YG4UEW9XJzHa53oijR0qw6JNN_SZ38WOBmYn3NPd0,1072
-PyFinitDiff-0.3.4.dist-info/METADATA,sha256=FtUO9s8MJcOJ4-8fhpM5IKx__rGxZtg4VxTLDemqiGY,3220
-PyFinitDiff-0.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-PyFinitDiff-0.3.4.dist-info/top_level.txt,sha256=yl_A1Z9VT4HxBK5PTOM4ZyRcXZb-VtbQo1TzRUc1mW4,12
-PyFinitDiff-0.3.4.dist-info/RECORD,,
+PyFinitDiff/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+PyFinitDiff/tools/directories.py,sha256=FU6Cp9_y1yHrA5MNTx3vN3WkBX3hohq6mrWE6Y_FEg4,906
+PyFinitDiff-0.3.5.dist-info/LICENSE,sha256=U6YG4UEW9XJzHa53oijR0qw6JNN_SZ38WOBmYn3NPd0,1072
+PyFinitDiff-0.3.5.dist-info/METADATA,sha256=iYDG0vG1u7kyoOj-AEFAcFlYhgI8BK_KA9EgrDtqO6I,3220
+PyFinitDiff-0.3.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+PyFinitDiff-0.3.5.dist-info/top_level.txt,sha256=yl_A1Z9VT4HxBK5PTOM4ZyRcXZb-VtbQo1TzRUc1mW4,12
+PyFinitDiff-0.3.5.dist-info/RECORD,,
```


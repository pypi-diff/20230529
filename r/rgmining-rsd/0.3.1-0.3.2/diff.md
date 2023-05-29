# Comparing `tmp/rgmining_rsd-0.3.1.tar.gz` & `tmp/rgmining_rsd-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgmining_rsd-0.3.1.tar", max compression
+gzip compressed data, was "rgmining_rsd-0.3.2.tar", max compression
```

## Comparing `rgmining_rsd-0.3.1.tar` & `rgmining_rsd-0.3.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    34500 2023-05-29 04:01:26.003076 rgmining_rsd-0.3.1/COPYING
--rw-r--r--   0        0        0     1998 2023-05-29 04:01:26.003076 rgmining_rsd-0.3.1/README.rst
--rw-r--r--   0        0        0     1948 2023-05-29 04:01:26.003076 rgmining_rsd-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     2293 2023-05-29 04:01:26.003076 rgmining_rsd-0.3.1/rsd/__init__.py
--rw-r--r--   0        0        0    15622 2023-05-29 04:01:26.003076 rgmining_rsd-0.3.1/rsd/graph.py
--rw-r--r--   0        0        0        0 2023-05-29 04:01:26.003076 rgmining_rsd-0.3.1/rsd/py.typed
--rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 rgmining_rsd-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    34500 2023-05-29 04:51:16.645119 rgmining_rsd-0.3.2/COPYING
+-rw-r--r--   0        0        0     1998 2023-05-29 04:51:16.645119 rgmining_rsd-0.3.2/README.rst
+-rw-r--r--   0        0        0     1948 2023-05-29 04:51:16.649119 rgmining_rsd-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2293 2023-05-29 04:51:16.649119 rgmining_rsd-0.3.2/rsd/__init__.py
+-rw-r--r--   0        0        0    15622 2023-05-29 04:51:16.649119 rgmining_rsd-0.3.2/rsd/graph.py
+-rw-r--r--   0        0        0        0 2023-05-29 04:51:16.649119 rgmining_rsd-0.3.2/rsd/py.typed
+-rw-r--r--   0        0        0     3133 1970-01-01 00:00:00.000000 rgmining_rsd-0.3.2/PKG-INFO
```

### Comparing `rgmining_rsd-0.3.1/COPYING` & `rgmining_rsd-0.3.2/COPYING`

 * *Files identical despite different names*

### Comparing `rgmining_rsd-0.3.1/README.rst` & `rgmining_rsd-0.3.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -37,11 +37,11 @@
    :target: https://www.gnu.org/copyleft/gpl.html
 .. |Build Status| image:: https://github.com/rgmining/rsd/actions/workflows/python-lib.yaml/badge.svg
    :target: https://github.com/rgmining/rsd/actions/workflows/python-lib.yaml
 .. |Maintainability| image:: https://api.codeclimate.com/v1/badges/6461704a370307ee0d55/maintainability
    :target: https://codeclimate.com/github/rgmining/rsd/maintainability
 .. |Test Coverage| image:: https://api.codeclimate.com/v1/badges/6461704a370307ee0d55/test_coverage
    :target: https://codeclimate.com/github/rgmining/rsd/test_coverage
-.. |Release| image:: https://img.shields.io/badge/release-0.3.1-brightgreen.svg
+.. |Release| image:: https://img.shields.io/badge/release-0.3.2-brightgreen.svg
    :target: https://pypi.org/project/rgmining-rsd/
 .. |Logo| image:: https://rgmining.github.io/synthetic/_static/image.png
    :target: https://rgmining.github.io/rsd/
```

### Comparing `rgmining_rsd-0.3.1/pyproject.toml` & `rgmining_rsd-0.3.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rgmining-rsd"
-version = "0.3.1"
+version = "0.3.2"
 description = "An implementation of Review Spammer Detection algorithm"
 license = "GPL-3.0-only"
 authors = ["Junpei Kawamoto <kawamoto.junpei@gmail.com>"]
 readme = "README.rst"
 homepage = "https://rgmining.github.io/rsd/"
 repository = "https://github.com/rgmining/rsd"
 documentation = "https://rgmining.github.io/rsd/"
```

### Comparing `rgmining_rsd-0.3.1/rsd/__init__.py` & `rgmining_rsd-0.3.2/rsd/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 .. _ICDM2011: http://ieeexplore.ieee.org/xpl/articleDetails.jsp?arnumber=6137345
 
 """
 from typing import Final
 
 from rsd.graph import ReviewGraph
 
-__version__: Final = "0.3.1"
+__version__: Final = "0.3.2"
 
 __all__: Final = ("ReviewGraph", "__version__")
```

### Comparing `rgmining_rsd-0.3.1/rsd/graph.py` & `rgmining_rsd-0.3.2/rsd/graph.py`

 * *Files identical despite different names*

### Comparing `rgmining_rsd-0.3.1/PKG-INFO` & `rgmining_rsd-0.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rgmining-rsd
-Version: 0.3.1
+Version: 0.3.2
 Summary: An implementation of Review Spammer Detection algorithm
 Home-page: https://rgmining.github.io/rsd/
 License: GPL-3.0-only
 Keywords: review,graph,mining,algorithm,icdm
 Author: Junpei Kawamoto
 Author-email: kawamoto.junpei@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -64,12 +64,12 @@
    :target: https://www.gnu.org/copyleft/gpl.html
 .. |Build Status| image:: https://github.com/rgmining/rsd/actions/workflows/python-lib.yaml/badge.svg
    :target: https://github.com/rgmining/rsd/actions/workflows/python-lib.yaml
 .. |Maintainability| image:: https://api.codeclimate.com/v1/badges/6461704a370307ee0d55/maintainability
    :target: https://codeclimate.com/github/rgmining/rsd/maintainability
 .. |Test Coverage| image:: https://api.codeclimate.com/v1/badges/6461704a370307ee0d55/test_coverage
    :target: https://codeclimate.com/github/rgmining/rsd/test_coverage
-.. |Release| image:: https://img.shields.io/badge/release-0.3.1-brightgreen.svg
+.. |Release| image:: https://img.shields.io/badge/release-0.3.2-brightgreen.svg
    :target: https://pypi.org/project/rgmining-rsd/
 .. |Logo| image:: https://rgmining.github.io/synthetic/_static/image.png
    :target: https://rgmining.github.io/rsd/
```


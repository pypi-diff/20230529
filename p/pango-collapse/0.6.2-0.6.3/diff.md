# Comparing `tmp/pango_collapse-0.6.2.tar.gz` & `tmp/pango_collapse-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pango_collapse-0.6.2.tar", max compression
+gzip compressed data, was "pango_collapse-0.6.3.tar", max compression
```

## Comparing `pango_collapse-0.6.2.tar` & `pango_collapse-0.6.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8598 2023-04-05 02:23:52.880453 pango_collapse-0.6.2/README.md
--rw-r--r--   0        0        0       33 2023-04-05 02:23:52.888454 pango_collapse-0.6.2/pango_collapse/__init__.py
--rw-r--r--   0        0        0       55 2023-04-05 02:23:52.888454 pango_collapse-0.6.2/pango_collapse/__main__.py
--rw-r--r--   0        0        0      324 2023-04-05 02:23:52.888454 pango_collapse-0.6.2/pango_collapse/collapse.txt
--rw-r--r--   0        0        0     1498 2023-04-05 02:23:52.888454 pango_collapse-0.6.2/pango_collapse/collapsor.py
--rw-r--r--   0        0        0     3874 2023-04-05 02:23:52.888454 pango_collapse-0.6.2/pango_collapse/main.py
--rw-r--r--   0        0        0      600 2023-04-05 02:23:52.888454 pango_collapse-0.6.2/pango_collapse/utils.py
--rw-r--r--   0        0        0      539 2023-04-05 02:23:52.888454 pango_collapse-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     9204 1970-01-01 00:00:00.000000 pango_collapse-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     8599 2023-05-29 02:08:01.012774 pango_collapse-0.6.3/README.md
+-rw-r--r--   0        0        0       33 2023-05-29 02:08:01.020774 pango_collapse-0.6.3/pango_collapse/__init__.py
+-rw-r--r--   0        0        0       55 2023-05-29 02:08:01.020774 pango_collapse-0.6.3/pango_collapse/__main__.py
+-rw-r--r--   0        0        0      334 2023-05-29 02:08:01.020774 pango_collapse-0.6.3/pango_collapse/collapse.txt
+-rw-r--r--   0        0        0     1498 2023-05-29 02:08:01.020774 pango_collapse-0.6.3/pango_collapse/collapsor.py
+-rw-r--r--   0        0        0     3874 2023-05-29 02:08:01.020774 pango_collapse-0.6.3/pango_collapse/main.py
+-rw-r--r--   0        0        0      600 2023-05-29 02:08:01.020774 pango_collapse-0.6.3/pango_collapse/utils.py
+-rw-r--r--   0        0        0      539 2023-05-29 02:08:01.020774 pango_collapse-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     9205 1970-01-01 00:00:00.000000 pango_collapse-0.6.3/PKG-INFO
```

### Comparing `pango_collapse-0.6.2/README.md` & `pango_collapse-0.6.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Pango-collapse 
 
 [![](https://img.shields.io/pypi/v/pango-collapse.svg)](https://pypi.org/project/pango-collapse/)
 [![tests](https://github.com/MDU-PHL/pango-collapse/actions/workflows/tests.yaml/badge.svg)](https://github.com/MDU-PHL/pango-collapse/actions/workflows/tests.yaml)
 
-CLI to collapse Pango linages for reporting
+CLI to collapse Pango lineages for reporting
 
 [![](images/collapse.gif)](https://mdu-phl.github.io/pango-watch/tree/)
 
 ## Install 
 
 Install from pypi with pip.
```

### Comparing `pango_collapse-0.6.2/pango_collapse/collapsor.py` & `pango_collapse-0.6.3/pango_collapse/collapsor.py`

 * *Files identical despite different names*

### Comparing `pango_collapse-0.6.2/pango_collapse/main.py` & `pango_collapse-0.6.3/pango_collapse/main.py`

 * *Files identical despite different names*

### Comparing `pango_collapse-0.6.2/pango_collapse/utils.py` & `pango_collapse-0.6.3/pango_collapse/utils.py`

 * *Files identical despite different names*

### Comparing `pango_collapse-0.6.2/pyproject.toml` & `pango_collapse-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pango-collapse"
-version = "0.6.2"
+version = "0.6.3"
 description = ""
 authors = ["wytamma <wytamma.wirth@me.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 pango-collapse = "pango_collapse.main:app"
```

### Comparing `pango_collapse-0.6.2/PKG-INFO` & `pango_collapse-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pango-collapse
-Version: 0.6.2
+Version: 0.6.3
 Summary: 
 Author: wytamma
 Author-email: wytamma.wirth@me.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -17,15 +17,15 @@
 Description-Content-Type: text/markdown
 
 # Pango-collapse 
 
 [![](https://img.shields.io/pypi/v/pango-collapse.svg)](https://pypi.org/project/pango-collapse/)
 [![tests](https://github.com/MDU-PHL/pango-collapse/actions/workflows/tests.yaml/badge.svg)](https://github.com/MDU-PHL/pango-collapse/actions/workflows/tests.yaml)
 
-CLI to collapse Pango linages for reporting
+CLI to collapse Pango lineages for reporting
 
 [![](images/collapse.gif)](https://mdu-phl.github.io/pango-watch/tree/)
 
 ## Install 
 
 Install from pypi with pip.
```


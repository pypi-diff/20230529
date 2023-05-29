# Comparing `tmp/py3d-0.0.95.tar.gz` & `tmp/py3d-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3d-0.0.95.tar", last modified: Mon May 29 15:52:40 2023, max compression
+gzip compressed data, was "py3d-0.0.96.tar", last modified: Mon May 29 15:54:55 2023, max compression
```

## Comparing `py3d-0.0.95.tar` & `py3d-0.0.96.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:52:40.406336 py3d-0.0.95/
--rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-05-29 15:52:40.406336 py3d-0.0.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-05-29 15:52:09.000000 py3d-0.0.95/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:52:40.402336 py3d-0.0.95/py3d/
--rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-29 15:51:25.000000 py3d-0.0.95/py3d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    27956 2023-05-29 15:51:25.000000 py3d-0.0.95/py3d/core.py
--rw-r--r--   0 runner    (1001) docker     (122)    22609 2023-05-29 15:51:25.000000 py3d-0.0.95/py3d/viewer.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:52:40.402336 py3d-0.0.95/py3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-05-29 15:52:40.000000 py3d-0.0.95/py3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-29 15:52:40.000000 py3d-0.0.95/py3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 15:52:40.000000 py3d-0.0.95/py3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-29 15:52:40.000000 py3d-0.0.95/py3d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-29 15:52:40.000000 py3d-0.0.95/py3d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-29 15:52:40.406336 py3d-0.0.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-29 15:51:25.000000 py3d-0.0.95/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:54:55.569288 py3d-0.0.96/
+-rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-05-29 15:54:55.569288 py3d-0.0.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1629 2023-05-29 15:54:29.000000 py3d-0.0.96/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:54:55.569288 py3d-0.0.96/py3d/
+-rw-r--r--   0 runner    (1001) docker     (122)      178 2023-05-29 15:53:50.000000 py3d-0.0.96/py3d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27956 2023-05-29 15:53:50.000000 py3d-0.0.96/py3d/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22609 2023-05-29 15:53:50.000000 py3d-0.0.96/py3d/viewer.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 15:54:55.569288 py3d-0.0.96/py3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2020 2023-05-29 15:54:55.000000 py3d-0.0.96/py3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      204 2023-05-29 15:54:55.000000 py3d-0.0.96/py3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 15:54:55.000000 py3d-0.0.96/py3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       26 2023-05-29 15:54:55.000000 py3d-0.0.96/py3d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        5 2023-05-29 15:54:55.000000 py3d-0.0.96/py3d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-29 15:54:55.569288 py3d-0.0.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1457 2023-05-29 15:53:50.000000 py3d-0.0.96/setup.py
```

### Comparing `py3d-0.0.95/PKG-INFO` & `py3d-0.0.96/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.95
+Version: 0.0.96
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.95/README.md` & `py3d-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `py3d-0.0.95/py3d/core.py` & `py3d-0.0.96/py3d/core.py`

 * *Files identical despite different names*

### Comparing `py3d-0.0.95/py3d/viewer.html` & `py3d-0.0.96/py3d/viewer.html`

 * *Files identical despite different names*

### Comparing `py3d-0.0.95/py3d.egg-info/PKG-INFO` & `py3d-0.0.96/py3d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3d
-Version: 0.0.95
+Version: 0.0.96
 Summary: py3d is a 3d computational geometry library that deals with 3d data in batches. And it embedded an interactive viewer that can work in jupyter notebook.
 Home-page: https://tumiz.github.io/scenario/
 Author: Tumiz
 Author-email: hh11698@163.com
 License: GPL-3.0 License
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
```

### Comparing `py3d-0.0.95/setup.py` & `py3d-0.0.96/setup.py`

 * *Files identical despite different names*


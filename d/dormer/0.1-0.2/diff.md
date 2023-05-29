# Comparing `tmp/dormer-0.1.tar.gz` & `tmp/dormer-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/palfrey/src/dormer/dist/.tmp-f44q1vvx/dormer-0.1.tar", last modified: Mon May 29 20:24:12 2023, max compression
+gzip compressed data, was "/home/palfrey/src/dormer/dist/.tmp-8s6to8il/dormer-0.2.tar", last modified: Mon May 29 20:31:16 2023, max compression
```

## Comparing `dormer-0.1.tar` & `dormer-0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-29 20:24:12.000000 dormer-0.1/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)    34520 2023-05-29 20:16:08.000000 dormer-0.1/LICENSE
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1725 2023-05-29 20:24:12.000000 dormer-0.1/PKG-INFO
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1353 2023-05-29 20:21:23.000000 dormer-0.1/README.md
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-29 20:24:12.000000 dormer-0.1/dormer/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3468 2023-05-29 20:21:23.000000 dormer-0.1/dormer/__init__.py
-drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-29 20:24:12.000000 dormer-0.1/dormer.egg-info/
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1725 2023-05-29 20:24:12.000000 dormer-0.1/dormer.egg-info/PKG-INFO
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      233 2023-05-29 20:24:12.000000 dormer-0.1/dormer.egg-info/SOURCES.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        1 2023-05-29 20:24:12.000000 dormer-0.1/dormer.egg-info/dependency_links.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       39 2023-05-29 20:24:12.000000 dormer-0.1/dormer.egg-info/entry_points.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       13 2023-05-29 20:24:12.000000 dormer-0.1/dormer.egg-info/requires.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)        7 2023-05-29 20:24:12.000000 dormer-0.1/dormer.egg-info/top_level.txt
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)      867 2023-05-29 20:21:23.000000 dormer-0.1/pyproject.toml
--rw-r--r--   0 palfrey   (1000) palfrey   (1000)       38 2023-05-29 20:24:12.000000 dormer-0.1/setup.cfg
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-29 20:31:16.000000 dormer-0.2/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)    34520 2023-05-29 20:16:08.000000 dormer-0.2/LICENSE
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1725 2023-05-29 20:31:16.000000 dormer-0.2/PKG-INFO
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1353 2023-05-29 20:21:23.000000 dormer-0.2/README.md
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-29 20:31:16.000000 dormer-0.2/dormer/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     3468 2023-05-29 20:21:23.000000 dormer-0.2/dormer/__init__.py
+drwxr-xr-x   0 palfrey   (1000) palfrey   (1000)        0 2023-05-29 20:31:16.000000 dormer-0.2/dormer.egg-info/
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)     1725 2023-05-29 20:31:16.000000 dormer-0.2/dormer.egg-info/PKG-INFO
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      233 2023-05-29 20:31:16.000000 dormer-0.2/dormer.egg-info/SOURCES.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        1 2023-05-29 20:31:16.000000 dormer-0.2/dormer.egg-info/dependency_links.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       39 2023-05-29 20:31:16.000000 dormer-0.2/dormer.egg-info/entry_points.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       31 2023-05-29 20:31:16.000000 dormer-0.2/dormer.egg-info/requires.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)        7 2023-05-29 20:31:16.000000 dormer-0.2/dormer.egg-info/top_level.txt
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)      891 2023-05-29 20:31:10.000000 dormer-0.2/pyproject.toml
+-rw-r--r--   0 palfrey   (1000) palfrey   (1000)       38 2023-05-29 20:31:16.000000 dormer-0.2/setup.cfg
```

### Comparing `dormer-0.1/LICENSE` & `dormer-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dormer-0.1/PKG-INFO` & `dormer-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dormer
-Version: 0.1
+Version: 0.2
 Summary: Tool for saving/restoring i3 workspace->output mappings
 Author-email: Tom Parker-Shemilt <palfrey@tevp.net>
 License: AGPL3
 Project-URL: Homepage, https://github.com/palfrey/dormer
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `dormer-0.1/README.md` & `dormer-0.2/README.md`

 * *Files identical despite different names*

### Comparing `dormer-0.1/dormer/__init__.py` & `dormer-0.2/dormer/__init__.py`

 * *Files identical despite different names*

### Comparing `dormer-0.1/dormer.egg-info/PKG-INFO` & `dormer-0.2/dormer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dormer
-Version: 0.1
+Version: 0.2
 Summary: Tool for saving/restoring i3 workspace->output mappings
 Author-email: Tom Parker-Shemilt <palfrey@tevp.net>
 License: AGPL3
 Project-URL: Homepage, https://github.com/palfrey/dormer
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `dormer-0.1/pyproject.toml` & `dormer-0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [project]
 name = "dormer"
-version = "0.1"
+version = "0.2"
 authors = [
     {name = "Tom Parker-Shemilt", email = "palfrey@tevp.net"},
 ]
 description = "Tool for saving/restoring i3 workspace->output mappings"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "AGPL3"}
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dependencies = [
     "i3ipc",
     "pyyaml",
+    "typing_extensions"
 ]
 
 [project.urls]
 Homepage = "https://github.com/palfrey/dormer"
 
 [tool.setuptools.packages.find]
 include = ["dormer"]
```


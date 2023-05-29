# Comparing `tmp/webpy-framework-1.2.0.tar.gz` & `tmp/webpy-framework-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webpy-framework-1.2.0.tar", last modified: Sun May 28 16:38:44 2023, max compression
+gzip compressed data, was "webpy-framework-1.2.1.tar", last modified: Mon May 29 14:37:04 2023, max compression
```

## Comparing `webpy-framework-1.2.0.tar` & `webpy-framework-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 16:38:44.420431 webpy-framework-1.2.0/
--rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.2.0/LICENSE
--rw-rw-rw-   0        0        0     6599 2023-05-28 16:38:44.418395 webpy-framework-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     4651 2023-05-27 01:42:52.000000 webpy-framework-1.2.0/README.md
--rw-rw-rw-   0        0        0     1075 2023-05-28 16:32:53.000000 webpy-framework-1.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 16:38:44.421421 webpy-framework-1.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 16:38:44.394428 webpy-framework-1.2.0/webpy/
--rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.2.0/webpy/__init__.py
--rw-rw-rw-   0        0        0    10754 2023-05-28 01:50:22.000000 webpy-framework-1.2.0/webpy/__main__.py
--rw-rw-rw-   0        0        0     1809 2023-05-27 15:07:10.000000 webpy-framework-1.2.0/webpy/fs_routes.py
--rw-rw-rw-   0        0        0     1492 2023-05-27 15:28:10.000000 webpy-framework-1.2.0/webpy/pysite_semantic_tags.py
--rw-rw-rw-   0        0        0      405 2023-05-28 16:34:47.000000 webpy-framework-1.2.0/webpy/pyx_snippets.py
-drwxrwxrwx   0        0        0        0 2023-05-28 16:38:44.415341 webpy-framework-1.2.0/webpy_framework.egg-info/
--rw-rw-rw-   0        0        0     6599 2023-05-28 16:38:44.000000 webpy-framework-1.2.0/webpy_framework.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-05-28 16:38:44.000000 webpy-framework-1.2.0/webpy_framework.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 16:38:44.000000 webpy-framework-1.2.0/webpy_framework.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-05-28 16:38:44.000000 webpy-framework-1.2.0/webpy_framework.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      155 2023-05-28 16:38:44.000000 webpy-framework-1.2.0/webpy_framework.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 16:38:44.000000 webpy-framework-1.2.0/webpy_framework.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 14:37:04.443269 webpy-framework-1.2.1/
+-rw-rw-rw-   0        0        0     1090 2023-05-26 17:17:20.000000 webpy-framework-1.2.1/LICENSE
+-rw-rw-rw-   0        0        0     6599 2023-05-29 14:37:04.442014 webpy-framework-1.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4651 2023-05-27 01:42:52.000000 webpy-framework-1.2.1/README.md
+-rw-rw-rw-   0        0        0     1116 2023-05-29 14:36:36.000000 webpy-framework-1.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 14:37:04.443269 webpy-framework-1.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 14:37:04.423205 webpy-framework-1.2.1/webpy/
+-rw-rw-rw-   0        0        0     1968 2023-03-17 14:31:38.000000 webpy-framework-1.2.1/webpy/__init__.py
+-rw-rw-rw-   0        0        0    10802 2023-05-29 14:35:09.000000 webpy-framework-1.2.1/webpy/__main__.py
+-rw-rw-rw-   0        0        0     1809 2023-05-27 15:07:10.000000 webpy-framework-1.2.1/webpy/fs_routes.py
+-rw-rw-rw-   0        0        0     1492 2023-05-27 15:28:10.000000 webpy-framework-1.2.1/webpy/pysite_semantic_tags.py
+-rw-rw-rw-   0        0        0      405 2023-05-28 16:34:47.000000 webpy-framework-1.2.1/webpy/pyx_snippets.py
+drwxrwxrwx   0        0        0        0 2023-05-29 14:37:04.439542 webpy-framework-1.2.1/webpy_framework.egg-info/
+-rw-rw-rw-   0        0        0     6599 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      155 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-29 14:37:04.000000 webpy-framework-1.2.1/webpy_framework.egg-info/top_level.txt
```

### Comparing `webpy-framework-1.2.0/LICENSE` & `webpy-framework-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.2.0/PKG-INFO` & `webpy-framework-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.2.0
+Version: 1.2.1
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `webpy-framework-1.2.0/README.md` & `webpy-framework-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.2.0/pyproject.toml` & `webpy-framework-1.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "webpy-framework"
-version = "1.2.0"
+version = "1.2.1"
 description = "Easy-to-use Python web framework built on top of Flask"
 readme = "README.md"
 authors = [{ name = "Carl Furtado", email = "carlzfurtado@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
 	"License :: OSI Approved :: MIT License",
 	"Programming Language :: Python",
@@ -31,8 +31,9 @@
 requires-python = ">= 3.9"
 
 [project.urls]
 Homepage = "https://github.com/User0332/webpy"
 Documentation = "https://webpy-framework.readthedocs.io/"
 
 [project.scripts]
-webpy = "webpy.__main__:main"
+webpy = "webpy.__main__:main"
+webpy-framework = "webpy.__main__:main"
```

### Comparing `webpy-framework-1.2.0/webpy/__init__.py` & `webpy-framework-1.2.1/webpy/__init__.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.2.0/webpy/__main__.py` & `webpy-framework-1.2.1/webpy/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,15 +362,15 @@
 """
 
 defaultrouteconf = {
 	"methods": ["GET"]
 }
 
 def main():
-	parser = ArgumentParser("webpy", description="CLI for the webpy framework")
+	parser = ArgumentParser("webpy", description="CLI for the webpy framework (docs: https://webpy-framework.readthedocs.io/)")
 	parser.add_argument(
 		"command", 
 		choices=(
 		"run",
 		"build",
 		"new",
 		"route",
```

### Comparing `webpy-framework-1.2.0/webpy/fs_routes.py` & `webpy-framework-1.2.1/webpy/fs_routes.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.2.0/webpy/pysite_semantic_tags.py` & `webpy-framework-1.2.1/webpy/pysite_semantic_tags.py`

 * *Files identical despite different names*

### Comparing `webpy-framework-1.2.0/webpy_framework.egg-info/PKG-INFO` & `webpy-framework-1.2.1/webpy_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webpy-framework
-Version: 1.2.0
+Version: 1.2.1
 Summary: Easy-to-use Python web framework built on top of Flask
 Author-email: Carl Furtado <carlzfurtado@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Carl Furtado
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```


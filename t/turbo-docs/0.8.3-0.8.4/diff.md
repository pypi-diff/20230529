# Comparing `tmp/turbo_docs-0.8.3.tar.gz` & `tmp/turbo_docs-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.8.3.tar", last modified: Mon May 29 19:25:03 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.8.4.tar", last modified: Mon May 29 19:37:26 2023, max compression
```

## Comparing `turbo_docs-0.8.3.tar` & `turbo_docs-0.8.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 19:25:03.681383 turbo_docs-0.8.3/
--rw-rw-rw-   0        0        0     2314 2023-05-29 19:25:03.680388 turbo_docs-0.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     1817 2023-05-29 19:21:28.000000 turbo_docs-0.8.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-29 19:25:03.682389 turbo_docs-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0      809 2023-05-29 19:25:00.000000 turbo_docs-0.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:25:03.641137 turbo_docs-0.8.3/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.3/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:25:03.666364 turbo_docs-0.8.3/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.8.3/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     2163 2023-05-26 13:55:07.000000 turbo_docs-0.8.3/turbo_docs/commands/docstring.py
--rw-rw-rw-   0        0        0      731 2023-05-29 19:17:05.000000 turbo_docs-0.8.3/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     1036 2023-05-29 19:09:40.000000 turbo_docs-0.8.3/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:25:03.677375 turbo_docs-0.8.3/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.3/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      653 2023-05-26 14:15:08.000000 turbo_docs-0.8.3/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     2913 2023-05-29 13:41:55.000000 turbo_docs-0.8.3/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0     1581 2023-05-29 19:09:31.000000 turbo_docs-0.8.3/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:25:03.659152 turbo_docs-0.8.3/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2314 2023-05-29 19:25:03.000000 turbo_docs-0.8.3/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-29 19:25:03.000000 turbo_docs-0.8.3/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 19:25:03.000000 turbo_docs-0.8.3/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-29 19:25:03.000000 turbo_docs-0.8.3/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-05-29 19:25:03.000000 turbo_docs-0.8.3/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-29 19:25:03.000000 turbo_docs-0.8.3/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 19:37:26.430960 turbo_docs-0.8.4/
+-rw-rw-rw-   0        0        0     2314 2023-05-29 19:37:26.428904 turbo_docs-0.8.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1817 2023-05-29 19:26:06.000000 turbo_docs-0.8.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 19:37:26.431971 turbo_docs-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0      809 2023-05-29 19:36:49.000000 turbo_docs-0.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:37:26.398384 turbo_docs-0.8.4/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.4/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:37:26.416868 turbo_docs-0.8.4/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.8.4/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2163 2023-05-26 13:55:07.000000 turbo_docs-0.8.4/turbo_docs/commands/docstring.py
+-rw-rw-rw-   0        0        0      731 2023-05-29 19:17:05.000000 turbo_docs-0.8.4/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     1036 2023-05-29 19:09:40.000000 turbo_docs-0.8.4/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:37:26.427866 turbo_docs-0.8.4/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.4/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-05-26 14:15:08.000000 turbo_docs-0.8.4/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2854 2023-05-29 19:36:03.000000 turbo_docs-0.8.4/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0     1581 2023-05-29 19:09:31.000000 turbo_docs-0.8.4/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-05-29 19:37:26.411864 turbo_docs-0.8.4/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2314 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-29 19:37:26.000000 turbo_docs-0.8.4/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.8.3/PKG-INFO` & `turbo_docs-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 0.8.3
+Version: 0.8.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `turbo_docs-0.8.3/README.md` & `turbo_docs-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.3/setup.py` & `turbo_docs-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.8.3",
+	version="0.8.4",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
```

### Comparing `turbo_docs-0.8.3/turbo_docs/commands/docstring.py` & `turbo_docs-0.8.4/turbo_docs/commands/docstring.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.3/turbo_docs/commands/readme.py` & `turbo_docs-0.8.4/turbo_docs/commands/readme.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.3/turbo_docs/generate.py` & `turbo_docs-0.8.4/turbo_docs/generate.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.3/turbo_docs/utils/cli_options.py` & `turbo_docs-0.8.4/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.3/turbo_docs/utils/directory.py` & `turbo_docs-0.8.4/turbo_docs/utils/directory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import fnmatch
 import os
-from pathlib import Path
 import toml
 from typing import List, Dict
 
 
 def read_exclude_config():
     """
     Reads the exclude.toml file and returns the exclude list.
     """
     try:
         with open("exclude.toml", "r") as config_file:
             config_data = toml.load(config_file)
+            exclude = config_data.get("exclude", [])
     except FileNotFoundError:
-        raise ValueError("exclude.toml file is missing.")
-
-    exclude = config_data.get("exclude", [])
-
+        exclude = []
     return exclude
 
 
 def ignored_files_init() -> List[str]:
     """
     Initialize a list of files to be ignored in directory.
     """
```

### Comparing `turbo_docs-0.8.3/turbo_docs/utils/openai_api.py` & `turbo_docs-0.8.4/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.3/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-0.8.4/turbo_docs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-docs
-Version: 0.8.3
+Version: 0.8.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```


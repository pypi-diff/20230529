# Comparing `tmp/turbo_docs-0.8.0.tar.gz` & `tmp/turbo_docs-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\turbo_docs-0.8.0.tar", last modified: Fri May 26 14:19:42 2023, max compression
+gzip compressed data, was "dist\turbo_docs-0.8.1.tar", last modified: Mon May 29 18:30:46 2023, max compression
```

## Comparing `turbo_docs-0.8.0.tar` & `turbo_docs-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 14:19:42.635946 turbo_docs-0.8.0/
--rw-rw-rw-   0        0        0     2080 2023-05-26 14:19:42.634953 turbo_docs-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     1624 2023-05-26 14:19:21.000000 turbo_docs-0.8.0/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 14:19:42.635946 turbo_docs-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0      757 2023-05-26 13:43:40.000000 turbo_docs-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:19:42.607699 turbo_docs-0.8.0/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.0/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:19:42.625803 turbo_docs-0.8.0/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.8.0/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     2163 2023-05-26 13:55:07.000000 turbo_docs-0.8.0/turbo_docs/commands/docstring.py
--rw-rw-rw-   0        0        0      663 2023-05-26 14:15:07.000000 turbo_docs-0.8.0/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     1036 2023-05-26 13:55:51.000000 turbo_docs-0.8.0/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:19:42.632948 turbo_docs-0.8.0/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.0/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      653 2023-05-26 14:15:08.000000 turbo_docs-0.8.0/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1871 2023-04-29 00:25:31.000000 turbo_docs-0.8.0/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0     1581 2023-05-26 14:15:10.000000 turbo_docs-0.8.0/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-05-26 14:19:42.618853 turbo_docs-0.8.0/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2080 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      487 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       51 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 14:19:42.000000 turbo_docs-0.8.0/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 18:30:46.146382 turbo_docs-0.8.1/
+-rw-rw-rw-   0        0        0     3296 2023-05-29 18:30:46.145389 turbo_docs-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2840 2023-05-29 12:31:39.000000 turbo_docs-0.8.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-29 18:30:46.147383 turbo_docs-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      757 2023-05-29 18:30:32.000000 turbo_docs-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:30:46.116678 turbo_docs-0.8.1/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.1/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:30:46.134122 turbo_docs-0.8.1/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-0.8.1/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2163 2023-05-26 13:55:07.000000 turbo_docs-0.8.1/turbo_docs/commands/docstring.py
+-rw-rw-rw-   0        0        0      663 2023-05-26 14:15:07.000000 turbo_docs-0.8.1/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     1036 2023-05-29 13:42:19.000000 turbo_docs-0.8.1/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:30:46.142391 turbo_docs-0.8.1/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-0.8.1/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-05-26 14:15:08.000000 turbo_docs-0.8.1/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     2913 2023-05-29 13:41:55.000000 turbo_docs-0.8.1/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0     1581 2023-05-26 14:15:10.000000 turbo_docs-0.8.1/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-05-29 18:30:46.129084 turbo_docs-0.8.1/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     3296 2023-05-29 18:30:46.000000 turbo_docs-0.8.1/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      487 2023-05-29 18:30:46.000000 turbo_docs-0.8.1/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 18:30:46.000000 turbo_docs-0.8.1/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-05-29 18:30:46.000000 turbo_docs-0.8.1/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       51 2023-05-29 18:30:46.000000 turbo_docs-0.8.1/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-29 18:30:46.000000 turbo_docs-0.8.1/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-0.8.0/setup.py` & `turbo_docs-0.8.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="0.8.0",
+	version="0.8.1",
 	packages=find_packages(),
 	install_requires=[
 		"requests",
 		"openai",
 		"click",
 		"pyperclip",
 		"redbaron",
```

### Comparing `turbo_docs-0.8.0/turbo_docs/commands/docstring.py` & `turbo_docs-0.8.1/turbo_docs/commands/docstring.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.0/turbo_docs/commands/readme.py` & `turbo_docs-0.8.1/turbo_docs/commands/readme.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.0/turbo_docs/generate.py` & `turbo_docs-0.8.1/turbo_docs/generate.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.0/turbo_docs/utils/cli_options.py` & `turbo_docs-0.8.1/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-0.8.0/turbo_docs/utils/directory.py` & `turbo_docs-0.8.1/turbo_docs/utils/directory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,62 +1,101 @@
-import json
+import fnmatch
 import os
 from pathlib import Path
+import toml
 from typing import List, Dict
 
 
+def read_exclude_config():
+    """
+    Reads the exclude.toml file and returns the exclude list.
+    """
+    try:
+        with open("exclude.toml", "r") as config_file:
+            config_data = toml.load(config_file)
+    except FileNotFoundError:
+        raise ValueError("exclude.toml file is missing.")
+
+    exclude = config_data.get("exclude", [])
+
+    return exclude
+
+
 def ignored_files_init() -> List[str]:
     """
     Initialize a list of files to be ignored in directory.
     """
-    ignored_files = ["README.md", "tests", "setup.py"]
+    ignore_files = ["README.md", "tests", "setup.py"]
     for file in os.listdir():
         if file[0] == ".":
-            ignored_files.append(file)
-    return ignored_files
+            ignore_files.append(file)
+    return ignore_files
 
 
 def read_gitignore() -> List[str]:
     """
     Reads in a .gitignore file and returns a list of ignored files.
     """
-    ignore_files = ignored_files_init()
+    ignore_files = []
     try:
         with open(".gitignore", "r") as gitignore:
             for line in gitignore:
                 ignore_files.append(line.strip())
     except FileNotFoundError:
         raise ValueError(
-            ".gitignore file required for excluding files from documentation generation")
+            ".gitignore file required for excluding files from documentation generation"
+        )
     return ignore_files
 
 
-def ignore_filepath(filepath: str, ignore_files: List[str]) -> bool:
+def get_ignore_list() -> List[str]:
     """
-    Check if the given filepath contains any of the given ignored files.
+    Returns a list of files to be ignored in directory.
     """
-    for part in Path(filepath).parts:
-        if part in ignore_files:
-            return True
-    return False
+    ignore_files = ignored_files_init()
+    ignore_files.extend(read_exclude_config())
+    ignore_files.extend(read_gitignore())
+    return ignore_files
+
+
+def matches_ignore_pattern(filepath: str, ignore_patterns: List[str]) -> bool:
+    """
+    Check if the given file path matches any of the ignore patterns.
+    """
+    filepath_parts = filepath.split(os.sep)
+    return any(
+        fnmatch.fnmatch(filepath, pattern)
+        or any(fnmatch.fnmatch(part, pattern) for part in filepath_parts)
+        for pattern in ignore_patterns
+    )
+
+def read_file_content(filepath: str) -> str:
+    """
+    Read the content of the file at the given path.
+    """
+    with open(filepath, "r") as f:
+        content = f.read()
+    return content.replace(" " * 4, "\t").strip()
 
 
 def get_files() -> Dict:
     """
-    Retrieve all text from files, excluding filepaths specified by .gitignore.
+    Retrieve all text from files, excluding filepaths specified by exclude.toml and .gitignore.
     """
     files_dict = {}
-    ignore_files = read_gitignore()
+    ignore_patterns = get_ignore_list()
 
     # Iterate over files
     for root, _, files in os.walk("."):
         for file in files:
-            filepath = os.path.join(root, file).replace(".\\", "")
+            filepath = os.path.join(root, file)
+
+            # If file path or its parent directories match any of the ignore patterns
+            if matches_ignore_pattern(filepath, ignore_patterns):
+                continue
 
             # If not in ignore, collect file text
-            if not ignore_filepath(filepath, ignore_files):
-                with open(filepath, "r") as f:
-                    content = f.read()
-                if content:
-                    files_dict[filepath] = content.replace(
-                        " " * 4, "\t").strip()
+            content = read_file_content(filepath)
+            if content:
+                files_dict[filepath] = content
+
     return files_dict
```

### Comparing `turbo_docs-0.8.0/turbo_docs/utils/openai_api.py` & `turbo_docs-0.8.1/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*


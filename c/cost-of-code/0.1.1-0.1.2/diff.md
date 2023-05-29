# Comparing `tmp/cost-of-code-0.1.1.tar.gz` & `tmp/cost-of-code-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cost-of-code-0.1.1.tar", last modified: Mon May 29 19:22:32 2023, max compression
+gzip compressed data, was "cost-of-code-0.1.2.tar", last modified: Mon May 29 19:46:24 2023, max compression
```

## Comparing `cost-of-code-0.1.1.tar` & `cost-of-code-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:22:32.980672 cost-of-code-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-29 19:22:32.980672 cost-of-code-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:22:32.980672 cost-of-code-0.1.1/cost_of_code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/code_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/cost_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/git_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/test_code_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:22:32.980672 cost-of-code-0.1.1/cost_of_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:22:32.980672 cost-of-code-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:46:24.389992 cost-of-code-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 19:46:24.389992 cost-of-code-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:46:24.385992 cost-of-code-0.1.2/cost_of_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/code_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/cost_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/git_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/test_code_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:46:24.389992 cost-of-code-0.1.2/cost_of_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:46:24.389992 cost-of-code-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/setup.py
```

### Comparing `cost-of-code-0.1.1/PKG-INFO` & `cost-of-code-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cost-of-code
-Version: 0.1.1
+Version: 0.1.2
 Summary: How much would it have cost if GPT-4 had written your code?
 Home-page: https://github.com/Ghost---Shadow/cost-of-code
 Author: Souradeep Nanda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Cost Of Code
 
 How much would it have cost if GPT-4 had written your code?
 
 ## Installation
```

### Comparing `cost-of-code-0.1.1/README.md` & `cost-of-code-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cost-of-code-0.1.1/cost_of_code/git_handler.py` & `cost-of-code-0.1.2/cost_of_code/git_handler.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import difflib
-import os
-from pathspec import PathSpec
-from pathspec.patterns import GitWildMatchPattern
+from pathlib import Path
 
 from git import GitCommandError, Repo, InvalidGitRepositoryError
 
 
 def get_added_lines(directory, extension_whitelist, branch_name):
     try:
         repo = Repo(directory)
@@ -33,54 +31,53 @@
         if item.type == "blob" and any(
             item.path.endswith(ext) for ext in extension_whitelist
         ):
             added_lines.extend(item.data_stream.read().decode().splitlines())
 
     for i in range(len(commits) - 1):
         diffs = commits[i].diff(commits[i + 1])
+        for diff in diffs.iter_change_type("A"):
+            if diff.a_blob is None:  # The file was created in this commit
+                added_lines.extend(diff.b_blob.data_stream.read().decode().splitlines())
         for diff in diffs.iter_change_type("M"):
             if any(diff.a_path.endswith(ext) for ext in extension_whitelist):
-                # Get the content of the file before and after the changes
-                a_data = diff.a_blob.data_stream.read().decode()
-                b_data = diff.b_blob.data_stream.read().decode()
+                a_data = diff.a_blob.data_stream.read().decode() if diff.a_blob else ""
+                b_data = diff.b_blob.data_stream.read().decode() if diff.b_blob else ""
 
                 # Generate the diff using difflib.unified_diff
                 diff_lines = difflib.unified_diff(
                     a_data.splitlines(), b_data.splitlines()
                 )
 
                 # Extract the added lines
                 for line in diff_lines:
                     if line.startswith("+") and not line.startswith("+++"):
                         added_lines.append(line[1:])
 
     return added_lines
 
 
-def get_code_files(directory, extension_whitelist):
+def get_current_lines(directory, extension_whitelist):
+    lines_of_code = []
+
     try:
         repo = Repo(directory)
     except InvalidGitRepositoryError:
         print("Error: The provided directory is not a git repository.")
         exit(1)
 
-    matches = []
+    # Get a list of all files in the repository
+    files_in_repo = repo.git.ls_files().splitlines()
 
-    # Read .gitignore file and create a PathSpec (pattern)
-    with open(os.path.join(directory, ".gitignore"), "r") as f:
-        gitignore = f.read()
-    pathspec = PathSpec.from_lines(GitWildMatchPattern, gitignore.splitlines())
-
-    # Get all files in the current commit
-    files = [
-        item.path for item in repo.head.commit.tree.traverse() if item.type == "blob"
+    # Filter the list of files based on the extension whitelist
+    files_to_check = [
+        file
+        for file in files_in_repo
+        if any(file.endswith(ext) for ext in extension_whitelist)
     ]
 
-    # Filter files by extension and by whether they are ignored
-    for file in files:
-        filename = os.path.basename(file)
-        relpath = os.path.relpath(file, directory)
-        if any(filename.endswith(ext) for ext in extension_whitelist):
-            if not pathspec.match_file(relpath):
-                matches.append(relpath)
+    # For each file, read its content and split it into lines
+    for file_path in files_to_check:
+        with open(Path(directory) / file_path, "r") as file:
+            lines_of_code.extend(file.readlines())
 
-    return matches
+    return lines_of_code
```

### Comparing `cost-of-code-0.1.1/cost_of_code/main.py` & `cost-of-code-0.1.2/cost_of_code/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import argparse
-from cost_of_code.git_handler import get_added_lines, get_code_files
+from cost_of_code.git_handler import get_added_lines, get_current_lines
 from cost_of_code.code_tokenizer import tokenize_code
 from cost_of_code.cost_estimator import estimate_cost
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Estimate the cost of generating the tokens of code in a git repo using GPT-4."
@@ -19,25 +19,23 @@
 
     repo_path = args.repo_path
     branch_name = args.branch_name
     cost_per_thousand_tokens = args.cost_per_thousand_tokens
     extension_whitelist = args.extension_whitelist
 
     # Get all code files in the repo
-    code_files = get_code_files(repo_path, extension_whitelist)
+    current_lines = get_current_lines(repo_path, extension_whitelist)
 
     # Get all added lines in the repo
     added_lines = get_added_lines(repo_path, extension_whitelist, branch_name)
 
     # Tokenize and count tokens in the current state of the repo
     total_tokens_current = 0
-    for file_path in code_files:
-        with open(file_path, "r") as file:
-            code = file.read()
-        total_tokens_current += tokenize_code(code)
+    for line in current_lines:
+        total_tokens_current += tokenize_code(line)
 
     # Tokenize and count tokens in all added lines
     total_tokens_complete = 0
     for line in added_lines:
         total_tokens_complete += tokenize_code(line)
 
     # Calculate the cost for the current state of the repo and all added lines
```

### Comparing `cost-of-code-0.1.1/cost_of_code.egg-info/PKG-INFO` & `cost-of-code-0.1.2/cost_of_code.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: cost-of-code
-Version: 0.1.1
+Version: 0.1.2
 Summary: How much would it have cost if GPT-4 had written your code?
 Home-page: https://github.com/Ghost---Shadow/cost-of-code
 Author: Souradeep Nanda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Cost Of Code
 
 How much would it have cost if GPT-4 had written your code?
 
 ## Installation
```

### Comparing `cost-of-code-0.1.1/setup.py` & `cost-of-code-0.1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # Get the base directory
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
-    name="cost-of-code",  # Replace with your own username
-    version="0.1.1",
+    name="cost-of-code",
+    version="0.1.2",
     author="Souradeep Nanda",
     description="How much would it have cost if GPT-4 had written your code?",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ghost---Shadow/cost-of-code",
     packages=find_packages(),
     install_requires=["GitPython", "tiktoken", "pathspec"],
```


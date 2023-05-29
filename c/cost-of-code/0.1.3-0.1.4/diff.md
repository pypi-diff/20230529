# Comparing `tmp/cost-of-code-0.1.3.tar.gz` & `tmp/cost-of-code-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cost-of-code-0.1.3.tar", last modified: Mon May 29 20:09:50 2023, max compression
+gzip compressed data, was "cost-of-code-0.1.4.tar", last modified: Mon May 29 20:13:29 2023, max compression
```

## Comparing `cost-of-code-0.1.3.tar` & `cost-of-code-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:09:50.192580 cost-of-code-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 20:09:50.192580 cost-of-code-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:09:50.192580 cost-of-code-0.1.3/cost_of_code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/code_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/cost_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/git_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/test_code_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:09:50.192580 cost-of-code-0.1.3/cost_of_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 20:09:50.192580 cost-of-code-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:13:29.674525 cost-of-code-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 20:13:16.000000 cost-of-code-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 20:13:29.674525 cost-of-code-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-29 20:13:16.000000 cost-of-code-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:13:29.674525 cost-of-code-0.1.4/cost_of_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:13:16.000000 cost-of-code-0.1.4/cost_of_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 20:13:16.000000 cost-of-code-0.1.4/cost_of_code/code_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 20:13:16.000000 cost-of-code-0.1.4/cost_of_code/cost_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-05-29 20:13:16.000000 cost-of-code-0.1.4/cost_of_code/git_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-29 20:13:16.000000 cost-of-code-0.1.4/cost_of_code/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-29 20:13:16.000000 cost-of-code-0.1.4/cost_of_code/test_code_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:13:29.674525 cost-of-code-0.1.4/cost_of_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 20:13:29.000000 cost-of-code-0.1.4/cost_of_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 20:13:29.000000 cost-of-code-0.1.4/cost_of_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:13:29.000000 cost-of-code-0.1.4/cost_of_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 20:13:29.000000 cost-of-code-0.1.4/cost_of_code.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-29 20:13:29.000000 cost-of-code-0.1.4/cost_of_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 20:13:29.000000 cost-of-code-0.1.4/cost_of_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 20:13:29.678525 cost-of-code-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-29 20:13:16.000000 cost-of-code-0.1.4/setup.py
```

### Comparing `cost-of-code-0.1.3/LICENSE` & `cost-of-code-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cost-of-code-0.1.3/PKG-INFO` & `cost-of-code-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-of-code
-Version: 0.1.3
+Version: 0.1.4
 Summary: How much would it have cost if GPT-4 had written your code?
 Home-page: https://github.com/Ghost---Shadow/cost-of-code
 Author: Souradeep Nanda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cost-of-code-0.1.3/README.md` & `cost-of-code-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cost-of-code-0.1.3/cost_of_code/git_handler.py` & `cost-of-code-0.1.4/cost_of_code/git_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import difflib
 from pathlib import Path
+from tqdm import tqdm
 
 from git import GitCommandError, Repo, InvalidGitRepositoryError
 
 
 def get_added_lines(directory, extension_whitelist, branch_name):
     try:
         repo = Repo(directory)
@@ -22,21 +23,21 @@
         commits = list(repo.iter_commits(branch_name))[::-1]
     except GitCommandError:
         print(f"Error: The branch '{branch_name}' does not exist in the repository.")
         exit(1)
 
     # Handle the initial commit separately
     initial_commit = commits.pop(0)
-    for item in initial_commit.tree.traverse():
+    for item in tqdm(initial_commit.tree.traverse(), leave=False):
         if item.type == "blob" and any(
             item.path.endswith(ext) for ext in extension_whitelist
         ):
             added_lines.extend(item.data_stream.read().decode().splitlines())
 
-    for i in range(len(commits) - 1):
+    for i in tqdm(range(len(commits) - 1), leave=False):
         diffs = commits[i].diff(commits[i + 1])
         for diff in diffs.iter_change_type("A"):
             if diff.a_blob is None:  # The file was created in this commit
                 added_lines.extend(diff.b_blob.data_stream.read().decode().splitlines())
         for diff in diffs.iter_change_type("M"):
             if any(diff.a_path.endswith(ext) for ext in extension_whitelist):
                 a_data = diff.a_blob.data_stream.read().decode() if diff.a_blob else ""
@@ -71,12 +72,12 @@
     files_to_check = [
         file
         for file in files_in_repo
         if any(file.endswith(ext) for ext in extension_whitelist)
     ]
 
     # For each file, read its content and split it into lines
-    for file_path in files_to_check:
+    for file_path in tqdm(files_to_check, leave=False):
         with open(Path(directory) / file_path, "r") as file:
             lines_of_code.extend(file.readlines())
 
     return lines_of_code
```

### Comparing `cost-of-code-0.1.3/cost_of_code/main.py` & `cost-of-code-0.1.4/cost_of_code/main.py`

 * *Files identical despite different names*

### Comparing `cost-of-code-0.1.3/cost_of_code.egg-info/PKG-INFO` & `cost-of-code-0.1.4/cost_of_code.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-of-code
-Version: 0.1.3
+Version: 0.1.4
 Summary: How much would it have cost if GPT-4 had written your code?
 Home-page: https://github.com/Ghost---Shadow/cost-of-code
 Author: Souradeep Nanda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cost-of-code-0.1.3/setup.py` & `cost-of-code-0.1.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="cost-of-code",
-    version="0.1.3",
+    version="0.1.4",
     author="Souradeep Nanda",
     description="How much would it have cost if GPT-4 had written your code?",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ghost---Shadow/cost-of-code",
     packages=find_packages(),
-    install_requires=["GitPython", "tiktoken", "pathspec"],
+    install_requires=["GitPython", "tiktoken", "pathspec", "tqdm"],
     python_requires=">=3.6",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```


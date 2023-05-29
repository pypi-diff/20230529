# Comparing `tmp/cost-of-code-0.1.2.tar.gz` & `tmp/cost-of-code-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cost-of-code-0.1.2.tar", last modified: Mon May 29 19:46:24 2023, max compression
+gzip compressed data, was "cost-of-code-0.1.3.tar", last modified: Mon May 29 20:09:50 2023, max compression
```

## Comparing `cost-of-code-0.1.2.tar` & `cost-of-code-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:46:24.389992 cost-of-code-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 19:46:24.389992 cost-of-code-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:46:24.385992 cost-of-code-0.1.2/cost_of_code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/code_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/cost_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/git_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/cost_of_code/test_code_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:46:24.389992 cost-of-code-0.1.2/cost_of_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 19:46:24.000000 cost-of-code-0.1.2/cost_of_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:46:24.389992 cost-of-code-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-29 19:46:14.000000 cost-of-code-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:09:50.192580 cost-of-code-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 20:09:50.192580 cost-of-code-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:09:50.192580 cost-of-code-0.1.3/cost_of_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/code_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/cost_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/git_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/cost_of_code/test_code_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:09:50.192580 cost-of-code-0.1.3/cost_of_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 20:09:50.000000 cost-of-code-0.1.3/cost_of_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 20:09:50.192580 cost-of-code-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-29 20:09:33.000000 cost-of-code-0.1.3/setup.py
```

### Comparing `cost-of-code-0.1.2/LICENSE` & `cost-of-code-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cost-of-code-0.1.2/PKG-INFO` & `cost-of-code-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-of-code
-Version: 0.1.2
+Version: 0.1.3
 Summary: How much would it have cost if GPT-4 had written your code?
 Home-page: https://github.com/Ghost---Shadow/cost-of-code
 Author: Souradeep Nanda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cost-of-code-0.1.2/README.md` & `cost-of-code-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cost-of-code-0.1.2/cost_of_code/git_handler.py` & `cost-of-code-0.1.3/cost_of_code/git_handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
     try:
         repo = Repo(directory)
     except InvalidGitRepositoryError:
         print("Error: The provided directory is not a git repository.")
         exit(1)
 
     if repo.is_dirty():
-        print("Error: There are uncommitted changes in the repository.")
-        exit(1)
+        print("Warning: There are uncommitted changes in the repository.")
 
     added_lines = []
 
     # getting commits in chronological order
     try:
         # getting commits in chronological order
         commits = list(repo.iter_commits(branch_name))[::-1]
```

### Comparing `cost-of-code-0.1.2/cost_of_code/main.py` & `cost-of-code-0.1.3/cost_of_code/main.py`

 * *Files identical despite different names*

### Comparing `cost-of-code-0.1.2/cost_of_code.egg-info/PKG-INFO` & `cost-of-code-0.1.3/cost_of_code.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cost-of-code
-Version: 0.1.2
+Version: 0.1.3
 Summary: How much would it have cost if GPT-4 had written your code?
 Home-page: https://github.com/Ghost---Shadow/cost-of-code
 Author: Souradeep Nanda
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `cost-of-code-0.1.2/setup.py` & `cost-of-code-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name="cost-of-code",
-    version="0.1.2",
+    version="0.1.3",
     author="Souradeep Nanda",
     description="How much would it have cost if GPT-4 had written your code?",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Ghost---Shadow/cost-of-code",
     packages=find_packages(),
     install_requires=["GitPython", "tiktoken", "pathspec"],
```


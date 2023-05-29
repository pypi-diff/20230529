# Comparing `tmp/vscode_task_runner-0.1.2.tar.gz` & `tmp/vscode_task_runner-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vscode_task_runner-0.1.2.tar", max compression
+gzip compressed data, was "vscode_task_runner-0.1.3.tar", max compression
```

## Comparing `vscode_task_runner-0.1.2.tar` & `vscode_task_runner-0.1.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1070 2023-05-29 18:23:16.098152 vscode_task_runner-0.1.2/LICENSE
--rw-r--r--   0        0        0     7537 2023-05-29 18:23:16.098152 vscode_task_runner-0.1.2/README.md
--rw-r--r--   0        0        0      844 2023-05-29 18:23:16.098152 vscode_task_runner-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 18:23:16.102152 vscode_task_runner-0.1.2/vtr/__init__.py
--rw-r--r--   0        0        0       39 2023-05-29 18:23:16.102152 vscode_task_runner-0.1.2/vtr/__main__.py
--rw-r--r--   0        0        0     2745 2023-05-29 18:23:16.102152 vscode_task_runner-0.1.2/vtr/console.py
--rw-r--r--   0        0        0     1551 2023-05-29 18:23:16.102152 vscode_task_runner-0.1.2/vtr/constants.py
--rw-r--r--   0        0        0     1193 2023-05-29 18:23:16.102152 vscode_task_runner-0.1.2/vtr/executor.py
--rw-r--r--   0        0        0     3740 2023-05-29 18:23:16.102152 vscode_task_runner-0.1.2/vtr/helpers.py
--rw-r--r--   0        0        0     1835 2023-05-29 18:23:16.102152 vscode_task_runner-0.1.2/vtr/json_parser.py
--rw-r--r--   0        0        0     1464 2023-05-29 18:23:16.102152 vscode_task_runner-0.1.2/vtr/models.py
--rw-r--r--   0        0        0     9296 2023-05-29 18:23:16.102152 vscode_task_runner-0.1.2/vtr/task.py
--rw-r--r--   0        0        0     7497 2023-05-29 18:23:16.102152 vscode_task_runner-0.1.2/vtr/terminal_task_system.py
--rw-r--r--   0        0        0     8048 1970-01-01 00:00:00.000000 vscode_task_runner-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 18:39:14.578192 vscode_task_runner-0.1.3/LICENSE
+-rw-r--r--   0        0        0     7591 2023-05-29 18:39:14.578192 vscode_task_runner-0.1.3/README.md
+-rw-r--r--   0        0        0     1273 2023-05-29 18:39:14.578192 vscode_task_runner-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/__init__.py
+-rw-r--r--   0        0        0       39 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/__main__.py
+-rw-r--r--   0        0        0     2745 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/console.py
+-rw-r--r--   0        0        0     1551 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/constants.py
+-rw-r--r--   0        0        0     1193 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/executor.py
+-rw-r--r--   0        0        0     3740 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/helpers.py
+-rw-r--r--   0        0        0     1835 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/json_parser.py
+-rw-r--r--   0        0        0     1464 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/models.py
+-rw-r--r--   0        0        0     9296 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/task.py
+-rw-r--r--   0        0        0     7497 2023-05-29 18:39:14.582192 vscode_task_runner-0.1.3/vtr/terminal_task_system.py
+-rw-r--r--   0        0        0     8561 1970-01-01 00:00:00.000000 vscode_task_runner-0.1.3/PKG-INFO
```

### Comparing `vscode_task_runner-0.1.2/LICENSE` & `vscode_task_runner-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.2/README.md` & `vscode_task_runner-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 check for merge conflicts................................................Passed
 mixed line ending........................................................Passed
 poetry-check.............................................................Passed
 poetry-lock..............................................................Passed
 absolufy-imports.........................................................Passed
 ruff.....................................................................Passed
 black....................................................................Passed
-vscode-task-runner...................................................................Passed
+pyleft...................................................................Passed
 pyright..................................................................Passed
 markdownlint.............................................................Passed
 ```
 
 Additionally, for convenience, extra arguments can be tacked on to a task.
 For example, you can add extra settings or overrides when running in CI/CD.
 Continuing the example above:
@@ -85,15 +85,15 @@
 check for merge conflicts................................................Passed
 mixed line ending........................................................Passed
 poetry-check.............................................................Passed
 poetry-lock..............................................................Passed
 absolufy-imports.........................................................Passed
 ruff.....................................................................Passed
 black....................................................................Passed
-vscode-task-runner...................................................................Passed
+pyleft...................................................................Passed
 pyright..................................................................Passed
 markdownlint.............................................................Passed
 ```
 
 This can only be used when running a single task.
 
 The `dependsOn` key is also supported:
@@ -137,14 +137,16 @@
 
 ```yaml
 repos:
   - repo: https://github.com/NathanVaughn/vscode-task-runner
     rev: v0.1.2
     hooks:
       - id: vtr
+        # Optionally override the hook name here
+        # name: Build & Test
         args:
           - build # put the tasks you want to run here
           - test
 ```
 
 The pre-commit hook does not match on any file types, and and will always execute.
```

### Comparing `vscode_task_runner-0.1.2/vtr/console.py` & `vscode_task_runner-0.1.3/vtr/console.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.2/vtr/constants.py` & `vscode_task_runner-0.1.3/vtr/constants.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.2/vtr/executor.py` & `vscode_task_runner-0.1.3/vtr/executor.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.2/vtr/helpers.py` & `vscode_task_runner-0.1.3/vtr/helpers.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.2/vtr/json_parser.py` & `vscode_task_runner-0.1.3/vtr/json_parser.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.2/vtr/models.py` & `vscode_task_runner-0.1.3/vtr/models.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.2/vtr/task.py` & `vscode_task_runner-0.1.3/vtr/task.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.2/vtr/terminal_task_system.py` & `vscode_task_runner-0.1.3/vtr/terminal_task_system.py`

 * *Files identical despite different names*

### Comparing `vscode_task_runner-0.1.2/PKG-INFO` & `vscode_task_runner-0.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 Metadata-Version: 2.1
 Name: vscode-task-runner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Task runner for VSCode tasks.json
+Home-page: https://github.com/NathanVaughn/vscode-task-runner
+License: MIT
 Author: Nathan Vaughn
 Author-email: nvaughn51@gmail.com
 Requires-Python: >=3.10,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: dacite (>=1.8.1,<2.0.0)
 Requires-Dist: pyjson5 (>=1.6.2,<2.0.0)
 Requires-Dist: shellingham (>=1.5.0.post1,<2.0.0)
+Project-URL: Issues, https://github.com/NathanVaughn/vscode-task-runner/issues
+Project-URL: Repository, https://github.com/NathanVaughn/vscode-task-runner.git
 Description-Content-Type: text/markdown
 
 # VS Code Task Runner
 
 [![Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
 [![GitHub license](https://img.shields.io/github/license/NathanVaughn/vscode-task-runner)](https://github.com/NathanVaughn/vscode-task-runner/blob/main/LICENSE)
@@ -76,15 +84,15 @@
 check for merge conflicts................................................Passed
 mixed line ending........................................................Passed
 poetry-check.............................................................Passed
 poetry-lock..............................................................Passed
 absolufy-imports.........................................................Passed
 ruff.....................................................................Passed
 black....................................................................Passed
-vscode-task-runner...................................................................Passed
+pyleft...................................................................Passed
 pyright..................................................................Passed
 markdownlint.............................................................Passed
 ```
 
 Additionally, for convenience, extra arguments can be tacked on to a task.
 For example, you can add extra settings or overrides when running in CI/CD.
 Continuing the example above:
@@ -100,15 +108,15 @@
 check for merge conflicts................................................Passed
 mixed line ending........................................................Passed
 poetry-check.............................................................Passed
 poetry-lock..............................................................Passed
 absolufy-imports.........................................................Passed
 ruff.....................................................................Passed
 black....................................................................Passed
-vscode-task-runner...................................................................Passed
+pyleft...................................................................Passed
 pyright..................................................................Passed
 markdownlint.............................................................Passed
 ```
 
 This can only be used when running a single task.
 
 The `dependsOn` key is also supported:
@@ -152,14 +160,16 @@
 
 ```yaml
 repos:
   - repo: https://github.com/NathanVaughn/vscode-task-runner
     rev: v0.1.2
     hooks:
       - id: vtr
+        # Optionally override the hook name here
+        # name: Build & Test
         args:
           - build # put the tasks you want to run here
           - test
 ```
 
 The pre-commit hook does not match on any file types, and and will always execute.
```


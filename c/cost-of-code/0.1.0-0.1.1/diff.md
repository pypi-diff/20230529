# Comparing `tmp/cost-of-code-0.1.0.tar.gz` & `tmp/cost-of-code-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cost-of-code-0.1.0.tar", last modified: Mon May 29 19:17:53 2023, max compression
+gzip compressed data, was "cost-of-code-0.1.1.tar", last modified: Mon May 29 19:22:32 2023, max compression
```

## Comparing `cost-of-code-0.1.0.tar` & `cost-of-code-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:17:53.236239 cost-of-code-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 19:17:53.236239 cost-of-code-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-29 19:17:43.000000 cost-of-code-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:17:53.236239 cost-of-code-0.1.0/cost_of_code/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:17:43.000000 cost-of-code-0.1.0/cost_of_code/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 19:17:43.000000 cost-of-code-0.1.0/cost_of_code/code_tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 19:17:43.000000 cost-of-code-0.1.0/cost_of_code/cost_estimator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-29 19:17:43.000000 cost-of-code-0.1.0/cost_of_code/git_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 19:17:43.000000 cost-of-code-0.1.0/cost_of_code/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-29 19:17:43.000000 cost-of-code-0.1.0/cost_of_code/test_code_tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:17:53.236239 cost-of-code-0.1.0/cost_of_code.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 19:17:53.000000 cost-of-code-0.1.0/cost_of_code.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 19:17:53.000000 cost-of-code-0.1.0/cost_of_code.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:17:53.000000 cost-of-code-0.1.0/cost_of_code.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 19:17:53.000000 cost-of-code-0.1.0/cost_of_code.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 19:17:53.000000 cost-of-code-0.1.0/cost_of_code.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 19:17:53.000000 cost-of-code-0.1.0/cost_of_code.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:17:53.236239 cost-of-code-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-29 19:17:43.000000 cost-of-code-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:22:32.980672 cost-of-code-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-29 19:22:32.980672 cost-of-code-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:22:32.980672 cost-of-code-0.1.1/cost_of_code/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/code_tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/cost_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/git_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/cost_of_code/test_code_tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:22:32.980672 cost-of-code-0.1.1/cost_of_code.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 19:22:32.000000 cost-of-code-0.1.1/cost_of_code.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:22:32.980672 cost-of-code-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-29 19:22:17.000000 cost-of-code-0.1.1/setup.py
```

### Comparing `cost-of-code-0.1.0/README.md` & `cost-of-code-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cost-of-code-0.1.0/cost_of_code/git_handler.py` & `cost-of-code-0.1.1/cost_of_code/git_handler.py`

 * *Files identical despite different names*

### Comparing `cost-of-code-0.1.0/cost_of_code/main.py` & `cost-of-code-0.1.1/cost_of_code/main.py`

 * *Files identical despite different names*


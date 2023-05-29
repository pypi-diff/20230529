# Comparing `tmp/srecli-0.0.5.tar.gz` & `tmp/srecli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "srecli-0.0.5.tar", last modified: Mon May 29 15:02:08 2023, max compression
+gzip compressed data, was "srecli-0.0.6.tar", last modified: Mon May 29 15:58:11 2023, max compression
```

## Comparing `srecli-0.0.5.tar` & `srecli-0.0.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.708823 srecli-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.704823 srecli-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.704823 srecli-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-29 15:01:57.000000 srecli-0.0.5/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 15:01:57.000000 srecli-0.0.5/.github/workflows/pypi_publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-29 15:01:57.000000 srecli-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-29 15:01:57.000000 srecli-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 15:02:08.708823 srecli-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 15:01:57.000000 srecli-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 15:01:57.000000 srecli-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 15:01:57.000000 srecli-0.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:02:08.708823 srecli-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 15:01:57.000000 srecli-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.704823 srecli-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.708823 srecli-0.0.5/src/srecli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:01:57.000000 srecli-0.0.5/src/srecli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-29 15:01:57.000000 srecli-0.0.5/src/srecli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.708823 srecli-0.0.5/src/srecli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:01:57.000000 srecli-0.0.5/src/srecli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-29 15:01:57.000000 srecli-0.0.5/src/srecli/commands/cmd_status.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.708823 srecli-0.0.5/src/srecli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 15:02:08.000000 srecli-0.0.5/src/srecli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:02:08.708823 srecli-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:01:57.000000 srecli-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-29 15:01:57.000000 srecli-0.0.5/tests/test_status_show.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-05-29 15:58:00.000000 srecli-0.0.6/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 15:58:00.000000 srecli-0.0.6/.github/workflows/pypi_publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-29 15:58:00.000000 srecli-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-29 15:58:00.000000 srecli-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-29 15:58:11.803555 srecli-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-29 15:58:00.000000 srecli-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-29 15:58:00.000000 srecli-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 15:58:00.000000 srecli-0.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 15:58:11.803555 srecli-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 15:58:00.000000 srecli-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/src/srecli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:00.000000 srecli-0.0.6/src/srecli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-29 15:58:00.000000 srecli-0.0.6/src/srecli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/src/srecli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:00.000000 srecli-0.0.6/src/srecli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-29 15:58:00.000000 srecli-0.0.6/src/srecli/commands/cmd_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/src/srecli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2390 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 15:58:11.000000 srecli-0.0.6/src/srecli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:11.803555 srecli-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 15:58:00.000000 srecli-0.0.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-29 15:58:00.000000 srecli-0.0.6/tests/test_status_show.py
```

### Comparing `srecli-0.0.5/.github/workflows/build.yaml` & `srecli-0.0.6/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `srecli-0.0.5/.github/workflows/pypi_publish.yaml` & `srecli-0.0.6/.github/workflows/pypi_publish.yaml`

 * *Files identical despite different names*

### Comparing `srecli-0.0.5/.gitignore` & `srecli-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `srecli-0.0.5/LICENSE` & `srecli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `srecli-0.0.5/pyproject.toml` & `srecli-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "srecli"
-version = "0.0.5"
+version = "0.0.6"
 description = "CLI tool for common SRE related work"
 authors = [
     {name = "Shibhikkiran D", email = "shibhikkiran@example.com"},
 ]
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `srecli-0.0.5/src/srecli/cli.py` & `srecli-0.0.6/src/srecli/cli.py`

 * *Files identical despite different names*

### Comparing `srecli-0.0.5/src/srecli/commands/cmd_status.py` & `srecli-0.0.6/src/srecli/commands/cmd_status.py`

 * *Files identical despite different names*

### Comparing `srecli-0.0.5/tests/test_status_show.py` & `srecli-0.0.6/tests/test_status_show.py`

 * *Files identical despite different names*


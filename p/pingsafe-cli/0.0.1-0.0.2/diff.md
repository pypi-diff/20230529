# Comparing `tmp/pingsafe_cli-0.0.1.tar.gz` & `tmp/pingsafe_cli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pingsafe_cli-0.0.1.tar", max compression
+gzip compressed data, was "pingsafe_cli-0.0.2.tar", max compression
```

## Comparing `pingsafe_cli-0.0.1.tar` & `pingsafe_cli-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      223 2023-05-26 11:36:48.516754 pingsafe_cli-0.0.1/LICENSE
--rw-r--r--   0        0        0       15 2023-05-25 13:06:21.256781 pingsafe_cli-0.0.1/README.md
--rw-r--r--   0        0        0      733 2023-05-27 10:00:18.543413 pingsafe_cli-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-23 11:23:40.371904 pingsafe_cli-0.0.1/src/pingsafe_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 11:23:40.524980 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 11:23:40.525045 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-05-23 11:23:40.525113 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/codescanner/__init__.py
--rw-r--r--   0        0        0     2351 2023-05-26 11:36:48.518444 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/codescanner/code_scanner.py
--rw-r--r--   0        0        0     7758 2023-05-27 06:19:12.408155 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/codescanner/secret.py
--rw-r--r--   0        0        0     5800 2023-05-27 06:01:03.181384 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/command_line_arguments.py
--rw-r--r--   0        0        0        0 2023-05-23 11:23:40.525444 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/config/__init__.py
--rw-r--r--   0        0        0      715 2023-05-25 09:26:45.864579 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/config/config.py
--rw-r--r--   0        0        0     2358 2023-05-27 07:42:06.043070 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/main.py
--rw-r--r--   0        0        0     1861 2023-05-27 09:58:35.527021 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/registry.py
--rw-r--r--   0        0        0     9771 2023-05-27 09:30:24.669069 pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/utils.py
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 pingsafe_cli-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      223 2023-05-26 11:36:48.516754 pingsafe_cli-0.0.2/LICENSE
+-rw-r--r--   0        0        0      453 2023-05-29 09:07:45.887168 pingsafe_cli-0.0.2/README.md
+-rw-r--r--   0        0        0      542 2023-05-29 09:05:44.471758 pingsafe_cli-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:40.371904 pingsafe_cli-0.0.2/src/pingsafe_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:40.524980 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:40.525045 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:40.525113 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/codescanner/__init__.py
+-rw-r--r--   0        0        0     2351 2023-05-26 11:36:48.518444 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/codescanner/code_scanner.py
+-rw-r--r--   0        0        0     7758 2023-05-27 06:19:12.408155 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/codescanner/secret.py
+-rw-r--r--   0        0        0     5800 2023-05-27 06:01:03.181384 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/command_line_arguments.py
+-rw-r--r--   0        0        0        0 2023-05-23 11:23:40.525444 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/config/__init__.py
+-rw-r--r--   0        0        0      715 2023-05-25 09:26:45.864579 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/config/config.py
+-rw-r--r--   0        0        0     2358 2023-05-27 07:42:06.043070 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/main.py
+-rw-r--r--   0        0        0     1861 2023-05-29 09:05:55.325411 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/registry.py
+-rw-r--r--   0        0        0     9771 2023-05-27 09:30:24.669069 pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/utils.py
+-rw-r--r--   0        0        0     1192 1970-01-01 00:00:00.000000 pingsafe_cli-0.0.2/PKG-INFO
```

### Comparing `pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/codescanner/code_scanner.py` & `pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/codescanner/code_scanner.py`

 * *Files identical despite different names*

### Comparing `pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/codescanner/secret.py` & `pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/codescanner/secret.py`

 * *Files identical despite different names*

### Comparing `pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/command_line_arguments.py` & `pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/command_line_arguments.py`

 * *Files identical despite different names*

### Comparing `pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/config/config.py` & `pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/config/config.py`

 * *Files identical despite different names*

### Comparing `pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/main.py` & `pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/main.py`

 * *Files identical despite different names*

### Comparing `pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/registry.py` & `pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/registry.py`

 * *Files identical despite different names*

### Comparing `pingsafe_cli-0.0.1/src/pingsafe_cli/scanner/cli/utils.py` & `pingsafe_cli-0.0.2/src/pingsafe_cli/scanner/cli/utils.py`

 * *Files identical despite different names*


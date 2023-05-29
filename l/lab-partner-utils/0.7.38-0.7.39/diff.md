# Comparing `tmp/lab-partner-utils-0.7.38.tar.gz` & `tmp/lab-partner-utils-0.7.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-utils-0.7.38.tar", last modified: Mon May 29 20:43:42 2023, max compression
+gzip compressed data, was "lab-partner-utils-0.7.39.tar", last modified: Mon May 29 20:58:29 2023, max compression
```

## Comparing `lab-partner-utils-0.7.38.tar` & `lab-partner-utils-0.7.39.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:42.117004 lab-partner-utils-0.7.38/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 20:43:03.000000 lab-partner-utils-0.7.38/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 20:43:42.113004 lab-partner-utils-0.7.38/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 20:43:03.000000 lab-partner-utils-0.7.38/README.md
--rw-r--r--   0 root         (0) root         (0)     1744 2023-05-29 20:43:35.000000 lab-partner-utils-0.7.38/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 20:43:03.000000 lab-partner-utils-0.7.38/run.sh
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 20:43:42.117004 lab-partner-utils-0.7.38/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:42.109004 lab-partner-utils-0.7.38/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:42.113004 lab-partner-utils-0.7.38/src/lab_partner_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 20:43:03.000000 lab-partner-utils-0.7.38/src/lab_partner_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 20:43:03.000000 lab-partner-utils-0.7.38/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 20:43:03.000000 lab-partner-utils-0.7.38/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 20:43:03.000000 lab-partner-utils-0.7.38/src/lab_partner_utils/commands.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 20:43:03.000000 lab-partner-utils-0.7.38/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 20:43:03.000000 lab-partner-utils-0.7.38/src/lab_partner_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:43:42.113004 lab-partner-utils-0.7.38/src/lab_partner_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 20:43:42.000000 lab-partner-utils-0.7.38/src/lab_partner_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      540 2023-05-29 20:43:42.000000 lab-partner-utils-0.7.38/src/lab_partner_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 20:43:42.000000 lab-partner-utils-0.7.38/src/lab_partner_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-29 20:43:42.000000 lab-partner-utils-0.7.38/src/lab_partner_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      210 2023-05-29 20:43:42.000000 lab-partner-utils-0.7.38/src/lab_partner_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 20:43:42.000000 lab-partner-utils-0.7.38/src/lab_partner_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:58:29.309747 lab-partner-utils-0.7.39/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 20:57:51.000000 lab-partner-utils-0.7.39/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 20:58:29.309747 lab-partner-utils-0.7.39/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 20:57:51.000000 lab-partner-utils-0.7.39/README.md
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-05-29 20:58:22.000000 lab-partner-utils-0.7.39/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 20:57:51.000000 lab-partner-utils-0.7.39/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 20:58:29.309747 lab-partner-utils-0.7.39/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:58:29.305747 lab-partner-utils-0.7.39/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:58:29.305747 lab-partner-utils-0.7.39/src/lab_partner_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 20:57:51.000000 lab-partner-utils-0.7.39/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 20:57:51.000000 lab-partner-utils-0.7.39/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 20:57:51.000000 lab-partner-utils-0.7.39/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 20:57:51.000000 lab-partner-utils-0.7.39/src/lab_partner_utils/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 20:57:51.000000 lab-partner-utils-0.7.39/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 20:57:51.000000 lab-partner-utils-0.7.39/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 20:58:29.309747 lab-partner-utils-0.7.39/src/lab_partner_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 20:58:29.000000 lab-partner-utils-0.7.39/src/lab_partner_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      540 2023-05-29 20:58:29.000000 lab-partner-utils-0.7.39/src/lab_partner_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 20:58:29.000000 lab-partner-utils-0.7.39/src/lab_partner_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-29 20:58:29.000000 lab-partner-utils-0.7.39/src/lab_partner_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      210 2023-05-29 20:58:29.000000 lab-partner-utils-0.7.39/src/lab_partner_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 20:58:29.000000 lab-partner-utils-0.7.39/src/lab_partner_utils.egg-info/top_level.txt
```

### Comparing `lab-partner-utils-0.7.38/LICENSE.md` & `lab-partner-utils-0.7.39/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.38/PKG-INFO` & `lab-partner-utils-0.7.39/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.38
+Version: 0.7.39
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.38/pyproject.toml` & `lab-partner-utils-0.7.39/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lab-partner-utils"
-version = "0.7.38"
+version = "0.7.39"
 description = "Utilities used to embed Lab Partner into python projects"
 dynamic = ["readme"]
 #dynamic = ["version", "readme"]
 authors = [
     {name = "Anthony Schexnaildre", email = "aps@enclarify.com"},
 ]
 maintainers = [
```

### Comparing `lab-partner-utils-0.7.38/src/lab_partner_utils/cli_command_factory.py` & `lab-partner-utils-0.7.39/src/lab_partner_utils/cli_command_factory.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.38/src/lab_partner_utils/command_builder.py` & `lab-partner-utils-0.7.39/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.38/src/lab_partner_utils/commands.py` & `lab-partner-utils-0.7.39/src/lab_partner_utils/commands.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.38/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-utils-0.7.39/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.38/src/lab_partner_utils/utils.py` & `lab-partner-utils-0.7.39/src/lab_partner_utils/utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.38/src/lab_partner_utils.egg-info/PKG-INFO` & `lab-partner-utils-0.7.39/src/lab_partner_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.38
+Version: 0.7.39
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.38/src/lab_partner_utils.egg-info/SOURCES.txt` & `lab-partner-utils-0.7.39/src/lab_partner_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*


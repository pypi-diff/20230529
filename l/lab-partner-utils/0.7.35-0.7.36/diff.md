# Comparing `tmp/lab-partner-utils-0.7.35.tar.gz` & `tmp/lab-partner-utils-0.7.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lab-partner-utils-0.7.35.tar", last modified: Mon May 29 16:27:59 2023, max compression
+gzip compressed data, was "lab-partner-utils-0.7.36.tar", last modified: Mon May 29 17:12:48 2023, max compression
```

## Comparing `lab-partner-utils-0.7.35.tar` & `lab-partner-utils-0.7.36.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:59.792127 lab-partner-utils-0.7.35/
--rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 16:27:12.000000 lab-partner-utils-0.7.35/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 16:27:59.792127 lab-partner-utils-0.7.35/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 16:27:12.000000 lab-partner-utils-0.7.35/README.md
--rw-r--r--   0 root         (0) root         (0)     1744 2023-05-29 16:27:50.000000 lab-partner-utils-0.7.35/pyproject.toml
--rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 16:27:12.000000 lab-partner-utils-0.7.35/run.sh
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 16:27:59.792127 lab-partner-utils-0.7.35/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:59.784126 lab-partner-utils-0.7.35/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:59.788127 lab-partner-utils-0.7.35/src/lab_partner_utils/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 16:27:12.000000 lab-partner-utils-0.7.35/src/lab_partner_utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 16:27:12.000000 lab-partner-utils-0.7.35/src/lab_partner_utils/cli_command_factory.py
--rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 16:27:12.000000 lab-partner-utils-0.7.35/src/lab_partner_utils/command_builder.py
--rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 16:27:12.000000 lab-partner-utils-0.7.35/src/lab_partner_utils/commands.py
--rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 16:27:12.000000 lab-partner-utils-0.7.35/src/lab_partner_utils/kernel_launcher.py
--rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 16:27:12.000000 lab-partner-utils-0.7.35/src/lab_partner_utils/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 16:27:59.792127 lab-partner-utils-0.7.35/src/lab_partner_utils.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 16:27:59.000000 lab-partner-utils-0.7.35/src/lab_partner_utils.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      540 2023-05-29 16:27:59.000000 lab-partner-utils-0.7.35/src/lab_partner_utils.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 16:27:59.000000 lab-partner-utils-0.7.35/src/lab_partner_utils.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      123 2023-05-29 16:27:59.000000 lab-partner-utils-0.7.35/src/lab_partner_utils.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      210 2023-05-29 16:27:59.000000 lab-partner-utils-0.7.35/src/lab_partner_utils.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 16:27:59.000000 lab-partner-utils-0.7.35/src/lab_partner_utils.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:48.425758 lab-partner-utils-0.7.36/
+-rw-r--r--   0 root         (0) root         (0)     1094 2023-05-29 17:12:09.000000 lab-partner-utils-0.7.36/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 17:12:48.425758 lab-partner-utils-0.7.36/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       65 2023-05-29 17:12:09.000000 lab-partner-utils-0.7.36/README.md
+-rw-r--r--   0 root         (0) root         (0)     1744 2023-05-29 17:12:41.000000 lab-partner-utils-0.7.36/pyproject.toml
+-rwxr-xr-x   0 root         (0) root         (0)      253 2023-05-29 17:12:09.000000 lab-partner-utils-0.7.36/run.sh
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 17:12:48.425758 lab-partner-utils-0.7.36/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:48.421757 lab-partner-utils-0.7.36/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:48.425758 lab-partner-utils-0.7.36/src/lab_partner_utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-29 17:12:09.000000 lab-partner-utils-0.7.36/src/lab_partner_utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8251 2023-05-29 17:12:09.000000 lab-partner-utils-0.7.36/src/lab_partner_utils/cli_command_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1706 2023-05-29 17:12:09.000000 lab-partner-utils-0.7.36/src/lab_partner_utils/command_builder.py
+-rwxr-xr-x   0 root         (0) root         (0)     7252 2023-05-29 17:12:09.000000 lab-partner-utils-0.7.36/src/lab_partner_utils/commands.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2023-05-29 17:12:09.000000 lab-partner-utils-0.7.36/src/lab_partner_utils/kernel_launcher.py
+-rw-r--r--   0 root         (0) root         (0)    13028 2023-05-29 17:12:09.000000 lab-partner-utils-0.7.36/src/lab_partner_utils/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 17:12:48.425758 lab-partner-utils-0.7.36/src/lab_partner_utils.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2011 2023-05-29 17:12:48.000000 lab-partner-utils-0.7.36/src/lab_partner_utils.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      540 2023-05-29 17:12:48.000000 lab-partner-utils-0.7.36/src/lab_partner_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 17:12:48.000000 lab-partner-utils-0.7.36/src/lab_partner_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      123 2023-05-29 17:12:48.000000 lab-partner-utils-0.7.36/src/lab_partner_utils.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      210 2023-05-29 17:12:48.000000 lab-partner-utils-0.7.36/src/lab_partner_utils.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-29 17:12:48.000000 lab-partner-utils-0.7.36/src/lab_partner_utils.egg-info/top_level.txt
```

### Comparing `lab-partner-utils-0.7.35/LICENSE.md` & `lab-partner-utils-0.7.36/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.35/PKG-INFO` & `lab-partner-utils-0.7.36/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.35
+Version: 0.7.36
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.35/pyproject.toml` & `lab-partner-utils-0.7.36/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=45", "wheel", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lab-partner-utils"
-version = "0.7.35"
+version = "0.7.36"
 description = "Utilities used to embed Lab Partner into python projects"
 dynamic = ["readme"]
 #dynamic = ["version", "readme"]
 authors = [
     {name = "Anthony Schexnaildre", email = "aps@enclarify.com"},
 ]
 maintainers = [
```

### Comparing `lab-partner-utils-0.7.35/src/lab_partner_utils/cli_command_factory.py` & `lab-partner-utils-0.7.36/src/lab_partner_utils/cli_command_factory.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.35/src/lab_partner_utils/command_builder.py` & `lab-partner-utils-0.7.36/src/lab_partner_utils/command_builder.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.35/src/lab_partner_utils/commands.py` & `lab-partner-utils-0.7.36/src/lab_partner_utils/commands.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.35/src/lab_partner_utils/kernel_launcher.py` & `lab-partner-utils-0.7.36/src/lab_partner_utils/kernel_launcher.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.35/src/lab_partner_utils/utils.py` & `lab-partner-utils-0.7.36/src/lab_partner_utils/utils.py`

 * *Files identical despite different names*

### Comparing `lab-partner-utils-0.7.35/src/lab_partner_utils.egg-info/PKG-INFO` & `lab-partner-utils-0.7.36/src/lab_partner_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lab-partner-utils
-Version: 0.7.35
+Version: 0.7.36
 Summary: Utilities used to embed Lab Partner into python projects
 Author-email: Anthony Schexnaildre <aps@enclarify.com>
 Maintainer-email: Anthony Schexnaildre <aps@enclarify.com>
 License: # Released under MIT License
         
         Copyright (c) 2021 Anthony Schexnaildre.
```

### Comparing `lab-partner-utils-0.7.35/src/lab_partner_utils.egg-info/SOURCES.txt` & `lab-partner-utils-0.7.36/src/lab_partner_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*


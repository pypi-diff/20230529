# Comparing `tmp/driveup-0.6.5.tar.gz` & `tmp/driveup-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "driveup-0.6.5.tar", last modified: Thu May 18 10:57:16 2023, max compression
+gzip compressed data, was "driveup-0.7.0.tar", last modified: Mon May 29 11:16:00 2023, max compression
```

## Comparing `driveup-0.6.5.tar` & `driveup-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:57:16.040570 driveup-0.6.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:57:16.040570 driveup-0.6.5/Driveup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:57:00.000000 driveup-0.6.5/Driveup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11643 2023-05-18 10:57:00.000000 driveup-0.6.5/Driveup/drive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:57:16.040570 driveup-0.6.5/Driveup/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 10:57:00.000000 driveup-0.6.5/Driveup/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-18 10:57:00.000000 driveup-0.6.5/Driveup/features/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-18 10:57:00.000000 driveup-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-18 10:57:16.040570 driveup-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-18 10:57:00.000000 driveup-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 10:57:16.040570 driveup-0.6.5/driveup.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-18 10:57:16.000000 driveup-0.6.5/driveup.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 10:57:16.000000 driveup-0.6.5/driveup.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 10:57:16.000000 driveup-0.6.5/driveup.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-18 10:57:16.000000 driveup-0.6.5/driveup.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 10:57:16.000000 driveup-0.6.5/driveup.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 10:57:16.040570 driveup-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-18 10:57:00.000000 driveup-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:16:00.446752 driveup-0.7.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:16:00.442752 driveup-0.7.0/Driveup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7418 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/drive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:16:00.442752 driveup-0.7.0/Driveup/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/features/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/features/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-05-29 11:15:48.000000 driveup-0.7.0/Driveup/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 11:15:48.000000 driveup-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-29 11:16:00.446752 driveup-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-29 11:15:48.000000 driveup-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 11:16:00.446752 driveup-0.7.0/driveup.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-29 11:16:00.000000 driveup-0.7.0/driveup.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-29 11:16:00.000000 driveup-0.7.0/driveup.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 11:16:00.000000 driveup-0.7.0/driveup.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-29 11:16:00.000000 driveup-0.7.0/driveup.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 11:16:00.000000 driveup-0.7.0/driveup.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 11:16:00.446752 driveup-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-29 11:15:48.000000 driveup-0.7.0/setup.py
```

### Comparing `driveup-0.6.5/Driveup/features/auth.py` & `driveup-0.7.0/Driveup/features/auth.py`

 * *Files identical despite different names*

### Comparing `driveup-0.6.5/LICENSE` & `driveup-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `driveup-0.6.5/PKG-INFO` & `driveup-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: driveup
-Version: 0.6.5
+Version: 0.7.0
 Summary: Python package for uploading files and folders to Google Drive.
 Home-page: https://github.com/raul-martin-dev/Driveup
 Author: Raúl M.R.
 Author-email: raul.martin4bc@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-Metadata-Version: 2.1 Name: driveup Version: 0.6.5 Summary: Python package for
+Metadata-Version: 2.1 Name: driveup Version: 0.7.0 Summary: Python package for
 uploading files and folders to Google Drive. Home-page: https://github.com/
 raul-martin-dev/Driveup Author: RaÃºl M.R. Author-email:
 raul.martin4bc@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Python package for uploading files and folders to Google
 Drive
                               [PyPI] [downloads]
```

### Comparing `driveup-0.6.5/driveup.egg-info/PKG-INFO` & `driveup-0.7.0/driveup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: driveup
-Version: 0.6.5
+Version: 0.7.0
 Summary: Python package for uploading files and folders to Google Drive.
 Home-page: https://github.com/raul-martin-dev/Driveup
 Author: Raúl M.R.
 Author-email: raul.martin4bc@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,7 +1,7 @@
-Metadata-Version: 2.1 Name: driveup Version: 0.6.5 Summary: Python package for
+Metadata-Version: 2.1 Name: driveup Version: 0.7.0 Summary: Python package for
 uploading files and folders to Google Drive. Home-page: https://github.com/
 raul-martin-dev/Driveup Author: RaÃºl M.R. Author-email:
 raul.martin4bc@gmail.com License: MIT Description-Content-Type: text/markdown
 License-File: LICENSE Python package for uploading files and folders to Google
 Drive
                               [PyPI] [downloads]
```


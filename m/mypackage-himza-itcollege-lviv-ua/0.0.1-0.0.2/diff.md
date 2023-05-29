# Comparing `tmp/mypackage_himza_itcollege_lviv_ua-0.0.1.tar.gz` & `tmp/mypackage_himza_itcollege_lviv_ua-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackage_himza_itcollege_lviv_ua-0.0.1.tar", last modified: Mon May 29 16:34:02 2023, max compression
+gzip compressed data, was "mypackage_himza_itcollege_lviv_ua-0.0.2.tar", last modified: Mon May 29 13:32:05 2023, max compression
```

## Comparing `mypackage_himza_itcollege_lviv_ua-0.0.1.tar` & `mypackage_himza_itcollege_lviv_ua-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:34:02.680170 mypackage_himza_itcollege_lviv_ua-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:33:54.000000 mypackage_himza_itcollege_lviv_ua-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-29 16:34:02.680170 mypackage_himza_itcollege_lviv_ua-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-29 16:33:54.000000 mypackage_himza_itcollege_lviv_ua-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-29 16:33:54.000000 mypackage_himza_itcollege_lviv_ua-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-29 16:34:02.684171 mypackage_himza_itcollege_lviv_ua-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:34:02.676170 mypackage_himza_itcollege_lviv_ua-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:34:02.680170 mypackage_himza_itcollege_lviv_ua-0.0.1/src/mypackage_himza_itcollege_lviv_ua/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:33:54.000000 mypackage_himza_itcollege_lviv_ua-0.0.1/src/mypackage_himza_itcollege_lviv_ua/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-29 16:33:54.000000 mypackage_himza_itcollege_lviv_ua-0.0.1/src/mypackage_himza_itcollege_lviv_ua/example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:34:02.680170 mypackage_himza_itcollege_lviv_ua-0.0.1/src/mypackage_himza_itcollege_lviv_ua.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-29 16:34:02.000000 mypackage_himza_itcollege_lviv_ua-0.0.1/src/mypackage_himza_itcollege_lviv_ua.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-29 16:34:02.000000 mypackage_himza_itcollege_lviv_ua-0.0.1/src/mypackage_himza_itcollege_lviv_ua.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:34:02.000000 mypackage_himza_itcollege_lviv_ua-0.0.1/src/mypackage_himza_itcollege_lviv_ua.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 16:34:02.000000 mypackage_himza_itcollege_lviv_ua-0.0.1/src/mypackage_himza_itcollege_lviv_ua.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 13:32:05.144586 mypackage_himza_itcollege_lviv_ua-0.0.2/
+-rw-rw-rw-   0        0        0        0 2023-05-29 13:01:25.000000 mypackage_himza_itcollege_lviv_ua-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      613 2023-05-29 13:32:05.145128 mypackage_himza_itcollege_lviv_ua-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2023-05-29 13:30:56.000000 mypackage_himza_itcollege_lviv_ua-0.0.2/README.md
+-rw-rw-rw-   0        0        0      108 2023-05-29 13:05:36.000000 mypackage_himza_itcollege_lviv_ua-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      693 2023-05-29 13:32:05.148086 mypackage_himza_itcollege_lviv_ua-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 13:32:05.071289 mypackage_himza_itcollege_lviv_ua-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 13:32:05.110264 mypackage_himza_itcollege_lviv_ua-0.0.2/src/mypackage_himza_itcollege_lviv_ua/
+-rw-rw-rw-   0        0        0        0 2023-05-29 13:02:47.000000 mypackage_himza_itcollege_lviv_ua-0.0.2/src/mypackage_himza_itcollege_lviv_ua/__init__.py
+-rw-rw-rw-   0        0        0       71 2023-05-29 13:22:54.000000 mypackage_himza_itcollege_lviv_ua-0.0.2/src/mypackage_himza_itcollege_lviv_ua/example.py
+drwxrwxrwx   0        0        0        0 2023-05-29 13:32:05.142873 mypackage_himza_itcollege_lviv_ua-0.0.2/src/mypackage_himza_itcollege_lviv_ua.egg-info/
+-rw-rw-rw-   0        0        0      613 2023-05-29 13:32:05.000000 mypackage_himza_itcollege_lviv_ua-0.0.2/src/mypackage_himza_itcollege_lviv_ua.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-05-29 13:32:05.000000 mypackage_himza_itcollege_lviv_ua-0.0.2/src/mypackage_himza_itcollege_lviv_ua.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 13:32:05.000000 mypackage_himza_itcollege_lviv_ua-0.0.2/src/mypackage_himza_itcollege_lviv_ua.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-29 13:32:05.000000 mypackage_himza_itcollege_lviv_ua-0.0.2/src/mypackage_himza_itcollege_lviv_ua.egg-info/top_level.txt
```

### Comparing `mypackage_himza_itcollege_lviv_ua-0.0.1/src/mypackage_himza_itcollege_lviv_ua.egg-info/PKG-INFO` & `mypackage_himza_itcollege_lviv_ua-0.0.2/src/mypackage_himza_itcollege_lviv_ua.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
-Name: mypackage-himza-itcollege-lviv-ua
-Version: 0.0.1
-Summary: Module for creating an email address
-Home-page: https://github.com/pypa/sampleproject
-Author: Dmytro Himza
-Author-email: dhimza2020@itcollege.lviv.ua
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# Example Package
-
-Module for creating an email address
+Metadata-Version: 2.1
+Name: mypackage-himza-itcollege-lviv-ua
+Version: 0.0.2
+Summary: Module for creating an email address
+Home-page: https://github.com/pypa/sampleproject
+Author: Dmytro Himza
+Author-email: dhimza2020@itcollege.lviv.ua
+Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# Example Package
+
+Module for creating an email address
```


# Comparing `tmp/openirt-0.1.1.tar.gz` & `tmp/openirt-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openirt-0.1.1.tar", last modified: Wed Mar  1 13:10:04 2023, max compression
+gzip compressed data, was "openirt-0.1.2.tar", last modified: Mon May 29 12:12:37 2023, max compression
```

## Comparing `openirt-0.1.1.tar` & `openirt-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 13:10:04.723431 openirt-0.1.1/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-03-01 13:09:32.000000 openirt-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      256 2023-03-01 13:10:04.723431 openirt-0.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-03-01 13:09:32.000000 openirt-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 13:10:04.714264 openirt-0.1.1/openirt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-01 13:09:32.000000 openirt-0.1.1/openirt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-03-01 13:09:32.000000 openirt-0.1.1/openirt/irtfunc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 13:10:04.717014 openirt-0.1.1/openirt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      256 2023-03-01 13:10:04.000000 openirt-0.1.1/openirt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      208 2023-03-01 13:10:04.000000 openirt-0.1.1/openirt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-01 13:10:04.000000 openirt-0.1.1/openirt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-03-01 13:10:04.000000 openirt-0.1.1/openirt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-01 13:10:04.723431 openirt-0.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-03-01 13:09:32.000000 openirt-0.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-01 13:10:04.717014 openirt-0.1.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-03-01 13:09:32.000000 openirt-0.1.1/tests/test_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 12:12:37.266515 openirt-0.1.2/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-29 12:12:15.000000 openirt-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-29 12:12:37.266515 openirt-0.1.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-29 12:12:15.000000 openirt-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 12:12:37.264515 openirt-0.1.2/openirt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6938 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/bayes3PL.py
+-rw-rw-rw-   0 root         (0) root         (0)     2081 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3930 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/irt_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1489 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/item_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/logistic_1P_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4293 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/logistic_3PM.py
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/norm_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3049 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/pl2.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-29 12:12:15.000000 openirt-0.1.2/openirt/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 12:12:37.265515 openirt-0.1.2/openirt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-29 12:12:37.000000 openirt-0.1.2/openirt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      376 2023-05-29 12:12:37.000000 openirt-0.1.2/openirt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 12:12:37.000000 openirt-0.1.2/openirt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-29 12:12:37.000000 openirt-0.1.2/openirt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 12:12:37.266515 openirt-0.1.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-29 12:12:15.000000 openirt-0.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 12:12:37.265515 openirt-0.1.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-29 12:12:15.000000 openirt-0.1.2/tests/test_func.py
```

### Comparing `openirt-0.1.1/LICENSE` & `openirt-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openirt-0.1.1/setup.py` & `openirt-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 
 setup(
     name='openirt',
     packages = find_packages(include=['openirt']),
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     url='https://gitlab.com/pleased/...',
-    version='0.1.1',
+    version='0.1.2',
     description='Item response theory toolkit',
     author='Johan Hay',
     license='MIT',
 )
```


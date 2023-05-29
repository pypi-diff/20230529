# Comparing `tmp/torchdevice-0.1.0.tar.gz` & `tmp/torchdevice-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchdevice-0.1.0.tar", last modified: Wed Feb  9 11:20:18 2022, max compression
+gzip compressed data, was "torchdevice-0.2.0.tar", last modified: Mon May 29 13:28:58 2023, max compression
```

## Comparing `torchdevice-0.1.0.tar` & `torchdevice-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 11:20:18.380533 torchdevice-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-02-09 11:20:18.380533 torchdevice-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      399 2022-02-09 11:20:07.000000 torchdevice-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-09 11:20:18.380533 torchdevice-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      548 2022-02-09 11:20:07.000000 torchdevice-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 11:20:18.380533 torchdevice-0.1.0/torchdevice/
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-02-09 11:20:07.000000 torchdevice-0.1.0/torchdevice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1079 2022-02-09 11:20:07.000000 torchdevice-0.1.0/torchdevice/cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-09 11:20:18.380533 torchdevice-0.1.0/torchdevice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-02-09 11:20:18.000000 torchdevice-0.1.0/torchdevice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      236 2022-02-09 11:20:18.000000 torchdevice-0.1.0/torchdevice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-09 11:20:18.000000 torchdevice-0.1.0/torchdevice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-02-09 11:20:18.000000 torchdevice-0.1.0/torchdevice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-02-09 11:20:18.000000 torchdevice-0.1.0/torchdevice.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:28:58.041492 torchdevice-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 13:28:58.041492 torchdevice-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-29 13:28:46.000000 torchdevice-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 13:28:58.041492 torchdevice-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-29 13:28:46.000000 torchdevice-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:28:58.041492 torchdevice-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-29 13:28:46.000000 torchdevice-0.2.0/tests/test_hello.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:28:58.041492 torchdevice-0.2.0/torchdevice/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-29 13:28:46.000000 torchdevice-0.2.0/torchdevice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-29 13:28:46.000000 torchdevice-0.2.0/torchdevice/cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:28:58.041492 torchdevice-0.2.0/torchdevice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-29 13:28:58.000000 torchdevice-0.2.0/torchdevice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-29 13:28:58.000000 torchdevice-0.2.0/torchdevice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:28:58.000000 torchdevice-0.2.0/torchdevice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-29 13:28:58.000000 torchdevice-0.2.0/torchdevice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 13:28:58.000000 torchdevice-0.2.0/torchdevice.egg-info/top_level.txt
```

### Comparing `torchdevice-0.1.0/setup.py` & `torchdevice-0.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from setuptools import setup, find_packages
+from setuptools import find_packages, setup
 
 name = 'torchdevice'
 
 setup(
     name=name,
-    version='0.1.0',
+    version='0.2.0',
     packages=[package for package in find_packages() if package.startswith(name)],
     url=f'https://github.com/speedcell4/{name}',
     license='MIT',
     author='speedcell4',
     author_email='speedcell4@gmail.com',
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     description='',
     install_requires=[
         'torch',
         'filelock',
     ],
     extras_require={
         'dev': [
```


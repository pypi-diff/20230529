# Comparing `tmp/my_provider-0.1.5.tar.gz` & `tmp/my-provider-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_provider-0.1.5.tar", last modified: Mon May 29 08:56:27 2023, max compression
+gzip compressed data, was "dist/my-provider-0.1.6.tar", last modified: Mon May 29 09:09:22 2023, max compression
```

## Comparing `my_provider-0.1.5.tar` & `my-provider-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 08:56:27.484363 my_provider-0.1.5/
--rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-29 08:56:27.483996 my_provider-0.1.5/PKG-INFO
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 08:56:27.479606 my_provider-0.1.5/my_provider/
--rw-r--r--   0 huangzheng   (501) staff       (20)      430 2023-05-29 08:56:25.000000 my_provider-0.1.5/my_provider/__init__.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 08:56:27.482088 my_provider-0.1.5/my_provider/hooks/
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my_provider-0.1.5/my_provider/hooks/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     7738 2023-05-26 07:27:32.000000 my_provider-0.1.5/my_provider/hooks/dlc_hook.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 08:56:27.483040 my_provider-0.1.5/my_provider/operators/
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my_provider-0.1.5/my_provider/operators/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     2665 2023-05-26 08:13:15.000000 my_provider-0.1.5/my_provider/operators/dlc_operator.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 08:56:27.481518 my_provider-0.1.5/my_provider.egg-info/
--rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-29 08:56:27.000000 my_provider-0.1.5/my_provider.egg-info/PKG-INFO
--rw-r--r--   0 huangzheng   (501) staff       (20)      376 2023-05-29 08:56:27.000000 my_provider-0.1.5/my_provider.egg-info/SOURCES.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-29 08:56:27.000000 my_provider-0.1.5/my_provider.egg-info/dependency_links.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       81 2023-05-29 08:56:27.000000 my_provider-0.1.5/my_provider.egg-info/entry_points.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-29 08:56:27.000000 my_provider-0.1.5/my_provider.egg-info/requires.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       12 2023-05-29 08:56:27.000000 my_provider-0.1.5/my_provider.egg-info/top_level.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-29 08:56:27.484483 my_provider-0.1.5/setup.cfg
--rw-r--r--   0 huangzheng   (501) staff       (20)      373 2023-05-29 08:56:25.000000 my_provider-0.1.5/setup.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:09:22.000000 my-provider-0.1.6/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-29 09:09:22.000000 my-provider-0.1.6/PKG-INFO
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:09:22.000000 my-provider-0.1.6/my_provider/
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:09:22.000000 my-provider-0.1.6/my_provider/operators/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my-provider-0.1.6/my_provider/operators/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     2665 2023-05-26 08:13:15.000000 my-provider-0.1.6/my_provider/operators/dlc_operator.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)      430 2023-05-29 09:08:13.000000 my-provider-0.1.6/my_provider/__init__.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:09:22.000000 my-provider-0.1.6/my_provider/hooks/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my-provider-0.1.6/my_provider/hooks/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     7738 2023-05-26 07:27:32.000000 my-provider-0.1.6/my_provider/hooks/dlc_hook.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)      373 2023-05-29 09:09:20.000000 my-provider-0.1.6/setup.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-29 09:09:22.000000 my-provider-0.1.6/my_provider.egg-info/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-29 09:09:22.000000 my-provider-0.1.6/my_provider.egg-info/PKG-INFO
+-rw-r--r--   0 huangzheng   (501) staff       (20)      376 2023-05-29 09:09:22.000000 my-provider-0.1.6/my_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       82 2023-05-29 09:09:22.000000 my-provider-0.1.6/my_provider.egg-info/entry_points.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-29 09:09:22.000000 my-provider-0.1.6/my_provider.egg-info/requires.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       12 2023-05-29 09:09:22.000000 my-provider-0.1.6/my_provider.egg-info/top_level.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-29 09:09:22.000000 my-provider-0.1.6/my_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-29 09:09:22.000000 my-provider-0.1.6/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `my_provider-0.1.5/my_provider/hooks/dlc_hook.py` & `my-provider-0.1.6/my_provider/hooks/dlc_hook.py`

 * *Files identical despite different names*

### Comparing `my_provider-0.1.5/my_provider/operators/dlc_operator.py` & `my-provider-0.1.6/my_provider/operators/dlc_operator.py`

 * *Files identical despite different names*


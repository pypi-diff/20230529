# Comparing `tmp/taskcli-0.0.3.tar.gz` & `tmp/taskcli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskcli-0.0.3.tar", last modified: Sun Dec  4 21:59:14 2022, max compression
+gzip compressed data, was "taskcli-0.0.5.tar", last modified: Mon May 29 15:01:35 2023, max compression
```

## Comparing `taskcli-0.0.3.tar` & `taskcli-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 p          (501) staff       (20)        0 2022-12-04 21:59:14.671577 taskcli-0.0.3/
--rw-r--r--   0 p          (501) staff       (20)     1062 2022-11-19 23:50:29.000000 taskcli-0.0.3/LICENSE
--rw-r--r--   0 p          (501) staff       (20)      219 2022-12-04 21:59:14.671644 taskcli-0.0.3/PKG-INFO
--rw-r--r--   0 p          (501) staff       (20)     3210 2022-12-04 21:55:22.000000 taskcli-0.0.3/README.md
--rw-r--r--   0 p          (501) staff       (20)       86 2022-11-19 23:50:29.000000 taskcli-0.0.3/pyproject.toml
--rw-r--r--   0 p          (501) staff       (20)      403 2022-12-04 21:59:14.671990 taskcli-0.0.3/setup.cfg
-drwxr-xr-x   0 p          (501) staff       (20)        0 2022-12-04 21:59:14.669737 taskcli-0.0.3/src/
-drwxr-xr-x   0 p          (501) staff       (20)        0 2022-12-04 21:59:14.670793 taskcli-0.0.3/src/taskcli/
--rw-r--r--   0 p          (501) staff       (20)      230 2022-12-04 21:56:41.000000 taskcli-0.0.3/src/taskcli/__init__.py
--rw-r--r--   0 p          (501) staff       (20)    13891 2022-12-04 20:09:02.000000 taskcli-0.0.3/src/taskcli/taskcli.py
-drwxr-xr-x   0 p          (501) staff       (20)        0 2022-12-04 21:59:14.671479 taskcli-0.0.3/src/taskcli.egg-info/
--rw-r--r--   0 p          (501) staff       (20)      219 2022-12-04 21:59:14.000000 taskcli-0.0.3/src/taskcli.egg-info/PKG-INFO
--rw-r--r--   0 p          (501) staff       (20)      229 2022-12-04 21:59:14.000000 taskcli-0.0.3/src/taskcli.egg-info/SOURCES.txt
--rw-r--r--   0 p          (501) staff       (20)        1 2022-12-04 21:59:14.000000 taskcli-0.0.3/src/taskcli.egg-info/dependency_links.txt
--rw-r--r--   0 p          (501) staff       (20)        8 2022-12-04 21:59:14.000000 taskcli-0.0.3/src/taskcli.egg-info/top_level.txt
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:01:35.857935 taskcli-0.0.5/
+-rw-r--r--   0 p          (501) staff       (20)     1062 2022-11-19 23:50:29.000000 taskcli-0.0.5/LICENSE
+-rw-r--r--   0 p          (501) staff       (20)      219 2023-05-29 15:01:35.858008 taskcli-0.0.5/PKG-INFO
+-rw-r--r--   0 p          (501) staff       (20)     1781 2023-05-29 14:52:00.000000 taskcli-0.0.5/README.md
+-rw-r--r--   0 p          (501) staff       (20)       86 2022-11-19 23:50:29.000000 taskcli-0.0.5/pyproject.toml
+-rw-r--r--   0 p          (501) staff       (20)      405 2023-05-29 15:01:35.858346 taskcli-0.0.5/setup.cfg
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:01:35.855103 taskcli-0.0.5/src/
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:01:35.856896 taskcli-0.0.5/src/taskcli/
+-rw-r--r--   0 p          (501) staff       (20)      144 2023-05-29 14:27:39.000000 taskcli-0.0.5/src/taskcli/__init__.py
+-rw-r--r--   0 p          (501) staff       (20)     8253 2023-05-29 14:25:30.000000 taskcli-0.0.5/src/taskcli/old.py
+-rw-r--r--   0 p          (501) staff       (20)    18599 2023-05-29 14:59:52.000000 taskcli-0.0.5/src/taskcli/taskcli.py
+drwxr-xr-x   0 p          (501) staff       (20)        0 2023-05-29 15:01:35.857828 taskcli-0.0.5/src/taskcli.egg-info/
+-rw-r--r--   0 p          (501) staff       (20)      219 2023-05-29 15:01:35.000000 taskcli-0.0.5/src/taskcli.egg-info/PKG-INFO
+-rw-r--r--   0 p          (501) staff       (20)      248 2023-05-29 15:01:35.000000 taskcli-0.0.5/src/taskcli.egg-info/SOURCES.txt
+-rw-r--r--   0 p          (501) staff       (20)        1 2023-05-29 15:01:35.000000 taskcli-0.0.5/src/taskcli.egg-info/dependency_links.txt
+-rw-r--r--   0 p          (501) staff       (20)        8 2023-05-29 15:01:35.000000 taskcli-0.0.5/src/taskcli.egg-info/top_level.txt
```

### Comparing `taskcli-0.0.3/LICENSE` & `taskcli-0.0.5/LICENSE`

 * *Files identical despite different names*


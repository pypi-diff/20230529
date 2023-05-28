# Comparing `tmp/asyncmake-0.1.0.tar.gz` & `tmp/asyncmake-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncmake-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "asyncmake-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `asyncmake-0.1.0.tar` & `asyncmake-0.1.1.tar`

### file list

```diff
@@ -1,12 +1,16 @@
--rw-r--r--   0        0        0      122 2023-05-28 20:56:08.814479 asyncmake-0.1.0/.gitignore
--rw-r--r--   0        0        0     1086 2023-05-28 20:56:08.814479 asyncmake-0.1.0/LICENSE
--rw-r--r--   0        0        0      162 2023-05-28 22:21:38.283168 asyncmake-0.1.0/Makefile
--rw-r--r--   0        0        0      463 2023-05-28 22:25:56.984971 asyncmake-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-28 20:56:08.814479 asyncmake-0.1.0/rplugin/python3/asyncmake.py
--rw-r--r--   0        0        0        0 2023-05-28 20:56:08.814479 asyncmake-0.1.0/src/asyncmake/__init__.py
--rw-r--r--   0        0        0        0 2023-05-28 22:21:38.283168 asyncmake-0.1.0/src/asyncmake/parse/__init__.py
--rw-r--r--   0        0        0      364 2023-05-28 22:21:38.283168 asyncmake-0.1.0/src/asyncmake/parse/base.py
--rw-r--r--   0        0        0      831 2023-05-28 22:21:38.286501 asyncmake-0.1.0/src/asyncmake/parse/parser.py
--rw-r--r--   0        0        0       61 2023-05-28 22:21:38.286501 asyncmake-0.1.0/test/data/Makefile1
--rw-r--r--   0        0        0      745 2023-05-28 22:21:38.286501 asyncmake-0.1.0/test/test_parser.py
--rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 asyncmake-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      122 2023-05-28 20:56:08.814479 asyncmake-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1086 2023-05-28 20:56:08.814479 asyncmake-0.1.1/LICENSE
+-rw-r--r--   0        0        0      162 2023-05-28 23:25:25.671837 asyncmake-0.1.1/Makefile
+-rw-r--r--   0        0        0      463 2023-05-28 23:27:41.372728 asyncmake-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 20:56:08.814479 asyncmake-0.1.1/rplugin/python3/asyncmake.py
+-rw-r--r--   0        0        0        0 2023-05-28 20:56:08.814479 asyncmake-0.1.1/src/asyncmake/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:27:41.376062 asyncmake-0.1.1/src/asyncmake/exec/__init__.py
+-rw-r--r--   0        0        0      380 2023-05-28 23:27:41.376062 asyncmake-0.1.1/src/asyncmake/exec/base.py
+-rw-r--r--   0        0        0      272 2023-05-28 23:27:41.376062 asyncmake-0.1.1/src/asyncmake/exec/make.py
+-rw-r--r--   0        0        0        0 2023-05-28 23:25:25.671837 asyncmake-0.1.1/src/asyncmake/parse/__init__.py
+-rw-r--r--   0        0        0      368 2023-05-28 23:27:41.376062 asyncmake-0.1.1/src/asyncmake/parse/base.py
+-rw-r--r--   0        0        0      831 2023-05-28 23:25:25.671837 asyncmake-0.1.1/src/asyncmake/parse/parser.py
+-rw-r--r--   0        0        0       61 2023-05-28 23:27:41.376062 asyncmake-0.1.1/test/data/Makefile
+-rw-r--r--   0        0        0      457 2023-05-28 23:27:41.376062 asyncmake-0.1.1/test/test_exec.py
+-rw-r--r--   0        0        0      698 2023-05-28 23:27:41.376062 asyncmake-0.1.1/test/test_parser.py
+-rw-r--r--   0        0        0      360 1970-01-01 00:00:00.000000 asyncmake-0.1.1/PKG-INFO
```

### Comparing `asyncmake-0.1.0/LICENSE` & `asyncmake-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `asyncmake-0.1.0/src/asyncmake/parse/parser.py` & `asyncmake-0.1.1/src/asyncmake/parse/parser.py`

 * *Files identical despite different names*


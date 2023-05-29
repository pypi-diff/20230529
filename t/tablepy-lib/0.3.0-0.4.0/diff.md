# Comparing `tmp/tablepy_lib-0.3.0.tar.gz` & `tmp/tablepy_lib-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tablepy_lib-0.3.0.tar", max compression
+gzip compressed data, was "tablepy_lib-0.4.0.tar", max compression
```

## Comparing `tablepy_lib-0.3.0.tar` & `tablepy_lib-0.4.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.3.0/LICENSE
--rw-r--r--   0        0        0      488 2023-05-24 21:38:17.333001 tablepy_lib-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 19:49:50.199768 tablepy_lib-0.3.0/README.md
--rw-r--r--   0        0        0       49 2023-05-24 21:31:44.458131 tablepy_lib-0.3.0/tablepy_lib/__init__.py
--rw-r--r--   0        0        0     2480 2023-05-24 21:38:03.255374 tablepy_lib-0.3.0/tablepy_lib/consoleFormatter.py
--rw-r--r--   0        0        0      554 1970-01-01 00:00:00.000000 tablepy_lib-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-05-24 20:04:11.338943 tablepy_lib-0.4.0/LICENSE
+-rw-r--r--   0        0        0      502 2023-05-29 14:01:31.354459 tablepy_lib-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1305 2023-05-29 14:01:08.849013 tablepy_lib-0.4.0/README.md
+-rw-r--r--   0        0        0       49 2023-05-24 21:31:44.458131 tablepy_lib-0.4.0/tablepy_lib/__init__.py
+-rw-r--r--   0        0        0     4471 2023-05-29 14:01:50.722503 tablepy_lib-0.4.0/tablepy_lib/consoleFormatter.py
+-rw-r--r--   0        0        0     1823 1970-01-01 00:00:00.000000 tablepy_lib-0.4.0/PKG-INFO
```

### Comparing `tablepy_lib-0.3.0/LICENSE` & `tablepy_lib-0.4.0/LICENSE`

 * *Files identical despite different names*


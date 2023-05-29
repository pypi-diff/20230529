# Comparing `tmp/optimuslib-0.0.8.tar.gz` & `tmp/optimuslib-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimuslib-0.0.8.tar", max compression
+gzip compressed data, was "optimuslib-0.0.9.tar", max compression
```

## Comparing `optimuslib-0.0.8.tar` & `optimuslib-0.0.9.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-05-29 13:32:12.741001 optimuslib-0.0.8/optimuslib/__init__.py
--rw-r--r--   0        0        0    31065 2023-05-29 17:23:26.114807 optimuslib-0.0.8/optimuslib/optimuslib.py
--rw-r--r--   0        0        0      372 2023-05-29 17:38:24.960062 optimuslib-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.8/README.md
--rw-r--r--   0        0        0      427 1970-01-01 00:00:00.000000 optimuslib-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-29 13:32:12.741001 optimuslib-0.0.9/optimuslib/__init__.py
+-rw-r--r--   0        0        0    31065 2023-05-29 17:23:26.114807 optimuslib-0.0.9/optimuslib/optimuslib.py
+-rw-r--r--   0        0        0      371 2023-05-29 17:50:36.290078 optimuslib-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.9/README.md
+-rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 optimuslib-0.0.9/PKG-INFO
```

### Comparing `optimuslib-0.0.8/optimuslib/optimuslib.py` & `optimuslib-0.0.9/optimuslib/optimuslib.py`

 * *Files identical despite different names*


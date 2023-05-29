# Comparing `tmp/sllim-0.1.1.tar.gz` & `tmp/sllim-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sllim-0.1.1.tar", max compression
+gzip compressed data, was "sllim-0.1.3.tar", max compression
```

## Comparing `sllim-0.1.1.tar` & `sllim-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1060 2023-05-15 16:22:10.877704 sllim-0.1.1/LICENSE
--rw-r--r--   0        0        0       16 2023-05-15 16:22:10.877792 sllim-0.1.1/README.md
--rw-r--r--   0        0        0      302 2023-05-16 13:15:21.609569 sllim-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2377 2023-05-16 13:14:46.317974 sllim-0.1.1/sllim/__init__.py
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 sllim-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1060 2023-05-15 16:22:10.877704 sllim-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1383 2023-05-29 12:04:13.123988 sllim-0.1.3/README.md
+-rw-r--r--   0        0        0      322 2023-05-29 12:04:35.638689 sllim-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9555 2023-05-29 12:04:13.125155 sllim-0.1.3/sllim/__init__.py
+-rw-r--r--   0        0        0     1869 1970-01-01 00:00:00.000000 sllim-0.1.3/PKG-INFO
```

### Comparing `sllim-0.1.1/LICENSE` & `sllim-0.1.3/LICENSE`

 * *Files identical despite different names*


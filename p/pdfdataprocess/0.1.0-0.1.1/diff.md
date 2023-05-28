# Comparing `tmp/pdfdataprocess-0.1.0.tar.gz` & `tmp/pdfdataprocess-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdfdataprocess-0.1.0.tar", max compression
+gzip compressed data, was "pdfdataprocess-0.1.1.tar", max compression
```

## Comparing `pdfdataprocess-0.1.0.tar` & `pdfdataprocess-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-05-28 20:36:12.887072 pdfdataprocess-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-28 20:36:12.887072 pdfdataprocess-0.1.0/pdfdataprocess/__init__.py
--rw-r--r--   0        0        0     1629 2023-05-28 21:20:53.332188 pdfdataprocess-0.1.0/pdfdataprocess/cli.py
--rw-r--r--   0        0        0     1911 2023-05-28 21:26:05.916932 pdfdataprocess-0.1.0/pdfdataprocess/process.py
--rw-r--r--   0        0        0      466 2023-05-28 21:13:42.517243 pdfdataprocess-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 pdfdataprocess-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1488 2023-05-28 22:19:47.614985 pdfdataprocess-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 20:36:12.887072 pdfdataprocess-0.1.1/pdfdataprocess/__init__.py
+-rw-r--r--   0        0        0     1629 2023-05-28 21:20:53.332188 pdfdataprocess-0.1.1/pdfdataprocess/cli.py
+-rw-r--r--   0        0        0     1911 2023-05-28 21:26:05.916932 pdfdataprocess-0.1.1/pdfdataprocess/process.py
+-rw-r--r--   0        0        0      531 2023-05-28 22:22:35.181111 pdfdataprocess-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2044 1970-01-01 00:00:00.000000 pdfdataprocess-0.1.1/PKG-INFO
```

### Comparing `pdfdataprocess-0.1.0/pdfdataprocess/cli.py` & `pdfdataprocess-0.1.1/pdfdataprocess/cli.py`

 * *Files identical despite different names*

### Comparing `pdfdataprocess-0.1.0/pdfdataprocess/process.py` & `pdfdataprocess-0.1.1/pdfdataprocess/process.py`

 * *Files identical despite different names*


# Comparing `tmp/triessentials-0.1.2.tar.gz` & `tmp/triessentials-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "triessentials-0.1.2.tar", max compression
+gzip compressed data, was "triessentials-0.1.3.tar", max compression
```

## Comparing `triessentials-0.1.2.tar` & `triessentials-0.1.3.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0      362 2023-05-29 18:22:52.229788 triessentials-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      272 2023-05-29 18:19:00.885919 triessentials-0.1.2/triessentials/__init__.py
--rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 triessentials-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      362 2023-05-29 18:36:48.173315 triessentials-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      281 2023-05-29 18:36:31.317325 triessentials-0.1.3/triessentials/__init__.py
+-rw-r--r--   0        0        0      345 1970-01-01 00:00:00.000000 triessentials-0.1.3/PKG-INFO
```


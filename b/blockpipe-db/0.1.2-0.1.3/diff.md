# Comparing `tmp/blockpipe_db-0.1.2.tar.gz` & `tmp/blockpipe_db-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blockpipe_db-0.1.2.tar", max compression
+gzip compressed data, was "blockpipe_db-0.1.3.tar", max compression
```

## Comparing `blockpipe_db-0.1.2.tar` & `blockpipe_db-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.2/README.md
--rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.2/blockpipe_db/__init__.py
--rw-r--r--   0        0        0     1236 2023-05-29 02:55:06.045479 blockpipe_db-0.1.2/blockpipe_db/client.py
--rw-r--r--   0        0        0      394 2023-05-29 02:55:16.506534 blockpipe_db-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 blockpipe_db-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       28 2023-05-28 13:20:46.955674 blockpipe_db-0.1.3/README.md
+-rw-r--r--   0        0        0       27 2023-05-28 13:31:46.448380 blockpipe_db-0.1.3/blockpipe_db/__init__.py
+-rw-r--r--   0        0        0     1236 2023-05-29 02:55:06.045479 blockpipe_db-0.1.3/blockpipe_db/client.py
+-rw-r--r--   0        0        0      393 2023-05-29 02:56:48.820379 blockpipe_db-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      734 1970-01-01 00:00:00.000000 blockpipe_db-0.1.3/PKG-INFO
```

### Comparing `blockpipe_db-0.1.2/blockpipe_db/client.py` & `blockpipe_db-0.1.3/blockpipe_db/client.py`

 * *Files identical despite different names*


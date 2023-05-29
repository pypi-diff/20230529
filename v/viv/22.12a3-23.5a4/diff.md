# Comparing `tmp/viv-22.12a3.tar.gz` & `tmp/viv-23.5a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viv-22.12a3.tar", last modified: Mon Dec 26 14:05:19 2022, max compression
+gzip compressed data, was "viv-23.5a4.tar", last modified: Mon May 29 17:52:49 2023, max compression
```

## Comparing `viv-22.12a3.tar` & `viv-23.5a4.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0 daylin    (1000) daylin    (1000)     1074 2022-12-26 14:03:58.055665 viv-22.12a3/LICENSE
--rw-r--r--   0 daylin    (1000) daylin    (1000)     1195 2022-12-21 21:10:42.734667 viv-22.12a3/README.md
--rw-r--r--   0 daylin    (1000) daylin    (1000)      627 2022-12-22 21:13:46.163552 viv-22.12a3/pyproject.toml
--rw-r--r--   0 daylin    (1000) daylin    (1000)       34 2022-12-20 18:40:31.561289 viv-22.12a3/src/viv/__init__.py
--rwxr-xr-x   0 daylin    (1000) daylin    (1000)    27380 2022-12-26 14:04:53.872985 viv-22.12a3/src/viv/viv.py
--rw-------   0 daylin    (1000) daylin    (1000)     1520 2022-12-26 14:05:19.639945 viv-22.12a3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2022-12-26 14:03:58.055665 viv-23.5a4/LICENSE
+-rw-r--r--   0        0        0     3928 2023-05-29 17:46:35.595217 viv-23.5a4/README.md
+-rw-r--r--   0        0        0      813 2023-05-29 17:43:32.762971 viv-23.5a4/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-05-28 22:22:55.204851 viv-23.5a4/src/viv/__init__.py
+-rw-r--r--   0        0        0       61 2023-02-03 19:40:10.351352 viv-23.5a4/src/viv/__main__.py
+-rwxr-xr-x   0        0        0    48457 2023-05-29 17:52:27.622335 viv-23.5a4/src/viv/viv.py
+-rw-r--r--   0        0        0     4252 1970-01-01 00:00:00.000000 viv-23.5a4/PKG-INFO
```

### Comparing `viv-22.12a3/LICENSE` & `viv-23.5a4/LICENSE`

 * *Files identical despite different names*


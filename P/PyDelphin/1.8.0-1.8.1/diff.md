# Comparing `tmp/PyDelphin-1.8.0.tar.gz` & `tmp/PyDelphin-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDelphin-1.8.0.tar", last modified: Sun Jan  8 20:22:45 2023, max compression
+gzip compressed data, was "PyDelphin-1.8.1.tar", last modified: Mon May 29 19:11:01 2023, max compression
```

## Comparing `PyDelphin-1.8.0.tar` & `PyDelphin-1.8.1.tar`

### file list

```diff
@@ -1,82 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 20:22:45.828364 PyDelphin-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-01-08 20:22:45.828364 PyDelphin-1.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 20:22:45.824364 PyDelphin-1.8.0/PyDelphin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-01-08 20:22:45.000000 PyDelphin-1.8.0/PyDelphin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-01-08 20:22:45.000000 PyDelphin-1.8.0/PyDelphin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 20:22:45.000000 PyDelphin-1.8.0/PyDelphin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-01-08 20:22:45.000000 PyDelphin-1.8.0/PyDelphin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-01-08 20:22:45.000000 PyDelphin-1.8.0/PyDelphin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-08 20:22:45.000000 PyDelphin-1.8.0/PyDelphin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 20:22:45.824364 PyDelphin-1.8.0/delphin/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25533 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/ace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 20:22:45.824364 PyDelphin-1.8.0/delphin/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/cli/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/cli/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/cli/edm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/cli/mkprof.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/cli/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/cli/repp.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/cli/select.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 20:22:45.828364 PyDelphin-1.8.0/delphin/codecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/ace.py
--rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/dmrsjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/dmrspenman.py
--rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/dmrstikz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/dmrx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/edsjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/edspenman.py
--rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/indexedmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/mrsjson.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/mrsprolog.py
--rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/mrx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/simpledmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/codecs/simplemrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    21375 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/derivation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 20:22:45.828364 PyDelphin-1.8.0/delphin/dmrs/
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/dmrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/dmrs/_dmrs.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/dmrs/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/dmrs/_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/edm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 20:22:45.828364 PyDelphin-1.8.0/delphin/eds/
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/eds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/eds/_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/eds/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/eds/_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/highlight.py
--rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/itsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/lnk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 20:22:45.828364 PyDelphin-1.8.0/delphin/mrs/
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/mrs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/mrs/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/mrs/_mrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/mrs/_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/predicate.py
--rw-r--r--   0 runner    (1001) docker     (123)    32288 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/repp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/sembase.py
--rw-r--r--   0 runner    (1001) docker     (123)    21087 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/semi.py
--rw-r--r--   0 runner    (1001) docker     (123)    52238 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/tdl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/tfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)    32485 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/tsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/tsql.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/vpm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 20:22:45.828364 PyDelphin-1.8.0/delphin/web/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/web/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/delphin/web/server.py
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 20:22:45.828364 PyDelphin-1.8.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-01-08 20:22:37.000000 PyDelphin-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:11:01.438953 PyDelphin-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-05-29 19:11:01.438953 PyDelphin-1.8.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:11:01.430953 PyDelphin-1.8.1/PyDelphin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10640 2023-05-29 19:11:01.000000 PyDelphin-1.8.1/PyDelphin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-29 19:11:01.000000 PyDelphin-1.8.1/PyDelphin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:11:01.000000 PyDelphin-1.8.1/PyDelphin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 19:11:01.000000 PyDelphin-1.8.1/PyDelphin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-29 19:11:01.000000 PyDelphin-1.8.1/PyDelphin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 19:11:01.000000 PyDelphin-1.8.1/PyDelphin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:11:01.434953 PyDelphin-1.8.1/delphin/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25533 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/ace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:11:01.434953 PyDelphin-1.8.1/delphin/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/cli/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/cli/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/cli/edm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/cli/mkprof.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/cli/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/cli/repp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/cli/select.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:11:01.438953 PyDelphin-1.8.1/delphin/codecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/ace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5982 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/dmrsjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8253 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/dmrspenman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5167 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/dmrstikz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11222 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/dmrx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10035 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/edsjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/edspenman.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11485 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/indexedmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6089 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/mrsjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/mrsprolog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13167 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/mrx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9544 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/simpledmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/codecs/simplemrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31081 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21375 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/derivation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:11:01.438953 PyDelphin-1.8.1/delphin/dmrs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/dmrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12504 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/dmrs/_dmrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/dmrs/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/dmrs/_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/edm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:11:01.438953 PyDelphin-1.8.1/delphin/eds/
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/eds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/eds/_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/eds/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9714 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/eds/_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11998 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7700 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/highlight.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8903 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34953 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/itsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6734 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/lnk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:11:01.438953 PyDelphin-1.8.1/delphin/mrs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/mrs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/mrs/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12696 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/mrs/_mrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11180 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/mrs/_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5304 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/predicate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32288 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/repp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10024 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6855 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/sembase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21087 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/semi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52238 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/tdl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/tfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6248 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32485 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/tsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/tsql.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3443 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/vpm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:11:01.438953 PyDelphin-1.8.1/delphin/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/web/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8905 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/delphin/web/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:11:01.438953 PyDelphin-1.8.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2765 2023-05-29 19:10:51.000000 PyDelphin-1.8.1/setup.py
```

### Comparing `PyDelphin-1.8.0/LICENSE` & `PyDelphin-1.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/PKG-INFO` & `PyDelphin-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDelphin
-Version: 1.8.0
+Version: 1.8.1
 Summary: Libraries and scripts for DELPH-IN data
 Home-page: https://github.com/delph-in/pydelphin
 Author: Michael Wayne Goodman
 Author-email: goodman.m.w@gmail.com
 License: MIT
 Keywords: nlp semantics hpsg delph-in linguistics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PyDelphin-1.8.0/PyDelphin.egg-info/PKG-INFO` & `PyDelphin-1.8.1/PyDelphin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDelphin
-Version: 1.8.0
+Version: 1.8.1
 Summary: Libraries and scripts for DELPH-IN data
 Home-page: https://github.com/delph-in/pydelphin
 Author: Michael Wayne Goodman
 Author-email: goodman.m.w@gmail.com
 License: MIT
 Keywords: nlp semantics hpsg delph-in linguistics
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `PyDelphin-1.8.0/PyDelphin.egg-info/SOURCES.txt` & `PyDelphin-1.8.1/PyDelphin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/README.md` & `PyDelphin-1.8.1/README.md`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/__about__.py` & `PyDelphin-1.8.1/delphin/__about__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 
 # This __about__.py file for storing project metadata is inspired by
 # the warehouse project:
 #   https://github.com/pypa/warehouse/blob/master/warehouse/__about__.py
 
-__version__ = '1.8.0'
+__version__ = '1.8.1'
 __version_info__ = __version__.replace('.', ' ').replace('-', ' ').split()
 
 __title__ = 'PyDelphin'
 __summary__ = 'Libraries and scripts for DELPH-IN data'
 __uri__ = 'https://github.com/delph-in/pydelphin'
 
 __author__ = 'Michael Wayne Goodman'
 __email__ = 'goodman.m.w@gmail.com'
 
-__maintainer__ = 'Michael Wayne Goodman and Angie McMillan-Major'
+__maintainer__ = 'Michael Wayne Goodman'
 
 __license__ = 'MIT'
 __copyright__ = '2013--2020 %s <%s> and contributors' % (__author__, __email__)
```

### Comparing `PyDelphin-1.8.0/delphin/ace.py` & `PyDelphin-1.8.1/delphin/ace.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/cli/compare.py` & `PyDelphin-1.8.1/delphin/cli/compare.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/cli/convert.py` & `PyDelphin-1.8.1/delphin/cli/convert.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/cli/edm.py` & `PyDelphin-1.8.1/delphin/cli/edm.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/cli/mkprof.py` & `PyDelphin-1.8.1/delphin/cli/mkprof.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/cli/process.py` & `PyDelphin-1.8.1/delphin/cli/process.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/cli/repp.py` & `PyDelphin-1.8.1/delphin/cli/repp.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/cli/select.py` & `PyDelphin-1.8.1/delphin/cli/select.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/ace.py` & `PyDelphin-1.8.1/delphin/codecs/ace.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/dmrsjson.py` & `PyDelphin-1.8.1/delphin/codecs/dmrsjson.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/dmrspenman.py` & `PyDelphin-1.8.1/delphin/codecs/dmrspenman.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/dmrstikz.py` & `PyDelphin-1.8.1/delphin/codecs/dmrstikz.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/dmrx.py` & `PyDelphin-1.8.1/delphin/codecs/dmrx.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/eds.py` & `PyDelphin-1.8.1/delphin/codecs/eds.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/edsjson.py` & `PyDelphin-1.8.1/delphin/codecs/edsjson.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/edspenman.py` & `PyDelphin-1.8.1/delphin/codecs/edspenman.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/indexedmrs.py` & `PyDelphin-1.8.1/delphin/codecs/indexedmrs.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/mrsjson.py` & `PyDelphin-1.8.1/delphin/codecs/mrsjson.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/mrsprolog.py` & `PyDelphin-1.8.1/delphin/codecs/mrsprolog.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/mrx.py` & `PyDelphin-1.8.1/delphin/codecs/mrx.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/simpledmrs.py` & `PyDelphin-1.8.1/delphin/codecs/simpledmrs.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/codecs/simplemrs.py` & `PyDelphin-1.8.1/delphin/codecs/simplemrs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Serialization functions for the SimpleMRS format.
 """
 
 from pathlib import Path
+from typing import Optional
 
 from delphin.util import Lexer
 from delphin import predicate
 from delphin.lnk import Lnk
 from delphin.sembase import (role_priority, property_priority)
 from delphin import variable
 from delphin.mrs import (
@@ -180,15 +181,15 @@
     top = index = lnk = surface = identifier = None
     rels = []
     hcons = []
     icons = []
     variables = {}
     lexer.expect_type(LBRACK)
     lnk = _decode_lnk(lexer)
-    surface = lexer.accept_type(DQSTRING)
+    surface = _decode_dqstring(lexer.accept_type(DQSTRING))
     feature = lexer.accept_type(FEATURE)
     while feature is not None:
         feature = feature.upper()
         if feature in ('LTOP', 'TOP'):
             top = lexer.expect_type(SYMBOL).lower()
         elif feature == 'INDEX':
             index = _decode_variable(lexer, variables)
@@ -219,14 +220,20 @@
 def _decode_lnk(lexer):
     lnk = lexer.accept_type(LNK)
     if lnk is not None:
         lnk = Lnk(lnk)
     return lnk
 
 
+def _decode_dqstring(dqstring: Optional[str]) -> Optional[str]:
+    if dqstring is not None:
+        dqstring = _unescape(dqstring)
+    return dqstring
+
+
 def _decode_variable(lexer, variables):
     var = lexer.expect_type(SYMBOL).lower()
     if var not in variables:
         variables[var] = {}
     props = variables[var]
     if lexer.accept_type(LBRACK):
         lexer.accept_type(SYMBOL)  # variable type
@@ -239,38 +246,46 @@
     return var
 
 
 def _decode_rel(lexer, variables):
     args = {}
     surface = None
     lexer.expect_type(LBRACK)
-    pred = predicate.normalize(
-        lexer.choice_type(DQSTRING, SQSYMBOL, PREDICATE, SYMBOL)[1])
+    pred = _decode_predicate(lexer)
     lnk = _decode_lnk(lexer)
-    surface = lexer.accept_type(DQSTRING)
+    surface = _decode_dqstring(lexer.accept_type(DQSTRING))
     _, label = lexer.expect((FEATURE, 'LBL'), (SYMBOL, None))
     # any remaining are arguments or a constant
     role = lexer.accept_type(FEATURE)
     while role is not None:
         role = role.upper()
         if role == 'CARG':
-            value = lexer.expect_type(DQSTRING)
+            value = _decode_dqstring(lexer.expect_type(DQSTRING))
         else:
             value = _decode_variable(lexer, variables)
         args[role] = value
         role = lexer.accept_type(FEATURE)
     lexer.expect_type(RBRACK)
     return EP(pred,
               label.lower(),
               args=args,
               lnk=lnk,
               surface=surface,
               base=None)
 
 
+def _decode_predicate(lexer) -> str:
+    predstring = lexer.accept_type(DQSTRING)
+    if predstring is not None:
+        predstring = _decode_dqstring(predstring)
+    else:
+        predstring = lexer.choice_type(SQSYMBOL, PREDICATE, SYMBOL)[1]
+    return predicate.normalize(predstring)
+
+
 def _decode_cons(lexer, cls, variables):
     lhs = _decode_variable(lexer, variables)
     relation = lexer.expect_type(SYMBOL).lower()
     rhs = _decode_variable(lexer, variables)
     return cls(lhs, relation, rhs)
 
 
@@ -308,15 +323,15 @@
 
 def _encode_surface_info(m, lnk):
     tokens = []
     if lnk:
         if m.lnk:
             tokens.append(str(m.lnk))
         if m.surface is not None:
-            tokens.append('"{}"'.format(m.surface))
+            tokens.append('"{}"'.format(_escape(m.surface)))
     return tokens
 
 
 def _encode_hook(m, varprops, indent):
     delim = '\n  ' if indent else ' '
     tokens = []
     if m.top is not None:
@@ -347,20 +362,20 @@
     tokens = []
     for rel in rels:
         pred = rel.predicate
         if lnk:
             pred += str(rel.lnk)
         reltoks = ['[', pred]
         if lnk and rel.surface is not None:
-            reltoks.append('"{}"'.format(rel.surface))
+            reltoks.append('"{}"'.format(_escape(rel.surface)))
         reltoks.extend(('LBL:', rel.label))
         for role in sorted(rel.args, key=role_priority):
             arg = rel.args[role]
             if role == CONSTANT_ROLE:
-                arg = '"{}"'.format(arg)
+                arg = '"{}"'.format(_escape(arg))
             else:
                 arg = _encode_variable(arg, varprops)
             reltoks.extend((role + ':', arg))
         reltoks.append(']')
         tokens.append(' '.join(reltoks))
     if tokens:
         tokens = ['RELS: <'] + [delim.join(tokens)] + ['>']
@@ -379,7 +394,41 @@
     tokens = ['{} {} {}'.format(_encode_variable(ic.left, varprops),
                                 ic.relation,
                                 _encode_variable(ic.right, varprops))
               for ic in icons]
     if tokens:
         tokens = ['ICONS: <'] + [' '.join(tokens)] + ['>']
     return tokens
+
+
+# Character Escaping
+
+
+_ESCAPES = {
+    '\\': '\\\\',
+    '"': '\\"',
+}
+
+
+_UNESCAPES = {
+    '\\\\': '\\',
+    '\\"': '"',
+}
+
+
+def _escape(s: str) -> str:
+    return "".join(_ESCAPES.get(c, c) for c in s)
+
+
+def _unescape(s: str) -> str:
+    if not s:
+        return s
+    cs = []
+    i = 0
+    while i < len(s):
+        if s[i] == '\\' and (i + 1) < len(s):
+            cs.append(s[i+1])
+            i += 2
+        else:
+            cs.append(s[i])
+            i += 1
+    return "".join(cs)
```

### Comparing `PyDelphin-1.8.0/delphin/commands.py` & `PyDelphin-1.8.1/delphin/commands.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/derivation.py` & `PyDelphin-1.8.1/delphin/derivation.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/dmrs/__init__.py` & `PyDelphin-1.8.1/delphin/dmrs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/dmrs/_dmrs.py` & `PyDelphin-1.8.1/delphin/dmrs/_dmrs.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/dmrs/_operations.py` & `PyDelphin-1.8.1/delphin/dmrs/_operations.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/edm.py` & `PyDelphin-1.8.1/delphin/edm.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/eds/__init__.py` & `PyDelphin-1.8.1/delphin/eds/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/eds/_eds.py` & `PyDelphin-1.8.1/delphin/eds/_eds.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/eds/_operations.py` & `PyDelphin-1.8.1/delphin/eds/_operations.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/exceptions.py` & `PyDelphin-1.8.1/delphin/exceptions.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/hierarchy.py` & `PyDelphin-1.8.1/delphin/hierarchy.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/highlight.py` & `PyDelphin-1.8.1/delphin/highlight.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/interface.py` & `PyDelphin-1.8.1/delphin/interface.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/itsdb.py` & `PyDelphin-1.8.1/delphin/itsdb.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/lnk.py` & `PyDelphin-1.8.1/delphin/lnk.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/main.py` & `PyDelphin-1.8.1/delphin/main.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/mrs/__init__.py` & `PyDelphin-1.8.1/delphin/mrs/__init__.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/mrs/_mrs.py` & `PyDelphin-1.8.1/delphin/mrs/_mrs.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/mrs/_operations.py` & `PyDelphin-1.8.1/delphin/mrs/_operations.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/predicate.py` & `PyDelphin-1.8.1/delphin/predicate.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/repp.py` & `PyDelphin-1.8.1/delphin/repp.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/scope.py` & `PyDelphin-1.8.1/delphin/scope.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/sembase.py` & `PyDelphin-1.8.1/delphin/sembase.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/semi.py` & `PyDelphin-1.8.1/delphin/semi.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/tdl.py` & `PyDelphin-1.8.1/delphin/tdl.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/tfs.py` & `PyDelphin-1.8.1/delphin/tfs.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/tokens.py` & `PyDelphin-1.8.1/delphin/tokens.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/tsdb.py` & `PyDelphin-1.8.1/delphin/tsdb.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/tsql.py` & `PyDelphin-1.8.1/delphin/tsql.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/util.py` & `PyDelphin-1.8.1/delphin/util.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/variable.py` & `PyDelphin-1.8.1/delphin/variable.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/vpm.py` & `PyDelphin-1.8.1/delphin/vpm.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/web/client.py` & `PyDelphin-1.8.1/delphin/web/client.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/delphin/web/server.py` & `PyDelphin-1.8.1/delphin/web/server.py`

 * *Files identical despite different names*

### Comparing `PyDelphin-1.8.0/setup.py` & `PyDelphin-1.8.1/setup.py`

 * *Files identical despite different names*


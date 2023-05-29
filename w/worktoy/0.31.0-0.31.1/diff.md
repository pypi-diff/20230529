# Comparing `tmp/worktoy-0.31.0.tar.gz` & `tmp/worktoy-0.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worktoy-0.31.0.tar", last modified: Sun May 28 09:10:02 2023, max compression
+gzip compressed data, was "worktoy-0.31.1.tar", last modified: Mon May 29 01:25:35 2023, max compression
```

## Comparing `worktoy-0.31.0.tar` & `worktoy-0.31.1.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.572964 worktoy-0.31.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-28 09:09:53.000000 worktoy-0.31.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-28 09:10:02.572964 worktoy-0.31.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-28 09:09:53.000000 worktoy-0.31.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-28 09:09:53.000000 worktoy-0.31.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-28 09:10:02.572964 worktoy-0.31.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.564964 worktoy-0.31.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.564964 worktoy-0.31.0/src/worktoy/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.564964 worktoy-0.31.0/src/worktoy/core/
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/core/_empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/core/_maybe.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/core/_plenty.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/core/_some.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.564964 worktoy-0.31.0/src/worktoy/dio/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/dio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/dio/_fileaccess.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/dio/_filewalk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/dio/_loadfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.568964 worktoy-0.31.0/src/worktoy/field/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/field/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/field/_basefield.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.568964 worktoy-0.31.0/src/worktoy/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/parsing/_extractarg.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/parsing/_maybetype.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/parsing/_maybetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/parsing/_searchkeys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.568964 worktoy-0.31.0/src/worktoy/stringtools/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/stringtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/stringtools/_camelcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/stringtools/_justify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/stringtools/_monospace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/stringtools/_stringlist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.568964 worktoy-0.31.0/src/worktoy/typetools/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/typetools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/typetools/_any.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/typetools/_callmemaybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/typetools/_tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/typetools/_typebag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.568964 worktoy-0.31.0/src/worktoy/waitaminute/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_accesserror.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_dioerror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_exceptioncore.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_instantiationerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_manualinterrupt.py
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_n00berror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_proceduralerror.py
--rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_readonlyerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_typeguarderror.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_unexpectedstateerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_validationerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_valueguard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.564964 worktoy-0.31.0/src/worktoy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-28 09:10:02.000000 worktoy-0.31.0/src/worktoy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-28 09:10:02.000000 worktoy-0.31.0/src/worktoy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 09:10:02.000000 worktoy-0.31.0/src/worktoy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 09:10:02.000000 worktoy-0.31.0/src/worktoy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.572964 worktoy-0.31.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__any.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__basefield.py
--rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__callmemaybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__camelcase.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__extractarg.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__maybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__maybetype.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__maybetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__plenty.py
--rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__searchkeys.py
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__some.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__tuple.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__typebag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.803164 worktoy-0.31.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-29 01:25:27.000000 worktoy-0.31.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-29 01:25:35.803164 worktoy-0.31.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-29 01:25:27.000000 worktoy-0.31.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-29 01:25:27.000000 worktoy-0.31.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-29 01:25:35.803164 worktoy-0.31.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.795164 worktoy-0.31.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.799164 worktoy-0.31.1/src/worktoy/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.799164 worktoy-0.31.1/src/worktoy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/core/_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/core/_maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/core/_plenty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/core/_some.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.799164 worktoy-0.31.1/src/worktoy/dio/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/dio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/dio/_fileaccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/dio/_filewalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/dio/_loadfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.799164 worktoy-0.31.1/src/worktoy/field/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/field/_basefield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.799164 worktoy-0.31.1/src/worktoy/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/parsing/_extractarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/parsing/_maybetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/parsing/_maybetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/parsing/_searchkeys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.799164 worktoy-0.31.1/src/worktoy/stringtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/stringtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/stringtools/_camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/stringtools/_justify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/stringtools/_monospace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/stringtools/_stringlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.799164 worktoy-0.31.1/src/worktoy/typetools/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/typetools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/typetools/_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/typetools/_callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/typetools/_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/typetools/_typebag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.803164 worktoy-0.31.1/src/worktoy/waitaminute/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_accesserror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_dioerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_exceptioncore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_instantiationerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_manualinterrupt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_n00berror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_proceduralerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_readonlyerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_typeguarderror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_unexpectedstateerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_validationerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-29 01:25:27.000000 worktoy-0.31.1/src/worktoy/waitaminute/_valueguard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.799164 worktoy-0.31.1/src/worktoy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-29 01:25:35.000000 worktoy-0.31.1/src/worktoy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-29 01:25:35.000000 worktoy-0.31.1/src/worktoy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 01:25:35.000000 worktoy-0.31.1/src/worktoy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 01:25:35.000000 worktoy-0.31.1/src/worktoy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:25:35.803164 worktoy-0.31.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__basefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__extractarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__maybetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__maybetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__plenty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__searchkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__some.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-29 01:25:27.000000 worktoy-0.31.1/tests/test__typebag.py
```

### Comparing `worktoy-0.31.0/LICENSE` & `worktoy-0.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/PKG-INFO` & `worktoy-0.31.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: worktoy
-Version: 0.31.0
+Version: 0.31.1
 Summary: Collection of Utilities
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
 Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# WorkToy v0.31.0
+# WorkToy v0.31.1
 
 Collection of General Utilities
 
 ```
 pip install worktoy
 ```
```

### Comparing `worktoy-0.31.0/README.md` & `worktoy-0.31.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# WorkToy v0.31.0
+# WorkToy v0.31.1
 
 Collection of General Utilities
 
 ```
 pip install worktoy
 ```
```

### Comparing `worktoy-0.31.0/pyproject.toml` & `worktoy-0.31.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools>=63.2']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "worktoy"
-version = "0.31.0"
+version = "0.31.1"
 authors = [
     { name = "Asger Jon Vistisen", email = "asgerjon2@gmail.com" },
 ]
 description = "Collection of Utilities"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `worktoy-0.31.0/setup.cfg` & `worktoy-0.31.1/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [METADATA]
 name = WorkToy
-version = 0.31.0
+version = 0.31.1
 author = Asger Jon Vistisen
 author_email = asgerjon2@gmail.com
 description = A Collection of Utilities
 long_description = file:README.md,LICENSE
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `worktoy-0.31.0/src/worktoy/core/_empty.py` & `worktoy-0.31.1/src/worktoy/core/_empty.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/core/_maybe.py` & `worktoy-0.31.1/src/worktoy/core/_maybe.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 arguments. The function is also licensed under the MIT License and was
 created by Asger Jon Vistisen in 2023.
 """
 #  Copyright (c) 2023 Asger Jon Vistisen
 #  MIT Licence
 from __future__ import annotations
 
-from typing import Any
+from worktoy.typetools import Any
 
 
 def maybe(*args) -> Any:
   """The None-aware 'maybe' implements the null-coalescence behaviour.
   #  MIT License
   #  Copyright (c) 2023 Asger Jon Vistisen"""
   for arg in args:
```

### Comparing `worktoy-0.31.0/src/worktoy/core/_plenty.py` & `worktoy-0.31.1/src/worktoy/core/_plenty.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/core/_some.py` & `worktoy-0.31.1/src/worktoy/core/_some.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/dio/_loadfile.py` & `worktoy-0.31.1/src/worktoy/dio/_loadfile.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/field/_basefield.py` & `worktoy-0.31.1/src/worktoy/field/_basefield.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """BaseField decorates classes with fields"""
 #  Copyright (c) 2023 Asger Jon Vistisen
 #  MIT Licence
 from __future__ import annotations
-from typing import Any, NoReturn
+from typing import NoReturn
 
 from icecream import ic
-
+from worktoy.typetools import Any
 from worktoy.core import maybe
 from worktoy.parsing import searchKeys
 from worktoy.stringtools import stringList
 from worktoy.waitaminute import ReadOnlyError, ProceduralError
 
 ic.configureOutput(includeContext=True)
```

### Comparing `worktoy-0.31.0/src/worktoy/parsing/_searchkeys.py` & `worktoy-0.31.1/src/worktoy/parsing/_searchkeys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """The searchKeys function provides a flexible way of extracting values
 from keyword arguments."""
 #  Copyright (c) 2023 Asger Jon Vistisen
 #  MIT Licence
 from __future__ import annotations
 
-from typing import Any, NoReturn
+from typing import NoReturn
 
-from worktoy.typetools import CallMeMaybe
+from worktoy.typetools import CallMeMaybe, Any
 
 
 class _SearchKeys:
   """The searchKeys function provides a flexible way of extracting values
   from keyword arguments.
   #  MIT License
   #  Copyright (c) 2023 Asger Jon Vistisen"""
```

### Comparing `worktoy-0.31.0/src/worktoy/stringtools/_camelcase.py` & `worktoy-0.31.1/src/worktoy/stringtools/_camelcase.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/stringtools/_justify.py` & `worktoy-0.31.1/src/worktoy/stringtools/_justify.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/stringtools/_monospace.py` & `worktoy-0.31.1/src/worktoy/stringtools/_monospace.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/stringtools/_stringlist.py` & `worktoy-0.31.1/src/worktoy/stringtools/_stringlist.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/typetools/_any.py` & `worktoy-0.31.1/src/worktoy/typetools/_any.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/typetools/_callmemaybe.py` & `worktoy-0.31.1/src/worktoy/typetools/_callmemaybe.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/typetools/_tuple.py` & `worktoy-0.31.1/src/worktoy/typetools/_tuple.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Tuple represents a tuple of types"""
 #  Copyright (c) 2023 Asger Jon Vistisen
 #  MIT Licence
 from __future__ import annotations
 
-from typing import Any
+from worktoy.typetools import Any
 import typing
 
 import _collections_abc
 
 from icecream import ic
 
 FakeTuple = getattr(typing, '_BaseGenericAlias')
```

### Comparing `worktoy-0.31.0/src/worktoy/typetools/_typebag.py` & `worktoy-0.31.1/src/worktoy/typetools/_typebag.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """TypeBag is a subclass of the typing union classes that support
 isinstance."""
 #  Copyright (c) 2023 Asger Jon Vistisen
 #  MIT Licence
 from __future__ import annotations
 
 import typing
-from typing import Any
+from worktoy.typetools import Any
 import collections.abc
 
 from icecream import ic
 
 from worktoy.core import maybe
 
 union = getattr(typing, '_UnionGenericAlias', None)
```

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/__init__.py` & `worktoy-0.31.1/src/worktoy/waitaminute/__init__.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_accesserror.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_accesserror.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """AccessError is similar to AttributeError. It should receive the object
 and name where name failed to correspond to an attribute on object."""
 #  Copyright (c) 2023 Asger Jon Vistisen
 #  MIT Licence
 from __future__ import annotations
 
-from typing import Any
+from worktoy.typetools import Any
 
 from worktoy.parsing import extractArg
 from worktoy.stringtools import stringList
 from worktoy.waitaminute import ExceptionCore
 
 
 class AccessError(ExceptionCore):
```

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_exceptioncore.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_exceptioncore.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_instantiationerror.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_instantiationerror.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_manualinterrupt.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_manualinterrupt.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_n00berror.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_n00berror.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_proceduralerror.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_proceduralerror.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 would be when a variable is added to the name space with a value of None
 awaiting initialisation, but where another process requests it, whilst it
 is still waiting."""
 #  Copyright (c) 2023 Asger Jon Vistisen
 #  MIT Licence
 from __future__ import annotations
 
-from typing import Any
+from worktoy.typetools import Any
 
 from worktoy.parsing import extractArg
 from worktoy.stringtools import stringList
 from worktoy.waitaminute import ExceptionCore
 
 
 class ProceduralError(ExceptionCore):
```

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_readonlyerror.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_readonlyerror.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_typeguarderror.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_typeguarderror.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_unexpectedstateerror.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_unexpectedstateerror.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_validationerror.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_validationerror.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/src/worktoy/waitaminute/_valueguard.py` & `worktoy-0.31.1/src/worktoy/waitaminute/_valueguard.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """The valueGuard function raises an error if a given argument is of the
 correct type, but of improper value."""
 #  Copyright (c) 2023 Asger Jon Vistisen
 #  MIT Licence
 from __future__ import annotations
 
-from typing import Any
+from worktoy.typetools import Any
 
 from worktoy.parsing import extractArg
 from worktoy.stringtools import stringList
 from worktoy.typetools import CallMeMaybe
 
 
 def valueGuard(test: Any, *args, **kwargs) -> Any:
```

### Comparing `worktoy-0.31.0/src/worktoy.egg-info/PKG-INFO` & `worktoy-0.31.1/src/worktoy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: worktoy
-Version: 0.31.0
+Version: 0.31.1
 Summary: Collection of Utilities
 Author-email: Asger Jon Vistisen <asgerjon2@gmail.com>
 Project-URL: Homepage, https://github.com/AsgerJon/WorkToy
 Project-URL: Bug Tracker, https://github.com/AsgerJon/WorkToy
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# WorkToy v0.31.0
+# WorkToy v0.31.1
 
 Collection of General Utilities
 
 ```
 pip install worktoy
 ```
```

### Comparing `worktoy-0.31.0/src/worktoy.egg-info/SOURCES.txt` & `worktoy-0.31.1/src/worktoy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__any.py` & `worktoy-0.31.1/tests/test__any.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__basefield.py` & `worktoy-0.31.1/tests/test__basefield.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__callmemaybe.py` & `worktoy-0.31.1/tests/test__callmemaybe.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__camelcase.py` & `worktoy-0.31.1/tests/test__camelcase.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__empty.py` & `worktoy-0.31.1/tests/test__empty.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__extractarg.py` & `worktoy-0.31.1/tests/test__extractarg.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__maybe.py` & `worktoy-0.31.1/tests/test__maybe.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__maybetype.py` & `worktoy-0.31.1/tests/test__maybetype.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__maybetypes.py` & `worktoy-0.31.1/tests/test__maybetypes.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__plenty.py` & `worktoy-0.31.1/tests/test__plenty.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__searchkeys.py` & `worktoy-0.31.1/tests/test__searchkeys.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__some.py` & `worktoy-0.31.1/tests/test__some.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__tuple.py` & `worktoy-0.31.1/tests/test__tuple.py`

 * *Files identical despite different names*

### Comparing `worktoy-0.31.0/tests/test__typebag.py` & `worktoy-0.31.1/tests/test__typebag.py`

 * *Files identical despite different names*


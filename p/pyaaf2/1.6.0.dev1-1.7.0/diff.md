# Comparing `tmp/pyaaf2-1.6.0.dev1.tar.gz` & `tmp/pyaaf2-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaaf2-1.6.0.dev1.tar", last modified: Sun Jul  3 05:49:15 2022, max compression
+gzip compressed data, was "pyaaf2-1.7.0.tar", last modified: Mon May 29 20:52:06 2023, max compression
```

## Comparing `pyaaf2-1.6.0.dev1.tar` & `pyaaf2-1.7.0.tar`

### file list

```diff
@@ -1,48 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 05:49:15.424656 pyaaf2-1.6.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2901 2022-07-03 05:49:15.424656 pyaaf2-1.6.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1449 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-07-03 05:49:15.424656 pyaaf2-1.6.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2639 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 05:49:15.420656 pyaaf2-1.6.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 05:49:15.420656 pyaaf2-1.6.0.dev1/src/aaf2/
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    17268 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/ama.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/audio.py
--rw-r--r--   0 runner    (1001) docker     (121)     3637 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/auid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)    67114 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/cfb.py
--rw-r--r--   0 runner    (1001) docker     (121)     8720 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/components.py
--rw-r--r--   0 runner    (1001) docker     (121)     2706 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/content.py
--rw-r--r--   0 runner    (1001) docker     (121)    11714 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     7509 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (121)     3240 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/essence.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    10739 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/file.py
--rw-r--r--   0 runner    (1001) docker     (121)     7164 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)    18388 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/metadict.py
--rw-r--r--   0 runner    (1001) docker     (121)    11944 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    19780 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/mobid.py
--rw-r--r--   0 runner    (1001) docker     (121)    14919 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/mobs.py
--rw-r--r--   0 runner    (1001) docker     (121)     3621 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/mobslots.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 05:49:15.424656 pyaaf2-1.6.0.dev1/src/aaf2/model/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    66538 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/model/classdefs.py
--rw-r--r--   0 runner    (1001) docker     (121)    24029 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/model/datadefs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 05:49:15.424656 pyaaf2-1.6.0.dev1/src/aaf2/model/ext/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/model/ext/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18448 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/model/ext/classdefs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6593 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/model/ext/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (121)    30863 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/model/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (121)    32870 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/mxf.py
--rw-r--r--   0 runner    (1001) docker     (121)    39581 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/properties.py
--rw-r--r--   0 runner    (1001) docker     (121)     3657 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/rational.py
--rw-r--r--   0 runner    (1001) docker     (121)    28617 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/types.py
--rw-r--r--   0 runner    (1001) docker     (121)     5089 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11838 2022-07-03 05:49:04.000000 pyaaf2-1.6.0.dev1/src/aaf2/video.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-03 05:49:15.424656 pyaaf2-1.6.0.dev1/src/pyaaf2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2901 2022-07-03 05:49:14.000000 pyaaf2-1.6.0.dev1/src/pyaaf2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      871 2022-07-03 05:49:15.000000 pyaaf2-1.6.0.dev1/src/pyaaf2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-03 05:49:14.000000 pyaaf2-1.6.0.dev1/src/pyaaf2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-07-03 05:49:15.000000 pyaaf2-1.6.0.dev1/src/pyaaf2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:52:06.954783 pyaaf2-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-29 20:52:06.954783 pyaaf2-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-29 20:52:06.958783 pyaaf2-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:52:06.942783 pyaaf2-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:52:06.950783 pyaaf2-1.7.0/src/aaf2/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17268 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/ama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3637 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/auid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66736 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/cfb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8915 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8606 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/essence.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11439 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7218 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21252 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/metadict.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11944 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19781 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/mobid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15828 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/mobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3621 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/mobslots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:52:06.950783 pyaaf2-1.7.0/src/aaf2/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66538 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/model/classdefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24029 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/model/datadefs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:52:06.950783 pyaaf2-1.7.0/src/aaf2/model/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/model/ext/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18448 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/model/ext/classdefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/model/ext/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30863 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/model/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33531 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/mxf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42711 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3657 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/rational.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30406 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15449 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/src/aaf2/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:52:06.950783 pyaaf2-1.7.0/src/pyaaf2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-05-29 20:52:06.000000 pyaaf2-1.7.0/src/pyaaf2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-29 20:52:06.000000 pyaaf2-1.7.0/src/pyaaf2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 20:52:06.000000 pyaaf2-1.7.0/src/pyaaf2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 20:52:06.000000 pyaaf2-1.7.0/src/pyaaf2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 20:52:06.954783 pyaaf2-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_aaf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11936 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_ama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8260 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_attach.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_auid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_cfb_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13050 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_cfb_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6409 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_create_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_editing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_essence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_mangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_mobid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7638 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2683 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_mxf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_rangelock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_retime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_tagged_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12822 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_wave.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-29 20:51:56.000000 pyaaf2-1.7.0/tests/test_write_structured_storage.py
```

### Comparing `pyaaf2-1.6.0.dev1/LICENSE` & `pyaaf2-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/PKG-INFO` & `pyaaf2-1.7.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaaf2
-Version: 1.6.0.dev1
+Version: 1.7.0
 Summary: A python module for reading and writing advanced authoring format files
 Home-page: https://github.com/markreidvfx/pyaaf2
 Author: Mark Reid
 Author-email: mindmark@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/markreidvfx/pyaaf2
 Project-URL: Documentation, http://pyaaf.readthedocs.io
@@ -41,14 +41,15 @@
 
 Features
 --------
 
 - Read/Write AAF files
 - Modifying existing AAF files inplace
 - Embedding DNxHD/DNxHR/WAV media
+- Copying objects between files
 - Low level read/write Compound File Binary access
 - Lazy file reading
 - Zero dependencies, does not use AAF SDK
 
 Requirements
 ------------
```

### Comparing `pyaaf2-1.6.0.dev1/README.rst` & `pyaaf2-1.7.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Features
 --------
 
 - Read/Write AAF files
 - Modifying existing AAF files inplace
 - Embedding DNxHD/DNxHR/WAV media
+- Copying objects between files
 - Low level read/write Compound File Binary access
 - Lazy file reading
 - Zero dependencies, does not use AAF SDK
 
 Requirements
 ------------
```

### Comparing `pyaaf2-1.6.0.dev1/setup.py` & `pyaaf2-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup, find_packages
 import setuptools.command.build_py
 
 PROJECT_METADATA = {
-    "version": "1.6.0.dev1",
+    "version": "1.7.0",
     "author": 'Mark Reid',
     "author_email": 'mindmark@gmail.com',
     "license": 'MIT',
 }
 
 METADATA_TEMPLATE = """
 __version__ = "{version}"
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/ama.py` & `pyaaf2-1.7.0/src/aaf2/ama.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/audio.py` & `pyaaf2-1.7.0/src/aaf2/audio.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/auid.py` & `pyaaf2-1.7.0/src/aaf2/auid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 import struct
 import traceback
 
 class AUID(object):
     """
-    A higher performance UUID class that is more specialised for AAF.
+    A higher performance UUID class that is more specialized for AAF.
     """
     __slots__ = ('bytes_le')
     def __init__(self, hex=None, bytes_le=None, bytes_be=None, int=None):
         if bytes_le:
             self.bytes_le = bytearray(bytes_le)
         elif isinstance(hex, (uuid.UUID, AUID)):
             self.bytes_le = bytearray(hex.bytes_le)
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/cache.py` & `pyaaf2-1.7.0/src/aaf2/cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         node.prev.next = node.next
         node.next.prev = node.prev
 
         # hook up new prev and next
         node.prev = self.head.prev
         node.next = self.head.prev.next
 
-        # update neighbours to point to new node
+        # update neighbors to point to new node
         node.next.prev = node
         node.prev.next = node
 
     def __contains__(self, key):
         return key in self.data
 
     def __setitem__(self, key, value):
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/cfb.py` & `pyaaf2-1.7.0/src/aaf2/cfb.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,25 +150,25 @@
         mini_sector_size = self.storage.mini_stream_sector_size
         mini_stream_chain = self.storage.mini_stream_chain
         read_sector_data = self.storage.read_sector_data
         sector_data = None
         prev_sid = -1
 
         if is_mini_stream:
-             mini_fat_index     = self.pos // mini_sector_size
-             mini_sector_offset = self.pos  % mini_sector_size
-             sector_size = mini_sector_size
+            mini_fat_index     = self.pos // mini_sector_size
+            mini_sector_offset = self.pos  % mini_sector_size
+            sector_size = mini_sector_size
         else:
             index      = self.pos // full_sector_size
             start_offset = self.pos  % full_sector_size
             sector_size = full_sector_size
 
         while bytes_to_read > 0:
 
-            # inlined on purpose this loop runs alot
+            # inlined on purpose this loop runs a lot
             if is_mini_stream:
                 mini_stream_sid = self.fat_chain[mini_fat_index]
                 mini_stream_pos = (mini_stream_sid * mini_sector_size) + mini_sector_offset
 
                 index      = mini_stream_pos // full_sector_size
                 sid_offset = mini_stream_pos  % full_sector_size
 
@@ -263,15 +263,15 @@
         else:
             index      = self.pos // full_sector_size
             sid_offset = self.pos  % full_sector_size
             sector_size = full_sector_size
 
         while data_size > 0:
 
-            # inlined on purpose this method can get called alot
+            # inlined on purpose this method can get called a lot
             if is_mini_stream:
                 mini_stream_sid = self.fat_chain[mini_fat_index]
                 mini_stream_pos  = (mini_stream_sid * mini_sector_size) + mini_sector_offset
 
                 index      = mini_stream_pos // full_sector_size
                 sid_offset = mini_stream_pos  % full_sector_size
 
@@ -401,15 +401,15 @@
     if left is not None and left >= root:
         raise CompoundFileBinaryError("Binary tree violation" )
 
     if right is not None and right <= root:
         raise CompoundFileBinaryError("Binary tree violation")
 
     # Black height mismatch
-    # cannot gerentee all aaf Implementions use rbtree
+    # cannot guarantee all aaf Implementations use rbtree
     # if lh != 0 and rh != 0 and lh != rh:
     #     print(lh, rh)
     #     raise CompoundFileBinaryError("Black violation {}".format(root.path()))
 
     if lh != 0 and rh != 0:
         return lh if is_red(root) else lh + 1
     else:
@@ -742,15 +742,15 @@
 
         if self.dir_id in self.storage.children_cache:
             self.storage.children_cache[self.dir_id][entry.name] = entry
 
     def insert(self, entry):
         """
         Inserts entry into child folder tree.
-        Trys to mantains a balanced red black tree.
+        Tries to maintain a balanced red black tree.
         Technique is base on topdown insert approach in described in
         https://eternallyconfuzzled.com/red-black-trees-c-the-most-common-balanced-binary-search-tree
         """
 
         dir_per_sector = self.storage.sector_size // 128
         max_dirs_entries = self.storage.dir_sector_count * dir_per_sector
 
@@ -1271,20 +1271,20 @@
 
 
     def read_header(self):
 
         f = self.f
         f.seek(0)
 
-        magic = f.read(8)
-        # logging.debug("magic: %s" % magic.encode("hex"))
-        logging.debug("magic: %s" % str([magic]))
+        self.magic = f.read(8)
+        logging.debug("magic: %s" % str([self.magic]))
+
+        if self.magic != b'\xd0\xcf\x11\xe0\xa1\xb1\x1a\xe1':
+            raise CompoundFileBinaryError("invalid file magic signature: {}".format([self.magic]))
 
-        # clsid = f.read(16)
-        # logging.debug("clsid: %s" % clsid.encode("hex"))
         self.class_id = auid.AUID(bytes_le=f.read(16))
         logging.debug("clsid: %s" % str(self.class_id))
 
         self.minor_version = read_u16le(f)
         logging.debug("minor_version: %d" % self.minor_version)
 
         self.major_version = read_u16le(f)
@@ -1341,15 +1341,14 @@
         logging.debug("difat_sector_count: %d" % self.difat_sector_count)
 
         self.difat = [[]]
 
         logging.debug("reading header difat at %d" % f.tell())
         for i in range(109):
             item = read_u32le(f)
-            # item = fat_sector_types.get(item, item)
             self.difat[0].append(item)
 
         sectors_left = self.difat_sector_count
 
         sid = self.difat_sector_start
 
         # reading difat sectors
@@ -1447,16 +1446,14 @@
 
         logging.debug("read %d fat sectors ", sector_count)
 
         if self.sector_size == 4096 and len(self.fat) > RANGELOCKSECT:
             if self.fat[RANGELOCKSECT] != ENDOFCHAIN:
                 logging.warning("range lock sector has data")
 
-        # logging.debug("fat: %s" % str(pretty_sectors(self.fat)))
-
     def write_fat(self):
         logging.debug("writing fat")
         f = self.f
         sector_count = 0
 
         assert len(self.fat)*4 % self.sector_size == 0
 
@@ -1491,28 +1488,23 @@
             f.seek((sid + 1) *  self.sector_size)
             extend_sid_table(f, self.minifat, self.sector_size)
             sector_count += 1
 
         if sys.byteorder == 'big':
              self.minifat.byteswap()
 
-        # mini_stream_byte_size = 0
         last_used_sector = 0
         for i,v in enumerate(self.minifat):
             if v == FREESECT:
                 self.minifat_freelist.append(i)
             else:
                 last_used_sector = i
-                # mini_stream_byte_size += self.mini_stream_sector_size
 
         mini_stream_byte_size = ((last_used_sector+1) * self.mini_stream_sector_size)
 
-        # for i, sect in enumerate(pretty_sectors(self.minifat)):
-        #     print(i, sect)
-
         logging.debug("read %d mini fat sectors", sector_count)
         return mini_stream_byte_size
 
     def write_minifat(self):
         f = self.f
         sector_count = 0
 
@@ -1692,16 +1684,16 @@
         sector_data = self.sector_cache.get(sid, None)
         if sector_data is not None:
             return sector_data
         else:
             pos = (sid + 1) *  self.sector_size
             self.f.seek(pos)
             sector_data = bytearray(self.sector_size)
-            #NOTE: if requested sector doesn't exist or
-            # is truncated will pad with zeros, expected behaviour
+            # NOTE: if requested sector doesn't exist or
+            # is truncated will pad with zeros, expected behavior
             bytes_read = self.f.readinto(sector_data)
             self.sector_cache[sid] = sector_data
             return sector_data
 
     def get_sid_offset(self, abs_pos):
         sid, sid_offset = divmod(abs_pos, self.sector_size)
         return sid-1, sid_offset
@@ -1721,16 +1713,14 @@
         if dir_id is None:
             return None
 
         entry = self.dir_cache.get(dir_id, None)
         if entry is not None:
             return entry
 
-        # print("reading", dir_id)
-
         # assert not dir_id in self.dir_freelist
 
         stream_pos = dir_id * 128
         chain_index = stream_pos // self.sector_size
         sid_offset  = stream_pos % self.sector_size
         sid = self.dir_fat_chain[chain_index]
 
@@ -1742,15 +1732,14 @@
         entry.parent = parent
         self.dir_cache[dir_id] = entry
         return entry
 
     def clear_sector(self, sid):
         sector_pos = (sid + 1) * self.sector_size
         self.f.seek(sector_pos)
-        # for i in range(self.sector_size):
         self.f.write(bytearray(self.sector_size))
 
     def next_free_dir_id(self):
 
         # use free list first
         if self.dir_freelist:
             return self.dir_freelist.pop(0)
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/components.py` & `pyaaf2-1.7.0/src/aaf2/components.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,14 +67,19 @@
 
 
 @register_class
 class Sequence(Segment):
     class_id = AUID("0d010101-0101-0f00-060e-2b3402060101")
     __slots__ = ()
 
+    def __init__(self, media_kind=None, length=None):
+        super(Sequence, self).__init__(media_kind, length)
+        # initialize components to empty list
+        self.components.value = []
+
     @property
     def components(self):
         return self['Components']
 
     def component_at_time(self, edit_unit):
         return self.components[self.index_at_time(edit_unit)]
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/content.py` & `pyaaf2-1.7.0/src/aaf2/content.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/core.py` & `pyaaf2-1.7.0/src/aaf2/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,35 @@
-
 from __future__ import (
     unicode_literals,
     absolute_import,
     print_function,
     division,
     )
 
 import sys
 from io import BytesIO
-import weakref
 import struct
 import array
 
 from .utils import (
-    read_u8,
-    read_u16le,
-    read_u32le,
     write_u8,
     write_u16le,
-    write_u32le,
     safe_print,
     )
 from .exceptions import AAFPropertyError, AAFAttachError
 from . import properties
 from .properties import property_formats
 from .auid import AUID
 
 P_HEADER_STRUCT = struct.Struct(str('<BBH'))
 
 OPERATIONGROUP_PARAMETERS_AUID = AUID("06010104-060a-0000-060e-2b3401010102")
 
+sentinel = object()
+
 
 class AAFObject(object):
     __slots__ = ('class_id', 'root', 'dir', 'property_entries', '__weakref__' )
 
     def __new__(cls, *args, **kwargs):
         self = super(AAFObject, cls).__new__(cls)
         self.root = None
@@ -104,16 +100,16 @@
                 p = property_formats[format](self, pid, format, version)
                 p.data = data
                 self.property_entries[pid] = p
 
             for p in self.property_entries.values():
                 p.decode()
                 if isinstance(p, (properties.StrongRefSetProperty,
-                                properties.StrongRefVectorProperty,
-                                properties.WeakRefArrayProperty)):
+                                  properties.StrongRefVectorProperty,
+                                  properties.WeakRefArrayProperty)):
                     p.read_index()
 
     def validate(self):
         missing = []
 
         for propertydef in self.classdef.all_propertydefs():
 
@@ -139,46 +135,39 @@
     def write_properties(self, validate=True):
         if validate:
             self.validate()
 
         s = self.dir.touch("properties").open(mode='rw')
 
         with BytesIO() as f:
-            # print("writing", f.dir.path())
             byte_order = 0x4c
             entry_count = len(self.property_entries)
             version = properties.PROPERTY_VERSION
 
             write_u8(f, byte_order)
             write_u8(f, version)
             write_u16le(f, entry_count)
 
             for p in self.property_entries.values():
+                assert p.data is not None
                 write_u16le(f, p.pid)
                 write_u16le(f, p.format)
-                if p.data is None:
-                    print("??", p)
-                    print("!!", p.data)
-                    print(p.value)
-                    raise Exception()
-
                 write_u16le(f, len(p.data))
 
             # write the data
             for p in self.property_entries.values():
                 f.write(p.data)
 
             s.write(f.getvalue())
             s.truncate()
             # write index's
             for p in self.property_entries.values():
                 if isinstance(p, (properties.StrongRefSetProperty,
-                                properties.StrongRefVectorProperty,
-                                properties.WeakRefArrayProperty)):
-                    # print('writing index', self, p)
+                                  properties.StrongRefVectorProperty,
+                                  properties.WeakRefArrayProperty)):
                     p.write_index()
 
     def detach(self, delete=False):
         items = []
         for item, streams in self.walk_references(topdown=True):
             # store reference not sure if necessary
             items.append(item)
@@ -253,26 +242,44 @@
         for obj in refs:
             for item, item_streams in obj.walk_references(topdown):
                 yield item, item_streams
 
         if topdown:
             yield self, streams
 
-    def copy(self, new_dir=None):
-        # new_obj = self.__class__(self.root)
+    def copy(self, new_dir=None, root=None, classdef_cache=None):
         new_obj = self.__class__.__new__(self.__class__)
-        new_obj.root = self.root
+        classdef_cache = classdef_cache or set()
+        root = root or self.root
+        new_obj.root = root
+
+        # if copying to new root make sure classdef is defined
+        # to prevent excessive calls a cache is used skip already
+        # processed classdefs
+        if root is not self.root:
+            classdef = self.classdef
+            if classdef.auid not in classdef_cache:
+                root.metadict.register_external_classdef(self.classdef)
+                classdef_cache.add(classdef.auid)
+
         if type(new_obj) is AAFObject:
             new_obj.class_id = self.class_id
         new_obj.dir = new_dir
         if new_dir:
+            assert new_dir.storage is root.cfb
             new_obj.dir.class_id = self.class_id
 
         for pid, p in self.property_entries.items():
-            new_obj.property_entries[pid] = p.copy(new_obj)
+            # the pid in the new root could be different
+            if pid >= 0x8000 and root is not self.root:
+                pdef = new_obj.classdef.lookup_propertydef(p.propertydef.auid)
+                assert pdef
+                pid = pdef.pid
+
+            new_obj.property_entries[pid] = p.copy(new_obj, pid, classdef_cache)
 
         return new_obj
 
     def properties(self):
 
         for pid, p in self.property_entries.items():
             yield p
@@ -315,37 +322,37 @@
 
         return default
 
     def getvalue(self, key, default=None):
         if key not in self.keys():
             return default
 
-        p = self.get(key, None)
-        if p is None:
+        p = self.get(key, sentinel)
+        if p is sentinel:
             return default
         return p.value
 
     def __getitem__(self, key):
-        result = self.get(key, default=None)
-        if result is None:
+        result = self.get(key, default=sentinel)
+        if result is sentinel:
             raise KeyError(key)
         return result
 
     def __delitem__(self, key):
-        result = self.get(key, default=None, allkeys=False)
-        if result is None:
+        result = self.get(key, default=sentinel, allkeys=False)
+        if result is sentinel:
             raise KeyError(key)
 
         del self.property_entries[result.pid]
         if self.dir:
             self.root.manager.add_modified(self)
 
-    def __contains__(self, key, all=False):
-        result = self.get(key, default=None, allkeys=False)
-        if result is None:
+    def __contains__(self, key):
+        result = self.get(key, default=sentinel, allkeys=False)
+        if result is sentinel:
             return False
         return True
 
     def __repr__(self):
         s = "%s.%s" % (self.__class__.__module__,
                        self.__class__.__name__)
         name = self.name
@@ -372,12 +379,10 @@
                 continue
 
             if isinstance(p, properties.StrongRefSetProperty):
                 safe_print(space, p.name, p.typedef)
                 for key, obj in p.items():
                     safe_print(space + indent, obj)
                     obj.dump(space + indent*2)
-
                 continue
-                # print(space, p.name,  p.typedef)
 
             safe_print(space, p.name, p.typedef, p.value)
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/dictionary.py` & `pyaaf2-1.7.0/src/aaf2/dictionary.py`

 * *Files 6% similar despite different names*

```diff
@@ -251,7 +251,31 @@
         return lookup_def(self, name, OperationDef, 'OperationDefinitions')
 
     def lookup_interperlationdef(self, name):
         return lookup_def(self, name, InterpolationDef, 'InterpolationDefinitions')
 
     def lookup_taggedvaluedef(self, name):
         return lookup_def(self, name, TaggedValueDef, 'TaggedValueDefinitions')
+
+    def update(self, other):
+        if not isinstance(other, Dictionary):
+            raise ValueError("other must be a Dictionary object")
+
+        for def_type in ('DataDefinitions',
+                         'ContainerDefinitions',
+                         'CodecDefinitions',
+                         'ParameterDefinitions',
+                         'OperationDefinitions',
+                         'InterpolationDefinitions',
+                         'TaggedValueDefinitions'):
+
+            for other_def in other[def_type].values():
+                if other_def.auid not in self[def_type]:
+                    self[def_type].append(other_def.copy(root=self.root))
+
+                elif def_type == 'OperationDefinitions':
+                    # make sure operation all the same parameters
+                    opdef = self.lookup_operationdef(other_def.auid)
+                    for p in other_def.parameters:
+                        param = self.lookup_parameterdef(p.auid)
+                        if param.unique_key not in opdef.parameters:
+                            opdef.append(param)
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/essence.py` & `pyaaf2-1.7.0/src/aaf2/essence.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/file.py` & `pyaaf2-1.7.0/src/aaf2/file.py`

 * *Files 6% similar despite different names*

```diff
@@ -146,14 +146,31 @@
 class AAFFile(object):
     """
     AAF File Object. This is the entry point object for most of the API.
     This object is designed to be like python's native open function.
     It is recommended to create this object with the `aaf.open` alias.
     It is also highly recommended to use the with statement.
 
+    .. warning::
+       If an exception is raised inside the with block and the file was opened
+       as writable, the final file should be considered bad or corrupted.
+
+       Take this snippet as an example:
+
+       .. code-block:: python
+
+           try:
+               with aaf.open('/path/to/aaf_file.aaf', 'r+') as f:
+                   raise ValueError('asd')
+           except:
+               pass
+
+       in this case, even if the exception is properly handled, the content
+       of ``/path/to/aaf_file.aaf`` shouldn't be trusted anymore.
+
     For example. Opening existing AAF file readonly::
 
         with aaf.open('/path/to/aaf_file.aaf', 'r') as f:
 
     Opening new AAF file overwriting existing one::
 
         with aaf.open('/path/to/aaf_file.aaf', 'w') as f:
@@ -324,14 +341,20 @@
             for pid in path:
                 write_u16le(f, pid)
             write_u16le(f, 0) # null terminated
 
     def __exit__(self, exc_type, exc_value, traceback):
         if (exc_type is None and exc_value is None and traceback is None):
             self.close()
+        else:
+            self.is_open = False
+            try:
+                self.cfb.close()
+            finally:
+                self.f.close()
 
     def __enter__(self):
         return self
 
     def dump(self):
         self.root.dump()
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/interpolation.py` & `pyaaf2-1.7.0/src/aaf2/interpolation.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     absolute_import,
     print_function,
     division,
     )
 import math
 import sys
 
-EPSILON = sys.float_info.epsilon
+EPSILON = 1e-10 # sys.float_info.epsilon
 
 def lerp(a, b, t):
     return a + (b - a) * t
 
 def cubic_bezier(p0, p1, p2, p3, t):
     u = 1.0 - t
     w1 = u * u * u
@@ -141,17 +141,15 @@
     #      /|<- result
     #     / |
     #    /  |
     #   /   |
     #  /    |
     # /p0---p2
     y = (p1[1] - p0[1]) * (p2[0] - p0[0]) / (p1[0] - p0[0])
-    p.y = p0.y + y;
-    p.x = p2.x;
-    return [p2[0], p[1] + y]
+    return [p2[0], p0[1] + y]
 
 def bezier_interpolate(p0, p1, p2, p3, x):
 
     # degenerate cases 1
     # p0 is after p3
     if p0[0] >= p3[0]:
         return p[1]
@@ -175,31 +173,32 @@
     pb = p1[0] - x
     pc = p2[0] - x
     pd = p3[0] - x
 
     # solve for x = 0
     roots = bezier_cubic_roots(pa, pb, pc, pd)
     if not roots:
+        # fall back to old method or decrease EPSILON precision?
         assert False
 
     # use the root as t for y
-    y = cubic_bezier(p0[1], p1[1], p2[1], p3[1], roots[0])
+    y = cubic_bezier(p0[1], p1[1], p2[1], p3[1], min(1.0, max(0, roots[0])))
     return y
 
 def bezier_interpolate_old(p0, p1, p2, p3, t):
 
     t_len = p3[0] - p0[0]
     t_diff = t - p0[0]
     t_mix = t_diff/t_len
 
     guess_t = t_mix
 
     # approximate the correct t value,
     # maybe this is the newtonian method?
-    # I kind of made it up, its slow but seems to work..
+    # I kind of made it up, its slow but seems to work
     for i in range(20):
         x = cubic_bezier(p0[0], p1[0], p2[0], p3[0], guess_t)
         if x == t:
             break
         offset = x - t
         guess_t -= offset/t_len
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/metadict.py` & `pyaaf2-1.7.0/src/aaf2/metadict.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import (
     unicode_literals,
     absolute_import,
     print_function,
     division,
     )
-import traceback
+
 from io import BytesIO
-from .exceptions import AAFPropertyError
 from . import types
 from .model import classdefs
 from .model import typedefs as base_typedefs
 from . import properties
 from .auid import AUID
 
 from . import core
@@ -27,14 +26,15 @@
 
 PID_PARENT     = 0x0008
 PID_PROPERTIES = 0x0009
 PID_CONCRETE   = 0x000A
 
 sentinel = object()
 
+
 @register_class
 class PropertyDef(core.AAFObject):
     class_id = AUID("0d010101-0202-0000-060e-2b3402060101")
     __slots__ = ('_typedef_id', '_auid', '_property_name')
 
     def __new__(cls, root=None, name=None, auid=None, pid=None, typedef=None, optional=None, unique=None):
         self = super(PropertyDef, cls).__new__(cls)
@@ -46,17 +46,14 @@
             properties.add_string_property(self, PID_NAME, name)
             properties.add_bool_property(self, PID_OPTIONAL, optional)
             properties.add_bool_property(self, PID_UNIQUE, unique)
             properties.add_u16le_property(self, PID_PID, pid)
             properties.add_auid_property(self, PID_AUID, auid)
             properties.add_auid_property(self, PID_TYPE, typedef)
 
-        # if auid == AUID("0e040101-0101-0111-060e-2b3401010101"):
-        #     print(name, pid)
-
         return self
 
     @property
     def property_name(self):
         if self._property_name:
             return self._property_name
 
@@ -120,15 +117,16 @@
             return self.root.metadict.lookup_typedef(type_id)
 
     @property
     def store_format(self):
         return self.typedef.store_format
 
     def __repr__(self):
-        return "<%s PropertyDef" % self.property_name
+        return "<%s PropertyDef>" % self.property_name
+
 
 @register_class
 class ClassDef(core.AAFObject):
     class_id = AUID("0d010101-0201-0000-060e-2b3402060101")
     __slots__ = ('propertydef_by_pid')
 
     def __new__(cls, root=None, name=None, class_auid=None, parent_auid=None, concrete=None):
@@ -226,37 +224,48 @@
 
     @property
     def propertydefs(self):
         if PID_PROPERTIES in self.property_entries:
             return self.property_entries[PID_PROPERTIES].values()
         return []
 
+    def lookup_propertydef(self, property_auid):
+        for classdef in self.relatives():
+            p = classdef.property_entries.get(PID_PROPERTIES, {}).get(property_auid, None)
+            if p:
+                return p
+
     def register_propertydef(self, name, property_auid, pid, typedef, optional, unique=False):
 
-        typedef = str2auid(typedef)
+        # check if PropertyDef is already defined
         property_auid = str2auid(property_auid)
+        p = self.property_entries.get(PID_PROPERTIES, {}).get(property_auid, None)
+        if p:
+            return p
+
+        typedef = str2auid(typedef)
         if isinstance(typedef, AUID):
             typedef_auid = typedef
         else:
             typedef = self.root.metadict.lookup_typedef(typedef)
             typedef_auid = typedef.auid
 
-        # check its not already defined
-        if property_auid in self.property_entries[PID_PROPERTIES].references:
-            return self.property_entries[PID_PROPERTIES].get(property_auid)
-
         # None signifies Dynamically allocated Local Tags
         # I think this is similar to MXF where pids > 0x8000 < 0xFFFF
         # are extensions pids
         if pid is None:
-            assert False
             pid = self.root.metadict.next_free_pid()
+            # assert False
 
         p = PropertyDef(self.root, name, property_auid, pid, typedef_auid, optional, unique)
         # # this is done low level to avoid recursion errors
+
+        if PID_PROPERTIES not in self.property_entries:
+            properties.add_strongref_set_property(self, PID_PROPERTIES, "Properties", PID_AUID)
+
         properties.add2set(self, PID_PROPERTIES, p.auid, p)
         self.propertydef_by_pid[pid] = p
         return p
 
     def relatives(self):
         root = self
         while root:
@@ -285,14 +294,15 @@
             return p
 
         return default
 
     def __repr__(self):
         return "<%s %s>" % (self.class_name, "ClassDef")
 
+
 root_classes = {
 'Root' : ('b3b398a5-1c90-11d4-8053-080036210804', None, True, {
     "Header"              : ('0d010301-0102-0100-060e-2b3401010102', 0x0002, '05022800-0000-0000-060E-2B3401040101', False, False),
     "MetaDictionary"      : ('0d010301-0101-0100-060e-2b3401010102', 0x0001, '05022700-0000-0000-060E-2B3401040101', False, False),
 })
 }
 
@@ -300,14 +310,15 @@
 "HeaderStrongRefence"             : ('05022800-0000-0000-060E-2B3401040101', "0d010101-0101-2f00-060e-2b3402060101"),
 "MetaDictionaryStrongReference"   : ('05022700-0000-0000-060E-2B3401040101', "0d010101-0225-0000-060e-2b3402060101"),
 }
 
 PID_CLASSDEFS = 0x0003
 PID_TYPEDEFS  = 0x0004
 
+
 @register_class
 class MetaDictionary(core.AAFObject):
     class_id = AUID("0d010101-0225-0000-060e-2b3402060101")
     def __init__(self, root):
         super(MetaDictionary, self).__init__(root)
 
         self.root = root
@@ -422,14 +433,85 @@
         self.classdefs_by_auid[c.auid] = c
 
         # Root is not include in the data model for some reason
         if c.class_name != "Root":
             properties.add2set(self, PID_CLASSDEFS, c.auid, c)
         return c
 
+    def register_external_typedef(self, ext_typedef):
+        if not isinstance(ext_typedef, types.TypeDef):
+            return None
+
+        typedef = self.lookup_typedef(ext_typedef.auid)
+
+        # create typedef if missing
+        if not typedef:
+            if isinstance(ext_typedef, (types.TypeDefStrongRef,
+                                        types.TypeDefWeakRef)):
+                # could this cause RecursionError?
+                classdef = ext_typedef.ref_classdef
+                self.register_external_classdef(classdef)
+
+            elif isinstance(ext_typedef, (types.TypeDefFixedArray,
+                                          types.TypeDefVarArray,
+                                          types.TypeDefSet,
+                                          types.TypeDefString,
+                                          types.TypeDefEnum)):
+
+                self.register_external_typedef(ext_typedef.element_typedef)
+
+            elif isinstance(ext_typedef, types.TypeDefRecord):
+                for t in ext_typedef.member_types:
+                    self.register_external_typedef(t)
+
+            elif isinstance(ext_typedef, types.TypeDefRename):
+                self.register_external_typedef(ext_typedef.renamed_typedef)
+
+            elif isinstance(ext_typedef, types.TypeDefEnum):
+                self.register_external_typedef(ext_typedef.element_typedef)
+
+            typedef = ext_typedef.copy(self.root)
+
+            self['TypeDefinitions'].append(typedef)
+            self.typedefs_by_name[typedef.type_name] = typedef
+            self.typedefs_by_auid[typedef.auid] = typedef
+
+        # make sure enum has all the values
+        if isinstance(ext_typedef, (types.TypeDefExtEnum, types.TypeDefEnum)):
+            ext_elements = ext_typedef.elements
+            elements = typedef.elements
+
+            for k, v in ext_elements.items():
+                if k not in elements:
+                    typedef.register_element(v, k)
+
+        return typedef
+
+    def register_external_classdef(self, ext_classdef):
+        class_chain = list(ext_classdef.relatives())
+        class_chain.reverse()
+        for c in class_chain[1:]:
+            classdef = self.lookup_classdef(c.auid)
+            if not classdef:
+                classdef = self.register_classdef(c.class_name,
+                                                  c.auid,
+                                                  c.parent.auid,
+                                                  c.concrete)
+
+            for p in c.propertydefs:
+                typedef = self.register_external_typedef(p.typedef)
+                pid = p.pid
+
+                if pid >= 0x8000:
+                    pid = None
+
+                classdef.register_propertydef(p.property_name, p.auid, pid, typedef.auid, p.optional, p.unique)
+
+        return self.lookup_classdef(ext_classdef.auid)
+
     def lookup_class(self, class_id):
         aaf_class = AAFClaseID_dict.get(class_id, None)
         if aaf_class:
             return aaf_class
 
         aaf_class = AAFClassName_dict.get(class_id, None)
         if aaf_class:
@@ -471,15 +553,14 @@
 
         result = self.next_pid
         self.next_pid -= 1
 
         self.local_pids.add(result)
         return result
 
-
     def read_properties(self):
         super(MetaDictionary, self).read_properties()
         for key, typedef in self['TypeDefinitions'].items():
             self.typedefs_by_name[typedef.type_name] = typedef
             self.typedefs_by_auid[typedef.auid] = typedef
 
         # reset local pids
@@ -499,15 +580,14 @@
 
         # add typedefs not defined by file data model
         if self.root.writeable:
             for key, typedef in self.typedefs_by_auid.items():
                 # skip root typedefs
                 if key in (AUID('05022800-0000-0000-060E-2B3401040101'),
                            AUID('05022700-0000-0000-060E-2B3401040101')):
-                    # print("skipping root typedef")
                     continue
 
                 if key not in self['TypeDefinitions']:
                     # this is super annoying, handle typedefs that have dynamic pids
                     classdef = self.classdefs_by_auid.get(typedef.class_id)
                     assert classdef
                     for pdef in classdef['Properties'].values():
@@ -517,26 +597,24 @@
                                 old_pid = pdef.pid
                                 new_pid = self.next_free_pid()
                                 pdef.pid = new_pid
 
                                 prop = typedef.property_entries.pop(old_pid)
                                 prop.pid = new_pid
                                 typedef.property_entries[new_pid] = prop
-                                # print("conflcit", typedef, pdef.name, old_pid, "->", new_pid)
 
                     self['TypeDefinitions'].append(typedef)
                     if classdef.auid not in self['ClassDefinitions']:
                         self['ClassDefinitions'].append(classdef)
 
         # add classdefs not defined by file data model
         if self.root.writeable:
             for key, classdef in self.classdefs_by_auid.items():
                 # skip root classdefs
                 if key in (AUID('b3b398a5-1c90-11d4-8053-080036210804'), ):
-                    # print("skipping root")
                     continue
 
                 if key not in self['ClassDefinitions']:
 
                     # handle any conflicting dynamic pids
                     for pdef in classdef['Properties'].values():
                         if pdef.pid >= 0x8000:
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/misc.py` & `pyaaf2-1.7.0/src/aaf2/misc.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/mobid.py` & `pyaaf2-1.7.0/src/aaf2/mobid.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     the material. The purpose of the instance number is to separately identify different representations or instances of
     audiovisual material. Thus, for example, a high-resolution picture and a thumbnail can both have the same
     material number because they both represent the same picture but, because they are different instances, they will
     have different instance numbers for the different representations. Guidance for the consistent application of new
     material numbers and instance numbers is given in SMPTE RP 205.
 
 
-    UMID univeral label (SMPTELabel)
+    UMID universal label (SMPTELabel)
 
     Byte No.   Description            Value (hex)                 Meaning
     ----------------------------------------------------------------------------------------
     1          Object identifier      06h                         Universal label start
     2          Label size             0Ah                         12-byte Universal label
     3          Designation: ISO       2Bh                         ISO registered
     4          Designation: SMPTE     34h                         SMPTE registered
@@ -56,15 +56,15 @@
     7          Structure              01h                         Dictionary standard (SMPTE ST 335)
     8          Version number         05h                         Version of the metadata dictionary (defined in SMPTE RP 210)
     9          Class                  01h                         Identifiers and locators
     10         Subclass               01h                         Globally unique identifiers
     11         Material type          XXh                         See Section 6.1.2.1
     12         Number creation method YYh                         See Section 6.1.2.2
 
-    6.1.2.1 - Meterial type identification
+    6.1.2.1 - Material type identification
 
     Byte 11 of the UL shall define the material type being identified using one of the values defined in Table 2.
     The use of material types '01h', '02h', '03h' and '04h' shall be deprecated for use in implementations using
     this revised standard. These values are preserved only for compatibility with systems implemented using
     SMPTE ST 330:2000#
 
     Table 2
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/mobs.py` & `pyaaf2-1.7.0/src/aaf2/mobs.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from . utils import register_class, rescale
 from . misc import TaggedValueHelper
 from . import essence
 from . import video
 from . import audio
 from .rational import AAFRational
 from .auid import AUID
+from .components import SourceReference
 
 
 @register_class
 class Mob(core.AAFObject):
     """
     Base Class for All Mob Objects
     """
@@ -101,55 +102,83 @@
 
         slot = self.root.create.TimelineMobSlot(slot_id, edit_rate=edit_rate)
         self.slots.append(slot)
         return slot
 
     def create_empty_sequence_slot(self, edit_rate, slot_id=None,  media_kind=None):
         """
-            Create an empty timeline slot and sets its segment to a new, empty 
-            `aaf2.components.Sequence` component. Timeline slots are for continuous, 
+            Create an empty timeline slot and sets its segment to a new, empty
+            `aaf2.components.Sequence` component. Timeline slots are for continuous,
             monotonically-changing media, like picture and sound.
         """
         slot = self.create_timeline_slot(edit_rate, slot_id)
         sequence = self.root.create.Sequence(media_kind=media_kind)
         sequence['Components'].value = []
         slot.segment = sequence
         return slot
 
     def create_picture_slot(self, edit_rate=25):
         """
-            Create an empty timeline slot, with the 'picture' media kind, and sets 
+            Create an empty timeline slot, with the 'picture' media kind, and sets
             its segment to a new, empty `aaf2.components.Sequence` component.
         """
         return self.create_empty_sequence_slot(edit_rate, media_kind="picture")
 
     def create_sound_slot(self, edit_rate=25):
         """
-            Create an empty timeline slot, with the 'sound' media kind, and sets 
+            Create an empty timeline slot, with the 'sound' media kind, and sets
             its segment to a new, empty `aaf2.components.Sequence` component.
         """
         return self.create_empty_sequence_slot(edit_rate, media_kind="sound")
 
     def create_source_clip(self, slot_id=None, start=None, length=None, media_kind=None):
         """
             Create a SourceClip of Mobs slot with `slot_id`. If no length given the default
-            length will be the full length of slots segment minius `start`.
+            length will be the full length of slots segment minus `start`.
             Returns :class:`aaf2.components.SourceClip` Object
         """
         source_slot = self.slot_at(slot_id)
         if not media_kind:
             media_kind = source_slot.media_kind
 
         clip = self.root.create.SourceClip(media_kind=media_kind)
         clip.mob = self
         clip.slot = source_slot
         clip.start = start or 0
         clip.length = length or max(source_slot.length - clip.start, 0)
         return clip
 
+    def dependant_mobs(self):
+        """
+            Yields all mobs that this mob is dependant on in depth first order.
+        """
+
+        visited = set()
+        stack = [self]
+
+        while stack:
+            mob = stack[-1]
+            children_processed = True
+
+            for obj, _ in mob.walk_references(topdown=True):
+                if isinstance(obj, SourceReference):
+                    ref_mob = obj.mob
+                    if not ref_mob:
+                        continue
+                    if ref_mob.mob_id not in visited:
+                        stack.append(ref_mob)
+                        children_processed = False
+
+            if children_processed:
+                stack.pop(-1)
+                if mob.mob_id not in visited:
+                    visited.add(mob.mob_id)
+                    if mob is not self:
+                        yield mob
+
     def __repr__(self):
         s = "%s.%s" % (self.__class__.__module__,
                        self.__class__.__name__)
         s += ' "%s" %s' % (self.name or "", str(self.mob_id))
 
         return '<%s at 0x%x>' % (s, id(self))
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/mobslots.py` & `pyaaf2-1.7.0/src/aaf2/mobslots.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/model/classdefs.py` & `pyaaf2-1.7.0/src/aaf2/model/classdefs.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/model/datadefs.py` & `pyaaf2-1.7.0/src/aaf2/model/datadefs.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/model/ext/classdefs.py` & `pyaaf2-1.7.0/src/aaf2/model/ext/classdefs.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/model/ext/typedefs.py` & `pyaaf2-1.7.0/src/aaf2/model/ext/typedefs.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/model/typedefs.py` & `pyaaf2-1.7.0/src/aaf2/model/typedefs.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/mxf.py` & `pyaaf2-1.7.0/src/aaf2/mxf.py`

 * *Files 6% similar despite different names*

```diff
@@ -505,15 +505,15 @@
             if tag == 0x3f01:
                 self.data['FileDescriptors'] = decode_strong_ref_array(f)
             elif tag == 0x3004:
                 self.data['ContainerFormat'] = reverse_auid(decode_auid(data))
             elif tag == 0x3005:
                 self.data['CodecDefinition'] = reverse_auid(decode_auid(data))
             elif tag == 0x3006:
-                self.data['LinkedTrackID'] = read_u32be(f)
+                self.data['LinkedSlotID'] = read_u32be(f)
             elif tag == 0x3203:
                 self.data['StoredWidth'] = read_u32be(f)
             elif tag == 0x3202:
                 self.data['StoredHeight'] = read_u32be(f)
             elif tag == 0x3208: #this is display
                 self.data['SampledHeight'] = read_u32be(f)
             elif tag == 0x3209: #this is display
@@ -599,18 +599,17 @@
         # required
         for key in ('ComponentWidth', 'HorizontalSubsampling', 'ImageAspectRatio',
            'StoredWidth', 'VideoLineMap', 'StoredHeight', 'SampleRate', 'FrameLayout'):
            d[key].value = self.data[key]
 
         d['Length'].value = self.data.get('Length', 0)
 
-
         # optional
         for key in ('FrameSampleSize', 'ResolutionID', 'Compression', 'VerticalSubsampling',
-                    'SampledWidth', 'SampledHeight'):
+                    'SampledWidth', 'SampledHeight', 'LinkedSlotID'):
             if key in self.data:
                 d[key].value = self.data[key]
 
         for item in self.iter_strong_refs("Locator"):
             d['Locator'].append(item.link())
             n = self.root.aaf.create.NetworkLocator()
             n['URLString'].value = ama_path(self.root.path)
@@ -632,18 +631,21 @@
     def create_aaf_instance(self):
         return self.root.aaf.create.RGBADescriptor()
 
     def link(self):
         d = self.create_aaf_instance()
 
         for key in ('ImageAspectRatio', 'StoredWidth', 'FrameLayout', 'PixelLayout',
-                    'VideoLineMap', 'StoredHeight', 'SampleRate', 'Length'):
+                    'VideoLineMap', 'StoredHeight', 'SampleRate', ):
             d[key].value = self.data[key]
 
-        for key in ('FrameSampleSize','SampledWidth', 'SampledHeight', 'Compression',):
+        d['Length'].value = self.data.get('Length', 0)
+
+        # optional
+        for key in ('FrameSampleSize','SampledWidth', 'SampledHeight', 'Compression', 'LinkedSlotID'):
             if key in self.data:
                 d[key].value = self.data[key]
 
         d['ContainerFormat'].value = self.root.aaf.dictionary.lookup_containerdef("AAFKLV")
         n = self.root.aaf.create.NetworkLocator()
         n['URLString'].value = ama_path(self.root.path)
         d['Locator'].append(n)
@@ -661,41 +663,64 @@
     class_id = AUID("060e2b34-0253-0101-0d01-010101015c00")
 
     def create_aaf_instance(self):
         return self.root.aaf.create.ANCDataDescriptor()
 
     def link(self):
         d = self.create_aaf_instance()
-        for key in ('SampleRate', 'Length',):
+        for key in ('SampleRate', ):
             d[key].value = self.data[key]
+
+        d['Length'].value = self.data.get('Length', 0)
+
+        # optional
+        for key in ('LinkedSlotID', ):
+            if key in self.data:
+                d[key].value = self.data[key]
+
         return d
 
 @register_mxf_class
 class MXFMPEG2VideoDescriptor(MXFCDCIDescriptor):
     class_id = AUID("060e2b34-0253-0101-0d01-010101015100")
 
     def link(self):
         # 060e2b34.04010103.04010202.01040300
         self.data['ResolutionID'] = 4076 #XDCAM HD 50Mbit
 
+        d['Length'].value = self.data.get('Length', 0)
+
+        # optional
+        for key in ('LinkedSlotID', ):
+            if key in self.data:
+                d[key].value = self.data[key]
+
         return super(MXFMPEG2VideoDescriptor, self).link()
 
 @register_mxf_class
 class MXFPCMDescriptor(MXFDescriptor):
     class_id = AUID("060e2b34-0253-0101-0d01-010101014800")
 
     def create_aaf_instance(self):
         return self.root.aaf.create.PCMDescriptor()
 
     def link(self):
         d = self.create_aaf_instance()
         # required
         for key in ('BlockAlign', 'AverageBPS', 'Channels',
-            'QuantizationBits', 'AudioSamplingRate', 'SampleRate', 'Length'):
+            'QuantizationBits', 'AudioSamplingRate', 'SampleRate'):
             d[key].value = self.data[key]
+
+        d['Length'].value = self.data.get('Length', 0)
+
+        # optional
+        for key in ('LinkedSlotID', ):
+            if key in self.data:
+                d[key].value = self.data[key]
+
         n = self.root.aaf.create.NetworkLocator()
         n['URLString'].value = ama_path(self.root.path)
         d['Locator'].append(n)
         if self.root.ama:
             n =  self.root.aaf.create.NetworkLocator()
             n['URLString'].value = ama_path(self.root.path)
             d['Locator'].append(n)
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/properties.py` & `pyaaf2-1.7.0/src/aaf2/properties.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from __future__ import (
     unicode_literals,
     absolute_import,
     print_function,
     division,
     )
 
@@ -35,39 +34,42 @@
 SF_DATA_STREAM                            = 0x42
 SF_STRONG_OBJECT_REFERENCE                = 0x22
 SF_STRONG_OBJECT_REFERENCE_VECTOR         = 0x32
 SF_STRONG_OBJECT_REFERENCE_SET            = 0x3A
 SF_WEAK_OBJECT_REFERENCE                  = 0x02
 SF_WEAK_OBJECT_REFERENCE_VECTOR           = 0x12
 SF_WEAK_OBJECT_REFERENCE_SET              = 0x1A
+
+# these formats are defined by spec but not used
 SF_WEAK_OBJECT_REFERENCE_STORED_OBJECT_ID = 0x03
 SF_UNIQUE_OBJECT_ID                       = 0x86
 SF_OPAQUE_STREAM                          = 0x40
-
-# not sure about these
 SF_DATA_VECTOR                            = 0xD2
 SF_DATA_SET                               = 0xDA
 
+CLASSDEF_AUID          = AUID("0d010101-0101-0100-060e-2b3402060101")
+TYPEDEF_AUID           = AUID("0d010101-0203-0000-060e-2b3402060101")
+
+MOB_MOBID_AUID         = AUID("01011510-0000-0000-060e-2b3401010101")
+ESSENCEDATA_MOBID_AUID = AUID("06010106-0100-0000-060e-2b3401010102")
+
 PROPERTY_VERSION=32
+sentinel = object()
+
 
 def writeonly(func):
     def func_wrapper(self, *args, **kwargs):
         if not self.writeable:
             raise AAFPropertyError("file readonly")
         result = func(self, *args, **kwargs)
         self.mark_modified()
         return result
 
     return func_wrapper
 
-CLASSDEF_AUID = AUID("0d010101-0101-0100-060e-2b3402060101")
-TYPEDEF_AUID = AUID("0d010101-0203-0000-060e-2b3402060101")
-
-MOB_MOBID_AUID = AUID("01011510-0000-0000-060e-2b3401010101")
-ESSENCEDATA_MOBID_AUID = AUID("06010106-0100-0000-060e-2b3401010102")
 
 class Property(object):
     __slots__ = ('pid', 'format', 'version', 'data', 'parent', '_propertydef')
     def __init__(self, parent, pid, format, version=PROPERTY_VERSION):
         self.pid = pid
         self.format = format
         self.version = version
@@ -129,16 +131,16 @@
 
     @property
     def typedef(self):
         propertydef = self.propertydef
         if propertydef:
             return propertydef.typedef
 
-    def copy(self, parent):
-        p = self.__class__(parent, self.pid, self.format, version=PROPERTY_VERSION)
+    def copy(self, parent, pid, cache=None):
+        p = self.__class__(parent, pid, self.format, version=PROPERTY_VERSION)
         p.data = bytes(self.data)
         return p
 
     @property
     def value(self):
         d = self.data
         if d is None:
@@ -175,41 +177,40 @@
     def __repr__(self):
         name = self.name
         if name:
             return "<%s %s>" % (name, str(self.typedef))
         else:
             return "<%s %d bytes>" % (self.__class__.__name__, len(self.data))
 
+
 class StreamProperty(Property):
     __slots__ = ('stream_name', 'dir')
     def __init__(self, parent, pid, format, version=PROPERTY_VERSION):
         super(StreamProperty, self).__init__(parent, pid, format, version)
         self.stream_name = None
         self.dir = None
 
-    def copy(self, parent):
-        p = super(StreamProperty, self).copy(parent)
-        p.stream_name = self.stream_name
-
+    def copy(self, parent, pid, cache):
+        p = super(StreamProperty, self).copy(parent, pid)
         a = self.open('r')
         b = p.open("w")
 
         byte_size = a.dir.byte_size
         read_size = self.parent.root.cfb.sector_size
 
         # copy stream data
         while byte_size > 0:
             d = a.read(read_size)
             b.write(d)
-            byte_size -= read_size
+            byte_size -= len(d)
 
         return p
 
     def decode(self):
-        # first byte is endianess
+        # first byte is endianness
         assert self.data[0:1] == b'\x55' # unspecified
         self.stream_name = decode_utf16le(self.data[1:])
 
     def encode(self, data):
         return  b'\x55' + encode_utf16le(data)
 
     def __repr__(self):
@@ -281,14 +282,15 @@
 
         self.dir = None
 
     @property
     def value(self):
         return self.parent.dir.get(self.stream_name)
 
+
 class StrongRefProperty(Property):
     __slots__ = ('ref', 'objectref')
     def __init__(self, parent, pid, format, version=PROPERTY_VERSION):
         super(StrongRefProperty, self).__init__(parent, pid, format, version)
         self.ref = None
         self.objectref = None
 
@@ -306,25 +308,27 @@
         if value is None:
             self.objectref = None
         elif self.attached:
             self.objectref = weakref.ref(value)
         else:
             self.objectref = value
 
-    def copy(self, parent):
-        p = super(StrongRefProperty, self).copy(parent)
-        p.ref = self.ref
-
-        dir_entry = None
-        if parent.dir:
-            dir_entry = parent.dir.get(p.ref)
-            if dir_entry is None:
-                dir_entry = parent.dir.makedir(p.ref)
+    def copy(self, parent, pid, cache):
+        p = super(StrongRefProperty, self).copy(parent, pid)
+        if parent.root is self.parent.root:
+            p.ref = self.ref
+            dir_entry = None
+            if parent.dir:
+                dir_entry = parent.dir.get(p.ref)
+                if dir_entry is None:
+                    dir_entry = parent.dir.makedir(p.ref)
 
-        p.object = self.value.copy(dir_entry)
+            p.object = self.value.copy(dir_entry)
+        else:
+            p.value = self.value.copy(root=parent.root, classdef_cache=cache)
         return p
 
     def decode(self):
         self.ref = decode_utf16le(self.data)
 
     def encode(self, data):
         return encode_utf16le(data)
@@ -339,28 +343,30 @@
         dir_entry = self.parent.dir.get(self.ref)
         obj = None
         if dir_entry:
             obj = self.parent.root.manager.read_object(dir_entry)
             self.object = obj
         return obj
 
-
     @value.setter
     @writeonly
     def value(self, value):
         if value is None:
             self.remove_pid_entry()
             return
 
         typedef = self.typedef
         ref_classdef = typedef.ref_classdef
 
         if not ref_classdef.isinstance(value.classdef):
             raise TypeError("must be instance of: %s" % ref_classdef.class_name)
 
+        if value.root is not self.parent.root:
+            raise AAFAttachError("Object is from a different root")
+
         if self.ref is None:
             propdef = self.propertydef
             self.ref = mangle_name(propdef.property_name, self.pid, 32)
             self.data = self.encode(self.ref)
 
         # before assigning new object detach old
         if self.object:
@@ -410,34 +416,39 @@
         self.last_free_key = 0xFFFFFFFF
 
         if self.attached:
             self.objects = weakref.WeakValueDictionary()
         else:
             self.objects = {}
 
-    def copy(self, parent):
-        p = super(StrongRefVectorProperty, self).copy(parent)
-        p.references = list(self.references)
-
-        p.objects = {}
-        p.index_name = self.index_name
-        p.next_free_key = self.next_free_key
-        p.last_free_key = self.last_free_key
-        p.data = self.data
+    def copy(self, parent, pid, cache):
+        p = super(StrongRefVectorProperty, self).copy(parent, pid)
 
-        for i, value in enumerate(self):
-            ref = self.index_ref_name(self.references[i])
-            dir_entry = None
-            if parent.dir:
-                dir_entry = parent.dir.get(ref)
-                if dir_entry is None:
-                    dir_entry = parent.dir.makedir(ref)
+        if parent.root is self.parent.root:
+            p.objects = {}
+            p.references = list(self.references)
+            p.index_name = p.index_name
+            p.next_free_key = self.next_free_key
+            p.last_free_key = self.last_free_key
+            p.data = self.data
+
+            for i, value in enumerate(self):
+                ref = self.index_ref_name(self.references[i])
+                dir_entry = None
+                if parent.dir:
+                    dir_entry = parent.dir.get(ref)
+                    if dir_entry is None:
+                        dir_entry = parent.dir.makedir(ref)
 
-            c = value.copy(dir_entry)
-            p.objects[i] = c
+                c = value.copy(dir_entry)
+                p.objects[i] = c
+        else:
+            for i, value in enumerate(self):
+                c = value.copy(root=parent.root, classdef_cache=cache)
+                p.append(c)
 
         return p
 
     @property
     def index_name(self):
         if self._index_name:
             return self._index_name
@@ -518,29 +529,32 @@
         for i in range(len(self.references)):
             yield self.get(i)
 
     def __len__(self):
         return len(self.references)
 
     def __getitem__(self, index):
-        item = self.get(index, None)
-        if item is None:
+        item = self.get(index, sentinel)
+        if item is sentinel:
             raise IndexError(index)
         return item
 
     @writeonly
     def __setitem__(self, index, value):
         if index < 0:
             index = max(0, len(self) + index)
 
         if index >= len(self):
             raise IndexError("StrongRefVectorProperty assignment index out of range")
 
+        if value.root is not self.parent.root:
+            raise AAFAttachError("Object is from a different root")
+
         if value.dir:
-            raise AAFAttachError("object already attached")
+            raise AAFAttachError("Object already attached")
 
         obj = self.get(index, None)
         if obj:
             obj.detach()
 
         self.objects[index] = value
         self.attach()
@@ -613,16 +627,20 @@
     @writeonly
     def extend(self, value):
         index_name = self.index_name # sets self.data
         ref_classdef = self.ref_classdef
 
         for obj in value:
             assert ref_classdef.isinstance(obj.classdef)
+
+            if obj.root is not self.parent.root:
+                raise AAFAttachError("Object is from a different root")
+
             if obj.dir:
-                raise AAFAttachError("object already attached")
+                raise AAFAttachError("Object already attached")
 
         for obj in value:
             i = len(self.references)
             self.references.append(self.next_free_key)
             self.objects[i] = obj
             self.next_free_key += 1
 
@@ -688,32 +706,37 @@
         self.key_size = None
 
         if self.attached:
             self.objects = weakref.WeakValueDictionary()
         else:
             self.objects = {}
 
-    def copy(self, parent):
-        p = super(StrongRefSetProperty, self).copy(parent)
+    def copy(self, parent, pid, cache):
+        p = super(StrongRefSetProperty, self).copy(parent, pid)
 
-        p.references = dict(self.references)
-        p.next_free_key = self.next_free_key
-        p.last_free_key = self.last_free_key
-        p.key_size = self.key_size
-        p.index_name = self.index_name
-        p.key_pid = self.key_pid
+        if parent.root is self.parent.root:
+            p.references = dict(self.references)
+            p.next_free_key = self.next_free_key
+            p.last_free_key = self.last_free_key
+            p.key_size = self.key_size
+            p.index_name = self.index_name
+            p.key_pid = self.key_pid
 
-        for key, value in self.items():
-            ref = self.index_ref_name(key)
-            dir_entry = None
-            if parent.dir:
-                dir_entry = parent.dir.get(ref)
-                if dir_entry is None:
-                    dir_entry = parent.dir.makedir(ref)
-            p.objects[key] = value.copy(dir_entry)
+            for key, value in self.items():
+                ref = self.index_ref_name(key)
+                dir_entry = None
+                if parent.dir:
+                    dir_entry = parent.dir.get(ref)
+                    if dir_entry is None:
+                        dir_entry = parent.dir.makedir(ref)
+                p.objects[key] = value.copy(dir_entry)
+        else:
+            for value in self.values():
+                c = value.copy(root=parent.root, classdef_cache=cache)
+                p.append(c)
 
         return p
 
     def encode(self, data):
         return encode_utf16le(data)
 
     def decode(self):
@@ -811,27 +834,22 @@
 
     def __iter__(self):
         return self.values()
 
     def __len__(self):
         return len(self.references)
 
-    def get_object(self, key):
-        for obj in self.value:
-            if obj.name == key:
-                return obj
-
     def get(self, key, default=None):
         if key not in self:
-            return default or self.get_object(key)
+            return default
         return self.read_object(key)
 
     def __getitem__(self, key):
-        result = self.get(key, default=None)
-        if result is None:
+        result = self.get(key, default=sentinel)
+        if result is sentinel:
             raise KeyError(key)
         return result
 
     @writeonly
     def swap_unique_key(self, old_key, new_key):
         obj = self.get(old_key)
 
@@ -852,16 +870,18 @@
         typedef = self.typedef
         classdef = typedef.ref_classdef
 
         # check values are the correct type
         for item in values:
             if not classdef.isinstance(item.classdef):
                 raise TypeError("Invalid Value, expected {}, got {}".format(classdef, item.classdef))
+            if item.root is not self.parent.root:
+                raise AAFAttachError("Object is from a different root")
             if item.dir:
-                raise AAFAttachError("object already attached")
+                raise AAFAttachError("Object already attached")
 
         if self.key_pid is None:
             self.key_pid = classdef.unique_key_pid
         if self.key_size is None:
             self.key_size = classdef.unique_key_size
 
         if self.index_name is None:
@@ -918,15 +938,14 @@
         self.references.pop(key)
         self.objects.pop(key)
 
         obj.detach()
 
         return obj
 
-
     @property
     def value(self):
         return [item for item in self]
 
     @value.setter
     @writeonly
     def value(self, value):
@@ -963,14 +982,15 @@
             if obj.dir != dir_entry:
                 obj.attach(dir_entry)
 
 
     def __repr__(self):
         return "<%s to %s %d items>" % (self.__class__.__name__, str(self.index_name), len(self.references))
 
+
 def resolve_weakref(p, ref):
     ref_class_id = p.ref_classdef.auid
     if ref_class_id == CLASSDEF_AUID:
         return p.parent.root.metadict.lookup_classdef(ref)
     elif ref_class_id == TYPEDEF_AUID:
         return p.parent.root.metadict.lookup_typedef(ref)
     else:
@@ -981,20 +1001,39 @@
     def __init__(self, parent, pid, format, version=PROPERTY_VERSION):
         super(WeakRefProperty, self).__init__(parent, pid, format, version)
         self.weakref_index = None
         self.key_pid = None
         self.key_size = None
         self.ref = None
 
-    def copy(self, parent):
-        p = super(WeakRefProperty, self).copy(parent)
-        p.weakref_index = self.weakref_index
-        p.key_pid = self.pid
-        p.key_size = self.key_size
-        p.ref = self.ref
+    def copy(self, parent, pid, cache):
+        p = super(WeakRefProperty, self).copy(parent, pid)
+
+        if parent.root is self.parent.root:
+            p.weakref_index = self.weakref_index
+            p.key_pid = self.pid
+            p.key_size = self.key_size
+            p.ref = self.ref
+        else:
+            weakref_index = parent.root.weakref_index(p.pid_path)
+            ref_parent, target_property = parent.root.weakref_prop(weakref_index)
+
+            # add property value if not present
+            if self.ref not in target_property:
+                v = self.value
+                if self.ref_classdef.auid == CLASSDEF_AUID:
+                    parent.root.metadict.register_external_classdef(v)
+                if self.ref_classdef.auid == TYPEDEF_AUID:
+                    parent.root.metadict.register_external_typedef(v)
+                else:
+                    c = v.copy(root=parent.root, classdef_cache=cache)
+                    target_property.append(c)
+
+            p.value = target_property[self.ref]
+
         return p
 
     def decode(self):
         with BytesIO(self.data) as f:
             self.weakref_index = read_u16le(f)
             self.key_pid = read_u16le(f)
             self.key_size = read_u8(f)
@@ -1037,42 +1076,55 @@
         if value is None:
             self.remove_pid_entry()
             return
 
         ref_classdef = self.ref_classdef
         assert ref_classdef.isinstance(value.classdef)
 
+        if value.root is not self.parent.root:
+            raise AAFAttachError("Object is from a different root")
+
         if self.key_pid is None:
             self.key_pid = ref_classdef.unique_key_pid
         if self.key_size is None:
             self.key_size = ref_classdef.unique_key_size
         if self.weakref_index is None:
             self.weakref_index = self.parent.root.weakref_index(self.pid_path)
 
         self.ref = value.unique_key
         self.data = self.encode()
         self.add_pid_entry()
 
+
 class WeakRefArrayProperty(Property):
     __slots__ = ('references', 'index_name', 'weakref_index', 'key_pid', 'key_size')
     def __init__(self, parent, pid, format, version=PROPERTY_VERSION):
         super(WeakRefArrayProperty, self).__init__(parent, pid, format, version)
         self.references = []
         self.index_name = None
         self.weakref_index = None
         self.key_pid = None
         self.key_size = None
 
-    def copy(self, parent):
-        p = super(WeakRefArrayProperty, self).copy(parent)
-        p.references = list(self.references)
-        p.index_name = self.index_name
-        p.weakref_index = self.weakref_index
-        p.key_pid = self.key_pid
-        p.key_size = self.key_size
+    def copy(self, parent, pid, cache):
+        p = super(WeakRefArrayProperty, self).copy(parent, pid)
+        if parent.root is self.parent.root:
+            p.references = list(self.references)
+            p.index_name = self.index_name
+            p.weakref_index = self.weakref_index
+            p.key_pid = self.key_pid
+            p.key_size = self.key_size
+        else:
+            weakref_index = parent.root.weakref_index(p.pid_path)
+            ref_parent, target_property = parent.root.weakref_prop(weakref_index)
+            for ref in self.references:
+                # copy property here if not present?
+                assert ref in target_property
+                p.append(target_property[ref])
+
         return p
 
     def encode(self, data):
         return encode_utf16le(data)
 
     def decode(self):
         self.index_name = decode_utf16le(self.data)
@@ -1123,30 +1175,51 @@
     def ref_classdef(self):
         return self.typedef.element_typedef.ref_classdef
 
     @property
     def pid_path(self):
         return self.typedef.element_typedef.pid_path
 
+    def __contains__(self, key):
+        return key in self.references
+
     def __len__(self):
         return len(self.references)
 
     def __iter__(self):
         for ref in self.references:
             r = resolve_weakref(self, ref)
             yield r
 
+    def get(self, key, default=None):
+        if key not in self:
+            return default
+        return resolve_weakref(self, key)
+
+    def __getitem__(self, key):
+        result = self.get(key, default=sentinel)
+        if result is sentinel:
+            raise KeyError(key)
+        return result
+
+    def items(self):
+        for key in self.references:
+            obj = resolve_weakref(self, key)
+            yield (key, obj)
+
     @writeonly
     def extend(self, values):
         ref_classdef = self.ref_classdef
 
         # check values are the correct type
         for item in values:
             if not ref_classdef.isinstance(item.classdef):
                 raise TypeError("Invalid Value")
+            if item.root is not self.parent.root:
+                raise AAFAttachError("Object is from a different root")
 
         if self.index_name is None:
             propdef = self.propertydef
             self.index_name = mangle_name(propdef.property_name, self.pid, 32-10)
             self.data = self.encode(self.index_name)
 
         if self.weakref_index is None:
@@ -1181,25 +1254,29 @@
 
         self.clear()
         self.extend(value)
 
 
 class WeakRefVectorProperty(WeakRefArrayProperty):
     pass
+
+
 class WeakRefSetProperty(WeakRefArrayProperty):
     pass
 
 
 # haven't see aaf files that contain these yet
 class WeakRefPropertyId(WeakRefProperty):
     pass
 
+
 class UniqueIdProperty(Property):
     pass
 
+
 class OpaqueStreamProperty(Property):
     pass
 
 property_formats = {
 SF_DATA                                    : Property,
 SF_DATA_STREAM                             : StreamProperty,
 SF_STRONG_OBJECT_REFERENCE                 : StrongRefProperty,
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/rational.py` & `pyaaf2-1.7.0/src/aaf2/rational.py`

 * *Files identical despite different names*

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/types.py` & `pyaaf2-1.7.0/src/aaf2/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,14 +37,17 @@
         self.root = root
         self._auid = None
         if root:
             properties.add_string_property(self, PID_NAME, name)
             properties.add_auid_property(self, PID_AUID, type_auid)
         return self
 
+    def copy(self, root=None):
+        return self.__class__(root or self.root, self.name, self.auid)
+
     @property
     def unique_key(self):
         return self.auid
 
     @property
     def auid(self):
         if self._auid:
@@ -81,14 +84,17 @@
     def __new__(cls, root=None, name=None, type_auid=None, size=None, signed=None):
         self = super(TypeDefInt, cls).__new__(cls, root, name, type_auid)
         if root:
             properties.add_u8_property(self, PID_INT_SIZE, size)
             properties.add_bool_property(self, PID_INT_SIGNED, signed)
         return self
 
+    def copy(self, root=None):
+        return TypeDefInt(root or self.root, self.name, self.auid, self.size, self.signed)
+
     @property
     def signed(self):
         return self.property_entries[PID_INT_SIGNED].data == b"\x01"
 
     @property
     def size(self):
         data  = self.property_entries[PID_INT_SIZE].data
@@ -136,14 +142,17 @@
 
     def __new__(cls, root=None, name=None, type_auid=None, classdef=None):
         self = super(TypeDefStrongRef, cls).__new__(cls, root, name, type_auid)
         if root:
             properties.add_classdef_weakref_property(self, PID_STRONGREF_REF_TYPE, classdef)
         return self
 
+    def copy(self, root=None):
+        return TypeDefStrongRef(root or self.root, self.name, self.auid, self.ref_classdef.auid)
+
     @property
     def store_format(self):
         return properties.SF_STRONG_OBJECT_REFERENCE
 
     @property
     def ref_classdef(self):
         if PID_STRONGREF_REF_TYPE in self.property_entries:
@@ -161,14 +170,17 @@
         self = super(TypeDefWeakRef, cls).__new__(cls, root, name, type_auid)
         if root:
             properties.add_classdef_weakref_property(self, PID_WEAKREF_REF_TYPE, classdef)
             properties.add_auid_array_propertry(self, PID_WEAKREF_TARGET_SET, path)
 
         return self
 
+    def copy(self, root=None):
+        return TypeDefWeakRef(root or self.root, self.name, self.auid, self.ref_classdef.auid, self.path)
+
     @property
     def store_format(self):
         return properties.SF_WEAK_OBJECT_REFERENCE
 
     @property
     def ref_classdef(self):
         if PID_WEAKREF_REF_TYPE in self.property_entries:
@@ -223,14 +235,17 @@
                 values.append(val)
 
             properties.add_utf16_array_property(self, PID_ENUM_NAMES, names)
             properties.add_s64le_array_property(self, PID_ENUM_VALUES, values)
 
         return self
 
+    def copy(self, root=None):
+        return TypeDefEnum(root or self.root, self.name, self.auid, self.element_typedef.auid, self.elements)
+
     @property
     def byte_size(self):
         return self.element_typedef.byte_size
 
     @property
     def elements(self):
         names = list(iter_utf16_array(self.property_entries[PID_ENUM_NAMES].data))
@@ -307,14 +322,17 @@
     def __new__(cls, root=None, name=None, type_auid=None, typedef=None, size=None):
         self = super(TypeDefFixedArray, cls).__new__(cls, root, name, type_auid)
         if root:
             properties.add_typedef_weakref_property(self, PID_FIXED_TYPE, typedef)
             properties.add_u32le_property(self, PID_FIXED_COUNT, size)
         return self
 
+    def copy(self, root=None):
+        return TypeDefFixedArray(root or self.root, self.name, self.auid, self.element_typedef.auid, self.size)
+
     @property
     def element_typedef(self):
         if PID_FIXED_TYPE in self.property_entries:
             return self.root.metadict.lookup_typedef(self.property_entries[PID_FIXED_TYPE].ref)
 
     @property
     def size(self):
@@ -375,14 +393,17 @@
     def __new__(cls, root=None, name=None, type_auid=None, typedef=None):
         self = super(TypeDefVarArray, cls).__new__(cls, root, name, type_auid)
 
         if root:
             properties.add_typedef_weakref_property(self, PID_VAR_TYPE, typedef)
         return self
 
+    def copy(self, root=None):
+        return TypeDefVarArray(root or self.root, self.name, self.auid, self.element_typedef.auid)
+
     @property
     def store_format(self):
         if self.element_typedef.store_format == properties.SF_WEAK_OBJECT_REFERENCE:
             return properties.SF_WEAK_OBJECT_REFERENCE_VECTOR
         elif self.element_typedef.store_format == properties.SF_STRONG_OBJECT_REFERENCE:
             return properties.SF_STRONG_OBJECT_REFERENCE_VECTOR
 
@@ -452,14 +473,17 @@
 
     def __new__(cls, root=None, name=None, type_auid=None, typedef=None):
         self = super(TypeDefSet, cls).__new__(cls, root, name, type_auid)
         if root:
             properties.add_typedef_weakref_property(self, PID_SET_TYPE, typedef)
         return self
 
+    def copy(self, root=None):
+        return TypeDefSet(root or self.root, self.name, self.auid, self.element_typedef)
+
     @property
     def element_typedef(self):
         if PID_SET_TYPE in self.property_entries:
             return self.root.metadict.lookup_typedef(self.property_entries[PID_SET_TYPE].ref)
 
     @property
     def ref_classdef(self):
@@ -471,15 +495,15 @@
         if self.element_typedef.store_format == properties.SF_STRONG_OBJECT_REFERENCE:
             return properties.SF_STRONG_OBJECT_REFERENCE_SET
         elif self.element_typedef.store_format == properties.SF_WEAK_OBJECT_REFERENCE:
             return properties.SF_WEAK_OBJECT_REFERENCE_SET
         elif self.element_typedef.store_format == properties.SF_DATA:
             return properties.SF_DATA
         else:
-            raise AAFPropertyError("unkown store format: 0x%x" % self.element_typedef.store_format)
+            raise AAFPropertyError("unknown store format: 0x%x" % self.element_typedef.store_format)
 
     def decode(self, data):
 
         typedef = self.element_typedef
         byte_size = typedef.byte_size
         count = len(data) // byte_size
         start = 0
@@ -511,14 +535,17 @@
 
     def __new__(cls, root=None, name=None, type_auid=None, typedef=None):
         self = super(TypeDefString, cls).__new__(cls, root, name, type_auid)
         if root:
             properties.add_typedef_weakref_property(self, PID_STR_TYPE, typedef)
         return self
 
+    def copy(self, root=None):
+        return TypeDefString(root or self.root, self.name, self.auid, self.element_typedef.auid)
+
     @property
     def element_typedef(self):
         if PID_STR_TYPE in self.property_entries:
             return self.root.metadict.lookup_typedef(self.property_entries[PID_STR_TYPE].ref)
 
     def decode(self, data):
         return decode_utf16le(data)
@@ -560,14 +587,19 @@
 
             properties.add_utf16_array_property(self, PID_RECORD_NAMES, names)
             properties.add_typedef_weakref_vector_property(self, PID_RECORD_TYPES, 'MemberTypes', types)
 
         self._fields = None
         return self
 
+    def copy(self, root=None):
+        names = list(iter_utf16_array(self['MemberNames'].data))
+        types = [typedef.auid for typedef in self['MemberTypes'].value]
+        return TypeDefRecord(root or self.root, self.name, self.auid, zip(names, types))
+
     @property
     def member_names(self):
         return list(iter_utf16_array(self['MemberNames'].data))
 
     @property
     def member_types(self):
         return self['MemberTypes']
@@ -715,14 +747,17 @@
 
     def __new__(cls,  root=None, name=None, type_auid=None, typedef=None):
         self = super(TypeDefRename, cls).__new__(cls, root, name, type_auid)
         if root:
             properties.add_typedef_weakref_property(self, PID_RENAME_TYPE, typedef)
         return self
 
+    def copy(self, root=None):
+        return TypeDefRename(root or self.root, self.name, self.auid, self.renamed_typedef.auid)
+
     @property
     def renamed_typedef(self):
         if PID_RENAME_TYPE in self.property_entries:
             return self.root.metadict.lookup_typedef(self.property_entries[PID_RENAME_TYPE].ref)
 
     def decode(self, data):
         return self.renamed_typedef.decode(data)
@@ -762,14 +797,17 @@
                 names.append(name)
 
             properties.add_utf16_array_property(self, PID_EXTENUM_NAMES, names)
             properties.add_auid_array_propertry(self, PID_EXTENUM_VALUES, values)
 
         return self
 
+    def copy(self, root=None):
+        return TypeDefExtEnum(root or self.root, self.name, self.auid, self.elements)
+
     def register_element(self, element_name, element_auid):
 
         element_names = []
         element_values = []
         for val, name in self.elements.items():
             if val == element_auid:
                 return
@@ -887,14 +925,17 @@
 
             assert dynamic_pid
             # classdef
             properties.add_u8_property(self, dynamic_pid, size)
 
         return self
 
+    def copy(self, root=None):
+        return TypeDefGenericCharacter(root or self.root, self.name, self.auid, self.size)
+
     @property
     def size(self):
         classdef = self.root.metadict.lookup_classdef(self.class_id)
         dynamic_pid = None
         for pdef in classdef.all_propertydefs():
             if pdef.auid == AUID("0e040101-0101-0111-060e-2b3401010101"):
                 dynamic_pid = pdef.pid
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/utils.py` & `pyaaf2-1.7.0/src/aaf2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,25 +162,25 @@
         return num
     elif byte_order == 'big':
         length = len(data) - 1
         for i, byte in enumerate(data):
             num += byte << ((length-i) * 8)
         return num
     else:
-        raise ValueError('endianess must be "little" or "big"')
+        raise ValueError('endianness must be "little" or "big"')
 
 def bytes_from_int(num, length, byte_order='big'):
     if byte_order == 'little':
         v = bytearray((num >> (i * 8) & 0xff for i in range(length)))
         return bytes(v)
     elif byte_order == 'big':
         v = bytearray((num >> (length - 1 - i) * 8) & 0xff for i in range(length))
         return bytes(v)
     else:
-        raise ValueError('endianess must be "little" or "big"')
+        raise ValueError('endianness must be "little" or "big"')
 
 
 def squeeze_name(name, size):
     if len(name) <= size:
         return name
 
     half = size//2
```

### Comparing `pyaaf2-1.6.0.dev1/src/aaf2/video.py` & `pyaaf2-1.7.0/src/aaf2/video.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,53 +6,91 @@
     )
 from struct import unpack
 from . utils import int_from_bytes
 from io import BytesIO
 from .auid import AUID
 
 dnx_profiles = {
+# cid 1235
 'dnx_1080p_175x_23.97' : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 175,  "pix_fmt" : "yuv422p10", "frame_rate" : "24000/1001", },
-'dnx_1080p_365x_50'    : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 185,  "pix_fmt" : "yuv422p10", "frame_rate" : "25/1",       },
-'dnx_1080p_365x_60'    : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 365,  "pix_fmt" : "yuv422p10", "frame_rate" : "50/1",       },
-'dnx_1080p_440x_23.97' : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 440,  "pix_fmt" : "yuv422p10", "frame_rate" : "60000/1001", },
+'dnx_1080p_175x_24'    : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 175,  "pix_fmt" : "yuv422p10", "frame_rate" : "24/1",       },
+'dnx_1080p_185x_25'    : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 185,  "pix_fmt" : "yuv422p10", "frame_rate" : "25/1",       },
+'dnx_1080p_365x_50'    : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 365,  "pix_fmt" : "yuv422p10", "frame_rate" : "50/1",       },
+'dnx_1080p_440x_59.94' : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 440,  "pix_fmt" : "yuv422p10", "frame_rate" : "60000/1001", },
+'dnx_1080p_440x_60'    : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 440,  "pix_fmt" : "yuv422p10", "frame_rate" : "60/1",       },
+# cid 1237
 'dnx_1080p_115_23.97'  : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 115,  "pix_fmt" : "yuv422p",   "frame_rate" : "24000/1001", },
+'dnx_1080p_115_24'     : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 115,  "pix_fmt" : "yuv422p",   "frame_rate" : "24/1",       },
 'dnx_1080p_120_25'     : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 120,  "pix_fmt" : "yuv422p",   "frame_rate" : "25/1",       },
 'dnx_1080p_145_29.97'  : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 145,  "pix_fmt" : "yuv422p",   "frame_rate" : "30000/1001", },
 'dnx_1080p_240_50'     : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 240,  "pix_fmt" : "yuv422p",   "frame_rate" : "50/1",       },
 'dnx_1080p_290_59.94'  : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 290,  "pix_fmt" : "yuv422p",   "frame_rate" : "60000/1001", },
+'dnx_1080p_290_60'     : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 290,  "pix_fmt" : "yuv422p",   "frame_rate" : "60/1",       },
+# cid 1238
 'dnx_1080p_175_23.97'  : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 175,  "pix_fmt" : "yuv422p",   "frame_rate" : "24000/1001", },
+'dnx_1080p_175_24'     : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 175,  "pix_fmt" : "yuv422p",   "frame_rate" : "24/1",       },
 'dnx_1080p_185_25'     : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 185,  "pix_fmt" : "yuv422p",   "frame_rate" : "25/1",       },
 'dnx_1080p_220_29.97'  : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 220,  "pix_fmt" : "yuv422p",   "frame_rate" : "30000/1001", },
 'dnx_1080p_365_50'     : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 365,  "pix_fmt" : "yuv422p",   "frame_rate" : "50/1",       },
 'dnx_1080p_440_59.94'  : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 440,  "pix_fmt" : "yuv422p",   "frame_rate" : "60000/1001", },
+'dnx_1080p_440_60'     : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 440,  "pix_fmt" : "yuv422p",   "frame_rate" : "60/1",       },
+# cid 1241
 'dnx_1080i_185x_25'    : { "size" : (1920, 1080), 'interlaced' : True,  "bitrate" : 185,  "pix_fmt" : "yuv422p10", "frame_rate" : "25/1",       },
 'dnx_1080i_220x_29.97' : { "size" : (1920, 1080), 'interlaced' : True,  "bitrate" : 220,  "pix_fmt" : "yuv422p10", "frame_rate" : "30000/1001", },
+# cid 1242
 'dnx_1080i_120_25'     : { "size" : (1920, 1080), 'interlaced' : True,  "bitrate" : 120,  "pix_fmt" : "yuv422p",   "frame_rate" : "25/1",       },
 'dnx_1080i_145_29.97'  : { "size" : (1920, 1080), 'interlaced' : True,  "bitrate" : 145,  "pix_fmt" : "yuv422p",   "frame_rate" : "30000/1001", },
+# cid 1243
 'dnx_1080i_185_25'     : { "size" : (1920, 1080), 'interlaced' : True,  "bitrate" : 185,  "pix_fmt" : "yuv422p",   "frame_rate" : "25/1",       },
 'dnx_1080i_220_29.97'  : { "size" : (1920, 1080), 'interlaced' : True,  "bitrate" : 220,  "pix_fmt" : "yuv422p",   "frame_rate" : "30000/1001", },
+# cid 1244
+'dnx_1440x1080i_120_25'   : { "size" : (1440, 1080), 'interlaced' : True, "bitrate" : 120, "pix_fmt" : "yuv422p" ,"frame_rate" : "25/1",        },
+'dnx_1440x1080i_145_29.97': { "size" : (1440, 1080), 'interlaced' : True, "bitrate" : 145, "pix_fmt" : "yuv422p", "frame_rate" : "30000/1001",  },
+# cid 1250
 'dnx_720p_90x_23.97'   : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 90,   "pix_fmt" : "yuv422p10", "frame_rate" : "24000/1001", },
+'dnx_720p_90x_24'      : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 90,   "pix_fmt" : "yuv422p10", "frame_rate" : "24/1",       },
 'dnx_720p_90x_25'      : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 90,   "pix_fmt" : "yuv422p10", "frame_rate" : "25/1",       },
 'dnx_720p_180x_50'     : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 180,  "pix_fmt" : "yuv422p10", "frame_rate" : "50/1",       },
 'dnx_720p_220x_59.94'  : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 220,  "pix_fmt" : "yuv422p10", "frame_rate" : "60000/1001", },
+'dnx_720p_220x_60'     : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 220,  "pix_fmt" : "yuv422p10", "frame_rate" : "60/1",       },
+# cid 1251
 'dnx_720p_90_23.97'    : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 90,   "pix_fmt" : "yuv422p",   "frame_rate" : "24000/1001", },
+'dnx_720p_90_24'       : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 90,   "pix_fmt" : "yuv422p",   "frame_rate" : "24/1",       },
 'dnx_720p_90_25'       : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 90,   "pix_fmt" : "yuv422p",   "frame_rate" : "25/1",       },
 'dnx_720p_110_29.97'   : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 110,  "pix_fmt" : "yuv422p",   "frame_rate" : "30000/1001", },
 'dnx_720p_180_50'      : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 180,  "pix_fmt" : "yuv422p",   "frame_rate" : "50/1",       },
 'dnx_720p_220_59.94'   : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 220,  "pix_fmt" : "yuv422p",   "frame_rate" : "60000/1001", },
+'dnx_720p_220_60'      : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 220,  "pix_fmt" : "yuv422p",   "frame_rate" : "60/1",       },
+# cid 1252
 'dnx_720p_60_23.97'    : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 60,   "pix_fmt" : "yuv422p",   "frame_rate" : "24000/1001", },
+'dnx_720p_60_24'       : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 60,   "pix_fmt" : "yuv422p",   "frame_rate" : "24/1",       },
 'dnx_720p_60_25'       : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 60,   "pix_fmt" : "yuv422p",   "frame_rate" : "25/1",       },
 'dnx_720p_75_29.97'    : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 75,   "pix_fmt" : "yuv422p",   "frame_rate" : "30000/1001", },
 'dnx_720p_120_50'      : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 120,  "pix_fmt" : "yuv422p",   "frame_rate" : "50/1",       },
 'dnx_720p_145_59.94'   : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 145,  "pix_fmt" : "yuv422p",   "frame_rate" : "60000/1001", },
+'dnx_720p_145_60'      : { "size" : (1280, 720),  'interlaced' : False, "bitrate" : 145,  "pix_fmt" : "yuv422p",   "frame_rate" : "60/1",       },
+# cid 1253
 'dnx_1080p_36_23.97'   : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 36,   "pix_fmt" : "yuv422p",   "frame_rate" : "24000/1001", },
+'dnx_1080p_36_24'      : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 36,   "pix_fmt" : "yuv422p",   "frame_rate" : "24/1",       },
 'dnx_1080p_36_25'      : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 36,   "pix_fmt" : "yuv422p",   "frame_rate" : "25/1",       },
 'dnx_1080p_45_29.97'   : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 45,   "pix_fmt" : "yuv422p",   "frame_rate" : "30000/1001", },
 'dnx_1080p_75_50'      : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 75,   "pix_fmt" : "yuv422p",   "frame_rate" : "50/1",       },
 'dnx_1080p_90_59.94'   : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 90,   "pix_fmt" : "yuv422p",   "frame_rate" : "60000/1001", },
+'dnx_1080p_90_60'      : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 90,   "pix_fmt" : "yuv422p",   "frame_rate" : "60/1",       },
+# cid 1256, 1920x1080
+'dnx_1080p_350x_23.97' : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 350, "pix_fmt" : "yuv444p10",  "frame_rate" : "24000/1001", },
+'dnx_1080p_350x_24'    : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 350, "pix_fmt" : "yuv444p10",  "frame_rate" : "24/1",       },
+'dnx_1080p_390x_25'    : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 390, "pix_fmt" : "yuv444p10",  "frame_rate" : "25/1",       },
+'dnx_1080p_440x_29.97' : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 440, "pix_fmt" : "yuv444p10",  "frame_rate" : "30000/1001", },
+'dnx_1080p_730x_50'    : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 730, "pix_fmt" : "yuv444p10",  "frame_rate" : "50/1",       },
+'dnx_1080p_880x_59.94' : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 880, "pix_fmt" : "yuv444p10",  "frame_rate" : "60000/1001", },
+'dnx_1080p_880x_60'    : { "size" : (1920, 1080), 'interlaced' : False, "bitrate" : 880, "pix_fmt" : "yuv444p10",  "frame_rate" : "60/1",       },
+# cid 1258, 960x720 need to verify these
+# cid 1259, 1440x1080,
+# cid 1260, 1440x1080i
 'dnxhr_lb'             : { "size" : None,         'interlaced' : False, "bitrate" : None, "pix_fmt" : "yuv422p",   "frame_rate" : None, "video_profile": "dnxhr_lb", },
 'dnxhr_sq'             : { "size" : None,         'interlaced' : False, "bitrate" : None, "pix_fmt" : "yuv422p",   "frame_rate" : None, "video_profile": "dnxhr_sq", },
 'dnxhr_hq'             : { "size" : None,         'interlaced' : False, "bitrate" : None, "pix_fmt" : "yuv422p",   "frame_rate" : None, "video_profile": "dnxhr_hq", },
 'dnxhr_hqx'            : { "size" : None,         'interlaced' : False, "bitrate" : None, "pix_fmt" : "yuv422p",   "frame_rate" : None, "video_profile": "dnxhr_hqx",},
 }
 
 dnxhd_frame_sizes = {
@@ -129,15 +167,15 @@
 }
 
 def dnx_frame_size(cid, width=None, height=None):
     size = dnxhd_frame_sizes.get(cid, None)
     if size:
         return size
 
-    # DNxHR frame size caclulation
+    # DNxHR frame size calculation
     ratio = dnxhr_compression_ratio[cid]
     size = ((height + 15) // 16) * ((width + 15) // 16) * ratio[0] // ratio[1]
     size = (size + 2048) // 4096 * 4096;
 
     return max(size, 8192);
```

### Comparing `pyaaf2-1.6.0.dev1/src/pyaaf2.egg-info/PKG-INFO` & `pyaaf2-1.7.0/src/pyaaf2.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaaf2
-Version: 1.6.0.dev1
+Version: 1.7.0
 Summary: A python module for reading and writing advanced authoring format files
 Home-page: https://github.com/markreidvfx/pyaaf2
 Author: Mark Reid
 Author-email: mindmark@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/markreidvfx/pyaaf2
 Project-URL: Documentation, http://pyaaf.readthedocs.io
@@ -41,14 +41,15 @@
 
 Features
 --------
 
 - Read/Write AAF files
 - Modifying existing AAF files inplace
 - Embedding DNxHD/DNxHR/WAV media
+- Copying objects between files
 - Low level read/write Compound File Binary access
 - Lazy file reading
 - Zero dependencies, does not use AAF SDK
 
 Requirements
 ------------
```


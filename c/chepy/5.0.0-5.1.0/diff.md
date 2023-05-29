# Comparing `tmp/chepy-5.0.0.tar.gz` & `tmp/chepy-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/chepy-5.0.0.tar", last modified: Sat Aug 20 14:37:06 2022, max compression
+gzip compressed data, was "dist/chepy-5.1.0.tar", last modified: Mon May 29 02:32:02 2023, max compression
```

## Comparing `chepy-5.0.0.tar` & `chepy-5.1.0.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:06.000000 chepy-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-08-20 14:37:05.000000 chepy-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6438 2022-08-20 14:37:06.000000 chepy-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4821 2022-08-20 14:37:05.000000 chepy-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy/
--rw-r--r--   0 runner    (1001) docker     (121)     1526 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13262 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/__version__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5507 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    43894 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy/extras/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/extras/bruteforce.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/extras/characters.py
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/extras/combinatons.py
--rw-r--r--   0 runner    (1001) docker     (121)     4772 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/extras/crypto.py
--rw-r--r--   0 runner    (1001) docker     (121)     2168 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/extras/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy/modules/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4440 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/aritmeticlogic.py
--rw-r--r--   0 runner    (1001) docker     (121)     6033 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/codetidy.py
--rw-r--r--   0 runner    (1001) docker     (121)    10894 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/compression.py
--rw-r--r--   0 runner    (1001) docker     (121)    40106 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/dataformat.py
--rw-r--r--   0 runner    (1001) docker     (121)     1547 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/datetimemodule.py
--rw-r--r--   0 runner    (1001) docker     (121)    35766 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/encryptionencoding.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14837 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/extractors.py
--rw-r--r--   0 runner    (1001) docker     (121)    17173 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/hashing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy/modules/internal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8248 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/internal/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2735 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/internal/colors.py
--rw-r--r--   0 runner    (1001) docker     (121)    10536 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     2843 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/language.py
--rw-r--r--   0 runner    (1001) docker     (121)     1964 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/links.py
--rw-r--r--   0 runner    (1001) docker     (121)     7069 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/networking.py
--rw-r--r--   0 runner    (1001) docker     (121)      752 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/other.py
--rw-r--r--   0 runner    (1001) docker     (121)     8806 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/publickey.py
--rw-r--r--   0 runner    (1001) docker     (121)     3459 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/search.py
--rw-r--r--   0 runner    (1001) docker     (121)    21018 2022-08-20 14:37:05.000000 chepy-5.0.0/chepy/modules/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6438 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-08-20 14:37:06.000000 chepy-5.0.0/chepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-08-20 14:37:05.000000 chepy-5.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-20 14:37:06.000000 chepy-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1592 2022-08-20 14:37:05.000000 chepy-5.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:06.000000 chepy-5.0.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:06.000000 chepy-5.0.0/tests/test_extras/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-20 14:37:05.000000 chepy-5.0.0/tests/test_extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-08-20 14:37:05.000000 chepy-5.0.0/tests/test_extras/test_bruteforce.py
--rw-r--r--   0 runner    (1001) docker     (121)     1032 2022-08-20 14:37:05.000000 chepy-5.0.0/tests/test_extras/test_characters.py
--rw-r--r--   0 runner    (1001) docker     (121)      389 2022-08-20 14:37:05.000000 chepy-5.0.0/tests/test_extras/test_combinations.py
--rw-r--r--   0 runner    (1001) docker     (121)      400 2022-08-20 14:37:05.000000 chepy-5.0.0/tests/test_extras/test_crypto_extras.py
--rw-r--r--   0 runner    (1001) docker     (121)      410 2022-08-20 14:37:05.000000 chepy-5.0.0/tests/test_extras/test_misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:02.000000 chepy-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-29 02:32:01.000000 chepy-5.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-05-29 02:32:02.000000 chepy-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-29 02:32:01.000000 chepy-5.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:02.000000 chepy-5.1.0/chepy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13262 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43894 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:02.000000 chepy-5.1.0/chepy/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/extras/bruteforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/extras/characters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/extras/combinatons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/extras/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/extras/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:02.000000 chepy-5.1.0/chepy/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/aritmeticlogic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6033 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/codetidy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10894 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41514 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/dataformat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1547 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/datetimemodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38731 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/encryptionencoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14837 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/extractors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17173 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/hashing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:02.000000 chepy-5.1.0/chepy/modules/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8248 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/internal/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/internal/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10536 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/other.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8806 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/publickey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21018 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy/modules/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:02.000000 chepy-5.1.0/chepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-29 02:32:02.000000 chepy-5.1.0/chepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 02:32:01.000000 chepy-5.1.0/chepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-29 02:32:01.000000 chepy-5.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-29 02:32:02.000000 chepy-5.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-29 02:32:01.000000 chepy-5.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:02.000000 chepy-5.1.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:02.000000 chepy-5.1.0/tests/test_extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 02:32:01.000000 chepy-5.1.0/tests/test_extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-29 02:32:01.000000 chepy-5.1.0/tests/test_extras/test_bruteforce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-29 02:32:01.000000 chepy-5.1.0/tests/test_extras/test_characters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-29 02:32:01.000000 chepy-5.1.0/tests/test_extras/test_combinations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-29 02:32:01.000000 chepy-5.1.0/tests/test_extras/test_crypto_extras.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-05-29 02:32:01.000000 chepy-5.1.0/tests/test_extras/test_misc.py
```

### Comparing `chepy-5.0.0/PKG-INFO` & `chepy-5.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chepy
-Version: 5.0.0
+Version: 5.1.0
 Summary: UNKNOWN
 Home-page: https://github.com/securisec/chepy
 Author: Hapsida @securisec
 License: GPL
 Project-URL: Documentation, https://chepy.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/securisec/chepy
 Description: <p align="center">
```

### Comparing `chepy-5.0.0/README.md` & `chepy-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/__init__.py` & `chepy-5.1.0/chepy/__init__.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/__main__.py` & `chepy-5.1.0/chepy/__main__.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/config.py` & `chepy-5.1.0/chepy/config.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/core.py` & `chepy-5.1.0/chepy/core.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/extras/bruteforce.py` & `chepy-5.1.0/chepy/extras/bruteforce.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/extras/characters.py` & `chepy-5.1.0/chepy/extras/characters.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/extras/combinatons.py` & `chepy-5.1.0/chepy/extras/combinatons.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/extras/crypto.py` & `chepy-5.1.0/chepy/extras/crypto.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/extras/misc.py` & `chepy-5.1.0/chepy/extras/misc.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/aritmeticlogic.py` & `chepy-5.1.0/chepy/modules/aritmeticlogic.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/codetidy.py` & `chepy-5.1.0/chepy/modules/codetidy.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/compression.py` & `chepy-5.1.0/chepy/modules/compression.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/dataformat.py` & `chepy-5.1.0/chepy/modules/dataformat.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,19 @@
             Chepy: The Chepy object.
 
         Examples:
             >>> Chepy(["a", "b", "c"]).list_to_str(",").o
             "a,b,c"
         """
         assert isinstance(self.state, list), "Data in state not a list"
+        # convert the list of items in state appropiately
+        if isinstance(join_by, str):
+            self.state = [str(x) for x in self.state]
+        elif isinstance(join_by, bytes):
+            self.state = [bytes(x) for x in self.state]
         self.state = join_by.join(self.state)
         return self
 
     @ChepyDecorators.call_stack
     def str_list_to_list(self) -> DataFormatT:
         """Convert a string list to a list
 
@@ -142,14 +147,34 @@
             '{"some":"data","a":["list",1,true]}'
         """
         assert isinstance(self.state, dict), "Not a dict object"
         self.state = json.dumps(self.state)
         return self
 
     @ChepyDecorators.call_stack
+    def dict_get_items(self, *keys) -> DataFormatT:
+        """Get items from a dict
+
+        Returns:
+            Chepy: The Chepy object.
+
+        Examples:
+            >>> o = Chepy({"a": 1, "b": 2}).dict_get_items("a", "b", "c").o
+            [1, 2]
+        """
+        assert isinstance(self.state, dict), "Not a dict object"
+        assert len(keys) > 0, "No keys provided"
+        o = list()
+        for k in keys:
+            if self.state.get(k):
+                o.append(self.state.get(k))
+        self.state = o
+        return self
+
+    @ChepyDecorators.call_stack
     def yaml_to_json(self) -> DataFormatT:
         """Convert yaml to a json string
 
         Returns:
             Chepy: The Chepy object.
         """
         self.state = json.dumps(yaml.safe_load(self.state))
@@ -1155,15 +1180,15 @@
         Returns:
             Chepy: The Chepy object.
         """
         self.state = self._convert_to_str().strip()
         return self
 
     @ChepyDecorators.call_stack
-    def convert_to_nato(self, join_by: str = " ") -> DataFormatT:
+    def to_nato(self, join_by: str = " ") -> DataFormatT:
         """Convert string to NATO phonetic format.
 
         Example: abc = Alpha Bravo Charlie
 
         Args:
             join_by (str, optional): [description]. Defaults to " ".
 
@@ -1178,14 +1203,30 @@
                 hold.append(nato_chars[d.upper()])
             else:
                 hold.append(d)
         self.state = join_by.join(hold)
         return self
 
     @ChepyDecorators.call_stack
+    def from_nato(self, delimiter: str = " ", join_by: str = "") -> DataFormatT:
+        """Translate NATO phoentic to words
+
+        Args:
+            delimiter (str, optional): Delimiter to split on. Defaults to ' '.
+            join_by (str, optional): Join result by. Defaults to ''.
+
+        Returns:
+            Chepy: The Chepy object
+        """
+        data = self._convert_to_str().split(delimiter)
+        d = {v: k for k, v in Encoding.NATO_CONSTANTS_DICT.items()}
+        self.state = join_by.join([d.get(p, "") for p in data])
+        return self
+
+    @ChepyDecorators.call_stack
     def swap_strings(self, by: int) -> DataFormatT:
         """Swap characters in string
 
         Args:
             by (int): Number of bytes to swap
 
         Returns:
```

### Comparing `chepy-5.0.0/chepy/modules/datetimemodule.py` & `chepy-5.1.0/chepy/modules/datetimemodule.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/encryptionencoding.py` & `chepy-5.1.0/chepy/modules/encryptionencoding.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import base64
 import binascii
 import codecs
 import itertools
 import string
-from typing import Literal, TypeVar
+from typing import Literal, TypeVar, Dict
 
 import lazy_import
 
 jwt = lazy_import.lazy_module("jwt")
 import pathlib
 
 import regex as re
 import json
 
 AES = lazy_import.lazy_module("Crypto.Cipher.AES")
 ARC4 = lazy_import.lazy_module("Crypto.Cipher.ARC4")
 DES = lazy_import.lazy_module("Crypto.Cipher.DES")
+ChaCha20 = lazy_import.lazy_module("Crypto.Cipher.ChaCha20")
 DES3 = lazy_import.lazy_module("Crypto.Cipher.DES3")
 RSA = lazy_import.lazy_module("Crypto.PublicKey.RSA")
 Hash = lazy_import.lazy_module("Crypto.Hash")
 PKCS1_15 = lazy_import.lazy_module("Crypto.Signature.pkcs1_15")
 PKCS1_OAEP = lazy_import.lazy_module("Crypto.Cipher.PKCS1_OAEP")
 Blowfish = lazy_import.lazy_module("Crypto.Cipher.Blowfish")
 Padding = lazy_import.lazy_module("Crypto.Util.Padding")
@@ -494,14 +495,66 @@
             return self
         elif mode == "OFB":
             cipher = DES.new(key, mode=DES.MODE_OFB, iv=iv)
             self.state = cipher.decrypt(self._convert_to_bytes())
             return self
 
     @ChepyDecorators.call_stack
+    def chacha_encrypt(
+        self,
+        key: str,
+        nonce: str = "0000000000000000",
+        key_format: str = "hex",
+        nonce_format: str = "hex",
+    ) -> EncryptionEncodingT:
+        """Encrypt raw state with ChaCha 20 rounds
+
+        Args:
+            key (str): Required. The secret key
+            nonce (str, optional): Nonce. Defaults to '0000000000000000'.
+            key_format (str, optional): Format of key. Defaults to 'hex'.
+            nonce_format (str, optional): Format of nonce. Defaults to 'hex'.
+
+        Returns:
+            Chepy: The Chepy object.
+        """
+
+        key, nonce = self._convert_key(key, nonce, key_format, nonce_format)
+
+        cipher = ChaCha20.new(key=key, nonce=nonce)
+        self.state = cipher.encrypt(self._convert_to_bytes())
+        return self
+
+    @ChepyDecorators.call_stack
+    def chacha_decrypt(
+        self,
+        key: str,
+        nonce: str = "0000000000000000",
+        key_format: str = "hex",
+        nonce_format: str = "hex",
+    ) -> EncryptionEncodingT:
+        """Decrypt raw state encrypted with ChaCha 20 rounds.
+
+        Args:
+            key (str): Required. The secret key
+            nonce (str, optional): nonce for certain modes only. Defaults to '0000000000000000'.
+            key_format (str, optional): Format of key. Defaults to 'hex'.
+            nonce_format (str, optional): Format of nonce. Defaults to 'hex'.
+
+        Returns:
+            Chepy: The Chepy object.
+        """
+
+        key, nonce = self._convert_key(key, nonce, key_format, nonce_format)
+
+        cipher = ChaCha20.new(key=key, nonce=nonce)
+        self.state = cipher.decrypt(self._convert_to_bytes())
+        return self
+
+    @ChepyDecorators.call_stack
     def triple_des_encrypt(
         self,
         key: str,
         iv: str = "0000000000000000",
         mode: str = "CBC",
         key_format: str = "hex",
         iv_format: str = "hex",
@@ -599,15 +652,16 @@
         self,
         key: str,
         iv: str = "00000000000000000000000000000000",
         mode: str = "CBC",
         key_format: str = "hex",
         iv_format: str = "hex",
     ) -> EncryptionEncodingT:
-        """Encrypt raw state with AES
+        """Encrypt raw state with AES.
+        CFB mode reflects Cyberchef and not native python behaviour.
 
         Args:
             key (str): Required. The secret key
             iv (str, optional): IV for certain modes only.
                 Defaults to '00000000000000000000000000000000'.
             mode (str, optional): Encryption mode. Defaults to 'CBC'.
             key_format (str, optional): Format of key. Defaults to 'hex'.
@@ -617,22 +671,26 @@
             Chepy: The Chepy object.
 
         Examples:
             >>> Chepy("some data").aes_encrypt("secret password!", mode="ECB").o
             b"5fb8c186394fc399849b89d3b6605fa3"
         """
 
-        assert mode in ["CBC", "OFB", "CTR", "ECB", "GCM"], "Not a valid mode."
+        assert mode in ["CBC", "CFB", "OFB", "CTR", "ECB", "GCM"], "Not a valid mode."
 
         key, iv = self._convert_key(key, iv, key_format, iv_format)
 
         if mode == "CBC":
             cipher = AES.new(key, mode=AES.MODE_CBC, iv=iv)
             self.state = cipher.encrypt(Padding.pad(self._convert_to_bytes(), 16))
             return self
+        elif mode == "CFB":
+            cipher = AES.new(key, mode=AES.MODE_CFB, iv=iv, segment_size=128)
+            self.state = cipher.encrypt(self._convert_to_bytes())
+            return self
         elif mode == "ECB":
             cipher = AES.new(key, mode=AES.MODE_ECB)
             self.state = cipher.encrypt(Padding.pad(self._convert_to_bytes(), 16))
             return self
         elif mode == "CTR":
             cipher = AES.new(key, mode=AES.MODE_CTR, nonce=b"")
             self.state = cipher.encrypt(self._convert_to_bytes())
@@ -656,14 +714,15 @@
         key: str,
         iv: str = "00000000000000000000000000000000",
         mode: str = "CBC",
         key_format: str = "hex",
         iv_format: str = "hex",
     ) -> EncryptionEncodingT:
         """Decrypt raw state encrypted with DES.
+        CFB mode reflects Cyberchef and not native python behaviour.
 
         Args:
             key (str): Required. The secret key
             iv (str, optional): IV for certain modes only.
                 Defaults to '00000000000000000000000000000000'.
             mode (str, optional): Encryption mode. Defaults to 'CBC'.
             hex_key (bool, optional): If the secret key is a hex string. Defaults to False.
@@ -676,22 +735,26 @@
             >>> c = Chepy("5fb8c186394fc399849b89d3b6605fa3")
             >>> c.hex_to_str()
             >>> c.aes_decrypt("7365637265742070617373776f726421")
             >>> c.o
             b"some data"
         """
 
-        assert mode in ["CBC", "OFB", "CTR", "ECB", "GCM"], "Not a valid mode."
+        assert mode in ["CBC", "CFB", "OFB", "CTR", "ECB", "GCM"], "Not a valid mode."
 
         key, iv = self._convert_key(key, iv, key_format, iv_format)
 
         if mode == "CBC":
             cipher = AES.new(key, mode=AES.MODE_CBC, iv=iv)
             self.state = Padding.unpad(cipher.decrypt(self._convert_to_bytes()), 16)
             return self
+        if mode == "CFB":
+            cipher = AES.new(key, mode=AES.MODE_CFB, iv=iv, segment_size=128)
+            self.state = cipher.decrypt(self._convert_to_bytes())
+            return self
         elif mode == "ECB":
             cipher = AES.new(key, mode=AES.MODE_ECB)
             self.state = Padding.unpad(cipher.decrypt(self._convert_to_bytes()), 16)
             return self
         elif mode == "CTR":
             cipher = AES.new(key, mode=AES.MODE_CTR, nonce=b"")
             self.state = cipher.decrypt(self._convert_to_bytes())
@@ -1038,7 +1101,26 @@
         """
         with open(str(self._abs_path(public_key_path)), "r") as f:
             pub_key = f.read()
             key = RSA.importKey(pub_key)
             h = Hash.SHA256.new(self._convert_to_bytes())
             self.state = PKCS1_15.new(key).verify(h, signature)
             return self
+
+    @ChepyDecorators.call_stack
+    def monoalphabetic_substitution(
+        self, mapping: Dict[str, str] = {}
+    ) -> EncryptionEncodingT:
+        """Monoalphabetic substitution. Re-map characters
+
+        Args:
+            mapping (Dict[str, str], optional): Mapping of characters where key is the character to map and value is the new character to replace with. Defaults to {}.
+
+        Returns:
+            Chepy: The Chepy object
+        """
+        hold = ""
+        cipher = self._convert_to_str()
+        for c in cipher:
+            hold += mapping.get(c.lower(), c)
+        self.state = hold
+        return self
```

### Comparing `chepy-5.0.0/chepy/modules/extractors.py` & `chepy-5.1.0/chepy/modules/extractors.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/hashing.py` & `chepy-5.1.0/chepy/modules/hashing.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/internal/cli.py` & `chepy-5.1.0/chepy/modules/internal/cli.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/internal/colors.py` & `chepy-5.1.0/chepy/modules/internal/colors.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/internal/constants.py` & `chepy-5.1.0/chepy/modules/internal/constants.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/language.py` & `chepy-5.1.0/chepy/modules/language.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,29 +34,29 @@
         Returns:
             Chepy: The Chepy object.
         """
         self.state = [e.get("emoji") for e in emoji.emoji_list(self._convert_to_str())]
         return self
 
     @ChepyDecorators.call_stack
-    def encode(self, encoding: str, errors: str='backslashreplace') -> LanguageT:
+    def encode(self, encoding: str, errors: str = "backslashreplace") -> LanguageT:
         """Encode the string using the given encoding.
 
         Args:
             encoding (str): Encoding to use.
             errors (str, optional): How to handle errors when encoding. Defaults to 'backslashreplace'.
 
         Returns:
             Chepy: The Chepy object.
         """
         self.state = self._convert_to_str().encode(encoding, errors=errors)
         return self
 
     @ChepyDecorators.call_stack
-    def decode(self, encoding: str, errors: str='backslashreplace') -> LanguageT:
+    def decode(self, encoding: str, errors: str = "backslashreplace") -> LanguageT:
         """Decode the string using the given encoding.
 
         Args:
             encoding (str): Encoding to use.
             errors (str, optional): How to handle errors when decoding. Defaults to 'backslashreplace'.
 
         Returns:
@@ -84,7 +84,17 @@
         Returns:
             Chepy: The Chepy object.
         """
         self.state = self._convert_to_bytes().decode(
             "unicode-escape", errors="backslashreplace"
         )
         return self
+
+    @ChepyDecorators.call_stack
+    def str_to_unicode(self) -> LanguageT:
+        """Convert unicode to str
+
+        Returns:
+            Chepy: The Chepy object.
+        """
+        self.state = self._convert_to_str().encode("unicode_escape")
+        return self
```

### Comparing `chepy-5.0.0/chepy/modules/links.py` & `chepy-5.1.0/chepy/modules/links.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/networking.py` & `chepy-5.1.0/chepy/modules/networking.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/other.py` & `chepy-5.1.0/chepy/modules/other.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/publickey.py` & `chepy-5.1.0/chepy/modules/publickey.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/search.py` & `chepy-5.1.0/chepy/modules/search.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy/modules/utils.py` & `chepy-5.1.0/chepy/modules/utils.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/chepy.egg-info/PKG-INFO` & `chepy-5.1.0/chepy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chepy
-Version: 5.0.0
+Version: 5.1.0
 Summary: UNKNOWN
 Home-page: https://github.com/securisec/chepy
 Author: Hapsida @securisec
 License: GPL
 Project-URL: Documentation, https://chepy.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/securisec/chepy
 Description: <p align="center">
```

### Comparing `chepy-5.0.0/chepy.egg-info/SOURCES.txt` & `chepy-5.1.0/chepy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/setup.py` & `chepy-5.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `chepy-5.0.0/tests/test_extras/test_characters.py` & `chepy-5.1.0/tests/test_extras/test_characters.py`

 * *Files identical despite different names*


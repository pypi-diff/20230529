# Comparing `tmp/random_names-0.1.0.tar.gz` & `tmp/random_names-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "random_names-0.1.0.tar", last modified: Sun Jan 24 14:46:41 2021, max compression
+gzip compressed data, was "random_names-0.2.0.tar", max compression
```

## Comparing `random_names-0.1.0.tar` & `random_names-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,23 @@
--rw-r--r--   0        0        0     1092 2021-01-23 22:56:57.627004 random_names-0.1.0/LICENSE
--rw-r--r--   0        0        0     2797 2021-01-24 14:46:28.101399 random_names-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2021-01-03 14:50:28.076000 random_names-0.1.0/random_names/__init__.py
--rw-r--r--   0        0        0    87477 2021-01-17 20:05:32.569000 random_names-0.1.0/random_names/clean_ten_k.txt
--rw-r--r--   0        0        0    50605 2021-01-24 14:13:19.515167 random_names-0.1.0/random_names/docker_style.py
--rw-r--r--   0        0        0        0 2021-01-04 05:33:29.458000 random_names-0.1.0/random_names/etl/__init__.py
--rw-r--r--   0        0        0     9414 2021-01-18 12:10:46.895000 random_names-0.1.0/random_names/etl/bad_words.txt
--rw-r--r--   0        0        0    87477 2021-01-17 20:05:32.586000 random_names-0.1.0/random_names/etl/clean_ten_k.txt
--rw-r--r--   0        0        0     9896 2021-01-04 05:08:11.643000 random_names-0.1.0/random_names/etl/most-common-nouns-english.csv
--rw-r--r--   0        0        0   133558 2021-01-04 05:22:31.030000 random_names-0.1.0/random_names/etl/people_names.txt
--rw-r--r--   0        0        0      842 2021-01-24 14:21:56.024922 random_names-0.1.0/random_names/etl/README.md
--rw-r--r--   0        0        0     3146 2021-01-17 19:19:49.452000 random_names-0.1.0/random_names/etl/reform_words.py
--rw-r--r--   0        0        0    22224 2021-01-04 04:59:58.024000 random_names-0.1.0/random_names/etl/three_k.txt
--rw-r--r--   0        0        0       73 2021-01-24 03:28:27.521686 random_names-0.1.0/random_names/etl/word_harvestor.py
--rw-r--r--   0        0        0    75880 2020-12-25 13:29:48.925000 random_names-0.1.0/random_names/etl/wordlist.10000.txt
--rw-r--r--   0        0        0     2510 2021-01-24 14:13:19.333168 random_names-0.1.0/random_names/make_name.py
--rw-r--r--   0        0        0       14 2021-01-24 00:55:01.258850 random_names-0.1.0/random_names/settings.py
--rw-r--r--   0        0        0        0 2020-12-29 03:42:11.682000 random_names-0.1.0/random_names/utils/__init__.py
--rw-r--r--   0        0        0      410 2020-12-29 03:44:32.762000 random_names-0.1.0/random_names/utils/files_utils.py
--rw-r--r--   0        0        0     2712 2020-08-17 12:16:27.385000 random_names-0.1.0/random_names/utils/guards.py
--rw-r--r--   0        0        0      194 2021-01-24 00:55:01.228851 random_names-0.1.0/random_names/utils/user_trace.py
--rw-r--r--   0        0        0     2759 2021-01-24 04:27:55.075269 random_names-0.1.0/README.md
--rw-r--r--   0        0        0     3497 2021-01-24 14:46:42.125681 random_names-0.1.0/setup.py
--rw-r--r--   0        0        0     3967 2021-01-24 14:46:42.125681 random_names-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-28 22:17:29.024946 random_names-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2759 2023-05-28 22:17:29.024946 random_names-0.2.0/README.md
+-rw-r--r--   0        0        0     2872 2023-05-28 22:17:29.024946 random_names-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-28 22:17:29.024946 random_names-0.2.0/random_names/__init__.py
+-rw-r--r--   0        0        0    77478 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/clean_ten_k.txt
+-rw-r--r--   0        0        0    50605 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/docker_style.py
+-rw-r--r--   0        0        0      842 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/etl/README.md
+-rw-r--r--   0        0        0        0 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/etl/__init__.py
+-rw-r--r--   0        0        0     9414 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/etl/bad_words.txt
+-rw-r--r--   0        0        0    77478 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/etl/clean_ten_k.txt
+-rw-r--r--   0        0        0     9896 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/etl/most-common-nouns-english.csv
+-rw-r--r--   0        0        0   133558 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/etl/people_names.txt
+-rw-r--r--   0        0        0     3218 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/etl/reform_words.py
+-rw-r--r--   0        0        0    22224 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/etl/three_k.txt
+-rw-r--r--   0        0        0       73 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/etl/word_harvestor.py
+-rw-r--r--   0        0        0    75880 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/etl/wordlist.10000.txt
+-rw-r--r--   0        0        0     2527 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/make_name.py
+-rw-r--r--   0        0        0       37 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/settings.py
+-rw-r--r--   0        0        0        0 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/utils/__init__.py
+-rw-r--r--   0        0        0      410 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/utils/files_utils.py
+-rw-r--r--   0        0        0     2618 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/utils/guards.py
+-rw-r--r--   0        0        0      194 2023-05-28 22:17:29.028946 random_names-0.2.0/random_names/utils/user_trace.py
+-rw-r--r--   0        0        0     4069 1970-01-01 00:00:00.000000 random_names-0.2.0/PKG-INFO
```

### Comparing `random_names-0.1.0/LICENSE` & `random_names-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2021 Matthew Martin
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2021 Matthew Martin
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `random_names-0.1.0/pyproject.toml` & `random_names-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 [tool.poetry]
 name = "random_names"
-version = "0.1.0"
+version = "0.2.0"
 description = "Convert int to random name, like tree_dance and convert it back to same int."
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["mneumonic", "pseudorandom", "name-generator"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
 ]
 include = [
     "random_names/**/*.py",
     "random_names/**/*.md",
     "random_names/**/*.txt",
     "random_names/**/*.html",
     "random_names/**/*.jinja",
@@ -45,15 +47,15 @@
 [tool.poetry.dev-dependencies]
 pytest = "*"
 pytest-cov = ">=2.10.1"
 pytest-timeout = "*"
 pytest-xdist = ">=2.1.0"
 pip-check = "==2.6"
 checksumdir = "==1.1.7"
-dodgy = "==0.2.1"
+
 gitchangelog = "==3.0.4"
 liccheck = "==0.4.3"
 psutil = "==5.6.7"
 pebble = "==4.5.0"
 gitpython = "*"
 sshtunnel = "*"
 ifaddr = "*"
```

### Comparing `random_names-0.1.0/random_names/docker_style.py` & `random_names-0.2.0/random_names/docker_style.py`

 * *Files identical despite different names*

### Comparing `random_names-0.1.0/random_names/etl/bad_words.txt` & `random_names-0.2.0/random_names/etl/bad_words.txt`

 * *Files identical despite different names*

### Comparing `random_names-0.1.0/random_names/etl/most-common-nouns-english.csv` & `random_names-0.2.0/random_names/etl/most-common-nouns-english.csv`

 * *Files identical despite different names*

### Comparing `random_names-0.1.0/random_names/etl/people_names.txt` & `random_names-0.2.0/random_names/etl/people_names.txt`

 * *Files identical despite different names*

### Comparing `random_names-0.1.0/random_names/etl/README.md` & `random_names-0.2.0/random_names/etl/README.md`

 * *Files identical despite different names*

### Comparing `random_names-0.1.0/random_names/etl/reform_words.py` & `random_names-0.2.0/random_names/etl/reform_words.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 Generate a list of 10,000 good words.
 """
 
 
 def run() -> None:
     """Combine lots of words, remove lots of bad words"""
     # Typo: In word 'acer'
-    with open("bad_words.txt") as bad:
+    with open("bad_words.txt", encoding="utf-8") as bad:
         bad_words = [
             _.strip(" ,*.") for _ in bad.read().split("\n") if not _.startswith("#")
         ]
 
-    with open("wordlist.10000.txt") as long_file:
+    with open("wordlist.10000.txt", encoding="utf-8") as long_file:
         ten_k = [
             _.strip(" ,*.")
             for _ in long_file.read().split("\n")
             if not _.startswith("#")
         ]
         for word in ten_k:
             if len(word) == 1:
@@ -44,15 +44,15 @@
                 bad_words.append(word)
             if word.upper() == word:
                 # accronyms
                 bad_words.append(word)
             if len([letter for letter in word if letter in "aeiou"]) == 0:
                 bad_words.append(word)
 
-    with open("most-common-nouns-english.csv") as most_common_file:
+    with open("most-common-nouns-english.csv", encoding="utf-8") as most_common_file:
         most_common = [
             _.strip(" ,*.")
             for _ in most_common_file.read().split("\n")
             if not _.startswith("#")
         ]
         for word in most_common:
             if len(word) == 1:
@@ -72,15 +72,15 @@
         if "," in word:
             parts = word.split(",")
             first = parts[0]
             most_common_simpler.append(first)
         else:
             most_common_simpler.append(word)
 
-    with open("people_names.txt") as people_file:
+    with open("people_names.txt", encoding="utf-8") as people_file:
         people = [
             _.strip(" ,*.")
             for _ in people_file.read().split("\n")
             if not _.startswith("#")
         ]
         people = people[:1000]
     dedupe = {
```

### Comparing `random_names-0.1.0/random_names/etl/three_k.txt` & `random_names-0.2.0/random_names/etl/three_k.txt`

 * *Files identical despite different names*

### Comparing `random_names-0.1.0/random_names/etl/wordlist.10000.txt` & `random_names-0.2.0/random_names/etl/wordlist.10000.txt`

 * *Files identical despite different names*

### Comparing `random_names-0.1.0/random_names/make_name.py` & `random_names-0.2.0/random_names/make_name.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,25 +18,25 @@
     if NAMES:
         return
 
     # words_path = find_file("most-common-nouns-english.csv",__file__)
     # source: https://www.mit.edu/~ecprice/wordlist.10000
     # See ETL for what it took to get a clean file.
     words_path = find_file(FILE, __file__)
-    with open(words_path) as name_file:
+    with open(words_path, encoding="utf-8") as name_file:
         NAMES.extend(name.strip() for name in name_file.readlines())
 
     if len(NAMES) != 10000:
         raise TypeError(f"Init failed, didn't find 10,000 words, got {len(NAMES)}")
 
 
 # TODO: replace with a SO sourced post.
 # https://www.geeksforgeeks.org/break-list-chunks-size-n-python/
 def divide_chunks(value: List[Any], number: int) -> Any:
-    """ looping till length l"""
+    """looping till length l"""
     for index in range(0, len(value), number):
         yield value[index : index + number]
 
 
 def number_from_name(name: str) -> int:
     """Convert name into number"""
     initialize()
```

### Comparing `random_names-0.1.0/random_names/utils/guards.py` & `random_names-0.2.0/random_names/utils/guards.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,94 +1,94 @@
-"""
-Utility functions to help with code coverage.
-
-Imagine:
-
-def foo(bar):
-    if bar is None:
-        raise Exception()
-
-Hitting the guard requires an extra unit test and provides little
-value to get 100% coverage. (And to hit 90% coverage, you need to
-have 100% coverage on most files)
-"""
-import logging
-from typing import Any, Dict
-
-LOGGER = logging.getLogger(__name__)
-
-
-def must_not_be_none(value: Any, message: str = "Value must not be none") -> None:
-    """
-    Raise exception if value is None
-    """
-    if value is None:
-        LOGGER.error(f"Can't be none, but got {value}")
-        raise TypeError(message)
-
-
-def must_not_be_truthy(value: bool, message: str = "Value must not be truthy") -> None:
-    """
-    Guard to assert truthiness & make it easier to get unit test coverage.
-    """
-    if value:
-        LOGGER.error(f"Can't be truthy, but got {value}")
-        raise TypeError(message)
-
-
-def must_be_truthy(value: Any, message: str = "Value must not be truthy") -> None:
-    """
-    Guard to assert truthiness & make it easier to get unit test coverage.
-    """
-    if not value:
-        LOGGER.error(f"Must be truthy, but got {value}")
-        raise TypeError(message)
-
-
-def must_not_be_falsy(value: Any, message: str = "Value must not be falsy") -> None:
-    """
-    Raise exception if value is falsy (i.e. False, "", None, [], etc)
-    """
-    if not value:
-        LOGGER.error(f"Must not be falsy, but got {value}")
-        raise TypeError(message)
-
-
-def must_be_falsy(value: Any, message: str = "Value must not be falsy") -> None:
-    """
-    Raise exception if value is not falsy (i.e. False, "", None, [], etc)
-    """
-    if value:
-        LOGGER.error(f"Must be falsy, but got {value}")
-        raise TypeError(message)
-
-
-def must_not_already_be_in_dictionary(
-    key: Any,
-    dictionary: Dict[Any, Any],
-    message: str = "Key already in dictionary",
-    warn_only: bool = False,
-) -> None:
-    """Assert we aren't about to insert a key twice to a dict"""
-    if key in dictionary:
-        if warn_only:
-            print(
-                f"{key} is already in dictionary where it has "
-                f"a value of {dictionary[key]}"
-            )
-        else:
-            raise TypeError(message)
-
-
-def assert_is_number(value: str) -> None:
-    """
-    Raise error if there is a value and the value is not a number
-    """
-    if value is None:
-        # Why did I do this?
-        return
-    # pylint: disable=broad-except
-    # noinspection PyBroadException
-    try:
-        _ = int(value)
-    except BaseException:
-        LOGGER.error(f"Expected numerical id, got {value}")
+"""
+Utility functions to help with code coverage.
+
+Imagine:
+
+def foo(bar):
+    if bar is None:
+        raise Exception()
+
+Hitting the guard requires an extra unit test and provides little
+value to get 100% coverage. (And to hit 90% coverage, you need to
+have 100% coverage on most files)
+"""
+import logging
+from typing import Any, Dict
+
+LOGGER = logging.getLogger(__name__)
+
+
+def must_not_be_none(value: Any, message: str = "Value must not be none") -> None:
+    """
+    Raise exception if value is None
+    """
+    if value is None:
+        LOGGER.error(f"Can't be none, but got {value}")
+        raise TypeError(message)
+
+
+def must_not_be_truthy(value: bool, message: str = "Value must not be truthy") -> None:
+    """
+    Guard to assert truthiness & make it easier to get unit test coverage.
+    """
+    if value:
+        LOGGER.error(f"Can't be truthy, but got {value}")
+        raise TypeError(message)
+
+
+def must_be_truthy(value: Any, message: str = "Value must not be truthy") -> None:
+    """
+    Guard to assert truthiness & make it easier to get unit test coverage.
+    """
+    if not value:
+        LOGGER.error(f"Must be truthy, but got {value}")
+        raise TypeError(message)
+
+
+def must_not_be_falsy(value: Any, message: str = "Value must not be falsy") -> None:
+    """
+    Raise exception if value is falsy (i.e. False, "", None, [], etc)
+    """
+    if not value:
+        LOGGER.error(f"Must not be falsy, but got {value}")
+        raise TypeError(message)
+
+
+def must_be_falsy(value: Any, message: str = "Value must not be falsy") -> None:
+    """
+    Raise exception if value is not falsy (i.e. False, "", None, [], etc)
+    """
+    if value:
+        LOGGER.error(f"Must be falsy, but got {value}")
+        raise TypeError(message)
+
+
+def must_not_already_be_in_dictionary(
+    key: Any,
+    dictionary: Dict[Any, Any],
+    message: str = "Key already in dictionary",
+    warn_only: bool = False,
+) -> None:
+    """Assert we aren't about to insert a key twice to a dict"""
+    if key in dictionary:
+        if warn_only:
+            print(
+                f"{key} is already in dictionary where it has "
+                f"a value of {dictionary[key]}"
+            )
+        else:
+            raise TypeError(message)
+
+
+def assert_is_number(value: str) -> None:
+    """
+    Raise error if there is a value and the value is not a number
+    """
+    if value is None:
+        # Why did I do this?
+        return
+    # pylint: disable=broad-except
+    # noinspection PyBroadException
+    try:
+        _ = int(value)
+    except BaseException:
+        LOGGER.error(f"Expected numerical id, got {value}")
```

### Comparing `random_names-0.1.0/README.md` & `random_names-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `random_names-0.1.0/setup.py` & `random_names-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,94 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: random-names
+Version: 0.2.0
+Summary: Convert int to random name, like tree_dance and convert it back to same int.
+Home-page: https://github.com/matthewdeanmartin/random_names
+License: MIT
+Keywords: mneumonic,pseudorandom,name-generator
+Author: Matthew Martin
+Author-email: matthewdeanmartin@gmail.com
+Requires-Python: >=3.6
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Project-URL: Bug Tracker, https://github.com/matthewdeanmartin/random_names/issues
+Project-URL: Change Log, https://github.com/matthewdeanmartin/random_names/blob/main/docs/CHANGES.md
+Project-URL: Documentation, https://github.com/matthewdeanmartin/random_names
+Project-URL: Repository, https://github.com/matthewdeanmartin/random_names
+Description-Content-Type: text/markdown
 
-packages = \
-['random_names', 'random_names.etl', 'random_names.utils']
+# random_names
+Convert int to random name, like tree_dance and convert it back to same int.
 
-package_data = \
-{'': ['*']}
+Like [git-name](https://pypi.org/project/git-name/) which converts hashes to memorable names and back.
 
-setup_kwargs = {
-    'name': 'random-names',
-    'version': '0.1.0',
-    'description': 'Convert int to random name, like tree_dance and convert it back to same int.',
-    'long_description': '# random_names\nConvert int to random name, like tree_dance and convert it back to same int.\n\nLike [git-name](https://pypi.org/project/git-name/) which converts hashes to memorable names and back.\n\nAlso like the [Mnemonic Major System](https://en.wikipedia.org/wiki/Mnemonic_major_system) which converts\nstrings of numbers it phrases to aid in memorization, implemented here [mnemonic-major-encoder](https://pypi.org/project/mnemonic-major-encoder/)\nIn action here: https://major-system.info/en/\n\nUsage\n-----\n```\nfrom random_names.make_names import number_to_name,number_from_name\n\n# TODO: needs a user specified separator\nname = number_to_name(100,"prefix","q")\nprint(name) # prefix_q_activated\n\nnumber = number_from_name(name)\nassert number==100\n```\n\n# Why\nLets say that your users need to type in a long number, 48342342. It would be easier to\ntype in tree_dance. But your app still needs that number, so you need to convert it\nback. This is similar to [docker container names](https://github.com/moby/moby/blob/master/pkg/namesgenerator/names-generator.go), except reversable.\n\n# How\nI map 10,000 words to 4 digits, twice. That yields two words\ncovering 100,000,000 numbers.\n\nIf you use a short word list, you can\'t generate enough names.\n\nIf you use any dictionary, you get a lot of funny, obscene or offensive names. So\nI ran the world list through cuss word detection & removed most of the worst.\n\nDocs\n----\n- [To do](TODO.md)\n\n\nRelated Pypi Packages\n--\nCrypocurrency related\n- [mnemonic](https://pypi.org/project/mnemonic/) Words to cryptocurrency "wallet"\n\nMneumonic Major System\n- [major_system](https://pypi.org/project/major_system/)\n- [mnemonic-major-encoder](https://pypi.org/project/mnemonic-major-encoder/)\n\nConverting arabic numbers, e.g. 22, to spoken equivalent, e.g. twenty-two and back.\n- [inflect](https://pypi.org/project/inflect/) Converts, 22 to twenty-two\n- [words2num](https://pypi.org/project/words2num/) Converts twenty-two to 22.\n- [num2words](https://pypi.org/project/num2words/) Converts 22 to twenty-two\n- [text2num](https://pypi.org/project/text2num/) Converts twenty-two to 22. Multilingual\n- [num2rus](https://pypi.org/project/num2rus/) Converts 22 to Russian currency\n- [num2fawords](https://pypi.org/project/num2fawords/) Convert number to Persian\n- [zahlwort2num](https://pypi.org/project/zahlwort2num/) Convert german to 22.\n\nConverting numbers to a shorter string, like [Ascii85](https://en.wikipedia.org/wiki/Ascii85)\n- [num-shorty](https://pypi.org/project/num-shorty/)\n- [ascii85](https://github.com/euske/pdfminer/blob/master/pdfminer/ascii85.py)\n\nRandom names, just random names. No way to convert to a number\n- [pypi search](https://pypi.org/search/?q=random+name) To many to list, mostly just a function or two.\n',
-    'author': 'Matthew Martin',
-    'author_email': 'matthewdeanmartin@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/matthewdeanmartin/random_names',
-    'packages': packages,
-    'package_data': package_data,
-    'python_requires': '>=3.6',
-}
+Also like the [Mnemonic Major System](https://en.wikipedia.org/wiki/Mnemonic_major_system) which converts
+strings of numbers it phrases to aid in memorization, implemented here [mnemonic-major-encoder](https://pypi.org/project/mnemonic-major-encoder/)
+In action here: https://major-system.info/en/
 
+Usage
+-----
+```
+from random_names.make_names import number_to_name,number_from_name
+
+# TODO: needs a user specified separator
+name = number_to_name(100,"prefix","q")
+print(name) # prefix_q_activated
+
+number = number_from_name(name)
+assert number==100
+```
+
+# Why
+Lets say that your users need to type in a long number, 48342342. It would be easier to
+type in tree_dance. But your app still needs that number, so you need to convert it
+back. This is similar to [docker container names](https://github.com/moby/moby/blob/master/pkg/namesgenerator/names-generator.go), except reversable.
+
+# How
+I map 10,000 words to 4 digits, twice. That yields two words
+covering 100,000,000 numbers.
+
+If you use a short word list, you can't generate enough names.
+
+If you use any dictionary, you get a lot of funny, obscene or offensive names. So
+I ran the world list through cuss word detection & removed most of the worst.
+
+Docs
+----
+- [To do](TODO.md)
+
+
+Related Pypi Packages
+--
+Crypocurrency related
+- [mnemonic](https://pypi.org/project/mnemonic/) Words to cryptocurrency "wallet"
+
+Mneumonic Major System
+- [major_system](https://pypi.org/project/major_system/)
+- [mnemonic-major-encoder](https://pypi.org/project/mnemonic-major-encoder/)
+
+Converting arabic numbers, e.g. 22, to spoken equivalent, e.g. twenty-two and back.
+- [inflect](https://pypi.org/project/inflect/) Converts, 22 to twenty-two
+- [words2num](https://pypi.org/project/words2num/) Converts twenty-two to 22.
+- [num2words](https://pypi.org/project/num2words/) Converts 22 to twenty-two
+- [text2num](https://pypi.org/project/text2num/) Converts twenty-two to 22. Multilingual
+- [num2rus](https://pypi.org/project/num2rus/) Converts 22 to Russian currency
+- [num2fawords](https://pypi.org/project/num2fawords/) Convert number to Persian
+- [zahlwort2num](https://pypi.org/project/zahlwort2num/) Convert german to 22.
+
+Converting numbers to a shorter string, like [Ascii85](https://en.wikipedia.org/wiki/Ascii85)
+- [num-shorty](https://pypi.org/project/num-shorty/)
+- [ascii85](https://github.com/euske/pdfminer/blob/master/pdfminer/ascii85.py)
+
+Random names, just random names. No way to convert to a number
+- [pypi search](https://pypi.org/search/?q=random+name) To many to list, mostly just a function or two.
 
-setup(**setup_kwargs)
```


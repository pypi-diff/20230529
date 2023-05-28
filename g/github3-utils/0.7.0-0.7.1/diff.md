# Comparing `tmp/github3_utils-0.7.0.tar.gz` & `tmp/github3_utils-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "github3_utils-0.7.0.tar", last modified: Sat Jun  4 14:12:31 2022, max compression
+gzip compressed data, was "github3_utils-0.7.1.tar", last modified: Sun May 28 22:06:03 2023, max compression
```

## Comparing `github3_utils-0.7.0.tar` & `github3_utils-0.7.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0 runner    (1001) docker     (121)     4979 2022-06-04 14:12:31.681067 github3_utils-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     5286 2022-06-04 14:12:31.681067 github3_utils-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-06-04 14:12:31.673067 github3_utils-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7161 2022-06-04 14:12:31.685067 github3_utils-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-04 14:12:31.681067 github3_utils-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6233 2022-06-04 14:11:53.724570 github3_utils-0.7.0/github3_utils/check_labels.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-04 14:11:53.724570 github3_utils-0.7.0/github3_utils/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     7501 2022-06-04 14:11:53.724570 github3_utils-0.7.0/github3_utils/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     3939 2022-06-04 14:11:53.724570 github3_utils-0.7.0/github3_utils/secrets.py
--rw-r--r--   0 runner    (1001) docker     (121)     9546 2022-06-04 14:11:53.724570 github3_utils-0.7.0/github3_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1540 2022-06-04 14:11:53.724570 github3_utils-0.7.0/github3_utils/headers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1985 2022-06-04 14:11:53.724570 github3_utils-0.7.0/github3_utils/click.py
--rw-r--r--   0 runner    (1001) docker     (121)     2951 2022-06-04 14:11:53.724570 github3_utils-0.7.0/github3_utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5288 2023-05-28 22:06:03.465244 github3_utils-0.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1069 2023-05-28 22:06:03.457244 github3_utils-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      234 2023-05-28 22:06:03.465244 github3_utils-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-05-28 22:06:03.465244 github3_utils-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     5115 2023-05-28 22:06:03.465244 github3_utils-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     2951 2023-05-28 22:05:26.720409 github3_utils-0.7.1/github3_utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6233 2023-05-28 22:05:26.720409 github3_utils-0.7.1/github3_utils/check_labels.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1540 2023-05-28 22:05:26.720409 github3_utils-0.7.1/github3_utils/headers.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-28 22:05:26.720409 github3_utils-0.7.1/github3_utils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-05-28 22:05:26.720409 github3_utils-0.7.1/github3_utils/click.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7501 2023-05-28 22:05:26.720409 github3_utils-0.7.1/github3_utils/apps.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3939 2023-05-28 22:05:26.720409 github3_utils-0.7.1/github3_utils/secrets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9544 2023-05-28 22:05:26.720409 github3_utils-0.7.1/github3_utils/__init__.py
```

### Comparing `github3_utils-0.7.0/pyproject.toml` & `github3_utils-0.7.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 [build-system]
 requires = [ "whey",]
 build-backend = "whey"
 
 [project]
 name = "github3-utils"
-version = "0.7.0"
+version = "0.7.1"
 description = "Handy utilities for github3.py"
 readme = "README.rst"
 keywords = [ "github",]
 dynamic = []
 dependencies = [
     "apeye-core>=1.0.0",
     "attrs>=20.3.0",
     "click>=7.1.2",
+    'cryptography<40; implementation_name == "pypy" and python_version <= "3.7"',
     "domdf-python-tools>=1.1.0",
     "github3-py>=1.3.0",
     "pynacl>=1.4.0",
     "requests>=2.25.1",
     "typing-extensions!=3.10.0.1,>=3.10.0.0",
 ]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
@@ -59,15 +61,15 @@
 [tool.whey]
 base-classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
-python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10",]
+python-versions = [ "3.6", "3.7", "3.8", "3.9", "3.10", "3.11",]
 python-implementations = [ "CPython", "PyPy",]
 platforms = [ "Windows", "macOS", "Linux",]
 license-key = "MIT"
 package = "github3_utils"
 
 [tool.dep_checker]
 allowed_unused = [ "cryptography",]
@@ -156,15 +158,15 @@
     "__new__",
     "__getnewargs__",
     "__abstractmethods__",
     "__hash__",
 ]
 
 [tool.mypy]
-python_version = "3.6"
+python_version = "3.8"
 namespace_packages = true
 check_untyped_defs = true
 warn_unused_ignores = true
 no_implicit_optional = true
 show_error_codes = true
 
 [tool.snippet-fmt]
```

### Comparing `github3_utils-0.7.0/README.rst` & `github3_utils-0.7.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -54,16 +54,16 @@
 	:target: https://github.com/domdfcoding/github3-utils/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/github3-utils/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/github3-utils/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/github3-utils/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/github3-utils/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/github3-utils/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/github3-utils/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/github3-utils/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/github3-utils?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/github3-utils?logo=codefactor
@@ -97,23 +97,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/github3-utils
 	:target: https://github.com/domdfcoding/github3-utils/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/github3-utils
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/github3-utils/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/github3-utils/v0.7.1
 	:target: https://github.com/domdfcoding/github3-utils/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/github3-utils
 	:target: https://github.com/domdfcoding/github3-utils/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/github3-utils
 	:target: https://pypi.org/project/github3-utils/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `github3_utils-0.7.0/LICENSE` & `github3_utils-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `github3_utils-0.7.0/PKG-INFO` & `github3_utils-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: github3-utils
-Version: 0.7.0
+Version: 0.7.1
 Summary: Handy utilities for github3.py
 Author-email: Dominic Davis-Foster <dominic@davis-foster.co.uk>
 License: MIT
 Keywords: github
 Home-page: https://github.com/domdfcoding/github3-utils
 Project-URL: Issue Tracker, https://github.com/domdfcoding/github3-utils/issues
 Project-URL: Source Code, https://github.com/domdfcoding/github3-utils
@@ -19,22 +19,24 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Requires-Dist: apeye-core>=1.0.0
 Requires-Dist: attrs>=20.3.0
 Requires-Dist: click>=7.1.2
+Requires-Dist: cryptography<40; implementation_name == "pypy" and python_version <= "3.7"
 Requires-Dist: domdf-python-tools>=1.1.0
 Requires-Dist: github3-py>=1.3.0
 Requires-Dist: pynacl>=1.4.0
 Requires-Dist: requests>=2.25.1
 Requires-Dist: typing-extensions!=3.10.0.1,>=3.10.0.0
 Requires-Dist: betamax>=0.8.1; extra == 'testing'
 Requires-Dist: pytest>=6.0.0; extra == 'testing'
@@ -101,16 +103,16 @@
 	:target: https://github.com/domdfcoding/github3-utils/actions?query=workflow%3A%22Flake8%22
 	:alt: Flake8 Status
 
 .. |actions_mypy| image:: https://github.com/domdfcoding/github3-utils/workflows/mypy/badge.svg
 	:target: https://github.com/domdfcoding/github3-utils/actions?query=workflow%3A%22mypy%22
 	:alt: mypy status
 
-.. |requires| image:: https://dependency-dash.herokuapp.com/github/domdfcoding/github3-utils/badge.svg
-	:target: https://dependency-dash.herokuapp.com/github/domdfcoding/github3-utils/
+.. |requires| image:: https://dependency-dash.repo-helper.uk/github/domdfcoding/github3-utils/badge.svg
+	:target: https://dependency-dash.repo-helper.uk/github/domdfcoding/github3-utils/
 	:alt: Requirements Status
 
 .. |coveralls| image:: https://img.shields.io/coveralls/github/domdfcoding/github3-utils/master?logo=coveralls
 	:target: https://coveralls.io/github/domdfcoding/github3-utils?branch=master
 	:alt: Coverage
 
 .. |codefactor| image:: https://img.shields.io/codefactor/grade/github/domdfcoding/github3-utils?logo=codefactor
@@ -144,23 +146,23 @@
 .. |license| image:: https://img.shields.io/github/license/domdfcoding/github3-utils
 	:target: https://github.com/domdfcoding/github3-utils/blob/master/LICENSE
 	:alt: License
 
 .. |language| image:: https://img.shields.io/github/languages/top/domdfcoding/github3-utils
 	:alt: GitHub top language
 
-.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/github3-utils/v0.7.0
+.. |commits-since| image:: https://img.shields.io/github/commits-since/domdfcoding/github3-utils/v0.7.1
 	:target: https://github.com/domdfcoding/github3-utils/pulse
 	:alt: GitHub commits since tagged version
 
 .. |commits-latest| image:: https://img.shields.io/github/last-commit/domdfcoding/github3-utils
 	:target: https://github.com/domdfcoding/github3-utils/commit/master
 	:alt: GitHub last commit
 
-.. |maintained| image:: https://img.shields.io/maintenance/yes/2022
+.. |maintained| image:: https://img.shields.io/maintenance/yes/2023
 	:alt: Maintenance
 
 .. |pypi-downloads| image:: https://img.shields.io/pypi/dm/github3-utils
 	:target: https://pypi.org/project/github3-utils/
 	:alt: PyPI - Downloads
 
 .. end shields
```

### Comparing `github3_utils-0.7.0/github3_utils/check_labels.py` & `github3_utils-0.7.1/github3_utils/check_labels.py`

 * *Files identical despite different names*

### Comparing `github3_utils-0.7.0/github3_utils/apps.py` & `github3_utils-0.7.1/github3_utils/apps.py`

 * *Files identical despite different names*

### Comparing `github3_utils-0.7.0/github3_utils/secrets.py` & `github3_utils-0.7.1/github3_utils/secrets.py`

 * *Files identical despite different names*

### Comparing `github3_utils-0.7.0/github3_utils/__init__.py` & `github3_utils-0.7.1/github3_utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 #
 #  __init__.py
 """
-Handy utilities for `github3.py <https://github3py.readthedocs.io/en/master/>`_.
+Handy utilities for `github3.py <https://github3.readthedocs.io/en/latest/>`_.
 """
 #
 #  Copyright © 2020 Dominic Davis-Foster <dominic@davis-foster.co.uk>
 #
 #  Permission is hereby granted, free of charge, to any person obtaining a copy
 #  of this software and associated documentation files (the "Software"), to deal
 #  in the Software without restriction, including without limitation the rights
@@ -71,15 +71,15 @@
 
 # this package
 from github3_utils.headers import LUKE_CAGE
 
 __author__: str = "Dominic Davis-Foster"
 __copyright__: str = "2020 Dominic Davis-Foster"
 __license__: str = "MIT License"
-__version__: str = "0.7.0"
+__version__: str = "0.7.1"
 __email__: str = "dominic@davis-foster.co.uk"
 
 __all__ = (
 		"RateLimitExceeded",
 		"echo_rate_limit",
 		"get_user",
 		"protect_branch",
```

### Comparing `github3_utils-0.7.0/github3_utils/headers.py` & `github3_utils-0.7.1/github3_utils/headers.py`

 * *Files identical despite different names*

### Comparing `github3_utils-0.7.0/github3_utils/click.py` & `github3_utils-0.7.1/github3_utils/click.py`

 * *Files identical despite different names*

### Comparing `github3_utils-0.7.0/github3_utils/testing.py` & `github3_utils-0.7.1/github3_utils/testing.py`

 * *Files identical despite different names*


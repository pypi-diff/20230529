# Comparing `tmp/rgmining_fraudar-0.7.0.tar.gz` & `tmp/rgmining_fraudar-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rgmining_fraudar-0.7.0.tar", max compression
+gzip compressed data, was "rgmining_fraudar-0.7.1.tar", max compression
```

## Comparing `rgmining_fraudar-0.7.0.tar` & `rgmining_fraudar-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0    34500 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/COPYING
--rw-r--r--   0        0        0    10703 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/LICENSE-2.0
--rw-r--r--   0        0        0     2044 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/README.rst
--rw-r--r--   0        0        0     1960 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/fraudar/__init__.py
--rw-r--r--   0        0        0      823 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/fraudar/__version__.py
--rw-r--r--   0        0        0     2735 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/fraudar/export/MinTree.py
--rw-r--r--   0        0        0     4490 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/fraudar/export/README
--rw-r--r--   0        0        0     1737 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/fraudar/export/__init__.py
--rw-r--r--   0        0        0     9233 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/fraudar/export/greedy.py
--rw-r--r--   0        0        0     2417 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/fraudar/export/run_greedy.py
--rw-r--r--   0        0        0     1408 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/fraudar/export/testMinTree.py
--rw-r--r--   0        0        0     6789 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/fraudar/graph.py
--rw-r--r--   0        0        0        0 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/fraudar/py.typed
--rw-r--r--   0        0        0     2093 2023-01-07 07:12:14.400713 rgmining_fraudar-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2841 1970-01-01 00:00:00.000000 rgmining_fraudar-0.7.0/setup.py
--rw-r--r--   0        0        0     3365 1970-01-01 00:00:00.000000 rgmining_fraudar-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    34500 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/COPYING
+-rw-r--r--   0        0        0    10703 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/LICENSE-2.0
+-rw-r--r--   0        0        0     2044 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/README.rst
+-rw-r--r--   0        0        0     1960 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/__init__.py
+-rw-r--r--   0        0        0      823 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/__version__.py
+-rw-r--r--   0        0        0     2735 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/MinTree.py
+-rw-r--r--   0        0        0     4490 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/README
+-rw-r--r--   0        0        0     1737 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/__init__.py
+-rw-r--r--   0        0        0     9233 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/greedy.py
+-rw-r--r--   0        0        0     2417 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/run_greedy.py
+-rw-r--r--   0        0        0     1408 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/export/testMinTree.py
+-rw-r--r--   0        0        0     6789 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/graph.py
+-rw-r--r--   0        0        0        0 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/fraudar/py.typed
+-rw-r--r--   0        0        0     2093 2023-05-29 05:23:01.816508 rgmining_fraudar-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     3213 1970-01-01 00:00:00.000000 rgmining_fraudar-0.7.1/PKG-INFO
```

### Comparing `rgmining_fraudar-0.7.0/COPYING` & `rgmining_fraudar-0.7.1/COPYING`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.0/LICENSE-2.0` & `rgmining_fraudar-0.7.1/LICENSE-2.0`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.0/README.rst` & `rgmining_fraudar-0.7.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -41,11 +41,11 @@
    :target: https://www.gnu.org/copyleft/gpl.html
 .. |Build Status| image:: https://github.com/rgmining/fraudar/actions/workflows/python-lib.yaml/badge.svg
    :target: https://github.com/rgmining/fraudar/actions/workflows/python-lib.yaml
 .. |Maintainability| image:: https://api.codeclimate.com/v1/badges/4c4c3df79b33f65b77cd/maintainability
    :target: https://codeclimate.com/github/rgmining/fraudar/maintainability
 .. |Test Coverage| image:: https://api.codeclimate.com/v1/badges/4c4c3df79b33f65b77cd/test_coverage
    :target: https://codeclimate.com/github/rgmining/fraudar/test_coverage
-.. |Release| image:: https://img.shields.io/badge/release-0.7.0-brightgreen.svg
+.. |Release| image:: https://img.shields.io/badge/release-0.7.1-brightgreen.svg
    :target: https://pypi.org/project/rgmining-fraudar/
 .. |Logo| image:: https://rgmining.github.io/fraudar/_static/image.png
    :target: https://rgmining.github.io/fraudar/
```

### Comparing `rgmining_fraudar-0.7.0/fraudar/__init__.py` & `rgmining_fraudar-0.7.1/fraudar/__init__.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.0/fraudar/__version__.py` & `rgmining_fraudar-0.7.1/fraudar/__version__.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #  GNU General Public License for more details.
 #
 #  You should have received a copy of the GNU General Public License
 #  along with rgmining-fraudar. If not, see <http://www.gnu.org/licenses/>.
 #
 from typing import Final
 
-__version__: Final = "0.7.0"
+__version__: Final = "0.7.1"
```

### Comparing `rgmining_fraudar-0.7.0/fraudar/export/MinTree.py` & `rgmining_fraudar-0.7.1/fraudar/export/MinTree.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.0/fraudar/export/README` & `rgmining_fraudar-0.7.1/fraudar/export/README`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.0/fraudar/export/__init__.py` & `rgmining_fraudar-0.7.1/fraudar/export/__init__.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.0/fraudar/export/greedy.py` & `rgmining_fraudar-0.7.1/fraudar/export/greedy.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.0/fraudar/export/run_greedy.py` & `rgmining_fraudar-0.7.1/fraudar/export/run_greedy.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.0/fraudar/export/testMinTree.py` & `rgmining_fraudar-0.7.1/fraudar/export/testMinTree.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.0/fraudar/graph.py` & `rgmining_fraudar-0.7.1/fraudar/graph.py`

 * *Files identical despite different names*

### Comparing `rgmining_fraudar-0.7.0/pyproject.toml` & `rgmining_fraudar-0.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rgmining-fraudar"
-version = "0.7.0"
+version = "0.7.1"
 description = "A wrapper of Fraudar algorithm for Review graph mining project"
 license = "GPL-3.0-only"
 authors = ["Junpei Kawamoto <kawamoto.junpei@gmail.com>"]
 readme = "README.rst"
 homepage = "https://rgmining.github.io/fraudar/"
 repository = "https://github.com/rgmining/fraudar"
 documentation = "https://rgmining.github.io/fraudar/"
```

### Comparing `rgmining_fraudar-0.7.0/setup.py` & `rgmining_fraudar-0.7.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,79 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: rgmining-fraudar
+Version: 0.7.1
+Summary: A wrapper of Fraudar algorithm for Review graph mining project
+Home-page: https://rgmining.github.io/fraudar/
+License: GPL-3.0-only
+Keywords: review,graph,mining,algorithm,kdd,fraudar
+Author: Junpei Kawamoto
+Author-email: kawamoto.junpei@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Information Analysis
+Classifier: Topic :: Software Development :: Libraries
+Requires-Dist: numpy (>=1.24.1,<2.0.0)
+Requires-Dist: scikit-learn (>=1.2.0,<2.0.0)
+Project-URL: Documentation, https://rgmining.github.io/fraudar/
+Project-URL: Repository, https://github.com/rgmining/fraudar
+Description-Content-Type: text/x-rst
+
+A wrapper of FRAUDAR algorithm
+==============================
+
+|GPLv3| |Build Status| |Maintainability| |Test Coverage| |Release|
+
+|Logo|
+
+This package implements a wrapper of
+`FRAUDAR <https://bhooi.github.io/projects/fraudar/index.html>`__
+algorithm to provide APIs defined in `Review Graph Mining
+project <https://rgmining.github.io/>`__.
+
+Installation
+------------
+
+Use ``pip`` to install this package.
+
+.. code:: shell
+
+    $pip install --upgrade rgmining-fraudar
+
+License
+-------
+
+This software is released under The GNU General Public License Version
+3, see
+`COPYING <https://github.com/rgmining/fraudar/blob/master/COPYING>`__
+for more detail.
+
+The original FRAUDAR source code is made by `Bryan
+Hooi <https://bhooi.github.io/index.html>`__, `Hyun Ah
+Song <http://www.cs.cmu.edu/~hyunahs/>`__, `Alex
+Beutel <http://alexbeutel.com/>`__, `Neil
+Shah <http://nshah.net/>`__, `Kijung
+Shin <https://kijungs.github.io/>`__, and `Christos
+Faloutsos <http://www.cs.cmu.edu/~christos/>`__, and licensed under
+`Apache License, Version 2.0 <LICENSE-2.0>`__. It is available at
+https://bhooi.github.io/projects/fraudar/index.html.
+
+.. |GPLv3| image:: https://img.shields.io/badge/license-GPLv3-blue.svg
+   :target: https://www.gnu.org/copyleft/gpl.html
+.. |Build Status| image:: https://github.com/rgmining/fraudar/actions/workflows/python-lib.yaml/badge.svg
+   :target: https://github.com/rgmining/fraudar/actions/workflows/python-lib.yaml
+.. |Maintainability| image:: https://api.codeclimate.com/v1/badges/4c4c3df79b33f65b77cd/maintainability
+   :target: https://codeclimate.com/github/rgmining/fraudar/maintainability
+.. |Test Coverage| image:: https://api.codeclimate.com/v1/badges/4c4c3df79b33f65b77cd/test_coverage
+   :target: https://codeclimate.com/github/rgmining/fraudar/test_coverage
+.. |Release| image:: https://img.shields.io/badge/release-0.7.1-brightgreen.svg
+   :target: https://pypi.org/project/rgmining-fraudar/
+.. |Logo| image:: https://rgmining.github.io/fraudar/_static/image.png
+   :target: https://rgmining.github.io/fraudar/
 
-packages = \
-['fraudar', 'fraudar.export']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numpy>=1.24.1,<2.0.0', 'scikit-learn>=1.2.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'rgmining-fraudar',
-    'version': '0.7.0',
-    'description': 'A wrapper of Fraudar algorithm for Review graph mining project',
-    'long_description': 'A wrapper of FRAUDAR algorithm\n==============================\n\n|GPLv3| |Build Status| |Maintainability| |Test Coverage| |Release|\n\n|Logo|\n\nThis package implements a wrapper of\n`FRAUDAR <https://bhooi.github.io/projects/fraudar/index.html>`__\nalgorithm to provide APIs defined in `Review Graph Mining\nproject <https://rgmining.github.io/>`__.\n\nInstallation\n------------\n\nUse ``pip`` to install this package.\n\n.. code:: shell\n\n    $pip install --upgrade rgmining-fraudar\n\nLicense\n-------\n\nThis software is released under The GNU General Public License Version\n3, see\n`COPYING <https://github.com/rgmining/fraudar/blob/master/COPYING>`__\nfor more detail.\n\nThe original FRAUDAR source code is made by `Bryan\nHooi <https://bhooi.github.io/index.html>`__, `Hyun Ah\nSong <http://www.cs.cmu.edu/~hyunahs/>`__, `Alex\nBeutel <http://alexbeutel.com/>`__, `Neil\nShah <http://nshah.net/>`__, `Kijung\nShin <https://kijungs.github.io/>`__, and `Christos\nFaloutsos <http://www.cs.cmu.edu/~christos/>`__, and licensed under\n`Apache License, Version 2.0 <LICENSE-2.0>`__. It is available at\nhttps://bhooi.github.io/projects/fraudar/index.html.\n\n.. |GPLv3| image:: https://img.shields.io/badge/license-GPLv3-blue.svg\n   :target: https://www.gnu.org/copyleft/gpl.html\n.. |Build Status| image:: https://github.com/rgmining/fraudar/actions/workflows/python-lib.yaml/badge.svg\n   :target: https://github.com/rgmining/fraudar/actions/workflows/python-lib.yaml\n.. |Maintainability| image:: https://api.codeclimate.com/v1/badges/4c4c3df79b33f65b77cd/maintainability\n   :target: https://codeclimate.com/github/rgmining/fraudar/maintainability\n.. |Test Coverage| image:: https://api.codeclimate.com/v1/badges/4c4c3df79b33f65b77cd/test_coverage\n   :target: https://codeclimate.com/github/rgmining/fraudar/test_coverage\n.. |Release| image:: https://img.shields.io/badge/release-0.7.0-brightgreen.svg\n   :target: https://pypi.org/project/rgmining-fraudar/\n.. |Logo| image:: https://rgmining.github.io/fraudar/_static/image.png\n   :target: https://rgmining.github.io/fraudar/\n',
-    'author': 'Junpei Kawamoto',
-    'author_email': 'kawamoto.junpei@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://rgmining.github.io/fraudar/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
-
-
-setup(**setup_kwargs)
```


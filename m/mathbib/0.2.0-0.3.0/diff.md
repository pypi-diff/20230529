# Comparing `tmp/mathbib-0.2.0.tar.gz` & `tmp/mathbib-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.2.0.tar", last modified: Sun May 28 17:11:31 2023, max compression
+gzip compressed data, was "mathbib-0.3.0.tar", max compression
```

## Comparing `mathbib-0.2.0.tar` & `mathbib-0.3.0.tar`

### file list

```diff
@@ -1,40 +1,25 @@
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.757627 mathbib-0.2.0/
--rw-r--r--   0 alexrutar   (501) staff       (20)       51 2023-05-25 15:29:52.000000 mathbib-0.2.0/MANIFEST.in
--rw-r--r--   0 alexrutar   (501) staff       (20)     5818 2023-05-28 17:11:31.757848 mathbib-0.2.0/PKG-INFO
--rw-r--r--   0 alexrutar   (501) staff       (20)     5354 2023-05-28 15:53:57.000000 mathbib-0.2.0/README.md
--rw-r--r--   0 alexrutar   (501) staff       (20)      318 2023-05-10 21:34:37.000000 mathbib-0.2.0/pyproject.toml
--rw-r--r--   0 alexrutar   (501) staff       (20)     1026 2023-05-28 17:11:31.759044 mathbib-0.2.0/setup.cfg
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.738276 mathbib-0.2.0/src/
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.743960 mathbib-0.2.0/src/mathbib/
--rw-r--r--   0 alexrutar   (501) staff       (20)      220 2023-05-28 17:10:17.000000 mathbib-0.2.0/src/mathbib/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)       63 2023-05-10 21:47:55.000000 mathbib-0.2.0/src/mathbib/__main__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1402 2023-05-28 11:08:27.000000 mathbib-0.2.0/src/mathbib/bibtex.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     2831 2023-05-28 15:54:03.000000 mathbib-0.2.0/src/mathbib/citegen.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     9963 2023-05-28 16:57:04.000000 mathbib-0.2.0/src/mathbib/command.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     2841 2023-05-28 16:33:13.000000 mathbib-0.2.0/src/mathbib/partition.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     9459 2023-05-28 15:11:22.000000 mathbib-0.2.0/src/mathbib/record.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.751658 mathbib-0.2.0/src/mathbib/remote/
--rw-r--r--   0 alexrutar   (501) staff       (20)     5481 2023-05-28 13:40:33.000000 mathbib-0.2.0/src/mathbib/remote/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     3088 2023-05-28 12:38:27.000000 mathbib-0.2.0/src/mathbib/remote/arxiv.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      923 2023-05-27 20:04:18.000000 mathbib-0.2.0/src/mathbib/remote/doi.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      855 2023-05-28 09:33:03.000000 mathbib-0.2.0/src/mathbib/remote/error.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1475 2023-05-27 20:04:18.000000 mathbib-0.2.0/src/mathbib/remote/isbn.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1194 2023-05-27 18:35:57.000000 mathbib-0.2.0/src/mathbib/remote/ol.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     4257 2023-05-28 15:10:12.000000 mathbib-0.2.0/src/mathbib/remote/utils.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      597 2023-05-25 12:11:18.000000 mathbib-0.2.0/src/mathbib/remote/zbl.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     1816 2023-05-28 12:19:04.000000 mathbib-0.2.0/src/mathbib/remote/zbmath.py
--rw-r--r--   0 alexrutar   (501) staff       (20)     5552 2023-05-28 12:31:57.000000 mathbib-0.2.0/src/mathbib/request.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.752581 mathbib-0.2.0/src/mathbib/resources/
--rw-r--r--   0 alexrutar   (501) staff       (20)        0 2023-05-25 15:24:07.000000 mathbib-0.2.0/src/mathbib/resources/__init__.py
--rw-r--r--   0 alexrutar   (501) staff       (20)   270192 2023-05-25 15:19:42.000000 mathbib-0.2.0/src/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0 alexrutar   (501) staff       (20)     2613 2023-05-28 12:14:16.000000 mathbib-0.2.0/src/mathbib/session.py
--rw-r--r--   0 alexrutar   (501) staff       (20)      705 2023-05-25 11:53:39.000000 mathbib-0.2.0/src/mathbib/term.py
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.747002 mathbib-0.2.0/src/mathbib.egg-info/
--rw-r--r--   0 alexrutar   (501) staff       (20)     5818 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/PKG-INFO
--rw-r--r--   0 alexrutar   (501) staff       (20)      835 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/SOURCES.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)        1 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/dependency_links.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)       45 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/entry_points.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)      131 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/requires.txt
--rw-r--r--   0 alexrutar   (501) staff       (20)        8 2023-05-28 17:11:31.000000 mathbib-0.2.0/src/mathbib.egg-info/top_level.txt
-drwxr-xr-x   0 alexrutar   (501) staff       (20)        0 2023-05-28 17:11:31.755687 mathbib-0.2.0/test/
--rw-r--r--   0 alexrutar   (501) staff       (20)      719 2023-05-27 20:04:18.000000 mathbib-0.2.0/test/test_partition.py
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.3.0/LICENSE
+-rw-r--r--   0        0        0     5354 2023-05-28 15:53:57.671925 mathbib-0.3.0/README.md
+-rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.3.0/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.3.0/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.3.0/mathbib/bibtex.py
+-rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.3.0/mathbib/citegen.py
+-rw-r--r--   0        0        0     9963 2023-05-29 16:24:57.749266 mathbib-0.3.0/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.3.0/mathbib/partition.py
+-rw-r--r--   0        0        0     9459 2023-05-28 15:11:22.084659 mathbib-0.3.0/mathbib/record.py
+-rw-r--r--   0        0        0     5481 2023-05-28 13:40:33.677396 mathbib-0.3.0/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.3.0/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.3.0/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.3.0/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.3.0/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.3.0/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4257 2023-05-28 15:10:12.248626 mathbib-0.3.0/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.3.0/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.3.0/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     5512 2023-05-29 16:27:20.815594 mathbib-0.3.0/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.3.0/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270192 2023-05-25 15:19:42.503313 mathbib-0.3.0/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     2613 2023-05-28 12:14:16.785236 mathbib-0.3.0/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.3.0/mathbib/term.py
+-rw-r--r--   0        0        0      917 2023-05-29 16:28:17.620701 mathbib-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6243 1970-01-01 00:00:00.000000 mathbib-0.3.0/PKG-INFO
```

### Comparing `mathbib-0.2.0/PKG-INFO` & `mathbib-0.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: mathbib
-Version: 0.2.0
-Summary: A mathematics BibLaTeX bibliography manager.
-Home-page: https://github.com/alexrutar/mathbib-py
-Author: Alex Rutar
-Author-email: alex@rutar.org
-Classifier: Development Status :: 3 - Alpha
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11.0
-Description-Content-Type: text/markdown
-
 # MathBib
 MathBib is a mathematics BibLaTeX bibliography manager.
 
 **WARNING: MathBib is currently in alpha state. The API and other implementation details may change substantially!**
 
 ## Installation and basic usage
 First, ensure that `mbib` is installed with
```

### Comparing `mathbib-0.2.0/README.md` & `mathbib-0.3.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,31 @@
+Metadata-Version: 2.1
+Name: mathbib
+Version: 0.3.0
+Summary: A mathematics BibLaTeX bibliography manager.
+Home-page: https://github.com/alexrutar/mathbib-py
+License: MIT
+Author: Alex Rutar
+Author-email: alex@rutar.org
+Requires-Python: >=3.11.0,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: bibtexparser (>=1.4.0,<2.0.0)
+Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: nameparser (>=1.1.2,<2.0.0)
+Requires-Dist: python-stdnum (>=1.18,<2.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
+Requires-Dist: xdg-base-dirs (>=6.0.0,<7.0.0)
+Project-URL: Repository, https://github.com/alexrutar/mathbib-py
+Description-Content-Type: text/markdown
+
 # MathBib
 MathBib is a mathematics BibLaTeX bibliography manager.
 
 **WARNING: MathBib is currently in alpha state. The API and other implementation details may change substantially!**
 
 ## Installation and basic usage
 First, ensure that `mbib` is installed with
@@ -124,7 +148,8 @@
 # Contributing and future improvements
 MathBib is still under active development!
 Some planned features include:
 
 1. Rework the code for remote record searching and parsing.
 2. Asynchronous requests for faster record downloading.
 3. Nicer printing and viewing using [rich](https://rich.readthedocs.io/en/stable/introduction.html).
+
```

### Comparing `mathbib-0.2.0/src/mathbib/bibtex.py` & `mathbib-0.3.0/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/citegen.py` & `mathbib-0.3.0/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/command.py` & `mathbib-0.3.0/mathbib/command.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/partition.py` & `mathbib-0.3.0/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/record.py` & `mathbib-0.3.0/mathbib/record.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/remote/__init__.py` & `mathbib-0.3.0/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/remote/arxiv.py` & `mathbib-0.3.0/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/remote/doi.py` & `mathbib-0.3.0/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/remote/error.py` & `mathbib-0.3.0/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/remote/isbn.py` & `mathbib-0.3.0/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/remote/ol.py` & `mathbib-0.3.0/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/remote/utils.py` & `mathbib-0.3.0/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/remote/zbl.py` & `mathbib-0.3.0/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/remote/zbmath.py` & `mathbib-0.3.0/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/request.py` & `mathbib-0.3.0/mathbib/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 import click
 import requests
 import sys
 import tomllib
 
 from xdg_base_dirs import xdg_config_home
 
-from . import __version__
 from .term import TermWrite
 from .remote import get_remote_record
 
 
 class RemoteSession:
     def __init__(
         self,
@@ -32,15 +31,15 @@
         self.session = requests.Session()
 
         contact_email = tomllib.loads(
             (xdg_config_home() / "mathbib" / "config.toml").read_text()
         ).get("email")
         if contact_email is not None:
             self.session.headers.update(
-                {"User-Agent": f"MathBib/{__version__} (mailto:{contact_email})"}
+                {"User-Agent": f"MathBib (mailto:{contact_email})"}
             )
 
         self.timeout = timeout
         self.print_info = info
         self.cache = cache
         self.remote = remote
```

### Comparing `mathbib-0.2.0/src/mathbib/resources/journal_abbrevs.json` & `mathbib-0.3.0/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/session.py` & `mathbib-0.3.0/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.2.0/src/mathbib/term.py` & `mathbib-0.3.0/mathbib/term.py`

 * *Files identical despite different names*


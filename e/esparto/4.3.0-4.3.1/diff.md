# Comparing `tmp/esparto-4.3.0.tar.gz` & `tmp/esparto-4.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esparto-4.3.0.tar", max compression
+gzip compressed data, was "esparto-4.3.1.tar", max compression
```

## Comparing `esparto-4.3.0.tar` & `esparto-4.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1071 2022-04-19 15:56:37.678436 esparto-4.3.0/LICENSE
--rw-r--r--   0        0        0     3792 2022-06-29 20:48:26.649962 esparto-4.3.0/README.md
--rw-r--r--   0        0        0     1317 2023-05-29 09:40:48.655809 esparto-4.3.0/esparto/__init__.py
--rw-r--r--   0        0        0       69 2022-04-20 07:43:09.473785 esparto-4.3.0/esparto/__main__.py
--rw-r--r--   0        0        0     3265 2022-04-20 07:43:09.473785 esparto-4.3.0/esparto/_cli.py
--rw-r--r--   0        0        0     7127 2023-05-29 09:20:09.460818 esparto-4.3.0/esparto/_options.py
--rw-r--r--   0        0        0        0 2022-04-20 07:43:09.473785 esparto-4.3.0/esparto/design/__init__.py
--rw-r--r--   0        0        0     3326 2023-05-29 09:41:13.871626 esparto-4.3.0/esparto/design/adaptors.py
--rw-r--r--   0        0        0     2506 2022-04-20 07:43:09.473785 esparto-4.3.0/esparto/design/base.py
--rw-r--r--   0        0        0    16968 2023-05-29 09:48:22.504510 esparto-4.3.0/esparto/design/content.py
--rw-r--r--   0        0        0    32166 2022-06-29 20:40:25.602795 esparto-4.3.0/esparto/design/layout.py
--rw-r--r--   0        0        0        0 2022-04-20 07:43:09.473785 esparto-4.3.0/esparto/publish/__init__.py
--rw-r--r--   0        0        0     2388 2023-05-29 09:39:11.168518 esparto-4.3.0/esparto/publish/contentdeps.py
--rw-r--r--   0        0        0     6344 2023-05-29 09:39:25.736412 esparto-4.3.0/esparto/publish/output.py
--rw-r--r--   0        0        0   163874 2022-06-29 14:45:25.039530 esparto-4.3.0/esparto/resources/css/bootstrap.min.css
--rw-r--r--   0        0        0     3041 2022-06-29 20:40:25.602795 esparto-4.3.0/esparto/resources/css/esparto.css
--rw-r--r--   0        0        0     3646 2022-11-10 18:27:36.095751 esparto-4.3.0/esparto/resources/jinja/base.html.jinja
--rw-r--r--   0        0        0      924 2022-06-29 20:40:25.602795 esparto-4.3.0/esparto/resources/js/esparto.js
--rw-r--r--   0        0        0     1856 2023-05-29 09:35:32.734106 esparto-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 esparto-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-04-19 15:56:37.678436 esparto-4.3.1/LICENSE
+-rw-r--r--   0        0        0     3792 2022-06-29 20:48:26.649962 esparto-4.3.1/README.md
+-rw-r--r--   0        0        0     1317 2023-05-29 10:25:11.386032 esparto-4.3.1/esparto/__init__.py
+-rw-r--r--   0        0        0       69 2022-04-20 07:43:09.473785 esparto-4.3.1/esparto/__main__.py
+-rw-r--r--   0        0        0     3265 2022-04-20 07:43:09.473785 esparto-4.3.1/esparto/_cli.py
+-rw-r--r--   0        0        0     7127 2023-05-29 10:18:59.195956 esparto-4.3.1/esparto/_options.py
+-rw-r--r--   0        0        0        0 2022-04-20 07:43:09.473785 esparto-4.3.1/esparto/design/__init__.py
+-rw-r--r--   0        0        0     3326 2023-05-29 10:18:59.195956 esparto-4.3.1/esparto/design/adaptors.py
+-rw-r--r--   0        0        0     2506 2022-04-20 07:43:09.473785 esparto-4.3.1/esparto/design/base.py
+-rw-r--r--   0        0        0    16968 2023-05-29 10:18:59.195956 esparto-4.3.1/esparto/design/content.py
+-rw-r--r--   0        0        0    32166 2022-06-29 20:40:25.602795 esparto-4.3.1/esparto/design/layout.py
+-rw-r--r--   0        0        0        0 2022-04-20 07:43:09.473785 esparto-4.3.1/esparto/publish/__init__.py
+-rw-r--r--   0        0        0     2388 2023-05-29 10:18:59.195956 esparto-4.3.1/esparto/publish/contentdeps.py
+-rw-r--r--   0        0        0     6344 2023-05-29 10:18:59.195956 esparto-4.3.1/esparto/publish/output.py
+-rw-r--r--   0        0        0   163874 2022-06-29 14:45:25.039530 esparto-4.3.1/esparto/resources/css/bootstrap.min.css
+-rw-r--r--   0        0        0     3041 2022-06-29 20:40:25.602795 esparto-4.3.1/esparto/resources/css/esparto.css
+-rw-r--r--   0        0        0     3646 2022-11-10 18:27:36.095751 esparto-4.3.1/esparto/resources/jinja/base.html.jinja
+-rw-r--r--   0        0        0     1182 2023-05-29 10:30:53.586388 esparto-4.3.1/esparto/resources/js/esparto.js
+-rw-r--r--   0        0        0     1856 2023-05-29 10:25:24.770067 esparto-4.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 esparto-4.3.1/PKG-INFO
```

### Comparing `esparto-4.3.0/LICENSE` & `esparto-4.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/README.md` & `esparto-4.3.1/README.md`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/__init__.py` & `esparto-4.3.1/esparto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import dataclasses as _dc
 from importlib.util import find_spec as _find_spec
 from pathlib import Path as _Path
 
 __author__ = """Dominic Thorn"""
 __email__ = "dominic.thorn@gmail.com"
-__version__ = "4.3.0"
+__version__ = "4.3.1"
 
 _MODULE_PATH: _Path = _Path(__file__).parent.absolute()
 
 
 @_dc.dataclass(frozen=True)
 class _OptionalDependencies:
     PIL: bool = _find_spec("PIL") is not None
```

### Comparing `esparto-4.3.0/esparto/_cli.py` & `esparto-4.3.1/esparto/_cli.py`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/_options.py` & `esparto-4.3.1/esparto/_options.py`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/design/adaptors.py` & `esparto-4.3.1/esparto/design/adaptors.py`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/design/base.py` & `esparto-4.3.1/esparto/design/base.py`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/design/content.py` & `esparto-4.3.1/esparto/design/content.py`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/design/layout.py` & `esparto-4.3.1/esparto/design/layout.py`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/publish/contentdeps.py` & `esparto-4.3.1/esparto/publish/contentdeps.py`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/publish/output.py` & `esparto-4.3.1/esparto/publish/output.py`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/resources/css/bootstrap.min.css` & `esparto-4.3.1/esparto/resources/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/resources/css/esparto.css` & `esparto-4.3.1/esparto/resources/css/esparto.css`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/esparto/resources/jinja/base.html.jinja` & `esparto-4.3.1/esparto/resources/jinja/base.html.jinja`

 * *Files identical despite different names*

### Comparing `esparto-4.3.0/pyproject.toml` & `esparto-4.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "esparto"
-version = "4.3.0"
+version = "4.3.1"
 description = "Data driven report builder for the PyData ecosystem."
 authors = ["Dominic Thorn <dominic.thorn@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://domvwt.github.io/esparto"
 repository = "https://github.com/domvwt/esparto"
 classifiers = [
```

### Comparing `esparto-4.3.0/PKG-INFO` & `esparto-4.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esparto
-Version: 4.3.0
+Version: 4.3.1
 Summary: Data driven report builder for the PyData ecosystem.
 Home-page: https://domvwt.github.io/esparto
 License: MIT
 Author: Dominic Thorn
 Author-email: dominic.thorn@gmail.com
 Requires-Python: >=3.6.1
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: esparto Version: 4.3.0 Summary: Data driven report
+Metadata-Version: 2.1 Name: esparto Version: 4.3.1 Summary: Data driven report
 builder for the PyData ecosystem. Home-page: https://domvwt.github.io/esparto
 License: MIT Author: Dominic Thorn Author-email: dominic.thorn@gmail.com
 Requires-Python: >=3.6.1 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```


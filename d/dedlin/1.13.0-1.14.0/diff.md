# Comparing `tmp/dedlin-1.13.0.tar.gz` & `tmp/dedlin-1.14.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedlin-1.13.0.tar", max compression
+gzip compressed data, was "dedlin-1.14.0.tar", max compression
```

## Comparing `dedlin-1.13.0.tar` & `dedlin-1.14.0.tar`

### file list

```diff
@@ -1,36 +1,35 @@
--rw-r--r--   0        0        0        0 2023-02-26 02:20:22.397674 dedlin-1.13.0/dedlin/__init__.py
--rw-r--r--   0        0        0     4282 2023-05-13 18:30:05.436664 dedlin-1.13.0/dedlin/__main__.py
--rw-r--r--   0        0        0     8790 2023-05-13 18:36:03.687054 dedlin-1.13.0/dedlin/basic_types.py
--rw-r--r--   0        0        0     4005 2023-02-25 20:07:21.449444 dedlin-1.13.0/dedlin/command_sources.py
--rw-r--r--   0        0        0    15363 2023-05-13 18:36:42.894018 dedlin-1.13.0/dedlin/document.py
--rw-r--r--   0        0        0     3113 2022-12-29 22:47:14.768636 dedlin-1.13.0/dedlin/document_sources.py
--rw-r--r--   0        0        0     2145 2023-05-13 18:30:05.467647 dedlin-1.13.0/dedlin/file_system.py
--rw-r--r--   0        0        0      243 2023-05-13 18:30:05.398607 dedlin-1.13.0/dedlin/flash.py
--rw-r--r--   0        0        0     1632 2023-05-13 18:30:05.520016 dedlin-1.13.0/dedlin/history_feature.py
--rw-r--r--   0        0        0     1726 2022-07-05 00:14:05.011630 dedlin-1.13.0/dedlin/logging_utils.py
--rw-r--r--   0        0        0    15662 2023-05-13 18:35:00.400481 dedlin-1.13.0/dedlin/main.py
--rw-r--r--   0        0        0        0 2023-03-26 21:45:09.221680 dedlin-1.13.0/dedlin/outputters/__init__.py
--rw-r--r--   0        0        0      355 2023-05-13 18:34:07.064200 dedlin-1.13.0/dedlin/outputters/plain.py
--rw-r--r--   0        0        0      919 2023-05-13 18:30:05.330744 dedlin-1.13.0/dedlin/outputters/rich_output.py
--rw-r--r--   0        0        0      653 2023-05-13 18:34:29.407911 dedlin-1.13.0/dedlin/outputters/talking_outputter.py
--rw-r--r--   0        0        0    10936 2023-05-13 18:30:05.630575 dedlin-1.13.0/dedlin/parsers.py
--rw-r--r--   0        0        0       80 2022-06-03 01:18:36.274653 dedlin-1.13.0/dedlin/py.typed
--rw-r--r--   0        0        0      588 2022-07-04 17:56:26.713572 dedlin-1.13.0/dedlin/pygments_code.py
--rw-r--r--   0        0        0     2215 2023-05-13 18:33:06.561257 dedlin-1.13.0/dedlin/string_comands.py
--rw-r--r--   0        0        0        0 2023-03-26 22:05:33.927432 dedlin-1.13.0/dedlin/text/__init__.py
--rw-r--r--   0        0        0     1948 2022-07-31 17:02:36.145350 dedlin-1.13.0/dedlin/text/help_text.py
--rw-r--r--   0        0        0        0 2023-03-26 21:45:53.009840 dedlin-1.13.0/dedlin/tools/__init__.py
--rw-r--r--   0        0        0      273 2023-05-13 18:30:05.403605 dedlin-1.13.0/dedlin/tools/export.py
--rw-r--r--   0        0        0      780 2022-06-26 01:45:04.623153 dedlin-1.13.0/dedlin/tools/info_bar.py
--rw-r--r--   0        0        0     1970 2022-06-18 23:31:53.155666 dedlin-1.13.0/dedlin/tools/lorem_data.py
--rw-r--r--   0        0        0      595 2023-01-02 22:38:48.075545 dedlin-1.13.0/dedlin/tools/spelling_overlay.py
--rw-r--r--   0        0        0      677 2022-06-26 01:40:42.646243 dedlin-1.13.0/dedlin/tools/web.py
--rw-r--r--   0        0        0        0 2022-06-09 18:10:08.703000 dedlin-1.13.0/dedlin/utils/__init__.py
--rw-r--r--   0        0        0      225 2022-06-19 21:12:46.591013 dedlin-1.13.0/dedlin/utils/exceptions.py
--rw-r--r--   0        0        0      366 2022-06-21 02:31:26.265490 dedlin-1.13.0/dedlin/utils/file_utils.py
--rw-r--r--   0        0        0     1529 2022-12-08 00:17:58.932590 dedlin-1.13.0/dedlin/web_api.py
--rw-r--r--   0        0        0     1071 2022-06-16 01:43:23.611981 dedlin-1.13.0/LICENSE
--rw-r--r--   0        0        0     3708 2023-05-13 18:37:28.881677 dedlin-1.13.0/pyproject.toml
--rw-r--r--   0        0        0     2913 2023-05-13 18:31:15.766160 dedlin-1.13.0/README.md
--rw-r--r--   0        0        0     4171 1970-01-01 00:00:00.000000 dedlin-1.13.0/setup.py
--rw-r--r--   0        0        0     4418 1970-01-01 00:00:00.000000 dedlin-1.13.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-29 14:10:45.270049 dedlin-1.14.0/LICENSE
+-rw-r--r--   0        0        0     2913 2023-05-29 14:12:44.753118 dedlin-1.14.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/__init__.py
+-rw-r--r--   0        0        0     4282 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/__main__.py
+-rw-r--r--   0        0        0     8790 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/basic_types.py
+-rw-r--r--   0        0        0     4005 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/command_sources.py
+-rw-r--r--   0        0        0    15363 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/document.py
+-rw-r--r--   0        0        0     3113 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/document_sources.py
+-rw-r--r--   0        0        0     2145 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/file_system.py
+-rw-r--r--   0        0        0      243 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/flash.py
+-rw-r--r--   0        0        0     1632 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/history_feature.py
+-rw-r--r--   0        0        0     1726 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/logging_utils.py
+-rw-r--r--   0        0        0    15662 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/main.py
+-rw-r--r--   0        0        0        0 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/outputters/__init__.py
+-rw-r--r--   0        0        0      355 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/outputters/plain.py
+-rw-r--r--   0        0        0      919 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/outputters/rich_output.py
+-rw-r--r--   0        0        0      653 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/outputters/talking_outputter.py
+-rw-r--r--   0        0        0    10936 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/parsers.py
+-rw-r--r--   0        0        0       80 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/py.typed
+-rw-r--r--   0        0        0      588 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/pygments_code.py
+-rw-r--r--   0        0        0     2215 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/string_comands.py
+-rw-r--r--   0        0        0        0 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/text/__init__.py
+-rw-r--r--   0        0        0     1948 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/text/help_text.py
+-rw-r--r--   0        0        0        0 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/tools/__init__.py
+-rw-r--r--   0        0        0      273 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/tools/export.py
+-rw-r--r--   0        0        0      780 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/tools/info_bar.py
+-rw-r--r--   0        0        0     1970 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/tools/lorem_data.py
+-rw-r--r--   0        0        0      595 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/tools/spelling_overlay.py
+-rw-r--r--   0        0        0      677 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/tools/web.py
+-rw-r--r--   0        0        0        0 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/utils/__init__.py
+-rw-r--r--   0        0        0      225 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/utils/exceptions.py
+-rw-r--r--   0        0        0      366 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/utils/file_utils.py
+-rw-r--r--   0        0        0     1529 2023-05-29 14:10:45.274049 dedlin-1.14.0/dedlin/web_api.py
+-rw-r--r--   0        0        0     3708 2023-05-29 14:10:45.274049 dedlin-1.14.0/pyproject.toml
+-rw-r--r--   0        0        0     4367 1970-01-01 00:00:00.000000 dedlin-1.14.0/PKG-INFO
```

### Comparing `dedlin-1.13.0/dedlin/__main__.py` & `dedlin-1.14.0/dedlin/__main__.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/basic_types.py` & `dedlin-1.14.0/dedlin/basic_types.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/command_sources.py` & `dedlin-1.14.0/dedlin/command_sources.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/document.py` & `dedlin-1.14.0/dedlin/document.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/document_sources.py` & `dedlin-1.14.0/dedlin/document_sources.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/file_system.py` & `dedlin-1.14.0/dedlin/file_system.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/history_feature.py` & `dedlin-1.14.0/dedlin/history_feature.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/logging_utils.py` & `dedlin-1.14.0/dedlin/logging_utils.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/main.py` & `dedlin-1.14.0/dedlin/main.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/outputters/rich_output.py` & `dedlin-1.14.0/dedlin/outputters/rich_output.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/outputters/talking_outputter.py` & `dedlin-1.14.0/dedlin/outputters/talking_outputter.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/parsers.py` & `dedlin-1.14.0/dedlin/parsers.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/pygments_code.py` & `dedlin-1.14.0/dedlin/pygments_code.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/string_comands.py` & `dedlin-1.14.0/dedlin/string_comands.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/text/help_text.py` & `dedlin-1.14.0/dedlin/text/help_text.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/tools/info_bar.py` & `dedlin-1.14.0/dedlin/tools/info_bar.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/tools/lorem_data.py` & `dedlin-1.14.0/dedlin/tools/lorem_data.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/tools/spelling_overlay.py` & `dedlin-1.14.0/dedlin/tools/spelling_overlay.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/tools/web.py` & `dedlin-1.14.0/dedlin/tools/web.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/dedlin/web_api.py` & `dedlin-1.14.0/dedlin/web_api.py`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/LICENSE` & `dedlin-1.14.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/pyproject.toml` & `dedlin-1.14.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dedlin"
-version = "1.13.0"
+version = "1.14.0"
 description = "Line editor, edlin clone with many improvements"
 authors = ["Matthew Martin <matthewdeanmartin@gmail.com>"]
 keywords = ["editor", "edlin", "line editor",]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `dedlin-1.13.0/README.md` & `dedlin-1.14.0/README.md`

 * *Files identical despite different names*

### Comparing `dedlin-1.13.0/PKG-INFO` & `dedlin-1.14.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: dedlin
-Version: 1.13.0
+Version: 1.14.0
 Summary: Line editor, edlin clone with many improvements
 Home-page: https://github.com/matthewdeanmartin/dedlin
 License: MIT
 Keywords: editor,edlin,line editor
 Author: Matthew Martin
 Author-email: matthewdeanmartin@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: webapi
 Requires-Dist: art
 Requires-Dist: docopt-ng
 Requires-Dist: fastapi ; extra == "webapi"
 Requires-Dist: html2text
 Requires-Dist: icontract
 Requires-Dist: mistune
```


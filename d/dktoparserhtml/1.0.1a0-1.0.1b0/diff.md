# Comparing `tmp/dktoparserhtml-1.0.1a0.tar.gz` & `tmp/dktoparserhtml-1.0.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dktoparserhtml-1.0.1a0.tar", last modified: Mon May 29 18:54:05 2023, max compression
+gzip compressed data, was "dktoparserhtml-1.0.1b0.tar", last modified: Mon May 29 19:08:29 2023, max compression
```

## Comparing `dktoparserhtml-1.0.1a0.tar` & `dktoparserhtml-1.0.1b0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:54:05.291263 dktoparserhtml-1.0.1a0/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1844 2023-05-29 18:54:05.291263 dktoparserhtml-1.0.1a0/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1057 2023-05-29 18:26:00.000000 dktoparserhtml-1.0.1a0/README.md
--rw-r--r--   0 pierre    (1000) pierre    (1000)      637 2023-05-29 18:54:05.291263 dktoparserhtml-1.0.1a0/setup.cfg
--rw-r--r--   0 pierre    (1000) pierre    (1000)      347 2023-05-29 15:44:08.000000 dktoparserhtml-1.0.1a0/setup.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:54:05.275263 dktoparserhtml-1.0.1a0/src/
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:54:05.279263 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1844 2023-05-29 18:54:05.000000 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)      505 2023-05-29 18:54:05.000000 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-05-29 18:54:05.000000 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       91 2023-05-29 18:54:05.000000 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       11 2023-05-29 18:54:05.000000 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/top_level.txt
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:54:05.291263 dktoparserhtml-1.0.1a0/src/parserhtml/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3410 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1576 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_html_to_markdown.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_html_to_utf8.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2054 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_recurs_function.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      998 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_remove_duplicates.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4828 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_simplify_html.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1299 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_utf8_to_html.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      573 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/remove_duplicates.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 19:08:29.595557 dktoparserhtml-1.0.1b0/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1844 2023-05-29 19:08:29.595557 dktoparserhtml-1.0.1b0/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1057 2023-05-29 18:26:00.000000 dktoparserhtml-1.0.1b0/README.md
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      641 2023-05-29 19:08:29.599557 dktoparserhtml-1.0.1b0/setup.cfg
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      347 2023-05-29 15:44:08.000000 dktoparserhtml-1.0.1b0/setup.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 19:08:29.567559 dktoparserhtml-1.0.1b0/src/
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 19:08:29.587558 dktoparserhtml-1.0.1b0/src/dktoparserhtml/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3410 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1576 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml/_html_to_markdown.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml/_html_to_utf8.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2054 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml/_recurs_function.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      998 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml/_remove_duplicates.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4828 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml/_simplify_html.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1299 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml/_utf8_to_html.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      573 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml/remove_duplicates.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 19:08:29.595557 dktoparserhtml-1.0.1b0/src/dktoparserhtml.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1844 2023-05-29 19:08:29.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      537 2023-05-29 19:08:29.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-05-29 19:08:29.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       91 2023-05-29 19:08:29.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       15 2023-05-29 19:08:29.000000 dktoparserhtml-1.0.1b0/src/dktoparserhtml.egg-info/top_level.txt
```

### Comparing `dktoparserhtml-1.0.1a0/PKG-INFO` & `dktoparserhtml-1.0.1b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dktoparserhtml
-Version: 1.0.1a0
+Version: 1.0.1b0
 Summary: Parser UTF8/HTML <-> pure HTML -> UTF8/Markdown
 Home-page: https://discord-catho.frama.io/parserhtml/
 Author: Pierre
 License: UNKNOWN
 Project-URL: Source Code, https://framagit.org/discord-catho/parserhtml
 Description: # Description
         Transformer de l'utf8 en HTML et de l'HTML en Markdown principalement.
```

### Comparing `dktoparserhtml-1.0.1a0/README.md` & `dktoparserhtml-1.0.1b0/README.md`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.1a0/setup.cfg` & `dktoparserhtml-1.0.1b0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = dktoparserhtml
-version = 1.0.1a
+version = 1.0.1b
 author = Pierre
 description = Parser UTF8/HTML <-> pure HTML -> UTF8/Markdown
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://discord-catho.frama.io/parserhtml/
 project_urls = 
 	Source Code = https://framagit.org/discord-catho/parserhtml
@@ -12,15 +12,15 @@
 
 [options]
 python_requires = >=3.9, <4
 install_requires = 
 	bs4==0.0.1
 package_dir = 
 	=src
-packages = parserhtml
+packages = dktoparserhtml
 
 [options.extras_require]
 doc = 
 	sphinx==6.2.1
 	sphinx-rtd-theme==1.2.1
 	myst-parser==1.0.0
 tests =
```

### Comparing `dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/PKG-INFO` & `dktoparserhtml-1.0.1b0/src/dktoparserhtml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dktoparserhtml
-Version: 1.0.1a0
+Version: 1.0.1b0
 Summary: Parser UTF8/HTML <-> pure HTML -> UTF8/Markdown
 Home-page: https://discord-catho.frama.io/parserhtml/
 Author: Pierre
 License: UNKNOWN
 Project-URL: Source Code, https://framagit.org/discord-catho/parserhtml
 Description: # Description
         Transformer de l'utf8 en HTML et de l'HTML en Markdown principalement.
```

### Comparing `dktoparserhtml-1.0.1a0/src/parserhtml/__init__.py` & `dktoparserhtml-1.0.1b0/src/dktoparserhtml/__init__.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.1a0/src/parserhtml/_html_to_markdown.py` & `dktoparserhtml-1.0.1b0/src/dktoparserhtml/_html_to_markdown.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.1a0/src/parserhtml/_html_to_utf8.py` & `dktoparserhtml-1.0.1b0/src/dktoparserhtml/_html_to_utf8.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.1a0/src/parserhtml/_recurs_function.py` & `dktoparserhtml-1.0.1b0/src/dktoparserhtml/_recurs_function.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.1a0/src/parserhtml/_remove_duplicates.py` & `dktoparserhtml-1.0.1b0/src/dktoparserhtml/_remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.1a0/src/parserhtml/_simplify_html.py` & `dktoparserhtml-1.0.1b0/src/dktoparserhtml/_simplify_html.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.1a0/src/parserhtml/_utf8_to_html.py` & `dktoparserhtml-1.0.1b0/src/dktoparserhtml/_utf8_to_html.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.1a0/src/parserhtml/remove_duplicates.py` & `dktoparserhtml-1.0.1b0/src/dktoparserhtml/remove_duplicates.py`

 * *Files identical despite different names*


# Comparing `tmp/dktoparserhtml-1.0.0.tar.gz` & `tmp/dktoparserhtml-1.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dktoparserhtml-1.0.0.tar", last modified: Mon May 29 18:22:12 2023, max compression
+gzip compressed data, was "dktoparserhtml-1.0.1a0.tar", last modified: Mon May 29 18:54:05 2023, max compression
```

## Comparing `dktoparserhtml-1.0.0.tar` & `dktoparserhtml-1.0.1a0.tar`

### file list

```diff
@@ -1,23 +1,21 @@
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:22:12.664260 dktoparserhtml-1.0.0/
--rw-r--r--   0 pierre    (1000) pierre    (1000)    34487 2023-05-29 18:00:49.000000 dktoparserhtml-1.0.0/LICENSE
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1366 2023-05-29 18:22:12.664260 dktoparserhtml-1.0.0/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)      943 2023-05-29 18:21:07.000000 dktoparserhtml-1.0.0/README.md
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:22:12.656261 dktoparserhtml-1.0.0/dktoparserhtml.egg-info/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1366 2023-05-29 18:22:12.000000 dktoparserhtml-1.0.0/dktoparserhtml.egg-info/PKG-INFO
--rw-r--r--   0 pierre    (1000) pierre    (1000)      487 2023-05-29 18:22:12.000000 dktoparserhtml-1.0.0/dktoparserhtml.egg-info/SOURCES.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-05-29 18:22:12.000000 dktoparserhtml-1.0.0/dktoparserhtml.egg-info/dependency_links.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       91 2023-05-29 18:22:12.000000 dktoparserhtml-1.0.0/dktoparserhtml.egg-info/requires.txt
--rw-r--r--   0 pierre    (1000) pierre    (1000)       11 2023-05-29 18:22:12.000000 dktoparserhtml-1.0.0/dktoparserhtml.egg-info/top_level.txt
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:22:12.660261 dktoparserhtml-1.0.0/parserhtml/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     3410 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.0/parserhtml/__init__.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1576 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.0/parserhtml/_html_to_markdown.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.0/parserhtml/_html_to_utf8.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     2054 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.0/parserhtml/_recurs_function.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      998 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.0/parserhtml/_remove_duplicates.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     4828 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.0/parserhtml/_simplify_html.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1299 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.0/parserhtml/_utf8_to_html.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      573 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.0/parserhtml/remove_duplicates.py
--rw-r--r--   0 pierre    (1000) pierre    (1000)      593 2023-05-29 18:22:12.664260 dktoparserhtml-1.0.0/setup.cfg
--rw-r--r--   0 pierre    (1000) pierre    (1000)      347 2023-05-29 15:44:08.000000 dktoparserhtml-1.0.0/setup.py
-drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:22:12.664260 dktoparserhtml-1.0.0/tests/
--rw-r--r--   0 pierre    (1000) pierre    (1000)     1733 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.0/tests/test_html_parser.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:54:05.291263 dktoparserhtml-1.0.1a0/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1844 2023-05-29 18:54:05.291263 dktoparserhtml-1.0.1a0/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1057 2023-05-29 18:26:00.000000 dktoparserhtml-1.0.1a0/README.md
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      637 2023-05-29 18:54:05.291263 dktoparserhtml-1.0.1a0/setup.cfg
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      347 2023-05-29 15:44:08.000000 dktoparserhtml-1.0.1a0/setup.py
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:54:05.275263 dktoparserhtml-1.0.1a0/src/
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:54:05.279263 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1844 2023-05-29 18:54:05.000000 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/PKG-INFO
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      505 2023-05-29 18:54:05.000000 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/SOURCES.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)        1 2023-05-29 18:54:05.000000 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/dependency_links.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       91 2023-05-29 18:54:05.000000 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/requires.txt
+-rw-r--r--   0 pierre    (1000) pierre    (1000)       11 2023-05-29 18:54:05.000000 dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/top_level.txt
+drwxr-xr-x   0 pierre    (1000) pierre    (1000)        0 2023-05-29 18:54:05.291263 dktoparserhtml-1.0.1a0/src/parserhtml/
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     3410 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/__init__.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1576 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_html_to_markdown.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      773 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_html_to_utf8.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     2054 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_recurs_function.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      998 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_remove_duplicates.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     4828 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_simplify_html.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)     1299 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/_utf8_to_html.py
+-rw-r--r--   0 pierre    (1000) pierre    (1000)      573 2023-05-29 13:07:51.000000 dktoparserhtml-1.0.1a0/src/parserhtml/remove_duplicates.py
```

### Comparing `dktoparserhtml-1.0.0/PKG-INFO` & `dktoparserhtml-1.0.1a0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 Metadata-Version: 2.1
 Name: dktoparserhtml
-Version: 1.0.0
+Version: 1.0.1a0
 Summary: Parser UTF8/HTML <-> pure HTML -> UTF8/Markdown
 Home-page: https://discord-catho.frama.io/parserhtml/
 Author: Pierre
+License: UNKNOWN
 Project-URL: Source Code, https://framagit.org/discord-catho/parserhtml
+Description: # Description
+        Transformer de l'utf8 en HTML et de l'HTML en Markdown principalement.
+        Utile pour plusieurs projets, donc création d'un repo séparé, qui sera ensuite appelé en tant que sous-module.
+        
+        # Installation
+        Module bs4 à installer :
+        ```
+        $ python -m venv env_module
+        $ source env_module/bin/activate
+        $ pip3 install -r requirements.txt
+        ```
+        
+        # Utilisation
+        ## Via pip
+        ```
+        $ pip install dktoparserhtml
+        ```
+        
+        ## Comme submodule
+        ```
+        $ cd /path/superprojet
+        $ mkdir -p scripts/external && cd scripts/external
+        $ git submodule add git@framagit.org:discord-catho/parserhtml.git
+        $ git submodule update --recursive --init
+        $ git submodule update --recursive --remote
+        
+        ```
+        
+        # Documentation
+        ## Version en ligne :
+        http://discord-catho.frama.io/parserhtml
+        
+        ## Installation locale
+        * Il faut les librairies Python :`sphinx`, `sphinx-rtd-theme` et `myst-parser`
+        * Compris dans le fichier requirements.txt (voir la section Installation)
+        
+        
+        # Liens :
+        * git : https://framagit.org/discord-catho/parserhtml
+        * Pypi : https://pypi.org/project/dktoparserhtml
+        
+        # Licence
+        GNU AGPL 3
 Keywords: parser,html,utf8,markdown
+Platform: UNKNOWN
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: tests
-License-File: LICENSE
-
-# Description
-Transformer de l'utf8 en HTML et de l'HTML en Markdown principalement.
-Utile pour plusieurs projets, donc création d'un repo séparé, qui sera ensuite appelé en tant que sous-module.
-
-# Installation
-Module bs4 à installer :
-```
-$ python -m venv env_module
-$ source env_module/bin/activate
-$ pip3 install -r requirements.txt
-```
-
-# Utilisation
-## Via pip
-```
-$ pip install dktoparserhtml
-```
-
-## Comme submodule
-```
-$ cd /path/superprojet
-$ mkdir -p scripts/external && cd scripts/external
-$ git submodule add git@framagit.org:discord-catho/parserhtml.git
-$ git submodule update --recursive --init
-$ git submodule update --recursive --remote
-
-```
-
-# Documentation
-## Version en ligne :
-http://discord-catho.frama.io/parserhtml
-
-## Installation locale
-* Il faut les librairies Python :`sphinx`, `sphinx-rtd-theme` et `myst-parser`
-* Compris dans le fichier requirements.txt (voir la section Installation)
-
-
-
-# Licence
-GNU AGPL
```

### Comparing `dktoparserhtml-1.0.0/dktoparserhtml.egg-info/PKG-INFO` & `dktoparserhtml-1.0.1a0/src/dktoparserhtml.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,57 @@
 Metadata-Version: 2.1
 Name: dktoparserhtml
-Version: 1.0.0
+Version: 1.0.1a0
 Summary: Parser UTF8/HTML <-> pure HTML -> UTF8/Markdown
 Home-page: https://discord-catho.frama.io/parserhtml/
 Author: Pierre
+License: UNKNOWN
 Project-URL: Source Code, https://framagit.org/discord-catho/parserhtml
+Description: # Description
+        Transformer de l'utf8 en HTML et de l'HTML en Markdown principalement.
+        Utile pour plusieurs projets, donc création d'un repo séparé, qui sera ensuite appelé en tant que sous-module.
+        
+        # Installation
+        Module bs4 à installer :
+        ```
+        $ python -m venv env_module
+        $ source env_module/bin/activate
+        $ pip3 install -r requirements.txt
+        ```
+        
+        # Utilisation
+        ## Via pip
+        ```
+        $ pip install dktoparserhtml
+        ```
+        
+        ## Comme submodule
+        ```
+        $ cd /path/superprojet
+        $ mkdir -p scripts/external && cd scripts/external
+        $ git submodule add git@framagit.org:discord-catho/parserhtml.git
+        $ git submodule update --recursive --init
+        $ git submodule update --recursive --remote
+        
+        ```
+        
+        # Documentation
+        ## Version en ligne :
+        http://discord-catho.frama.io/parserhtml
+        
+        ## Installation locale
+        * Il faut les librairies Python :`sphinx`, `sphinx-rtd-theme` et `myst-parser`
+        * Compris dans le fichier requirements.txt (voir la section Installation)
+        
+        
+        # Liens :
+        * git : https://framagit.org/discord-catho/parserhtml
+        * Pypi : https://pypi.org/project/dktoparserhtml
+        
+        # Licence
+        GNU AGPL 3
 Keywords: parser,html,utf8,markdown
+Platform: UNKNOWN
 Requires-Python: <4,>=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: tests
-License-File: LICENSE
-
-# Description
-Transformer de l'utf8 en HTML et de l'HTML en Markdown principalement.
-Utile pour plusieurs projets, donc création d'un repo séparé, qui sera ensuite appelé en tant que sous-module.
-
-# Installation
-Module bs4 à installer :
-```
-$ python -m venv env_module
-$ source env_module/bin/activate
-$ pip3 install -r requirements.txt
-```
-
-# Utilisation
-## Via pip
-```
-$ pip install dktoparserhtml
-```
-
-## Comme submodule
-```
-$ cd /path/superprojet
-$ mkdir -p scripts/external && cd scripts/external
-$ git submodule add git@framagit.org:discord-catho/parserhtml.git
-$ git submodule update --recursive --init
-$ git submodule update --recursive --remote
-
-```
-
-# Documentation
-## Version en ligne :
-http://discord-catho.frama.io/parserhtml
-
-## Installation locale
-* Il faut les librairies Python :`sphinx`, `sphinx-rtd-theme` et `myst-parser`
-* Compris dans le fichier requirements.txt (voir la section Installation)
-
-
-
-# Licence
-GNU AGPL
```

### Comparing `dktoparserhtml-1.0.0/parserhtml/__init__.py` & `dktoparserhtml-1.0.1a0/src/parserhtml/__init__.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.0/parserhtml/_html_to_markdown.py` & `dktoparserhtml-1.0.1a0/src/parserhtml/_html_to_markdown.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.0/parserhtml/_html_to_utf8.py` & `dktoparserhtml-1.0.1a0/src/parserhtml/_html_to_utf8.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.0/parserhtml/_recurs_function.py` & `dktoparserhtml-1.0.1a0/src/parserhtml/_recurs_function.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.0/parserhtml/_remove_duplicates.py` & `dktoparserhtml-1.0.1a0/src/parserhtml/_remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.0/parserhtml/_simplify_html.py` & `dktoparserhtml-1.0.1a0/src/parserhtml/_simplify_html.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.0/parserhtml/_utf8_to_html.py` & `dktoparserhtml-1.0.1a0/src/parserhtml/_utf8_to_html.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.0/parserhtml/remove_duplicates.py` & `dktoparserhtml-1.0.1a0/src/parserhtml/remove_duplicates.py`

 * *Files identical despite different names*

### Comparing `dktoparserhtml-1.0.0/setup.cfg` & `dktoparserhtml-1.0.1a0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [metadata]
 name = dktoparserhtml
-version = 1.0.0
+version = 1.0.1a
 author = Pierre
 description = Parser UTF8/HTML <-> pure HTML -> UTF8/Markdown
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://discord-catho.frama.io/parserhtml/
 project_urls = 
 	Source Code = https://framagit.org/discord-catho/parserhtml
 keywords = parser, html, utf8, markdown
 
 [options]
 python_requires = >=3.9, <4
 install_requires = 
 	bs4==0.0.1
+package_dir = 
+	=src
+packages = parserhtml
 
 [options.extras_require]
 doc = 
 	sphinx==6.2.1
 	sphinx-rtd-theme==1.2.1
 	myst-parser==1.0.0
 tests =
```


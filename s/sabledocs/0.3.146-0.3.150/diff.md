# Comparing `tmp/sabledocs-0.3.146.tar.gz` & `tmp/sabledocs-0.3.150.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.3.146.tar", last modified: Mon May 29 13:50:43 2023, max compression
+gzip compressed data, was "sabledocs-0.3.150.tar", last modified: Mon May 29 16:48:22 2023, max compression
```

## Comparing `sabledocs-0.3.146.tar` & `sabledocs-0.3.150.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 13:50:43.446899 sabledocs-0.3.146/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-05-29 13:50:30.000000 sabledocs-0.3.146/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-05-29 13:50:30.000000 sabledocs-0.3.146/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4702 2023-05-29 13:50:43.446899 sabledocs-0.3.146/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4162 2023-05-29 13:50:30.000000 sabledocs-0.3.146/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-29 13:50:30.000000 sabledocs-0.3.146/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-05-29 13:50:43.446899 sabledocs-0.3.146/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 13:50:43.438899 sabledocs-0.3.146/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 13:50:43.442899 sabledocs-0.3.146/src/sabledocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3346 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/lunr_search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13645 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 13:50:43.438899 sabledocs-0.3.146/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 13:50:43.446899 sabledocs-0.3.146/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2582 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/templates/_default/search.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 13:50:43.446899 sabledocs-0.3.146/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   257784 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-05-29 13:50:30.000000 sabledocs-0.3.146/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 13:50:43.442899 sabledocs-0.3.146/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4702 2023-05-29 13:50:43.000000 sabledocs-0.3.146/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-05-29 13:50:43.000000 sabledocs-0.3.146/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-29 13:50:43.000000 sabledocs-0.3.146/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-29 13:50:43.000000 sabledocs-0.3.146/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-05-29 13:50:43.000000 sabledocs-0.3.146/src/sabledocs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-05-29 13:50:43.000000 sabledocs-0.3.146/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 16:48:22.330278 sabledocs-0.3.150/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-05-29 16:48:09.000000 sabledocs-0.3.150/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-05-29 16:48:09.000000 sabledocs-0.3.150/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4800 2023-05-29 16:48:22.330278 sabledocs-0.3.150/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4260 2023-05-29 16:48:09.000000 sabledocs-0.3.150/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-29 16:48:09.000000 sabledocs-0.3.150/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-05-29 16:48:22.330278 sabledocs-0.3.150/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 16:48:22.326278 sabledocs-0.3.150/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 16:48:22.330278 sabledocs-0.3.150/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3346 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2109 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/lunr_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13645 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 16:48:22.326278 sabledocs-0.3.150/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 16:48:22.330278 sabledocs-0.3.150/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2582 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/templates/_default/search.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 16:48:22.330278 sabledocs-0.3.150/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   257784 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-05-29 16:48:09.000000 sabledocs-0.3.150/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 16:48:22.330278 sabledocs-0.3.150/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4800 2023-05-29 16:48:22.000000 sabledocs-0.3.150/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-05-29 16:48:22.000000 sabledocs-0.3.150/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-29 16:48:22.000000 sabledocs-0.3.150/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-29 16:48:22.000000 sabledocs-0.3.150/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-05-29 16:48:22.000000 sabledocs-0.3.150/src/sabledocs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-05-29 16:48:22.000000 sabledocs-0.3.150/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.3.146/LICENSE` & `sabledocs-0.3.150/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/PKG-INFO` & `sabledocs-0.3.150/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.3.146
+Version: 0.3.150
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
 
 *(It's important to use the `--include_source_info` flag, otherwise the comments will not be included in the generated documentation.)*
 
 The generated `descriptor.pb` file will be the input needed to build the documentation site.
 
 ### Build the documetation
 
-Install the `sabledocs` package.
+Install the `sabledocs` package. It requires [Python](https://www.python.org/downloads/) (version 3.11 or higher) to be installed.
 
 ```
 pip install sabledocs
 ```
 
 In the same folder where the generated `descriptor.pb` file is located, execute the command.
```

### Comparing `sabledocs-0.3.146/README.md` & `sabledocs-0.3.150/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 *(It's important to use the `--include_source_info` flag, otherwise the comments will not be included in the generated documentation.)*
 
 The generated `descriptor.pb` file will be the input needed to build the documentation site.
 
 ### Build the documetation
 
-Install the `sabledocs` package.
+Install the `sabledocs` package. It requires [Python](https://www.python.org/downloads/) (version 3.11 or higher) to be installed.
 
 ```
 pip install sabledocs
 ```
 
 In the same folder where the generated `descriptor.pb` file is located, execute the command.
```

### Comparing `sabledocs-0.3.146/pyproject.toml` & `sabledocs-0.3.150/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/__main__.py` & `sabledocs-0.3.150/src/sabledocs/__main__.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/lunr_search.py` & `sabledocs-0.3.150/src/sabledocs/lunr_search.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.3.150/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/proto_model.py` & `sabledocs-0.3.150/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/sable_config.py` & `sabledocs-0.3.150/src/sabledocs/sable_config.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/templates/_default/base.html` & `sabledocs-0.3.150/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.3.150/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/templates/_default/index.html` & `sabledocs-0.3.150/src/sabledocs/templates/_default/index.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/templates/_default/message.html` & `sabledocs-0.3.150/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/templates/_default/package.html` & `sabledocs-0.3.150/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/templates/_default/search.html` & `sabledocs-0.3.150/src/sabledocs/templates/_default/search.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/templates/_default/service.html` & `sabledocs-0.3.150/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.3.150/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.3.150/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.3.146/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.3.150/src/sabledocs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.3.146
+Version: 0.3.150
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,15 +36,15 @@
 
 *(It's important to use the `--include_source_info` flag, otherwise the comments will not be included in the generated documentation.)*
 
 The generated `descriptor.pb` file will be the input needed to build the documentation site.
 
 ### Build the documetation
 
-Install the `sabledocs` package.
+Install the `sabledocs` package. It requires [Python](https://www.python.org/downloads/) (version 3.11 or higher) to be installed.
 
 ```
 pip install sabledocs
 ```
 
 In the same folder where the generated `descriptor.pb` file is located, execute the command.
```

### Comparing `sabledocs-0.3.146/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.3.150/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


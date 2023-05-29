# Comparing `tmp/sabledocs-0.2.138.tar.gz` & `tmp/sabledocs-0.3.142.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sabledocs-0.2.138.tar", last modified: Thu May 18 16:00:31 2023, max compression
+gzip compressed data, was "sabledocs-0.3.142.dev0.tar", last modified: Mon May 29 12:54:33 2023, max compression
```

## Comparing `sabledocs-0.2.138.tar` & `sabledocs-0.3.142.dev0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.808618 sabledocs-0.2.138/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-05-18 16:00:18.000000 sabledocs-0.2.138/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-05-18 16:00:18.000000 sabledocs-0.2.138/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4117 2023-05-18 16:00:31.808618 sabledocs-0.2.138/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3577 2023-05-18 16:00:18.000000 sabledocs-0.2.138/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-18 16:00:18.000000 sabledocs-0.2.138/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       74 2023-05-18 16:00:31.808618 sabledocs-0.2.138/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.804618 sabledocs-0.2.138/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.808618 sabledocs-0.2.138/src/sabledocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2853 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2023 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/lunr_search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13645 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/proto_descriptor_parser.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/proto_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2088 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/sable_config.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.804618 sabledocs-0.2.138/src/sabledocs/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.808618 sabledocs-0.2.138/src/sabledocs/templates/_default/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/base.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/enum.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      528 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/index.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/message.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/package.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2582 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/search.html
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/service.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.808618 sabledocs-0.2.138/src/sabledocs/templates/_default/static/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   257784 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/static/mystyles.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-05-18 16:00:18.000000 sabledocs-0.2.138/src/sabledocs/templates/_default/type_name.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-18 16:00:31.808618 sabledocs-0.2.138/src/sabledocs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4117 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-05-18 16:00:31.000000 sabledocs-0.2.138/src/sabledocs.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 12:54:33.406640 sabledocs-0.3.142.dev0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1078 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       44 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4122 2023-05-29 12:54:33.406640 sabledocs-0.3.142.dev0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3577 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      877 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       77 2023-05-29 12:54:33.406640 sabledocs-0.3.142.dev0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 12:54:33.402639 sabledocs-0.3.142.dev0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 12:54:33.402639 sabledocs-0.3.142.dev0/src/sabledocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3346 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2023 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/lunr_search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13645 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/proto_descriptor_parser.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/proto_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2198 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/sable_config.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 12:54:33.402639 sabledocs-0.3.142.dev0/src/sabledocs/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 12:54:33.406640 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2242 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/base.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      826 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/enum.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      751 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/index.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1399 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/message.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1889 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/package.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2582 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/search.html
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/service.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 12:54:33.406640 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/static/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   257784 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/static/mystyles.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      560 2023-05-29 12:54:13.000000 sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/type_name.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-29 12:54:33.402639 sabledocs-0.3.142.dev0/src/sabledocs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4122 2023-05-29 12:54:33.000000 sabledocs-0.3.142.dev0/src/sabledocs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      873 2023-05-29 12:54:33.000000 sabledocs-0.3.142.dev0/src/sabledocs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-29 12:54:33.000000 sabledocs-0.3.142.dev0/src/sabledocs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-05-29 12:54:33.000000 sabledocs-0.3.142.dev0/src/sabledocs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-05-29 12:54:33.000000 sabledocs-0.3.142.dev0/src/sabledocs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2023-05-29 12:54:33.000000 sabledocs-0.3.142.dev0/src/sabledocs.egg-info/top_level.txt
```

### Comparing `sabledocs-0.2.138/LICENSE` & `sabledocs-0.3.142.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/PKG-INFO` & `sabledocs-0.3.142.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.2.138
+Version: 0.3.142.dev0
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.2.138/README.md` & `sabledocs-0.3.142.dev0/README.md`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/pyproject.toml` & `sabledocs-0.3.142.dev0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sabledocs"
-version = "0.2"
+version = "0.3"
 authors = [
   { name="Mark Vincze", email="mrk.vincze@gmail.com" },
 ]
 description = "Static documentation generator for Protobuf and gRPC"
 readme = "README.md"
 requires-python = ">=3.11.0"
 dependencies = [
```

### Comparing `sabledocs-0.2.138/src/sabledocs/lunr_search.py` & `sabledocs-0.3.142.dev0/src/sabledocs/lunr_search.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs/proto_descriptor_parser.py` & `sabledocs-0.3.142.dev0/src/sabledocs/proto_descriptor_parser.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs/proto_model.py` & `sabledocs-0.3.142.dev0/src/sabledocs/proto_model.py`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs/sable_config.py` & `sabledocs-0.3.142.dev0/src/sabledocs/sable_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class SableConfig:
     def __init__(self, config_file_path):
         self.module_title = "Protobuf module documentation"
         self.input_descriptor_file = "descriptor.pb"
         self.template = "_default"
         self.footer_content = ""
+        self.main_page_content_file = ""
         self.output_dir = "sabledocs_output"
         self.enable_lunr_search = True
         self.repository_url = ""
         self.repository_branch = ""
         self.repository_type = RepositoryType.NONE
 
         if path.exists(config_file_path):
@@ -30,24 +31,25 @@
 
                 self.input_descriptor_file = config_values.get('input-descriptor-file', self.input_descriptor_file)
 
                 self.template = config_values.get('template', self.template).rstrip("/\\")
 
                 self.footer_content = config_values.get('footer-content', self.footer_content)
 
+                self.main_page_content_file = config_values.get('main-page-content-file', self.main_page_content_file)
+
                 self.output_dir = config_values.get('output-dir', self.output_dir).rstrip("/\\")
 
                 self.enable_lunr_search = config_values.get('enable-lunr-search', True)
 
                 self.repository_url = config_values.get('repository-url', self.repository_url)
 
                 self.repository_branch = config_values.get('repository-branch', self.repository_branch)
 
                 if 'repository-type' in config_values:
-                    print("repository-type found")
                     match config_values['repository-type']:
                         case 'github':
                             self.repository_type = RepositoryType.GITHUB
                         case 'bitbucket':
                             self.repository_type = RepositoryType.BITBUCKET
         else:
             print("sabledocs.toml file not found, using default configuration.")
```

### Comparing `sabledocs-0.2.138/src/sabledocs/templates/_default/base.html` & `sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/base.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs/templates/_default/enum.html` & `sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/enum.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs/templates/_default/message.html` & `sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/message.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs/templates/_default/package.html` & `sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/package.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs/templates/_default/search.html` & `sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/search.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs/templates/_default/service.html` & `sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/service.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs/templates/_default/static/mystyles.css` & `sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/static/mystyles.css`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs/templates/_default/type_name.html` & `sabledocs-0.3.142.dev0/src/sabledocs/templates/_default/type_name.html`

 * *Files identical despite different names*

### Comparing `sabledocs-0.2.138/src/sabledocs.egg-info/PKG-INFO` & `sabledocs-0.3.142.dev0/src/sabledocs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sabledocs
-Version: 0.2.138
+Version: 0.3.142.dev0
 Summary: Static documentation generator for Protobuf and gRPC
 Author-email: Mark Vincze <mrk.vincze@gmail.com>
 Project-URL: Homepage, https://github.com/markvincze/sabledocs
 Project-URL: Bug Tracker, https://github.com/markvincze/sabledocs/issues
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sabledocs-0.2.138/src/sabledocs.egg-info/SOURCES.txt` & `sabledocs-0.3.142.dev0/src/sabledocs.egg-info/SOURCES.txt`

 * *Files identical despite different names*


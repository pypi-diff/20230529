# Comparing `tmp/bloic-1.0.1.tar.gz` & `tmp/bloic-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloic-1.0.1.tar", last modified: Sun May 21 14:35:43 2023, max compression
+gzip compressed data, was "bloic-1.1.0.tar", last modified: Mon May 29 19:52:30 2023, max compression
```

## Comparing `bloic-1.0.1.tar` & `bloic-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 14:35:43.157767 bloic-1.0.1/
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-05-21 14:35:34.000000 bloic-1.0.1/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      887 2023-05-21 14:35:34.000000 bloic-1.0.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1337 2023-05-21 14:35:34.000000 bloic-1.0.1/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-21 14:35:34.000000 bloic-1.0.1/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-21 14:35:34.000000 bloic-1.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2303 2023-05-21 14:35:43.156767 bloic-1.0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1692 2023-05-21 14:35:34.000000 bloic-1.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 14:35:43.155767 bloic-1.0.1/bloic/
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-21 14:35:34.000000 bloic-1.0.1/bloic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-21 14:35:34.000000 bloic-1.0.1/bloic/__main__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1924 2023-05-21 14:35:34.000000 bloic-1.0.1/bloic/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 14:35:43.156767 bloic-1.0.1/bloic.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2303 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       56 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      934 2023-05-21 14:35:34.000000 bloic-1.0.1/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-21 14:35:34.000000 bloic-1.0.1/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 14:35:43.157767 bloic-1.0.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:52:30.985868 bloic-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)      805 2023-05-29 19:52:21.000000 bloic-1.1.0/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-05-29 19:52:21.000000 bloic-1.1.0/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     2045 2023-05-29 19:52:21.000000 bloic-1.1.0/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      466 2023-05-29 19:52:21.000000 bloic-1.1.0/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-29 19:52:21.000000 bloic-1.1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-29 19:52:21.000000 bloic-1.1.0/Makefile
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-05-29 19:52:30.985868 bloic-1.1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2023-05-29 19:52:21.000000 bloic-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:52:30.983868 bloic-1.1.0/bloic/
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-29 19:52:21.000000 bloic-1.1.0/bloic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-29 19:52:21.000000 bloic-1.1.0/bloic/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-29 19:52:30.000000 bloic-1.1.0/bloic/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1924 2023-05-29 19:52:21.000000 bloic-1.1.0/bloic/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-29 19:52:30.984867 bloic-1.1.0/bloic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-05-29 19:52:30.000000 bloic-1.1.0/bloic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      359 2023-05-29 19:52:30.000000 bloic-1.1.0/bloic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-29 19:52:30.000000 bloic-1.1.0/bloic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-29 19:52:30.000000 bloic-1.1.0/bloic.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-29 19:52:30.000000 bloic-1.1.0/bloic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-29 19:52:30.000000 bloic-1.1.0/bloic.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-05-29 19:52:21.000000 bloic-1.1.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-29 19:52:21.000000 bloic-1.1.0/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-29 19:52:30.985868 bloic-1.1.0/setup.cfg
```

### Comparing `bloic-1.0.1/.dockerignore` & `bloic-1.1.0/.dockerignore`

 * *Files 12% similar despite different names*

```diff
@@ -56,15 +56,14 @@
 .DS_Store
 
 # Editors
 .vscode/
 .idea/
 
 # Git
-.git
 .gitlab-ci.yml
 .gitignore
 
 # Docker
 Dockerfile
 .dockerignore
```

### Comparing `bloic-1.0.1/.gitignore` & `bloic-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bloic-1.0.1/LICENSE` & `bloic-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bloic-1.0.1/PKG-INFO` & `bloic-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloic
-Version: 1.0.1
+Version: 1.1.0
 Summary: Tool to convert and resize image for blog post.
 Author: romaiiiiinnn
 License: MIT
 Project-URL: Homepage, https://gitlab.com/romaiiiinnn/blog-post-image-converter
 Project-URL: Bug Tracker, https://gitlab.com/romaiiiinnn/blog-post-image-converter/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
```

### Comparing `bloic-1.0.1/README.md` & `bloic-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `bloic-1.0.1/bloic/entrypoint.py` & `bloic-1.1.0/bloic/entrypoint.py`

 * *Files identical despite different names*

### Comparing `bloic-1.0.1/bloic.egg-info/PKG-INFO` & `bloic-1.1.0/bloic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloic
-Version: 1.0.1
+Version: 1.1.0
 Summary: Tool to convert and resize image for blog post.
 Author: romaiiiiinnn
 License: MIT
 Project-URL: Homepage, https://gitlab.com/romaiiiinnn/blog-post-image-converter
 Project-URL: Bug Tracker, https://gitlab.com/romaiiiinnn/blog-post-image-converter/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
```

### Comparing `bloic-1.0.1/pyproject.toml` & `bloic-1.1.0/pyproject.toml`

 * *Files identical despite different names*


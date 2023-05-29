# Comparing `tmp/DI-toolkit-0.1.0.tar.gz` & `tmp/DI-toolkit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DI-toolkit-0.1.0.tar", last modified: Sun Nov 13 09:27:19 2022, max compression
+gzip compressed data, was "DI-toolkit-0.2.0.tar", last modified: Mon May 29 13:00:10 2023, max compression
```

## Comparing `DI-toolkit-0.1.0.tar` & `DI-toolkit-0.2.0.tar`

### file list

```diff
@@ -1,33 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-13 09:27:19.665291 DI-toolkit-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-13 09:27:19.661291 DI-toolkit-0.1.0/DI_toolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4500 2022-11-13 09:27:19.000000 DI-toolkit-0.1.0/DI_toolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      577 2022-11-13 09:27:19.000000 DI-toolkit-0.1.0/DI_toolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-11-13 09:27:19.000000 DI-toolkit-0.1.0/DI_toolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      487 2022-11-13 09:27:19.000000 DI-toolkit-0.1.0/DI_toolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        5 2022-11-13 09:27:19.000000 DI-toolkit-0.1.0/DI_toolkit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    11357 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      125 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     4500 2022-11-13 09:27:19.665291 DI-toolkit-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3449 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-13 09:27:19.661291 DI-toolkit-0.1.0/ditk/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-13 09:27:19.661291 DI-toolkit-0.1.0/ditk/config/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      455 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/config/meta.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-11-13 09:27:19.665291 DI-toolkit-0.1.0/ditk/logging/
--rw-r--r--   0 runner    (1001) docker     (116)      191 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       58 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/logging/base.py
--rw-r--r--   0 runner    (1001) docker     (116)      616 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/logging/explicit.py
--rw-r--r--   0 runner    (1001) docker     (116)     1385 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/logging/file.py
--rw-r--r--   0 runner    (1001) docker     (116)     3051 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/logging/func.py
--rw-r--r--   0 runner    (1001) docker     (116)      354 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/logging/inherit.py
--rw-r--r--   0 runner    (1001) docker     (116)     2274 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/logging/log.py
--rw-r--r--   0 runner    (1001) docker     (116)      977 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/logging/rich.py
--rw-r--r--   0 runner    (1001) docker     (116)      843 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/logging/stream.py
--rw-r--r--   0 runner    (1001) docker     (116)     1526 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/ditk/logging/terminal.py
--rw-r--r--   0 runner    (1001) docker     (116)      164 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/requirements-doc.txt
--rw-r--r--   0 runner    (1001) docker     (116)       25 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/requirements-style.txt
--rw-r--r--   0 runner    (1001) docker     (116)      244 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (116)       28 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2022-11-13 09:27:19.665291 DI-toolkit-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2157 2022-11-13 09:26:47.000000 DI-toolkit-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:00:10.454521 DI-toolkit-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:00:10.438521 DI-toolkit-0.2.0/DI_toolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-29 13:00:10.000000 DI-toolkit-0.2.0/DI_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-29 13:00:10.000000 DI-toolkit-0.2.0/DI_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 13:00:10.000000 DI-toolkit-0.2.0/DI_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-29 13:00:10.000000 DI-toolkit-0.2.0/DI_toolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 13:00:10.000000 DI-toolkit-0.2.0/DI_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-29 13:00:10.454521 DI-toolkit-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:00:10.438521 DI-toolkit-0.2.0/ditk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:00:10.438521 DI-toolkit-0.2.0/ditk/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/config/meta.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:00:10.438521 DI-toolkit-0.2.0/ditk/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/doc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:00:10.442521 DI-toolkit-0.2.0/ditk/doc/annotated/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/doc/annotated/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/doc/annotated/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10487 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/doc/annotated/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/doc/annotated/ppo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32206 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/doc/annotated/pylit.css
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/doc/annotated/solarized.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:00:10.446521 DI-toolkit-0.2.0/ditk/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/logging/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/logging/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/logging/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/logging/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/logging/inherit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/logging/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/logging/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/logging/stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/logging/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:00:10.446521 DI-toolkit-0.2.0/ditk/tensorboard/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/tensorboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/tensorboard/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 13:00:10.454521 DI-toolkit-0.2.0/ditk/tensorboard/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/tensorboard/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4290 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/ditk/tensorboard/plots/range.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/requirements-style.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 13:00:10.454521 DI-toolkit-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-05-29 12:57:09.000000 DI-toolkit-0.2.0/setup.py
```

### Comparing `DI-toolkit-0.1.0/DI_toolkit.egg-info/SOURCES.txt` & `DI-toolkit-0.2.0/DI_toolkit.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -10,17 +10,28 @@
 DI_toolkit.egg-info/SOURCES.txt
 DI_toolkit.egg-info/dependency_links.txt
 DI_toolkit.egg-info/requires.txt
 DI_toolkit.egg-info/top_level.txt
 ditk/__init__.py
 ditk/config/__init__.py
 ditk/config/meta.py
+ditk/doc/__init__.py
+ditk/doc/annotated/__init__.py
+ditk/doc/annotated/__main__.py
+ditk/doc/annotated/generate.py
+ditk/doc/annotated/ppo.py
+ditk/doc/annotated/pylit.css
+ditk/doc/annotated/solarized.css
 ditk/logging/__init__.py
 ditk/logging/base.py
 ditk/logging/explicit.py
 ditk/logging/file.py
 ditk/logging/func.py
 ditk/logging/inherit.py
 ditk/logging/log.py
 ditk/logging/rich.py
 ditk/logging/stream.py
-ditk/logging/terminal.py
+ditk/logging/terminal.py
+ditk/tensorboard/__init__.py
+ditk/tensorboard/log.py
+ditk/tensorboard/plots/__init__.py
+ditk/tensorboard/plots/range.py
```

### Comparing `DI-toolkit-0.1.0/LICENSE` & `DI-toolkit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `DI-toolkit-0.1.0/ditk/logging/explicit.py` & `DI-toolkit-0.2.0/ditk/logging/explicit.py`

 * *Files identical despite different names*

### Comparing `DI-toolkit-0.1.0/ditk/logging/file.py` & `DI-toolkit-0.2.0/ditk/logging/file.py`

 * *Files identical despite different names*

### Comparing `DI-toolkit-0.1.0/ditk/logging/func.py` & `DI-toolkit-0.2.0/ditk/logging/func.py`

 * *Files identical despite different names*

### Comparing `DI-toolkit-0.1.0/ditk/logging/log.py` & `DI-toolkit-0.2.0/ditk/logging/log.py`

 * *Files identical despite different names*

### Comparing `DI-toolkit-0.1.0/ditk/logging/rich.py` & `DI-toolkit-0.2.0/ditk/logging/rich.py`

 * *Files identical despite different names*

### Comparing `DI-toolkit-0.1.0/ditk/logging/stream.py` & `DI-toolkit-0.2.0/ditk/logging/stream.py`

 * *Files identical despite different names*

### Comparing `DI-toolkit-0.1.0/ditk/logging/terminal.py` & `DI-toolkit-0.2.0/ditk/logging/terminal.py`

 * *Files identical despite different names*

### Comparing `DI-toolkit-0.1.0/setup.py` & `DI-toolkit-0.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     readme = f.read()
 
 setup(
     # information
     name=meta['__TITLE__'],
     version=meta['__VERSION__'],
     packages=find_packages(include=(_package_name, "%s.*" % _package_name)),
-    package_data={package_name: ['*.yaml', '*.yml']
+    package_data={package_name: ['*.yaml', '*.yml', '*.css', '*.js']
                   for package_name in find_packages(include=('*'))},
     description=meta['__DESCRIPTION__'],
     long_description=readme,
     long_description_content_type='text/markdown',
     author=meta['__AUTHOR__'],
     author_email=meta['__AUTHOR_EMAIL__'],
     license='Apache License, Version 2.0',
```


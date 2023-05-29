# Comparing `tmp/backgroundremover-0.2.2.tar.gz` & `tmp/backgroundremover-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/backgroundremover-0.2.2.tar", last modified: Tue May 16 04:26:44 2023, max compression
+gzip compressed data, was "dist/backgroundremover-0.2.3.tar", last modified: Mon May 29 01:29:12 2023, max compression
```

## Comparing `backgroundremover-0.2.2.tar` & `backgroundremover-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/
--rw-rw-r--   0 john      (1000) john      (1000)     1171 2022-03-30 21:01:22.000000 backgroundremover-0.2.2/LICENSE.txt
--rw-rw-r--   0 john      (1000) john      (1000)      183 2022-03-30 21:01:22.000000 backgroundremover-0.2.2/MANIFEST.in
--rw-rw-r--   0 john      (1000) john      (1000)     8136 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)     6191 2023-05-15 23:12:59.000000 backgroundremover-0.2.2/README.md
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/backgroundremover/
--rw-rw-r--   0 john      (1000) john      (1000)      175 2023-05-16 04:22:05.000000 backgroundremover-0.2.2/backgroundremover/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     6962 2023-05-16 02:33:37.000000 backgroundremover-0.2.2/backgroundremover/bg.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/backgroundremover/cmd/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/cmd/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/cmd/cli.py
--rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/cmd/server.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/backgroundremover/u2net/
--rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/u2net/__init__.py
--rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/u2net/data_loader.py
--rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/u2net/detect.py
--rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-04-30 19:07:55.000000 backgroundremover-0.2.2/backgroundremover/u2net/u2net.py
--rw-rw-r--   0 john      (1000) john      (1000)    12628 2023-05-15 23:12:59.000000 backgroundremover-0.2.2/backgroundremover/utilities.py
-drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/backgroundremover.egg-info/
--rw-rw-r--   0 john      (1000) john      (1000)     8136 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/PKG-INFO
--rw-rw-r--   0 john      (1000) john      (1000)      654 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/SOURCES.txt
--rw-rw-r--   0 john      (1000) john      (1000)        1 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/dependency_links.txt
--rw-rw-r--   0 john      (1000) john      (1000)       70 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/entry_points.txt
--rw-rw-r--   0 john      (1000) john      (1000)      350 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/requires.txt
--rw-rw-r--   0 john      (1000) john      (1000)       18 2023-05-16 04:26:43.000000 backgroundremover-0.2.2/backgroundremover.egg-info/top_level.txt
--rw-rw-r--   0 john      (1000) john      (1000)      230 2022-03-30 21:01:23.000000 backgroundremover-0.2.2/pyproject.toml
--rw-rw-r--   0 john      (1000) john      (1000)      350 2023-05-06 14:07:42.000000 backgroundremover-0.2.2/requirements.txt
--rw-rw-r--   0 john      (1000) john      (1000)       78 2023-05-16 04:26:44.000000 backgroundremover-0.2.2/setup.cfg
--rw-rw-r--   0 john      (1000) john      (1000)     1027 2023-05-16 04:26:22.000000 backgroundremover-0.2.2/setup.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/
+-rw-rw-r--   0 john      (1000) john      (1000)     1171 2022-03-30 21:01:22.000000 backgroundremover-0.2.3/LICENSE.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      183 2022-03-30 21:01:22.000000 backgroundremover-0.2.3/MANIFEST.in
+-rw-rw-r--   0 john      (1000) john      (1000)     8136 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)     6191 2023-05-15 23:12:59.000000 backgroundremover-0.2.3/README.md
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover/
+-rw-rw-r--   0 john      (1000) john      (1000)      175 2023-05-29 01:28:23.000000 backgroundremover-0.2.3/backgroundremover/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     6964 2023-05-29 01:24:44.000000 backgroundremover-0.2.3/backgroundremover/bg.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover/cmd/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/cmd/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)     8314 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/cmd/cli.py
+-rw-rw-r--   0 john      (1000) john      (1000)     2717 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/cmd/server.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover/u2net/
+-rw-rw-r--   0 john      (1000) john      (1000)        0 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/u2net/__init__.py
+-rw-rw-r--   0 john      (1000) john      (1000)    11552 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/u2net/data_loader.py
+-rw-rw-r--   0 john      (1000) john      (1000)     4307 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/u2net/detect.py
+-rw-rw-r--   0 john      (1000) john      (1000)    15477 2023-04-30 19:07:55.000000 backgroundremover-0.2.3/backgroundremover/u2net/u2net.py
+-rw-rw-r--   0 john      (1000) john      (1000)    12628 2023-05-15 23:12:59.000000 backgroundremover-0.2.3/backgroundremover/utilities.py
+drwxrwxr-x   0 john      (1000) john      (1000)        0 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/
+-rw-rw-r--   0 john      (1000) john      (1000)     8136 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/PKG-INFO
+-rw-rw-r--   0 john      (1000) john      (1000)      654 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/SOURCES.txt
+-rw-rw-r--   0 john      (1000) john      (1000)        1 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/dependency_links.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       70 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/entry_points.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      350 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/requires.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       18 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/backgroundremover.egg-info/top_level.txt
+-rw-rw-r--   0 john      (1000) john      (1000)      230 2022-03-30 21:01:23.000000 backgroundremover-0.2.3/pyproject.toml
+-rw-rw-r--   0 john      (1000) john      (1000)      350 2023-05-06 14:07:42.000000 backgroundremover-0.2.3/requirements.txt
+-rw-rw-r--   0 john      (1000) john      (1000)       78 2023-05-29 01:29:12.000000 backgroundremover-0.2.3/setup.cfg
+-rw-rw-r--   0 john      (1000) john      (1000)     1027 2023-05-29 01:28:23.000000 backgroundremover-0.2.3/setup.py
```

### Comparing `backgroundremover-0.2.2/LICENSE.txt` & `backgroundremover-0.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.2/PKG-INFO` & `backgroundremover-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.2.2
+Version: 0.2.3
 Summary: Background remover from image and video using AI
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 License: UNKNOWN
 Description: # BackgroundRemover
         ![Background Remover](https://raw.githubusercontent.com/nadermx/backgroundremover/main/examplefiles/backgroundremoverexample.png)
```

### Comparing `backgroundremover-0.2.2/README.md` & `backgroundremover-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.2/backgroundremover/bg.py` & `backgroundremover-0.2.3/backgroundremover/bg.py`

 * *Files 0% similar despite different names*

```diff
@@ -124,15 +124,15 @@
     # guess likely foreground/background
     is_foreground = mask > foreground_threshold
     is_background = mask < background_threshold
 
     # erode foreground/background
     structure = None
     if erode_structure_size > 0:
-        structure = np.ones((erode_structure_size, erode_structure_size), dtype=np.int)
+        structure = np.ones((erode_structure_size, erode_structure_size), dtype=np.int64)
 
     is_foreground = binary_erosion(is_foreground, structure=structure)
     is_background = binary_erosion(is_background, structure=structure, border_value=1)
 
     # build trimap
     # 0   = background
     # 128 = unknown
```

### Comparing `backgroundremover-0.2.2/backgroundremover/cmd/cli.py` & `backgroundremover-0.2.3/backgroundremover/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.2/backgroundremover/cmd/server.py` & `backgroundremover-0.2.3/backgroundremover/cmd/server.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.2/backgroundremover/u2net/data_loader.py` & `backgroundremover-0.2.3/backgroundremover/u2net/data_loader.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.2/backgroundremover/u2net/detect.py` & `backgroundremover-0.2.3/backgroundremover/u2net/detect.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.2/backgroundremover/u2net/u2net.py` & `backgroundremover-0.2.3/backgroundremover/u2net/u2net.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.2/backgroundremover/utilities.py` & `backgroundremover-0.2.3/backgroundremover/utilities.py`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.2/backgroundremover.egg-info/PKG-INFO` & `backgroundremover-0.2.3/backgroundremover.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backgroundremover
-Version: 0.2.2
+Version: 0.2.3
 Summary: Background remover from image and video using AI
 Home-page: https://github.com/nadermx/backgroundremover
 Author: Johnathan Nader
 Author-email: john@nader.mx
 License: UNKNOWN
 Description: # BackgroundRemover
         ![Background Remover](https://raw.githubusercontent.com/nadermx/backgroundremover/main/examplefiles/backgroundremoverexample.png)
```

### Comparing `backgroundremover-0.2.2/backgroundremover.egg-info/SOURCES.txt` & `backgroundremover-0.2.3/backgroundremover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backgroundremover-0.2.2/setup.py` & `backgroundremover-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 with open("requirements.txt") as f:
     requireds = f.read().splitlines()
 
 setup(
     name="backgroundremover",
-    version="0.2.2",
+    version="0.2.3",
     description="Background remover from image and video using AI",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nadermx/backgroundremover",
     author="Johnathan Nader",
     author_email="john@nader.mx",
     classifiers=[
```


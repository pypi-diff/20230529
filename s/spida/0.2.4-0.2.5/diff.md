# Comparing `tmp/spida-0.2.4.tar.gz` & `tmp/spida-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spida-0.2.4.tar", last modified: Sun May 28 19:05:17 2023, max compression
+gzip compressed data, was "spida-0.2.5.tar", last modified: Sun May 28 23:04:08 2023, max compression
```

## Comparing `spida-0.2.4.tar` & `spida-0.2.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 19:05:17.508336 spida-0.2.4/
--rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.2.4/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.2.4/MANIFEST.in
--rw-rw-rw-   0        0        0     6148 2023-05-28 19:05:17.507148 spida-0.2.4/PKG-INFO
--rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.2.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-28 19:05:17.508336 spida-0.2.4/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-05-28 19:02:39.000000 spida-0.2.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:05:17.464731 spida-0.2.4/spida/
--rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.2.4/spida/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:05:17.496319 spida-0.2.4/spida/data/
--rw-rw-rw-   0        0        0        2 2023-05-28 19:01:46.000000 spida-0.2.4/spida/data/config.json
--rw-rw-rw-   0        0        0    16560 2023-05-28 18:51:43.000000 spida-0.2.4/spida/stable_diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:05:17.504045 spida-0.2.4/spida/utils/
--rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.2.4/spida/utils/__init__.py
--rw-rw-rw-   0        0        0     5913 2023-05-26 19:58:34.000000 spida-0.2.4/spida/utils/img.py
--rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.2.4/spida/utils/misc.py
--rw-rw-rw-   0        0        0      861 2023-05-17 04:00:18.000000 spida-0.2.4/spida/utils/net.py
-drwxrwxrwx   0        0        0        0 2023-05-28 19:05:17.494320 spida-0.2.4/spida.egg-info/
--rw-rw-rw-   0        0        0     6148 2023-05-28 19:05:17.000000 spida-0.2.4/spida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-28 19:05:17.000000 spida-0.2.4/spida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 19:05:17.000000 spida-0.2.4/spida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-05-28 19:05:17.000000 spida-0.2.4/spida.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-28 19:05:17.000000 spida-0.2.4/spida.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 23:04:08.218916 spida-0.2.5/
+-rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.2.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     6148 2023-05-28 23:04:08.217878 spida-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5690 2023-05-28 19:01:11.000000 spida-0.2.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 23:04:08.218916 spida-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-05-28 23:02:53.000000 spida-0.2.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:04:08.164530 spida-0.2.5/spida/
+-rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.2.5/spida/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:04:08.196623 spida-0.2.5/spida/data/
+-rw-rw-rw-   0        0        0        2 2023-05-28 23:00:43.000000 spida-0.2.5/spida/data/config.json
+-rw-rw-rw-   0        0        0    16560 2023-05-28 18:51:43.000000 spida-0.2.5/spida/stable_diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:04:08.215854 spida-0.2.5/spida/utils/
+-rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.2.5/spida/utils/__init__.py
+-rw-rw-rw-   0        0        0     5913 2023-05-26 19:58:34.000000 spida-0.2.5/spida/utils/img.py
+-rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.2.5/spida/utils/misc.py
+-rw-rw-rw-   0        0        0     1087 2023-05-28 22:57:32.000000 spida-0.2.5/spida/utils/net.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:04:08.194627 spida-0.2.5/spida.egg-info/
+-rw-rw-rw-   0        0        0     6148 2023-05-28 23:04:07.000000 spida-0.2.5/spida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-28 23:04:08.000000 spida-0.2.5/spida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:04:07.000000 spida-0.2.5/spida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-05-28 23:04:07.000000 spida-0.2.5/spida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 23:04:07.000000 spida-0.2.5/spida.egg-info/top_level.txt
```

### Comparing `spida-0.2.4/LICENSE` & `spida-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `spida-0.2.4/PKG-INFO` & `spida-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `spida-0.2.4/README.md` & `spida-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `spida-0.2.4/setup.py` & `spida-0.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="spida",
-    version="0.2.4",
+    version="0.2.5",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description="A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="h2see",
```

### Comparing `spida-0.2.4/spida/stable_diffusion.py` & `spida-0.2.5/spida/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `spida-0.2.4/spida/utils/img.py` & `spida-0.2.5/spida/utils/img.py`

 * *Files identical despite different names*

### Comparing `spida-0.2.4/spida/utils/misc.py` & `spida-0.2.5/spida/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spida-0.2.4/spida.egg-info/PKG-INFO` & `spida-0.2.5/spida.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.2.4
+Version: 0.2.5
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```


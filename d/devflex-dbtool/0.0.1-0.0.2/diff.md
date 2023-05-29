# Comparing `tmp/devflex-dbtool-0.0.1.tar.gz` & `tmp/devflex-dbtool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devflex-dbtool-0.0.1.tar", last modified: Mon May 29 15:06:40 2023, max compression
+gzip compressed data, was "devflex-dbtool-0.0.2.tar", last modified: Mon May 29 15:27:51 2023, max compression
```

## Comparing `devflex-dbtool-0.0.1.tar` & `devflex-dbtool-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:40.706747 devflex-dbtool-0.0.1/
--rw-rw-rw-   0        0        0     1112 2023-05-29 14:57:47.000000 devflex-dbtool-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      491 2023-05-29 15:06:40.705576 devflex-dbtool-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       45 2023-05-29 15:06:35.000000 devflex-dbtool-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 15:06:40.704414 devflex-dbtool-0.0.1/devflex_dbtool.egg-info/
--rw-rw-rw-   0        0        0      491 2023-05-29 15:06:40.000000 devflex-dbtool-0.0.1/devflex_dbtool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-05-29 15:06:40.000000 devflex-dbtool-0.0.1/devflex_dbtool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 15:06:40.000000 devflex-dbtool-0.0.1/devflex_dbtool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-29 15:06:40.000000 devflex-dbtool-0.0.1/devflex_dbtool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 15:06:40.000000 devflex-dbtool-0.0.1/devflex_dbtool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 15:06:40.706747 devflex-dbtool-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      729 2023-05-29 15:05:57.000000 devflex-dbtool-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 15:27:51.579780 devflex-dbtool-0.0.2/
+-rw-rw-rw-   0        0        0     1112 2023-05-29 14:57:47.000000 devflex-dbtool-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      493 2023-05-29 15:27:51.579780 devflex-dbtool-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2023-05-29 15:06:35.000000 devflex-dbtool-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 15:27:51.577776 devflex-dbtool-0.0.2/devflex_dbtool.egg-info/
+-rw-rw-rw-   0        0        0      493 2023-05-29 15:27:51.000000 devflex-dbtool-0.0.2/devflex_dbtool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-05-29 15:27:51.000000 devflex-dbtool-0.0.2/devflex_dbtool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 15:27:51.000000 devflex-dbtool-0.0.2/devflex_dbtool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-29 15:27:51.000000 devflex-dbtool-0.0.2/devflex_dbtool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 15:27:51.000000 devflex-dbtool-0.0.2/devflex_dbtool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 15:27:51.579780 devflex-dbtool-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      731 2023-05-29 15:27:21.000000 devflex-dbtool-0.0.2/setup.py
```

### Comparing `devflex-dbtool-0.0.1/LICENSE.txt` & `devflex-dbtool-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `devflex-dbtool-0.0.1/setup.py` & `devflex-dbtool-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="devflex-dbtool", # Replace with your own username
-    version="0.0.1",
+    version="0.0.2",
     author="DevFlex",
-    author_email="author@example.com",
+    author_email="workall350@gmail.com",
     description="my ezdb tool",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OverMony/python-devflex-dbtool-lib",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```


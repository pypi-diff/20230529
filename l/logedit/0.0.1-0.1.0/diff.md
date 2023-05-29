# Comparing `tmp/logedit-0.0.1.tar.gz` & `tmp/logedit-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logedit-0.0.1.tar", last modified: Sun May 28 20:08:10 2023, max compression
+gzip compressed data, was "logedit-0.1.0.tar", last modified: Mon May 29 04:24:12 2023, max compression
```

## Comparing `logedit-0.0.1.tar` & `logedit-0.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 gpriday    (501) staff       (20)        0 2023-05-28 20:08:10.592559 logedit-0.0.1/
--rw-r--r--   0 gpriday    (501) staff       (20)     3119 2023-05-28 20:08:10.592410 logedit-0.0.1/PKG-INFO
--rw-r--r--   0 gpriday    (501) staff       (20)     2737 2023-05-28 20:02:57.000000 logedit-0.0.1/README.md
-drwxr-xr-x   0 gpriday    (501) staff       (20)        0 2023-05-28 20:08:10.592066 logedit-0.0.1/logedit.egg-info/
--rw-r--r--   0 gpriday    (501) staff       (20)     3119 2023-05-28 20:08:10.000000 logedit-0.0.1/logedit.egg-info/PKG-INFO
--rw-r--r--   0 gpriday    (501) staff       (20)      206 2023-05-28 20:08:10.000000 logedit-0.0.1/logedit.egg-info/SOURCES.txt
--rw-r--r--   0 gpriday    (501) staff       (20)        1 2023-05-28 20:08:10.000000 logedit-0.0.1/logedit.egg-info/dependency_links.txt
--rw-r--r--   0 gpriday    (501) staff       (20)       55 2023-05-28 20:08:10.000000 logedit-0.0.1/logedit.egg-info/entry_points.txt
--rw-r--r--   0 gpriday    (501) staff       (20)       68 2023-05-28 20:08:10.000000 logedit-0.0.1/logedit.egg-info/requires.txt
--rw-r--r--   0 gpriday    (501) staff       (20)        1 2023-05-28 20:08:10.000000 logedit-0.0.1/logedit.egg-info/top_level.txt
--rw-r--r--   0 gpriday    (501) staff       (20)       38 2023-05-28 20:08:10.592617 logedit-0.0.1/setup.cfg
--rw-r--r--   0 gpriday    (501) staff       (20)      864 2023-05-28 18:09:03.000000 logedit-0.0.1/setup.py
+drwxr-xr-x   0 gpriday    (501) staff       (20)        0 2023-05-29 04:24:12.826684 logedit-0.1.0/
+-rw-r--r--   0 gpriday    (501) staff       (20)     3119 2023-05-29 04:24:12.826568 logedit-0.1.0/PKG-INFO
+-rw-r--r--   0 gpriday    (501) staff       (20)     2737 2023-05-28 20:02:57.000000 logedit-0.1.0/README.md
+drwxr-xr-x   0 gpriday    (501) staff       (20)        0 2023-05-29 04:24:12.826400 logedit-0.1.0/logedit.egg-info/
+-rw-r--r--   0 gpriday    (501) staff       (20)     3119 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/PKG-INFO
+-rw-r--r--   0 gpriday    (501) staff       (20)      206 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/SOURCES.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)        1 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/dependency_links.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)       55 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/entry_points.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)       78 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/requires.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)        1 2023-05-29 04:24:12.000000 logedit-0.1.0/logedit.egg-info/top_level.txt
+-rw-r--r--   0 gpriday    (501) staff       (20)       38 2023-05-29 04:24:12.826722 logedit-0.1.0/setup.cfg
+-rw-r--r--   0 gpriday    (501) staff       (20)      877 2023-05-29 04:22:06.000000 logedit-0.1.0/setup.py
```

### Comparing `logedit-0.0.1/PKG-INFO` & `logedit-0.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logedit
-Version: 0.0.1
+Version: 0.1.0
 Summary: A package to auto-generate changelogs from git commits using OpenAI's APIs
 Home-page: https://github.com/gregpriday/logedit/
 Author: Greg Priday
 Author-email: greg@siteorigin.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `logedit-0.0.1/README.md` & `logedit-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `logedit-0.0.1/logedit.egg-info/PKG-INFO` & `logedit-0.1.0/logedit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: logedit
-Version: 0.0.1
+Version: 0.1.0
 Summary: A package to auto-generate changelogs from git commits using OpenAI's APIs
 Home-page: https://github.com/gregpriday/logedit/
 Author: Greg Priday
 Author-email: greg@siteorigin.com
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
```

### Comparing `logedit-0.0.1/setup.py` & `logedit-0.1.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as readme_file:
     readme = readme_file.read()
 
-requirements = ["gitpython>=3.1.14", "tqdm>=4.60.0", "openai>=0.27.0", "python-dotenv>=0.17.0"]
+requirements = ["gitpython>=3.1.14", "tqdm>=4.60.0", "openai>=0.27.0", "backoff>=1.10.0", "tiktoken>=0.4.0"]
 
 setup(
     name="logedit",
-    version="0.0.1",
+    version="0.1.0",
     author="Greg Priday",
     author_email="greg@siteorigin.com",
     description="A package to auto-generate changelogs from git commits using OpenAI's APIs",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/gregpriday/logedit/",
     packages=find_packages(),
```


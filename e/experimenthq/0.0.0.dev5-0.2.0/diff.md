# Comparing `tmp/experimenthq-0.0.0.dev5.tar.gz` & `tmp/experimenthq-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "experimenthq-0.0.0.dev5.tar", last modified: Wed May 17 01:07:09 2023, max compression
+gzip compressed data, was "experimenthq-0.2.0.tar", last modified: Mon May 29 19:57:06 2023, max compression
```

## Comparing `experimenthq-0.0.0.dev5.tar` & `experimenthq-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 01:07:09.298314 experimenthq-0.0.0.dev5/
--rw-r--r--   0 ramonabendias   (501) staff       (20)     1071 2023-04-28 20:27:57.000000 experimenthq-0.0.0.dev5/LICENSE
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3608 2023-05-17 01:07:09.298408 experimenthq-0.0.0.dev5/PKG-INFO
--rw-r--r--   0 ramonabendias   (501) staff       (20)     2383 2023-05-14 20:21:42.000000 experimenthq-0.0.0.dev5/README.md
--rw-r--r--   0 ramonabendias   (501) staff       (20)      983 2023-05-17 01:07:09.298770 experimenthq-0.0.0.dev5/setup.cfg
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3265 2023-05-17 00:15:07.000000 experimenthq-0.0.0.dev5/setup.py
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 01:07:09.294641 experimenthq-0.0.0.dev5/src/
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 01:07:09.296589 experimenthq-0.0.0.dev5/src/experimenthq/
--rw-r--r--   0 ramonabendias   (501) staff       (20)      148 2023-05-14 19:40:55.000000 experimenthq-0.0.0.dev5/src/experimenthq/__init__.py
--rw-r--r--   0 ramonabendias   (501) staff       (20)      129 2023-05-17 01:06:58.000000 experimenthq-0.0.0.dev5/src/experimenthq/_about.py
--rw-r--r--   0 ramonabendias   (501) staff       (20)     2857 2023-05-17 01:06:47.000000 experimenthq-0.0.0.dev5/src/experimenthq/experiment.py
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 01:07:09.297857 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/
--rw-r--r--   0 ramonabendias   (501) staff       (20)     3608 2023-05-17 01:07:09.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/PKG-INFO
--rw-r--r--   0 ramonabendias   (501) staff       (20)      386 2023-05-17 01:07:09.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/SOURCES.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-17 01:07:09.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/dependency_links.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-06 11:57:37.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/not-zip-safe
--rw-r--r--   0 ramonabendias   (501) staff       (20)      126 2023-05-17 01:07:09.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/requires.txt
--rw-r--r--   0 ramonabendias   (501) staff       (20)       13 2023-05-17 01:07:09.000000 experimenthq-0.0.0.dev5/src/experimenthq.egg-info/top_level.txt
-drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-17 01:07:09.298014 experimenthq-0.0.0.dev5/tests/
--rw-r--r--   0 ramonabendias   (501) staff       (20)       36 2023-05-15 17:54:05.000000 experimenthq-0.0.0.dev5/tests/test_experiment.py
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-29 19:57:06.678453 experimenthq-0.2.0/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     1071 2023-04-28 20:27:57.000000 experimenthq-0.2.0/LICENSE
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3603 2023-05-29 19:57:06.678547 experimenthq-0.2.0/PKG-INFO
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     2383 2023-05-14 20:21:42.000000 experimenthq-0.2.0/README.md
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      983 2023-05-29 19:57:06.678903 experimenthq-0.2.0/setup.cfg
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3358 2023-05-29 14:01:33.000000 experimenthq-0.2.0/setup.py
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-29 19:57:06.674811 experimenthq-0.2.0/src/
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-29 19:57:06.676727 experimenthq-0.2.0/src/experimenthq/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      176 2023-05-29 14:16:05.000000 experimenthq-0.2.0/src/experimenthq/__init__.py
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      124 2023-05-29 19:56:54.000000 experimenthq-0.2.0/src/experimenthq/_about.py
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     4828 2023-05-29 19:55:55.000000 experimenthq-0.2.0/src/experimenthq/experiment.py
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     2219 2023-05-29 18:21:24.000000 experimenthq-0.2.0/src/experimenthq/notion_types.py
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-29 19:57:06.678187 experimenthq-0.2.0/src/experimenthq.egg-info/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)     3603 2023-05-29 19:57:06.000000 experimenthq-0.2.0/src/experimenthq.egg-info/PKG-INFO
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      419 2023-05-29 19:57:06.000000 experimenthq-0.2.0/src/experimenthq.egg-info/SOURCES.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-29 19:57:06.000000 experimenthq-0.2.0/src/experimenthq.egg-info/dependency_links.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)        1 2023-05-06 11:57:37.000000 experimenthq-0.2.0/src/experimenthq.egg-info/not-zip-safe
+-rw-r--r--   0 ramonabendias   (501) staff       (20)      163 2023-05-29 19:57:06.000000 experimenthq-0.2.0/src/experimenthq.egg-info/requires.txt
+-rw-r--r--   0 ramonabendias   (501) staff       (20)       13 2023-05-29 19:57:06.000000 experimenthq-0.2.0/src/experimenthq.egg-info/top_level.txt
+drwxr-xr-x   0 ramonabendias   (501) staff       (20)        0 2023-05-29 19:57:06.678332 experimenthq-0.2.0/tests/
+-rw-r--r--   0 ramonabendias   (501) staff       (20)        0 2023-05-29 18:31:18.000000 experimenthq-0.2.0/tests/test_experiment.py
```

### Comparing `experimenthq-0.0.0.dev5/LICENSE` & `experimenthq-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev5/PKG-INFO` & `experimenthq-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimenthq
-Version: 0.0.0.dev5
+Version: 0.2.0
 Summary: A Python package for tracking experiments in Notion
 Author: 
 Author-email: 
 License: MIT
 Project-URL: Website, https://www.experiment-hq.com/
 Keywords: notion,tracking,ml,machine learning,experiment,experimentation,experiment tracking,python,sync
 Classifier: Programming Language :: Python :: 3
```

### Comparing `experimenthq-0.0.0.dev5/README.md` & `experimenthq-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev5/setup.cfg` & `experimenthq-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `experimenthq-0.0.0.dev5/setup.py` & `experimenthq-0.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,21 @@
     author_email=EMAIL,
     python_requires=REQUIRES_PYTHON,
     license=LICENSE,
     packages=find_packages(where="src", exclude=("tests", "test", "examples", "docs")),
     package_dir={"": "src"},
     py_modules=[splitext(basename(path))[0] for path in glob("src/*.py")],
     zip_safe=False,
-    install_requires=["requests", "types-requests"],
+    install_requires=[
+        "requests",
+        "types-requests",
+        "python-dateutil",
+        "phonenumbers",
+        "urllib3",
+    ],
     extras_require={
         # extras can be installed via: pip install package[dev]
         "dev": [
             "pytest",
             "pytest-cov",
             "flake8",
             "black",
```

### Comparing `experimenthq-0.0.0.dev5/src/experimenthq.egg-info/PKG-INFO` & `experimenthq-0.2.0/src/experimenthq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: experimenthq
-Version: 0.0.0.dev5
+Version: 0.2.0
 Summary: A Python package for tracking experiments in Notion
 Author: 
 Author-email: 
 License: MIT
 Project-URL: Website, https://www.experiment-hq.com/
 Keywords: notion,tracking,ml,machine learning,experiment,experimentation,experiment tracking,python,sync
 Classifier: Programming Language :: Python :: 3
```


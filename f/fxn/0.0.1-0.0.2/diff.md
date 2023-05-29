# Comparing `tmp/fxn-0.0.1.tar.gz` & `tmp/fxn-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fxn-0.0.1.tar", last modified: Tue May 16 16:10:07 2023, max compression
+gzip compressed data, was "fxn-0.0.2.tar", last modified: Mon May 29 01:02:25 2023, max compression
```

## Comparing `fxn-0.0.1.tar` & `fxn-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,35 @@
-drwxr-xr-x   0 yusuf      (501) staff       (20)        0 2023-05-16 16:10:07.389680 fxn-0.0.1/
--rw-r--r--   0 yusuf      (501) staff       (20)    11356 2023-05-16 16:06:40.000000 fxn-0.0.1/LICENSE
--rw-r--r--   0 yusuf      (501) staff       (20)      709 2023-05-16 16:10:07.389363 fxn-0.0.1/PKG-INFO
--rw-r--r--   0 yusuf      (501) staff       (20)       27 2023-05-16 16:06:53.000000 fxn-0.0.1/README.md
-drwxr-xr-x   0 yusuf      (501) staff       (20)        0 2023-05-16 16:10:07.388276 fxn-0.0.1/fxn.egg-info/
--rw-r--r--   0 yusuf      (501) staff       (20)      709 2023-05-16 16:10:07.000000 fxn-0.0.1/fxn.egg-info/PKG-INFO
--rw-r--r--   0 yusuf      (501) staff       (20)      160 2023-05-16 16:10:07.000000 fxn-0.0.1/fxn.egg-info/SOURCES.txt
--rw-r--r--   0 yusuf      (501) staff       (20)        1 2023-05-16 16:10:07.000000 fxn-0.0.1/fxn.egg-info/dependency_links.txt
--rw-r--r--   0 yusuf      (501) staff       (20)       42 2023-05-16 16:10:07.000000 fxn-0.0.1/fxn.egg-info/requires.txt
--rw-r--r--   0 yusuf      (501) staff       (20)        1 2023-05-16 16:10:07.000000 fxn-0.0.1/fxn.egg-info/top_level.txt
--rw-r--r--   0 yusuf      (501) staff       (20)       38 2023-05-16 16:10:07.389785 fxn-0.0.1/setup.cfg
--rw-r--r--   0 yusuf      (501) staff       (20)     1506 2023-05-16 16:09:22.000000 fxn-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:25.681276 fxn-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-29 01:02:04.000000 fxn-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 01:02:25.677276 fxn-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 01:02:04.000000 fxn-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:25.677276 fxn-0.0.2/fxn/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:25.677276 fxn-0.0.2/fxn/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      511 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4113 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/featureinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/prediction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:25.677276 fxn-0.0.2/fxn/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1826 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/predictors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/cli/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-29 01:02:04.000000 fxn-0.0.2/fxn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:02:25.677276 fxn-0.0.2/fxn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-29 01:02:25.000000 fxn-0.0.2/fxn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 01:02:25.681276 fxn-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-05-29 01:02:04.000000 fxn-0.0.2/setup.py
```

### Comparing `fxn-0.0.1/LICENSE` & `fxn-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fxn-0.0.1/PKG-INFO` & `fxn-0.0.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.1
-Summary: Edge and cloud prediction functions for building AI applications.
+Version: 0.0.2
+Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Function
 *Coming soon...*
+
```

### Comparing `fxn-0.0.1/fxn.egg-info/PKG-INFO` & `fxn-0.0.2/fxn.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: fxn
-Version: 0.0.1
-Summary: Edge and cloud prediction functions for building AI applications.
+Version: 0.0.2
+Summary: Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.
 Home-page: https://fxn.ai
 Author: NatML Inc.
 Author-email: hi@fxn.ai
 License: Apache License 2.0
 Project-URL: Documentation, https://docs.fxn.ai
 Project-URL: Source, https://github.com/fxnai/fxn
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Image Recognition
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Function
 *Coming soon...*
+
```

### Comparing `fxn-0.0.1/setup.py` & `fxn-0.0.2/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 # Setup
 setup(
     name="fxn",
     version=version,
     author="NatML Inc.",
     author_email="hi@fxn.ai",
-    description="Edge and cloud prediction functions for building AI applications.",
+    description="Run on-device and cloud AI prediction functions in Python. Register at https://hub.fxn.ai.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache License 2.0",
 	python_requires=">=3.7",
     install_requires=[
         "filetype",
         "numpy",
@@ -35,19 +35,19 @@
         "typer"
     ],
     url="https://fxn.ai",
     packages=find_packages(
         include=["fxn", "fxn.*"],
         exclude=["test", "examples"]
     ),
-    # entry_points={
-    #     "console_scripts": [
-    #         "fxn=fxn.cli.__init__:app"
-    #     ]
-    # },
+    entry_points={
+        "console_scripts": [
+            "fxn=fxn.cli.__init__:app"
+        ]
+    },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: Image Recognition",
         "Topic :: Software Development :: Libraries",
     ],
```


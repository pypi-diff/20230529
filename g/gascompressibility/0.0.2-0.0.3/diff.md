# Comparing `tmp/gascompressibility-0.0.2.tar.gz` & `tmp/gascompressibility-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gascompressibility-0.0.2.tar", last modified: Mon May 29 07:14:22 2023, max compression
+gzip compressed data, was "gascompressibility-0.0.3.tar", last modified: Mon May 29 07:16:19 2023, max compression
```

## Comparing `gascompressibility-0.0.2.tar` & `gascompressibility-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:14:22.600367 gascompressibility-0.0.2/
--rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     2094 2023-05-29 07:14:22.599367 gascompressibility-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2023-05-29 07:13:43.000000 gascompressibility-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 07:14:22.587368 gascompressibility-0.0.2/gascompressibility/
--rw-rw-rw-   0        0        0       89 2023-05-25 15:06:36.000000 gascompressibility-0.0.2/gascompressibility/__init__.py
--rw-rw-rw-   0        0        0    23949 2023-05-29 05:17:48.000000 gascompressibility-0.0.2/gascompressibility/zfactor.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:14:22.597368 gascompressibility-0.0.2/gascompressibility.egg-info/
--rw-rw-rw-   0        0        0     2094 2023-05-29 07:14:22.000000 gascompressibility-0.0.2/gascompressibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      336 2023-05-29 07:14:22.000000 gascompressibility-0.0.2/gascompressibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:14:22.000000 gascompressibility-0.0.2/gascompressibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-05-29 07:14:22.000000 gascompressibility-0.0.2/gascompressibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-05-29 07:14:22.000000 gascompressibility-0.0.2/gascompressibility.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 07:14:22.600367 gascompressibility-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1198 2023-05-29 07:09:24.000000 gascompressibility-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:14:22.598368 gascompressibility-0.0.2/tests/
--rw-rw-rw-   0        0        0       77 2023-05-25 15:06:36.000000 gascompressibility-0.0.2/tests/__init__.py
--rw-rw-rw-   0        0        0     9581 2023-05-29 05:23:18.000000 gascompressibility-0.0.2/tests/test_gascomp.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:16:19.988836 gascompressibility-0.0.3/
+-rw-rw-rw-   0        0        0     1095 2023-05-23 14:19:22.000000 gascompressibility-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     2094 2023-05-29 07:16:19.988836 gascompressibility-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2023-05-29 07:13:43.000000 gascompressibility-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 07:16:19.976836 gascompressibility-0.0.3/gascompressibility/
+-rw-rw-rw-   0        0        0       89 2023-05-25 15:06:36.000000 gascompressibility-0.0.3/gascompressibility/__init__.py
+-rw-rw-rw-   0        0        0    23949 2023-05-29 05:17:48.000000 gascompressibility-0.0.3/gascompressibility/zfactor.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:16:19.986837 gascompressibility-0.0.3/gascompressibility.egg-info/
+-rw-rw-rw-   0        0        0     2094 2023-05-29 07:16:19.000000 gascompressibility-0.0.3/gascompressibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      336 2023-05-29 07:16:19.000000 gascompressibility-0.0.3/gascompressibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 07:16:19.000000 gascompressibility-0.0.3/gascompressibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-29 07:16:19.000000 gascompressibility-0.0.3/gascompressibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-29 07:16:19.000000 gascompressibility-0.0.3/gascompressibility.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 07:16:19.988836 gascompressibility-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1198 2023-05-29 07:16:14.000000 gascompressibility-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:16:19.987837 gascompressibility-0.0.3/tests/
+-rw-rw-rw-   0        0        0       77 2023-05-25 15:06:36.000000 gascompressibility-0.0.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     9581 2023-05-29 05:23:18.000000 gascompressibility-0.0.3/tests/test_gascomp.py
```

### Comparing `gascompressibility-0.0.2/LICENSE` & `gascompressibility-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.0.2/PKG-INFO` & `gascompressibility-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.0.2
+Version: 0.0.3
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gascompressibility-0.0.2/README.md` & `gascompressibility-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.0.2/gascompressibility/zfactor.py` & `gascompressibility-0.0.3/gascompressibility/zfactor.py`

 * *Files identical despite different names*

### Comparing `gascompressibility-0.0.2/gascompressibility.egg-info/PKG-INFO` & `gascompressibility-0.0.3/gascompressibility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gascompressibility
-Version: 0.0.2
+Version: 0.0.3
 Summary: GasCompressibility-py is a Python library for calculating the gas compressibility factor, Z, based on real gas law.
 Home-page: https://github.com/aegis4048/GasCompressibiltiy-py/tree/main
 Author: Eric Kim
 Author-email: aegis4048@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
```

### Comparing `gascompressibility-0.0.2/setup.py` & `gascompressibility-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def classifiers():
     with open('classifiers.txt') as f:
         return f.read().strip().split('\n')
 
 
 setup(
     name='gascompressibility',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(exclude=[
         "tutorials",
         "LICENSE",
         ".gitignore",
         "README.md",
         "misc",
         ".travis.yml",
```

### Comparing `gascompressibility-0.0.2/tests/test_gascomp.py` & `gascompressibility-0.0.3/tests/test_gascomp.py`

 * *Files identical despite different names*


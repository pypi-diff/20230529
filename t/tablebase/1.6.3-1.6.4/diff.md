# Comparing `tmp/tablebase-1.6.3.tar.gz` & `tmp/tablebase-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\AllFiles\PythonLibs\tablebase\dist\.tmp-xk2ow7pa\tablebase-1.6.3.tar", last modified: Mon May 29 20:18:26 2023, max compression
+gzip compressed data, was "C:\AllFiles\PythonLibs\tablebase\dist\.tmp-n28p5rp3\tablebase-1.6.4.tar", last modified: Mon May 29 20:42:39 2023, max compression
```

## Comparing `tablebase-1.6.3.tar` & `tablebase-1.6.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 20:18:26.404408 tablebase-1.6.3/
--rw-rw-rw-   0        0        0     1086 2022-07-18 21:48:23.000000 tablebase-1.6.3/LICENSE
--rw-rw-rw-   0        0        0     1084 2021-04-03 19:09:23.000000 tablebase-1.6.3/LICENSE.txt
--rw-rw-rw-   0        0        0     1102 2023-05-29 20:18:26.404408 tablebase-1.6.3/PKG-INFO
--rw-rw-rw-   0        0        0      770 2023-05-29 20:11:43.000000 tablebase-1.6.3/README.md
--rw-rw-rw-   0        0        0       86 2022-11-01 20:19:29.000000 tablebase-1.6.3/pyproject.toml
--rw-rw-rw-   0        0        0      443 2023-05-29 20:18:26.464976 tablebase-1.6.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-29 20:18:26.356405 tablebase-1.6.3/tablebase/
--rw-rw-rw-   0        0        0       40 2022-05-08 21:07:22.000000 tablebase-1.6.3/tablebase/__init__.py
--rw-rw-rw-   0        0        0    10725 2023-05-29 19:49:23.000000 tablebase-1.6.3/tablebase/tablebase.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:18:26.397400 tablebase-1.6.3/tablebase.egg-info/
--rw-rw-rw-   0        0        0     1102 2023-05-29 20:18:26.000000 tablebase-1.6.3/tablebase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-29 20:18:26.000000 tablebase-1.6.3/tablebase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 20:18:26.000000 tablebase-1.6.3/tablebase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-29 20:18:26.000000 tablebase-1.6.3/tablebase.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 20:18:26.400401 tablebase-1.6.3/tests/
--rw-rw-rw-   0        0        0     5368 2023-05-29 19:46:38.000000 tablebase-1.6.3/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-29 20:42:39.381078 tablebase-1.6.4/
+-rw-rw-rw-   0        0        0     1086 2022-07-18 21:48:23.000000 tablebase-1.6.4/LICENSE
+-rw-rw-rw-   0        0        0     1084 2021-04-03 19:09:23.000000 tablebase-1.6.4/LICENSE.txt
+-rw-rw-rw-   0        0        0     1143 2023-05-29 20:42:39.382079 tablebase-1.6.4/PKG-INFO
+-rw-rw-rw-   0        0        0      770 2023-05-29 20:25:44.000000 tablebase-1.6.4/README.md
+-rw-rw-rw-   0        0        0       86 2022-11-01 20:19:29.000000 tablebase-1.6.4/pyproject.toml
+-rw-rw-rw-   0        0        0      490 2023-05-29 20:42:39.386076 tablebase-1.6.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 20:42:39.181673 tablebase-1.6.4/tablebase/
+-rw-rw-rw-   0        0        0       40 2022-05-08 21:07:22.000000 tablebase-1.6.4/tablebase/__init__.py
+-rw-rw-rw-   0        0        0    10725 2023-05-29 19:49:23.000000 tablebase-1.6.4/tablebase/tablebase.py
+drwxrwxrwx   0        0        0        0 2023-05-29 20:42:39.346051 tablebase-1.6.4/tablebase.egg-info/
+-rw-rw-rw-   0        0        0     1143 2023-05-29 20:42:38.000000 tablebase-1.6.4/tablebase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-29 20:42:39.000000 tablebase-1.6.4/tablebase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 20:42:39.000000 tablebase-1.6.4/tablebase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-29 20:42:39.000000 tablebase-1.6.4/tablebase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 20:42:39.378079 tablebase-1.6.4/tests/
+-rw-rw-rw-   0        0        0     5368 2023-05-29 19:46:38.000000 tablebase-1.6.4/tests/test.py
```

### Comparing `tablebase-1.6.3/LICENSE` & `tablebase-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tablebase-1.6.3/LICENSE.txt` & `tablebase-1.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tablebase-1.6.3/PKG-INFO` & `tablebase-1.6.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tablebase
-Version: 1.6.3
+Version: 1.6.4
 Summary: A lightweight tool to make tables easily in python.
 Author: Maximilian Lange
 Author-email: maxhlange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 Tablebase
 =============
 
 If you found a bug, need a feature, or have question please open an [issue](https://github.com/sasmlange/tablebase/issues).
```

### Comparing `tablebase-1.6.3/README.md` & `tablebase-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `tablebase-1.6.3/tablebase/tablebase.py` & `tablebase-1.6.4/tablebase/tablebase.py`

 * *Files identical despite different names*

### Comparing `tablebase-1.6.3/tablebase.egg-info/PKG-INFO` & `tablebase-1.6.4/tablebase.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: tablebase
-Version: 1.6.3
+Version: 1.6.4
 Summary: A lightweight tool to make tables easily in python.
 Author: Maximilian Lange
 Author-email: maxhlange@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE.txt
 
 Tablebase
 =============
 
 If you found a bug, need a feature, or have question please open an [issue](https://github.com/sasmlange/tablebase/issues).
```

### Comparing `tablebase-1.6.3/tests/test.py` & `tablebase-1.6.4/tests/test.py`

 * *Files identical despite different names*


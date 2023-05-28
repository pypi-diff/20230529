# Comparing `tmp/matchmeta-2023.5.28.tar.gz` & `tmp/matchmeta-2023.5.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matchmeta-2023.5.28.tar", last modified: Sun May 28 22:18:42 2023, max compression
+gzip compressed data, was "matchmeta-2023.5.29.tar", last modified: Sun May 28 22:32:20 2023, max compression
```

## Comparing `matchmeta-2023.5.28.tar` & `matchmeta-2023.5.29.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:18:42.770353 matchmeta-2023.5.28/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-28 22:18:42.770353 matchmeta-2023.5.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:18:42.770353 matchmeta-2023.5.28/matchmeta.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-28 22:18:42.000000 matchmeta-2023.5.28/matchmeta.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:18:42.770353 matchmeta-2023.5.28/mmi/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/mmi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/mmi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9784 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/mmi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 22:18:42.770353 matchmeta-2023.5.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-28 22:18:28.000000 matchmeta-2023.5.28/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:32:20.587558 matchmeta-2023.5.29/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-28 22:32:20.587558 matchmeta-2023.5.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3123 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:32:20.587558 matchmeta-2023.5.29/matchmeta.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3423 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-28 22:32:20.000000 matchmeta-2023.5.29/matchmeta.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:32:20.587558 matchmeta-2023.5.29/mmi/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/mmi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/mmi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9976 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/mmi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 22:32:20.587558 matchmeta-2023.5.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-28 22:32:09.000000 matchmeta-2023.5.29/setup.py
```

### Comparing `matchmeta-2023.5.28/LICENSE` & `matchmeta-2023.5.29/LICENSE`

 * *Files identical despite different names*

### Comparing `matchmeta-2023.5.28/PKG-INFO` & `matchmeta-2023.5.29/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmeta
-Version: 2023.5.28
+Version: 2023.5.29
 Summary: OS Triage for Anyone and Everyone
 Home-page: https://github.com/jblukach/mmi
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `matchmeta-2023.5.28/README.md` & `matchmeta-2023.5.29/README.md`

 * *Files identical despite different names*

### Comparing `matchmeta-2023.5.28/matchmeta.egg-info/PKG-INFO` & `matchmeta-2023.5.29/matchmeta.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matchmeta
-Version: 2023.5.28
+Version: 2023.5.29
 Summary: OS Triage for Anyone and Everyone
 Home-page: https://github.com/jblukach/mmi
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `matchmeta-2023.5.28/mmi/__init__.py` & `matchmeta-2023.5.29/mmi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,8 +6,8 @@
 __largefile__ = LARGEFILE = '\033[91m{}\033[00m'        ### RED ###
 __nofilehash__ = NOFILEHASH = '\033[93m{}\033[00m'      ### YELLOW ###
 __partialmeta__ = PARTIALMETA = '\033[97m{}\033[00m'    ### GREY ###
 
 __gtfo__ = GTFO = pathlib.Path.joinpath(pathlib.Path.home(), 'gtfo.bloom')
 __mmi__ = MMI = pathlib.Path.joinpath(pathlib.Path.home(), 'mmi.bloom')
 
-__version__ = VERSION = '2023.5.28'
+__version__ = VERSION = '2023.5.29'
```

### Comparing `matchmeta-2023.5.28/mmi/cli.py` & `matchmeta-2023.5.29/mmi/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -288,9 +288,14 @@
     parser.add_argument('-s', '--skip', help='Skip File Hashing', action='store_true')
     parser.add_argument('-v', '--version', action='version', version=__version__)
     args = parser.parse_args()
 
     if args.download:
         download()
     else:
-        with concurrent.futures.ThreadPoolExecutor() as executor:
-            executor.submit(start, args.skip)
+        if __mmi__.is_file() == False:
+            print('MISSING: '+str(__mmi__))
+        elif __gtfo__.is_file() == False:
+            print('MISSING: '+str(__gtfo__))
+        else:
+            with concurrent.futures.ThreadPoolExecutor() as executor:
+                executor.submit(start, args.skip)
```

### Comparing `matchmeta-2023.5.28/setup.py` & `matchmeta-2023.5.29/setup.py`

 * *Files identical despite different names*


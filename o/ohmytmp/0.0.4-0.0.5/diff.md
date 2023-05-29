# Comparing `tmp/ohmytmp-0.0.4.tar.gz` & `tmp/ohmytmp-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ohmytmp-0.0.4.tar", last modified: Sun May 28 14:21:02 2023, max compression
+gzip compressed data, was "ohmytmp-0.0.5.tar", last modified: Mon May 29 10:41:54 2023, max compression
```

## Comparing `ohmytmp-0.0.4.tar` & `ohmytmp-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 14:21:02.134951 ohmytmp-0.0.4/
--rw-rw-rw-   0        0        0     1064 2023-05-28 04:17:27.000000 ohmytmp-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1826 2023-05-28 14:21:02.133952 ohmytmp-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0        6 2023-05-28 04:17:27.000000 ohmytmp-0.0.4/README.md
--rw-rw-rw-   0        0        0      705 2023-05-28 14:19:58.000000 ohmytmp-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-28 14:21:02.134951 ohmytmp-0.0.4/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 14:21:02.116951 ohmytmp-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 14:21:02.128951 ohmytmp-0.0.4/src/ohmytmp/
--rw-rw-rw-   0        0        0      149 2023-05-28 14:19:59.000000 ohmytmp-0.0.4/src/ohmytmp/__init__.py
--rw-rw-rw-   0        0        0     1752 2023-05-28 14:19:38.000000 ohmytmp-0.0.4/src/ohmytmp/constant.py
--rw-rw-rw-   0        0        0     1033 2023-05-28 14:10:26.000000 ohmytmp-0.0.4/src/ohmytmp/core.py
--rw-rw-rw-   0        0        0     1042 2023-05-28 14:19:20.000000 ohmytmp-0.0.4/src/ohmytmp/destination.py
--rw-rw-rw-   0        0        0     2101 2023-05-28 14:04:45.000000 ohmytmp-0.0.4/src/ohmytmp/guesstype.py
--rw-rw-rw-   0        0        0     2457 2023-05-28 14:19:20.000000 ohmytmp-0.0.4/src/ohmytmp/initialization.py
--rw-rw-rw-   0        0        0      756 2023-05-28 14:03:56.000000 ohmytmp-0.0.4/src/ohmytmp/plugin.py
-drwxrwxrwx   0        0        0        0 2023-05-28 14:21:02.132952 ohmytmp-0.0.4/src/ohmytmp.egg-info/
--rw-rw-rw-   0        0        0     1826 2023-05-28 14:21:02.000000 ohmytmp-0.0.4/src/ohmytmp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      344 2023-05-28 14:21:02.000000 ohmytmp-0.0.4/src/ohmytmp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 14:21:02.000000 ohmytmp-0.0.4/src/ohmytmp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-05-28 14:21:02.000000 ohmytmp-0.0.4/src/ohmytmp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 10:41:54.433860 ohmytmp-0.0.5/
+-rw-rw-rw-   0        0        0     1064 2023-05-28 04:17:27.000000 ohmytmp-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1891 2023-05-29 10:41:54.433341 ohmytmp-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       73 2023-05-29 10:32:35.000000 ohmytmp-0.0.5/README.md
+-rw-rw-rw-   0        0        0      705 2023-05-29 10:33:20.000000 ohmytmp-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 10:41:54.433860 ohmytmp-0.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-29 10:41:54.416126 ohmytmp-0.0.5/src/
+drwxrwxrwx   0        0        0        0 2023-05-29 10:41:54.423422 ohmytmp-0.0.5/src/ohmytmp/
+-rw-rw-rw-   0        0        0      149 2023-05-29 10:31:50.000000 ohmytmp-0.0.5/src/ohmytmp/__init__.py
+-rw-rw-rw-   0        0        0     1752 2023-05-28 14:19:38.000000 ohmytmp-0.0.5/src/ohmytmp/constant.py
+-rw-rw-rw-   0        0        0     1071 2023-05-29 10:36:21.000000 ohmytmp-0.0.5/src/ohmytmp/core.py
+-rw-rw-rw-   0        0        0     2100 2023-05-29 10:31:02.000000 ohmytmp-0.0.5/src/ohmytmp/guesstype.py
+-rw-rw-rw-   0        0        0      745 2023-05-29 10:35:50.000000 ohmytmp-0.0.5/src/ohmytmp/plugin.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:41:54.432304 ohmytmp-0.0.5/src/ohmytmp.egg-info/
+-rw-rw-rw-   0        0        0     1891 2023-05-29 10:41:54.000000 ohmytmp-0.0.5/src/ohmytmp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-29 10:41:54.000000 ohmytmp-0.0.5/src/ohmytmp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 10:41:54.000000 ohmytmp-0.0.5/src/ohmytmp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-05-29 10:41:54.000000 ohmytmp-0.0.5/src/ohmytmp.egg-info/top_level.txt
```

### Comparing `ohmytmp-0.0.4/LICENSE` & `ohmytmp-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ohmytmp-0.0.4/PKG-INFO` & `ohmytmp-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp
-Version: 0.0.4
+Version: 0.0.5
 Summary: ohmytmp-core
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
         
@@ -33,7 +33,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # core
+
+```sh
+pip install ohmytmp
+```
+
+```py
+import ohmytmp
+```
```

### Comparing `ohmytmp-0.0.4/pyproject.toml` & `ohmytmp-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ohmytmp"
-version = "0.0.4"
+version = "0.0.5"
 description = "ohmytmp-core"
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 keywords = ["file"]
 
 authors = [
```

### Comparing `ohmytmp-0.0.4/src/ohmytmp/constant.py` & `ohmytmp-0.0.5/src/ohmytmp/constant.py`

 * *Files identical despite different names*

### Comparing `ohmytmp-0.0.4/src/ohmytmp/core.py` & `ohmytmp-0.0.5/src/ohmytmp/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from copy import deepcopy as dcp
 
 from .constant import FUNC, Info
-from .plugin import *
+from .plugin import PluginBase, PluginAnalysis, PluginAfter
 
 
 class Ohmytmp:
     def __init__(self) -> None:
         self.func = {i: list() for i in FUNC.to_dict().values()}
         from .guesstype import guesstype
         self.register(PluginAnalysis(guesstype))
```

### Comparing `ohmytmp-0.0.4/src/ohmytmp/guesstype.py` & `ohmytmp-0.0.5/src/ohmytmp/guesstype.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,8 +66,8 @@
 def guess_ext(e: str) -> str:
     return ext_re.get(e, TYPE.UNKNOWN)
 
 
 def guesstype(info: Info) -> None:
     info.TYPE = guess_ext(info.EXT)
     if info.TYPE == TYPE.UNKNOWN:
-        info.TYPE == guess_mime(info.SRC)
+        info.TYPE = guess_mime(info.SRC)
```

### Comparing `ohmytmp-0.0.4/src/ohmytmp/plugin.py` & `ohmytmp-0.0.5/src/ohmytmp/plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import os
 from typing import Callable
 
 from .constant import Info, FUNC
 
 
 class PluginBase:
     def __init__(self, func: Callable = None) -> None:
```

### Comparing `ohmytmp-0.0.4/src/ohmytmp.egg-info/PKG-INFO` & `ohmytmp-0.0.5/src/ohmytmp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ohmytmp
-Version: 0.0.4
+Version: 0.0.5
 Summary: ohmytmp-core
 Author-email: userElaina <userelaina@pm.me>
 Maintainer-email: userElaina <userelaina@pm.me>
 License: MIT License
         
         Copyright (c) 2023 ohmytmp
         
@@ -33,7 +33,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # core
+
+```sh
+pip install ohmytmp
+```
+
+```py
+import ohmytmp
+```
```


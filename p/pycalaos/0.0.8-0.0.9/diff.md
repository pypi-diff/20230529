# Comparing `tmp/pycalaos-0.0.8.tar.gz` & `tmp/pycalaos-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycalaos-0.0.8.tar", last modified: Tue Mar 21 19:39:42 2023, max compression
+gzip compressed data, was "pycalaos-0.0.9.tar", last modified: Tue Mar 21 20:02:01 2023, max compression
```

## Comparing `pycalaos-0.0.8.tar` & `pycalaos-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-03-21 19:39:42.862504 pycalaos-0.0.8/
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     1167 2023-03-21 19:39:42.862504 pycalaos-0.0.8/PKG-INFO
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)      580 2023-03-06 19:10:02.707762 pycalaos-0.0.8/README.md
-drwxrwxr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-03-21 19:39:42.862504 pycalaos-0.0.8/pycalaos/
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)       75 2023-03-04 12:02:40.684120 pycalaos-0.0.8/pycalaos/__init__.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     6276 2023-03-21 06:37:26.806736 pycalaos-0.0.8/pycalaos/client.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     1652 2023-03-06 19:09:40.418887 pycalaos-0.0.8/pycalaos/discovery.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     4734 2023-03-21 18:42:54.424685 pycalaos-0.0.8/pycalaos/item.py
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)       40 2023-03-05 09:58:40.818431 pycalaos-0.0.8/setup.cfg
--rw-rw-r--   0 sebastien  (1000) sebastien  (1000)      729 2023-03-21 19:39:22.725930 pycalaos-0.0.8/setup.py
+drwxrwxr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-03-21 20:02:01.776926 pycalaos-0.0.9/
+-rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     1167 2023-03-21 20:02:01.776926 pycalaos-0.0.9/PKG-INFO
+-rw-rw-r--   0 sebastien  (1000) sebastien  (1000)      580 2023-03-06 19:10:02.707762 pycalaos-0.0.9/README.md
+drwxrwxr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-03-21 20:02:01.776926 pycalaos-0.0.9/pycalaos/
+-rw-rw-r--   0 sebastien  (1000) sebastien  (1000)      115 2023-03-21 19:44:40.250988 pycalaos-0.0.9/pycalaos/__init__.py
+-rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     6276 2023-03-21 06:37:26.806736 pycalaos-0.0.9/pycalaos/client.py
+-rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     1652 2023-03-06 19:09:40.418887 pycalaos-0.0.9/pycalaos/discovery.py
+-rw-rw-r--   0 sebastien  (1000) sebastien  (1000)     4688 2023-03-21 19:46:32.434189 pycalaos-0.0.9/pycalaos/item.py
+-rw-rw-r--   0 sebastien  (1000) sebastien  (1000)       40 2023-03-05 09:58:40.818431 pycalaos-0.0.9/setup.cfg
+-rw-rw-r--   0 sebastien  (1000) sebastien  (1000)      729 2023-03-21 20:01:48.172475 pycalaos-0.0.9/setup.py
```

### Comparing `pycalaos-0.0.8/PKG-INFO` & `pycalaos-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: pycalaos
-Version: 0.0.8
+Version: 0.0.9
 Summary: Calaos home automation client library
 Home-page: https://github.com/tiramiseb/pycalaos
 Author: Sébastien Maccagnoni
 Author-email: sebastien@maccagnoni.eu
 License: MIT
 Description: # Python Calaos
```

### Comparing `pycalaos-0.0.8/README.md` & `pycalaos-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pycalaos-0.0.8/pycalaos/client.py` & `pycalaos-0.0.9/pycalaos/client.py`

 * *Files identical despite different names*

### Comparing `pycalaos-0.0.8/pycalaos/discovery.py` & `pycalaos-0.0.9/pycalaos/discovery.py`

 * *Files identical despite different names*

### Comparing `pycalaos-0.0.8/pycalaos/item.py` & `pycalaos-0.0.9/pycalaos/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 from enum import Enum
 
 
-class NotAnOutputError(Exception):
-    pass
-
-
 class Event:
     """An item state change event"""
 
     def __init__(self, item):
         """Initialize the event with the item and the current item state
 
         Create the event after changing the item state.
```

### Comparing `pycalaos-0.0.8/setup.py` & `pycalaos-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pycalaos",
-    version="0.0.8",
+    version="0.0.9",
     description="Calaos home automation client library",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Sébastien Maccagnoni",
     author_email="sebastien@maccagnoni.eu",
     url="https://github.com/tiramiseb/pycalaos",
     packages=["pycalaos"],
```


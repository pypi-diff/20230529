# Comparing `tmp/noconf-0.1a2.tar.gz` & `tmp/noconf-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noconf-0.1a2.tar", last modified: Wed May 10 15:27:52 2023, max compression
+gzip compressed data, was "noconf-0.1a3.tar", last modified: Mon May 29 14:09:01 2023, max compression
```

## Comparing `noconf-0.1a2.tar` & `noconf-0.1a3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-10 15:27:52.172481 noconf-0.1a2/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1282 2023-05-10 15:27:52.172481 noconf-0.1a2/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      849 2023-05-10 15:17:45.000000 noconf-0.1a2/README.rst
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-10 15:27:52.172481 noconf-0.1a2/noconf/
--rw-r--r--   0 daniel    (1000) daniel    (1000)       52 2023-05-10 15:26:56.000000 noconf-0.1a2/noconf/__init__.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)     7787 2023-04-28 21:45:25.000000 noconf-0.1a2/noconf/conf.py
--rw-r--r--   0 daniel    (1000) daniel    (1000)    10109 2023-04-28 21:45:35.000000 noconf-0.1a2/noconf/test_conf.py
-drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-10 15:27:52.172481 noconf-0.1a2/noconf.egg-info/
--rw-r--r--   0 daniel    (1000) daniel    (1000)     1282 2023-05-10 15:27:52.000000 noconf-0.1a2/noconf.egg-info/PKG-INFO
--rw-r--r--   0 daniel    (1000) daniel    (1000)      261 2023-05-10 15:27:52.000000 noconf-0.1a2/noconf.egg-info/SOURCES.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-10 15:27:52.000000 noconf-0.1a2/noconf.egg-info/dependency_links.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-17 13:33:57.000000 noconf-0.1a2/noconf.egg-info/not-zip-safe
--rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-05-10 15:27:52.000000 noconf-0.1a2/noconf.egg-info/requires.txt
--rw-r--r--   0 daniel    (1000) daniel    (1000)        7 2023-05-10 15:27:52.000000 noconf-0.1a2/noconf.egg-info/top_level.txt
--rwxrwxr-x   0 daniel    (1000) daniel    (1000)      507 2023-05-10 15:27:52.172481 noconf-0.1a2/setup.cfg
--rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-02-23 12:20:39.000000 noconf-0.1a2/setup.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-29 14:09:01.961011 noconf-0.1a3/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1023 2023-05-29 14:09:01.961011 noconf-0.1a3/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      849 2023-05-10 15:17:45.000000 noconf-0.1a3/README.rst
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-29 14:09:01.957011 noconf-0.1a3/noconf/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       52 2023-05-29 14:06:06.000000 noconf-0.1a3/noconf/__init__.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     7894 2023-05-29 14:06:06.000000 noconf-0.1a3/noconf/conf.py
+-rw-r--r--   0 daniel    (1000) daniel    (1000)    10109 2023-04-28 21:45:35.000000 noconf-0.1a3/noconf/test_conf.py
+drwxr-xr-x   0 daniel    (1000) daniel    (1000)        0 2023-05-29 14:09:01.961011 noconf-0.1a3/noconf.egg-info/
+-rw-r--r--   0 daniel    (1000) daniel    (1000)     1023 2023-05-29 14:09:01.000000 noconf-0.1a3/noconf.egg-info/PKG-INFO
+-rw-r--r--   0 daniel    (1000) daniel    (1000)      261 2023-05-29 14:09:01.000000 noconf-0.1a3/noconf.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-05-29 14:09:01.000000 noconf-0.1a3/noconf.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        1 2023-04-17 13:33:57.000000 noconf-0.1a3/noconf.egg-info/not-zip-safe
+-rw-r--r--   0 daniel    (1000) daniel    (1000)       21 2023-05-29 14:09:01.000000 noconf-0.1a3/noconf.egg-info/requires.txt
+-rw-r--r--   0 daniel    (1000) daniel    (1000)        7 2023-05-29 14:09:01.000000 noconf-0.1a3/noconf.egg-info/top_level.txt
+-rwxrwxr-x   0 daniel    (1000) daniel    (1000)      507 2023-05-29 14:09:01.961011 noconf-0.1a3/setup.cfg
+-rw-rw-r--   0 daniel    (1000) daniel    (1000)       38 2023-02-23 12:20:39.000000 noconf-0.1a3/setup.py
```

### Comparing `noconf-0.1a2/PKG-INFO` & `noconf-0.1a3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: noconf
-Version: 0.1a2
+Version: 0.1a3
 Summary: Component-based configuration for everyone!
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: ======
-        noconf
-        ======
-        
-        Key features
-        ============
-        
-        1. **Flexible configuration**: noconf allows you to configure your
-           Python applications using configuration files that use Python
-           syntax.
-        
-        2. **Multiple configuration files**: noconf allows you to split your
-           configuration across multiple files, making it easier to manage and
-           update your configuration as your application grows.
-        
-        3. **Configuration referencing**: noconf allows you to reference other
-           parts of your configuration from within your configuration,
-           avoiding duplication and keeping your configuration DRY (Don't
-           Repeat Yourself).
-        
-        4. **Component-based programming**: noconf enables you to initialize
-           classes using your configuration, making it easy to compose complex
-           systems out of smaller, reusable components. This promotes code
-           reuse and maintainability.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: devel
+
+======
+noconf
+======
+
+Key features
+============
+
+1. **Flexible configuration**: noconf allows you to configure your
+   Python applications using configuration files that use Python
+   syntax.
+
+2. **Multiple configuration files**: noconf allows you to split your
+   configuration across multiple files, making it easier to manage and
+   update your configuration as your application grows.
+
+3. **Configuration referencing**: noconf allows you to reference other
+   parts of your configuration from within your configuration,
+   avoiding duplication and keeping your configuration DRY (Don't
+   Repeat Yourself).
+
+4. **Component-based programming**: noconf enables you to initialize
+   classes using your configuration, making it easy to compose complex
+   systems out of smaller, reusable components. This promotes code
+   reuse and maintainability.
```

### Comparing `noconf-0.1a2/README.rst` & `noconf-0.1a3/README.rst`

 * *Files identical despite different names*

### Comparing `noconf-0.1a2/noconf/conf.py` & `noconf-0.1a3/noconf/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from copy import deepcopy
+import functools
 from functools import cache
 from functools import wraps
 from importlib import import_module
 from logging.config import dictConfig
 import os
 import sys
 from threading import RLock
@@ -21,14 +22,18 @@
         with lock:
             return func(*args, **kwargs)
     if hasattr(func, 'cache_clear'):
         wrapper.cache_clear = func.cache_clear
     return wrapper
 
 
+def partial(func, *args, **kwargs):
+    return functools.partial(func, *args, **kwargs)
+
+
 def resolve_dotted_name(dotted_name):
     if ':' in dotted_name:
         module, name = dotted_name.split(':')
     elif '.' in dotted_name:
         module, name = dotted_name.rsplit('.', 1)
     else:
         module, name = dotted_name, None
```

### Comparing `noconf-0.1a2/noconf/test_conf.py` & `noconf-0.1a3/noconf/test_conf.py`

 * *Files identical despite different names*

### Comparing `noconf-0.1a2/noconf.egg-info/PKG-INFO` & `noconf-0.1a3/noconf.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Metadata-Version: 2.1
 Name: noconf
-Version: 0.1a2
+Version: 0.1a3
 Summary: Component-based configuration for everyone!
-Home-page: UNKNOWN
-License: UNKNOWN
-Description: ======
-        noconf
-        ======
-        
-        Key features
-        ============
-        
-        1. **Flexible configuration**: noconf allows you to configure your
-           Python applications using configuration files that use Python
-           syntax.
-        
-        2. **Multiple configuration files**: noconf allows you to split your
-           configuration across multiple files, making it easier to manage and
-           update your configuration as your application grows.
-        
-        3. **Configuration referencing**: noconf allows you to reference other
-           parts of your configuration from within your configuration,
-           avoiding duplication and keeping your configuration DRY (Don't
-           Repeat Yourself).
-        
-        4. **Component-based programming**: noconf enables you to initialize
-           classes using your configuration, making it easy to compose complex
-           systems out of smaller, reusable components. This promotes code
-           reuse and maintainability.
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: devel
+
+======
+noconf
+======
+
+Key features
+============
+
+1. **Flexible configuration**: noconf allows you to configure your
+   Python applications using configuration files that use Python
+   syntax.
+
+2. **Multiple configuration files**: noconf allows you to split your
+   configuration across multiple files, making it easier to manage and
+   update your configuration as your application grows.
+
+3. **Configuration referencing**: noconf allows you to reference other
+   parts of your configuration from within your configuration,
+   avoiding duplication and keeping your configuration DRY (Don't
+   Repeat Yourself).
+
+4. **Component-based programming**: noconf enables you to initialize
+   classes using your configuration, making it easy to compose complex
+   systems out of smaller, reusable components. This promotes code
+   reuse and maintainability.
```


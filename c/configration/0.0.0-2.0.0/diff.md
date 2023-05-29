# Comparing `tmp/configration-0.0.0.tar.gz` & `tmp/configration-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configration-0.0.0.tar", last modified: Wed May 10 10:09:22 2023, max compression
+gzip compressed data, was "configration-2.0.0.tar", last modified: Mon May 29 08:07:59 2023, max compression
```

## Comparing `configration-0.0.0.tar` & `configration-2.0.0.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 10:09:22.642401 configration-0.0.0/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-0.0.0/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)      597 2023-05-10 10:09:22.642401 configration-0.0.0/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-0.0.0/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 10:09:22.639068 configration-0.0.0/configration/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      135 2023-05-10 09:37:10.000000 configration-0.0.0/configration/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-10 09:17:32.000000 configration-0.0.0/configration/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 10:09:22.642401 configration-0.0.0/configration/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-0.0.0/configration/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2191 2023-05-10 09:59:24.000000 configration-0.0.0/configration/src/json_config.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-10 10:09:22.642401 configration-0.0.0/configration.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      597 2023-05-10 10:09:22.000000 configration-0.0.0/configration.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      295 2023-05-10 10:09:22.000000 configration-0.0.0/configration.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-10 10:09:22.000000 configration-0.0.0/configration.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-05-10 10:09:22.000000 configration-0.0.0/configration.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-10 10:09:22.642401 configration-0.0.0/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-0.0.0/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:07:59.045557 configration-2.0.0/
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.0/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      761 2023-05-29 08:07:59.048890 configration-2.0.0/PKG-INFO
+-rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.0/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:07:59.042224 configration-2.0.0/configration/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      135 2023-05-10 09:37:10.000000 configration-2.0.0/configration/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-05-29 06:50:37.000000 configration-2.0.0/configration/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:07:59.045557 configration-2.0.0/configration/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-09 13:37:49.000000 configration-2.0.0/configration/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1695 2023-05-28 08:11:27.000000 configration-2.0.0/configration/src/config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      350 2023-05-28 09:52:46.000000 configration-2.0.0/configration/src/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      952 2023-05-28 09:53:21.000000 configration-2.0.0/configration/src/json_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      948 2023-05-28 09:52:59.000000 configration-2.0.0/configration/src/toml_config.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:07:59.045557 configration-2.0.0/configration/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-05-25 20:06:22.000000 configration-2.0.0/configration/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1563 2023-05-28 09:59:14.000000 configration-2.0.0/configration/tests/test_json.py
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1563 2023-05-28 10:00:21.000000 configration-2.0.0/configration/tests/test_toml.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:07:59.042224 configration-2.0.0/configration.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      761 2023-05-29 08:07:58.000000 configration-2.0.0/configration.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      498 2023-05-29 08:07:58.000000 configration-2.0.0/configration.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-05-29 08:07:58.000000 configration-2.0.0/configration.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-05-29 08:07:58.000000 configration-2.0.0/configration.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-05-29 08:07:59.048890 configration-2.0.0/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1001)     1179 2023-05-10 10:07:07.000000 configration-2.0.0/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-05-29 08:07:59.045557 configration-2.0.0/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1001)      205 2023-05-26 07:00:53.000000 configration-2.0.0/tests/test_json.py
```

### Comparing `configration-0.0.0/LICENSE.txt` & `configration-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configration-0.0.0/PKG-INFO` & `configration-2.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 0.0.0
+Version: 2.0.0
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,12 +20,23 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 1.0.0 29 May 2023
+
+1. Implement Toml configs
+2. Test suit introduced
+
+Version 0.0.1 11 May 2023
+
+1. Better error message if config file is missing
+
+------
+
 Version 0.0.0 10 May 2023
 
 1. Initial version
 
 ------
```

### Comparing `configration-0.0.0/configration/src/json_config.py` & `configration-2.0.0/configration/src/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""Return a valid config object from a json file for the application."""
+"""Base class for config object for the application."""
 
-import json
 from termcolor import cprint
 import colorama
 
+from .constants import ERROR_COLOUR, CORRUPT_FILE_MSG, MISSING_ATTR_MSG, NOT_OF_TYPE_MSG
+
 colorama.init()
 
-ERROR_COLOUR = 'red'
 
-class JsonConfig():
+class Config():
     """
     The class takes a path to a json file and if valid, returns a config dict.
 
     Attributes
     ----------
 
     path: str
@@ -23,46 +23,33 @@
         The dict item holds a list of allowed types for each files
 
         If there are attrs, then the config is validated.
     """
 
     def __init__(self, path: str, attrs: dict[str, list[type]] = {}):
         self.path = path
-        self .attrs = attrs
+        self.attrs = attrs
         self.config = self._get_config()
         for key, item in self.config.items():
             self.__dict__[key] = item
 
     def _get_config(self) -> dict[str, object]:
         # Return config, if contents are valid.
         config = self._read_config()
 
         if not self.attrs:
             return config
 
         if self._validate_config(config):
             return config
-        quit()
-
-    def _read_config(self) -> dict[str, object]:
-        # Open the config file and return the file handle
-        try:
-            with open(self.path , 'r') as f_config:
-                try:
-                    return json.load(f_config)
-                except json.decoder.JSONDecodeError:
-                    cprint(f"Invalid json format in {self.path }", ERROR_COLOUR)
-                    quit()
-        except FileNotFoundError:
-            cprint(f"The file {self.path } is not in the expected location", ERROR_COLOUR)
-            quit()
+        return {}
 
     def _validate_config(self, config: dict[str, type]) -> bool:
         # Return True if structure and values in config are valid.
-        for name, item_types in self .attrs.items():
+        for name, item_types in self.attrs.items():
             if name not in config:
-                cprint(f"Corrupt config file. {name} missing", ERROR_COLOUR)
+                cprint(f"{CORRUPT_FILE_MSG} {MISSING_ATTR_MSG} {name}", ERROR_COLOUR)
                 return False
             if type(config[name]) not in item_types:
-                cprint(f"Corrupt config file. {name} not of type {item_types}", ERROR_COLOUR)
+                cprint(f"{CORRUPT_FILE_MSG} {name} {NOT_OF_TYPE_MSG} {item_types}", ERROR_COLOUR)
                 return False
         return True
```

### Comparing `configration-0.0.0/configration.egg-info/PKG-INFO` & `configration-2.0.0/configration.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 0.0.0
+Version: 2.0.0
 Summary: """A collection of modules that supports workbooks with openpyxl."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
 Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
 Keywords: cli,input
@@ -20,12 +20,23 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 1.0.0 29 May 2023
+
+1. Implement Toml configs
+2. Test suit introduced
+
+Version 0.0.1 11 May 2023
+
+1. Better error message if config file is missing
+
+------
+
 Version 0.0.0 10 May 2023
 
 1. Initial version
 
 ------
```

### Comparing `configration-0.0.0/setup.py` & `configration-2.0.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/cabinet-2023.5.20.2.tar.gz` & `tmp/cabinet-2023.5.29.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cabinet-2023.5.20.2.tar", last modified: Sat May 20 06:30:08 2023, max compression
+gzip compressed data, was "cabinet-2023.5.29.1.tar", last modified: Mon May 29 07:37:37 2023, max compression
```

## Comparing `cabinet-2023.5.20.2.tar` & `cabinet-2023.5.29.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-20 06:30:08.480119 cabinet-2023.5.20.2/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.5.20.2/LICENSE
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6494 2023-05-20 06:30:08.480119 cabinet-2023.5.20.2/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6142 2023-04-16 16:59:23.000000 cabinet-2023.5.20.2/README.md
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.5.20.2/pyproject.toml
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-05-20 06:30:08.484119 cabinet-2023.5.20.2/setup.cfg
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-20 06:30:08.480119 cabinet-2023.5.20.2/src/
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-20 06:30:08.480119 cabinet-2023.5.20.2/src/cabinet/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    25639 2023-05-20 06:28:19.000000 cabinet-2023.5.20.2/src/cabinet/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-20 06:28:13.000000 cabinet-2023.5.20.2/src/cabinet/__main__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.5.20.2/src/cabinet/mail.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-20 06:30:08.480119 cabinet-2023.5.20.2/src/cabinet.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     6494 2023-05-20 06:30:08.000000 cabinet-2023.5.20.2/src/cabinet.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      288 2023-05-20 06:30:08.000000 cabinet-2023.5.20.2/src/cabinet.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-20 06:30:08.000000 cabinet-2023.5.20.2/src/cabinet.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-05-20 06:30:08.000000 cabinet-2023.5.20.2/src/cabinet.egg-info/entry_points.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-05-20 06:30:08.000000 cabinet-2023.5.20.2/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11357 2023-03-06 03:35:41.000000 cabinet-2023.5.29.1/LICENSE
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6580 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6228 2023-05-29 07:33:24.000000 cabinet-2023.5.29.1/README.md
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       98 2023-03-06 04:41:10.000000 cabinet-2023.5.29.1/pyproject.toml
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      750 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/setup.cfg
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/src/
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/src/cabinet/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    26102 2023-05-29 07:33:24.000000 cabinet-2023.5.29.1/src/cabinet/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       69 2023-05-20 07:12:29.000000 cabinet-2023.5.29.1/src/cabinet/__main__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3687 2023-04-16 16:59:23.000000 cabinet-2023.5.29.1/src/cabinet/mail.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/src/cabinet.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     6580 2023-05-29 07:37:37.000000 cabinet-2023.5.29.1/src/cabinet.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      310 2023-05-29 07:37:37.000000 cabinet-2023.5.29.1/src/cabinet.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2023-05-29 07:37:37.000000 cabinet-2023.5.29.1/src/cabinet.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       41 2023-05-29 07:37:37.000000 cabinet-2023.5.29.1/src/cabinet.egg-info/entry_points.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        8 2023-05-29 07:37:37.000000 cabinet-2023.5.29.1/src/cabinet.egg-info/top_level.txt
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2023-05-29 07:37:37.181556 cabinet-2023.5.29.1/test/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     5868 2023-05-29 07:26:03.000000 cabinet-2023.5.29.1/test/test___init__.py
```

### Comparing `cabinet-2023.5.20.2/LICENSE` & `cabinet-2023.5.29.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cabinet-2023.5.20.2/PKG-INFO` & `cabinet-2023.5.29.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.5.20.2
+Version: 2023.5.29.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -270,12 +270,15 @@
 - smtplib
 
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
+## Unit Tests
+- Unit tests are available in `test/`; use `pytest test/` to run them.
+
 ## Author
 
 - Tyler Woodfin
   - [GitHub](https://www.github.com/tylerjwoodfin)
   - [Website](http://tyler.cloud)
```

### Comparing `cabinet-2023.5.20.2/README.md` & `cabinet-2023.5.29.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -258,12 +258,15 @@
 - smtplib
 
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
+## Unit Tests
+- Unit tests are available in `test/`; use `pytest test/` to run them.
+
 ## Author
 
 - Tyler Woodfin
   - [GitHub](https://www.github.com/tylerjwoodfin)
   - [Website](http://tyler.cloud)
```

### Comparing `cabinet-2023.5.20.2/setup.cfg` & `cabinet-2023.5.29.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cabinet
-version = 2023.05.20.2
+version = 2023.05.29.1
 author = Tyler Woodfin
 author_email = feedback@tyler.cloud
 description = Easily manage data storage and logging across repos
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/tylerjwoodfin/cabinet
 project_urls =
```

### Comparing `cabinet-2023.5.20.2/src/cabinet/__init__.py` & `cabinet-2023.5.29.1/src/cabinet/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,35 +46,35 @@
 
     def __init__(self, path_cabinet: str = None):
         """
         The main module for file management
 
         Args:
             - path_cabinet (str, optional): the directory of a settings.json file to be used
-                Defaults to ~/cabinet if unset
+                Defaults to get_config('path_cabinet') or ~/cabinet if unset
 
         Returns:
             None
 
         Usage:
             ```
             from cabinet import Cabinet
             cab = cabinet.Cabinet()
             ```
         """
 
         # config file, stored within the package
-        self.path_config_file = pathlib.Path(
-            __file__).resolve().parent / "config.json"
+        self.path_config_file = str(pathlib.Path(
+            __file__).resolve().parent / "config.json")
 
         # determines where settings.json is stored; by default, this is ~/cabinet
-        self.path_cabinet = os.path.expanduser(
+        self.path_cabinet = path_cabinet or os.path.expanduser(
             self._get_config('path_cabinet'))
 
-        path_cabinet = path_cabinet or self.path_cabinet
+        path_cabinet = self.path_cabinet
 
         # new setup
         if path_cabinet is None:
             self.new_setup = True
             path_cabinet = input(self.NEW_SETUP_MSG)
             if not path_cabinet:
                 path_cabinet = str(pathlib.Path.home() / "cabinet")
@@ -412,17 +412,18 @@
 
         settings = self.settings_json
 
         for index, item in enumerate(attributes):
             if item in settings:
                 settings = settings[item]
             elif warn_missing and (len(attributes) < 2 or attributes[1] != "edit"):
-                is_print(
-                    f"Warning: {item} not found in \
-                        {settings if index > 0 else f'{self.path_cabinet}/settings.json'}")
+                msg_settings = settings if index > 0 else f'{self.path_cabinet}/settings.json'
+                self._ifprint(
+                    f"Warning: {item} not found in {msg_settings}",
+                    is_print)
                 self._ifprint("None", is_print)
                 return None
             else:
                 self._ifprint("None", is_print)
                 return None
 
         self._ifprint(settings, is_print)
@@ -434,45 +435,52 @@
 
         Args:
             *attribute (str): A series of keys in the JSON object
                 to identify the location of the property.
             value (optional): The value to put into the property.
                 If not specified, the last argument will be used.
             file_name (str): The name of the JSON file to put the property in.
+                File must be in the `path_cabinet` folder.
+                Default: 'settings.json'
 
         Returns:
             The value that was put into the property.
         """
 
         path_full = f"{self.path_cabinet}/{file_name}"
 
+        maximum_attribute_index = 0
+        attribute_max_attribute_index = attribute
+
         if not value:
             value = attribute[-1]
+            maximum_attribute_index = -1
+            attribute_max_attribute_index = attribute[:maximum_attribute_index]
 
         _settings = self.settings_json if file_name == 'settings.json' else json.load(
             open(path_full, encoding="utf8"))
 
         # iterate through entire JSON object and replace 2nd to last attribute with value
 
         partition = _settings
 
-        for index, item in enumerate(attribute[:-1]):
+        for index, item in enumerate(attribute_max_attribute_index):
             if item not in partition:
                 try:
                     partition[item] = value if index == len(
-                        attribute) - 2 else {}
+                        attribute) + maximum_attribute_index - 1 else {}
                     partition = partition[item]
                     self.log(
                         f"Adding new key '{item}' to {partition if index > 0 else path_full}",
                         is_quiet=self.new_setup)
                 except TypeError as error:
                     self.log(f"{error}\n\n{attribute[index-1]} is currently a string, so it cannot \
 be treated as an object with multiple properties.", level="error")
             else:
-                if index == len(attribute) - 2:
+                if index == len(attribute) + maximum_attribute_index - 1:
                     partition[item] = value
                 else:
                     partition = partition[item]
 
         with open(path_full, 'w+', encoding="utf8") as file:
             json.dump(_settings, file, indent=4)
```

### Comparing `cabinet-2023.5.20.2/src/cabinet/mail.py` & `cabinet-2023.5.29.1/src/cabinet/mail.py`

 * *Files identical despite different names*

### Comparing `cabinet-2023.5.20.2/src/cabinet.egg-info/PKG-INFO` & `cabinet-2023.5.29.1/src/cabinet.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cabinet
-Version: 2023.5.20.2
+Version: 2023.5.29.1
 Summary: Easily manage data storage and logging across repos
 Home-page: https://github.com/tylerjwoodfin/cabinet
 Author: Tyler Woodfin
 Author-email: feedback@tyler.cloud
 License: : OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -270,12 +270,15 @@
 - smtplib
 
 ## Disclaimers
 
 - Although I've done quite a bit of testing, I can't guarantee everything that works on my machine will work on yours. Always back up your data to multiple places to avoid data loss.
 - If you find any issues, please contact me... or get your hands dirty and raise a PR!
 
+## Unit Tests
+- Unit tests are available in `test/`; use `pytest test/` to run them.
+
 ## Author
 
 - Tyler Woodfin
   - [GitHub](https://www.github.com/tylerjwoodfin)
   - [Website](http://tyler.cloud)
```


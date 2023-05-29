# Comparing `tmp/global_hotkeys-0.1.2.tar.gz` & `tmp/global_hotkeys-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "global_hotkeys-0.1.2.tar", last modified: Sun May 28 21:40:56 2023, max compression
+gzip compressed data, was "global_hotkeys-0.1.3.tar", last modified: Mon May 29 03:26:01 2023, max compression
```

## Comparing `global_hotkeys-0.1.2.tar` & `global_hotkeys-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 21:40:56.717408 global_hotkeys-0.1.2/
--rw-rw-rw-   0        0        0     1218 2023-05-28 21:40:10.000000 global_hotkeys-0.1.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     8736 2023-05-28 21:40:56.716407 global_hotkeys-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     6984 2023-05-28 21:39:05.000000 global_hotkeys-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 21:40:56.700407 global_hotkeys-0.1.2/global_hotkeys/
--rw-rw-rw-   0        0        0     3306 2023-05-28 21:29:56.000000 global_hotkeys-0.1.2/global_hotkeys/__init__.py
--rw-rw-rw-   0        0        0    10334 2023-05-28 21:25:45.000000 global_hotkeys-0.1.2/global_hotkeys/hotkey_checker.py
--rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.2/global_hotkeys/keycodes.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:40:56.713409 global_hotkeys-0.1.2/global_hotkeys.egg-info/
--rw-rw-rw-   0        0        0     8736 2023-05-28 21:40:56.000000 global_hotkeys-0.1.2/global_hotkeys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      383 2023-05-28 21:40:56.000000 global_hotkeys-0.1.2/global_hotkeys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:40:56.000000 global_hotkeys-0.1.2/global_hotkeys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-28 21:40:56.000000 global_hotkeys-0.1.2/global_hotkeys.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-28 21:40:56.000000 global_hotkeys-0.1.2/global_hotkeys.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-28 21:40:56.717408 global_hotkeys-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      802 2023-05-28 21:39:20.000000 global_hotkeys-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:40:56.715408 global_hotkeys-0.1.2/tests/
--rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.2/tests/_t.py
--rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.2/tests/global_snippets.py
--rw-rw-rw-   0        0        0     1381 2023-05-28 21:29:00.000000 global_hotkeys-0.1.2/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:26:01.960146 global_hotkeys-0.1.3/
+-rw-rw-rw-   0        0        0     1403 2023-05-29 03:25:19.000000 global_hotkeys-0.1.3/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1066 2023-05-27 07:09:18.000000 global_hotkeys-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0       30 2023-05-27 07:09:18.000000 global_hotkeys-0.1.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     8921 2023-05-29 03:26:01.960146 global_hotkeys-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6984 2023-05-28 21:39:05.000000 global_hotkeys-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 03:26:01.927352 global_hotkeys-0.1.3/global_hotkeys/
+-rw-rw-rw-   0        0        0     3486 2023-05-29 03:21:04.000000 global_hotkeys-0.1.3/global_hotkeys/__init__.py
+-rw-rw-rw-   0        0        0    10334 2023-05-28 21:25:45.000000 global_hotkeys-0.1.3/global_hotkeys/hotkey_checker.py
+-rw-rw-rw-   0        0        0     3796 2023-05-28 05:06:18.000000 global_hotkeys-0.1.3/global_hotkeys/keycodes.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:26:01.944145 global_hotkeys-0.1.3/global_hotkeys.egg-info/
+-rw-rw-rw-   0        0        0     8921 2023-05-29 03:26:01.000000 global_hotkeys-0.1.3/global_hotkeys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      383 2023-05-29 03:26:01.000000 global_hotkeys-0.1.3/global_hotkeys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 03:26:01.000000 global_hotkeys-0.1.3/global_hotkeys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-29 03:26:01.000000 global_hotkeys-0.1.3/global_hotkeys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-29 03:26:01.000000 global_hotkeys-0.1.3/global_hotkeys.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 03:26:01.960146 global_hotkeys-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      802 2023-05-29 03:23:27.000000 global_hotkeys-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:26:01.958145 global_hotkeys-0.1.3/tests/
+-rw-rw-rw-   0        0        0      261 2023-05-28 11:37:24.000000 global_hotkeys-0.1.3/tests/_t.py
+-rw-rw-rw-   0        0        0     2219 2023-05-28 06:41:24.000000 global_hotkeys-0.1.3/tests/global_snippets.py
+-rw-rw-rw-   0        0        0     1381 2023-05-29 03:22:24.000000 global_hotkeys-0.1.3/tests/test.py
```

### Comparing `global_hotkeys-0.1.2/CHANGELOG.txt` & `global_hotkeys-0.1.3/CHANGELOG.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Change Log
 ==========
 
+0.1.3 (5/28/2023)
+-----------------
+- Implemented retrofitting for the original hotkey style: e.g. ["control", "alt", "z"]. This is converted automatically to "control + alt + z".
+
 0.1.2 (5/28/2023)
 -----------------
 - Added dict binding format support. Also added support for supplying callback parameters for bindings.
 
 0.1.1 (5/28/2023)
 -----------------
 - Added syntax update warning for anyone still using the old hotkey binding syntax. Updated the singular register_hotkey function.
```

### Comparing `global_hotkeys-0.1.2/LICENSE.txt` & `global_hotkeys-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.2/PKG-INFO` & `global_hotkeys-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global_hotkeys
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -312,14 +312,18 @@
 '
 `
 ```
 
 Change Log
 ==========
 
+0.1.3 (5/28/2023)
+-----------------
+- Implemented retrofitting for the original hotkey style: e.g. ["control", "alt", "z"]. This is converted automatically to "control + alt + z".
+
 0.1.2 (5/28/2023)
 -----------------
 - Added dict binding format support. Also added support for supplying callback parameters for bindings.
 
 0.1.1 (5/28/2023)
 -----------------
 - Added syntax update warning for anyone still using the old hotkey binding syntax. Updated the singular register_hotkey function.
```

### Comparing `global_hotkeys-0.1.2/README.md` & `global_hotkeys-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.2/global_hotkeys/__init__.py` & `global_hotkeys-0.1.3/global_hotkeys/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,33 @@
         hotkey_string = str(binding)
         valid_hotkey_string = " + ".join(binding)
         raise Exception(
             "You've specified the hotkey as a list. The syntax has changed to being specified as a string now.\n"+
             f"Your hotkey {hotkey_string} should now be specified as \"{valid_hotkey_string}\""
         )
 
+def retrofit_old_bindings(binding):
+     if isinstance(binding, list):
+          return " + ".join(binding)
+     return binding
+
 def sanitize_binding(binding_raw):
     if (isinstance(binding_raw, list)):
-        _binding = binding_raw[0]
+        _binding = retrofit_old_bindings(binding_raw[0])
         keydown_function = binding_raw[1]
         keyup_function = binding_raw[2]
         actuate_on_partial_release = True
         if len(binding_raw) > 3:
             actuate_on_partial_release = binding_raw[3]
         params = None
         if len(binding_raw) > 4:
             params = binding_raw[4]
         return [_binding, keydown_function, keyup_function, actuate_on_partial_release, params]
     elif (isinstance(binding_raw, dict)):
-        _binding = binding_raw["hotkey"]
+        _binding = retrofit_old_bindings(binding_raw["hotkey"])
         keydown_function = binding_raw["on_press_callback"]
         keyup_function = binding_raw["on_release_callback"]
         actuate_on_partial_release = True
         if "actuate_on_partial_release" in binding_raw:
             actuate_on_partial_release = binding_raw["actuate_on_partial_release"]
         params = None
         if "callback_params" in binding_raw:
```

### Comparing `global_hotkeys-0.1.2/global_hotkeys/hotkey_checker.py` & `global_hotkeys-0.1.3/global_hotkeys/hotkey_checker.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.2/global_hotkeys/keycodes.py` & `global_hotkeys-0.1.3/global_hotkeys/keycodes.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.2/global_hotkeys.egg-info/PKG-INFO` & `global_hotkeys-0.1.3/global_hotkeys.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: global-hotkeys
-Version: 0.1.2
+Version: 0.1.3
 Home-page: https://github.com/btsdev
 Author: btsdev
 Author-email: btsdevman@gmail.com
 License: MIT
 Keywords: hotkeys,shortcuts
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -312,14 +312,18 @@
 '
 `
 ```
 
 Change Log
 ==========
 
+0.1.3 (5/28/2023)
+-----------------
+- Implemented retrofitting for the original hotkey style: e.g. ["control", "alt", "z"]. This is converted automatically to "control + alt + z".
+
 0.1.2 (5/28/2023)
 -----------------
 - Added dict binding format support. Also added support for supplying callback parameters for bindings.
 
 0.1.1 (5/28/2023)
 -----------------
 - Added syntax update warning for anyone still using the old hotkey binding syntax. Updated the singular register_hotkey function.
```

### Comparing `global_hotkeys-0.1.2/setup.py` & `global_hotkeys-0.1.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
 
 setup(
   name='global_hotkeys',
-  version='0.1.2',
+  version='0.1.3',
   description='',
   long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.txt').read(),
   long_description_content_type='text/markdown',
   url='https://github.com/btsdev',
   author='btsdev',
   author_email='btsdevman@gmail.com',
   license='MIT',
```

### Comparing `global_hotkeys-0.1.2/tests/global_snippets.py` & `global_hotkeys-0.1.3/tests/global_snippets.py`

 * *Files identical despite different names*

### Comparing `global_hotkeys-0.1.2/tests/test.py` & `global_hotkeys-0.1.3/tests/test.py`

 * *Files identical despite different names*


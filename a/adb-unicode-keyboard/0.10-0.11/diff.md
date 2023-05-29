# Comparing `tmp/adb_unicode_keyboard-0.10.tar.gz` & `tmp/adb_unicode_keyboard-0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adb_unicode_keyboard-0.10.tar", last modified: Wed Nov 30 02:38:38 2022, max compression
+gzip compressed data, was "adb_unicode_keyboard-0.11.tar", last modified: Mon May 29 01:01:17 2023, max compression
```

## Comparing `adb_unicode_keyboard-0.10.tar` & `adb_unicode_keyboard-0.11.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-11-30 02:38:38.430735 adb_unicode_keyboard-0.10/
--rw-rw-rw-   0        0        0     1148 2022-11-30 02:38:29.000000 adb_unicode_keyboard-0.10/LICENSE.rst
--rw-rw-rw-   0        0        0      169 2022-11-30 02:38:28.000000 adb_unicode_keyboard-0.10/MANIFEST.in
--rw-rw-rw-   0        0        0     2336 2022-11-30 02:38:38.431711 adb_unicode_keyboard-0.10/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2022-11-30 02:34:33.000000 adb_unicode_keyboard-0.10/README.md
-drwxrwxrwx   0        0        0        0 2022-11-30 02:38:38.427808 adb_unicode_keyboard-0.10/adb_unicode_keyboard/
--rw-rw-rw-   0        0        0     1069 2022-10-02 04:27:48.000000 adb_unicode_keyboard-0.10/adb_unicode_keyboard/LICENSE
--rw-rw-rw-   0        0        0     1385 2022-11-30 02:34:33.000000 adb_unicode_keyboard-0.10/adb_unicode_keyboard/README.MD
--rw-rw-rw-   0        0        0    58786 2022-11-30 02:34:55.000000 adb_unicode_keyboard-0.10/adb_unicode_keyboard/__init__.py
--rw-rw-rw-   0        0        0       51 2022-11-30 02:38:37.000000 adb_unicode_keyboard-0.10/adb_unicode_keyboard/requirements.txt
--rw-rw-rw-   0        0        0        2 2022-11-30 02:38:37.000000 adb_unicode_keyboard-0.10/adb_unicode_keyboard/thirdparty.json
-drwxrwxrwx   0        0        0        0 2022-11-30 02:38:38.430735 adb_unicode_keyboard-0.10/adb_unicode_keyboard.egg-info/
--rw-rw-rw-   0        0        0     2336 2022-11-30 02:38:38.000000 adb_unicode_keyboard-0.10/adb_unicode_keyboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      439 2022-11-30 02:38:38.000000 adb_unicode_keyboard-0.10/adb_unicode_keyboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-30 02:38:38.000000 adb_unicode_keyboard-0.10/adb_unicode_keyboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2022-11-30 02:38:38.000000 adb_unicode_keyboard-0.10/adb_unicode_keyboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2022-11-30 02:38:38.000000 adb_unicode_keyboard-0.10/adb_unicode_keyboard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      115 2022-11-30 02:38:38.431711 adb_unicode_keyboard-0.10/setup.cfg
--rw-rw-rw-   0        0        0     1520 2022-11-30 02:38:37.000000 adb_unicode_keyboard-0.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:01:17.287182 adb_unicode_keyboard-0.11/
+-rw-rw-rw-   0        0        0     1148 2023-05-29 01:01:06.000000 adb_unicode_keyboard-0.11/LICENSE.rst
+-rw-rw-rw-   0        0        0      131 2023-05-29 01:01:06.000000 adb_unicode_keyboard-0.11/MANIFEST.in
+-rw-rw-rw-   0        0        0     2039 2023-05-29 01:01:17.287182 adb_unicode_keyboard-0.11/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2023-04-15 00:18:28.000000 adb_unicode_keyboard-0.11/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 01:01:17.283180 adb_unicode_keyboard-0.11/adb_unicode_keyboard/
+-rw-rw-rw-   0        0        0     1385 2023-04-15 00:18:28.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard/README.MD
+-rw-rw-rw-   0        0        0    58943 2023-05-29 00:54:24.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard/__init__.py
+-rw-rw-rw-   0        0        0       51 2023-05-29 01:01:16.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard/requirements.txt
+-rw-rw-rw-   0        0        0    26472 2023-05-29 01:01:16.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-29 01:01:17.286172 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/
+-rw-rw-rw-   0        0        0     2039 2023-05-29 01:01:17.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-05-29 01:01:17.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 01:01:17.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-29 01:01:17.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-29 01:01:17.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-29 01:01:17.288167 adb_unicode_keyboard-0.11/setup.cfg
+-rw-rw-rw-   0        0        0     1420 2023-05-29 01:01:16.000000 adb_unicode_keyboard-0.11/setup.py
```

### Comparing `adb_unicode_keyboard-0.10/LICENSE.rst` & `adb_unicode_keyboard-0.11/LICENSE.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
  The MIT License (MIT)
- Copyright (c) 2022 Johannes Fischer
+ Copyright (c) 2023 Johannes Fischer
  
  Permission is hereby granted, free of charge, to any person obtaining a copy
  of this software and associated documentation files (the "Software"), to deal
  in the Software without restriction, including without limitation the rights
  to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
  copies of the Software, and to permit persons to whom the Software is
  furnished to do so, subject to the following conditions:
```

### Comparing `adb_unicode_keyboard-0.10/PKG-INFO` & `adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,55 +1,50 @@
 Metadata-Version: 2.1
-Name: adb_unicode_keyboard
-Version: 0.10
+Name: adb-unicode-keyboard
+Version: 0.11
 Summary: Send any Unicode character to your Android device
 Home-page: https://github.com/hansalemaos/adb_unicode_keyboard
 Author: Johannes Fischer
-Author-email: <aulasparticularesdealemaosp@gmail.com>
+Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,unicode,keyboard
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Scientific/Engineering :: Visualization
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Text Editors :: Text Processing
-Classifier: Topic :: Text Processing :: General
-Classifier: Topic :: Text Processing :: Indexing
-Classifier: Topic :: Text Processing :: Filters
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 License-File: LICENSE.rst
 
 
-### Send any Unicode character to your Android device
-
-```python
-pip install adb-unicode-keyboard
-
-from adb_unicode_keyboard import  AdbUnicodeKeyboard
-from time import sleep
-adbkeyboard = AdbUnicodeKeyboard(adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe",
-deviceserial = "localhost:5735", exit_keys="ctrl+x")
-adbkeyboard.connect_to_adb()
-oldkeyboard = adbkeyboard.get_all_installed_keyboards()[0]
-adbkeyboard.install_adb_keyboard() # installs "https://github.com/senzhk/ADBKeyBoard/raw/master/ADBKeyboard.apk"
-adbkeyboard.activate_adb_keyboard()
-if adbkeyboard.is_keyboard_shown():
-
-    adbkeyboard.send_unicode_text('öü')
-    adbkeyboard.send_unicode_text_with_delay('öü', delay_range=(0.05, 0.3))
-    sleep(1)
-    adbkeyboard.longpress_66_keycode_enter() # not executed with ADBKeyBoard / all keycodes are available as methods
-    sleep(1)
-    adbkeyboard.press_66_keycode_enter() # not executed with ADBKeyBoard  / all keycodes are available as methods
-
-adbkeyboard.disable_adb_keyboard(new_keyboard_name=None) # If no keyboard name is passed, will be reset to default
-adbkeyboard.disable_adb_keyboard(new_keyboard_name=oldkeyboard)
-
-#adbkeyboard.uninstall_adb_keyboard()
-
-# Chaining is possible
-adbkeyboard.connect_to_adb().activate_adb_keyboard().send_unicode_text('böb&oö').disable_adb_keyboard()
-
-```
-
+### Send any Unicode character to your Android device
+
+```python
+pip install adb-unicode-keyboard
+
+from adb_unicode_keyboard import  AdbUnicodeKeyboard
+from time import sleep
+adbkeyboard = AdbUnicodeKeyboard(adb_path = "C:\\Users\\Gamer\\AppData\\Local\\Android\\Sdk\\platform-tools\\adb.exe",
+deviceserial = "localhost:5735", exit_keys="ctrl+x")
+adbkeyboard.connect_to_adb()
+oldkeyboard = adbkeyboard.get_all_installed_keyboards()[0]
+adbkeyboard.install_adb_keyboard() # installs "https://github.com/senzhk/ADBKeyBoard/raw/master/ADBKeyboard.apk"
+adbkeyboard.activate_adb_keyboard()
+if adbkeyboard.is_keyboard_shown():
+
+    adbkeyboard.send_unicode_text('öü')
+    adbkeyboard.send_unicode_text_with_delay('öü', delay_range=(0.05, 0.3))
+    sleep(1)
+    adbkeyboard.longpress_66_keycode_enter() # not executed with ADBKeyBoard / all keycodes are available as methods
+    sleep(1)
+    adbkeyboard.press_66_keycode_enter() # not executed with ADBKeyBoard  / all keycodes are available as methods
+
+adbkeyboard.disable_adb_keyboard(new_keyboard_name=None) # If no keyboard name is passed, will be reset to default
+adbkeyboard.disable_adb_keyboard(new_keyboard_name=oldkeyboard)
+
+#adbkeyboard.uninstall_adb_keyboard()
+
+# Chaining is possible
+adbkeyboard.connect_to_adb().activate_adb_keyboard().send_unicode_text('böb&oö').disable_adb_keyboard()
+
+```
+
```

### Comparing `adb_unicode_keyboard-0.10/README.md` & `adb_unicode_keyboard-0.11/README.md`

 * *Files identical despite different names*

### Comparing `adb_unicode_keyboard-0.10/adb_unicode_keyboard/README.MD` & `adb_unicode_keyboard-0.11/adb_unicode_keyboard/README.MD`

 * *Files identical despite different names*

### Comparing `adb_unicode_keyboard-0.10/adb_unicode_keyboard/__init__.py` & `adb_unicode_keyboard-0.11/adb_unicode_keyboard/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1754,14 +1754,18 @@
         ).stdout.decode("utf-8", "ignore")
 
     def activate_adb_keyboard(self):
         keyboards = self.get_all_installed_keyboards()
         keyba = [x for x in keyboards if "com.android.adbkeyboard" in x][0]
         execute_adb_command(
             cmd=f"{self.adb_path} -s {self.deviceserial} shell",
+            subcommands=[f"ime enable {keyba}"],
+        )
+        execute_adb_command(
+            cmd=f"{self.adb_path} -s {self.deviceserial} shell",
             subcommands=[f"ime set {keyba}"],
         )
         return self
 
     def disable_adb_keyboard(self, new_keyboard_name=None):
         if new_keyboard_name is None:
             keyboards = self.get_all_installed_keyboards()
```

### Comparing `adb_unicode_keyboard-0.10/setup.py` & `adb_unicode_keyboard-0.11/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 from setuptools import setup, find_packages
 import codecs
 import os
-
-#change to dict
+# 
 here = os.path.abspath(os.path.dirname(__file__))
+# 
+with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
+    long_description = "\n" + fh.read()\
 
-with codecs.open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
-    long_description = "\n" + fh.read()
+from pathlib import Path
+this_directory = Path(__file__).parent
+#long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.10'
-DESCRIPTION = "Send any Unicode character to your Android device"
+VERSION = '''0.11'''
+DESCRIPTION = '''Send any Unicode character to your Android device'''
 
 # Setting up
 setup(
     name="adb_unicode_keyboard",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/adb_unicode_keyboard',
     author="Johannes Fischer",
-    author_email="<aulasparticularesdealemaosp@gmail.com>",
+    author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
-    long_description_content_type="text/markdown",
-    long_description=long_description,
-    #packages=['flexible_partial', 'keyboard', 'psutil', 'regex', 'requests'],
+long_description = long_description,
+long_description_content_type="text/markdown",
+    #packages=['flexible_partial', 'keyboard', 'psutil', 'regex', 'Requests'],
     keywords=['adb', 'android', 'unicode', 'keyboard'],
-    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.9', 'Topic :: Scientific/Engineering :: Visualization', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Text Editors :: Text Processing', 'Topic :: Text Processing :: General', 'Topic :: Text Processing :: Indexing', 'Topic :: Text Processing :: Filters', 'Topic :: Utilities'],
-    install_requires=['flexible_partial', 'keyboard', 'psutil', 'regex', 'requests'],
+    classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
+    install_requires=['flexible_partial', 'keyboard', 'psutil', 'regex', 'Requests'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```


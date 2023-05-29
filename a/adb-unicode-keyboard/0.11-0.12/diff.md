# Comparing `tmp/adb_unicode_keyboard-0.11.tar.gz` & `tmp/adb_unicode_keyboard-0.12.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adb_unicode_keyboard-0.11.tar", last modified: Mon May 29 01:01:17 2023, max compression
+gzip compressed data, was "adb_unicode_keyboard-0.12.tar", last modified: Mon May 29 01:58:38 2023, max compression
```

## Comparing `adb_unicode_keyboard-0.11.tar` & `adb_unicode_keyboard-0.12.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 01:01:17.287182 adb_unicode_keyboard-0.11/
--rw-rw-rw-   0        0        0     1148 2023-05-29 01:01:06.000000 adb_unicode_keyboard-0.11/LICENSE.rst
--rw-rw-rw-   0        0        0      131 2023-05-29 01:01:06.000000 adb_unicode_keyboard-0.11/MANIFEST.in
--rw-rw-rw-   0        0        0     2039 2023-05-29 01:01:17.287182 adb_unicode_keyboard-0.11/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2023-04-15 00:18:28.000000 adb_unicode_keyboard-0.11/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 01:01:17.283180 adb_unicode_keyboard-0.11/adb_unicode_keyboard/
--rw-rw-rw-   0        0        0     1385 2023-04-15 00:18:28.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard/README.MD
--rw-rw-rw-   0        0        0    58943 2023-05-29 00:54:24.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard/__init__.py
--rw-rw-rw-   0        0        0       51 2023-05-29 01:01:16.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard/requirements.txt
--rw-rw-rw-   0        0        0    26472 2023-05-29 01:01:16.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-05-29 01:01:17.286172 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/
--rw-rw-rw-   0        0        0     2039 2023-05-29 01:01:17.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2023-05-29 01:01:17.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 01:01:17.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-05-29 01:01:17.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-29 01:01:17.000000 adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-05-29 01:01:17.288167 adb_unicode_keyboard-0.11/setup.cfg
--rw-rw-rw-   0        0        0     1420 2023-05-29 01:01:16.000000 adb_unicode_keyboard-0.11/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 01:58:38.615830 adb_unicode_keyboard-0.12/
+-rw-rw-rw-   0        0        0     1148 2023-05-29 01:58:30.000000 adb_unicode_keyboard-0.12/LICENSE.rst
+-rw-rw-rw-   0        0        0      131 2023-05-29 01:58:29.000000 adb_unicode_keyboard-0.12/MANIFEST.in
+-rw-rw-rw-   0        0        0     2039 2023-05-29 01:58:38.615830 adb_unicode_keyboard-0.12/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2023-05-29 01:02:44.000000 adb_unicode_keyboard-0.12/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 01:58:38.612838 adb_unicode_keyboard-0.12/adb_unicode_keyboard/
+-rw-rw-rw-   0        0        0     1385 2023-05-29 01:02:44.000000 adb_unicode_keyboard-0.12/adb_unicode_keyboard/README.MD
+-rw-rw-rw-   0        0        0    58943 2023-05-29 01:02:44.000000 adb_unicode_keyboard-0.12/adb_unicode_keyboard/__init__.py
+-rw-rw-rw-   0        0        0       51 2023-05-29 01:58:37.000000 adb_unicode_keyboard-0.12/adb_unicode_keyboard/requirements.txt
+-rw-rw-rw-   0        0        0    26472 2023-05-29 01:58:37.000000 adb_unicode_keyboard-0.12/adb_unicode_keyboard/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-05-29 01:58:38.614833 adb_unicode_keyboard-0.12/adb_unicode_keyboard.egg-info/
+-rw-rw-rw-   0        0        0     2039 2023-05-29 01:58:38.000000 adb_unicode_keyboard-0.12/adb_unicode_keyboard.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      410 2023-05-29 01:58:38.000000 adb_unicode_keyboard-0.12/adb_unicode_keyboard.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 01:58:38.000000 adb_unicode_keyboard-0.12/adb_unicode_keyboard.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-05-29 01:58:38.000000 adb_unicode_keyboard-0.12/adb_unicode_keyboard.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-29 01:58:38.000000 adb_unicode_keyboard-0.12/adb_unicode_keyboard.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-05-29 01:58:38.616827 adb_unicode_keyboard-0.12/setup.cfg
+-rw-rw-rw-   0        0        0     1420 2023-05-29 01:58:37.000000 adb_unicode_keyboard-0.12/setup.py
```

### Comparing `adb_unicode_keyboard-0.11/LICENSE.rst` & `adb_unicode_keyboard-0.12/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `adb_unicode_keyboard-0.11/PKG-INFO` & `adb_unicode_keyboard-0.12/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb_unicode_keyboard
-Version: 0.11
+Version: 0.12
 Summary: Send any Unicode character to your Android device
 Home-page: https://github.com/hansalemaos/adb_unicode_keyboard
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,unicode,keyboard
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adb_unicode_keyboard-0.11/README.md` & `adb_unicode_keyboard-0.12/README.md`

 * *Files identical despite different names*

### Comparing `adb_unicode_keyboard-0.11/adb_unicode_keyboard/README.MD` & `adb_unicode_keyboard-0.12/adb_unicode_keyboard/README.MD`

 * *Files identical despite different names*

### Comparing `adb_unicode_keyboard-0.11/adb_unicode_keyboard/__init__.py` & `adb_unicode_keyboard-0.12/adb_unicode_keyboard/__init__.py`

 * *Files identical despite different names*

### Comparing `adb_unicode_keyboard-0.11/adb_unicode_keyboard/thirdparty.json` & `adb_unicode_keyboard-0.12/adb_unicode_keyboard/thirdparty.json`

 * *Files identical despite different names*

### Comparing `adb_unicode_keyboard-0.11/adb_unicode_keyboard.egg-info/PKG-INFO` & `adb_unicode_keyboard-0.12/adb_unicode_keyboard.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adb-unicode-keyboard
-Version: 0.11
+Version: 0.12
 Summary: Send any Unicode character to your Android device
 Home-page: https://github.com/hansalemaos/adb_unicode_keyboard
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,unicode,keyboard
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adb_unicode_keyboard-0.11/setup.py` & `adb_unicode_keyboard-0.12/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.11'''
+VERSION = '''0.12'''
 DESCRIPTION = '''Send any Unicode character to your Android device'''
 
 # Setting up
 setup(
     name="adb_unicode_keyboard",
     version=VERSION,
     license='MIT',
     url = 'https://github.com/hansalemaos/adb_unicode_keyboard',
     author="Johannes Fischer",
     author_email="aulasparticularesdealemaosp@gmail.com",
     description=DESCRIPTION,
 long_description = long_description,
 long_description_content_type="text/markdown",
-    #packages=['flexible_partial', 'keyboard', 'psutil', 'regex', 'Requests'],
+    #packages=['flexible_partial', 'keyboard', 'psutil', 'regex', 'requests'],
     keywords=['adb', 'android', 'unicode', 'keyboard'],
     classifiers=['Development Status :: 4 - Beta', 'Programming Language :: Python :: 3 :: Only', 'Programming Language :: Python :: 3.10', 'Topic :: Software Development :: Libraries :: Python Modules', 'Topic :: Utilities'],
-    install_requires=['flexible_partial', 'keyboard', 'psutil', 'regex', 'Requests'],
+    install_requires=['flexible_partial', 'keyboard', 'psutil', 'regex', 'requests'],
     include_package_data=True
 )
 #python setup.py sdist bdist_wheel
 #twine upload dist/*
```


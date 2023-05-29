# Comparing `tmp/consoleprinter-93.tar.gz` & `tmp/consoleprinter-95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/consoleprinter-93.tar", last modified: Tue May 30 14:09:29 2017, max compression
+gzip compressed data, was "consoleprinter-95.tar", last modified: Mon May 29 08:24:51 2023, max compression
```

## Comparing `consoleprinter-93.tar` & `consoleprinter-95.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 rabshakeh   (502) staff       (20)        0 2017-05-30 14:09:29.000000 consoleprinter-93/
-drwxr-xr-x   0 rabshakeh   (502) staff       (20)        0 2017-05-30 14:09:29.000000 consoleprinter-93/consoleprinter/
--rw-r--r--   0 rabshakeh   (502) staff       (20)    98019 2017-02-07 14:39:14.000000 consoleprinter-93/consoleprinter/__init__.py
-drwxr-xr-x   0 rabshakeh   (502) staff       (20)        0 2017-05-30 14:09:29.000000 consoleprinter-93/consoleprinter.egg-info/
--rw-r--r--   0 rabshakeh   (502) staff       (20)        1 2017-05-30 14:09:29.000000 consoleprinter-93/consoleprinter.egg-info/dependency_links.txt
--rw-r--r--   0 rabshakeh   (502) staff       (20)      668 2017-05-30 14:09:29.000000 consoleprinter-93/consoleprinter.egg-info/PKG-INFO
--rw-r--r--   0 rabshakeh   (502) staff       (20)       28 2017-05-30 14:09:29.000000 consoleprinter-93/consoleprinter.egg-info/requires.txt
--rw-r--r--   0 rabshakeh   (502) staff       (20)      268 2017-05-30 14:09:29.000000 consoleprinter-93/consoleprinter.egg-info/SOURCES.txt
--rw-r--r--   0 rabshakeh   (502) staff       (20)       15 2017-05-30 14:09:29.000000 consoleprinter-93/consoleprinter.egg-info/top_level.txt
--rw-r--r--   0 rabshakeh   (502) staff       (20)        1 2017-05-30 14:09:29.000000 consoleprinter-93/consoleprinter.egg-info/zip-safe
--rw-r--r--   0 rabshakeh   (502) staff       (20)      668 2017-05-30 14:09:29.000000 consoleprinter-93/PKG-INFO
--rw-r--r--   0 rabshakeh   (502) staff       (20)     2962 2017-05-30 14:09:28.000000 consoleprinter-93/README.rst
--rw-r--r--   0 rabshakeh   (502) staff       (20)       59 2017-05-30 14:09:29.000000 consoleprinter-93/setup.cfg
--rw-r--r--   0 rabshakeh   (502) staff       (20)      917 2017-05-29 12:23:17.000000 consoleprinter-93/setup.py
+drwxr-xr-x   0 rabshakeh   (501) staff       (20)        0 2023-05-29 08:24:51.341131 consoleprinter-95/
+-rw-r--r--   0 rabshakeh   (501) staff       (20)    18027 2017-12-18 21:19:52.000000 consoleprinter-95/LICENSE
+-rw-r--r--   0 rabshakeh   (501) staff       (20)      651 2023-05-29 08:24:51.340634 consoleprinter-95/PKG-INFO
+-rw-r--r--   0 rabshakeh   (501) staff       (20)     2899 2023-05-29 08:24:50.000000 consoleprinter-95/README.rst
+drwxr-xr-x   0 rabshakeh   (501) staff       (20)        0 2023-05-29 08:24:51.336333 consoleprinter-95/consoleprinter/
+-rw-r--r--   0 rabshakeh   (501) staff       (20)    98043 2023-05-29 08:10:05.000000 consoleprinter-95/consoleprinter/__init__.py
+drwxr-xr-x   0 rabshakeh   (501) staff       (20)        0 2023-05-29 08:24:51.339873 consoleprinter-95/consoleprinter.egg-info/
+-rw-r--r--   0 rabshakeh   (501) staff       (20)      651 2023-05-29 08:24:51.000000 consoleprinter-95/consoleprinter.egg-info/PKG-INFO
+-rw-r--r--   0 rabshakeh   (501) staff       (20)      276 2023-05-29 08:24:51.000000 consoleprinter-95/consoleprinter.egg-info/SOURCES.txt
+-rw-r--r--   0 rabshakeh   (501) staff       (20)        1 2023-05-29 08:24:51.000000 consoleprinter-95/consoleprinter.egg-info/dependency_links.txt
+-rw-r--r--   0 rabshakeh   (501) staff       (20)       28 2023-05-29 08:24:51.000000 consoleprinter-95/consoleprinter.egg-info/requires.txt
+-rw-r--r--   0 rabshakeh   (501) staff       (20)       15 2023-05-29 08:24:51.000000 consoleprinter-95/consoleprinter.egg-info/top_level.txt
+-rw-r--r--   0 rabshakeh   (501) staff       (20)        1 2023-05-29 08:24:51.000000 consoleprinter-95/consoleprinter.egg-info/zip-safe
+-rw-r--r--   0 rabshakeh   (501) staff       (20)       38 2023-05-29 08:24:51.341261 consoleprinter-95/setup.cfg
+-rw-r--r--   0 rabshakeh   (501) staff       (20)      917 2018-12-27 13:50:41.000000 consoleprinter-95/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `consoleprinter-93/consoleprinter/__init__.py` & `consoleprinter-95/consoleprinter/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -652,15 +652,15 @@
 
 
 def strex(val):
     """
     @type val: str
     @return: None
     """
-    return val is not "" and val is not None
+    return val != "" and val != None
 
 
 def camel_case(mystring, uppercase_first_letter=True, remove_spaces=True):
     """
     @type mystring: str
     @type uppercase_first_letter: bool
     @type remove_spaces: bool
@@ -2256,15 +2256,15 @@
     try:
         answer = input("$: ").lower()
     except KeyboardInterrupt:
         answer = "quit"
 
     answer = get_safe_string(answer.strip())
 
-    if answer is "" and default is not None:
+    if answer == "" and default != None:
         answer = default
     try:
         answeri = int(answer)
 
         if str(answeri) == answer:
             answer = answeri
     except ValueError:
@@ -2314,15 +2314,15 @@
 
         if numdashes > currnumdashes:
             s += "\n"
 
         currnumdashes = numdashes
         numspaces = i.count(" ") - i.lstrip(" ").count(" ")
 
-        if numspaces is 0 and currnumspaces > 0:
+        if numspaces == 0 and currnumspaces > 0:
             if not s.endswith("\n\n"):
                 s += "\n"
 
         currnumspaces = numspaces
         ls = [x for x in i.split(":") if x]
         cnt = 0
 
@@ -2405,26 +2405,26 @@
 def get_safe_filename_string(filepath):
     """
     @type filepath: string
     @return: string
     """
     hiddenfile = os.path.basename(filepath).startswith(".")
 
-    s = os.path.basename(filepath).replace(' ', '_').replace('__', '_').replace('___', '_').replace('..', '.').replace('._', '_').lower().replace('|', '_').replace('\'', '').lower().strip('_')
+    s = os.path.basename(filepath).replace('.', '_').replace(' ', '_').replace('__', '_').replace('___', '_').replace('..', '.').replace('._', '_').lower().replace('|', '_').replace('\'', '').lower().strip('_')
     s = get_safe_string(s)
     if hiddenfile:
         s = "."+s
     return s
 
 def get_safe_filepath_string(filepath):
     """
     @type filepath: string
     @return: string
     """
-    s = filepath.replace(' ', '_').replace('-', '_').replace('__', '_').replace('___', '_').replace('..', '.').replace('._', '_').lower().replace('|', '_').replace('\'', '').lower().strip('_')
+    s = filepath.replace('.', '_').replace(' ', '_').replace('-', '_').replace('__', '_').replace('___', '_').replace('..', '.').replace('._', '_').lower().replace('|', '_').replace('\'', '').lower().strip('_')
     s = get_safe_string(s, extrachars='/')
     return s
 
 def get_value_as_text(colors, indent, return_string, value, dbs, plaintext=False, iterate_members=False):
     """
     @type colors: dict
     @type indent: int
```

### Comparing `consoleprinter-93/consoleprinter.egg-info/PKG-INFO` & `consoleprinter-95/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: consoleprinter
-Version: 93
+Version: 95
 Summary: Console printer with linenumbers, stacktraces, logging, conversions and coloring..
 Home-page: https://github.com/erikdejonge/consoleprinter
 Author: Erik de Jonge
 Author-email: erik@a8.nl
 License: GPL
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System
+License-File: LICENSE
```

### Comparing `consoleprinter-93/PKG-INFO` & `consoleprinter-95/consoleprinter.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: consoleprinter
-Version: 93
+Version: 95
 Summary: Console printer with linenumbers, stacktraces, logging, conversions and coloring..
 Home-page: https://github.com/erikdejonge/consoleprinter
 Author: Erik de Jonge
 Author-email: erik@a8.nl
 License: GPL
-Description: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)
 Classifier: Operating System :: POSIX
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System
+License-File: LICENSE
```

### Comparing `consoleprinter-93/README.rst` & `consoleprinter-95/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,133 +2,136 @@
 ==============
 
 Console printer with linenumbers, stacktraces, logging, conversions and
 coloring.
 
 ::
 
-    Active8 BV
-    Active8 (05-03-15)
-    license: GNU-GPL2
+   Active8 BV
+   Active8 (05-03-15)
+   license: GNU-GPL2
 
-    .. figure:: res/consoleprinter.gif
-       :alt: animation
+..
 
-       animation
+   .. figure:: res/consoleprinter.gif
+      :alt: animation
 
-example
-~~~~~~~
+      animation
+
+###example
 
 Add a method call to console somewhere in your code, for example
 
 .. code:: python
 
-    console(os, print_stack=True, color="red")
+   console(os, print_stack=True, color="red")
+
+..
 
-    .. figure:: res/code.png
-       :alt: code
+   .. figure:: res/code.png
+      :alt: code
 
-       code
+      code
 
 It will give a stacktrace in the terminal
 
-    .. figure:: res/terminal2.png
-       :alt: tterminal
+   .. figure:: res/terminal2.png
+      :alt: tterminal
 
-       tterminal
+      tterminal
 
 If the printer detects an object it will try to do a dir an give the
 layout with values
 
 .. code:: python
 
 
-    class MyObject(object):
-        """
-        MyObject
-        """
-        m_float = 8.0
-        m_string = "hello"
-        m_int = 8
-
-        @staticmethod
-        def foo():
-            """
-            foo
-            """
-            pass
-
-        def __str__(self):
-            """
-            __str__
-            """
-            return "My Little Object"
+   class MyObject(object):
+       """
+       MyObject
+       """
+       m_float = 8.0
+       m_string = "hello"
+       m_int = 8
+
+       @staticmethod
+       def foo():
+           """
+           foo
+           """
+           pass
+
+       def __str__(self):
+           """
+           __str__
+           """
+           return "My Little Object"
+
+   mo = MyObject()
+   console(mo)
 
-    mo = MyObject()
-    console(mo)
+..
 
-    .. figure:: res/object.png
-       :alt: object
+   .. figure:: res/object.png
+      :alt: object
 
-       object
+      object
 
 .. code:: bash
 
-    0.17 | arguments/__init__.py", line 957 (print_commandline_help) | <arguments.Arguments.print_commandline_help.<locals.MyObject object at 0x1034026d8>: My Little Object
-         | MyObject                          type                           value
-         | ------------------------------------------------------------------------------------------
-         | foo                               function
-         | m_float                           float                          8.0
-         | m_int                             int                            8
-         | m_string                          str                            hello
+   0.17 | arguments/__init__.py", line 957 (print_commandline_help) | <arguments.Arguments.print_commandline_help.<locals.MyObject object at 0x1034026d8>: My Little Object
+        | MyObject                          type                           value
+        | ------------------------------------------------------------------------------------------
+        | foo                               function
+        | m_float                           float                          8.0
+        | m_int                             int                            8
+        | m_string                          str                            hello
 
-install
--------
+##install
 
 .. code:: bash
 
-    pip install consoleprinter
+   pip install consoleprinter
 
-contains
---------
+##contains Utility functions for working with commandline applications.
+Logging Printing Exception parsing Stacktracing Object reflection
+printing
 
-Utility functions for working with commandline applications. Logging
-Printing Exception parsing Stacktracing Object reflection printing
-
-usage
------
+##usage
 
 .. code:: python
 
-    from consoleprinter import console
+   from consoleprinter import console
 
-    colors = ['black', 'blue', 'cyan', 'default', 'green', 'grey', 'magenta', 'orange', 'red', 'white', 'yellow']
+   colors = ['black', 'blue', 'cyan', 'default', 'green', 'grey', 'magenta', 'orange', 'red', 'white', 'yellow']
 
-    for color in colors:
-        console(color, color=color)
+   for color in colors:
+       console(color, color=color)
 
 PyCharm
 -------
 
 Console detects when run in PyCharm or Intellij, and adds links to the
 orinating line
 
 .. code:: python
 
-        if len(suite._tests) == 0:
-            console_warning("Can't find tests, looked in test*.py")
+       if len(suite._tests) == 0:
+           console_warning("Can't find tests, looked in test*.py")
 
-\`\ ``bash 2.48 | unittester.py:85 | == | Can't find tests, looked in test*.py | File "/Users/rabshakeh/workspace/unittester/unittester/unittester.py", line 85 (run_unit_test) | ==``
+.. code:: bash
 
-Reflection
-----------
+   2.48 | unittester.py:85 | == | Can't find tests, looked in test*.py | File "/Users/rabshakeh/workspace/unittester/unittester/unittester.py", line 85 (run_unit_test) | ==
+   ``
 
-.. code:: python
+   ##Reflection
+   ```python
+   with zipfile.ZipFile(zippath) as zf:
+       for member in zf.infolist():
+           console(member)
 
-    with zipfile.ZipFile(zippath) as zf:
-        for member in zf.infolist():
-            console(member)
+..
 
-    .. figure:: res/Screen%20Shot%202015-03-17%20at%2017.45.50.png
-       :alt: console
+   .. figure:: res/Screen%20Shot%202015-03-17%20at%2017.45.50.png
+      :alt: console
 
-       console
+      console
```

### Comparing `consoleprinter-93/setup.py` & `consoleprinter-95/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 appinstance
 Active8 (04-03-15)
 license: GNU-GPL2
 """
 
 from setuptools import setup
 setup(name='consoleprinter',
-      version='93',
+      version='95',
       description='Console printer with linenumbers, stacktraces, logging, conversions and coloring..',
       url='https://github.com/erikdejonge/consoleprinter',
       author='Erik de Jonge',
       author_email='erik@a8.nl',
       license='GPL',
       packages=['consoleprinter'],
       zip_safe=True,
```


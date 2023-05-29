# Comparing `tmp/testcell-0.0.5.tar.gz` & `tmp/testcell-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcell-0.0.5.tar", last modified: Sun May 14 22:08:32 2023, max compression
+gzip compressed data, was "testcell-0.0.6.tar", last modified: Mon May 29 08:01:55 2023, max compression
```

## Comparing `testcell-0.0.5.tar` & `testcell-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-14 22:08:32.995519 testcell-0.0.5/
--rw-rw-r--   0 dldev     (1000) dldev     (1000)    11357 2023-05-01 12:51:46.000000 testcell-0.0.5/LICENSE
--rw-rw-r--   0 dldev     (1000) dldev     (1000)      111 2023-04-27 10:12:58.000000 testcell-0.0.5/MANIFEST.in
--rw-r--r--   0 dldev     (1000) dldev     (1000)     6222 2023-05-14 22:08:32.995519 testcell-0.0.5/PKG-INFO
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     5400 2023-05-13 16:03:22.000000 testcell-0.0.5/README.md
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     1018 2023-05-14 22:04:21.000000 testcell-0.0.5/settings.ini
--rw-r--r--   0 dldev     (1000) dldev     (1000)       38 2023-05-14 22:08:32.995519 testcell-0.0.5/setup.cfg
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     2596 2023-04-27 10:12:58.000000 testcell-0.0.5/setup.py
-drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-14 22:08:32.991518 testcell-0.0.5/testcell/
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     1289 2023-05-14 22:04:21.000000 testcell-0.0.5/testcell/__init__.py
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     1612 2023-05-14 22:04:21.000000 testcell-0.0.5/testcell/_modidx.py
--rw-rw-r--   0 dldev     (1000) dldev     (1000)     3175 2023-05-14 22:04:21.000000 testcell-0.0.5/testcell/core.py
-drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-14 22:08:32.995519 testcell-0.0.5/testcell.egg-info/
--rw-r--r--   0 dldev     (1000) dldev     (1000)     6222 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/PKG-INFO
--rw-r--r--   0 dldev     (1000) dldev     (1000)      334 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/SOURCES.txt
--rw-r--r--   0 dldev     (1000) dldev     (1000)        1 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/dependency_links.txt
--rw-r--r--   0 dldev     (1000) dldev     (1000)       38 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/entry_points.txt
--rw-r--r--   0 dldev     (1000) dldev     (1000)        1 2023-05-01 13:54:05.000000 testcell-0.0.5/testcell.egg-info/not-zip-safe
--rw-r--r--   0 dldev     (1000) dldev     (1000)       25 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/requires.txt
--rw-r--r--   0 dldev     (1000) dldev     (1000)        9 2023-05-14 22:08:32.000000 testcell-0.0.5/testcell.egg-info/top_level.txt
+drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-29 08:01:55.449756 testcell-0.0.6/
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)    11357 2023-05-01 12:51:46.000000 testcell-0.0.6/LICENSE
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)      111 2023-04-27 10:12:58.000000 testcell-0.0.6/MANIFEST.in
+-rw-r--r--   0 dldev     (1000) dldev     (1000)     7061 2023-05-29 08:01:55.449756 testcell-0.0.6/PKG-INFO
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     6239 2023-05-29 07:52:53.000000 testcell-0.0.6/README.md
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     1018 2023-05-27 00:04:32.000000 testcell-0.0.6/settings.ini
+-rw-r--r--   0 dldev     (1000) dldev     (1000)       38 2023-05-29 08:01:55.449756 testcell-0.0.6/setup.cfg
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     2596 2023-04-27 10:12:58.000000 testcell-0.0.6/setup.py
+drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-29 08:01:55.449756 testcell-0.0.6/testcell/
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     2186 2023-05-29 07:41:48.000000 testcell-0.0.6/testcell/__init__.py
+-rw-r--r--   0 dldev     (1000) dldev     (1000)     1522 2023-05-29 07:41:48.000000 testcell-0.0.6/testcell/_modidx.py
+-rw-rw-r--   0 dldev     (1000) dldev     (1000)     2840 2023-05-29 07:41:48.000000 testcell-0.0.6/testcell/core.py
+drwxr-xr-x   0 dldev     (1000) dldev     (1000)        0 2023-05-29 08:01:55.449756 testcell-0.0.6/testcell.egg-info/
+-rw-r--r--   0 dldev     (1000) dldev     (1000)     7061 2023-05-29 08:01:55.000000 testcell-0.0.6/testcell.egg-info/PKG-INFO
+-rw-r--r--   0 dldev     (1000) dldev     (1000)      334 2023-05-29 08:01:55.000000 testcell-0.0.6/testcell.egg-info/SOURCES.txt
+-rw-r--r--   0 dldev     (1000) dldev     (1000)        1 2023-05-29 08:01:55.000000 testcell-0.0.6/testcell.egg-info/dependency_links.txt
+-rw-r--r--   0 dldev     (1000) dldev     (1000)       38 2023-05-29 08:01:55.000000 testcell-0.0.6/testcell.egg-info/entry_points.txt
+-rw-r--r--   0 dldev     (1000) dldev     (1000)        1 2023-05-01 13:54:05.000000 testcell-0.0.6/testcell.egg-info/not-zip-safe
+-rw-r--r--   0 dldev     (1000) dldev     (1000)       25 2023-05-29 08:01:55.000000 testcell-0.0.6/testcell.egg-info/requires.txt
+-rw-r--r--   0 dldev     (1000) dldev     (1000)        9 2023-05-29 08:01:55.000000 testcell-0.0.6/testcell.egg-info/top_level.txt
```

### Comparing `testcell-0.0.5/LICENSE` & `testcell-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `testcell-0.0.5/PKG-INFO` & `testcell-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcell
-Version: 0.0.5
+Version: 0.0.6
 Summary: testcell prevents your testing cells from affecting the global namespace
 Home-page: https://github.com/artste/testcell
 Author: Stefano Giomo
 Author-email: artste@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -24,26 +24,38 @@
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 **TL;DR**: `%%testcell` prevents your testing cells from affecting the
 global namespace.
 
 The Python cell magic `%%testcell` executes a cell without *polluting*
-the notebook’s global variables. This is useful whenever you want to
+the notebook’s global namespace. This is useful whenever you want to
 test your code without having any of the local variables escape that
 cell.
 
 What’s happening under the hood is that your cell code, before being
 executed, is wrapped in a temporary function that will be deleted after
-execution. To give you the feeling of “seamless integration” the last
-line is optionally wrapped with a `display` statement if needed.
+execution. To give you the feeling of *seamless integration* the last
+statement is optionally returned like it happens in a normal cell.
 
 **WARNING:** this don’t protect you from *the side effects of your code*
 like deleting a file or mutating the state of a global variable.
 
+<div>
+
+[![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/artste/testcell/blob/main/demo/testcell_demo.ipynb)
+
+</div>
+
+<div>
+
+[![](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/artste/introducing-testcell)
+
+</div>
+
 ## Install
 
 ``` sh
 pip install testcell
 ```
 
 ## How to use
@@ -63,32 +75,34 @@
 assert 'a' not in locals()
 ```
 
 What is happening under the hood is that `%%testcell` wraps your cell’s
 code with a function, execute it and then deletes it. Adding the
 `verbose` keywork will print which code will be executed.
 
+NOTE: The actual cell code is enclosed within `BEGIN` and `END` comment
+blocks for improved readability.
+
 ``` python
 %%testcell verbose
 a = "'a' is not polluting global scope"
 a
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
-        display( # %%testcell
-        a
-        ) # %%testcell
+        return a # %%testcell
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    _ # This will be added to global scope
     ### END
 
     "'a' is not polluting global scope"
 
 If you’re just interested in seeing what will be executed, but actually
 not executing it, you ca use `dryrun` option:
 
@@ -99,84 +113,100 @@
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
-        display( # %%testcell
-        a
-        ) # %%testcell
+        return a # %%testcell
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    if _ is not None: display(_)
     ### END
 
-On top of *wrapping* your cell’s code, it will optinally add a
-`display(...)` call on your last cell’s row, trying to emulate what a
-real cell usually does. If you explicitly add a semicolon `;` in the
-end, this output will be suppressed.
+If you add a semicolon `;` at the end of your last statement no `return`
+statement is added and nothing is displayed like a normal jupyter cell.
 
 ``` python
 %%testcell verbose
 a = "'a' is not polluting global scope"
 a;
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
         a;
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    _ # This will be added to global scope
     ### END
 
-There are more cases where `display(...)` is avoided: \* `display`: if
-this is already present on the last line. \* `print`: even in this case
-no print is preserved and no other display call is added. \*
-`# comment...#`: these are preserved
+`testcell` works seamlessly with existing `print` or `display`statements
+on last line:
 
 ``` python
 %%testcell verbose
 a = "'a' is not polluting global scope"
 print(a)
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
-        print(a)
+        return print(a) # %%testcell
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    _ # This will be added to global scope
     ### END
     'a' is not polluting global scope
 
-### Run in isolation
+Moreover, thanks to `ast`, it properly deals with complex situations
+like comments on the last line and multi lines statements
 
-`%%testcelln` is a shourtcut for `%%testcell noglobals` and executes the
-cell in complete isolation from global scope. This is very useful when
-you want to be sure that global variables or namespace should be part of
-the cell.
+``` python
+%%testcell verbose
+a = "'a' is not polluting global scope"
+(a,
+ True)
+# this is a comment on last line
+```
 
-## Run in isolation
 
-`%%testcelln` is a shortcut for `%%testcell noglobals` and executes the
-cell in complete isolation from the global scope.
+    ### BEGIN
+    def _test_cell_():
+        #| echo: false
+        a = "'a' is not polluting global scope"
+        return (a,
+         True) # %%testcell
+    try:
+        _ = _test_cell_()
+    finally:
+        del _test_cell_
+    _ # This will be added to global scope
+    ### END
 
-This is very useful when you want to ensure that global variables or
-namespaces are not accessible within the cell.
+    ("'a' is not polluting global scope", True)
+
+### Run in isolation
+
+`%%testcelln` is a shortcut for `%%testcell noglobals` and executes the
+cell in complete isolation from the global scope. This is very useful
+when you want to ensure that global variables or namespaces are not
+accessible within the cell.
 
 ``` python
 aaa = 'global variable'
 ```
 
 ``` python
 %%testcell
@@ -200,20 +230,19 @@
     False
 
 ``` python
 %%testcelln
 globals().keys()
 ```
 
-    dict_keys(['__builtins__', '_test_cell_'])
+    dict_keys(['__builtins__'])
 
-Inside the cell, from the *global scope*, only these two items are
-available: + `__builtins__` : built in python’s functions. +
-`_test_cell_` : `%%testcell` wrapped function executed (we can’t avoid
-this).
+With `%%testcelln` inside the cell, you’ll be able to access only to
+`__builtins__` (aka: standard python’s functions). **It behaves like a
+notebook-in-notebook**.
 
 ``` python
 %%testcell
 def my_function(x):
     print(aaa) # global variable
     return x
 
@@ -265,12 +294,20 @@
 
     'modified global variable'
 
 ``` python
 del aaa
 ```
 
-## TODO:
+## Links:
+
+- PROJECT PAGE: <https://github.com/artste/testcell>
+- DOCUMENTATION: <https://artste.github.io/testcell>
+- PYPI: <https://pypi.org/project/testcell>
+- COLAB DEMO:
+  [testcell_demo.ipynb](https://colab.research.google.com/github/artste/testcell/blob/main/demo/testcell_demo.ipynb)
+- KAGGLE SAMPLE NOTEBOOK:
+  <https://www.kaggle.com/artste/introducing-testcell>
+
+## Todo:
 
 - Install as a plugin to enable it by default like other cell’s magic.
-- Eval possibility to run code on a new kernel to reduce even more
-  possible side effects.
```

### Comparing `testcell-0.0.5/README.md` & `testcell-0.0.6/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -2,26 +2,38 @@
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 **TL;DR**: `%%testcell` prevents your testing cells from affecting the
 global namespace.
 
 The Python cell magic `%%testcell` executes a cell without *polluting*
-the notebook’s global variables. This is useful whenever you want to
+the notebook’s global namespace. This is useful whenever you want to
 test your code without having any of the local variables escape that
 cell.
 
 What’s happening under the hood is that your cell code, before being
 executed, is wrapped in a temporary function that will be deleted after
-execution. To give you the feeling of “seamless integration” the last
-line is optionally wrapped with a `display` statement if needed.
+execution. To give you the feeling of *seamless integration* the last
+statement is optionally returned like it happens in a normal cell.
 
 **WARNING:** this don’t protect you from *the side effects of your code*
 like deleting a file or mutating the state of a global variable.
 
+<div>
+
+[![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/artste/testcell/blob/main/demo/testcell_demo.ipynb)
+
+</div>
+
+<div>
+
+[![](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/artste/introducing-testcell)
+
+</div>
+
 ## Install
 
 ``` sh
 pip install testcell
 ```
 
 ## How to use
@@ -41,32 +53,34 @@
 assert 'a' not in locals()
 ```
 
 What is happening under the hood is that `%%testcell` wraps your cell’s
 code with a function, execute it and then deletes it. Adding the
 `verbose` keywork will print which code will be executed.
 
+NOTE: The actual cell code is enclosed within `BEGIN` and `END` comment
+blocks for improved readability.
+
 ``` python
 %%testcell verbose
 a = "'a' is not polluting global scope"
 a
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
-        display( # %%testcell
-        a
-        ) # %%testcell
+        return a # %%testcell
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    _ # This will be added to global scope
     ### END
 
     "'a' is not polluting global scope"
 
 If you’re just interested in seeing what will be executed, but actually
 not executing it, you ca use `dryrun` option:
 
@@ -77,84 +91,100 @@
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
-        display( # %%testcell
-        a
-        ) # %%testcell
+        return a # %%testcell
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    if _ is not None: display(_)
     ### END
 
-On top of *wrapping* your cell’s code, it will optinally add a
-`display(...)` call on your last cell’s row, trying to emulate what a
-real cell usually does. If you explicitly add a semicolon `;` in the
-end, this output will be suppressed.
+If you add a semicolon `;` at the end of your last statement no `return`
+statement is added and nothing is displayed like a normal jupyter cell.
 
 ``` python
 %%testcell verbose
 a = "'a' is not polluting global scope"
 a;
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
         a;
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    _ # This will be added to global scope
     ### END
 
-There are more cases where `display(...)` is avoided: \* `display`: if
-this is already present on the last line. \* `print`: even in this case
-no print is preserved and no other display call is added. \*
-`# comment...#`: these are preserved
+`testcell` works seamlessly with existing `print` or `display`statements
+on last line:
 
 ``` python
 %%testcell verbose
 a = "'a' is not polluting global scope"
 print(a)
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
-        print(a)
+        return print(a) # %%testcell
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    _ # This will be added to global scope
     ### END
     'a' is not polluting global scope
 
-### Run in isolation
+Moreover, thanks to `ast`, it properly deals with complex situations
+like comments on the last line and multi lines statements
 
-`%%testcelln` is a shourtcut for `%%testcell noglobals` and executes the
-cell in complete isolation from global scope. This is very useful when
-you want to be sure that global variables or namespace should be part of
-the cell.
+``` python
+%%testcell verbose
+a = "'a' is not polluting global scope"
+(a,
+ True)
+# this is a comment on last line
+```
 
-## Run in isolation
 
-`%%testcelln` is a shortcut for `%%testcell noglobals` and executes the
-cell in complete isolation from the global scope.
+    ### BEGIN
+    def _test_cell_():
+        #| echo: false
+        a = "'a' is not polluting global scope"
+        return (a,
+         True) # %%testcell
+    try:
+        _ = _test_cell_()
+    finally:
+        del _test_cell_
+    _ # This will be added to global scope
+    ### END
 
-This is very useful when you want to ensure that global variables or
-namespaces are not accessible within the cell.
+    ("'a' is not polluting global scope", True)
+
+### Run in isolation
+
+`%%testcelln` is a shortcut for `%%testcell noglobals` and executes the
+cell in complete isolation from the global scope. This is very useful
+when you want to ensure that global variables or namespaces are not
+accessible within the cell.
 
 ``` python
 aaa = 'global variable'
 ```
 
 ``` python
 %%testcell
@@ -178,20 +208,19 @@
     False
 
 ``` python
 %%testcelln
 globals().keys()
 ```
 
-    dict_keys(['__builtins__', '_test_cell_'])
+    dict_keys(['__builtins__'])
 
-Inside the cell, from the *global scope*, only these two items are
-available: + `__builtins__` : built in python’s functions. +
-`_test_cell_` : `%%testcell` wrapped function executed (we can’t avoid
-this).
+With `%%testcelln` inside the cell, you’ll be able to access only to
+`__builtins__` (aka: standard python’s functions). **It behaves like a
+notebook-in-notebook**.
 
 ``` python
 %%testcell
 def my_function(x):
     print(aaa) # global variable
     return x
 
@@ -243,12 +272,20 @@
 
     'modified global variable'
 
 ``` python
 del aaa
 ```
 
-## TODO:
+## Links:
+
+- PROJECT PAGE: <https://github.com/artste/testcell>
+- DOCUMENTATION: <https://artste.github.io/testcell>
+- PYPI: <https://pypi.org/project/testcell>
+- COLAB DEMO:
+  [testcell_demo.ipynb](https://colab.research.google.com/github/artste/testcell/blob/main/demo/testcell_demo.ipynb)
+- KAGGLE SAMPLE NOTEBOOK:
+  <https://www.kaggle.com/artste/introducing-testcell>
+
+## Todo:
 
 - Install as a plugin to enable it by default like other cell’s magic.
-- Eval possibility to run code on a new kernel to reduce even more
-  possible side effects.
```

### Comparing `testcell-0.0.5/settings.ini` & `testcell-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = testcell
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = testcell
```

### Comparing `testcell-0.0.5/setup.py` & `testcell-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `testcell-0.0.5/testcell/_modidx.py` & `testcell-0.0.6/testcell/_modidx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # Autogenerated by nbdev
 
 d = { 'settings': { 'branch': 'main',
                 'doc_baseurl': '/testcell',
                 'doc_host': 'https://artste.github.io',
                 'git_url': 'https://github.com/artste/testcell',
                 'lib_path': 'testcell'},
-  'syms': { 'testcell.core': { 'testcell.core.auto_display': ('ast.html#auto_display', 'testcell/core.py'),
+  'syms': { 'testcell.core': { 'testcell.core.auto_return': ('ast.html#auto_return', 'testcell/core.py'),
                                'testcell.core.code_till_node': ('ast.html#code_till_node', 'testcell/core.py'),
+                               'testcell.core.end_of_last_line_of_code': ('ast.html#end_of_last_line_of_code', 'testcell/core.py'),
                                'testcell.core.extract_call': ('ast.html#extract_call', 'testcell/core.py'),
                                'testcell.core.is_assignment': ('ast.html#is_assignment', 'testcell/core.py'),
                                'testcell.core.is_ast_node': ('ast.html#is_ast_node', 'testcell/core.py'),
-                               'testcell.core.is_function_call': ('ast.html#is_function_call', 'testcell/core.py'),
                                'testcell.core.is_import_statement': ('ast.html#is_import_statement', 'testcell/core.py'),
                                'testcell.core.last_node': ('ast.html#last_node', 'testcell/core.py'),
                                'testcell.core.last_statement_has_semicolon': ('ast.html#last_statement_has_semicolon', 'testcell/core.py'),
-                               'testcell.core.need_display': ('ast.html#need_display', 'testcell/core.py'),
-                               'testcell.core.node_source': ('ast.html#node_source', 'testcell/core.py'),
-                               'testcell.core.wrap_node': ('ast.html#wrap_node', 'testcell/core.py')}}}
+                               'testcell.core.need_return': ('ast.html#need_return', 'testcell/core.py'),
+                               'testcell.core.node_source': ('ast.html#node_source', 'testcell/core.py')}}}
```

### Comparing `testcell-0.0.5/testcell/core.py` & `testcell-0.0.6/testcell/core.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/01_ast.ipynb.
 
 # %% auto 0
-__all__ = ['last_node', 'node_source', 'is_assignment', 'extract_call', 'is_function_call', 'is_import_statement', 'is_ast_node',
-           'need_display', 'wrap_node', 'last_statement_has_semicolon', 'code_till_node', 'auto_display']
+__all__ = ['last_node', 'node_source', 'is_assignment', 'extract_call', 'is_import_statement', 'is_ast_node', 'need_return',
+           'end_of_last_line_of_code', 'last_statement_has_semicolon', 'code_till_node', 'auto_return']
 
-# %% ../nbs/01_ast.ipynb 3
+# %% ../nbs/01_ast.ipynb 4
 import ast
 
 # %% ../nbs/01_ast.ipynb 5
 def last_node(code):
     tree = ast.parse(code)
     if len(tree.body)==0: return None
     src = tree.body[-1]
@@ -37,65 +37,57 @@
     if isinstance(node, ast.Call):
         n = node.func # step in
         if isinstance(n, ast.Name): return n.id # "fn()"
         if isinstance(n, ast.Attribute): return n.attr
     return None # all the rest is not supported
 
 # %% ../nbs/01_ast.ipynb 17
-def is_function_call(node,names):
-    function_name = extract_call(node)
-    if function_name is None: return False # this is not a function call
-    return function_name in names
-
-# %% ../nbs/01_ast.ipynb 19
 def is_import_statement(node):
     return isinstance(node, (ast.Import, ast.ImportFrom))
 
-# %% ../nbs/01_ast.ipynb 21
+# %% ../nbs/01_ast.ipynb 19
 def is_ast_node(x,ref):
     for t in ref:
         if isinstance(x,t): return True
     return False
 
-# %% ../nbs/01_ast.ipynb 24
-def need_display(node):
+# %% ../nbs/01_ast.ipynb 22
+def need_return(node):
     if node is None: return False
     if is_assignment(node): return False
-    if is_function_call(node,names=['print','display']): return False
     if is_ast_node(node,ref=[ast.Delete, ast.Assert, ast.Global, ast.Nonlocal]): return False
     if is_import_statement(node): return False
     return True
 
-# %% ../nbs/01_ast.ipynb 26
-def wrap_node(node,function_name):
-    return ast.Expr(
-        value=ast.Call(
-            func=ast.Name(id=function_name, ctx=ast.Load()),
-            args=[node],
-            keywords=[])
-        )
+# %% ../nbs/01_ast.ipynb 24
+def end_of_last_line_of_code(code:str,node):
+    if node is None: return ''
+    t = code.splitlines()
+    t = t[:node.lineno]
+    return t[-1][node.end_col_offset:]
 
-# %% ../nbs/01_ast.ipynb 29
+# %% ../nbs/01_ast.ipynb 27
 def last_statement_has_semicolon(code):
-    t = [x.strip() for x in code.splitlines()]
-    t = [x for x in t if not x.startswith('#')]
-    return t[-1].endswith(';')
+    e = end_of_last_line_of_code(code, last_node(code))
+    e = e.strip()
+    return e.startswith(';')
 
-# %% ../nbs/01_ast.ipynb 31
+# %% ../nbs/01_ast.ipynb 30
 def code_till_node(code:str,node):
+    if node is None: return code
     t = code.splitlines()
     t = t[:node.lineno]
     t[-1] = t[-1][:node.col_offset]
     if len(t[-1])==0: t = t[:-1]
     return '\n'.join(t)
 
-# %% ../nbs/01_ast.ipynb 34
-def auto_display(code):
+# %% ../nbs/01_ast.ipynb 33
+def auto_return(code):
     if last_statement_has_semicolon(code): return code
     
     n = last_node(code)
-    if not need_display(n): return code
+    if not need_return(n): return code
     
     ns = node_source(n,code)
     ret = code_till_node(code, last_node(code))
-    ret += f'\ndisplay( # %%testcell\n{ns}\n) # %%testcell'
+    ret += f'\nreturn {ns} # %%testcell'
     return ret
```

### Comparing `testcell-0.0.5/testcell.egg-info/PKG-INFO` & `testcell-0.0.6/testcell.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcell
-Version: 0.0.5
+Version: 0.0.6
 Summary: testcell prevents your testing cells from affecting the global namespace
 Home-page: https://github.com/artste/testcell
 Author: Stefano Giomo
 Author-email: artste@users.noreply.github.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
@@ -24,26 +24,38 @@
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 **TL;DR**: `%%testcell` prevents your testing cells from affecting the
 global namespace.
 
 The Python cell magic `%%testcell` executes a cell without *polluting*
-the notebook’s global variables. This is useful whenever you want to
+the notebook’s global namespace. This is useful whenever you want to
 test your code without having any of the local variables escape that
 cell.
 
 What’s happening under the hood is that your cell code, before being
 executed, is wrapped in a temporary function that will be deleted after
-execution. To give you the feeling of “seamless integration” the last
-line is optionally wrapped with a `display` statement if needed.
+execution. To give you the feeling of *seamless integration* the last
+statement is optionally returned like it happens in a normal cell.
 
 **WARNING:** this don’t protect you from *the side effects of your code*
 like deleting a file or mutating the state of a global variable.
 
+<div>
+
+[![](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/artste/testcell/blob/main/demo/testcell_demo.ipynb)
+
+</div>
+
+<div>
+
+[![](https://kaggle.com/static/images/open-in-kaggle.svg)](https://www.kaggle.com/artste/introducing-testcell)
+
+</div>
+
 ## Install
 
 ``` sh
 pip install testcell
 ```
 
 ## How to use
@@ -63,32 +75,34 @@
 assert 'a' not in locals()
 ```
 
 What is happening under the hood is that `%%testcell` wraps your cell’s
 code with a function, execute it and then deletes it. Adding the
 `verbose` keywork will print which code will be executed.
 
+NOTE: The actual cell code is enclosed within `BEGIN` and `END` comment
+blocks for improved readability.
+
 ``` python
 %%testcell verbose
 a = "'a' is not polluting global scope"
 a
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
-        display( # %%testcell
-        a
-        ) # %%testcell
+        return a # %%testcell
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    _ # This will be added to global scope
     ### END
 
     "'a' is not polluting global scope"
 
 If you’re just interested in seeing what will be executed, but actually
 not executing it, you ca use `dryrun` option:
 
@@ -99,84 +113,100 @@
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
-        display( # %%testcell
-        a
-        ) # %%testcell
+        return a # %%testcell
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    if _ is not None: display(_)
     ### END
 
-On top of *wrapping* your cell’s code, it will optinally add a
-`display(...)` call on your last cell’s row, trying to emulate what a
-real cell usually does. If you explicitly add a semicolon `;` in the
-end, this output will be suppressed.
+If you add a semicolon `;` at the end of your last statement no `return`
+statement is added and nothing is displayed like a normal jupyter cell.
 
 ``` python
 %%testcell verbose
 a = "'a' is not polluting global scope"
 a;
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
         a;
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    _ # This will be added to global scope
     ### END
 
-There are more cases where `display(...)` is avoided: \* `display`: if
-this is already present on the last line. \* `print`: even in this case
-no print is preserved and no other display call is added. \*
-`# comment...#`: these are preserved
+`testcell` works seamlessly with existing `print` or `display`statements
+on last line:
 
 ``` python
 %%testcell verbose
 a = "'a' is not polluting global scope"
 print(a)
 ```
 
 
     ### BEGIN
     def _test_cell_():
         #| echo: false
         a = "'a' is not polluting global scope"
-        print(a)
+        return print(a) # %%testcell
     try:
-        _test_cell_()
+        _ = _test_cell_()
     finally:
         del _test_cell_
+    _ # This will be added to global scope
     ### END
     'a' is not polluting global scope
 
-### Run in isolation
+Moreover, thanks to `ast`, it properly deals with complex situations
+like comments on the last line and multi lines statements
 
-`%%testcelln` is a shourtcut for `%%testcell noglobals` and executes the
-cell in complete isolation from global scope. This is very useful when
-you want to be sure that global variables or namespace should be part of
-the cell.
+``` python
+%%testcell verbose
+a = "'a' is not polluting global scope"
+(a,
+ True)
+# this is a comment on last line
+```
 
-## Run in isolation
 
-`%%testcelln` is a shortcut for `%%testcell noglobals` and executes the
-cell in complete isolation from the global scope.
+    ### BEGIN
+    def _test_cell_():
+        #| echo: false
+        a = "'a' is not polluting global scope"
+        return (a,
+         True) # %%testcell
+    try:
+        _ = _test_cell_()
+    finally:
+        del _test_cell_
+    _ # This will be added to global scope
+    ### END
 
-This is very useful when you want to ensure that global variables or
-namespaces are not accessible within the cell.
+    ("'a' is not polluting global scope", True)
+
+### Run in isolation
+
+`%%testcelln` is a shortcut for `%%testcell noglobals` and executes the
+cell in complete isolation from the global scope. This is very useful
+when you want to ensure that global variables or namespaces are not
+accessible within the cell.
 
 ``` python
 aaa = 'global variable'
 ```
 
 ``` python
 %%testcell
@@ -200,20 +230,19 @@
     False
 
 ``` python
 %%testcelln
 globals().keys()
 ```
 
-    dict_keys(['__builtins__', '_test_cell_'])
+    dict_keys(['__builtins__'])
 
-Inside the cell, from the *global scope*, only these two items are
-available: + `__builtins__` : built in python’s functions. +
-`_test_cell_` : `%%testcell` wrapped function executed (we can’t avoid
-this).
+With `%%testcelln` inside the cell, you’ll be able to access only to
+`__builtins__` (aka: standard python’s functions). **It behaves like a
+notebook-in-notebook**.
 
 ``` python
 %%testcell
 def my_function(x):
     print(aaa) # global variable
     return x
 
@@ -265,12 +294,20 @@
 
     'modified global variable'
 
 ``` python
 del aaa
 ```
 
-## TODO:
+## Links:
+
+- PROJECT PAGE: <https://github.com/artste/testcell>
+- DOCUMENTATION: <https://artste.github.io/testcell>
+- PYPI: <https://pypi.org/project/testcell>
+- COLAB DEMO:
+  [testcell_demo.ipynb](https://colab.research.google.com/github/artste/testcell/blob/main/demo/testcell_demo.ipynb)
+- KAGGLE SAMPLE NOTEBOOK:
+  <https://www.kaggle.com/artste/introducing-testcell>
+
+## Todo:
 
 - Install as a plugin to enable it by default like other cell’s magic.
-- Eval possibility to run code on a new kernel to reduce even more
-  possible side effects.
```


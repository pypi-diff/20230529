# Comparing `tmp/Fenv-0.0.8.tar.gz` & `tmp/Fenv-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Fenv-0.0.8.tar", last modified: Fri Feb  3 18:16:40 2023, max compression
+gzip compressed data, was "Fenv-0.0.9.tar", last modified: Fri Feb  3 18:23:55 2023, max compression
```

## Comparing `Fenv-0.0.8.tar` & `Fenv-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-02-03 18:16:40.184782 Fenv-0.0.8/
-drwxrwxrwx   0        0        0        0 2023-02-03 18:16:40.182270 Fenv-0.0.8/Fenv.egg-info/
--rw-rw-rw-   0        0        0     2395 2023-02-03 18:16:40.000000 Fenv-0.0.8/Fenv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2023-02-03 18:16:40.000000 Fenv-0.0.8/Fenv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-03 18:16:40.000000 Fenv-0.0.8/Fenv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       40 2023-02-03 18:16:40.000000 Fenv-0.0.8/Fenv.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       11 2023-02-03 18:16:40.000000 Fenv-0.0.8/Fenv.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-02-03 18:16:40.000000 Fenv-0.0.8/Fenv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2395 2023-02-03 18:16:40.184782 Fenv-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-03 18:16:40.183272 Fenv-0.0.8/fenv/
--rw-rw-rw-   0        0        0        0 2023-02-03 18:10:06.000000 Fenv-0.0.8/fenv/__init__.py
--rw-rw-rw-   0        0        0     6898 2023-02-03 18:14:16.000000 Fenv-0.0.8/fenv/fenv.py
--rw-rw-rw-   0        0        0       42 2023-02-03 18:16:40.184782 Fenv-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1345 2023-02-03 18:09:48.000000 Fenv-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-03 18:23:55.168639 Fenv-0.0.9/
+drwxrwxrwx   0        0        0        0 2023-02-03 18:23:55.164590 Fenv-0.0.9/Fenv.egg-info/
+-rw-rw-rw-   0        0        0     2518 2023-02-03 18:23:55.000000 Fenv-0.0.9/Fenv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      208 2023-02-03 18:23:55.000000 Fenv-0.0.9/Fenv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-03 18:23:55.000000 Fenv-0.0.9/Fenv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2023-02-03 18:23:55.000000 Fenv-0.0.9/Fenv.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       11 2023-02-03 18:23:55.000000 Fenv-0.0.9/Fenv.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-02-03 18:23:55.000000 Fenv-0.0.9/Fenv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2518 2023-02-03 18:23:55.168639 Fenv-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-02-03 18:23:55.167133 Fenv-0.0.9/fenv/
+-rw-rw-rw-   0        0        0        0 2023-02-03 18:10:06.000000 Fenv-0.0.9/fenv/__init__.py
+-rw-rw-rw-   0        0        0     6913 2023-02-03 18:20:59.000000 Fenv-0.0.9/fenv/fenv.py
+-rw-rw-rw-   0        0        0       42 2023-02-03 18:23:55.168639 Fenv-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1345 2023-02-03 18:23:51.000000 Fenv-0.0.9/setup.py
```

### Comparing `Fenv-0.0.8/Fenv.egg-info/PKG-INFO` & `Fenv-0.0.9/Fenv.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fenv
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate a folder, establish a virtual environment with a single command.
 Author: wk18k (watchakorn-18k)
 Author-email: <porton555@gmail.com>
 Keywords: python,virtualenv,create file,create folder,fenv,wk-18k
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -58,10 +58,22 @@
 for linux
 
 ```
 cd project_folder
 source env/bin/activate
 ```
 
+## Build
+
+```
+python setup.py sdist bdist_wheel
+```
+
+## Testing
+
+```
+pip install --editable .
+```
+
 ## Conclusion
 
 Fenv is a powerful tool for managing virtual environments and creating basic Python files. With its simple and efficient design, it's the perfect solution for developers who want to streamline their workflow and focus on coding. Get started today and see the difference Fenv can make in your Python development process!
```

### Comparing `Fenv-0.0.8/PKG-INFO` & `Fenv-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Fenv
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generate a folder, establish a virtual environment with a single command.
 Author: wk18k (watchakorn-18k)
 Author-email: <porton555@gmail.com>
 Keywords: python,virtualenv,create file,create folder,fenv,wk-18k
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -58,10 +58,22 @@
 for linux
 
 ```
 cd project_folder
 source env/bin/activate
 ```
 
+## Build
+
+```
+python setup.py sdist bdist_wheel
+```
+
+## Testing
+
+```
+pip install --editable .
+```
+
 ## Conclusion
 
 Fenv is a powerful tool for managing virtual environments and creating basic Python files. With its simple and efficient design, it's the perfect solution for developers who want to streamline their workflow and focus on coding. Get started today and see the difference Fenv can make in your Python development process!
```

### Comparing `Fenv-0.0.8/fenv/fenv.py` & `Fenv-0.0.9/fenv/fenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -209,15 +209,15 @@
 
 def main():
     """
     It creates a folder, creates a virtual environment, creates a settings file for vscode, creates a
     base file, and runs the install module base
     """
     parser = ArgumentParser()
-    parser.add_argument('-new', help="folder name", type=str)
+    parser.add_argument('-new', help="folder name", type=str, required=True)
     args: Namespace = parser.parse_args()
     if create_folder(args.new) != 1:
         create_virtualenv(args.new)
         create_setting_vscode(args.new)
         create_file_base(args.new)
         run_install_module_base(args.new)
```

### Comparing `Fenv-0.0.8/setup.py` & `Fenv-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Generate a folder, establish a virtual environment with a single command.'
 LONG_DESCRIPTION = 'Generate a folder, establish a virtual environment, and simultaneously create the essential basic Python files, all with a single command'
 
 # Setting up
 setup(
     name="Fenv",
     version=VERSION,
```


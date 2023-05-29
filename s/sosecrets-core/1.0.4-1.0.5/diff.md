# Comparing `tmp/sosecrets_core-1.0.4.tar.gz` & `tmp/sosecrets_core-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sosecrets_core-1.0.4.tar", last modified: Mon May 29 09:18:17 2023, max compression
+gzip compressed data, was "sosecrets_core-1.0.5.tar", last modified: Mon May 29 16:57:28 2023, max compression
```

## Comparing `sosecrets_core-1.0.4.tar` & `sosecrets_core-1.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 09:18:17.288836 sosecrets_core-1.0.4/
--rw-rw-rw-   0        0        0     1061 2023-05-29 07:32:28.000000 sosecrets_core-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     3806 2023-05-29 09:18:17.286835 sosecrets_core-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2986 2023-05-29 09:18:11.000000 sosecrets_core-1.0.4/README.md
--rw-rw-rw-   0        0        0      312 2023-05-29 09:18:11.000000 sosecrets_core-1.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 09:18:17.289839 sosecrets_core-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2260 2023-05-29 09:18:11.000000 sosecrets_core-1.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 09:18:17.268838 sosecrets_core-1.0.4/sosecrets_core/
--rw-rw-rw-   0        0        0   244666 2023-05-29 09:08:20.000000 sosecrets_core-1.0.4/sosecrets_core/secrets.c
-drwxrwxrwx   0        0        0        0 2023-05-29 09:18:17.283867 sosecrets_core-1.0.4/sosecrets_core.egg-info/
--rw-rw-rw-   0        0        0     3806 2023-05-29 09:18:17.000000 sosecrets_core-1.0.4/sosecrets_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      218 2023-05-29 09:18:17.000000 sosecrets_core-1.0.4/sosecrets_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 09:18:17.000000 sosecrets_core-1.0.4/sosecrets_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-05-29 09:18:17.000000 sosecrets_core-1.0.4/sosecrets_core.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 16:57:28.945361 sosecrets_core-1.0.5/
+-rw-rw-rw-   0        0        0     1061 2023-05-29 07:32:28.000000 sosecrets_core-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     3950 2023-05-29 16:57:28.943364 sosecrets_core-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3089 2023-05-29 16:56:30.000000 sosecrets_core-1.0.5/README.md
+-rw-rw-rw-   0        0        0     1209 2023-05-29 16:56:30.000000 sosecrets_core-1.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-29 16:57:28.945361 sosecrets_core-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2312 2023-05-29 16:56:30.000000 sosecrets_core-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:57:28.924379 sosecrets_core-1.0.5/sosecrets_core/
+-rw-rw-rw-   0        0        0   244666 2023-05-29 16:57:24.000000 sosecrets_core-1.0.5/sosecrets_core/secrets.c
+drwxrwxrwx   0        0        0        0 2023-05-29 16:57:28.940370 sosecrets_core-1.0.5/sosecrets_core.egg-info/
+-rw-rw-rw-   0        0        0     3950 2023-05-29 16:57:28.000000 sosecrets_core-1.0.5/sosecrets_core.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      218 2023-05-29 16:57:28.000000 sosecrets_core-1.0.5/sosecrets_core.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 16:57:28.000000 sosecrets_core-1.0.5/sosecrets_core.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-05-29 16:57:28.000000 sosecrets_core-1.0.5/sosecrets_core.egg-info/top_level.txt
```

### Comparing `sosecrets_core-1.0.4/LICENSE` & `sosecrets_core-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sosecrets_core-1.0.4/PKG-INFO` & `sosecrets_core-1.0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosecrets_core
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simple Secret Primitive for Python
 Home-page: http://github.com/jymchng/sosecrets-core
 Author: Jim Chng
 Author-email: jimchng@outlook.com
 License: MIT
 Keywords: secrets security secrets-management
 Classifier: Programming Language :: Python
@@ -13,30 +13,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Cython
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sosecrets-core
 
-![https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml](https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml) ![https://img.shields.io/pypi/pyversions/sosecrets-core](https://img.shields.io/pypi/pyversions/sosecrets-core)
+![https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml](https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml) ![https://img.shields.io/pypi/pyversions/sosecrets-core](https://img.shields.io/pypi/pyversions/sosecrets-core) ![https://img.shields.io/pypi/dm/sosecrets-core](https://img.shields.io/pypi/dm/sosecrets-core)
 
-Version: 1.0.4
+Version: 1.0.5
 
-This Repo is a Cython implementation of a `Secret` class that allows you to hide a value or function behind a layer of security. The idea is that you can expose the secret value or function only a limited number of times, and only through a function call that checks the current exposure count against a maximum exposure count.
+This Repo is a Cython implementation of a `Secret` class that allows you to hide a value or function behind a layer of security.
+
+The idea is that you can expose the secret value only a limited number of times, and only through a function call that checks the current exposure count against a maximum exposure count.
 
 The `Secret` class has four attributes:
 
-`inner_secret`: a private attribute that stores the actual secret value or function.
-`expose_count`: a readonly attribute that keeps track of how many times the secret has been exposed.
-`max_expose_count`: a public (read and write) attribute that sets the maximum number of times the secret can be exposed. If set to any negative integers, there is no limit to the number of exposures.
-`apply`: a public method that applies a given function to the exposed secret and returns a new `Secret` object with the result.
+* `inner_secret`: a private attribute that stores the actual secret value or function.
+* `expose_count`: a readonly attribute that keeps track of how many times the secret has been exposed.
+* `max_expose_count`: a public (read and write) attribute that sets the maximum number of times the secret can be exposed. If set to any negative integers, there is no limit to the number of exposures.
+* `apply`: a public method that applies a given function to the exposed secret and returns a new `Secret` object with the result.
 
 ## API
 
 ### Secret
 
 A class representing a secret value with controlled exposure.
 
@@ -47,15 +50,15 @@
 Notes:
 1. `Secret` is not thread-safe, because `expose_count` is not atomically-mutated.
 
 * value: The initial value of the `Secret` object. If provided, it takes precedence over `func`.
 * func: A function used to generate the initial value of the `Secret` object. Ignored if value is provided.
 * func_args: Positional arguments to pass to the `func` function.
 * func_kwargs: Keyword arguments to pass to the `func` function.
-* max_expose_count: The maximum number of times the `Secret` object can be exposed. Set to -1 for unlimited.
+* max_expose_count: The maximum number of times the `Secret` object can be exposed. Initialized to -1 for unlimited.
 
 Raises:
 
 * ValueError: If both `value` and `func` arguments are provided.
 
 ### `Secret.expose_secret()`
```

### Comparing `sosecrets_core-1.0.4/README.md` & `sosecrets_core-1.0.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 # sosecrets-core
 
-![https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml](https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml) ![https://img.shields.io/pypi/pyversions/sosecrets-core](https://img.shields.io/pypi/pyversions/sosecrets-core)
+![https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml](https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml) ![https://img.shields.io/pypi/pyversions/sosecrets-core](https://img.shields.io/pypi/pyversions/sosecrets-core) ![https://img.shields.io/pypi/dm/sosecrets-core](https://img.shields.io/pypi/dm/sosecrets-core)
 
-Version: 1.0.4
+Version: 1.0.5
 
-This Repo is a Cython implementation of a `Secret` class that allows you to hide a value or function behind a layer of security. The idea is that you can expose the secret value or function only a limited number of times, and only through a function call that checks the current exposure count against a maximum exposure count.
+This Repo is a Cython implementation of a `Secret` class that allows you to hide a value or function behind a layer of security.
+
+The idea is that you can expose the secret value only a limited number of times, and only through a function call that checks the current exposure count against a maximum exposure count.
 
 The `Secret` class has four attributes:
 
-`inner_secret`: a private attribute that stores the actual secret value or function.
-`expose_count`: a readonly attribute that keeps track of how many times the secret has been exposed.
-`max_expose_count`: a public (read and write) attribute that sets the maximum number of times the secret can be exposed. If set to any negative integers, there is no limit to the number of exposures.
-`apply`: a public method that applies a given function to the exposed secret and returns a new `Secret` object with the result.
+* `inner_secret`: a private attribute that stores the actual secret value or function.
+* `expose_count`: a readonly attribute that keeps track of how many times the secret has been exposed.
+* `max_expose_count`: a public (read and write) attribute that sets the maximum number of times the secret can be exposed. If set to any negative integers, there is no limit to the number of exposures.
+* `apply`: a public method that applies a given function to the exposed secret and returns a new `Secret` object with the result.
 
 ## API
 
 ### Secret
 
 A class representing a secret value with controlled exposure.
 
@@ -26,15 +28,15 @@
 Notes:
 1. `Secret` is not thread-safe, because `expose_count` is not atomically-mutated.
 
 * value: The initial value of the `Secret` object. If provided, it takes precedence over `func`.
 * func: A function used to generate the initial value of the `Secret` object. Ignored if value is provided.
 * func_args: Positional arguments to pass to the `func` function.
 * func_kwargs: Keyword arguments to pass to the `func` function.
-* max_expose_count: The maximum number of times the `Secret` object can be exposed. Set to -1 for unlimited.
+* max_expose_count: The maximum number of times the `Secret` object can be exposed. Initialized to -1 for unlimited.
 
 Raises:
 
 * ValueError: If both `value` and `func` arguments are provided.
 
 ### `Secret.expose_secret()`
```

### Comparing `sosecrets_core-1.0.4/setup.py` & `sosecrets_core-1.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,27 +38,28 @@
 else:
     ext_modules += [
         Extension("sosecrets_core.secrets", ["sosecrets_core/secrets.c"]),
     ]
 
 setup(
     name='sosecrets_core',
-    version="1.0.4",
+    version="1.0.5",
     description='Simple Secret Primitive for Python',
     author='Jim Chng',
     author_email='jimchng@outlook.com',
     url='http://github.com/jymchng/sosecrets-core',
     packages=['sosecrets_core'],
     package_dir={
         'sosecrets_core': 'sosecrets_core',
     },
     cmdclass=cmdclass,
     ext_modules=ext_modules,
 
     long_description=open('README.md').read(),
+    long_description_content_type='text/markdown',
 
     license="MIT",
     classifiers = [
         "Programming Language :: Python",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
```

### Comparing `sosecrets_core-1.0.4/sosecrets_core/secrets.c` & `sosecrets_core-1.0.5/sosecrets_core/secrets.c`

 * *Files identical despite different names*

### Comparing `sosecrets_core-1.0.4/sosecrets_core.egg-info/PKG-INFO` & `sosecrets_core-1.0.5/sosecrets_core.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sosecrets-core
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simple Secret Primitive for Python
 Home-page: http://github.com/jymchng/sosecrets-core
 Author: Jim Chng
 Author-email: jimchng@outlook.com
 License: MIT
 Keywords: secrets security secrets-management
 Classifier: Programming Language :: Python
@@ -13,30 +13,33 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Cython
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # sosecrets-core
 
-![https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml](https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml) ![https://img.shields.io/pypi/pyversions/sosecrets-core](https://img.shields.io/pypi/pyversions/sosecrets-core)
+![https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml](https://img.shields.io/github/actions/workflow/status/jymchng/sosecrets-core/testing.yml) ![https://img.shields.io/pypi/pyversions/sosecrets-core](https://img.shields.io/pypi/pyversions/sosecrets-core) ![https://img.shields.io/pypi/dm/sosecrets-core](https://img.shields.io/pypi/dm/sosecrets-core)
 
-Version: 1.0.4
+Version: 1.0.5
 
-This Repo is a Cython implementation of a `Secret` class that allows you to hide a value or function behind a layer of security. The idea is that you can expose the secret value or function only a limited number of times, and only through a function call that checks the current exposure count against a maximum exposure count.
+This Repo is a Cython implementation of a `Secret` class that allows you to hide a value or function behind a layer of security.
+
+The idea is that you can expose the secret value only a limited number of times, and only through a function call that checks the current exposure count against a maximum exposure count.
 
 The `Secret` class has four attributes:
 
-`inner_secret`: a private attribute that stores the actual secret value or function.
-`expose_count`: a readonly attribute that keeps track of how many times the secret has been exposed.
-`max_expose_count`: a public (read and write) attribute that sets the maximum number of times the secret can be exposed. If set to any negative integers, there is no limit to the number of exposures.
-`apply`: a public method that applies a given function to the exposed secret and returns a new `Secret` object with the result.
+* `inner_secret`: a private attribute that stores the actual secret value or function.
+* `expose_count`: a readonly attribute that keeps track of how many times the secret has been exposed.
+* `max_expose_count`: a public (read and write) attribute that sets the maximum number of times the secret can be exposed. If set to any negative integers, there is no limit to the number of exposures.
+* `apply`: a public method that applies a given function to the exposed secret and returns a new `Secret` object with the result.
 
 ## API
 
 ### Secret
 
 A class representing a secret value with controlled exposure.
 
@@ -47,15 +50,15 @@
 Notes:
 1. `Secret` is not thread-safe, because `expose_count` is not atomically-mutated.
 
 * value: The initial value of the `Secret` object. If provided, it takes precedence over `func`.
 * func: A function used to generate the initial value of the `Secret` object. Ignored if value is provided.
 * func_args: Positional arguments to pass to the `func` function.
 * func_kwargs: Keyword arguments to pass to the `func` function.
-* max_expose_count: The maximum number of times the `Secret` object can be exposed. Set to -1 for unlimited.
+* max_expose_count: The maximum number of times the `Secret` object can be exposed. Initialized to -1 for unlimited.
 
 Raises:
 
 * ValueError: If both `value` and `func` arguments are provided.
 
 ### `Secret.expose_secret()`
```


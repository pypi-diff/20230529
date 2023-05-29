# Comparing `tmp/pers-0.1.3.tar.gz` & `tmp/pers-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pers-0.1.3.tar", last modified: Sun May 28 10:08:49 2023, max compression
+gzip compressed data, was "pers-0.1.4.tar", last modified: Mon May 29 18:46:08 2023, max compression
```

## Comparing `pers-0.1.3.tar` & `pers-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-28 10:08:49.774864 pers-0.1.3/
--rw-r--r--   0 ok        (1000) ok        (1000)    35149 2023-05-02 13:14:10.000000 pers-0.1.3/LICENSE
--rw-r--r--   0 ok        (1000) ok        (1000)     3495 2023-05-28 10:08:49.774864 pers-0.1.3/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)     2983 2023-05-15 19:47:59.000000 pers-0.1.3/README.md
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-28 10:08:49.773864 pers-0.1.3/pers/
--rw-r--r--   0 ok        (1000) ok        (1000)       19 2023-05-02 13:13:28.000000 pers-0.1.3/pers/__init__.py
--rw-r--r--   0 ok        (1000) ok        (1000)     5758 2023-05-28 10:04:18.000000 pers-0.1.3/pers/pers.py
--rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-05-28 08:15:19.000000 pers-0.1.3/pers/version.py
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-28 10:08:49.774864 pers-0.1.3/pers.egg-info/
--rw-r--r--   0 ok        (1000) ok        (1000)     3495 2023-05-28 10:08:49.000000 pers-0.1.3/pers.egg-info/PKG-INFO
--rw-r--r--   0 ok        (1000) ok        (1000)      232 2023-05-28 10:08:49.000000 pers-0.1.3/pers.egg-info/SOURCES.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-05-28 10:08:49.000000 pers-0.1.3/pers.egg-info/dependency_links.txt
--rw-r--r--   0 ok        (1000) ok        (1000)       12 2023-05-28 10:08:49.000000 pers-0.1.3/pers.egg-info/requires.txt
--rw-r--r--   0 ok        (1000) ok        (1000)        5 2023-05-28 10:08:49.000000 pers-0.1.3/pers.egg-info/top_level.txt
--rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-05-28 10:08:49.774864 pers-0.1.3/setup.cfg
--rw-r--r--   0 ok        (1000) ok        (1000)     1133 2023-05-15 19:49:22.000000 pers-0.1.3/setup.py
-drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-28 10:08:49.774864 pers-0.1.3/tests/
--rw-r--r--   0 ok        (1000) ok        (1000)     3254 2023-05-28 09:19:46.000000 pers-0.1.3/tests/tests.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-29 18:46:08.967730 pers-0.1.4/
+-rw-r--r--   0 ok        (1000) ok        (1000)    35149 2023-05-02 13:14:10.000000 pers-0.1.4/LICENSE
+-rw-r--r--   0 ok        (1000) ok        (1000)     3456 2023-05-29 18:46:08.967730 pers-0.1.4/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)     2944 2023-05-28 20:32:01.000000 pers-0.1.4/README.md
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-29 18:46:08.965730 pers-0.1.4/pers/
+-rw-r--r--   0 ok        (1000) ok        (1000)       19 2023-05-02 13:13:28.000000 pers-0.1.4/pers/__init__.py
+-rw-r--r--   0 ok        (1000) ok        (1000)     5665 2023-05-29 18:45:21.000000 pers-0.1.4/pers/pers.py
+-rw-r--r--   0 ok        (1000) ok        (1000)       21 2023-05-29 18:45:23.000000 pers-0.1.4/pers/version.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-29 18:46:08.966730 pers-0.1.4/pers.egg-info/
+-rw-r--r--   0 ok        (1000) ok        (1000)     3456 2023-05-29 18:46:08.000000 pers-0.1.4/pers.egg-info/PKG-INFO
+-rw-r--r--   0 ok        (1000) ok        (1000)      232 2023-05-29 18:46:08.000000 pers-0.1.4/pers.egg-info/SOURCES.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        1 2023-05-29 18:46:08.000000 pers-0.1.4/pers.egg-info/dependency_links.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       12 2023-05-29 18:46:08.000000 pers-0.1.4/pers.egg-info/requires.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)        5 2023-05-29 18:46:08.000000 pers-0.1.4/pers.egg-info/top_level.txt
+-rw-r--r--   0 ok        (1000) ok        (1000)       38 2023-05-29 18:46:08.967730 pers-0.1.4/setup.cfg
+-rw-r--r--   0 ok        (1000) ok        (1000)     1133 2023-05-15 19:49:22.000000 pers-0.1.4/setup.py
+drwxr-xr-x   0 ok        (1000) ok        (1000)        0 2023-05-29 18:46:08.967730 pers-0.1.4/tests/
+-rw-r--r--   0 ok        (1000) ok        (1000)     3254 2023-05-28 09:19:46.000000 pers-0.1.4/tests/tests.py
```

### Comparing `pers-0.1.3/LICENSE` & `pers-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pers-0.1.3/PKG-INFO` & `pers-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pers
-Version: 0.1.3
+Version: 0.1.4
 Summary: Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
 Home-page: https://github.com/rsusik/pers
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,16 @@
     <img src="https://img.shields.io/pypi/v/pers?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://github.com/rsusik/pers/blob/master/LICENSE" target="_blank">
     <img src="https://img.shields.io/github/license/rsusik/pers" alt="Package version">
 </a>
 </p>
 
-Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
+Persistent results is a Python class that ensures the results will be available even if interruptions occur.
+
 
 ## Installation:
 
 ```
 pip install pers
 ```
 
@@ -36,30 +37,28 @@
 
 ### Example 1
 
 If the code below breaks for some reason (let's say the computer shuts down because of a power outage or some exception), you can restart it to continue from the step it finished.
 
 ```python
 from pers import PersistentResults
-import pandas as pd
+import pandas as pd # pandas is not required
 
 results = PersistentResults(
     'test.pickle', # filename for result caching
     interval=1,    # how often dump the results
     tmpfilename='~test.pickle' # tmp cache file (optional)
 )
 
 fun = lambda x, y, a, b: x**2 + y
 for x in range(10):
     for y in range(11):
         results.append(fun, x, y, a=x, b=y)
 results.save()
 
-print(results[90])
-print(len(results))
 print(pd.DataFrame(results.data))
 ```
 
 Output:
 
 ```
 {'result': 66, 'x': 8, 'y': 2, 'a': 8, 'b': 2}
```

### Comparing `pers-0.1.3/README.md` & `pers-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,16 @@
     <img src="https://img.shields.io/pypi/v/pers?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://github.com/rsusik/pers/blob/master/LICENSE" target="_blank">
     <img src="https://img.shields.io/github/license/rsusik/pers" alt="Package version">
 </a>
 </p>
 
-Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
+Persistent results is a Python class that ensures the results will be available even if interruptions occur.
+
 
 ## Installation:
 
 ```
 pip install pers
 ```
 
@@ -21,30 +22,28 @@
 
 ### Example 1
 
 If the code below breaks for some reason (let's say the computer shuts down because of a power outage or some exception), you can restart it to continue from the step it finished.
 
 ```python
 from pers import PersistentResults
-import pandas as pd
+import pandas as pd # pandas is not required
 
 results = PersistentResults(
     'test.pickle', # filename for result caching
     interval=1,    # how often dump the results
     tmpfilename='~test.pickle' # tmp cache file (optional)
 )
 
 fun = lambda x, y, a, b: x**2 + y
 for x in range(10):
     for y in range(11):
         results.append(fun, x, y, a=x, b=y)
 results.save()
 
-print(results[90])
-print(len(results))
 print(pd.DataFrame(results.data))
 ```
 
 Output:
 
 ```
 {'result': 66, 'x': 8, 'y': 2, 'a': 8, 'b': 2}
```

### Comparing `pers-0.1.3/pers/pers.py` & `pers-0.1.4/pers/pers.py`

 * *Files 7% similar despite different names*

```diff
@@ -47,15 +47,15 @@
             return {f'{self.result_prefix}{idx}':x for idx, x in enumerate(res)}
         else:
             return {self.result_key: res}
 
 
     def _get_args_kwargs_hash(self, el, args, kwargs):
         _args = el[:len(args)]
-        _kwargs = dict(zip(kwargs.keys(), el[len(kwargs.keys()):]))
+        _kwargs = dict(zip(kwargs.keys(), el[len(args):]))
         _hash = self.results.get_hash([_args, _kwargs])
         return _args, _kwargs, _hash
 
 
     def all(self, *args:List, **kwargs:List)->bool:
         '''
         Returns True if results contain all records for
@@ -63,15 +63,14 @@
         '''
         l = product(*args, *kwargs.values())
         for el in l:
             _, _, _hash = self._get_args_kwargs_hash(el, args, kwargs)
             try:
                 _ = self.results.get_value(_hash)
             except Cache.NoCacheValue:
-                print('WRONG', el)
                 return False
         return True
 
 
     def any(self, *args:List, **kwargs:List)->bool:
         '''
         Returns True if any results contain any records 
@@ -88,15 +87,14 @@
         return False
 
 
     def missing(self, *args:List, **kwargs:List)->List[Tuple[list, dict]]:
         '''
         Returns all missing records for product of given arguments
         '''
-        print(*args, 'kwargs', *kwargs.values())
         l = product(*args, *kwargs.values())
         missing = []
         for el in l:
             _args, _kwargs, _hash = self._get_args_kwargs_hash(el, args, kwargs)
             try:
                 _ = self.results.get_value(_hash)
             except Cache.NoCacheValue:
```

### Comparing `pers-0.1.3/pers.egg-info/PKG-INFO` & `pers-0.1.4/pers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pers
-Version: 0.1.3
+Version: 0.1.4
 Summary: Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
 Home-page: https://github.com/rsusik/pers
 Author: Robert Susik
 Author-email: robert.susik@gmail.com
 License: GPLv3
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,16 @@
     <img src="https://img.shields.io/pypi/v/pers?color=%2334D058&label=pypi%20package" alt="Package version">
 </a>
 <a href="https://github.com/rsusik/pers/blob/master/LICENSE" target="_blank">
     <img src="https://img.shields.io/github/license/rsusik/pers" alt="Package version">
 </a>
 </p>
 
-Persistent results is a Python class that ensures the results of tests will be available even if interruptions during the tests occur.
+Persistent results is a Python class that ensures the results will be available even if interruptions occur.
+
 
 ## Installation:
 
 ```
 pip install pers
 ```
 
@@ -36,30 +37,28 @@
 
 ### Example 1
 
 If the code below breaks for some reason (let's say the computer shuts down because of a power outage or some exception), you can restart it to continue from the step it finished.
 
 ```python
 from pers import PersistentResults
-import pandas as pd
+import pandas as pd # pandas is not required
 
 results = PersistentResults(
     'test.pickle', # filename for result caching
     interval=1,    # how often dump the results
     tmpfilename='~test.pickle' # tmp cache file (optional)
 )
 
 fun = lambda x, y, a, b: x**2 + y
 for x in range(10):
     for y in range(11):
         results.append(fun, x, y, a=x, b=y)
 results.save()
 
-print(results[90])
-print(len(results))
 print(pd.DataFrame(results.data))
 ```
 
 Output:
 
 ```
 {'result': 66, 'x': 8, 'y': 2, 'a': 8, 'b': 2}
```

### Comparing `pers-0.1.3/setup.py` & `pers-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `pers-0.1.3/tests/tests.py` & `pers-0.1.4/tests/tests.py`

 * *Files identical despite different names*


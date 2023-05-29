# Comparing `tmp/lib-dzne-auto-interface-0.2.0.tar.gz` & `tmp/lib-dzne-auto-interface-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-auto-interface-0.2.0.tar", last modified: Fri May 26 20:42:20 2023, max compression
+gzip compressed data, was "lib-dzne-auto-interface-0.2.1.tar", last modified: Mon May 29 13:00:01 2023, max compression
```

## Comparing `lib-dzne-auto-interface-0.2.0.tar` & `lib-dzne-auto-interface-0.2.1.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-26 20:42:20.125642 lib-dzne-auto-interface-0.2.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.2.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1538 2023-05-26 20:42:20.125642 lib-dzne-auto-interface-0.2.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      547 2023-05-25 04:55:40.000000 lib-dzne-auto-interface-0.2.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-26 20:42:20.125642 lib-dzne-auto-interface-0.2.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-26 20:42:20.121648 lib-dzne-auto-interface-0.2.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-26 20:42:20.125642 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface/
--rw-r--r--   0 base      (1001) base      (1001)     8390 2023-05-26 20:40:19.000000 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-26 20:42:20.125642 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1538 2023-05-26 20:42:20.000000 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      276 2023-05-26 20:42:20.000000 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-26 20:42:20.000000 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       24 2023-05-26 20:42:20.000000 lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:00:01.603648 lib-dzne-auto-interface-0.2.1/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.2.1/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-05-29 13:00:01.603648 lib-dzne-auto-interface-0.2.1/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       26 2023-05-29 09:37:30.000000 lib-dzne-auto-interface-0.2.1/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      547 2023-05-29 12:59:01.000000 lib-dzne-auto-interface-0.2.1/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 13:00:01.603648 lib-dzne-auto-interface-0.2.1/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:00:01.599648 lib-dzne-auto-interface-0.2.1/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:00:01.603648 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface/
+-rw-r--r--   0 base      (1001) base      (1001)     8456 2023-05-29 12:59:34.000000 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:00:01.603648 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-05-29 13:00:01.000000 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      286 2023-05-29 13:00:01.000000 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 13:00:01.000000 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       24 2023-05-29 13:00:01.000000 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/top_level.txt
```

### Comparing `lib-dzne-auto-interface-0.2.0/LICENSE` & `lib-dzne-auto-interface-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-auto-interface-0.2.0/PKG-INFO` & `lib-dzne-auto-interface-0.2.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.2.0
+Version: 0.2.1
 Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -13,7 +13,9 @@
         
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# lib-dzne-auto-interface
```

### Comparing `lib-dzne-auto-interface-0.2.0/pyproject.toml` & `lib-dzne-auto-interface-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-auto-interface"
-version = "0.2.0"
+version = "0.2.1"
 description = "Libary for automatically created interfaces. "
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface/__init__.py` & `lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,16 @@
     	return list(self._subknots)
 
 class _Argument(_Knot):
     def __init__(self, *args, **kwargs):
         info = Information()
         info.kwargs = dict(*args, **kwargs)
         info.args = info.pop('option_strings', [])
-        self._action_string = (info['action'] := info.get('action', 'store'))
+        info['action'] = info.get('action', 'store')
+        self._action_string = info['action']
         if self._action_string not in (
             'store', 
             #'store_const',
             'store_true', 
             'store_false', 
             #'append',
             #'append_const',
@@ -225,14 +226,15 @@
         		if a.ispositional:
         			info.append(value)
         		else:
         			info[a.dest] = value
         if len(kwargs):
         	raise KeyError()
         result = info.exec(self._value)
+        result = outfile.fileDataType(result)
         outfile.save(result)
     def _go(self):
     	kwargs = self._read_gui()
     	self._run(kwargs)
     @property
     def parameters(self):
     	return self.subknots[:-1]
```

### Comparing `lib-dzne-auto-interface-0.2.0/src/lib_dzne_auto_interface.egg-info/PKG-INFO` & `lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.2.0
+Version: 0.2.1
 Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
@@ -13,7 +13,9 @@
         
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
+
+# lib-dzne-auto-interface
```


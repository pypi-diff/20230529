# Comparing `tmp/lib-dzne-auto-interface-0.2.1.tar.gz` & `tmp/lib-dzne-auto-interface-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-auto-interface-0.2.1.tar", last modified: Mon May 29 13:00:01 2023, max compression
+gzip compressed data, was "lib-dzne-auto-interface-0.2.2.tar", last modified: Mon May 29 14:10:07 2023, max compression
```

## Comparing `lib-dzne-auto-interface-0.2.1.tar` & `lib-dzne-auto-interface-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:00:01.603648 lib-dzne-auto-interface-0.2.1/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.2.1/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-05-29 13:00:01.603648 lib-dzne-auto-interface-0.2.1/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       26 2023-05-29 09:37:30.000000 lib-dzne-auto-interface-0.2.1/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      547 2023-05-29 12:59:01.000000 lib-dzne-auto-interface-0.2.1/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 13:00:01.603648 lib-dzne-auto-interface-0.2.1/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:00:01.599648 lib-dzne-auto-interface-0.2.1/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:00:01.603648 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface/
--rw-r--r--   0 base      (1001) base      (1001)     8456 2023-05-29 12:59:34.000000 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 13:00:01.603648 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-05-29 13:00:01.000000 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      286 2023-05-29 13:00:01.000000 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 13:00:01.000000 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       24 2023-05-29 13:00:01.000000 lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-auto-interface-0.2.2/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       26 2023-05-29 09:37:30.000000 lib-dzne-auto-interface-0.2.2/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      547 2023-05-29 14:09:22.000000 lib-dzne-auto-interface-0.2.2/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface/
+-rw-r--r--   0 base      (1001) base      (1001)     8959 2023-05-29 14:07:49.000000 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 14:10:07.459888 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1565 2023-05-29 14:10:07.000000 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      286 2023-05-29 14:10:07.000000 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 14:10:07.000000 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       24 2023-05-29 14:10:07.000000 lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/top_level.txt
```

### Comparing `lib-dzne-auto-interface-0.2.1/LICENSE` & `lib-dzne-auto-interface-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-auto-interface-0.2.1/PKG-INFO` & `lib-dzne-auto-interface-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.2.1
+Version: 0.2.2
 Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-auto-interface-0.2.1/pyproject.toml` & `lib-dzne-auto-interface-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-auto-interface"
-version = "0.2.1"
+version = "0.2.2"
 description = "Libary for automatically created interfaces. "
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface/__init__.py` & `lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,67 +13,67 @@
     def args(self, value):
         self._args = list(value)
     @property
     def kwargs(self):
         return dict(self._kwargs)
     @kwargs.setter
     def kwargs(self, value):
-    	self._kwargs = dict(value)
-    	if not all(type(k) is str for k, v in self._kwargs.items()):
-    		raise TypeError()
+        self._kwargs = dict(value)
+        if not all(type(k) is str for k, v in self._kwargs.items()):
+            raise TypeError()
     def __add__(self, other):
         return Information(
             args = self.args + other.args,
             kwargs = dict(**self.kwargs, **other.kwargs),
         )
     def __getitem__(self, key):
-    	if type(key) in (int, slice):
-    		return self._args[key]
-    	if type(key) is str:
-    		return self._kwargs[key]
-    	raise TypeError()
+        if type(key) in (int, slice):
+            return self._args[key]
+        if type(key) is str:
+            return self._kwargs[key]
+        raise TypeError()
     def __setitem__(self, key, value):
-    	if type(key) in (int, slice):
-    		a = list(self.args)
-    		a[key] = value
-    		self.args = a
-    		return
-    	if type(key) is str:
-    		self._kwargs[key] = value
-    		return
-    	raise TypeError()
+        if type(key) in (int, slice):
+            a = list(self.args)
+            a[key] = value
+            self.args = a
+            return
+        if type(key) is str:
+            self._kwargs[key] = value
+            return
+        raise TypeError()
     def __delitem__(self, key):
-    	if type(key) in (int, slice):
-    		a = list(self.args)
-    		del a[key]
-    		self.args = a
-    		return
-    	if type(key) is str:
-    		del self._kwargs[key]
-    		return
-    	raise TypeError()
+        if type(key) in (int, slice):
+            a = list(self.args)
+            del a[key]
+            self.args = a
+            return
+        if type(key) is str:
+            del self._kwargs[key]
+            return
+        raise TypeError()
     def pop(self, key=-1, /, *args):
-    	if type(key) in (int, slice):
-    		return self._args.pop(key, *args)
-    	if type(key) is str:
-    		return self._kwargs.pop(key, *args)
-    	raise TypeError()
+        if type(key) in (int, slice):
+            return self._args.pop(key, *args)
+        if type(key) is str:
+            return self._kwargs.pop(key, *args)
+        raise TypeError()
     def get(self, key, default=None, /):
-    	if type(key) in (int, slice):
-    		try:
-    			return self._args[key]
-    		except IndexError:
-    			return default
-    	if type(key) is str:
-    		return self._kwargs.get(key, default)
-    	raise TypeError()
+        if type(key) in (int, slice):
+            try:
+                return self._args[key]
+            except IndexError:
+                return default
+        if type(key) is str:
+            return self._kwargs.get(key, default)
+        raise TypeError()
     def append(self, value):
-    	self._args.append(value)
+        self._args.append(value)
     def exec(self, func):
-    	return func(*self._args, **self._kwargs)
+        return func(*self._args, **self._kwargs)
 
 
 class _Knot(object):
     def _make_parser(self, *args, **kwargs):
         return _ap.ArgumentParser(
             *args,
             **kwargs,
@@ -85,15 +85,15 @@
             parents=[self._parser],
             description=self._parser.description,
         )
     def parse(self, args):
         return vars(self._parser.parse_args(args))
     @property
     def subknots(self):
-    	return list(self._subknots)
+        return list(self._subknots)
 
 class _Argument(_Knot):
     def __init__(self, *args, **kwargs):
         info = Information()
         info.kwargs = dict(*args, **kwargs)
         info.args = info.pop('option_strings', [])
         info['action'] = info.get('action', 'store')
@@ -103,16 +103,16 @@
             #'store_const',
             'store_true', 
             'store_false', 
             #'append',
             #'append_const',
         ):
             raise ValueError()
-        self._action = info.exec(self._parser.add_argument)
         self._parser = self._make_parser()
+        self._action = info.exec(self._parser.add_argument)
         self._subknots = list()
     @property
     def ispositional(self):
         return self.option_strings is None
     @property
     def option_strings(self):
         ans = self._action.option_strings
@@ -124,21 +124,21 @@
     def action(self):
         return self._action_string
     @property
     def dest(self):
         return self._action.dest
     @property
     def help(self):
-    	return self._action.help
+        return self._action.help
     @staticmethod
     def of_return(annotation, *, details={}):
+        if annotation is _ins.Parameter.empty:
+            return None
         if callable(annotation):
             annotation = {'type': annotation}
-        elif annotation is _ins.Parameter.empty:
-            annotation = {}
         elif type(annotation) is str:
             annotation = {'help': annotation}
         return _Argument(**annotation, **details)
 
 class _Parameter(_Knot):
     def __init__(self, value):
         self._subknots = self._get_subknots(value)
@@ -180,97 +180,101 @@
         else:
             raise ValueError()
         ans = _Argument(**ans, **ann)
         return [ans]
 
 
 class _Main(_Knot):
-	def run_cli(self, args):
-		kwargs = self.parse(args)
-		self._run(kwargs)
+    def run_cli(self, args):
+        kwargs = self.parser(add_help=True).parse_args(args)
+        self._run(kwargs)
     def run_gui(self):
-    	#implement!
-    	#launch root window
-    	raise NotImplementedError()
+        #implement!
+        #launch root window
+        raise NotImplementedError()
     def _run(self, kwargs):
         raise NotImplementedError()
     @property
     def description(self):
-    	return self._parser.description
+        return self._parser.description
 
 
 class _Callable(_Main):
     def __init__(self, value, return_details):
         self._value = value
         signature = _ins.signature(value)
-        self._subknots = [_Parameter(p) for n, p in signature.parameters.items()]
-        self._subknots += [
-        	_Argument.of_return(
-	            annotation=signature.return_annotation,
-	            details=return_details,
-	        )
-	    ]
-	    parents = [x.parser(add_help=False) for x in self.subknots]
+        self._parameters = [_Parameter(p) for n, p in signature.parameters.items()]
+        self._argument_of_return = _Argument.of_return(
+            annotation=signature.return_annotation,
+            details=return_details,
+        )
+        parents = [x.parser(add_help=False) for x in self.subknots]
         self._parser = self._make_parser(
             description=value.__doc__,
             parents=parents,
         )
     def _read_gui(self):
-    	raise NotImplementedError()
-    	#implement!
+        raise NotImplementedError()
+        #implement!
     def _run(self, kwargs):
         outfile = kwargs.pop(self.argument_of_return.dest)
         info = Information()
         for p in self.parameters:
-        	for a in p.subknots:
-        		value = kwargs.pop(a.dest)
-        		if a.ispositional:
-        			info.append(value)
-        		else:
-        			info[a.dest] = value
+            for a in p.subknots:
+                value = kwargs.pop(a.dest)
+                if a.ispositional:
+                    info.append(value)
+                else:
+                    info[a.dest] = value
         if len(kwargs):
-        	raise KeyError()
+            raise KeyError()
         result = info.exec(self._value)
         result = outfile.fileDataType(result)
         outfile.save(result)
     def _go(self):
-    	kwargs = self._read_gui()
-    	self._run(kwargs)
+        kwargs = self._read_gui()
+        self._run(kwargs)
+    @property
+    def _subknots(self):
+        ans = self.parameters
+        if self.argument_of_return is not None:
+            ans.append(self.argument_of_return)
+        return ans
     @property
     def parameters(self):
-    	return self.subknots[:-1]
+        return list(self._parameters)
     @property
     def argument_of_return(self):
-    	return self.subknots[-1]
+        return self._argument_of_return
 
 class _Uncallable(_Main):
     def __init__(self, value, return_details):
         self._dest = value._dest
         self._subknots = dict()
         parser = self._make_parser()
         subparsers = parser.add_subparsers(dest=value._dest)
         for n, m in _ins.getmembers(value):
             if n.startswith("_"):
                 continue
             self._subknots[n] = make(m, return_details=return_details)
             subparsers.add_parser(
-            	n.replace("_", "-"),
+                n.replace("_", "-"),
                 parents=[self._subknots[n].parser(add_help=False)],
                 add_help=True,
             )
         self._parser = self._make_parser(
             parents=[parser],
             description=value.__doc__,
         )
     def _run(self, kwargs):
         value = kwargs.pop(self.dest)
         return self.subknots[value]._run(kwargs)
     @property
     def dest(self):
-    	return self._dest
+        return self._dest
 
 
 
 def make(value, *, return_details):
     cls = _Callable if callable(value) else _Uncallable
     return cls(value, return_details=return_details)
```

### Comparing `lib-dzne-auto-interface-0.2.1/src/lib_dzne_auto_interface.egg-info/PKG-INFO` & `lib-dzne-auto-interface-0.2.2/src/lib_dzne_auto_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-auto-interface
-Version: 0.2.1
+Version: 0.2.2
 Summary: Libary for automatically created interfaces. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


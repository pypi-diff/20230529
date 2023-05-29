# Comparing `tmp/lib-dzne-seq-0.2.0.tar.gz` & `tmp/lib-dzne-seq-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-seq-0.2.0.tar", last modified: Thu May 18 18:14:56 2023, max compression
+gzip compressed data, was "lib-dzne-seq-0.2.2.tar", last modified: Mon May 29 12:51:47 2023, max compression
```

## Comparing `lib-dzne-seq-0.2.0.tar` & `lib-dzne-seq-0.2.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-seq-0.2.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1481 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      556 2023-05-18 17:21:53.000000 lib-dzne-seq-0.2.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/src/lib_dzne_seq/
--rw-rw-r--   0 base      (1001) base      (1001)     4030 2023-05-18 18:09:49.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq/__init__.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-18 18:14:56.972388 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1481 2023-05-18 18:14:56.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      260 2023-05-18 18:14:56.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-18 18:14:56.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       32 2023-05-18 18:14:56.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       13 2023-05-18 18:14:56.000000 lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:51:47.440034 lib-dzne-seq-0.2.2/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-seq-0.2.2/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1481 2023-05-29 12:51:47.440034 lib-dzne-seq-0.2.2/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       15 2023-05-29 09:16:34.000000 lib-dzne-seq-0.2.2/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      588 2023-05-29 12:51:33.000000 lib-dzne-seq-0.2.2/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-05-29 12:51:47.440034 lib-dzne-seq-0.2.2/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:51:47.440034 lib-dzne-seq-0.2.2/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:51:47.440034 lib-dzne-seq-0.2.2/src/lib_dzne_seq/
+-rw-rw-r--   0 base      (1001) base      (1001)     4668 2023-05-29 12:47:17.000000 lib-dzne-seq-0.2.2/src/lib_dzne_seq/__init__.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-05-29 12:51:47.440034 lib-dzne-seq-0.2.2/src/lib_dzne_seq.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1481 2023-05-29 12:51:47.000000 lib-dzne-seq-0.2.2/src/lib_dzne_seq.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      270 2023-05-29 12:51:47.000000 lib-dzne-seq-0.2.2/src/lib_dzne_seq.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-05-29 12:51:47.000000 lib-dzne-seq-0.2.2/src/lib_dzne_seq.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       57 2023-05-29 12:51:47.000000 lib-dzne-seq-0.2.2/src/lib_dzne_seq.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       13 2023-05-29 12:51:47.000000 lib-dzne-seq-0.2.2/src/lib_dzne_seq.egg-info/top_level.txt
```

### Comparing `lib-dzne-seq-0.2.0/LICENSE` & `lib-dzne-seq-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-seq-0.2.0/PKG-INFO` & `lib-dzne-seq-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-seq
-Version: 0.2.0
+Version: 0.2.2
 Summary: Libary for handling genetic sequences. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-seq-0.2.0/pyproject.toml` & `lib-dzne-seq-0.2.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-seq"
-version = "0.2.0"
+version = "0.2.2"
 description = "Libary for handling genetic sequences. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
 dependencies = [
     'Bio>=1.5.3',
-    'lib-dzne-data>=0.1.2',
+    'lib-dzne-math>=0.2.0',
+    'lib-dzne-filedata>=0.4.0',
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-seq-0.2.0/src/lib_dzne_seq/__init__.py` & `lib-dzne-seq-0.2.2/src/lib_dzne_seq/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import Bio.Seq as _Seq
 import Bio.SeqIO as _SeqIO
 import Bio.SeqRecord as _SeqRecord
-import lib_dzne_data as _lib_dzne_data
+import lib_dzne_filedata as _fd
+import lib_dzne_math.na as _na
 
 
 class SeqRead:
     def __init__(self, **kwargs):
         keys = set(kwargs.keys())
         if keys == {'seq', 'qv'}:
             self.seq = kwargs['seq']
@@ -53,17 +54,39 @@
         value = int(round(value))
         if 0 <= value <= 100:
             self._qv = value
         else:
             raise ValueError("Quality Value must be in the range from 0 to 100. ")
     
 
+class SeqReadData(_fd.FileData):
+    @staticmethod
+    def clone_data(data):
+        return SeqRead(read=data)
+    @classmethod
+    def _load(cls, /, file):
+        return SeqRead(file=file, format=cls._format)
+    def _save(self, /, file):
+        self._data.save(file=file, format=type(self)._format)
+    @classmethod
+    def _default(cls):
+        return SeqRead()
+    @classmethod
+    def from_file(cls, file, /):
+        return super().from_file(file, PHDSeqReadData, ABISeqReadData)
+
+class PHDSeqReadData(SeqReadData):
+    _ext = '.phd'
+    _format = 'phd'
+class ABISeqReadData(SeqReadData):
+    _ext = '.ab1'
+    _format = 'abi'
 
 def data(*, seq, go, end):
-    if _lib_dzne_data.anyisna(seq, go, end):
+    if _na.anyisna(seq, go, end):
         return None
     ans = dict()
     ans['go'] = go
     ans['end'] = end
     ans['seq'] = cut(seq, go, end, strict=True)
     ans['seq-len'] = len(ans['seq'])
     ans['tr'] = tr(ans['seq'])
@@ -136,15 +159,15 @@
         'T':-0.7,
         'V':4.2,
         'W':-0.9,
         'X':float('nan'),
         'Y':-1.3,
         '-':float('nan'),
     }
-    answers = [values[k] for k in translation if _lib_dzne_data.notna(values[k])]
+    answers = [values[k] for k in translation if _na.notna(values[k])]
     if len(answers):
         return sum(answers) / len(answers)
     return float('nan')
```

### Comparing `lib-dzne-seq-0.2.0/src/lib_dzne_seq.egg-info/PKG-INFO` & `lib-dzne-seq-0.2.2/src/lib_dzne_seq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-seq
-Version: 0.2.0
+Version: 0.2.2
 Summary: Libary for handling genetic sequences. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```


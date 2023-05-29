# Comparing `tmp/urlopen2-1.0.0.tar.gz` & `tmp/urlopen2-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urlopen2-1.0.0.tar", max compression
+gzip compressed data, was "urlopen2-1.0.1.tar", max compression
```

## Comparing `urlopen2-1.0.0.tar` & `urlopen2-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1084 2023-05-29 07:15:28.083692 urlopen2-1.0.0/LICENSE
--rw-r--r--   0        0        0      409 2023-05-29 07:32:49.450952 urlopen2-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      514 2023-05-29 08:06:49.944797 urlopen2-1.0.0/README.md
--rw-r--r--   0        0        0       28 2023-05-29 06:42:37.689478 urlopen2-1.0.0/urlopen2/__init__.py
--rw-r--r--   0        0        0     2673 2023-05-29 07:40:17.403452 urlopen2-1.0.0/urlopen2/urlfile.py
--rw-r--r--   0        0        0      720 2023-05-29 07:40:28.892802 urlopen2-1.0.0/urlopen2/urlfile.pyi
--rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 urlopen2-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-29 07:15:28.083692 urlopen2-1.0.1/LICENSE
+-rw-r--r--   0        0        0      409 2023-05-29 09:38:35.642659 urlopen2-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      514 2023-05-29 08:06:49.944797 urlopen2-1.0.1/README.md
+-rw-r--r--   0        0        0       28 2023-05-29 06:42:37.689478 urlopen2-1.0.1/urlopen2/__init__.py
+-rw-r--r--   0        0        0     2751 2023-05-29 09:35:54.223369 urlopen2-1.0.1/urlopen2/urlfile.py
+-rw-r--r--   0        0        0      720 2023-05-29 07:40:28.892802 urlopen2-1.0.1/urlopen2/urlfile.pyi
+-rw-r--r--   0        0        0     1058 1970-01-01 00:00:00.000000 urlopen2-1.0.1/PKG-INFO
```

### Comparing `urlopen2-1.0.0/LICENSE` & `urlopen2-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `urlopen2-1.0.0/README.md` & `urlopen2-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `urlopen2-1.0.0/urlopen2/urlfile.py` & `urlopen2-1.0.1/urlopen2/urlfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,25 +54,28 @@
     
     def _fullload(self) -> None:
         if not self._full:
             ct = self.tell()
             self._buffer.seek(0, 2)
             while len(data:=self._furl.read(65536)) > 0:
                 self._buffer.write(data)
+            self._furl.close()
             self._full = True
-            self._buffer.close()
             self._buffer.seek(ct)
     
     def read(self, n: int=-1):
         if n is None:
             n = -1
-        if (n > 0) and (not self._full):
-            s = n - (self._getsize() - self.tell())
-            if s > 0:
-                self._topload(s)
+        if not self._full:
+            if n > 0:
+                s = n - (self._getsize() - self.tell())
+                if s > 0:
+                    self._topload(s)
+            elif n < 0:
+                self._fullload()
         return self._buffer.read(n)
     
     def seek(self, offset: int, whence: int=0) -> None:
         if (offset > 0) and (not self._full):
             if whence == 0:
                 s = self._getsize() - offset
                 if s > 0:
```

### Comparing `urlopen2-1.0.0/urlopen2/urlfile.pyi` & `urlopen2-1.0.1/urlopen2/urlfile.pyi`

 * *Files identical despite different names*

### Comparing `urlopen2-1.0.0/PKG-INFO` & `urlopen2-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urlopen2
-Version: 1.0.0
+Version: 1.0.1
 Summary: Improvement for the `urlopen` function.
 License: MIT
 Keywords: urlopen,urllib.request,urlfile,readable,seekable
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```


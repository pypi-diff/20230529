# Comparing `tmp/libtetrabz-0.1.0.tar.gz` & `tmp/libtetrabz-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libtetrabz-0.1.0.tar", last modified: Thu Mar 31 13:09:02 2022, max compression
+gzip compressed data, was "libtetrabz-0.1.1.tar", last modified: Mon May 29 08:48:10 2023, max compression
```

## Comparing `libtetrabz-0.1.0.tar` & `libtetrabz-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,16 @@
-drwxrwxrwx   0 kawamura  (1000) kawamura  (1000)        0 2022-03-31 13:09:02.414558 libtetrabz-0.1.0/
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)      106 2022-03-24 11:21:39.000000 libtetrabz-0.1.0/.gitignore
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)     1075 2021-10-21 16:53:53.000000 libtetrabz-0.1.0/LICENSE
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)     1460 2022-03-31 13:09:02.412022 libtetrabz-0.1.0/PKG-INFO
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)      891 2022-03-31 10:04:05.000000 libtetrabz-0.1.0/README.md
-drwxrwxrwx   0 kawamura  (1000) kawamura  (1000)        0 2022-03-31 13:09:02.310860 libtetrabz-0.1.0/doc/
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)      634 2021-11-08 07:12:42.000000 libtetrabz-0.1.0/doc/Makefile
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)    13024 2021-11-08 08:42:07.000000 libtetrabz-0.1.0/doc/api.rst
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)     1932 2021-11-08 08:23:52.000000 libtetrabz-0.1.0/doc/conf.py
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)      521 2021-11-17 03:16:23.000000 libtetrabz-0.1.0/doc/index.rst
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)     2421 2021-11-17 03:12:32.000000 libtetrabz-0.1.0/doc/overview.rst
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)      184 2021-11-08 07:38:01.000000 libtetrabz-0.1.0/doc/ref.rst
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)      117 2021-11-07 13:17:18.000000 libtetrabz-0.1.0/pyproject.toml
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)       38 2022-03-31 13:09:02.415549 libtetrabz-0.1.0/setup.cfg
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)      930 2022-03-31 10:04:43.000000 libtetrabz-0.1.0/setup.py
-drwxrwxrwx   0 kawamura  (1000) kawamura  (1000)        0 2022-03-31 13:09:02.332564 libtetrabz-0.1.0/src/
-drwxrwxrwx   0 kawamura  (1000) kawamura  (1000)        0 2022-03-31 13:09:02.349337 libtetrabz-0.1.0/src/libtetrabz/
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)     8439 2022-03-24 14:36:05.000000 libtetrabz-0.1.0/src/libtetrabz/__init__.py
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)   123835 2022-03-24 14:36:27.000000 libtetrabz-0.1.0/src/libtetrabz/libtetrabz.c
-drwxrwxrwx   0 kawamura  (1000) kawamura  (1000)        0 2022-03-31 13:09:02.397254 libtetrabz-0.1.0/src/libtetrabz.egg-info/
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)     1460 2022-03-31 13:09:00.000000 libtetrabz-0.1.0/src/libtetrabz.egg-info/PKG-INFO
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)      381 2022-03-31 13:09:02.000000 libtetrabz-0.1.0/src/libtetrabz.egg-info/SOURCES.txt
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)        1 2022-03-31 13:09:00.000000 libtetrabz-0.1.0/src/libtetrabz.egg-info/dependency_links.txt
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)       11 2022-03-31 13:09:01.000000 libtetrabz-0.1.0/src/libtetrabz.egg-info/top_level.txt
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)    42273 2022-03-31 11:49:15.000000 libtetrabz-0.1.0/src/libtetrabz_tutorial.ipynb
--rwxrwxrwx   0 kawamura  (1000) kawamura  (1000)    11749 2021-11-04 13:53:56.000000 libtetrabz-0.1.0/src/test.py
+drwxr-xr-x   0 kawamura  (1000) kawamura  (1000)        0 2023-05-29 08:48:10.022018 libtetrabz-0.1.1/
+-rw-r--r--   0 kawamura  (1000) kawamura  (1000)     1075 2021-10-21 16:53:53.000000 libtetrabz-0.1.1/LICENSE
+-rw-r--r--   0 kawamura  (1000) kawamura  (1000)     1500 2023-05-29 08:48:10.022018 libtetrabz-0.1.1/PKG-INFO
+-rw-r--r--   0 kawamura  (1000) kawamura  (1000)      948 2023-05-29 08:33:16.000000 libtetrabz-0.1.1/README.md
+-rw-r--r--   0 kawamura  (1000) kawamura  (1000)      117 2021-11-07 13:17:18.000000 libtetrabz-0.1.1/pyproject.toml
+-rw-r--r--   0 kawamura  (1000) kawamura  (1000)       38 2023-05-29 08:48:10.022018 libtetrabz-0.1.1/setup.cfg
+-rwxr--r--   0 kawamura  (1000) kawamura  (1000)      950 2023-05-29 08:34:17.000000 libtetrabz-0.1.1/setup.py
+drwxr-xr-x   0 kawamura  (1000) kawamura  (1000)        0 2023-05-29 08:48:10.022018 libtetrabz-0.1.1/src/
+drwxr-xr-x   0 kawamura  (1000) kawamura  (1000)        0 2023-05-29 08:48:10.022018 libtetrabz-0.1.1/src/libtetrabz/
+-rwxr--r--   0 kawamura  (1000) kawamura  (1000)     8439 2022-03-24 14:36:05.000000 libtetrabz-0.1.1/src/libtetrabz/__init__.py
+-rw-r--r--   0 kawamura  (1000) kawamura  (1000)   123835 2022-03-24 14:36:27.000000 libtetrabz-0.1.1/src/libtetrabz/libtetrabz.c
+drwxr-xr-x   0 kawamura  (1000) kawamura  (1000)        0 2023-05-29 08:48:10.022018 libtetrabz-0.1.1/src/libtetrabz.egg-info/
+-rw-r--r--   0 kawamura  (1000) kawamura  (1000)     1500 2023-05-29 08:48:10.000000 libtetrabz-0.1.1/src/libtetrabz.egg-info/PKG-INFO
+-rw-r--r--   0 kawamura  (1000) kawamura  (1000)      248 2023-05-29 08:48:10.000000 libtetrabz-0.1.1/src/libtetrabz.egg-info/SOURCES.txt
+-rw-r--r--   0 kawamura  (1000) kawamura  (1000)        1 2023-05-29 08:48:10.000000 libtetrabz-0.1.1/src/libtetrabz.egg-info/dependency_links.txt
+-rw-r--r--   0 kawamura  (1000) kawamura  (1000)       11 2023-05-29 08:48:10.000000 libtetrabz-0.1.1/src/libtetrabz.egg-info/top_level.txt
```

### Comparing `libtetrabz-0.1.0/LICENSE` & `libtetrabz-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `libtetrabz-0.1.0/PKG-INFO` & `libtetrabz-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: libtetrabz
-Version: 0.1.0
+Version: 0.1.1
 Summary: Optimized tetrahedron method to perform brillouin-zone integral
-Home-page: https://libtetrabz.osdn.jp/
+Home-page: https://mitsuaki1987.github.io/libtetrabz/
 Author: Mitsuaki Kawamura
 Author-email: kawamitsuaki@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://osdn.net/projects/libtetrabz/forums/
-Platform: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/mitsuaki1987/libtetrabz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -21,19 +19,19 @@
 integration in the electronic structure calculation in a solid by 
 using the tetrahedron method.
 
 ## Quick start guide
 
 To experience libtetrabz, please open the following python notebook with jupyter, Google colab, etc.
 
-https://libtetrabz.osdn.jp/python/libtetrabz_tutorial.ipynb
+https://github.com/mitsuaki1987/libtetrabz/blob/main/python/src/libtetrabz_tutorial.ipynb
 
 ## Manual
 
-https://libtetrabz.osdn.jp/python/
+https://mitsuaki1987.github.io/libtetrabz/python/_build/html/index.html
 
 ## For citing libtetrabz
 We would appreciate if you cite the following article in your 
 research with libtetrabz.
 
 "Improved tetrahedron method for the Brillouin-zone integration applicable to response functions",
 
@@ -41,10 +39,8 @@
 arXiv:2203.15648
 
 https://journals.aps.org/prb/abstract/10.1103/PhysRevB.89.094515
 https://arxiv.org/abs/2203.15648
 
 ## Git repository
 
-https://osdn.net/projects/libtetrabz/scm/git/python/
-
-
+https://github.com/mitsuaki1987/libtetrabz
```

### Comparing `libtetrabz-0.1.0/README.md` & `libtetrabz-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 integration in the electronic structure calculation in a solid by 
 using the tetrahedron method.
 
 ## Quick start guide
 
 To experience libtetrabz, please open the following python notebook with jupyter, Google colab, etc.
 
-https://libtetrabz.osdn.jp/python/libtetrabz_tutorial.ipynb
+https://github.com/mitsuaki1987/libtetrabz/blob/main/python/src/libtetrabz_tutorial.ipynb
 
 ## Manual
 
-https://libtetrabz.osdn.jp/python/
+https://mitsuaki1987.github.io/libtetrabz/python/_build/html/index.html
 
 ## For citing libtetrabz
 We would appreciate if you cite the following article in your 
 research with libtetrabz.
 
 "Improved tetrahedron method for the Brillouin-zone integration applicable to response functions",
 
@@ -24,8 +24,8 @@
 arXiv:2203.15648
 
 https://journals.aps.org/prb/abstract/10.1103/PhysRevB.89.094515
 https://arxiv.org/abs/2203.15648
 
 ## Git repository
 
-https://osdn.net/projects/libtetrabz/scm/git/python/
+https://github.com/mitsuaki1987/libtetrabz
```

### Comparing `libtetrabz-0.1.0/src/libtetrabz/__init__.py` & `libtetrabz-0.1.1/src/libtetrabz/__init__.py`

 * *Files identical despite different names*

### Comparing `libtetrabz-0.1.0/src/libtetrabz/libtetrabz.c` & `libtetrabz-0.1.1/src/libtetrabz/libtetrabz.c`

 * *Files identical despite different names*

### Comparing `libtetrabz-0.1.0/src/libtetrabz.egg-info/PKG-INFO` & `libtetrabz-0.1.1/src/libtetrabz.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: libtetrabz
-Version: 0.1.0
+Version: 0.1.1
 Summary: Optimized tetrahedron method to perform brillouin-zone integral
-Home-page: https://libtetrabz.osdn.jp/
+Home-page: https://mitsuaki1987.github.io/libtetrabz/
 Author: Mitsuaki Kawamura
 Author-email: kawamitsuaki@gmail.com
-License: UNKNOWN
-Project-URL: Bug Tracker, https://osdn.net/projects/libtetrabz/forums/
-Platform: UNKNOWN
+Project-URL: Bug Tracker, https://github.com/mitsuaki1987/libtetrabz/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -21,19 +19,19 @@
 integration in the electronic structure calculation in a solid by 
 using the tetrahedron method.
 
 ## Quick start guide
 
 To experience libtetrabz, please open the following python notebook with jupyter, Google colab, etc.
 
-https://libtetrabz.osdn.jp/python/libtetrabz_tutorial.ipynb
+https://github.com/mitsuaki1987/libtetrabz/blob/main/python/src/libtetrabz_tutorial.ipynb
 
 ## Manual
 
-https://libtetrabz.osdn.jp/python/
+https://mitsuaki1987.github.io/libtetrabz/python/_build/html/index.html
 
 ## For citing libtetrabz
 We would appreciate if you cite the following article in your 
 research with libtetrabz.
 
 "Improved tetrahedron method for the Brillouin-zone integration applicable to response functions",
 
@@ -41,10 +39,8 @@
 arXiv:2203.15648
 
 https://journals.aps.org/prb/abstract/10.1103/PhysRevB.89.094515
 https://arxiv.org/abs/2203.15648
 
 ## Git repository
 
-https://osdn.net/projects/libtetrabz/scm/git/python/
-
-
+https://github.com/mitsuaki1987/libtetrabz
```


# Comparing `tmp/HEIC2PNG-1.0.0.tar.gz` & `tmp/HEIC2PNG-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HEIC2PNG-1.0.0.tar", last modified: Sat Sep  3 18:48:14 2022, max compression
+gzip compressed data, was "HEIC2PNG-1.0.1.tar", last modified: Mon May 29 05:06:09 2023, max compression
```

## Comparing `HEIC2PNG-1.0.0.tar` & `HEIC2PNG-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 18:48:14.365208 HEIC2PNG-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-09-03 18:48:06.000000 HEIC2PNG-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       85 2022-09-03 18:48:06.000000 HEIC2PNG-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-09-03 18:48:14.365208 HEIC2PNG-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1225 2022-09-03 18:48:06.000000 HEIC2PNG-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       98 2022-09-03 18:48:06.000000 HEIC2PNG-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      111 2022-09-03 18:48:14.365208 HEIC2PNG-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1671 2022-09-03 18:48:06.000000 HEIC2PNG-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 18:48:14.361207 HEIC2PNG-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 18:48:14.365208 HEIC2PNG-1.0.0/src/HEIC2PNG.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2279 2022-09-03 18:48:14.000000 HEIC2PNG-1.0.0/src/HEIC2PNG.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      374 2022-09-03 18:48:14.000000 HEIC2PNG-1.0.0/src/HEIC2PNG.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-03 18:48:14.000000 HEIC2PNG-1.0.0/src/HEIC2PNG.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-03 18:48:14.000000 HEIC2PNG-1.0.0/src/HEIC2PNG.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       46 2022-09-03 18:48:14.000000 HEIC2PNG-1.0.0/src/HEIC2PNG.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-03 18:48:14.000000 HEIC2PNG-1.0.0/src/HEIC2PNG.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 18:48:14.365208 HEIC2PNG-1.0.0/src/heic2png/
--rw-r--r--   0 runner    (1001) docker     (121)       68 2022-09-03 18:48:06.000000 HEIC2PNG-1.0.0/src/heic2png/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      882 2022-09-03 18:48:06.000000 HEIC2PNG-1.0.0/src/heic2png/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)      883 2022-09-03 18:48:06.000000 HEIC2PNG-1.0.0/src/heic2png/heic2png.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 18:48:14.365208 HEIC2PNG-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-09-03 18:48:06.000000 HEIC2PNG-1.0.0/tests/test_heic2png.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:06:08.998602 HEIC2PNG-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-29 05:05:56.000000 HEIC2PNG-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-29 05:05:56.000000 HEIC2PNG-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-29 05:06:08.998602 HEIC2PNG-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-29 05:05:56.000000 HEIC2PNG-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-29 05:05:56.000000 HEIC2PNG-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-29 05:06:08.998602 HEIC2PNG-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-29 05:05:56.000000 HEIC2PNG-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:06:08.990602 HEIC2PNG-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:06:08.994602 HEIC2PNG-1.0.1/src/HEIC2PNG.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2279 2023-05-29 05:06:08.000000 HEIC2PNG-1.0.1/src/HEIC2PNG.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 05:06:08.000000 HEIC2PNG-1.0.1/src/HEIC2PNG.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 05:06:08.000000 HEIC2PNG-1.0.1/src/HEIC2PNG.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-29 05:06:08.000000 HEIC2PNG-1.0.1/src/HEIC2PNG.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-29 05:06:08.000000 HEIC2PNG-1.0.1/src/HEIC2PNG.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 05:06:08.000000 HEIC2PNG-1.0.1/src/HEIC2PNG.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:06:08.998602 HEIC2PNG-1.0.1/src/heic2png/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-29 05:05:56.000000 HEIC2PNG-1.0.1/src/heic2png/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-29 05:05:56.000000 HEIC2PNG-1.0.1/src/heic2png/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-29 05:05:56.000000 HEIC2PNG-1.0.1/src/heic2png/heic2png.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 05:06:08.998602 HEIC2PNG-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-29 05:05:56.000000 HEIC2PNG-1.0.1/tests/test_heic2png.py
```

### Comparing `HEIC2PNG-1.0.0/LICENSE` & `HEIC2PNG-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `HEIC2PNG-1.0.0/PKG-INFO` & `HEIC2PNG-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HEIC2PNG
-Version: 1.0.0
+Version: 1.0.1
 Summary: Convert format of HEIC image to PNG by using Python.
 Home-page: https://github.com/natlee/HEIC2PNG
 Author: Nat Lee
 Author-email: natlee.work@gmail.com
 Project-URL: Documentation, https://github.com/natlee/HEIC2PNG
 Project-URL: Bug Reports, https://github.com/natlee/HEIC2PNG/issues
 Project-URL: Source Code, https://github.com/natlee/HEIC2PNG
```

### Comparing `HEIC2PNG-1.0.0/README.md` & `HEIC2PNG-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `HEIC2PNG-1.0.0/setup.py` & `HEIC2PNG-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `HEIC2PNG-1.0.0/src/HEIC2PNG.egg-info/PKG-INFO` & `HEIC2PNG-1.0.1/src/HEIC2PNG.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HEIC2PNG
-Version: 1.0.0
+Version: 1.0.1
 Summary: Convert format of HEIC image to PNG by using Python.
 Home-page: https://github.com/natlee/HEIC2PNG
 Author: Nat Lee
 Author-email: natlee.work@gmail.com
 Project-URL: Documentation, https://github.com/natlee/HEIC2PNG
 Project-URL: Bug Reports, https://github.com/natlee/HEIC2PNG/issues
 Project-URL: Source Code, https://github.com/natlee/HEIC2PNG
```

### Comparing `HEIC2PNG-1.0.0/src/heic2png/cli.py` & `HEIC2PNG-1.0.1/src/heic2png/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         print(f'----- Set the output path is `{output_path}`')
     try:
         heic_img = HEIC2PNG(input_path)
         print(f'----- Processing...')
         output_path = heic_img.save(output_path)
         print(f'----- Output file path is `{output_path}`')
     except FileExistsError:
-        print('----- File has been already existed!')
+        print('----- File already exists!')
     except ValueError:
         print('----- You need to check the format of image!')
         print('Input must be `.heic` and output must be `.png`.')
     except Exception as e:
         print(f'----- Error with {e}')
         print('----- Please report this issue!')
```

### Comparing `HEIC2PNG-1.0.0/src/heic2png/heic2png.py` & `HEIC2PNG-1.0.1/src/heic2png/heic2png.py`

 * *Files identical despite different names*

### Comparing `HEIC2PNG-1.0.0/tests/test_heic2png.py` & `HEIC2PNG-1.0.1/tests/test_heic2png.py`

 * *Files identical despite different names*


# Comparing `tmp/nounseed-1.0.1.tar.gz` & `tmp/nounseed-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nounseed-1.0.1.tar", last modified: Sun May 28 23:33:39 2023, max compression
+gzip compressed data, was "nounseed-1.0.2.tar", last modified: Sun May 28 23:45:01 2023, max compression
```

## Comparing `nounseed-1.0.1.tar` & `nounseed-1.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-28 23:33:39.871210 nounseed-1.0.1/
--rw-r--r--   0 bloom      (501) staff       (20)     1074 2023-05-23 23:15:34.000000 nounseed-1.0.1/LICENSE
--rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-28 23:33:39.871082 nounseed-1.0.1/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)     1710 2023-05-28 23:21:44.000000 nounseed-1.0.1/README.md
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-28 23:33:39.870271 nounseed-1.0.1/nounseed/
--rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 00:19:28.000000 nounseed-1.0.1/nounseed/__init__.py
--rw-r--r--   0 bloom      (501) staff       (20)     5060 2023-05-28 23:29:25.000000 nounseed-1.0.1/nounseed/__main__.py
-drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-28 23:33:39.870905 nounseed-1.0.1/nounseed.egg-info/
--rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-28 23:33:39.000000 nounseed-1.0.1/nounseed.egg-info/PKG-INFO
--rw-r--r--   0 bloom      (501) staff       (20)      277 2023-05-28 23:33:39.000000 nounseed-1.0.1/nounseed.egg-info/SOURCES.txt
--rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-28 23:33:39.000000 nounseed-1.0.1/nounseed.egg-info/dependency_links.txt
--rw-r--r--   0 bloom      (501) staff       (20)       53 2023-05-28 23:33:39.000000 nounseed-1.0.1/nounseed.egg-info/entry_points.txt
--rw-r--r--   0 bloom      (501) staff       (20)       17 2023-05-28 23:33:39.000000 nounseed-1.0.1/nounseed.egg-info/requires.txt
--rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-28 23:33:39.000000 nounseed-1.0.1/nounseed.egg-info/top_level.txt
--rw-r--r--   0 bloom      (501) staff       (20)       90 2023-05-28 22:55:02.000000 nounseed-1.0.1/pyproject.toml
--rw-r--r--   0 bloom      (501) staff       (20)       38 2023-05-28 23:33:39.871254 nounseed-1.0.1/setup.cfg
--rw-r--r--   0 bloom      (501) staff       (20)      379 2023-05-28 23:33:26.000000 nounseed-1.0.1/setup.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-28 23:45:01.880256 nounseed-1.0.2/
+-rw-r--r--   0 bloom      (501) staff       (20)     1074 2023-05-23 23:15:34.000000 nounseed-1.0.2/LICENSE
+-rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-28 23:45:01.880106 nounseed-1.0.2/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)     1710 2023-05-28 23:44:14.000000 nounseed-1.0.2/README.md
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-28 23:45:01.879126 nounseed-1.0.2/nounseed/
+-rw-r--r--   0 bloom      (501) staff       (20)        0 2023-05-24 00:19:28.000000 nounseed-1.0.2/nounseed/__init__.py
+-rw-r--r--   0 bloom      (501) staff       (20)     5056 2023-05-28 23:43:50.000000 nounseed-1.0.2/nounseed/__main__.py
+drwxr-xr-x   0 bloom      (501) staff       (20)        0 2023-05-28 23:45:01.879894 nounseed-1.0.2/nounseed.egg-info/
+-rw-r--r--   0 bloom      (501) staff       (20)      213 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/PKG-INFO
+-rw-r--r--   0 bloom      (501) staff       (20)      277 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/SOURCES.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        1 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/dependency_links.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       53 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/entry_points.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       17 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/requires.txt
+-rw-r--r--   0 bloom      (501) staff       (20)        9 2023-05-28 23:45:01.000000 nounseed-1.0.2/nounseed.egg-info/top_level.txt
+-rw-r--r--   0 bloom      (501) staff       (20)       90 2023-05-28 22:55:02.000000 nounseed-1.0.2/pyproject.toml
+-rw-r--r--   0 bloom      (501) staff       (20)       38 2023-05-28 23:45:01.880302 nounseed-1.0.2/setup.cfg
+-rw-r--r--   0 bloom      (501) staff       (20)      379 2023-05-28 23:44:50.000000 nounseed-1.0.2/setup.py
```

### Comparing `nounseed-1.0.1/LICENSE` & `nounseed-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nounseed-1.0.1/README.md` & `nounseed-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nounseed-1.0.1/nounseed/__main__.py` & `nounseed-1.0.2/nounseed/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,8 +142,7 @@
         ideas_manager.ideas = ideas_manager.original_ideas
 
     print("Exiting the program.")
 
 
 if __name__ == '__main__':
     main()
-
```


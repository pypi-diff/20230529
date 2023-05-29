# Comparing `tmp/MinAtar-1.0.14.tar.gz` & `tmp/MinAtar-1.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MinAtar-1.0.14.tar", last modified: Mon May  8 17:31:51 2023, max compression
+gzip compressed data, was "MinAtar-1.0.15.tar", last modified: Mon May 29 16:45:26 2023, max compression
```

## Comparing `MinAtar-1.0.14.tar` & `MinAtar-1.0.15.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 17:31:51.631857 MinAtar-1.0.14/
-drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 17:31:51.623069 MinAtar-1.0.14/MinAtar.egg-info/
--rw-r--r--   0 kjyoung    (502) staff       (20)      260 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/PKG-INFO
--rw-r--r--   0 kjyoung    (502) staff       (20)      496 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/SOURCES.txt
--rw-r--r--   0 kjyoung    (502) staff       (20)        1 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/dependency_links.txt
--rw-r--r--   0 kjyoung    (502) staff       (20)       47 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/entry_points.txt
--rw-r--r--   0 kjyoung    (502) staff       (20)      198 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/requires.txt
--rw-r--r--   0 kjyoung    (502) staff       (20)        8 2023-05-08 17:31:51.000000 MinAtar-1.0.14/MinAtar.egg-info/top_level.txt
--rw-r--r--   0 kjyoung    (502) staff       (20)      260 2023-05-08 17:31:51.631412 MinAtar-1.0.14/PKG-INFO
--rw-r--r--   0 kjyoung    (502) staff       (20)    14086 2023-05-08 17:20:45.000000 MinAtar-1.0.14/README.md
-drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 17:31:51.625642 MinAtar-1.0.14/minatar/
--rw-r--r--   0 kjyoung    (502) staff       (20)       36 2021-11-05 15:11:24.000000 MinAtar-1.0.14/minatar/__init__.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     3935 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environment.py
-drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-08 17:31:51.630689 MinAtar-1.0.14/minatar/environments/
--rw-r--r--   0 kjyoung    (502) staff       (20)       15 2021-11-05 15:11:24.000000 MinAtar-1.0.14/minatar/environments/__init__.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     6222 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environments/asterix.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     5100 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environments/breakout.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     5819 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environments/freeway.py
--rw-r--r--   0 kjyoung    (502) staff       (20)    13034 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environments/seaquest.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     6887 2023-05-08 16:54:56.000000 MinAtar-1.0.14/minatar/environments/space_invaders.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     4085 2021-11-05 15:11:24.000000 MinAtar-1.0.14/minatar/gui.py
--rw-r--r--   0 kjyoung    (502) staff       (20)     3252 2023-05-08 17:20:45.000000 MinAtar-1.0.14/minatar/gym.py
--rw-r--r--   0 kjyoung    (502) staff       (20)       93 2022-04-10 19:37:26.000000 MinAtar-1.0.14/pyproject.toml
--rw-r--r--   0 kjyoung    (502) staff       (20)       38 2023-05-08 17:31:51.632012 MinAtar-1.0.14/setup.cfg
--rw-r--r--   0 kjyoung    (502) staff       (20)      877 2023-05-08 17:20:45.000000 MinAtar-1.0.14/setup.py
+drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-29 16:45:26.262312 MinAtar-1.0.15/
+drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-29 16:45:26.258729 MinAtar-1.0.15/MinAtar.egg-info/
+-rw-r--r--   0 kjyoung    (502) staff       (20)      260 2023-05-29 16:45:26.000000 MinAtar-1.0.15/MinAtar.egg-info/PKG-INFO
+-rw-r--r--   0 kjyoung    (502) staff       (20)      496 2023-05-29 16:45:26.000000 MinAtar-1.0.15/MinAtar.egg-info/SOURCES.txt
+-rw-r--r--   0 kjyoung    (502) staff       (20)        1 2023-05-29 16:45:26.000000 MinAtar-1.0.15/MinAtar.egg-info/dependency_links.txt
+-rw-r--r--   0 kjyoung    (502) staff       (20)       53 2023-05-29 16:45:26.000000 MinAtar-1.0.15/MinAtar.egg-info/entry_points.txt
+-rw-r--r--   0 kjyoung    (502) staff       (20)      198 2023-05-29 16:45:26.000000 MinAtar-1.0.15/MinAtar.egg-info/requires.txt
+-rw-r--r--   0 kjyoung    (502) staff       (20)        8 2023-05-29 16:45:26.000000 MinAtar-1.0.15/MinAtar.egg-info/top_level.txt
+-rw-r--r--   0 kjyoung    (502) staff       (20)      260 2023-05-29 16:45:26.262057 MinAtar-1.0.15/PKG-INFO
+-rw-r--r--   0 kjyoung    (502) staff       (20)    14086 2023-05-08 17:20:45.000000 MinAtar-1.0.15/README.md
+drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-29 16:45:26.259925 MinAtar-1.0.15/minatar/
+-rw-r--r--   0 kjyoung    (502) staff       (20)       36 2021-11-05 15:11:24.000000 MinAtar-1.0.15/minatar/__init__.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     3935 2023-05-08 16:54:56.000000 MinAtar-1.0.15/minatar/environment.py
+drwxr-xr-x   0 kjyoung    (502) staff       (20)        0 2023-05-29 16:45:26.261701 MinAtar-1.0.15/minatar/environments/
+-rw-r--r--   0 kjyoung    (502) staff       (20)       15 2021-11-05 15:11:24.000000 MinAtar-1.0.15/minatar/environments/__init__.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     6222 2023-05-08 16:54:56.000000 MinAtar-1.0.15/minatar/environments/asterix.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     5100 2023-05-08 16:54:56.000000 MinAtar-1.0.15/minatar/environments/breakout.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     5819 2023-05-08 16:54:56.000000 MinAtar-1.0.15/minatar/environments/freeway.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)    13034 2023-05-08 16:54:56.000000 MinAtar-1.0.15/minatar/environments/seaquest.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     6887 2023-05-08 16:54:56.000000 MinAtar-1.0.15/minatar/environments/space_invaders.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     4085 2021-11-05 15:11:24.000000 MinAtar-1.0.15/minatar/gui.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)     3252 2023-05-08 17:20:45.000000 MinAtar-1.0.15/minatar/gym.py
+-rw-r--r--   0 kjyoung    (502) staff       (20)       93 2022-04-10 19:37:26.000000 MinAtar-1.0.15/pyproject.toml
+-rw-r--r--   0 kjyoung    (502) staff       (20)       38 2023-05-29 16:45:26.262397 MinAtar-1.0.15/setup.cfg
+-rw-r--r--   0 kjyoung    (502) staff       (20)      883 2023-05-29 16:43:48.000000 MinAtar-1.0.15/setup.py
```

### Comparing `MinAtar-1.0.14/README.md` & `MinAtar-1.0.15/README.md`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.14/minatar/environment.py` & `MinAtar-1.0.15/minatar/environment.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.14/minatar/environments/asterix.py` & `MinAtar-1.0.15/minatar/environments/asterix.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.14/minatar/environments/breakout.py` & `MinAtar-1.0.15/minatar/environments/breakout.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.14/minatar/environments/freeway.py` & `MinAtar-1.0.15/minatar/environments/freeway.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.14/minatar/environments/seaquest.py` & `MinAtar-1.0.15/minatar/environments/seaquest.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.14/minatar/environments/space_invaders.py` & `MinAtar-1.0.15/minatar/environments/space_invaders.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.14/minatar/gui.py` & `MinAtar-1.0.15/minatar/gui.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.14/minatar/gym.py` & `MinAtar-1.0.15/minatar/gym.py`

 * *Files identical despite different names*

### Comparing `MinAtar-1.0.14/setup.py` & `MinAtar-1.0.15/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 ]
 
 examples_requires = [
     'torch>=1.0.0',
 ]
 
 entry_points = {
-    'gym.envs': ['MinAtar=minatar.gym:register_envs']
+    'gymnasium.envs': ['MinAtar=minatar.gym:register_envs']
 }
 
 setup(
     name='MinAtar',
-    version='1.0.14',
+    version='1.0.15',
     description='A miniaturized version of the Arcade Learning Environment.',
     url='https://github.com/kenjyoung/MinAtar',
     author='Kenny Young',
     author_email='kjyoung@ualberta.ca',
     license='GPL',
     packages=packages,
     entry_points=entry_points,
```


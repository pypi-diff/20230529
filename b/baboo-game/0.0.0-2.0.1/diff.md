# Comparing `tmp/baboo_game-0.0.0.tar.gz` & `tmp/baboo_game-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baboo_game-0.0.0.tar", last modified: Mon May 29 16:31:07 2023, max compression
+gzip compressed data, was "baboo_game-2.0.1.tar", last modified: Mon May 29 16:26:50 2023, max compression
```

## Comparing `baboo_game-0.0.0.tar` & `baboo_game-2.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:31:07.296459 baboo_game-0.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:31:07.292459 baboo_game-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:31:07.296459 baboo_game-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-29 16:30:56.000000 baboo_game-0.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-29 16:30:56.000000 baboo_game-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 16:30:56.000000 baboo_game-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-29 16:31:07.296459 baboo_game-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-29 16:30:56.000000 baboo_game-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-29 16:30:56.000000 baboo_game-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 16:30:56.000000 baboo_game-0.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:31:07.296459 baboo_game-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:31:07.296459 baboo_game-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:31:07.296459 baboo_game-0.0.0/src/baboo_game/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:31:07.296459 baboo_game-0.0.0/src/baboo_game/game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/game/baboo_game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:31:07.296459 baboo_game-0.0.0/src/baboo_game/game/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/game/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/game/config/color_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/game/config/game_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/game/config/text_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:31:07.296459 baboo_game-0.0.0/src/baboo_game/game/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/game/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/game/library/abstract_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/game/render_game.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 16:30:56.000000 baboo_game-0.0.0/src/baboo_game/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:31:07.296459 baboo_game-0.0.0/src/baboo_game.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-29 16:31:07.000000 baboo_game-0.0.0/src/baboo_game.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-29 16:31:07.000000 baboo_game-0.0.0/src/baboo_game.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:31:07.000000 baboo_game-0.0.0/src/baboo_game.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 16:31:07.000000 baboo_game-0.0.0/src/baboo_game.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 16:31:07.000000 baboo_game-0.0.0/src/baboo_game.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.665062 baboo_game-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.661062 baboo_game-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.661062 baboo_game-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-29 16:26:37.000000 baboo_game-2.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-29 16:26:37.000000 baboo_game-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 16:26:37.000000 baboo_game-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-29 16:26:50.665062 baboo_game-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-29 16:26:37.000000 baboo_game-2.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-29 16:26:37.000000 baboo_game-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 16:26:37.000000 baboo_game-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:26:50.665062 baboo_game-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.661062 baboo_game-2.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.661062 baboo_game-2.0.1/src/baboo_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.665062 baboo_game-2.0.1/src/baboo_game/game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/baboo_game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.665062 baboo_game-2.0.1/src/baboo_game/game/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/config/color_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/config/game_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/config/text_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.665062 baboo_game-2.0.1/src/baboo_game/game/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/library/abstract_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/render_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.665062 baboo_game-2.0.1/src/baboo_game.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-29 16:26:50.000000 baboo_game-2.0.1/src/baboo_game.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-29 16:26:50.000000 baboo_game-2.0.1/src/baboo_game.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:26:50.000000 baboo_game-2.0.1/src/baboo_game.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 16:26:50.000000 baboo_game-2.0.1/src/baboo_game.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 16:26:50.000000 baboo_game-2.0.1/src/baboo_game.egg-info/top_level.txt
```

### Comparing `baboo_game-0.0.0/.github/workflows/python-publish.yml` & `baboo_game-2.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `baboo_game-0.0.0/.gitignore` & `baboo_game-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `baboo_game-0.0.0/LICENSE` & `baboo_game-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `baboo_game-0.0.0/PKG-INFO` & `baboo_game-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baboo_game
-Version: 0.0.0
+Version: 2.0.1
 Summary: A dice game prototype
 Author-email: Vitalii Sili <vitaliisili@yahoo.com>
 License: MIT License
         
         Copyright (c) 2023 Vitalii Sili
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `baboo_game-0.0.0/README.md` & `baboo_game-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `baboo_game-0.0.0/pyproject.toml` & `baboo_game-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm[toml]"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "baboo_game"
-dynamic = ["version"]
-#version = "2.0.2" # Insert manual version
+version = "2.0.1" # Insert manual version
 #dynamic = ["version", "dependencies"]
 authors = [
    { name="Vitalii Sili", email="vitaliisili@yahoo.com" },
 ]
 license = {file = "LICENSE"}
 description = "A dice game prototype"
 readme = "README.md"
```

### Comparing `baboo_game-0.0.0/src/baboo_game/game/baboo_game.py` & `baboo_game-2.0.1/src/baboo_game/game/baboo_game.py`

 * *Files identical despite different names*

### Comparing `baboo_game-0.0.0/src/baboo_game/game/config/text_constant.py` & `baboo_game-2.0.1/src/baboo_game/game/config/text_constant.py`

 * *Files identical despite different names*

### Comparing `baboo_game-0.0.0/src/baboo_game/game/library/abstract_dice.py` & `baboo_game-2.0.1/src/baboo_game/game/library/abstract_dice.py`

 * *Files identical despite different names*

### Comparing `baboo_game-0.0.0/src/baboo_game/game/render_game.py` & `baboo_game-2.0.1/src/baboo_game/game/render_game.py`

 * *Files identical despite different names*

### Comparing `baboo_game-0.0.0/src/baboo_game.egg-info/PKG-INFO` & `baboo_game-2.0.1/src/baboo_game.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baboo-game
-Version: 0.0.0
+Version: 2.0.1
 Summary: A dice game prototype
 Author-email: Vitalii Sili <vitaliisili@yahoo.com>
 License: MIT License
         
         Copyright (c) 2023 Vitalii Sili
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `baboo_game-0.0.0/src/baboo_game.egg-info/SOURCES.txt` & `baboo_game-2.0.1/src/baboo_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*


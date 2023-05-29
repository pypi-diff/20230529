# Comparing `tmp/baboo_game-2.0.5.tar.gz` & `tmp/baboo_game-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baboo_game-2.0.5.tar", last modified: Mon May 29 17:41:22 2023, max compression
+gzip compressed data, was "baboo_game-2.0.6.tar", last modified: Mon May 29 19:52:05 2023, max compression
```

## Comparing `baboo_game-2.0.5.tar` & `baboo_game-2.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 17:41:11.000000 baboo_game-2.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-29 17:41:22.518499 baboo_game-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-29 17:41:11.000000 baboo_game-2.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-29 17:41:11.000000 baboo_game-2.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:41:22.518499 baboo_game-2.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/baboo_game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/baboo_game/game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/baboo_game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/baboo_game/game/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/config/color_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/config/game_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/config/text_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/baboo_game/game/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/library/abstract_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/render_game.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/baboo_game.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-29 17:41:22.000000 baboo_game-2.0.5/src/baboo_game.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 17:41:22.000000 baboo_game-2.0.5/src/baboo_game.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:41:22.000000 baboo_game-2.0.5/src/baboo_game.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 17:41:22.000000 baboo_game-2.0.5/src/baboo_game.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 17:41:22.000000 baboo_game-2.0.5/src/baboo_game.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.922050 baboo_game-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 19:51:54.000000 baboo_game-2.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-29 19:52:05.922050 baboo_game-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-29 19:51:54.000000 baboo_game-2.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-29 19:51:54.000000 baboo_game-2.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:52:05.922050 baboo_game-2.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.918050 baboo_game-2.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.918050 baboo_game-2.0.6/src/baboo_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.922050 baboo_game-2.0.6/src/baboo_game/game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/baboo_game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.922050 baboo_game-2.0.6/src/baboo_game/game/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/config/color_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/config/game_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/config/text_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.922050 baboo_game-2.0.6/src/baboo_game/game/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/library/abstract_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/game/render_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 19:51:54.000000 baboo_game-2.0.6/src/baboo_game/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:52:05.922050 baboo_game-2.0.6/src/baboo_game.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4680 2023-05-29 19:52:05.000000 baboo_game-2.0.6/src/baboo_game.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 19:52:05.000000 baboo_game-2.0.6/src/baboo_game.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:52:05.000000 baboo_game-2.0.6/src/baboo_game.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 19:52:05.000000 baboo_game-2.0.6/src/baboo_game.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 19:52:05.000000 baboo_game-2.0.6/src/baboo_game.egg-info/top_level.txt
```

### Comparing `baboo_game-2.0.5/LICENSE` & `baboo_game-2.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.5/pyproject.toml` & `baboo_game-2.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "baboo_game"
-version = "2.0.5" # Insert manual version
+version = "2.0.6" # Insert manual version
 authors = [
    { name="Vitalii Sili", email="vitaliisili@yahoo.com" },
 ]
 license = {file = "LICENSE"}
 description = "A dice game prototype"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `baboo_game-2.0.5/src/baboo_game/game/baboo_game.py` & `baboo_game-2.0.6/src/baboo_game/game/baboo_game.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.5/src/baboo_game/game/config/text_constant.py` & `baboo_game-2.0.6/src/baboo_game/game/config/text_constant.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.5/src/baboo_game/game/library/abstract_dice.py` & `baboo_game-2.0.6/src/baboo_game/game/library/abstract_dice.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.5/src/baboo_game/game/render_game.py` & `baboo_game-2.0.6/src/baboo_game/game/render_game.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.5/src/baboo_game.egg-info/SOURCES.txt` & `baboo_game-2.0.6/src/baboo_game.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/baboo_game-2.0.1.tar.gz` & `tmp/baboo_game-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baboo_game-2.0.1.tar", last modified: Mon May 29 16:26:50 2023, max compression
+gzip compressed data, was "baboo_game-2.0.5.tar", last modified: Mon May 29 17:41:22 2023, max compression
```

## Comparing `baboo_game-2.0.1.tar` & `baboo_game-2.0.5.tar`

### file list

```diff
@@ -1,33 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.665062 baboo_game-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.661062 baboo_game-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.661062 baboo_game-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-29 16:26:37.000000 baboo_game-2.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-05-29 16:26:37.000000 baboo_game-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 16:26:37.000000 baboo_game-2.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-29 16:26:50.665062 baboo_game-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-29 16:26:37.000000 baboo_game-2.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-29 16:26:37.000000 baboo_game-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-29 16:26:37.000000 baboo_game-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 16:26:50.665062 baboo_game-2.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.661062 baboo_game-2.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.661062 baboo_game-2.0.1/src/baboo_game/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.665062 baboo_game-2.0.1/src/baboo_game/game/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/baboo_game.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.665062 baboo_game-2.0.1/src/baboo_game/game/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/config/color_config.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/config/game_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/config/text_constant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.665062 baboo_game-2.0.1/src/baboo_game/game/library/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/library/abstract_dice.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/game/render_game.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 16:26:37.000000 baboo_game-2.0.1/src/baboo_game/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:26:50.665062 baboo_game-2.0.1/src/baboo_game.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-29 16:26:50.000000 baboo_game-2.0.1/src/baboo_game.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-29 16:26:50.000000 baboo_game-2.0.1/src/baboo_game.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:26:50.000000 baboo_game-2.0.1/src/baboo_game.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 16:26:50.000000 baboo_game-2.0.1/src/baboo_game.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 16:26:50.000000 baboo_game-2.0.1/src/baboo_game.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-29 17:41:11.000000 baboo_game-2.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-29 17:41:22.518499 baboo_game-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-29 17:41:11.000000 baboo_game-2.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-29 17:41:11.000000 baboo_game-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 17:41:22.518499 baboo_game-2.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/baboo_game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/baboo_game/game/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/baboo_game.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/baboo_game/game/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/config/color_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/config/game_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/config/text_constant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/baboo_game/game/library/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/library/abstract_dice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/game/render_game.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-29 17:41:11.000000 baboo_game-2.0.5/src/baboo_game/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 17:41:22.518499 baboo_game-2.0.5/src/baboo_game.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2542 2023-05-29 17:41:22.000000 baboo_game-2.0.5/src/baboo_game.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-29 17:41:22.000000 baboo_game-2.0.5/src/baboo_game.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 17:41:22.000000 baboo_game-2.0.5/src/baboo_game.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 17:41:22.000000 baboo_game-2.0.5/src/baboo_game.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 17:41:22.000000 baboo_game-2.0.5/src/baboo_game.egg-info/top_level.txt
```

### Comparing `baboo_game-2.0.1/LICENSE` & `baboo_game-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.1/PKG-INFO` & `baboo_game-2.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baboo_game
-Version: 2.0.1
+Version: 2.0.5
 Summary: A dice game prototype
 Author-email: Vitalii Sili <vitaliisili@yahoo.com>
 License: MIT License
         
         Copyright (c) 2023 Vitalii Sili
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,24 +24,26 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/vitaliisili/dice_game_python
 Project-URL: documentation, https://github.com/vitaliisili/dice_game_python
 Project-URL: repository, https://github.com/vitaliisili/dice_game_python
+Keywords: dicegame,python,console game
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Baboo Dice Game
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 ![Release](https://img.shields.io/github/v/release/vitaliisili/dice_game_python)
+![PyPI version](https://img.shields.io/pypi/v/baboo-game)
 ![Watchers](https://img.shields.io/github/watchers/vitaliisili/dice_game_python?style=social)
-[![PyPI version](https://badge.fury.io/py/pypi.svg)](https://pypi.org/project/smart-nine/)
+
 
 ![baboo](https://lh3.googleusercontent.com/pw/AJFCJaWOlNjWnEZ6Lcp7Z8AE3YGCv1CaVTXDX-9VXJxfnNVw_Qljmyfhx-khr0Shs1wI2oESp3tbQ8dmKpcmOHViL-OoKLZE10lQ1qUbnz7cikdgstf7bFq7fds7V1WK7DTMOjJejmubcV0MMieJMfxASOtl=w577-h433-s-no)
```

### Comparing `baboo_game-2.0.1/README.md` & `baboo_game-2.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Baboo Dice Game
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 ![Release](https://img.shields.io/github/v/release/vitaliisili/dice_game_python)
+![PyPI version](https://img.shields.io/pypi/v/baboo-game)
 ![Watchers](https://img.shields.io/github/watchers/vitaliisili/dice_game_python?style=social)
-[![PyPI version](https://badge.fury.io/py/pypi.svg)](https://pypi.org/project/smart-nine/)
+
 
 ![baboo](https://lh3.googleusercontent.com/pw/AJFCJaWOlNjWnEZ6Lcp7Z8AE3YGCv1CaVTXDX-9VXJxfnNVw_Qljmyfhx-khr0Shs1wI2oESp3tbQ8dmKpcmOHViL-OoKLZE10lQ1qUbnz7cikdgstf7bFq7fds7V1WK7DTMOjJejmubcV0MMieJMfxASOtl=w577-h433-s-no)
```

### Comparing `baboo_game-2.0.1/src/baboo_game/game/baboo_game.py` & `baboo_game-2.0.5/src/baboo_game/game/baboo_game.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.1/src/baboo_game/game/config/text_constant.py` & `baboo_game-2.0.5/src/baboo_game/game/config/text_constant.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.1/src/baboo_game/game/library/abstract_dice.py` & `baboo_game-2.0.5/src/baboo_game/game/library/abstract_dice.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.1/src/baboo_game/game/render_game.py` & `baboo_game-2.0.5/src/baboo_game/game/render_game.py`

 * *Files identical despite different names*

### Comparing `baboo_game-2.0.1/src/baboo_game.egg-info/PKG-INFO` & `baboo_game-2.0.5/src/baboo_game.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baboo-game
-Version: 2.0.1
+Version: 2.0.5
 Summary: A dice game prototype
 Author-email: Vitalii Sili <vitaliisili@yahoo.com>
 License: MIT License
         
         Copyright (c) 2023 Vitalii Sili
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,24 +24,26 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: homepage, https://github.com/vitaliisili/dice_game_python
 Project-URL: documentation, https://github.com/vitaliisili/dice_game_python
 Project-URL: repository, https://github.com/vitaliisili/dice_game_python
+Keywords: dicegame,python,console game
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Baboo Dice Game
 
 [![made-with-python](https://img.shields.io/badge/Made%20with-Python-1f425f.svg)](https://www.python.org/)
 ![Release](https://img.shields.io/github/v/release/vitaliisili/dice_game_python)
+![PyPI version](https://img.shields.io/pypi/v/baboo-game)
 ![Watchers](https://img.shields.io/github/watchers/vitaliisili/dice_game_python?style=social)
-[![PyPI version](https://badge.fury.io/py/pypi.svg)](https://pypi.org/project/smart-nine/)
+
 
 ![baboo](https://lh3.googleusercontent.com/pw/AJFCJaWOlNjWnEZ6Lcp7Z8AE3YGCv1CaVTXDX-9VXJxfnNVw_Qljmyfhx-khr0Shs1wI2oESp3tbQ8dmKpcmOHViL-OoKLZE10lQ1qUbnz7cikdgstf7bFq7fds7V1WK7DTMOjJejmubcV0MMieJMfxASOtl=w577-h433-s-no)
```

### Comparing `baboo_game-2.0.1/src/baboo_game.egg-info/SOURCES.txt` & `baboo_game-2.0.5/src/baboo_game.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,10 @@
-.gitignore
 LICENSE
 README.md
 pyproject.toml
-requirements.txt
-.github/workflows/python-publish.yml
 src/baboo_game/__init__.py
 src/baboo_game/main.py
 src/baboo_game.egg-info/PKG-INFO
 src/baboo_game.egg-info/SOURCES.txt
 src/baboo_game.egg-info/dependency_links.txt
 src/baboo_game.egg-info/requires.txt
 src/baboo_game.egg-info/top_level.txt
```


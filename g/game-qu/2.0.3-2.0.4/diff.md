# Comparing `tmp/game_qu-2.0.3.tar.gz` & `tmp/game_qu-2.0.4.tar.gz`

## Comparing `game_qu-2.0.3.tar` & `game_qu-2.0.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 game_qu-2.0.3/LISCENCE
--rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 game_qu-2.0.3/.idea/workspace.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/__init__.py
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/game_runner.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/library_abstraction.py
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/colors.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/engines.py
--rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/events.py
--rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/file_reader.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/fraction.py
--rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/game_movement.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/game_runner_function.py
--rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/history_keeper.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/id_creator.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/important_constants.py
--rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/important_variables.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/keyboard.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/library_changer.py
--rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/library_independant_utility_functions.py
--rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/lines.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/paths.py
--rw-r--r--   0        0        0    13518 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/quadratic_equations.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/range.py
--rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/unique_ids_list.py
--rw-r--r--   0        0        0     9677 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/utility_functions.py
--rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/base/velocity_calculator.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/gui_components/component.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/gui_components/dimensions.py
--rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/gui_components/grid.py
--rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/gui_components/hud.py
--rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/gui_components/intermediate_screen.py
--rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/gui_components/navigation_screen.py
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/gui_components/screen.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/gui_components/text_box.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/gui_components/window.py
--rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/pygame_abstraction/keys.py
--rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/pygame_abstraction/utility_functions.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/pygame_abstraction/variables.py
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/pyglet_abstraction/keys.py
--rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/pyglet_abstraction/utility_functions.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 game_qu-2.0.3/src/game_qu/pyglet_abstraction/variables.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.3/README.md
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 game_qu-2.0.3/pyproject.toml
--rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 game_qu-2.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 game_qu-2.0.4/LISCENCE
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 game_qu-2.0.4/.idea/workspace.xml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/__init__.py
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/game_runner.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/library_abstraction.py
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/colors.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/engines.py
+-rw-r--r--   0        0        0     4496 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/events.py
+-rw-r--r--   0        0        0     4028 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/file_reader.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/fraction.py
+-rw-r--r--   0        0        0     4088 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/game_movement.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/game_runner_function.py
+-rw-r--r--   0        0        0     3768 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/history_keeper.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/id_creator.py
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/important_constants.py
+-rw-r--r--   0        0        0     2613 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/important_variables.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/keyboard.py
+-rw-r--r--   0        0        0     4753 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/library_changer.py
+-rw-r--r--   0        0        0     2692 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/library_independant_utility_functions.py
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/lines.py
+-rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/paths.py
+-rw-r--r--   0        0        0    13518 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/quadratic_equations.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/range.py
+-rw-r--r--   0        0        0     6001 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/unique_ids_list.py
+-rw-r--r--   0        0        0     9939 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/utility_functions.py
+-rw-r--r--   0        0        0      976 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/base/velocity_calculator.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/gui_components/component.py
+-rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/gui_components/dimensions.py
+-rw-r--r--   0        0        0     6595 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/gui_components/grid.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/gui_components/hud.py
+-rw-r--r--   0        0        0     4074 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/gui_components/intermediate_screen.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/gui_components/navigation_screen.py
+-rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/gui_components/screen.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/gui_components/text_box.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/gui_components/window.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/pygame_abstraction/keys.py
+-rw-r--r--   0        0        0     6126 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/pygame_abstraction/utility_functions.py
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/pygame_abstraction/variables.py
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/pyglet_abstraction/keys.py
+-rw-r--r--   0        0        0     6825 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/pyglet_abstraction/utility_functions.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 game_qu-2.0.4/src/game_qu/pyglet_abstraction/variables.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 game_qu-2.0.4/README.md
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 game_qu-2.0.4/pyproject.toml
+-rw-r--r--   0        0        0      341 2020-02-02 00:00:00.000000 game_qu-2.0.4/PKG-INFO
```

### Comparing `game_qu-2.0.3/LISCENCE` & `game_qu-2.0.4/LISCENCE`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/.idea/workspace.xml` & `game_qu-2.0.4/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/colors.py` & `game_qu-2.0.4/src/game_qu/base/colors.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/engines.py` & `game_qu-2.0.4/src/game_qu/base/engines.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/events.py` & `game_qu-2.0.4/src/game_qu/base/events.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/file_reader.py` & `game_qu-2.0.4/src/game_qu/base/file_reader.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/fraction.py` & `game_qu-2.0.4/src/game_qu/base/fraction.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/game_movement.py` & `game_qu-2.0.4/src/game_qu/base/game_movement.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/game_runner_function.py` & `game_qu-2.0.4/src/game_qu/base/game_runner_function.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/history_keeper.py` & `game_qu-2.0.4/src/game_qu/base/history_keeper.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/id_creator.py` & `game_qu-2.0.4/src/game_qu/base/id_creator.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/important_variables.py` & `game_qu-2.0.4/src/game_qu/base/important_variables.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/keyboard.py` & `game_qu-2.0.4/src/game_qu/base/keyboard.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/library_changer.py` & `game_qu-2.0.4/src/game_qu/base/library_changer.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 class LibraryChanger:
     """ A class that allows the user to modify constants and other variables instead of actually modifying the code.
         IMPORTANT: All the methods of this class must be called from the second line onwards with the first line being
         from game_qu.base.library_changer import LibraryChanger, so none of the other code is initialized with the old constants."""
 
     library_has_been_set = False
     current_library_name = ""
+    overrided_functions = {}
 
     @staticmethod
     def set_screen_dimensions(screen_length, screen_height):
             """Sets the dimensions of the screen. IMPORTANT see class description for details on how to call the methods """
 
             important_constants.SCREEN_LENGTH = screen_length
             important_constants.SCREEN_HEIGHT = screen_height
@@ -77,7 +78,25 @@
         """Makes the size of the application full screen. NOTE: This only works with pygame"""
 
         if LibraryChanger.current_library_name == "pygame":
             important_constants.IS_FULL_SCREEN = is_full_screen
 
         else:
             raise ValueError("Setting to full screen can only be done when the game engine is pygame")
+
+    @staticmethod
+    def set_function(function_name, function):
+        """ Sets the normal function to the new function provided. For instance, this could override the default rendering
+            style. This is generally not recommended unless you know what you are doing"""
+
+        LibraryChanger.overrided_functions[function_name] = function
+
+    @staticmethod
+    def get_function(module, function_name):
+        """ :returns: function; the normal function if the function was not overrided otherwise the overrided function"""
+
+        return_value = getattr(module, function_name)
+
+        if LibraryChanger.overrided_functions.__contains__(function_name):
+            return_value = LibraryChanger.get(function_name)
+
+        return return_value
```

### Comparing `game_qu-2.0.3/src/game_qu/base/library_independant_utility_functions.py` & `game_qu-2.0.4/src/game_qu/base/library_independant_utility_functions.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/lines.py` & `game_qu-2.0.4/src/game_qu/base/lines.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/paths.py` & `game_qu-2.0.4/src/game_qu/base/paths.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/quadratic_equations.py` & `game_qu-2.0.4/src/game_qu/base/quadratic_equations.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/range.py` & `game_qu-2.0.4/src/game_qu/base/range.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/unique_ids_list.py` & `game_qu-2.0.4/src/game_qu/base/unique_ids_list.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/base/utility_functions.py` & `game_qu-2.0.4/src/game_qu/base/utility_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,28 +7,29 @@
 from game_qu.base.fraction import Fraction
 from game_qu.base.important_variables import keyboard, SCREEN_LENGTH, SCREEN_HEIGHT, IS_USING_CONTROLLER
 import random
 
 from game_qu.library_abstraction import utility_functions
 from game_qu.base.range import Range
 
+
 # Retrieving the functions from the game library code
-load_image = getattr(utility_functions, "load_image")
-load_text = getattr(utility_functions, "load_text")
-render_text = getattr(utility_functions, "render_text")
-render_image = getattr(utility_functions, "render_image")
-render_rectangle = getattr(utility_functions, "render_rectangle")
-set_up_window = getattr(utility_functions, "set_up_window")
-key_is_pressed = getattr(utility_functions, "key_is_pressed")
-mouse_was_pressed = getattr(utility_functions, "mouse_was_pressed")
-call_every_cycle = getattr(utility_functions, "call_every_cycle")
-is_mouse_collision = getattr(utility_functions, "is_mouse_collision")
-get_time_passed = getattr(utility_functions, "get_time_passed")
-load_and_transform_image = getattr(utility_functions, "load_and_transform_image")
-get_directional_path_to_image = getattr(utility_functions, "get_directional_path_to_image")
+load_image = LibraryChanger.get_function(utility_functions, "load_image")
+load_text = LibraryChanger.get_function(utility_functions, "load_text")
+render_text = LibraryChanger.get_function(utility_functions, "render_text")
+render_image = LibraryChanger.get_function(utility_functions, "render_image")
+render_rectangle = LibraryChanger.get_function(utility_functions, "render_rectangle")
+set_up_window = LibraryChanger.get_function(utility_functions, "set_up_window")
+key_is_pressed = LibraryChanger.get_function(utility_functions, "key_is_pressed")
+mouse_was_pressed = LibraryChanger.get_function(utility_functions, "mouse_was_pressed")
+call_every_cycle = LibraryChanger.get_function(utility_functions, "call_every_cycle")
+is_mouse_collision = LibraryChanger.get_function(utility_functions, "is_mouse_collision")
+get_time_passed = LibraryChanger.get_function(utility_functions, "get_time_passed")
+load_and_transform_image = LibraryChanger.get_function(utility_functions, "load_and_transform_image")
+get_directional_path_to_image = LibraryChanger.get_function(utility_functions, "get_directional_path_to_image")
 
 def key_is_pressed(key):
     """:returns: bool; whether that key is currently held down (pressed)"""
 
     return keyboard.get_key_event(key).happened_this_cycle
```

### Comparing `game_qu-2.0.3/src/game_qu/base/velocity_calculator.py` & `game_qu-2.0.4/src/game_qu/base/velocity_calculator.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/gui_components/component.py` & `game_qu-2.0.4/src/game_qu/gui_components/component.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/gui_components/dimensions.py` & `game_qu-2.0.4/src/game_qu/gui_components/dimensions.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/gui_components/grid.py` & `game_qu-2.0.4/src/game_qu/gui_components/grid.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/gui_components/hud.py` & `game_qu-2.0.4/src/game_qu/gui_components/hud.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/gui_components/intermediate_screen.py` & `game_qu-2.0.4/src/game_qu/gui_components/intermediate_screen.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/gui_components/navigation_screen.py` & `game_qu-2.0.4/src/game_qu/gui_components/navigation_screen.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/gui_components/screen.py` & `game_qu-2.0.4/src/game_qu/gui_components/screen.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/gui_components/text_box.py` & `game_qu-2.0.4/src/game_qu/gui_components/text_box.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/gui_components/window.py` & `game_qu-2.0.4/src/game_qu/gui_components/window.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/pygame_abstraction/keys.py` & `game_qu-2.0.4/src/game_qu/pygame_abstraction/keys.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/pygame_abstraction/utility_functions.py` & `game_qu-2.0.4/src/game_qu/pygame_abstraction/utility_functions.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/pyglet_abstraction/keys.py` & `game_qu-2.0.4/src/game_qu/pyglet_abstraction/keys.py`

 * *Files identical despite different names*

### Comparing `game_qu-2.0.3/src/game_qu/pyglet_abstraction/utility_functions.py` & `game_qu-2.0.4/src/game_qu/pyglet_abstraction/utility_functions.py`

 * *Files identical despite different names*


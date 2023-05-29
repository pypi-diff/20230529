# Comparing `tmp/svgecko-0.3.0.tar.gz` & `tmp/svgecko-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svgecko-0.3.0.tar", last modified: Tue May 23 10:31:58 2023, max compression
+gzip compressed data, was "svgecko-0.3.1.tar", last modified: Mon May 29 09:12:58 2023, max compression
```

## Comparing `svgecko-0.3.0.tar` & `svgecko-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:31:58.091433 svgecko-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 10:31:58.091433 svgecko-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-23 10:31:42.000000 svgecko-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 10:31:58.091433 svgecko-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-23 10:31:42.000000 svgecko-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:31:58.091433 svgecko-0.3.0/svgecko/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:31:42.000000 svgecko-0.3.0/svgecko/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:31:58.091433 svgecko-0.3.0/svgecko/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-05-23 10:31:42.000000 svgecko-0.3.0/svgecko/resources/python-logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-05-23 10:31:42.000000 svgecko-0.3.0/svgecko/svg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-05-23 10:31:42.000000 svgecko-0.3.0/svgecko/svg_path.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-23 10:31:42.000000 svgecko-0.3.0/svgecko/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:31:58.091433 svgecko-0.3.0/svgecko.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-23 10:31:58.000000 svgecko-0.3.0/svgecko.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-23 10:31:58.000000 svgecko-0.3.0/svgecko.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 10:31:58.000000 svgecko-0.3.0/svgecko.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-23 10:31:58.000000 svgecko-0.3.0/svgecko.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-23 10:31:58.000000 svgecko-0.3.0/svgecko.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 10:31:58.091433 svgecko-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-23 10:31:42.000000 svgecko-0.3.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-23 10:31:42.000000 svgecko-0.3.0/tests/test_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:58.432427 svgecko-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-29 09:12:58.432427 svgecko-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-29 09:12:44.000000 svgecko-0.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:12:58.436427 svgecko-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 09:12:44.000000 svgecko-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:58.432427 svgecko-0.3.1/svgecko/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:58.432427 svgecko-0.3.1/svgecko/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/resources/cross.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     9237 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/resources/python-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/svg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/svg_path.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-29 09:12:44.000000 svgecko-0.3.1/svgecko/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:58.432427 svgecko-0.3.1/svgecko.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-29 09:12:58.000000 svgecko-0.3.1/svgecko.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-29 09:12:58.000000 svgecko-0.3.1/svgecko.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:12:58.000000 svgecko-0.3.1/svgecko.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-29 09:12:58.000000 svgecko-0.3.1/svgecko.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 09:12:58.000000 svgecko-0.3.1/svgecko.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:58.432427 svgecko-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 09:12:44.000000 svgecko-0.3.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-29 09:12:44.000000 svgecko-0.3.1/tests/test_svg.py
```

### Comparing `svgecko-0.3.0/setup.py` & `svgecko-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='svgecko',
-    version='0.3.0',
+    version='0.3.1',
     author='Josef Ondrej',
     author_email='josef.ondrej@outlook.com',
     description='Lightweight library for arbitrary geometric SVG transformations',
     long_description='Lightweight library for arbitrary geometric SVG transformations',
     long_description_content_type='text/markdown',
     packages=find_packages(),
     package_data={'svgecko': ['resources/*.svg']},
```

### Comparing `svgecko-0.3.0/svgecko/resources/python-logo.svg` & `svgecko-0.3.1/svgecko/resources/python-logo.svg`

 * *Files identical despite different names*

### Comparing `svgecko-0.3.0/svgecko/svg.py` & `svgecko-0.3.1/svgecko/svg.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,22 +31,42 @@
         :param svg_string: SVG string in XML format
         :param encoding: encoding of the SVG string
         :return: SVG object
         """
         svg_tree = etree.fromstring(bytes(svg_string, encoding=encoding))
         return SVG(svg_tree)
 
+    @classmethod
+    def from_file(cls, file_path: str, encoding: str = 'utf-8') -> SVG:
+        """
+        Parses an SVG file and returns an SVG object.
+        :param file_path: path to SVG file
+        :return: SVG object
+        """
+        with open(file_path, 'r', encoding=encoding) as file:
+            svg_string = file.read()
+        return SVG.from_string(svg_string, encoding=encoding)
+
     def to_string(self, encoding: str = 'utf-8') -> str:
         """
         Returns the SVG object as a string in XML format.
         :param encoding: encoding of the SVG string
         :return: SVG string in XML format
         """
         return etree.tostring(self._xml, encoding=encoding).decode(encoding=encoding)
 
+    def to_file(self, file_path: str, encoding: str = 'utf-8') -> None:
+        """
+        Writes the SVG object to a file.
+        :param file_path: path to SVG file
+        :param encoding: encoding of the SVG string
+        """
+        with open(file_path, 'w', encoding=encoding) as file:
+            file.write(self.to_string(encoding=encoding))
+
     def __copy__(self):
         return SVG(self._xml)
 
     def __deepcopy__(self, memodict={}):
         return SVG(deepcopy(self._xml))
 
     @property
@@ -72,15 +92,15 @@
         self._transform_paths(svg, transformation)
         self._transform_xy_attributes(svg, transformation)
 
         return svg
 
     @staticmethod
     def _transform_xy_attributes(svg: SVG, transformation: Callable[[Tuple[float, float]], Tuple[float, float]]):
-        for attribute_pairs in [('x', 'y'), ('x1', 'y1'), ('x2', 'y2')]:
+        for attribute_pairs in [('x', 'y'), ('x1', 'y1'), ('x2', 'y2'), ('cx', 'cy')]:
             elements_with_both_attributes_selector = f'//*[@{attribute_pairs[0]} and @{attribute_pairs[1]}]'
             elements_with_both_attributes = svg.xml.xpath(elements_with_both_attributes_selector)
             for element in elements_with_both_attributes:
                 x_name, y_name = attribute_pairs
                 x, y = float(element.attrib[x_name]), float(element.attrib[y_name])
                 transformed_x, transformed_y = transformation((x, y))
                 element.attrib[x_name], element.attrib[y_name] = str(transformed_x), str(transformed_y)
```

### Comparing `svgecko-0.3.0/svgecko/svg_path.py` & `svgecko-0.3.1/svgecko/svg_path.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,56 +1,109 @@
-from typing import Callable, Tuple, List, Optional
+from __future__ import annotations
+
+import re
+from typing import Callable, Tuple, List, Optional, Any
 
 COMMAND_TYPES = 'MmLlCcSsQqTtAaZzHhVv'
 
 
+class Path:
+    def __init__(self, commands: List[PathCommand]):
+        self._commands = commands
+
+    @classmethod
+    def from_command_string(cls, command_string: str) -> Path:
+        commands = parse_commands(command_string)
+        return Path(commands=commands)
+
+    @property
+    def command_string(self):
+        return ''.join([str(command) for command in self._commands])
+
+    def transform(self, transformation: Callable[[Tuple[float, float]], Tuple[float, float]]) -> Path:
+        path_start_coordinates = None  # Coordinates of the start of the path in the untransformed coordinate system
+        current_coordinates = (0, 0)  # Current coordinates in the untransformed coordinate system
+        transformed_commands = list()
+
+        for command in self._commands:
+            if command.type in ['M', 'L', 'C', 'S', 'Q', 'T']:
+                transformed_coordinates = flatten([
+                    transformation((command.coordinates[i], command.coordinates[i + 1])) for i in
+                    range(0, len(command.coordinates), 2)])
+                transformed_command = PathCommand(command.type, transformed_coordinates)
+                current_coordinates = tuple(command.coordinates[-2:])
+            elif command.type in ['H']:
+                transformed_coordinates = flatten(
+                    [transformation((x, current_coordinates[1])) for x in command.coordinates])
+                transformed_command = PathCommand('L', transformed_coordinates)
+                current_coordinates = (command.coordinates[-1], current_coordinates[1])
+            elif command.type in ['V']:
+                transformed_coordinates = flatten(
+                    [transformation((current_coordinates[0], y)) for y in command.coordinates])
+                transformed_command = PathCommand('L', transformed_coordinates)
+                current_coordinates = (current_coordinates[0], command.coordinates[-1])
+            elif command.type in ['A', 'a']:
+                raise NotImplementedError('Arcs are not implemented yet')
+            elif command.type in ['m', 'l', 'c', 's', 'q', 't']:
+                raise NotImplementedError('Relative commands are not implemented yet')
+            elif command.type in ['Z', 'z']:
+                transformed_command = PathCommand('Z')
+                current_coordinates = path_start_coordinates
+                path_start_coordinates = None
+
+            if path_start_coordinates is None:
+                path_start_coordinates = current_coordinates
+
+            transformed_commands.append(transformed_command)
+
+        return Path(transformed_commands)
+
+
 class PathCommand:
     def __init__(self, command_type: str, coordinates: Optional[List[float]] = None):
         if command_type not in COMMAND_TYPES and len(command_type) != 1:
             raise ValueError(f'Invalid command type: {command_type}')
 
         self._command_type = command_type
         self._coordinates = coordinates if coordinates is not None else list()
 
-    def transform(self, transformation: Callable[[Tuple[int, int]], Tuple[int, int]]):
-        if self._command_type in ['M', 'L', 'C', 'S', 'Q', 'T']:
-            transformed_coordinates = [
-                transformation((self._coordinates[i], self._coordinates[i + 1])) for i in
-                range(0, len(self._coordinates), 2)]
-            self._coordinates = [coordinate for point in transformed_coordinates for coordinate in point]
-        elif self._command_type in ['H']:
-            self._coordinates = [
-                transformation((self._coordinates[i], 0)
-                               )[0] for i in range(len(self._coordinates))]
-        elif self._command_type in ['V']:
-            self._coordinates = [
-                transformation((0, self._coordinates[i]))[1] for i in range(len(self._coordinates))]
-        elif self._command_type in ['A', 'a']:
-            raise NotImplementedError('Arcs are not implemented yet')
-        elif self._command_type in ['m', 'l', 'c', 's', 'q', 't', 'h', 'v']:
-            raise NotImplementedError('Relative commands are not implemented yet')
-        elif self._command_type in ['Z', 'z']:
-            pass
+    @property
+    def type(self) -> str:
+        return self._command_type
+
+    @property
+    def coordinates(self) -> Tuple[float, float]:
+        return self._coordinates
 
     def __str__(self):
         return self._command_type + ' '.join([str(coordinate) for coordinate in self._coordinates])
 
     def __repr__(self):
         return f'PathCommand({self._command_type}, {self._coordinates})'
 
 
+def flatten(nested_list: List[Tuple[Any]]) -> List[Any]:
+    """
+    Flattens a nested list of tuples into a list of elements.
+    :param nested_list: Nested list of tuples
+    :return: List of elements
+    """
+    return [element for nested_tuple in nested_list for element in nested_tuple]
+
+
 def parse_coordinates(coordinates: str) -> List[float]:
     """
     Parses a string of coordinates into a list of floats.
     :param coordinates: String of coordinates
     :return: List of floats
     """
     if coordinates.strip() == '':
         return list()
-    return [float(coordinate.strip()) for coordinate in coordinates.strip().split(' ')]
+
+    return [float(coordinate.strip()) for coordinate in re.split(r'[, ]+', coordinates.strip())]
 
 
 def parse_commands(path_command_string: str) -> List[PathCommand]:
     """
     Parses a path command string into a list of PathCommands.
     :param path_command_string: Raw SVG path command string
     :return: List of PathCommands
@@ -76,11 +129,10 @@
                                   transformation: Callable[[Tuple[float, float]], Tuple[float, float]]) -> str:
     """
     Transforms a path command string by applying a transformation to every point.
     :param path_command_string: SVG path command string
     :param transformation: Transformation that maps points from R2 to R2
     :return: Transformed path command string
     """
-    commands = parse_commands(path_command_string)
-    for command in commands:
-        command.transform(transformation)
-    return ''.join([str(command) for command in commands])
+    path = Path.from_command_string(path_command_string)
+    transformed_path = path.transform(transformation)
+    return transformed_path.command_string
```

### Comparing `svgecko-0.3.0/tests/test_svg.py` & `svgecko-0.3.1/tests/test_svg.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,19 @@
+import os
+import re
+
 import numpy as np
 import pytest
 
 from svgecko.svg import SVG
-from svgecko.utils import load_python_logo
+from svgecko.utils import load_python_logo, CROSS_PATH
+
+
+def _replace_whitespaces_with_space(string: str) -> str:
+    return re.sub(r'\s+', ' ', string)
 
 
 @pytest.fixture
 def python_logo() -> SVG:
     return load_python_logo()
 
 
@@ -75,7 +82,27 @@
     assert transformed_array == expected_transformed_array
 
 
 def test_shape(python_logo: SVG):
     width, height = python_logo.shape
     assert abs(width - 92.070236) < 1e-6
     assert abs(height - 101.00108) < 1e-6
+
+
+def test_from_file():
+    svg = SVG.from_file(CROSS_PATH)
+    svg_string = svg.to_string()
+    expected_svg_string = """<svg xmlns="http://www.w3.org/2000/svg" class="icon  icon--plus" width="5" height="5" viewBox="0 0 5 5"> <path d="M2 1 H3 V2 H4 V3 H3 V4 H2 V3 H1 V2 H2 Z"/> </svg>"""
+    assert _replace_whitespaces_with_space(svg_string) == _replace_whitespaces_with_space(expected_svg_string)
+
+
+@pytest.fixture
+def temp_svg_file_path() -> str:
+    yield 'temp.svg'
+    os.remove('temp.svg')
+
+
+def test_to_file(temp_svg_file_path):
+    svg = SVG.from_file(CROSS_PATH)
+    svg.to_file(temp_svg_file_path)
+    svg_retrieved = SVG.from_file(temp_svg_file_path)
+    assert svg_retrieved.to_string() == svg.to_string()
```


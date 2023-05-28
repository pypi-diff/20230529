# Comparing `tmp/vision6D-0.1.1.tar.gz` & `tmp/vision6D-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.1.1.tar", last modified: Sun May 28 21:44:45 2023, max compression
+gzip compressed data, was "dist\vision6D-0.1.2.tar", last modified: Sun May 28 23:49:00 2023, max compression
```

## Comparing `vision6D-0.1.1.tar` & `vision6D-0.1.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 21:44:45.160272 vision6D-0.1.1/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.1/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1603 2023-05-28 21:44:45.161273 vision6D-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-28 01:21:42.000000 vision6D-0.1.1/README.md
--rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2023-05-28 21:44:45.168279 vision6D-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-05-28 01:21:42.000000 vision6D-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:44:44.897270 vision6D-0.1.1/test/
--rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.1/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.1/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:44:45.034308 vision6D-0.1.1/vision6D/
--rw-rw-rw-   0        0        0    50430 2023-05-28 21:28:42.000000 vision6D-0.1.1/vision6D/GUI.py
--rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.1/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.1/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.1/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:44:45.156274 vision6D-0.1.1/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.1/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.1/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.1/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.1/vision6D/interface.py
--rw-rw-rw-   0        0        0    26131 2023-05-28 21:42:04.000000 vision6D-0.1.1/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.1/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.1/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.1/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.1/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-28 21:44:45.106272 vision6D-0.1.1/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-05-28 21:44:44.000000 vision6D-0.1.1/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-28 21:44:44.000000 vision6D-0.1.1/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 21:44:44.000000 vision6D-0.1.1/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-28 21:44:44.000000 vision6D-0.1.1/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-28 21:44:44.000000 vision6D-0.1.1/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 23:49:00.574271 vision6D-0.1.2/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1603 2023-05-28 23:49:00.575271 vision6D-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-28 01:21:42.000000 vision6D-0.1.2/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2023-05-28 23:49:00.578273 vision6D-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-05-28 01:21:42.000000 vision6D-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:49:00.494270 vision6D-0.1.2/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.2/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.2/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:49:00.521273 vision6D-0.1.2/vision6D/
+-rw-rw-rw-   0        0        0    50486 2023-05-28 23:47:25.000000 vision6D-0.1.2/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.2/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.2/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.2/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:49:00.572271 vision6D-0.1.2/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.2/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.2/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.2/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.2/vision6D/interface.py
+-rw-rw-rw-   0        0        0    26131 2023-05-28 21:42:04.000000 vision6D-0.1.2/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.2/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.2/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.2/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.2/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:49:00.560271 vision6D-0.1.2/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-05-28 23:49:00.000000 vision6D-0.1.2/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-28 23:49:00.000000 vision6D-0.1.2/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:49:00.000000 vision6D-0.1.2/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-28 23:49:00.000000 vision6D-0.1.2/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-28 23:49:00.000000 vision6D-0.1.2/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.1.1/LICENSE` & `vision6D-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/PKG-INFO` & `vision6D-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.1
+Version: 0.1.2
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.1.1/README.md` & `vision6D-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/setup.cfg` & `vision6D-0.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e31 0d0a 7572  sion = 0.1.1..ur
+00000020: 7369 6f6e 203d 2030 2e31 2e32 0d0a 7572  sion = 0.1.2..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.1.1/test/test_create_dataset.py` & `vision6D-0.1.2/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/test/test_projection.py` & `vision6D-0.1.2/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/GUI.py` & `vision6D-0.1.2/vision6D/GUI.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # General import
-import os
-import logging
 import numpy as np
 import pyvista as pv
 import functools
 import trimesh
 import pathlib
 import PIL
 import ast
@@ -136,14 +134,16 @@
 
     def get_text(self):
         return self.user_text
 
 class MyMainWindow(MainWindow):
     def __init__(self, parent=None):
         QtWidgets.QMainWindow.__init__(self, parent)
+        # Fix the QMainWindow size to the desktop resolution
+        self.setGeometry(QtWidgets.QApplication.desktop().screenGeometry())
 
         # Set up the main window layout
         self.setWindowTitle("Vision6D")
         self.window_size = (1920, 1080)
         self.main_widget = QtWidgets.QWidget()
         self.setCentralWidget(self.main_widget)
         self.setAcceptDrops(True)
@@ -1002,15 +1002,15 @@
         self.panel_layout.addWidget(self.output)
 
     #^ Show plot
     def create_plotter(self):
         self.frame = QtWidgets.QFrame()
         self.frame.setFixedSize(*self.window_size)
         self.plotter = QtInteractor(self.frame)
-        # self.plotter.setFixedSize(*self.window_size) # but camera locate in the center instead of top left
+        # self.plotter.setFixedSize(*self.window_size)
         self.render = pv.Plotter(window_size=[self.window_size[0], self.window_size[1]], lighting=None, off_screen=True) 
         self.render.set_background('black'); 
         assert self.render.background_color == "black", "render's background need to be black"
         self.signal_close.connect(self.plotter.close)
 
     def show_plot(self):
         self.plotter.enable_joystick_actor_style()
@@ -1032,8 +1032,8 @@
         self.plotter.add_camera_orientation_widget()
 
         self.plotter.show()
         self.show()
 
     def showMaximized(self):
         super(MyMainWindow, self).showMaximized()
-        self.splitter.setSizes([int(self.width() * 0.05), int(self.width() * 0.95)])
+        self.splitter.setSizes([int(self.width() * 0.2), int(self.width() * 0.8)])
```

### Comparing `vision6D-0.1.1/vision6D/__init__.py` & `vision6D-0.1.2/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/app.py` & `vision6D-0.1.2/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/config.py` & `vision6D-0.1.2/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.1.2/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.1.2/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/data/style.qss` & `vision6D-0.1.2/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/interface.py` & `vision6D-0.1.2/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/interface_gui.py` & `vision6D-0.1.2/vision6D/interface_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/mainwindow.py` & `vision6D-0.1.2/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/run_gui.py` & `vision6D-0.1.2/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D/utils.py` & `vision6D-0.1.2/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.1/vision6D.egg-info/PKG-INFO` & `vision6D-0.1.2/vision6D.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.1
+Version: 0.1.2
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.1.1/vision6D.egg-info/SOURCES.txt` & `vision6D-0.1.2/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*


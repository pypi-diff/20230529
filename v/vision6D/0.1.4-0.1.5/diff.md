# Comparing `tmp/vision6D-0.1.4.tar.gz` & `tmp/vision6D-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.1.4.tar", last modified: Mon May 29 16:28:21 2023, max compression
+gzip compressed data, was "dist\vision6D-0.1.5.tar", last modified: Mon May 29 20:36:08 2023, max compression
```

## Comparing `vision6D-0.1.4.tar` & `vision6D-0.1.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 16:28:21.529007 vision6D-0.1.4/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     1603 2023-05-29 16:28:21.529007 vision6D-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-28 01:21:42.000000 vision6D-0.1.4/README.md
--rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2023-05-29 16:28:21.535007 vision6D-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-05-28 01:21:42.000000 vision6D-0.1.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 16:28:21.299204 vision6D-0.1.4/test/
--rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.4/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.4/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-29 16:28:21.393353 vision6D-0.1.4/vision6D/
--rw-rw-rw-   0        0        0    51799 2023-05-29 16:18:26.000000 vision6D-0.1.4/vision6D/GUI.py
--rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.4/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.4/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.4/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-29 16:28:21.521537 vision6D-0.1.4/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.4/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.4/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.4/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.4/vision6D/interface.py
--rw-rw-rw-   0        0        0    26131 2023-05-28 21:42:04.000000 vision6D-0.1.4/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.4/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.4/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.4/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.4/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 16:28:21.472067 vision6D-0.1.4/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-05-29 16:28:20.000000 vision6D-0.1.4/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-29 16:28:21.000000 vision6D-0.1.4/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 16:28:21.000000 vision6D-0.1.4/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-29 16:28:21.000000 vision6D-0.1.4/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 16:28:21.000000 vision6D-0.1.4/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 20:36:07.946940 vision6D-0.1.5/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     1603 2023-05-29 20:36:07.947940 vision6D-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-28 01:21:42.000000 vision6D-0.1.5/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2023-05-29 20:36:07.953939 vision6D-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-05-28 01:21:42.000000 vision6D-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 20:36:07.711492 vision6D-0.1.5/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.5/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.5/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-29 20:36:07.824497 vision6D-0.1.5/vision6D/
+-rw-rw-rw-   0        0        0    51583 2023-05-29 20:31:40.000000 vision6D-0.1.5/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.5/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.5/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.5/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-29 20:36:07.943939 vision6D-0.1.5/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.5/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.5/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.5/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.5/vision6D/interface.py
+-rw-rw-rw-   0        0        0    26129 2023-05-29 20:26:33.000000 vision6D-0.1.5/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.5/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.5/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.5/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.5/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 20:36:07.897480 vision6D-0.1.5/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-05-29 20:36:07.000000 vision6D-0.1.5/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-29 20:36:07.000000 vision6D-0.1.5/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 20:36:07.000000 vision6D-0.1.5/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-29 20:36:07.000000 vision6D-0.1.5/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 20:36:07.000000 vision6D-0.1.5/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.1.4/LICENSE` & `vision6D-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/PKG-INFO` & `vision6D-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.4
+Version: 0.1.5
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.1.4/README.md` & `vision6D-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/setup.cfg` & `vision6D-0.1.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e34 0d0a 7572  sion = 0.1.4..ur
+00000020: 7369 6f6e 203d 2030 2e31 2e35 0d0a 7572  sion = 0.1.5..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.1.4/test/test_create_dataset.py` & `vision6D-0.1.5/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/test/test_projection.py` & `vision6D-0.1.5/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D/GUI.py` & `vision6D-0.1.5/vision6D/GUI.py`

 * *Files 2% similar despite different names*

```diff
@@ -214,14 +214,15 @@
         # Set menu bar
         self.set_menu_bars()
 
         # Create the plotter
         self.create_plotter()
         
         # Set the camera
+        self.camera = pv.Camera()
         self.fx = 50000
         self.fy = 50000
         self.cx = 960
         self.cy = 540
         self.cam_viewup = (0, -1, 0)
         self.cam_position = -500
         self.set_camera_props()
@@ -366,16 +367,14 @@
         self.camera.SetWindowCenter(wcx, wcy) # (0,0)
         
         # Setting the view angle in degrees
         view_angle = (180 / math.pi) * (2.0 * math.atan2(self.window_size[1]/2.0, self.fx)) # or view_angle = np.degrees(2.0 * math.atan2(height/2.0, f)) # focal_length = (1080 / 2.0) / math.tan(math.radians(self.plotter.camera.view_angle / 2))
         self.camera.SetViewAngle(view_angle) # view angle should be in degrees
  
     def set_camera_props(self):
-        # Set up the camera
-        self.camera = pv.Camera()
         self.set_camera_intrinsics()
         self.set_camera_extrinsics()
         self.plotter.camera = self.camera.copy()
 
     def camera_calibrate(self):
         if self.image_path != '' and self.image_path is not None:
             original_image = np.array(PIL.Image.open(self.image_path), dtype='uint8')
@@ -468,17 +467,17 @@
             self.pose_path = workspace['pose_path']
             mesh_paths = workspace['mesh_path']
 
             self.add_image_file(prompt=False)
             self.add_mask_file(prompt=False)
             self.add_pose_file()
 
-            for item in mesh_paths.items():
-                mesh_name, self.mesh_path = item
-                self.add_mesh_file(mesh_name=mesh_name, prompt=False)
+            for mesh_path in mesh_paths:
+                self.mesh_path = mesh_path
+                self.add_mesh_file(prompt=False)
 
     def add_image_file(self, prompt=True):
         if prompt:
             if self.image_path == None or self.image_path == '':
                 self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg)")
             else:
                 self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.image_path).parent), "Files (*.png *.jpg)")
@@ -498,27 +497,24 @@
         
         if self.mask_path != '' and self.mask_path is not None:
             self.hintLabel.hide()
             mask_source = np.array(PIL.Image.open(self.mask_path), dtype='uint8')
             if len(mask_source.shape) == 2: mask_source = mask_source[..., None]
             self.add_mask(mask_source)
 
-    def add_mesh_file(self, mesh_name=None, prompt=True):
+    def add_mesh_file(self, prompt=True):
         if prompt:
             if self.mesh_path == None or self.mesh_path == '':
                 self.mesh_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.mesh *.ply *.stl *.obj *.off *.dae *.fbx *.3ds *.x3d)")
             else:
                 self.mesh_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.mesh_path).parent), "Files (*.mesh *.ply)")
         
         if self.mesh_path != '' and self.mesh_path is not None:
             self.hintLabel.hide()
-            if mesh_name is None:
-                mesh_name, ok = self.input_dialog.getText(self, 'Input', 'Specify the object Class name')#, text='ossicles')
-                if not ok: return 0
-
+            mesh_name = pathlib.Path(self.mesh_path).stem
             self.meshdict[mesh_name] = self.mesh_path
             self.mesh_opacity[mesh_name] = self.surface_opacity
             transformation_matrix = self.transformation_matrix
             if self.mirror_x: transformation_matrix = np.array([[-1, 0, 0, 0], [0, 1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix
             if self.mirror_y: transformation_matrix = np.array([[1, 0, 0, 0], [0, -1, 0, 0], [0, 0, 1, 0], [0, 0, 0, 1]]) @ transformation_matrix                   
             self.add_mesh(mesh_name, self.mesh_path, transformation_matrix)
```

### Comparing `vision6D-0.1.4/vision6D/__init__.py` & `vision6D-0.1.5/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D/app.py` & `vision6D-0.1.5/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D/config.py` & `vision6D-0.1.5/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.1.5/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.1.5/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D/data/style.qss` & `vision6D-0.1.5/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D/interface.py` & `vision6D-0.1.5/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D/interface_gui.py` & `vision6D-0.1.5/vision6D/interface_gui.py`

 * *Files 0% similar despite different names*

```diff
@@ -167,15 +167,15 @@
   
     def add_pose(self, matrix:np.ndarray=None, rot:np.ndarray=None, trans:np.ndarray=None):
         if matrix is None: matrix = np.vstack((np.hstack((rot, trans)), [0, 0, 0, 1])) #if (rot is not None and trans is not None) else None
         self.initial_pose = matrix #if matrix is not None else self.transformation_matrix
         self.reset_gt_pose()
         self.reset_camera()
 
-    def add_mesh(self, mesh_name, mesh_source, transformation_matrix = None):
+    def add_mesh(self, mesh_name, mesh_source, transformation_matrix=None):
         """ add a mesh to the pyqt frame """
 
         flag = False
                               
         if isinstance(mesh_source, pathlib.WindowsPath) or isinstance(mesh_source, str):
             # Load the '.mesh' file
             if pathlib.Path(mesh_source).suffix == '.mesh': mesh_source = vis.utils.load_trimesh(mesh_source)
```

### Comparing `vision6D-0.1.4/vision6D/mainwindow.py` & `vision6D-0.1.5/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D/run_gui.py` & `vision6D-0.1.5/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D/utils.py` & `vision6D-0.1.5/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.4/vision6D.egg-info/PKG-INFO` & `vision6D-0.1.5/vision6D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.4
+Version: 0.1.5
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.1.4/vision6D.egg-info/SOURCES.txt` & `vision6D-0.1.5/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*


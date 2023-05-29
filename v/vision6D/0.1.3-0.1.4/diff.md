# Comparing `tmp/vision6D-0.1.3.tar.gz` & `tmp/vision6D-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.1.3.tar", last modified: Mon May 29 01:07:15 2023, max compression
+gzip compressed data, was "dist\vision6D-0.1.4.tar", last modified: Mon May 29 16:28:21 2023, max compression
```

## Comparing `vision6D-0.1.3.tar` & `vision6D-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 01:07:14.744768 vision6D-0.1.3/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.3/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1603 2023-05-29 01:07:14.745765 vision6D-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-28 01:21:42.000000 vision6D-0.1.3/README.md
--rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.3/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2023-05-29 01:07:14.750761 vision6D-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-05-28 01:21:42.000000 vision6D-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:07:14.556880 vision6D-0.1.3/test/
--rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.3/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.3/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:07:14.616877 vision6D-0.1.3/vision6D/
--rw-rw-rw-   0        0        0    50295 2023-05-29 01:06:23.000000 vision6D-0.1.3/vision6D/GUI.py
--rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.3/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.3/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.3/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:07:14.741767 vision6D-0.1.3/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.3/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.3/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.3/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.3/vision6D/interface.py
--rw-rw-rw-   0        0        0    26131 2023-05-28 21:42:04.000000 vision6D-0.1.3/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.3/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.3/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.3/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.3/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 01:07:14.680090 vision6D-0.1.3/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-05-29 01:07:14.000000 vision6D-0.1.3/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-29 01:07:14.000000 vision6D-0.1.3/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 01:07:14.000000 vision6D-0.1.3/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-29 01:07:14.000000 vision6D-0.1.3/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 01:07:14.000000 vision6D-0.1.3/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 16:28:21.529007 vision6D-0.1.4/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1603 2023-05-29 16:28:21.529007 vision6D-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-28 01:21:42.000000 vision6D-0.1.4/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.4/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2023-05-29 16:28:21.535007 vision6D-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-05-28 01:21:42.000000 vision6D-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:28:21.299204 vision6D-0.1.4/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.4/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.4/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:28:21.393353 vision6D-0.1.4/vision6D/
+-rw-rw-rw-   0        0        0    51799 2023-05-29 16:18:26.000000 vision6D-0.1.4/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.4/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.4/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.4/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:28:21.521537 vision6D-0.1.4/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.4/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.4/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.4/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.4/vision6D/interface.py
+-rw-rw-rw-   0        0        0    26131 2023-05-28 21:42:04.000000 vision6D-0.1.4/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.4/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.4/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.4/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.4/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 16:28:21.472067 vision6D-0.1.4/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-05-29 16:28:20.000000 vision6D-0.1.4/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-29 16:28:21.000000 vision6D-0.1.4/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 16:28:21.000000 vision6D-0.1.4/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-29 16:28:21.000000 vision6D-0.1.4/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 16:28:21.000000 vision6D-0.1.4/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.1.3/LICENSE` & `vision6D-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/PKG-INFO` & `vision6D-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.3
+Version: 0.1.4
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.1.3/README.md` & `vision6D-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/setup.cfg` & `vision6D-0.1.4/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e33 0d0a 7572  sion = 0.1.3..ur
+00000020: 7369 6f6e 203d 2030 2e31 2e34 0d0a 7572  sion = 0.1.4..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.1.3/test/test_create_dataset.py` & `vision6D-0.1.4/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/test/test_projection.py` & `vision6D-0.1.4/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/GUI.py` & `vision6D-0.1.4/vision6D/GUI.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import trimesh
 import pathlib
 import PIL
 import ast
 import json
 import math
 import copy
+from skimage.metrics import peak_signal_noise_ratio, structural_similarity
 
 # Qt5 import
 from PyQt5 import QtWidgets, QtGui
 from pyvistaqt import QtInteractor, MainWindow
 from PyQt5.QtCore import Qt, QPoint
 
 # self defined package import
@@ -87,14 +88,70 @@
         return (self.args1.text(), 
                 self.args2.text(), 
                 self.args3.text(),
                 self.args4.text(),
                 self.args5.text(),
                 self.args6.text())
     
+class CalibrationPopWindow(QtWidgets.QDialog):
+    def __init__(self, calibrated_image, original_image, parent=None):
+        super(CalibrationPopWindow, self).__init__(parent)
+        self.setWindowFlags(self.windowFlags() & ~Qt.WindowContextHelpButtonHint)
+
+        self.calibrated_image = calibrated_image
+        self.original_image = original_image
+
+        self.setWindowTitle("Vision6D")
+        self.setFixedSize(960, 540)
+
+        overall = QtWidgets.QVBoxLayout()
+        layout = QtWidgets.QHBoxLayout()
+
+        vbox1layout = QtWidgets.QVBoxLayout()
+        label1 = QtWidgets.QLabel("Calibrated image", self)
+        label1.setAlignment(Qt.AlignCenter)
+        pixmap_label1 = QtWidgets.QLabel(self)
+        qimage1 = QtGui.QImage(self.calibrated_image, self.calibrated_image.shape[1], self.calibrated_image.shape[0], QtGui.QImage.Format_RGB888)
+        pixmap1 = QtGui.QPixmap.fromImage(qimage1)
+        pixmap1 = QtGui.QPixmap.fromImage(qimage1).scaled(960, 540, Qt.KeepAspectRatio)
+        pixmap_label1.setPixmap(pixmap1)
+        pixmap_label1.setAlignment(Qt.AlignCenter)
+        vbox1layout.addWidget(label1)
+        vbox1layout.addWidget(pixmap_label1)
+
+        vbox2layout = QtWidgets.QVBoxLayout()
+        label2 = QtWidgets.QLabel("Original image", self)
+        label2.setAlignment(Qt.AlignCenter)
+        pixmap_label2 = QtWidgets.QLabel(self)
+        qimage2 = QtGui.QImage(self.original_image, self.original_image.shape[1], self.original_image.shape[0], QtGui.QImage.Format_RGB888)
+        pixmap2 = QtGui.QPixmap.fromImage(qimage2)
+        pixmap2 = QtGui.QPixmap.fromImage(qimage2).scaled(960, 540, Qt.KeepAspectRatio)
+        pixmap_label2.setPixmap(pixmap2)
+        pixmap_label2.setAlignment(Qt.AlignCenter)
+
+        vbox2layout.addWidget(label2)
+        vbox2layout.addWidget(pixmap_label2)
+
+        layout.addLayout(vbox1layout)
+        layout.addLayout(vbox2layout)
+
+        psnr, ssim = self.calculate_similarity()
+        similarity_label = QtWidgets.QLabel(f"PSNR is {psnr} and SSIM is {ssim}", self)
+        similarity_label.setAlignment(Qt.AlignCenter)
+
+        overall.addLayout(layout)
+        overall.addWidget(similarity_label)
+
+        self.setLayout(overall)
+
+    def calculate_similarity(self):
+        psnr = peak_signal_noise_ratio(self.calibrated_image, self.original_image, data_range=255)
+        ssim = structural_similarity(self.calibrated_image, self.original_image, data_range=255, channel_axis=2)
+        return psnr, ssim
+
 class GetTextDialog(QtWidgets.QDialog):
     def __init__(self, parent=None):
         super(GetTextDialog, self).__init__(parent)
 
         layout = QtWidgets.QVBoxLayout(self)
         
         self.setWindowTitle("Vision6D")
@@ -258,14 +315,15 @@
         exportMenu.addAction('Mask Render', self.export_mask_plot)
         exportMenu.addAction('Mesh Render', self.export_mesh_plot)
         exportMenu.addAction('SegMesh Render', self.export_segmesh_plot)
         exportMenu.addAction('Pose', self.export_pose)
                 
         # Add camera related actions
         CameraMenu = mainMenu.addMenu('Camera')
+        CameraMenu.addAction('Calibrate', self.camera_calibrate)
         CameraMenu.addAction('Reset Camera (c)', self.reset_camera)
         CameraMenu.addAction('Zoom In (x)', self.zoom_in)
         CameraMenu.addAction('Zoom Out (z)', self.zoom_out)
 
         # add mirror actors related actions
         mirrorMenu = mainMenu.addMenu('Mirror')
         mirror_x = functools.partial(self.mirror_actors, direction='x')
@@ -314,14 +372,25 @@
     def set_camera_props(self):
         # Set up the camera
         self.camera = pv.Camera()
         self.set_camera_intrinsics()
         self.set_camera_extrinsics()
         self.plotter.camera = self.camera.copy()
 
+    def camera_calibrate(self):
+        if self.image_path != '' and self.image_path is not None:
+            original_image = np.array(PIL.Image.open(self.image_path), dtype='uint8')
+            calibrated_image = np.array(self.render_image(self.image_actor, self.plotter.camera.copy()), dtype='uint8')
+        else:
+            QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
+            return 0
+        
+        calibrate_pop = CalibrationPopWindow(calibrated_image, original_image)
+        calibrate_pop.exec_()
+
     def set_camera(self):
         dialog = CameraPropsInputDialog(
             line1=("Fx", self.fx), 
             line2=("Fy", self.fy), 
             line3=("Cx", self.cx), 
             line4=("Cy", self.cy), 
             line5=("View Up", self.cam_viewup), 
@@ -573,34 +642,56 @@
         self.used_colors = []
         self.color_button.setText("Color")
 
         self.ignore_slider_value_change = True
         self.opacity_slider.setValue(100)
         self.ignore_slider_value_change = False
 
+    def render_image(self, actor, camera):
+        self.render.clear()
+        render_actor = actor.copy(deep=True)
+        render_actor.GetProperty().opacity = 1
+        self.render.add_actor(render_actor, pickable=False)
+        self.render.camera = camera
+        self.render.disable()
+        self.render.show(auto_close=False)
+        image = self.render.last_image
+        return image
+    
+    def render_mesh(self, render_all_meshes, camera, point_clouds):
+        self.render.clear()
+        for mesh_name, mesh_actor in self.mesh_actors.items():
+            if not render_all_meshes:
+                if mesh_name != self.reference: continue
+            vertices, faces = vis.utils.get_mesh_actor_vertices_faces(mesh_actor)
+            mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
+            colors = vis.utils.get_mesh_actor_scalars(mesh_actor)
+            if colors is not None: 
+                assert colors.shape == vertices.shape, "colors shape should be the same as vertices shape"
+                mesh = self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='surface', opacity=1, name=mesh_name) if not point_clouds else self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=mesh_name)
+            else:
+                mesh = self.render.add_mesh(mesh_data, color=self.mesh_colors[mesh_name], style='surface', opacity=1, name=mesh_name) if not point_clouds else self.render.add_mesh(mesh_data, color=self.mesh_colors[mesh_name], style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=mesh_name)
+            mesh.user_matrix = self.mesh_actors[self.reference].user_matrix
+        self.render.camera = camera
+        self.render.disable()
+        self.render.show(auto_close=False)
+        image = self.render.last_image
+        return image
+
     def export_image_plot(self):
 
         if self.image_actor is None:
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load an image first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         
         reply = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
         if reply == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
         else: camera = self.plotter.camera.copy()
 
-        self.render.clear()
-        image_actor = self.image_actor.copy(deep=True)
-        image_actor.GetProperty().opacity = 1
-        self.render.add_actor(image_actor, pickable=False, name="image")
-        self.render.camera = camera
-        self.render.disable()
-        self.render.show(auto_close=False)
-
-        # obtain the rendered image
-        image = self.render.last_image
+        image = self.render_image(self.image_actor, camera)
         output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Image Files (*.png)")
         if output_path: 
             rendered_image = PIL.Image.fromarray(image)
             rendered_image.save(output_path)
             self.output_text.append(f"-> Export image render to:\n {str(output_path)}")
 
     def export_mask_plot(self):
@@ -608,24 +699,15 @@
             QtWidgets.QMessageBox.warning(self, 'vision6D', "Need to load a mask first!", QtWidgets.QMessageBox.Ok, QtWidgets.QMessageBox.Ok)
             return 0
         
         reply = QtWidgets.QMessageBox.question(self,"vision6D", "Reset Camera?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
         if reply == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
         else: camera = self.plotter.camera.copy()
 
-        self.render.clear()
-        mask_actor = self.mask_actor.copy(deep=True)
-        mask_actor.GetProperty().opacity = 1
-        self.render.add_actor(mask_actor, pickable=False, name="mask")
-        self.render.camera = camera
-        self.render.disable()
-        self.render.show(auto_close=False)
-
-        # obtain the rendered image
-        image = self.render.last_image
+        image = self.render_image(self.mask_actor, camera)
         output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Mask Files (*.png)")
         if output_path:
             rendered_image = PIL.Image.fromarray(image)
             rendered_image.save(output_path)
             self.output_text.append(f"-> Export mask render to:\n {str(output_path)}")
 
     def export_mesh_plot(self, reply_reset_camera=None, reply_render_mesh=None, reply_export_surface=None, save_render=True):
@@ -642,36 +724,16 @@
         if reply_reset_camera == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
         else: camera = self.plotter.camera.copy()
         if reply_render_mesh == QtWidgets.QMessageBox.No: render_all_meshes = True
         else: render_all_meshes = False
         if reply_export_surface == QtWidgets.QMessageBox.No: point_clouds = True
         else: point_clouds = False
         
-        # Clear out the render
-        self.render.clear()
-
-        for mesh_name, mesh_actor in self.mesh_actors.items():
-            if not render_all_meshes:
-                if mesh_name != self.reference: continue
-            vertices, faces = vis.utils.get_mesh_actor_vertices_faces(mesh_actor)
-            mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
-            colors = vis.utils.get_mesh_actor_scalars(mesh_actor)
-            if colors is not None: 
-                assert colors.shape == vertices.shape, "colors shape should be the same as vertices shape"
-                mesh = self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='surface', opacity=1, name=mesh_name) if not point_clouds else self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=mesh_name)
-            else:
-                mesh = self.render.add_mesh(mesh_data, color=self.mesh_colors[mesh_name], style='surface', opacity=1, name=mesh_name) if not point_clouds else self.render.add_mesh(mesh_data, color=self.mesh_colors[mesh_name], style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=mesh_name)
-            mesh.user_matrix = self.mesh_actors[self.reference].user_matrix
-      
-        self.render.camera = camera
-        self.render.disable(); self.render.show(auto_close=False)
-
-        # obtain the rendered image
-        image = self.render.last_image
-
+        image = self.render_mesh(render_all_meshes, camera, point_clouds)
+        
         if save_render:
             output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "Mesh Files (*.png)")
             if output_path:
                 rendered_image = PIL.Image.fromarray(image)
                 rendered_image.save(output_path)
                 self.output_text.append(f"-> Export reference mesh render to:\n {str(output_path)}")
 
@@ -691,43 +753,17 @@
         reply_export_surface = QtWidgets.QMessageBox.question(self,"vision6D", "Export the mesh as surface?", QtWidgets.QMessageBox.Yes, QtWidgets.QMessageBox.No)
 
         if reply_reset_camera == QtWidgets.QMessageBox.Yes: camera = self.camera.copy()
         else: camera = self.plotter.camera.copy()
         if reply_export_surface == QtWidgets.QMessageBox.No: point_clouds = True
         else: point_clouds = False
 
-        self.render.clear()
-        mask_actor = self.mask_actor.copy(deep=True)
-        mask_actor.GetProperty().opacity = 1
-        self.render.add_actor(mask_actor, pickable=False, name="mask")
-        self.render.camera = camera
-        self.render.disable()
-        self.render.show(auto_close=False)
-        segmask = self.render.last_image
+        segmask = self.render_image(self.mask_actor, camera)
         if np.max(segmask) > 1: segmask = segmask / 255
-
-        self.render.clear()
-                
-        # Render the targeting objects
-        vertices, faces = vis.utils.get_mesh_actor_vertices_faces(self.mesh_actors[self.reference])
-        mesh_data = pv.wrap(trimesh.Trimesh(vertices, faces, process=False))
-        colors = vis.utils.get_mesh_actor_scalars(self.mesh_actors[self.reference])
-        if colors is not None: 
-            assert colors.shape == vertices.shape, "colors shape should be the same as vertices shape"
-            mesh = self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='surface', opacity=1, name=self.reference) if not point_clouds else self.render.add_mesh(mesh_data, scalars=colors, rgb=True, style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=self.reference)
-        else:
-            mesh = self.render.add_mesh(mesh_data, color=self.mesh_colors[self.reference], style='surface', opacity=1, name=self.reference) if not point_clouds else self.render.add_mesh(mesh_data, color=self.mesh_colors[self.reference], style='points', point_size=1, render_points_as_spheres=False, opacity=1, name=self.reference)
-
-        mesh.user_matrix = self.mesh_actors[self.reference].user_matrix
-
-        self.render.camera = camera
-        self.render.disable(); self.render.show(auto_close=False)
-
-        # obtain the rendered image
-        image = self.render.last_image
+        image = self.render_mesh(False, camera, point_clouds)
         image = (image * segmask).astype(np.uint8)
         output_path, _ = QtWidgets.QFileDialog.getSaveFileName(self, "Save File", "", "SegMesh Files (*.png)")
         if output_path:
             rendered_image = PIL.Image.fromarray(image)
             rendered_image.save(output_path)
             self.output_text.append(f"-> Export segmask render:\n to {str(output_path)}")
```

### Comparing `vision6D-0.1.3/vision6D/__init__.py` & `vision6D-0.1.4/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/app.py` & `vision6D-0.1.4/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/config.py` & `vision6D-0.1.4/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.1.4/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.1.4/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/data/style.qss` & `vision6D-0.1.4/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/interface.py` & `vision6D-0.1.4/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/interface_gui.py` & `vision6D-0.1.4/vision6D/interface_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/mainwindow.py` & `vision6D-0.1.4/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/run_gui.py` & `vision6D-0.1.4/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D/utils.py` & `vision6D-0.1.4/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.3/vision6D.egg-info/PKG-INFO` & `vision6D-0.1.4/vision6D.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.3
+Version: 0.1.4
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.1.3/vision6D.egg-info/SOURCES.txt` & `vision6D-0.1.4/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*


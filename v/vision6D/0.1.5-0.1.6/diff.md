# Comparing `tmp/vision6D-0.1.5.tar.gz` & `tmp/vision6D-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\vision6D-0.1.5.tar", last modified: Mon May 29 20:36:08 2023, max compression
+gzip compressed data, was "dist\vision6D-0.1.6.tar", last modified: Mon May 29 21:13:38 2023, max compression
```

## Comparing `vision6D-0.1.5.tar` & `vision6D-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 20:36:07.946940 vision6D-0.1.5/
--rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1603 2023-05-29 20:36:07.947940 vision6D-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-28 01:21:42.000000 vision6D-0.1.5/README.md
--rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0     1927 2023-05-29 20:36:07.953939 vision6D-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0      165 2023-05-28 01:21:42.000000 vision6D-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:36:07.711492 vision6D-0.1.5/test/
--rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.5/test/test_create_dataset.py
--rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.5/test/test_projection.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:36:07.824497 vision6D-0.1.5/vision6D/
--rw-rw-rw-   0        0        0    51583 2023-05-29 20:31:40.000000 vision6D-0.1.5/vision6D/GUI.py
--rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.5/vision6D/__init__.py
--rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.5/vision6D/app.py
--rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.5/vision6D/config.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:36:07.943939 vision6D-0.1.5/vision6D/data/
--rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.5/vision6D/data/ossiclesCoordinateMapping.json
--rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.5/vision6D/data/ossiclesCoordinateMappingv1.json
--rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.5/vision6D/data/style.qss
--rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.5/vision6D/interface.py
--rw-rw-rw-   0        0        0    26129 2023-05-29 20:26:33.000000 vision6D-0.1.5/vision6D/interface_gui.py
--rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.5/vision6D/mainwindow.py
--rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.5/vision6D/run_gui.py
--rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.5/vision6D/run_interface.py
--rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.5/vision6D/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-29 20:36:07.897480 vision6D-0.1.5/vision6D.egg-info/
--rw-rw-rw-   0        0        0     1603 2023-05-29 20:36:07.000000 vision6D-0.1.5/vision6D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      597 2023-05-29 20:36:07.000000 vision6D-0.1.5/vision6D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 20:36:07.000000 vision6D-0.1.5/vision6D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-29 20:36:07.000000 vision6D-0.1.5/vision6D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 20:36:07.000000 vision6D-0.1.5/vision6D.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 21:13:38.444724 vision6D-0.1.6/
+-rw-rw-rw-   0        0        0     1086 2023-01-03 15:55:06.000000 vision6D-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       33 2023-05-27 00:07:11.000000 vision6D-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1603 2023-05-29 21:13:38.446096 vision6D-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-28 01:21:42.000000 vision6D-0.1.6/README.md
+-rw-rw-rw-   0        0        0      413 2023-01-03 15:55:07.000000 vision6D-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0     1927 2023-05-29 21:13:38.451724 vision6D-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      165 2023-05-28 01:21:42.000000 vision6D-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 21:13:38.210260 vision6D-0.1.6/test/
+-rw-rw-rw-   0        0        0    21974 2023-05-17 18:41:02.000000 vision6D-0.1.6/test/test_create_dataset.py
+-rw-rw-rw-   0        0        0     3630 2023-05-14 22:36:01.000000 vision6D-0.1.6/test/test_projection.py
+drwxrwxrwx   0        0        0        0 2023-05-29 21:13:38.312759 vision6D-0.1.6/vision6D/
+-rw-rw-rw-   0        0        0    51646 2023-05-29 21:09:55.000000 vision6D-0.1.6/vision6D/GUI.py
+-rw-rw-rw-   0        0        0      939 2023-05-28 01:21:42.000000 vision6D-0.1.6/vision6D/__init__.py
+-rw-rw-rw-   0        0        0    19331 2023-05-14 22:36:01.000000 vision6D-0.1.6/vision6D/app.py
+-rw-rw-rw-   0        0        0    12369 2023-05-28 01:21:42.000000 vision6D-0.1.6/vision6D/config.py
+drwxrwxrwx   0        0        0        0 2023-05-29 21:13:38.440722 vision6D-0.1.6/vision6D/data/
+-rw-rw-rw-   0        0        0   445902 2023-05-14 22:36:01.000000 vision6D-0.1.6/vision6D/data/ossiclesCoordinateMapping.json
+-rw-rw-rw-   0        0        0   335336 2023-05-14 22:36:02.000000 vision6D-0.1.6/vision6D/data/ossiclesCoordinateMappingv1.json
+-rw-rw-rw-   0        0        0    12109 2023-05-15 22:13:50.000000 vision6D-0.1.6/vision6D/data/style.qss
+-rw-rw-rw-   0        0        0    22897 2023-05-14 22:36:02.000000 vision6D-0.1.6/vision6D/interface.py
+-rw-rw-rw-   0        0        0    25978 2023-05-29 21:10:54.000000 vision6D-0.1.6/vision6D/interface_gui.py
+-rw-rw-rw-   0        0        0    33713 2023-05-14 22:36:02.000000 vision6D-0.1.6/vision6D/mainwindow.py
+-rw-rw-rw-   0        0        0    14068 2023-05-15 23:19:36.000000 vision6D-0.1.6/vision6D/run_gui.py
+-rw-rw-rw-   0        0        0      197 2023-05-14 22:53:44.000000 vision6D-0.1.6/vision6D/run_interface.py
+-rw-rw-rw-   0        0        0    14911 2023-05-14 22:36:02.000000 vision6D-0.1.6/vision6D/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-29 21:13:38.385809 vision6D-0.1.6/vision6D.egg-info/
+-rw-rw-rw-   0        0        0     1603 2023-05-29 21:13:37.000000 vision6D-0.1.6/vision6D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      597 2023-05-29 21:13:38.000000 vision6D-0.1.6/vision6D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 21:13:38.000000 vision6D-0.1.6/vision6D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-29 21:13:38.000000 vision6D-0.1.6/vision6D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 21:13:38.000000 vision6D-0.1.6/vision6D.egg-info/top_level.txt
```

### Comparing `vision6D-0.1.5/LICENSE` & `vision6D-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/PKG-INFO` & `vision6D-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.5
+Version: 0.1.6
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.1.5/README.md` & `vision6D-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/setup.cfg` & `vision6D-0.1.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2076 6973 696f 6e36 440d 0a76 6572   = vision6D..ver
-00000020: 7369 6f6e 203d 2030 2e31 2e35 0d0a 7572  sion = 0.1.5..ur
+00000020: 7369 6f6e 203d 2030 2e31 2e36 0d0a 7572  sion = 0.1.6..ur
 00000030: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000040: 7562 2e63 6f6d 2f79 6b7a 7a6b 792f 7669  ub.com/ykzzky/vi
 00000050: 7369 6f6e 3644 0d0a 6465 7363 7269 7074  sion6D..descript
 00000060: 696f 6e20 3d20 7669 7369 6f6e 3644 3a20  ion = vision6D: 
 00000070: 4120 746f 6f6c 2066 6f72 2036 4420 706f  A tool for 6D po
 00000080: 7365 2065 7374 696d 6174 696f 6e20 616e  se estimation an
 00000090: 6e6f 7461 7469 6f6e 0d0a 6c6f 6e67 5f64  notation..long_d
```

### Comparing `vision6D-0.1.5/test/test_create_dataset.py` & `vision6D-0.1.6/test/test_create_dataset.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/test/test_projection.py` & `vision6D-0.1.6/test/test_projection.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D/GUI.py` & `vision6D-0.1.6/vision6D/GUI.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,14 +471,17 @@
             self.add_mask_file(prompt=False)
             self.add_pose_file()
 
             for mesh_path in mesh_paths:
                 self.mesh_path = mesh_path
                 self.add_mesh_file(prompt=False)
 
+            # reset camera
+            self.reset_camera()
+
     def add_image_file(self, prompt=True):
         if prompt:
             if self.image_path == None or self.image_path == '':
                 self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", "", "Files (*.png *.jpg)")
             else:
                 self.image_path, _ = self.file_dialog.getOpenFileName(None, "Open file", str(pathlib.Path(self.image_path).parent), "Files (*.png *.jpg)")
```

### Comparing `vision6D-0.1.5/vision6D/__init__.py` & `vision6D-0.1.6/vision6D/__init__.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D/app.py` & `vision6D-0.1.6/vision6D/app.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D/config.py` & `vision6D-0.1.6/vision6D/config.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D/data/ossiclesCoordinateMapping.json` & `vision6D-0.1.6/vision6D/data/ossiclesCoordinateMapping.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D/data/ossiclesCoordinateMappingv1.json` & `vision6D-0.1.6/vision6D/data/ossiclesCoordinateMappingv1.json`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D/data/style.qss` & `vision6D-0.1.6/vision6D/data/style.qss`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D/interface.py` & `vision6D-0.1.6/vision6D/interface.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D/interface_gui.py` & `vision6D-0.1.6/vision6D/interface_gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,14 @@
         # add remove current image to removeMenu
         if 'image' not in self.track_actors_names:
             self.track_actors_names.append('image')
             self.add_button_actor_name('image')
 
         self.check_button('image')
 
-        # reset the camera
-        self.reset_camera()
-
     def add_mask(self, mask_source):
 
         if isinstance(mask_source, pathlib.WindowsPath) or isinstance(mask_source, str):
             mask_source = np.array(PIL.Image.open(mask_source), dtype='uint8')
         if len(mask_source.shape) == 2: 
             mask_source = mask_source[..., None]
 
@@ -158,17 +155,14 @@
         # add remove current image to removeMenu
         if 'mask' not in self.track_actors_names:
             self.track_actors_names.append('mask')
             self.add_button_actor_name('mask')
 
         self.check_button('mask')
 
-        # reset the camera
-        self.reset_camera()
-  
     def add_pose(self, matrix:np.ndarray=None, rot:np.ndarray=None, trans:np.ndarray=None):
         if matrix is None: matrix = np.vstack((np.hstack((rot, trans)), [0, 0, 0, 1])) #if (rot is not None and trans is not None) else None
         self.initial_pose = matrix #if matrix is not None else self.transformation_matrix
         self.reset_gt_pose()
         self.reset_camera()
 
     def add_mesh(self, mesh_name, mesh_source, transformation_matrix=None):
@@ -223,16 +217,14 @@
         actor_vertices, actor_faces = vis.utils.get_mesh_actor_vertices_faces(actor)
         assert (actor_vertices == source_verts).all(), "vertices should be the same"
         assert (actor_faces == source_faces).all(), "faces should be the same"
         assert actor.name == mesh_name, "actor's name should equal to mesh_name"
         
         self.mesh_actors[mesh_name] = actor
 
-        self.reset_camera()
-
         # add remove current mesh to removeMenu
         if mesh_name not in self.track_actors_names:
             self.track_actors_names.append(mesh_name)
             self.add_button_actor_name(mesh_name)
 
         self.check_button(mesh_name)
```

### Comparing `vision6D-0.1.5/vision6D/mainwindow.py` & `vision6D-0.1.6/vision6D/mainwindow.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D/run_gui.py` & `vision6D-0.1.6/vision6D/run_gui.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D/utils.py` & `vision6D-0.1.6/vision6D/utils.py`

 * *Files identical despite different names*

### Comparing `vision6D-0.1.5/vision6D.egg-info/PKG-INFO` & `vision6D-0.1.6/vision6D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision6D
-Version: 0.1.5
+Version: 0.1.6
 Summary: vision6D: A tool for 6D pose estimation annotation
 Home-page: https://github.com/ykzzky/vision6D
 License: GNU GENERAL Public License
 Project-URL: Bug Tracker, https://github.com/ykzzky/vision6D/issues
 Keywords: multimodal,data,analysis,real-time,distributed
 Platform: any
 Classifier: Programming Language :: Python :: 3
```

### Comparing `vision6D-0.1.5/vision6D.egg-info/SOURCES.txt` & `vision6D-0.1.6/vision6D.egg-info/SOURCES.txt`

 * *Files identical despite different names*


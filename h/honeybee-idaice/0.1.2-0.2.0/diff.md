# Comparing `tmp/honeybee-idaice-0.1.2.tar.gz` & `tmp/honeybee-idaice-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.1.2.tar", last modified: Sun May 28 23:34:22 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.2.0.tar", last modified: Mon May 29 01:27:31 2023, max compression
```

## Comparing `honeybee-idaice-0.1.2.tar` & `honeybee-idaice-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/geometry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/geometry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/setup.py
```

### Comparing `honeybee-idaice-0.1.2/LICENSE` & `honeybee-idaice-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/PKG-INFO` & `honeybee-idaice-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.1.2
+Version: 0.2.0
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.1.2/README.md` & `honeybee-idaice-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/archive.py` & `honeybee-idaice-0.2.0/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.2.0/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/geometry_utils.py` & `honeybee-idaice-0.2.0/honeybee_idaice/geometry_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     boundaries = Polygon2D.boolean_union_all(boundaries, tolerance=0.001)
 
     assert boundaries, f'Failed to calculate the floor boundary for {room.display_name}'
     boundary = boundaries[0]
 
     # insert missing points for the wall starting points
     wall_st_pts = [
-        face.geometry.lower_left_corner
+        face.geometry.lower_left_counter_clockwise_vertices[0]
         for face in room.faces
         if isinstance(face.type, Wall)
     ]
 
     vertices = boundary.vertices
     wall_st_pts_2d = [Point2D(v[0], v[1]) for v in wall_st_pts]
     polygon_update = []
@@ -69,15 +69,20 @@
         Point3D(point.x, point.y, z) for point in boundary.vertices
     ]
 
     geometry = Face3D(boundary, plane=floor_geom[0].plane)
     geometry = geometry.flip()
 
     vertices = geometry.lower_left_counter_clockwise_vertices
-    pole = geometry.pole_of_inaccessibility(0.01)
+    center = geometry.center
+    if geometry.is_point_on_face(center, 0.01):
+        pole = center
+    else:
+        pole = geometry.pole_of_inaccessibility(0.01)
+
     return vertices, pole
 
 
 def get_ceiling_boundary(ceilings):
     """Get a list of vertices for ceiling boundary for a room.
 
     This function joins all the floor faces and returns a list of Point3D that define the
```

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.2.0/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.2.0/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.2.0/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.2.0/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.2.0/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.2.0/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/writer.py` & `honeybee-idaice-0.2.0/honeybee_idaice/writer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Write an idm file from a HBJSON file."""
 import pathlib
 import shutil
 import math
-from typing import List
+from typing import List, Union
 
-from honeybee.model import Model, Room, Face, Aperture
+from honeybee.model import Model, Room, Face, Aperture, Door
 from honeybee.facetype import RoofCeiling, Wall, Floor
 from ladybug_geometry.geometry3d import Point3D, Vector3D, Plane, Face3D
 from ladybug_geometry.bounding import bounding_box
 
 from .archive import create_idm
 from .geometry_utils import get_floor_boundary, get_ceiling_boundary
 
 
-def opening_to_idm(opening: Aperture) -> str:
+def opening_to_idm(opening: Union[Aperture, Door], is_aperture=True) -> str:
     """Translate a HBJSON aperture to an IDM Window."""
     # name = opening.display_name
     name = opening.identifier
 
     # IDA-ICE looks to apertures from inside the room
     parent: Face3D = opening.parent.geometry.flip()
     opening: Face3D = opening.geometry.flip()
@@ -38,19 +38,27 @@
 
     ref_plane = Plane(rel_plane.n, parent_llc, proj_x)
     min_2d = ref_plane.xyz_to_xy(apt_llc)
     max_2d = ref_plane.xyz_to_xy(apt_urc)
     height = max_2d.y - min_2d.y
     width = max_2d.x - min_2d.x
 
-    opening_idm = f'\n ((CE-WINDOW :N "{name}" :T WINDOW)\n' \
-        f'  (:PAR :N X :V {min_2d.x})\n' \
-        f'  (:PAR :N Y :V {min_2d.y})\n' \
-        f'  (:PAR :N DX :V {width})\n' \
-        f'  (:PAR :N DY :V {height}))'
+    if is_aperture:
+        opening_idm = f'\n ((CE-WINDOW :N "{name}" :T WINDOW)\n' \
+            f'  (:PAR :N X :V {min_2d.x})\n' \
+            f'  (:PAR :N Y :V {min_2d.y})\n' \
+            f'  (:PAR :N DX :V {width})\n' \
+            f'  (:PAR :N DY :V {height}))'
+    else:
+        opening_idm = f'\n ((OPENING :N "{name}" :T OPENING)\n' \
+            f'  (:PAR :N X :V {min_2d.x})\n' \
+            f'  (:PAR :N Y :V {min_2d.y})\n' \
+            f'  (:PAR :N DX :V {width})\n' \
+            f'  (:PAR :N DY :V {height})\n' \
+            f'  (:RES :N OPENING-SCHEDULE :V ALWAYS_OFF))'
 
     return opening_idm
 
 
 def face_to_idm(face: Face, origin: Point3D, index: int):
     """Translate a HBJSON face to an IDM ENCLOSING-ELEMENT."""
     _face_mapper = {
@@ -70,18 +78,27 @@
     # add apertures
     windows = ['']
     for aperture in face.apertures:
         windows.append(opening_to_idm(aperture))
 
     windows = ''.join(windows)
 
+    # add doors
+    doors = ['']
+    for door in face.doors:
+        if door.user_data and door.user_data.get('ignore', False):
+            continue
+        doors.append(opening_to_idm(door, is_aperture=False))
+
+    doors = ''.join(doors)
+
     face = f'((ENCLOSING-ELEMENT :N "{name}" :T {type_} :INDEX {index})\n' \
         f' ((AGGREGATE :N GEOMETRY)\n' \
         f'  (:PAR :N CORNERS :DIM ({count} 3) :SP ({count} 3) :V #2A({vertices_idm}))\n' \
-        f'  (:PAR :N SLOPE :V {face.altitude + 90})){windows})'
+        f'  (:PAR :N SLOPE :V {face.altitude + 90})){windows}\n{doors})'
 
     return face
 
 
 def ceilings_to_idm(faces: List[Face], origin: Point3D):
     """Translate a collection of ceilings face to an IDM ENCLOSING-ELEMENT."""
     index = -1000
@@ -179,15 +196,15 @@
             floors.append(face)
         else:
             # air boundary
             print(f'Face from type {type_} is not currently supported.')
 
     protected = False
     for w in walls:
-        if abs(w.altitude) <= 0.1:
+        if abs(w.altitude) > 5:
             # non-vertical wall
             protected = True
             break
     if protected:
         geometry = '((AGGREGATE :N GEOMETRY :X NIL)\n' \
             ' (:PAR :N PROTECTED_SHAPE :V :TRUE)\n' \
             f' (:PAR :N ORIGIN :V #({origin.x} {origin.y}))\n' \
@@ -342,14 +359,28 @@
         bldg_template = templates_folder.joinpath('building.idm')
         for line in bldg_template.open('r'):
             bldg.write(line)
         # create a building section for each floor
         for grouped_room, floor_height in zip(grouped_rooms, floor_heights):
             section = section_to_idm(grouped_room, name=f'Level_{floor_height}')
             bldg.write(section)
+
+            # filter the doors
+            tolerance = 0.75  # assuming the door centers are not closer than this dist
+            door_tracker = []
+            for room in grouped_room:
+                for face in room.faces:
+                    for door in face.doors:
+                        center = door.geometry.center
+                        for pt in door_tracker:
+                            if pt.distance_to_point(center) <= tolerance:
+                                door.user_data = {'ignore': True}
+                                break
+                        door_tracker.append(center)
+
         # add rooms as zones
         for room in model.rooms:
             bldg.write(f'((CE-ZONE :N "{room.display_name}" :T ZONE))\n')
         bldg.write(f';[end of {bldg_name}.idm]\n')
 
     # copy template files
     templates = ['plant.idm', 'ahu.idc', 'ahu.idm', 'plant.idc']
```

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.2.0/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.2.0/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.1.2
+Version: 0.2.0
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.1.2/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.2.0/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.2/setup.py` & `honeybee-idaice-0.2.0/setup.py`

 * *Files identical despite different names*


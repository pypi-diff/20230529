# Comparing `tmp/honeybee-idaice-0.1.1.tar.gz` & `tmp/honeybee-idaice-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.1.1.tar", last modified: Sun May 28 18:57:15 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.1.2.tar", last modified: Sun May 28 23:34:22 2023, max compression
```

## Comparing `honeybee-idaice-0.1.1.tar` & `honeybee-idaice-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/geometry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    12695 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 18:57:15.000000 honeybee-idaice-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-28 18:55:58.000000 honeybee-idaice-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/geometry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    14137 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-28 23:34:22.000000 honeybee-idaice-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-28 23:32:57.000000 honeybee-idaice-0.1.2/setup.py
```

### Comparing `honeybee-idaice-0.1.1/LICENSE` & `honeybee-idaice-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/PKG-INFO` & `honeybee-idaice-0.1.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.1.1
+Version: 0.1.2
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.1.1/README.md` & `honeybee-idaice-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/archive.py` & `honeybee-idaice-0.1.2/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.1.2/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/geometry_utils.py` & `honeybee-idaice-0.1.2/honeybee_idaice/geometry_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,20 +32,21 @@
     boundaries = Polygon2D.boolean_union_all(boundaries, tolerance=0.001)
 
     assert boundaries, f'Failed to calculate the floor boundary for {room.display_name}'
     boundary = boundaries[0]
 
     # insert missing points for the wall starting points
     wall_st_pts = [
-        face.geometry.lower_left_corner for face in room.faces
+        face.geometry.lower_left_corner
+        for face in room.faces
         if isinstance(face.type, Wall)
     ]
+
     vertices = boundary.vertices
     wall_st_pts_2d = [Point2D(v[0], v[1]) for v in wall_st_pts]
-
     polygon_update = []
     for pt in wall_st_pts_2d:
         # check if pt is already included
         for v in vertices:
             if pt.distance_to_point(v) <= 0.001:
                 break
         else:
@@ -68,16 +69,16 @@
         Point3D(point.x, point.y, z) for point in boundary.vertices
     ]
 
     geometry = Face3D(boundary, plane=floor_geom[0].plane)
     geometry = geometry.flip()
 
     vertices = geometry.lower_left_counter_clockwise_vertices
-
-    return vertices
+    pole = geometry.pole_of_inaccessibility(0.01)
+    return vertices, pole
 
 
 def get_ceiling_boundary(ceilings):
     """Get a list of vertices for ceiling boundary for a room.
 
     This function joins all the floor faces and returns a list of Point3D that define the
     border of the floor in counter clockwise order starting from the lower left corner.
```

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.1.2/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.1.2/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.1.2/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.1.2/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.1.2/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.1.2/honeybee_idaice/templates/room.idm`

 * *Files 17% similar despite different names*

```diff
@@ -12,25 +12,14 @@
  (:PAR :N MIN_CO2 :V 700)
  (:PAR :N MAX_CO2 :V 1100)
  (:PAR :N MIN_LIGHT :V 100)
  (:PAR :N MAX_LIGHT :V 10000))
 ((AGGREGATE :N CENTRAL-AHU)
  (:PAR :N CAV_VENT_AIR :V 2.0)
  (:PAR :N CAV_VENT_SUP :V 2.0))
-((LIGHT :N "Light" :T LIGHT)
- (:PAR :N X :V 1.077)
- (:PAR :N Y :V 1.486)
- (:PAR :N DX :V 0.5384)
- (:PAR :N DY :V 0.743)
- (:PAR :N RATED_INPUT :V 50.0)
- (:RES :N SCHEDULE_0-1 :V ALWAYS_ON))
-((OCCUPANT :N "Occupant" :T OCCUPANT)
- (:PAR :N NUMBER_OF :V 1)
- (:RES :N SCHEDULE_0-1 :V ALWAYS_ON)
- (:PAR :N POSITION :V #(1.35 1.86 0.6)))
 ((EQUIPMENT :N "Equipment" :T EQUIPMENT)
  (:PAR :N EMITTED_SENSIBLE_POWER :V 150.0)
  (:RES :N SCHEDULE_0-1 :V ALWAYS_ON))
 ((MASS :N "Furniture" :T FURNITURE)
  (:PAR :N AREA :V 2.0))
 ((HC-UNIT :N "Ideal cooler" :T IDEAL-COOLER)
  (:PAR :N PMAX :V 2000))
```

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/writer.py` & `honeybee-idaice-0.1.2/honeybee_idaice/writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -128,29 +128,48 @@
         ceiling_idm.append(cp)
 
     return '\n'.join(ceiling_idm) + ')'
 
 
 def room_to_idm(room: Room):
     """Translate a Honeybee Room to an IDM Zone."""
+    room_idm = []
+
     # find floor boundary and llc for origin
-    vertices = get_floor_boundary(room)
+    vertices, pole = get_floor_boundary(room)
     origin = vertices[0]
+
+    # relative coordinates of the pole
+    rp = pole - origin
+    # arbitrary x and y size for lighting fixtures
+    lighting_x = 0.5
+    lighting_y = 0.5
+    min_x = rp.x - lighting_x
+    min_y = rp.y - lighting_y
+    # set the location of light and occupant
+    light_occ = '((LIGHT :N "Light" :T LIGHT)\n' \
+        f' (:PAR :N X :V {min_x})\n' \
+        f' (:PAR :N Y :V {min_y})\n' \
+        f' (:PAR :N DX :V {lighting_x})\n' \
+        f' (:PAR :N DY :V {lighting_y})\n' \
+        ' (:PAR :N RATED_INPUT :V 50.0)\n' \
+        ' (:RES :N SCHEDULE_0-1 :V ALWAYS_ON))\n' \
+        '((OCCUPANT :N "Occupant" :T OCCUPANT)\n' \
+        ' (:PAR :N NUMBER_OF :V 1)\n' \
+        ' (:RES :N SCHEDULE_0-1 :V ALWAYS_ON)\n' \
+        f' (:PAR :N POSITION :V #({rp.x} {rp.y} {0.6})))'
+
+    room_idm.append(light_occ)
+
     count = len(vertices)
     elevation = origin.z
     vertices_idm = ' '.join(
         f'({v.x - origin.x} {v.y - origin.y})' for v in vertices
     )
-    geometry = '((AGGREGATE :N GEOMETRY :X NIL)\n' \
-        f' (:PAR :N ORIGIN :V #({origin.x} {origin.y}))\n' \
-        f' (:PAR :N NCORN :V {count})\n' \
-        f' (:PAR :N CORNERS :DIM ({count} 2) :V #2A({vertices_idm}))\n' \
-        f' (:PAR :N FLOOR_HEIGHT_FROM_GROUND :V {elevation}))'
 
-    room_idm = [geometry]
     walls = []
     floors = []
     ceilings = []
     for face in room.faces:
         type_ = face.type
         if isinstance(type_, Wall):
             walls.append(face)
@@ -158,14 +177,36 @@
             ceilings.append(face)
         elif isinstance(type_, Floor):
             floors.append(face)
         else:
             # air boundary
             print(f'Face from type {type_} is not currently supported.')
 
+    protected = False
+    for w in walls:
+        if abs(w.altitude) <= 0.1:
+            # non-vertical wall
+            protected = True
+            break
+    if protected:
+        geometry = '((AGGREGATE :N GEOMETRY :X NIL)\n' \
+            ' (:PAR :N PROTECTED_SHAPE :V :TRUE)\n' \
+            f' (:PAR :N ORIGIN :V #({origin.x} {origin.y}))\n' \
+            f' (:PAR :N NCORN :V {count})\n' \
+            f' (:PAR :N CORNERS :DIM ({count} 2) :V #2A({vertices_idm}))\n' \
+            f' (:PAR :N FLOOR_HEIGHT_FROM_GROUND :V {elevation}))'
+    else:
+        geometry = '((AGGREGATE :N GEOMETRY :X NIL)\n' \
+            f' (:PAR :N ORIGIN :V #({origin.x} {origin.y}))\n' \
+            f' (:PAR :N NCORN :V {count})\n' \
+            f' (:PAR :N CORNERS :DIM ({count} 2) :V #2A({vertices_idm}))\n' \
+            f' (:PAR :N FLOOR_HEIGHT_FROM_GROUND :V {elevation}))'
+
+    room_idm.append(geometry)
+
     # write faces
     used_index = []
     last_index = len(walls) + 1
     for wall in walls:
         llc = wall.geometry.lower_left_corner
         sorted_vertices = sorted(vertices, key=lambda x: x.distance_to_point(llc))
         index = vertices.index(sorted_vertices[0]) + 1
@@ -174,16 +215,16 @@
             # use a new index and hope it doesn't have an aperture
             index = last_index
             last_index += 1
         used_index.append(index)
         face_idm = face_to_idm(wall, origin=origin, index=index)
         room_idm.append(face_idm)
 
-    for floor in floors:
-        face_idm = face_to_idm(floor, origin=origin, index=-2000)
+    for count, floor in enumerate(floors):
+        face_idm = face_to_idm(floor, origin=origin, index=-(2000 + count))
         room_idm.append(face_idm)
 
     ceiling_idm = ceilings_to_idm(ceilings, origin=origin)
     room_idm.append(ceiling_idm)
 
     return '\n'.join(room_idm)
```

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.1.2/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.1.2/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.1.1
+Version: 0.1.2
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.1.1/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.1.2/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.1.1/setup.py` & `honeybee-idaice-0.1.2/setup.py`

 * *Files identical despite different names*


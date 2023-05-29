# Comparing `tmp/honeybee-idaice-0.2.0.tar.gz` & `tmp/honeybee-idaice-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.2.0.tar", last modified: Mon May 29 01:27:31 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.2.1.tar", last modified: Mon May 29 01:44:26 2023, max compression
```

## Comparing `honeybee-idaice-0.2.0.tar` & `honeybee-idaice-0.2.1.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/geometry_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    15392 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 01:27:30.000000 honeybee-idaice-0.2.0/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-29 01:27:31.000000 honeybee-idaice-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-29 01:26:18.000000 honeybee-idaice-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3962 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/geometry_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20423 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    15400 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-29 01:44:26.000000 honeybee-idaice-0.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-29 01:42:57.000000 honeybee-idaice-0.2.1/setup.py
```

### Comparing `honeybee-idaice-0.2.0/LICENSE` & `honeybee-idaice-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/PKG-INFO` & `honeybee-idaice-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.2.0
+Version: 0.2.1
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.2.0/README.md` & `honeybee-idaice-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/archive.py` & `honeybee-idaice-0.2.1/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.2.1/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/geometry_utils.py` & `honeybee-idaice-0.2.1/honeybee_idaice/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.2.1/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.2.1/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.2.1/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.2.1/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.2.1/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.2.1/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/writer.py` & `honeybee-idaice-0.2.1/honeybee_idaice/writer.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,16 +156,16 @@
     origin = vertices[0]
 
     # relative coordinates of the pole
     rp = pole - origin
     # arbitrary x and y size for lighting fixtures
     lighting_x = 0.5
     lighting_y = 0.5
-    min_x = rp.x - lighting_x
-    min_y = rp.y - lighting_y
+    min_x = rp.x - lighting_x / 2
+    min_y = rp.y - lighting_y / 2
     # set the location of light and occupant
     light_occ = '((LIGHT :N "Light" :T LIGHT)\n' \
         f' (:PAR :N X :V {min_x})\n' \
         f' (:PAR :N Y :V {min_y})\n' \
         f' (:PAR :N DX :V {lighting_x})\n' \
         f' (:PAR :N DY :V {lighting_y})\n' \
         ' (:PAR :N RATED_INPUT :V 50.0)\n' \
```

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.2.1/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.2.1/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.2.0
+Version: 0.2.1
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.2.0/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.2.1/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.2.0/setup.py` & `honeybee-idaice-0.2.1/setup.py`

 * *Files identical despite different names*


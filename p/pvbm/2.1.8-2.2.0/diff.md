# Comparing `tmp/pvbm-2.1.8.tar.gz` & `tmp/pvbm-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvbm-2.1.8.tar", last modified: Wed May 24 15:48:25 2023, max compression
+gzip compressed data, was "pvbm-2.2.0.tar", last modified: Mon May 29 01:29:03 2023, max compression
```

## Comparing `pvbm-2.1.8.tar` & `pvbm-2.2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:48:25.403873 pvbm-2.1.8/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-05-24 15:48:25.403738 pvbm-2.1.8/PKG-INFO
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:48:25.401662 pvbm-2.1.8/PVBM/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)    11109 2023-05-17 16:00:48.000000 pvbm-2.1.8/PVBM/FractalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4883 2023-05-24 15:47:18.000000 pvbm-2.1.8/PVBM/GeometricalAnalysis.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.8/PVBM/__init__.py
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:48:25.402810 pvbm-2.1.8/PVBM/helpers/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.1.8/PVBM/helpers/__init__.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     5391 2023-04-15 11:00:40.000000 pvbm-2.1.8/PVBM/helpers/branching2.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     6285 2023-05-17 15:55:49.000000 pvbm-2.1.8/PVBM/helpers/branching_angle.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     1209 2023-05-24 15:27:09.000000 pvbm-2.1.8/PVBM/helpers/perimeter.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-2.1.8/PVBM/helpers/tortuosity.py
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     3778 2023-05-17 15:59:09.000000 pvbm-2.1.8/README.md
-drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-24 15:48:25.403553 pvbm-2.1.8/pvbm.egg-info/
--rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-05-24 15:48:25.000000 pvbm-2.1.8/pvbm.egg-info/PKG-INFO
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      363 2023-05-24 15:48:25.000000 pvbm-2.1.8/pvbm.egg-info/SOURCES.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-24 15:48:25.000000 pvbm-2.1.8/pvbm.egg-info/dependency_links.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-24 15:48:25.000000 pvbm-2.1.8/pvbm.egg-info/requires.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-24 15:48:25.000000 pvbm-2.1.8/pvbm.egg-info/top_level.txt
--rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-24 15:48:25.403913 pvbm-2.1.8/setup.cfg
--rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-24 15:48:22.000000 pvbm-2.1.8/setup.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-29 01:29:03.166965 pvbm-2.2.0/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-05-29 01:29:03.166840 pvbm-2.2.0/PKG-INFO
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-29 01:29:03.164689 pvbm-2.2.0/PVBM/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)    11109 2023-05-17 16:00:48.000000 pvbm-2.2.0/PVBM/FractalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4883 2023-05-24 15:47:18.000000 pvbm-2.2.0/PVBM/GeometricalAnalysis.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.2.0/PVBM/__init__.py
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-29 01:29:03.165854 pvbm-2.2.0/PVBM/helpers/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-04 16:40:03.000000 pvbm-2.2.0/PVBM/helpers/__init__.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     5403 2023-05-29 01:28:32.000000 pvbm-2.2.0/PVBM/helpers/branching2.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     6285 2023-05-17 15:55:49.000000 pvbm-2.2.0/PVBM/helpers/branching_angle.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     1209 2023-05-24 15:27:09.000000 pvbm-2.2.0/PVBM/helpers/perimeter.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     2265 2023-04-13 10:18:09.000000 pvbm-2.2.0/PVBM/helpers/tortuosity.py
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     3778 2023-05-17 15:59:09.000000 pvbm-2.2.0/README.md
+drwxr-xr-x   0 jonathanfhima   (501) staff       (20)        0 2023-05-29 01:29:03.166658 pvbm-2.2.0/pvbm.egg-info/
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)     4040 2023-05-29 01:29:03.000000 pvbm-2.2.0/pvbm.egg-info/PKG-INFO
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      363 2023-05-29 01:29:03.000000 pvbm-2.2.0/pvbm.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        1 2023-05-29 01:29:03.000000 pvbm-2.2.0/pvbm.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       32 2023-05-29 01:29:03.000000 pvbm-2.2.0/pvbm.egg-info/requires.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)        5 2023-05-29 01:29:03.000000 pvbm-2.2.0/pvbm.egg-info/top_level.txt
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)       38 2023-05-29 01:29:03.167006 pvbm-2.2.0/setup.cfg
+-rw-r--r--   0 jonathanfhima   (501) staff       (20)      696 2023-05-29 01:28:08.000000 pvbm-2.2.0/setup.py
```

### Comparing `pvbm-2.1.8/PKG-INFO` & `pvbm-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.1.8
+Version: 2.2.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.1.8/PVBM/FractalAnalysis.py` & `pvbm-2.2.0/PVBM/FractalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.8/PVBM/GeometricalAnalysis.py` & `pvbm-2.2.0/PVBM/GeometricalAnalysis.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.8/PVBM/helpers/branching2.py` & `pvbm-2.2.0/PVBM/helpers/branching2.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         if skeleton[down_left[0]][down_left[1]] ==1:      
             if down_left in all_important_index or dist == max_size:
                 connected[(i_or,j_or)] = connected.get((i_or,j_or),[]) + [down_left]
                 
             else : 
                 recursive(i_or,j_or,skeleton,down_left[0],down_left[1],visited,all_important_index,connected,dist+1 , plot = plot)
                 
-    if down_right[0] < len(skeleton) and down_right[1] >=0 and visited[down_right] ==0:
+    if down_right[0] < len(skeleton) and down_right[1] < len(skeleton) and visited[down_right] ==0:
         visited[down_right] = 1
         if skeleton[down_right[0]][down_right[1]] ==1:            
             if dist == max_size:
                 connected[(i_or,j_or)] = connected.get((i_or,j_or),[]) + [down_right]
                 
             else : 
                 recursive(i_or,j_or,skeleton,down_right[0],down_right[1],visited,all_important_index,connected,dist+1, plot = plot)
```

### Comparing `pvbm-2.1.8/PVBM/helpers/branching_angle.py` & `pvbm-2.2.0/PVBM/helpers/branching_angle.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.8/PVBM/helpers/perimeter.py` & `pvbm-2.2.0/PVBM/helpers/perimeter.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.8/PVBM/helpers/tortuosity.py` & `pvbm-2.2.0/PVBM/helpers/tortuosity.py`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.8/README.md` & `pvbm-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pvbm-2.1.8/pvbm.egg-info/PKG-INFO` & `pvbm-2.2.0/pvbm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvbm
-Version: 2.1.8
+Version: 2.2.0
 Summary: Python Vasculature Biomarker toolbox
 Home-page: https://github.com/aim-lab/PVBM
 Author: Jonathan Fhima, Yevgeniy Men
 Author-email: jonathanfh@campus.technion.ac.il
 Description-Content-Type: text/markdown
 
 # Python Vasculature BioMarker toolbox documentation
```

### Comparing `pvbm-2.1.8/setup.py` & `pvbm-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
         return file.read()
 
 long_description = read_readme("README.md")
 
 
 setup(
     name='pvbm',
-    version='2.1.8',
+    version='2.2.0',
     packages=find_packages(),
     install_requires=[
         "numpy",
         "scipy",
         "scikit-image",
         "pillow"
```


# Comparing `tmp/radvis-0.1.2.tar.gz` & `tmp/radvis-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radvis-0.1.2.tar", last modified: Mon May 29 00:57:25 2023, max compression
+gzip compressed data, was "radvis-0.1.3.tar", last modified: Mon May 29 02:24:25 2023, max compression
```

## Comparing `radvis-0.1.2.tar` & `radvis-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.426522 radvis-0.1.2/
--rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2512 2023-05-29 00:57:25.425516 radvis-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2209 2023-05-13 14:36:03.000000 radvis-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.390170 radvis-0.1.2/radvis/
--rw-rw-rw-   0        0        0      339 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.406499 radvis-0.1.2/radvis/image/
--rw-rw-rw-   0        0        0       56 2023-04-23 13:31:34.000000 radvis-0.1.2/radvis/image/__init__.py
--rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.1.2/radvis/image/load.py
--rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.1.2/radvis/image/rad_dicom_image.py
--rw-rw-rw-   0        0        0     3603 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/image/rad_image.py
--rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/image/rad_nifti_image.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.409498 radvis-0.1.2/radvis/mesh/
--rw-rw-rw-   0        0        0      115 2023-04-23 03:21:29.000000 radvis-0.1.2/radvis/mesh/__init__.py
--rw-rw-rw-   0        0        0     1638 2023-05-09 03:22:52.000000 radvis-0.1.2/radvis/mesh/compute_mesh.py
--rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.1.2/radvis/mesh/rad_mesh.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.413498 radvis-0.1.2/radvis/process/
--rw-rw-rw-   0        0        0      167 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/process/__init__.py
--rw-rw-rw-   0        0        0     2401 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/process/filtering.py
--rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/process/registration.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.417008 radvis-0.1.2/radvis/visualize/
--rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/visualize/__init__.py
--rw-rw-rw-   0        0        0     8860 2023-05-29 00:55:04.000000 radvis-0.1.2/radvis/visualize/rad_slicer.py
--rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/visualize/rad_slicer_group.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.401195 radvis-0.1.2/radvis.egg-info/
--rw-rw-rw-   0        0        0     2512 2023-05-29 00:57:25.000000 radvis-0.1.2/radvis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-05-29 00:57:25.000000 radvis-0.1.2/radvis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 00:57:25.000000 radvis-0.1.2/radvis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-29 00:57:25.000000 radvis-0.1.2/radvis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-29 00:57:25.000000 radvis-0.1.2/radvis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 00:57:25.426522 radvis-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-05-29 00:57:21.000000 radvis-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.418007 radvis-0.1.2/tests/
--rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.1.2/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.420009 radvis-0.1.2/tests/mocks/
--rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.1.2/tests/mocks/__init__.py
--rw-rw-rw-   0        0        0      281 2023-05-09 03:12:06.000000 radvis-0.1.2/tests/mocks/mock_rad_image.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.422007 radvis-0.1.2/tests/test_mesh/
--rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.1.2/tests/test_mesh/__init__.py
--rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.1.2/tests/test_mesh/test_compute_mesh.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.425008 radvis-0.1.2/tests/test_visualize/
--rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.1.2/tests/test_visualize/__init__.py
--rw-rw-rw-   0        0        0      924 2023-05-09 03:13:53.000000 radvis-0.1.2/tests/test_visualize/test_rad_slicer.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.342868 radvis-0.1.3/
+-rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2512 2023-05-29 02:24:25.341868 radvis-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2209 2023-05-13 14:36:03.000000 radvis-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.298027 radvis-0.1.3/radvis/
+-rw-rw-rw-   0        0        0      361 2023-05-29 02:23:43.000000 radvis-0.1.3/radvis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.321141 radvis-0.1.3/radvis/image/
+-rw-rw-rw-   0        0        0       78 2023-05-29 02:23:29.000000 radvis-0.1.3/radvis/image/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.1.3/radvis/image/load.py
+-rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.1.3/radvis/image/rad_dicom_image.py
+-rw-rw-rw-   0        0        0     3603 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/image/rad_image.py
+-rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/image/rad_nifti_image.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.324143 radvis-0.1.3/radvis/mesh/
+-rw-rw-rw-   0        0        0      115 2023-04-23 03:21:29.000000 radvis-0.1.3/radvis/mesh/__init__.py
+-rw-rw-rw-   0        0        0     1638 2023-05-09 03:22:52.000000 radvis-0.1.3/radvis/mesh/compute_mesh.py
+-rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.1.3/radvis/mesh/rad_mesh.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.328359 radvis-0.1.3/radvis/process/
+-rw-rw-rw-   0        0        0      167 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/process/__init__.py
+-rw-rw-rw-   0        0        0     2401 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/process/filtering.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/process/registration.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.332360 radvis-0.1.3/radvis/visualize/
+-rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/visualize/__init__.py
+-rw-rw-rw-   0        0        0     8860 2023-05-29 00:55:04.000000 radvis-0.1.3/radvis/visualize/rad_slicer.py
+-rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/visualize/rad_slicer_group.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.314101 radvis-0.1.3/radvis.egg-info/
+-rw-rw-rw-   0        0        0     2512 2023-05-29 02:24:24.000000 radvis-0.1.3/radvis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-05-29 02:24:25.000000 radvis-0.1.3/radvis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 02:24:24.000000 radvis-0.1.3/radvis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-29 02:24:24.000000 radvis-0.1.3/radvis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 02:24:24.000000 radvis-0.1.3/radvis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 02:24:25.342868 radvis-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-05-29 02:24:10.000000 radvis-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.333353 radvis-0.1.3/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.1.3/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.335869 radvis-0.1.3/tests/mocks/
+-rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.1.3/tests/mocks/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-05-09 03:12:06.000000 radvis-0.1.3/tests/mocks/mock_rad_image.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.337873 radvis-0.1.3/tests/test_mesh/
+-rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.1.3/tests/test_mesh/__init__.py
+-rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.1.3/tests/test_mesh/test_compute_mesh.py
+drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.340873 radvis-0.1.3/tests/test_visualize/
+-rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.1.3/tests/test_visualize/__init__.py
+-rw-rw-rw-   0        0        0      924 2023-05-09 03:13:53.000000 radvis-0.1.3/tests/test_visualize/test_rad_slicer.py
```

### Comparing `radvis-0.1.2/LICENSE` & `radvis-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/PKG-INFO` & `radvis-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radvis
-Version: 0.1.2
+Version: 0.1.3
 Summary: A visualization tool for medical images
 Home-page: https://github.com/medlee-code/RadVis
 Author: Matthew lee
 Author-email: matthewlee@medlee.io
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `radvis-0.1.2/README.md` & `radvis-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/radvis/image/load.py` & `radvis-0.1.3/radvis/image/load.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/radvis/image/rad_dicom_image.py` & `radvis-0.1.3/radvis/image/rad_dicom_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/radvis/image/rad_image.py` & `radvis-0.1.3/radvis/image/rad_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/radvis/image/rad_nifti_image.py` & `radvis-0.1.3/radvis/image/rad_nifti_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/radvis/mesh/compute_mesh.py` & `radvis-0.1.3/radvis/mesh/compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/radvis/mesh/rad_mesh.py` & `radvis-0.1.3/radvis/mesh/rad_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/radvis/process/filtering.py` & `radvis-0.1.3/radvis/process/filtering.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/radvis/visualize/rad_slicer.py` & `radvis-0.1.3/radvis/visualize/rad_slicer.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/radvis/visualize/rad_slicer_group.py` & `radvis-0.1.3/radvis/visualize/rad_slicer_group.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/radvis.egg-info/PKG-INFO` & `radvis-0.1.3/radvis.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radvis
-Version: 0.1.2
+Version: 0.1.3
 Summary: A visualization tool for medical images
 Home-page: https://github.com/medlee-code/RadVis
 Author: Matthew lee
 Author-email: matthewlee@medlee.io
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `radvis-0.1.2/radvis.egg-info/SOURCES.txt` & `radvis-0.1.3/radvis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/setup.py` & `radvis-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='radvis',
-    version='0.1.2',
+    version='0.1.3',
     url='https://github.com/medlee-code/RadVis',
     author='Matthew lee',
     author_email='matthewlee@medlee.io',
     description='A visualization tool for medical images',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `radvis-0.1.2/tests/test_mesh/test_compute_mesh.py` & `radvis-0.1.3/tests/test_mesh/test_compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.2/tests/test_visualize/test_rad_slicer.py` & `radvis-0.1.3/tests/test_visualize/test_rad_slicer.py`

 * *Files identical despite different names*


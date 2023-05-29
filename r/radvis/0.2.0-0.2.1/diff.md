# Comparing `tmp/radvis-0.2.0.tar.gz` & `tmp/radvis-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radvis-0.2.0.tar", last modified: Mon May 29 03:08:11 2023, max compression
+gzip compressed data, was "radvis-0.2.1.tar", last modified: Mon May 29 03:21:46 2023, max compression
```

## Comparing `radvis-0.2.0.tar` & `radvis-0.2.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.627532 radvis-0.2.0/
--rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     4225 2023-05-29 03:08:11.627532 radvis-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3922 2023-05-29 03:06:20.000000 radvis-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.579346 radvis-0.2.0/radvis/
--rw-rw-rw-   0        0        0      344 2023-05-29 02:55:24.000000 radvis-0.2.0/radvis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.604383 radvis-0.2.0/radvis/image/
--rw-rw-rw-   0        0        0       78 2023-05-29 02:23:29.000000 radvis-0.2.0/radvis/image/__init__.py
--rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.2.0/radvis/image/load.py
--rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.2.0/radvis/image/rad_dicom_image.py
--rw-rw-rw-   0        0        0     3673 2023-05-29 02:54:49.000000 radvis-0.2.0/radvis/image/rad_image.py
--rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.2.0/radvis/image/rad_nifti_image.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.607383 radvis-0.2.0/radvis/mesh/
--rw-rw-rw-   0        0        0      130 2023-05-29 03:00:11.000000 radvis-0.2.0/radvis/mesh/__init__.py
--rw-rw-rw-   0        0        0     1618 2023-05-29 03:00:19.000000 radvis-0.2.0/radvis/mesh/compute_mesh.py
--rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.2.0/radvis/mesh/rad_mesh.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.610543 radvis-0.2.0/radvis/processing/
--rw-rw-rw-   0        0        0      143 2023-05-29 03:00:30.000000 radvis-0.2.0/radvis/processing/__init__.py
--rw-rw-rw-   0        0        0     3165 2023-05-29 03:04:44.000000 radvis-0.2.0/radvis/processing/image.py
--rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.2.0/radvis/processing/registration.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.614549 radvis-0.2.0/radvis/visualize/
--rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.2.0/radvis/visualize/__init__.py
--rw-rw-rw-   0        0        0     8860 2023-05-29 00:55:04.000000 radvis-0.2.0/radvis/visualize/rad_slicer.py
--rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.2.0/radvis/visualize/rad_slicer_group.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.598383 radvis-0.2.0/radvis.egg-info/
--rw-rw-rw-   0        0        0     4225 2023-05-29 03:08:11.000000 radvis-0.2.0/radvis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      874 2023-05-29 03:08:11.000000 radvis-0.2.0/radvis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 03:08:11.000000 radvis-0.2.0/radvis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-29 03:08:11.000000 radvis-0.2.0/radvis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-29 03:08:11.000000 radvis-0.2.0/radvis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 03:08:11.627532 radvis-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-05-29 03:07:05.000000 radvis-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.615543 radvis-0.2.0/tests/
--rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.2.0/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.617544 radvis-0.2.0/tests/mocks/
--rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.2.0/tests/mocks/__init__.py
--rw-rw-rw-   0        0        0      455 2023-05-29 02:42:01.000000 radvis-0.2.0/tests/mocks/mock_rad_image.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.619869 radvis-0.2.0/tests/test_mesh/
--rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.2.0/tests/test_mesh/__init__.py
--rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.2.0/tests/test_mesh/test_compute_mesh.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.623874 radvis-0.2.0/tests/test_processing/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:40:16.000000 radvis-0.2.0/tests/test_processing/__init__.py
--rw-rw-rw-   0        0        0     1645 2023-05-29 02:59:47.000000 radvis-0.2.0/tests/test_processing/test_image.py
-drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.626021 radvis-0.2.0/tests/test_visualize/
--rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.2.0/tests/test_visualize/__init__.py
--rw-rw-rw-   0        0        0      837 2023-05-29 02:59:35.000000 radvis-0.2.0/tests/test_visualize/test_rad_slicer.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.765209 radvis-0.2.1/
+-rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4225 2023-05-29 03:21:46.764210 radvis-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3922 2023-05-29 03:06:20.000000 radvis-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.701792 radvis-0.2.1/radvis/
+-rw-rw-rw-   0        0        0      372 2023-05-29 03:20:53.000000 radvis-0.2.1/radvis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.723088 radvis-0.2.1/radvis/image/
+-rw-rw-rw-   0        0        0       78 2023-05-29 02:23:29.000000 radvis-0.2.1/radvis/image/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.2.1/radvis/image/load.py
+-rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.2.1/radvis/image/rad_dicom_image.py
+-rw-rw-rw-   0        0        0     3673 2023-05-29 02:54:49.000000 radvis-0.2.1/radvis/image/rad_image.py
+-rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.2.1/radvis/image/rad_nifti_image.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.731607 radvis-0.2.1/radvis/mesh/
+-rw-rw-rw-   0        0        0      130 2023-05-29 03:00:11.000000 radvis-0.2.1/radvis/mesh/__init__.py
+-rw-rw-rw-   0        0        0     1618 2023-05-29 03:00:19.000000 radvis-0.2.1/radvis/mesh/compute_mesh.py
+-rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.2.1/radvis/mesh/rad_mesh.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.744114 radvis-0.2.1/radvis/processing/
+-rw-rw-rw-   0        0        0      171 2023-05-29 03:20:54.000000 radvis-0.2.1/radvis/processing/__init__.py
+-rw-rw-rw-   0        0        0     3165 2023-05-29 03:04:44.000000 radvis-0.2.1/radvis/processing/image.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.2.1/radvis/processing/registration.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.749114 radvis-0.2.1/radvis/visualize/
+-rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.2.1/radvis/visualize/__init__.py
+-rw-rw-rw-   0        0        0     8860 2023-05-29 00:55:04.000000 radvis-0.2.1/radvis/visualize/rad_slicer.py
+-rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.2.1/radvis/visualize/rad_slicer_group.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.715888 radvis-0.2.1/radvis.egg-info/
+-rw-rw-rw-   0        0        0     4225 2023-05-29 03:21:46.000000 radvis-0.2.1/radvis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      874 2023-05-29 03:21:46.000000 radvis-0.2.1/radvis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 03:21:46.000000 radvis-0.2.1/radvis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-29 03:21:46.000000 radvis-0.2.1/radvis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 03:21:46.000000 radvis-0.2.1/radvis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 03:21:46.765209 radvis-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-05-29 03:21:14.000000 radvis-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.750176 radvis-0.2.1/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.2.1/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.753182 radvis-0.2.1/tests/mocks/
+-rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.2.1/tests/mocks/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-05-29 02:42:01.000000 radvis-0.2.1/tests/mocks/mock_rad_image.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.755693 radvis-0.2.1/tests/test_mesh/
+-rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.2.1/tests/test_mesh/__init__.py
+-rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.2.1/tests/test_mesh/test_compute_mesh.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.759203 radvis-0.2.1/tests/test_processing/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:40:16.000000 radvis-0.2.1/tests/test_processing/__init__.py
+-rw-rw-rw-   0        0        0     1645 2023-05-29 02:59:47.000000 radvis-0.2.1/tests/test_processing/test_image.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:21:46.763209 radvis-0.2.1/tests/test_visualize/
+-rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.2.1/tests/test_visualize/__init__.py
+-rw-rw-rw-   0        0        0      837 2023-05-29 02:59:35.000000 radvis-0.2.1/tests/test_visualize/test_rad_slicer.py
```

### Comparing `radvis-0.2.0/LICENSE` & `radvis-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/PKG-INFO` & `radvis-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radvis
-Version: 0.2.0
+Version: 0.2.1
 Summary: A visualization tool for medical images
 Home-page: https://github.com/medlee-code/RadVis
 Author: Matthew lee
 Author-email: matthewlee@medlee.io
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `radvis-0.2.0/README.md` & `radvis-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/radvis/image/load.py` & `radvis-0.2.1/radvis/image/load.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/radvis/image/rad_dicom_image.py` & `radvis-0.2.1/radvis/image/rad_dicom_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/radvis/image/rad_image.py` & `radvis-0.2.1/radvis/image/rad_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/radvis/image/rad_nifti_image.py` & `radvis-0.2.1/radvis/image/rad_nifti_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/radvis/mesh/compute_mesh.py` & `radvis-0.2.1/radvis/mesh/compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/radvis/mesh/rad_mesh.py` & `radvis-0.2.1/radvis/mesh/rad_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/radvis/processing/image.py` & `radvis-0.2.1/radvis/processing/image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/radvis/visualize/rad_slicer.py` & `radvis-0.2.1/radvis/visualize/rad_slicer.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/radvis/visualize/rad_slicer_group.py` & `radvis-0.2.1/radvis/visualize/rad_slicer_group.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/radvis.egg-info/PKG-INFO` & `radvis-0.2.1/radvis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radvis
-Version: 0.2.0
+Version: 0.2.1
 Summary: A visualization tool for medical images
 Home-page: https://github.com/medlee-code/RadVis
 Author: Matthew lee
 Author-email: matthewlee@medlee.io
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `radvis-0.2.0/radvis.egg-info/SOURCES.txt` & `radvis-0.2.1/radvis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/setup.py` & `radvis-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='radvis',
-    version='0.2.0',
+    version='0.2.1',
     url='https://github.com/medlee-code/RadVis',
     author='Matthew lee',
     author_email='matthewlee@medlee.io',
     description='A visualization tool for medical images',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `radvis-0.2.0/tests/test_mesh/test_compute_mesh.py` & `radvis-0.2.1/tests/test_mesh/test_compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/tests/test_processing/test_image.py` & `radvis-0.2.1/tests/test_processing/test_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.2.0/tests/test_visualize/test_rad_slicer.py` & `radvis-0.2.1/tests/test_visualize/test_rad_slicer.py`

 * *Files identical despite different names*


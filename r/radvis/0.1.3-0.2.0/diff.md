# Comparing `tmp/radvis-0.1.3.tar.gz` & `tmp/radvis-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radvis-0.1.3.tar", last modified: Mon May 29 02:24:25 2023, max compression
+gzip compressed data, was "radvis-0.2.0.tar", last modified: Mon May 29 03:08:11 2023, max compression
```

## Comparing `radvis-0.1.3.tar` & `radvis-0.2.0.tar`

### file list

```diff
@@ -1,43 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.342868 radvis-0.1.3/
--rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     2512 2023-05-29 02:24:25.341868 radvis-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     2209 2023-05-13 14:36:03.000000 radvis-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.298027 radvis-0.1.3/radvis/
--rw-rw-rw-   0        0        0      361 2023-05-29 02:23:43.000000 radvis-0.1.3/radvis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.321141 radvis-0.1.3/radvis/image/
--rw-rw-rw-   0        0        0       78 2023-05-29 02:23:29.000000 radvis-0.1.3/radvis/image/__init__.py
--rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.1.3/radvis/image/load.py
--rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.1.3/radvis/image/rad_dicom_image.py
--rw-rw-rw-   0        0        0     3603 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/image/rad_image.py
--rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/image/rad_nifti_image.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.324143 radvis-0.1.3/radvis/mesh/
--rw-rw-rw-   0        0        0      115 2023-04-23 03:21:29.000000 radvis-0.1.3/radvis/mesh/__init__.py
--rw-rw-rw-   0        0        0     1638 2023-05-09 03:22:52.000000 radvis-0.1.3/radvis/mesh/compute_mesh.py
--rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.1.3/radvis/mesh/rad_mesh.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.328359 radvis-0.1.3/radvis/process/
--rw-rw-rw-   0        0        0      167 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/process/__init__.py
--rw-rw-rw-   0        0        0     2401 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/process/filtering.py
--rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/process/registration.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.332360 radvis-0.1.3/radvis/visualize/
--rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/visualize/__init__.py
--rw-rw-rw-   0        0        0     8860 2023-05-29 00:55:04.000000 radvis-0.1.3/radvis/visualize/rad_slicer.py
--rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.1.3/radvis/visualize/rad_slicer_group.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.314101 radvis-0.1.3/radvis.egg-info/
--rw-rw-rw-   0        0        0     2512 2023-05-29 02:24:24.000000 radvis-0.1.3/radvis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-05-29 02:24:25.000000 radvis-0.1.3/radvis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 02:24:24.000000 radvis-0.1.3/radvis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       69 2023-05-29 02:24:24.000000 radvis-0.1.3/radvis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-29 02:24:24.000000 radvis-0.1.3/radvis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 02:24:25.342868 radvis-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      669 2023-05-29 02:24:10.000000 radvis-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.333353 radvis-0.1.3/tests/
--rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.1.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.335869 radvis-0.1.3/tests/mocks/
--rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.1.3/tests/mocks/__init__.py
--rw-rw-rw-   0        0        0      281 2023-05-09 03:12:06.000000 radvis-0.1.3/tests/mocks/mock_rad_image.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.337873 radvis-0.1.3/tests/test_mesh/
--rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.1.3/tests/test_mesh/__init__.py
--rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.1.3/tests/test_mesh/test_compute_mesh.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:24:25.340873 radvis-0.1.3/tests/test_visualize/
--rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.1.3/tests/test_visualize/__init__.py
--rw-rw-rw-   0        0        0      924 2023-05-09 03:13:53.000000 radvis-0.1.3/tests/test_visualize/test_rad_slicer.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.627532 radvis-0.2.0/
+-rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     4225 2023-05-29 03:08:11.627532 radvis-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3922 2023-05-29 03:06:20.000000 radvis-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.579346 radvis-0.2.0/radvis/
+-rw-rw-rw-   0        0        0      344 2023-05-29 02:55:24.000000 radvis-0.2.0/radvis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.604383 radvis-0.2.0/radvis/image/
+-rw-rw-rw-   0        0        0       78 2023-05-29 02:23:29.000000 radvis-0.2.0/radvis/image/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.2.0/radvis/image/load.py
+-rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.2.0/radvis/image/rad_dicom_image.py
+-rw-rw-rw-   0        0        0     3673 2023-05-29 02:54:49.000000 radvis-0.2.0/radvis/image/rad_image.py
+-rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.2.0/radvis/image/rad_nifti_image.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.607383 radvis-0.2.0/radvis/mesh/
+-rw-rw-rw-   0        0        0      130 2023-05-29 03:00:11.000000 radvis-0.2.0/radvis/mesh/__init__.py
+-rw-rw-rw-   0        0        0     1618 2023-05-29 03:00:19.000000 radvis-0.2.0/radvis/mesh/compute_mesh.py
+-rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.2.0/radvis/mesh/rad_mesh.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.610543 radvis-0.2.0/radvis/processing/
+-rw-rw-rw-   0        0        0      143 2023-05-29 03:00:30.000000 radvis-0.2.0/radvis/processing/__init__.py
+-rw-rw-rw-   0        0        0     3165 2023-05-29 03:04:44.000000 radvis-0.2.0/radvis/processing/image.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.2.0/radvis/processing/registration.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.614549 radvis-0.2.0/radvis/visualize/
+-rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.2.0/radvis/visualize/__init__.py
+-rw-rw-rw-   0        0        0     8860 2023-05-29 00:55:04.000000 radvis-0.2.0/radvis/visualize/rad_slicer.py
+-rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.2.0/radvis/visualize/rad_slicer_group.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.598383 radvis-0.2.0/radvis.egg-info/
+-rw-rw-rw-   0        0        0     4225 2023-05-29 03:08:11.000000 radvis-0.2.0/radvis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      874 2023-05-29 03:08:11.000000 radvis-0.2.0/radvis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 03:08:11.000000 radvis-0.2.0/radvis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-29 03:08:11.000000 radvis-0.2.0/radvis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 03:08:11.000000 radvis-0.2.0/radvis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 03:08:11.627532 radvis-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-05-29 03:07:05.000000 radvis-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.615543 radvis-0.2.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.2.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.617544 radvis-0.2.0/tests/mocks/
+-rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.2.0/tests/mocks/__init__.py
+-rw-rw-rw-   0        0        0      455 2023-05-29 02:42:01.000000 radvis-0.2.0/tests/mocks/mock_rad_image.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.619869 radvis-0.2.0/tests/test_mesh/
+-rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.2.0/tests/test_mesh/__init__.py
+-rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.2.0/tests/test_mesh/test_compute_mesh.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.623874 radvis-0.2.0/tests/test_processing/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:40:16.000000 radvis-0.2.0/tests/test_processing/__init__.py
+-rw-rw-rw-   0        0        0     1645 2023-05-29 02:59:47.000000 radvis-0.2.0/tests/test_processing/test_image.py
+drwxrwxrwx   0        0        0        0 2023-05-29 03:08:11.626021 radvis-0.2.0/tests/test_visualize/
+-rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.2.0/tests/test_visualize/__init__.py
+-rw-rw-rw-   0        0        0      837 2023-05-29 02:59:35.000000 radvis-0.2.0/tests/test_visualize/test_rad_slicer.py
```

### Comparing `radvis-0.1.3/LICENSE` & `radvis-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `radvis-0.1.3/radvis/image/load.py` & `radvis-0.2.0/radvis/image/load.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.3/radvis/image/rad_dicom_image.py` & `radvis-0.2.0/radvis/image/rad_dicom_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.3/radvis/image/rad_image.py` & `radvis-0.2.0/radvis/image/rad_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,26 +8,24 @@
         """
         Initialize the RadImage base class.
 
         :param file_path: The file path to the image file, defaults to None
         """
         self.file_path = file_path
         self.data = None
-        self.image_data: Optional[np.ndarray] = None
-        self.metadata = None
+        self.image_data: np.ndarray = np.array([])
+        self.metadata:dict = {}
         if self.file_path:
             self.load()
 
     @property
     def shape(self) -> tuple:
         """
         Return the shape of the image data.
         """
-        if self.image_data is None:
-            return None
         return self.image_data.shape
 
     @abstractmethod
     def load(self) -> None:
         """
         Load the image from the file path. This method should be implemented
         by subclasses to handle specific image formats.
@@ -82,28 +80,34 @@
             raise ValueError(f"Index {index} is out of bounds for axis {axis}")
 
         # Slice along the appropriate axis
         slicer = [slice(None)] * self.image_data.ndim
         slicer[axis] = index
         return self.image_data[tuple(slicer)]
     
-    def copy(self):
+    def copy(self) -> 'RadImage':
         """ 
         Return a copy of the image.
         """
         new_image = self.__class__(self.file_path)
         new_image.data = self.data
-        new_image.image_data = np.copy(self.image_data)
-        new_image.metadata = self.metadata.copy() if self.metadata else None
+
+        if self.image_data is not None:
+            new_image.image_data = np.copy(self.image_data)
+
+        new_image.metadata = self.metadata.copy()
         return new_image
 
     def __recv__(self) -> str:
         """
         Return a string representation of the image data.
         """
         return self.get_image_info()
     
-    def __getitem__(self, value:list) -> np.ndarray:
+    def __getitem__(self, value:list) -> Optional[np.ndarray]:
         """
         Return the image data at the given index.
         """
-        return self.image_data[value]
+        if self.image_data is not None:
+            return self.image_data[value]
+        else:
+            return None
```

### Comparing `radvis-0.1.3/radvis/image/rad_nifti_image.py` & `radvis-0.2.0/radvis/image/rad_nifti_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.3/radvis/mesh/compute_mesh.py` & `radvis-0.2.0/radvis/mesh/compute_mesh.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 Returns:
     A ResMesh object with the following attributes:
         vertices: A numpy array of shape (n, 3) containing the vertices of the mesh.
         faces: A numpy array of shape (m, 3) containing the faces of the mesh.
         normals: A numpy array of shape (n, 3) containing the normals of the mesh.
         values: A numpy array of shape (n,) containing the values of the mesh.
 """
-import numpy as np
 from skimage import measure
 from typing import Any, Dict
 from .rad_mesh import RadMesh    
 from radvis.image.rad_image import RadImage    
 
 def compute_marching_cubes(radimage: RadImage, threshold: float, **kwargs: Dict[str, Any]) -> RadMesh:
     """ Wrapper for skimage.measure.marching_cubes """
```

### Comparing `radvis-0.1.3/radvis/mesh/rad_mesh.py` & `radvis-0.2.0/radvis/mesh/rad_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.3/radvis/process/filtering.py` & `radvis-0.2.0/radvis/processing/image.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from radvis.image.rad_image import RadImage 
 import numpy as np
 from scipy.ndimage import gaussian_filter
 
 
-def intensity_normalization(rad_image: RadImage) -> RadImage:
+def normalization(rad_image: RadImage, min_val:float, max_val:float) -> RadImage:
     """
     Perform intensity normalization on a given RadImage.
     
     :param rad_image: The RadImage object to be normalized.
 
     :return: The normalized RadImage object.
 
     :raises ValueError: If image data is not loaded.
     """
     new_rad_image = rad_image.copy()
     if new_rad_image.image_data is None:
         raise ValueError("Image data not loaded")
 
-    new_rad_image.image_data = (new_rad_image.image_data - np.min(new_rad_image.image_data)) / (np.max(new_rad_image.image_data) - np.min(new_rad_image.image_data))
+    # Normalize the image data
+    new_rad_image.image_data = (new_rad_image.image_data - min_val) / (max_val - min_val)
     return new_rad_image
 
 def noise_reduction(rad_image: RadImage, sigma: float) -> RadImage:
     """
     Reduce noise in a given RadImage using Gaussian filtering.
     
     :param rad_image: The RadImage object to be processed.
@@ -56,8 +57,30 @@
 
     # Compute the lower and upper intensity values
     lower = np.percentile(new_rad_image.image_data, lower_percentile)
     upper = np.percentile(new_rad_image.image_data, upper_percentile)
 
     # Clip the image data
     new_rad_image.image_data = np.clip(new_rad_image.image_data, lower, upper)
+    return new_rad_image
+
+
+def add_padding(rad_image: RadImage, target_shape: tuple) -> RadImage:
+    """
+    Adds padding to either side of the image to match the expected shape.
+
+    :param rad_image: The RadImage object to be padded.
+    :param target_shape: The expected shape of the image.
+
+    :return: The RadImage object with padding added.
+    """
+    new_rad_image = rad_image.copy()
+    if new_rad_image.image_data is None:
+        raise ValueError("Image data not loaded")
+
+    # Compute the padding
+    padding = np.subtract(target_shape, new_rad_image.image_data.shape)
+    padding = np.array([padding // 2, padding - padding // 2]).T
+
+    # Pad the image data
+    new_rad_image.image_data = np.pad(new_rad_image.image_data, padding, mode='constant')
     return new_rad_image
```

### Comparing `radvis-0.1.3/radvis/visualize/rad_slicer.py` & `radvis-0.2.0/radvis/visualize/rad_slicer.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.3/radvis/visualize/rad_slicer_group.py` & `radvis-0.2.0/radvis/visualize/rad_slicer_group.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.3/radvis.egg-info/SOURCES.txt` & `radvis-0.2.0/radvis.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -11,20 +11,22 @@
 radvis/image/load.py
 radvis/image/rad_dicom_image.py
 radvis/image/rad_image.py
 radvis/image/rad_nifti_image.py
 radvis/mesh/__init__.py
 radvis/mesh/compute_mesh.py
 radvis/mesh/rad_mesh.py
-radvis/process/__init__.py
-radvis/process/filtering.py
-radvis/process/registration.py
+radvis/processing/__init__.py
+radvis/processing/image.py
+radvis/processing/registration.py
 radvis/visualize/__init__.py
 radvis/visualize/rad_slicer.py
 radvis/visualize/rad_slicer_group.py
 tests/__init__.py
 tests/mocks/__init__.py
 tests/mocks/mock_rad_image.py
 tests/test_mesh/__init__.py
 tests/test_mesh/test_compute_mesh.py
+tests/test_processing/__init__.py
+tests/test_processing/test_image.py
 tests/test_visualize/__init__.py
 tests/test_visualize/test_rad_slicer.py
```

### Comparing `radvis-0.1.3/setup.py` & `radvis-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='radvis',
-    version='0.1.3',
+    version='0.2.0',
     url='https://github.com/medlee-code/RadVis',
     author='Matthew lee',
     author_email='matthewlee@medlee.io',
     description='A visualization tool for medical images',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `radvis-0.1.3/tests/test_mesh/test_compute_mesh.py` & `radvis-0.2.0/tests/test_mesh/test_compute_mesh.py`

 * *Files identical despite different names*


# Comparing `tmp/radvis-0.1.1.tar.gz` & `tmp/radvis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radvis-0.1.1.tar", last modified: Sat May 13 14:33:47 2023, max compression
+gzip compressed data, was "radvis-0.1.2.tar", last modified: Mon May 29 00:57:25 2023, max compression
```

## Comparing `radvis-0.1.1.tar` & `radvis-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,43 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 14:33:47.521878 radvis-0.1.1/
--rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2513 2023-05-13 14:33:47.520878 radvis-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2210 2023-05-13 14:31:12.000000 radvis-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 14:33:47.497308 radvis-0.1.1/radvis/
--rw-rw-rw-   0        0        0      152 2023-05-09 04:13:22.000000 radvis-0.1.1/radvis/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:33:47.508823 radvis-0.1.1/radvis/image/
--rw-rw-rw-   0        0        0       56 2023-04-23 13:31:34.000000 radvis-0.1.1/radvis/image/__init__.py
--rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.1.1/radvis/image/load.py
--rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.1.1/radvis/image/rad_dicom_image.py
--rw-rw-rw-   0        0        0     3312 2023-05-13 13:23:44.000000 radvis-0.1.1/radvis/image/rad_image.py
--rw-rw-rw-   0        0        0     1375 2023-05-13 13:28:40.000000 radvis-0.1.1/radvis/image/rad_nifti_image.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:33:47.511824 radvis-0.1.1/radvis/mesh/
--rw-rw-rw-   0        0        0      115 2023-04-23 03:21:29.000000 radvis-0.1.1/radvis/mesh/__init__.py
--rw-rw-rw-   0        0        0     1638 2023-05-09 03:22:52.000000 radvis-0.1.1/radvis/mesh/compute_mesh.py
--rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.1.1/radvis/mesh/rad_mesh.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:33:47.513823 radvis-0.1.1/radvis/visualize/
--rw-rw-rw-   0        0        0       60 2023-04-29 06:26:05.000000 radvis-0.1.1/radvis/visualize/__init__.py
--rw-rw-rw-   0        0        0     6601 2023-05-13 13:56:23.000000 radvis-0.1.1/radvis/visualize/rad_slicer.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:33:47.504308 radvis-0.1.1/radvis.egg-info/
--rw-rw-rw-   0        0        0     2513 2023-05-13 14:33:47.000000 radvis-0.1.1/radvis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      676 2023-05-13 14:33:47.000000 radvis-0.1.1/radvis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 14:33:47.000000 radvis-0.1.1/radvis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      112 2023-05-13 14:33:47.000000 radvis-0.1.1/radvis.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-13 14:33:47.000000 radvis-0.1.1/radvis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-13 14:33:47.521878 radvis-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      748 2023-05-13 14:32:31.000000 radvis-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:33:47.514824 radvis-0.1.1/tests/
--rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.1.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:33:47.515823 radvis-0.1.1/tests/mocks/
--rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.1.1/tests/mocks/__init__.py
--rw-rw-rw-   0        0        0      281 2023-05-09 03:12:06.000000 radvis-0.1.1/tests/mocks/mock_rad_image.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:33:47.517879 radvis-0.1.1/tests/test_mesh/
--rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.1.1/tests/test_mesh/__init__.py
--rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.1.1/tests/test_mesh/test_compute_mesh.py
-drwxrwxrwx   0        0        0        0 2023-05-13 14:33:47.519878 radvis-0.1.1/tests/test_visualize/
--rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.1.1/tests/test_visualize/__init__.py
--rw-rw-rw-   0        0        0      924 2023-05-09 03:13:53.000000 radvis-0.1.1/tests/test_visualize/test_rad_slicer.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.426522 radvis-0.1.2/
+-rw-rw-rw-   0        0        0     1089 2023-04-22 03:52:40.000000 radvis-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2512 2023-05-29 00:57:25.425516 radvis-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2209 2023-05-13 14:36:03.000000 radvis-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.390170 radvis-0.1.2/radvis/
+-rw-rw-rw-   0        0        0      339 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.406499 radvis-0.1.2/radvis/image/
+-rw-rw-rw-   0        0        0       56 2023-04-23 13:31:34.000000 radvis-0.1.2/radvis/image/__init__.py
+-rw-rw-rw-   0        0        0      720 2023-04-23 13:36:03.000000 radvis-0.1.2/radvis/image/load.py
+-rw-rw-rw-   0        0        0     1345 2023-05-13 13:29:04.000000 radvis-0.1.2/radvis/image/rad_dicom_image.py
+-rw-rw-rw-   0        0        0     3603 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/image/rad_image.py
+-rw-rw-rw-   0        0        0     1408 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/image/rad_nifti_image.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.409498 radvis-0.1.2/radvis/mesh/
+-rw-rw-rw-   0        0        0      115 2023-04-23 03:21:29.000000 radvis-0.1.2/radvis/mesh/__init__.py
+-rw-rw-rw-   0        0        0     1638 2023-05-09 03:22:52.000000 radvis-0.1.2/radvis/mesh/compute_mesh.py
+-rw-rw-rw-   0        0        0     4074 2023-04-23 04:59:23.000000 radvis-0.1.2/radvis/mesh/rad_mesh.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.413498 radvis-0.1.2/radvis/process/
+-rw-rw-rw-   0        0        0      167 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/process/__init__.py
+-rw-rw-rw-   0        0        0     2401 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/process/filtering.py
+-rw-rw-rw-   0        0        0        0 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/process/registration.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.417008 radvis-0.1.2/radvis/visualize/
+-rw-rw-rw-   0        0        0      124 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/visualize/__init__.py
+-rw-rw-rw-   0        0        0     8860 2023-05-29 00:55:04.000000 radvis-0.1.2/radvis/visualize/rad_slicer.py
+-rw-rw-rw-   0        0        0     1857 2023-05-29 00:52:44.000000 radvis-0.1.2/radvis/visualize/rad_slicer_group.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.401195 radvis-0.1.2/radvis.egg-info/
+-rw-rw-rw-   0        0        0     2512 2023-05-29 00:57:25.000000 radvis-0.1.2/radvis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-05-29 00:57:25.000000 radvis-0.1.2/radvis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 00:57:25.000000 radvis-0.1.2/radvis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       69 2023-05-29 00:57:25.000000 radvis-0.1.2/radvis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-29 00:57:25.000000 radvis-0.1.2/radvis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 00:57:25.426522 radvis-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      669 2023-05-29 00:57:21.000000 radvis-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.418007 radvis-0.1.2/tests/
+-rw-rw-rw-   0        0        0        0 2023-04-22 04:25:04.000000 radvis-0.1.2/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.420009 radvis-0.1.2/tests/mocks/
+-rw-rw-rw-   0        0        0       40 2023-04-30 09:03:02.000000 radvis-0.1.2/tests/mocks/__init__.py
+-rw-rw-rw-   0        0        0      281 2023-05-09 03:12:06.000000 radvis-0.1.2/tests/mocks/mock_rad_image.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.422007 radvis-0.1.2/tests/test_mesh/
+-rw-rw-rw-   0        0        0        0 2023-04-23 02:35:32.000000 radvis-0.1.2/tests/test_mesh/__init__.py
+-rw-rw-rw-   0        0        0     2248 2023-05-09 03:23:13.000000 radvis-0.1.2/tests/test_mesh/test_compute_mesh.py
+drwxrwxrwx   0        0        0        0 2023-05-29 00:57:25.425008 radvis-0.1.2/tests/test_visualize/
+-rw-rw-rw-   0        0        0        0 2023-04-30 08:55:21.000000 radvis-0.1.2/tests/test_visualize/__init__.py
+-rw-rw-rw-   0        0        0      924 2023-05-09 03:13:53.000000 radvis-0.1.2/tests/test_visualize/test_rad_slicer.py
```

### Comparing `radvis-0.1.1/LICENSE` & `radvis-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `radvis-0.1.1/PKG-INFO` & `radvis-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radvis
-Version: 0.1.1
+Version: 0.1.2
 Summary: A visualization tool for medical images
 Home-page: https://github.com/medlee-code/RadVis
 Author: Matthew lee
 Author-email: matthewlee@medlee.io
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,15 +55,15 @@
 blue_mask[70:150, 70:150, 70:150] = 1
 
 slicer.add_mask(red_mask, color="red")
 slicer.add_mask(blue_mask, color="blue")
 
 slicer.display()
 ```
-![](https://raw.githubusercontent.com/medlee-code/RadVis/main/images/example_mask_0.gif?token=GHSAT0AAAAAACBJZC7OHBDQFXT7KM5L42NUZC7T4SQ))
+![](https://raw.githubusercontent.com/medlee-code/RadVis/main/images/example_mask_0.gif?token=GHSAT0AAAAAACBJZC7OHBDQFXT7KM5L42NUZC7T4SQ)
 
 Mask can be another RadImage object so you can load up your masks from a DICOM or NIFTI
 ```python
 import radvis as rv
 import numpy as np
 
 AXIS = 1
```

### Comparing `radvis-0.1.1/README.md` & `radvis-0.1.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 blue_mask[70:150, 70:150, 70:150] = 1
 
 slicer.add_mask(red_mask, color="red")
 slicer.add_mask(blue_mask, color="blue")
 
 slicer.display()
 ```
-![](https://raw.githubusercontent.com/medlee-code/RadVis/main/images/example_mask_0.gif?token=GHSAT0AAAAAACBJZC7OHBDQFXT7KM5L42NUZC7T4SQ))
+![](https://raw.githubusercontent.com/medlee-code/RadVis/main/images/example_mask_0.gif?token=GHSAT0AAAAAACBJZC7OHBDQFXT7KM5L42NUZC7T4SQ)
 
 Mask can be another RadImage object so you can load up your masks from a DICOM or NIFTI
 ```python
 import radvis as rv
 import numpy as np
 
 AXIS = 1
```

### Comparing `radvis-0.1.1/radvis/image/load.py` & `radvis-0.1.2/radvis/image/load.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.1/radvis/image/rad_dicom_image.py` & `radvis-0.1.2/radvis/image/rad_dicom_image.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.1/radvis/image/rad_image.py` & `radvis-0.1.2/radvis/image/rad_image.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,22 +76,29 @@
         # Checks that axis is within the bounds of the image data
         if axis < 0 or axis >= len(self.image_data.shape):
             raise ValueError(f"Axis {axis} is out of bounds for image data of shape {self.image_data.shape}")
         
         # Checks that the index is within the bounds of the image data
         if index < 0 or index >= self.image_data.shape[axis]:
             raise ValueError(f"Index {index} is out of bounds for axis {axis}")
-        
-        # Swap the desired axis with the first axis
-        data = np.swapaxes(self.image_data, 0, axis)
-
-        # Select the slice along the first axis
-        slice_2d = data[index]
 
-        return slice_2d
+        # Slice along the appropriate axis
+        slicer = [slice(None)] * self.image_data.ndim
+        slicer[axis] = index
+        return self.image_data[tuple(slicer)]
+    
+    def copy(self):
+        """ 
+        Return a copy of the image.
+        """
+        new_image = self.__class__(self.file_path)
+        new_image.data = self.data
+        new_image.image_data = np.copy(self.image_data)
+        new_image.metadata = self.metadata.copy() if self.metadata else None
+        return new_image
 
     def __recv__(self) -> str:
         """
         Return a string representation of the image data.
         """
         return self.get_image_info()
```

### Comparing `radvis-0.1.1/radvis/image/rad_nifti_image.py` & `radvis-0.1.2/radvis/image/rad_nifti_image.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .rad_image import RadImage
 import nibabel as nib
 import os
 from typing import Optional
 import numpy as np
-
+nib.Nifti1Header.quaternion_threshold = -1e-06
 
 class RadNiftiImage(RadImage):
     def __init__(self, file_path: Optional[str] = None):
         """
         Initialize the RadNiftiImage class.
 
         :param file_path: The file path to the NIFTI image file, defaults to None
@@ -31,9 +31,9 @@
         Save the NIFTI image to the output file path using the nibabel library.
 
         :param output_file_path: The output file path to save the NIFTI image
         """
         if self.image_data is None:
             raise ValueError("No image data to save.")
 
-        nifti_data = nifti_data = nib.Nifti1Image(self.image_data, affine=np.eye(4))
+        nifti_data = nib.Nifti1Image(self.image_data, affine=np.eye(4))
         nib.save(nifti_data, output_file_path)
```

### Comparing `radvis-0.1.1/radvis/mesh/compute_mesh.py` & `radvis-0.1.2/radvis/mesh/compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.1/radvis/mesh/rad_mesh.py` & `radvis-0.1.2/radvis/mesh/rad_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.1/radvis/visualize/rad_slicer.py` & `radvis-0.1.2/radvis/visualize/rad_slicer.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,136 @@
+import copy
+import matplotlib.cm as cm
 from matplotlib.animation import FuncAnimation, PillowWriter
-from matplotlib.colors import ListedColormap
+from matplotlib.colors import Colormap, ListedColormap
 import matplotlib.pyplot as plt
 from matplotlib.widgets import Slider
 from radvis.image.rad_image import RadImage
 import numpy as np
 import numpy.ma as ma
-import IPython
-from ipywidgets import interact, IntSlider, Layout
+try:
+    import IPython
+    from ipywidgets import interact, IntSlider
+except ImportError:
+    print("Warning: ipywidgets not installed. RadSlicer will not work in Jupyter Notebook.")
 
 
 class RadSlicer:
     def __init__(self, radimage: RadImage, axis: int = 0, title=None, cmap: str = "gray",
-                 width=4, height=4) -> None:
+                 width:int=4, height:int=4, show_slider:bool = True) -> None:
         """
         Initialize the RadSlicer class.
 
         :param radimage: A RadImage object containing the image data
         :param axis: The image axis to slice along, defaults to 0
         :param cmap: The colormap to use for displaying the image, defaults to "gray"
         """
         self.radimage = radimage
         self.axis = axis
         self._title = title
         self._slider = None
+        self._show_slider = show_slider
         self._image_plot = None
         self._mask_plots = []
         self._masks = []
         self._ax = None
         self._cmap = cmap
         self._figsize = (width, height)
         self._notebook_environment = IPython.get_ipython().__class__.__name__ == 'ZMQInteractiveShell'
-
+        self._slider_coords = None
+        
     @property
     def title(self):
         """
         Returns the title. If title is 'None' then returns the title 'Axis: {axis}'
         """
         if self._title is None:
             return f"Axis: {self.axis}"
         return self._title    
 
+    @property
+    def width(self):
+        """
+        Returns the width of the figure.
+        """
+        return self._figsize[0]
+    
+    @property
+    def height(self):
+        """
+        Returns the height of the figure.
+        """
+        return self._figsize[1]
+    
+    @property
+    def figsize(self):
+        """
+        Returns the figure size.
+        """
+        return self._figsize
+
+    def remove_slider(self) -> None:
+        """
+        Remove the slider from the plot.
+        """
+        self._show_slider = False
+        del self._slider
+        self._slider = None
+    
+    def set_slider_coordinates(self, x:float, y:float, width:float, height:float) -> None:
+        """
+        Set the coordinates of the slider.
+
+        :param x: The x-coordinate of the slider
+        :param y: The y-coordinate of the slider
+        :param width: The width of the slider
+        :param height: The height of the slider
+        """
+        self._slider_coords = [x, y, width, height]
+    
     def _update_image(self, val:int) -> None:
         """
         Update the image plot with the selected slice.
 
         :param val: The index of the slice to display
         """
         image_slice = int(val)
         self._image_plot.set_data(self.radimage.get_slice(image_slice, self.axis))
         for plot, (mask, _, _) in zip(self._mask_plots, self._masks):
             plot.set_data(mask[image_slice, :, :] if self.axis == 0 else
                           mask[:, image_slice, :] if self.axis == 1 else
                           mask[:, :, image_slice])
         self.fig.canvas.draw_idle()
 
-    def _create_slider(self, ax: plt.Axes, initial_index: int = 0) -> Slider:
+    def _create_slider(self, ax: plt.Axes, initial_index: int = 0) -> Slider|None:
         """
         Create a slider for the given plt.Axes object.
 
         :param ax: The plt.Axes object to add the slider to
         :param initial_index: The initial slice index, defaults to 0
-        :return: A slider object (either ipywidgets.IntSlider or matplotlib Slider)
+        :return: A slider object (either ipywidgets.IntSlider or matplotlib Slider) or None
         """
+        if self._show_slider is False:
+            return None
+        
         if self._notebook_environment:
             slider = interact(lambda val: self._update_image(val), 
                               val=IntSlider(min=0, max=self.radimage.shape[self.axis]-1, step=1, value=initial_index, 
                                             description=f"{self.title}: Slice"))
         else:
             ax_position = ax.get_position()
             slider_width = ax_position.width - 0.2
+            slider_height = 0.03
             slider_x = ax_position.x0 + 0.1
             slider_y = ax_position.y0 - 0.15
-
-            ax_slider = plt.axes([slider_x, slider_y, slider_width, 0.03])
+            
+            if self._slider_coords is not None:
+                slider_x, slider_y, slider_width, slider_height = self._slider_coords
+                
+            ax_slider = plt.axes([slider_x, slider_y, slider_width, slider_height])
             slider = Slider(ax_slider, f"Slice", 0, self.radimage.shape[self.axis] - 1, valstep=1, valfmt="%d",
                                 valinit=initial_index)
             slider.on_changed(self._update_image)
         return slider
     
     def _plot_image(self, ax: plt.Axes, initial_index: int = 0) -> None:
         """
@@ -93,37 +147,42 @@
             interpolation='none'
         )
         for mask, cmap, alpha in self._masks:
             mask_plot = ax.imshow(mask[initial_index, :, :] if self.axis == 0 else
                       mask[:, initial_index, :] if self.axis == 1 else
                       mask[:, :, initial_index],
                       cmap=cmap, interpolation='none', alpha=alpha,
-                      vmin=0, vmax=1)
+                      vmin=0, vmax=mask.max())
             self._mask_plots.append(mask_plot)
         self._slider = self._create_slider(ax, initial_index)
 
 
-    def display(self, ax: plt.Axes = None, initial_index: int = 0) -> None:
+    def display(self, ax: plt.Axes = None, initial_index: int = 0, show_plot=True) -> None:
         """
         Display the RadSlicer plot with a slider to control the displayed slice.
         """
         if len(self.radimage.shape) != 3:
             raise ValueError("display method expects a 3D image")
 
         if ax is None:
             self.fig, self._ax = plt.subplots()
             plt.subplots_adjust(bottom=0.2)
-            
+        else:
+            self._ax = ax
+            self.fig = ax.get_figure()
+               
         self._ax.set_title(self.title, y=1)
         self.fig.set_size_inches(self._figsize[0], self._figsize[1], forward=False)
         
         self._plot_image(self._ax, initial_index)
-        plt.show()
+        
+        if show_plot:
+            plt.show()
 
-    def add_mask(self, mask: np.ndarray | RadImage, color: str = 'red', alpha: float = 0.5):
+    def add_mask(self, mask: np.ndarray | RadImage, color: str | Colormap = 'red', alpha: float = 0.5):
         """
         Adds a mask to the RadSlicer.
 
         :param mask: A 3D array that matches the shape of the radimage
         :param color: The color of the mask
         :param alpha: The opacity of the mask
         """
@@ -131,16 +190,25 @@
             raise ValueError("Mask must be a numpy array or RadImage object")
         
         if isinstance(mask, RadImage):
             mask = mask.image_data
         
         if mask.shape != self.radimage.shape:
             raise ValueError("Mask shape must match image shape")
-
-        cmap = ListedColormap([color])
+        
+        if isinstance(color, str):
+            if color in plt.colormaps():
+                cmap = cm.get_cmap(color)
+            else:
+                cmap = ListedColormap([color])
+        elif isinstance(color, Colormap):
+            cmap = color
+        else:
+            raise ValueError("Color must be a string or a Colormap object")
+        
         mask = ma.masked_where(mask == 0, mask)
         
         self._masks.append((mask, cmap, alpha))
     
     def save_animation(self, filepath: str, fps: int = 10) -> None:
         """
         Save an animation of all slices to a GIF file.
@@ -155,8 +223,14 @@
         # Create the animation
         anim = FuncAnimation(self.fig, self._update_image, frames=self.radimage.shape[self.axis], interval=1000//fps)
 
         try:
             anim.save(filepath, writer=PillowWriter(fps=fps))
         except Exception as e:
             print(f"Could not save the animation due to the following error: {e}")
+            
+    def copy(self):
+        """
+        Create a copy of the RadSlicer object.
+        """
+        return copy.deepcopy(self)
```

### Comparing `radvis-0.1.1/radvis.egg-info/PKG-INFO` & `radvis-0.1.2/radvis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: radvis
-Version: 0.1.1
+Version: 0.1.2
 Summary: A visualization tool for medical images
 Home-page: https://github.com/medlee-code/RadVis
 Author: Matthew lee
 Author-email: matthewlee@medlee.io
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -55,15 +55,15 @@
 blue_mask[70:150, 70:150, 70:150] = 1
 
 slicer.add_mask(red_mask, color="red")
 slicer.add_mask(blue_mask, color="blue")
 
 slicer.display()
 ```
-![](https://raw.githubusercontent.com/medlee-code/RadVis/main/images/example_mask_0.gif?token=GHSAT0AAAAAACBJZC7OHBDQFXT7KM5L42NUZC7T4SQ))
+![](https://raw.githubusercontent.com/medlee-code/RadVis/main/images/example_mask_0.gif?token=GHSAT0AAAAAACBJZC7OHBDQFXT7KM5L42NUZC7T4SQ)
 
 Mask can be another RadImage object so you can load up your masks from a DICOM or NIFTI
 ```python
 import radvis as rv
 import numpy as np
 
 AXIS = 1
```

### Comparing `radvis-0.1.1/setup.py` & `radvis-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='radvis',
-    version='0.1.1',
+    version='0.1.2',
     url='https://github.com/medlee-code/RadVis',
     author='Matthew lee',
     author_email='matthewlee@medlee.io',
     description='A visualization tool for medical images',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
-        'pytest==7.3.1',
-        'meshio==5.3.4',
         'scikit-image==0.20.0',
         'pydicom==2.3.1',
         'nibabel==5.1.0',
-        'matplotlib==3.7.1',
-        'jupyter==1.0.0'
+        'matplotlib==3.7.1'
     ],
     python_requires='>=3.10',
 )
```

### Comparing `radvis-0.1.1/tests/test_mesh/test_compute_mesh.py` & `radvis-0.1.2/tests/test_mesh/test_compute_mesh.py`

 * *Files identical despite different names*

### Comparing `radvis-0.1.1/tests/test_visualize/test_rad_slicer.py` & `radvis-0.1.2/tests/test_visualize/test_rad_slicer.py`

 * *Files identical despite different names*


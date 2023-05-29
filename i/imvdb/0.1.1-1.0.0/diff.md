# Comparing `tmp/imvdb-0.1.1-py3-none-any.whl.zip` & `tmp/imvdb-1.0.0-cy310-cp310-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 4595977 bytes, number of entries: 16
+Zip file size: 4608248 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat   335360 b- defN 23-May-24 03:59 imvdb/Imath-3_1.dll
--rw-rw-rw-  2.0 fat       68 b- defN 23-May-26 09:46 imvdb/__init__.py
--rw-rw-rw-  2.0 fat     2545 b- defN 23-May-26 09:42 imvdb/__main__.py
+-rw-rw-rw-  2.0 fat       68 b- defN 23-May-29 06:05 imvdb/__init__.py
+-rw-rw-rw-  2.0 fat     5065 b- defN 23-May-29 06:22 imvdb/__main__.py
 -rw-rw-rw-  2.0 fat    56320 b- defN 23-May-24 04:04 imvdb/blosc.dll
--rw-rw-rw-  2.0 fat     1608 b- defN 23-May-26 09:42 imvdb/grid.py
--rw-rw-rw-  2.0 fat      894 b- defN 23-May-26 09:42 imvdb/image.py
+-rw-rw-rw-  2.0 fat     2044 b- defN 23-May-28 11:34 imvdb/grid.py
+-rw-rw-rw-  2.0 fat      995 b- defN 23-May-29 06:18 imvdb/image.py
 -rw-rw-rw-  2.0 fat   121344 b- defN 23-May-24 04:04 imvdb/lz4.dll
 -rw-rw-rw-  2.0 fat 24425984 b- defN 23-May-24 04:12 imvdb/openvdb.dll
 -rw-rw-rw-  2.0 fat   313856 b- defN 23-May-24 03:59 imvdb/tbb12.dll
--rw-rw-rw-  2.0 fat   466944 b- defN 23-May-26 08:26 imvdb/vdb.cp310-win_amd64.pyd
+-rw-rw-rw-  2.0 fat   492032 b- defN 23-May-28 11:37 imvdb/vdb.cp310-win_amd64.pyd
 -rw-rw-rw-  2.0 fat    89600 b- defN 23-May-24 03:59 imvdb/zlib1.dll
 -rw-rw-rw-  2.0 fat   647680 b- defN 23-May-24 04:03 imvdb/zstd.dll
--rw-rw-rw-  2.0 fat      522 b- defN 23-May-26 09:46 imvdb-0.1.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-26 09:46 imvdb-0.1.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-26 09:46 imvdb-0.1.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1183 b- defN 23-May-26 09:46 imvdb-0.1.1.dist-info/RECORD
-16 files, 26464006 bytes uncompressed, 4594103 bytes compressed:  82.6%
+-rw-rw-rw-  2.0 fat      661 b- defN 23-May-29 06:26 imvdb-1.0.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-29 06:26 imvdb-1.0.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-29 06:26 imvdb-1.0.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1183 b- defN 23-May-29 06:26 imvdb-1.0.0.dist-info/RECORD
+16 files, 26492290 bytes uncompressed, 4606374 bytes compressed:  82.6%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: imvdb/zlib1.dll
 Comment: 
 
 Filename: imvdb/zstd.dll
 Comment: 
 
-Filename: imvdb-0.1.1.dist-info/METADATA
+Filename: imvdb-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: imvdb-0.1.1.dist-info/WHEEL
+Filename: imvdb-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: imvdb-0.1.1.dist-info/top_level.txt
+Filename: imvdb-1.0.0.dist-info/top_level.txt
 Comment: 
 
-Filename: imvdb-0.1.1.dist-info/RECORD
+Filename: imvdb-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imvdb/__init__.py

```diff
@@ -1,4 +1,4 @@
 from .grid import *
 from .image import *
 
-__version__ = '0.1.1'
+__version__ = '1.0.0'
```

## imvdb/__main__.py

```diff
@@ -1,62 +1,139 @@
+import os
+from pathlib import Path
+
 import click
 import itk
+import pyvista as pv
+import pyvista.examples as pve
 import numpy as np
 
 import imvdb
 
 
 @click.group()
 def main():
     pass
 
 
 @main.command()
-@click.argument('input_image', type=str)
-@click.argument('iso_value', type=float)
-@click.option('--threshold_min', type=float, default=-np.inf)
-@click.option('--threshold_max', type=float, default=np.inf)
-@click.option('--fog_volume_vdb', type=str, default=None)
+@click.argument('workspace', type=str)
+@click.option('--input_image', type=str, default=None)
+@click.option('--iso_value', type=float, default=1500)
+@click.option('--threshold_min', type=float, default=1000)
+@click.option('--threshold_max', type=float, default=3000)
 @click.option('--fog_volume_name', type=str, default='fog_volume')
-@click.option('--fog_volume_image', type=str, default=None)
-@click.option('--level_set_vdb', type=str, default=None)
+@click.option('--fog_volume_vdb', type=str, default='fog_volume.vdb')
+@click.option('--fog_volume_image', type=str, default='fog_volume.nii.gz')
+@click.option('--fog_volume_mesh', type=str, default='fog_volume.stl')
 @click.option('--level_set_name', type=str, default='level_set')
-@click.option('--level_set_image', type=str, default=None)
-@click.option('--creator', type=str, default='creator')
-def image(input_image: str, iso_value: float, threshold_min: float = -np.inf, threshold_max: float = np.inf,
-          fog_volume_vdb: str = None, fog_volume_name: str = 'fog_volume', fog_volume_image: str = None,
-          level_set_vdb: str = None, level_set_name: str = 'level_set', level_set_image: str = None,
-          creator: str = 'creator'):
-    array, origin, spacing = imvdb.array_from_imread(input_image, (threshold_min, threshold_max))
-
-    if fog_volume_vdb is not None or level_set_vdb is not None:
-        fog_volume = imvdb.fog_volume_from_array(array, origin, spacing)
-        fog_volume.name = fog_volume_name
-        fog_volume.creator = creator
-
-        if fog_volume_vdb is not None:
-            imvdb.write(fog_volume, fog_volume_vdb)
-
-        if fog_volume_image is not None:
-            array, origin, spacing = imvdb.array_from_grid(fog_volume)
-            itk_image = itk.image_from_array(array)
-            itk_image.SetOrigin(origin)
-            itk_image.SetSpacing(spacing)
-            itk.imwrite(itk_image, fog_volume_image)
-
-        if level_set_vdb is not None:
-            iso_value = (iso_value - threshold_min) / (threshold_max - threshold_min)
-            level_set = imvdb.fog_to_sdf(fog_volume, iso_value)
-            level_set.name = level_set_name
-            level_set.creator = creator
-            imvdb.write(level_set, level_set_vdb)
-
-            if level_set_image is not None:
-                array, origin, spacing = imvdb.array_from_grid(level_set)
-                itk_image = itk.image_from_array(array)
-                itk_image.SetOrigin(origin)
-                itk_image.SetSpacing(spacing)
-                itk.imwrite(itk_image, level_set_image)
+@click.option('--level_set_vdb', type=str, default='level_set.vdb')
+@click.option('--level_set_image', type=str, default='level_set.nii.gz')
+@click.option('--level_set_mesh', type=str, default='level_set.stl')
+@click.option('--creator', type=str, default='imvdb')
+def demo(workspace: str, input_image: str, iso_value: float, threshold_min: float, threshold_max: float,
+         fog_volume_vdb: str, fog_volume_name: str, fog_volume_image: str, fog_volume_mesh: str,
+         level_set_vdb: str, level_set_name: str, level_set_image: str, level_set_mesh: str,
+         creator: str, ):
+    workspace = Path(workspace)
+    os.makedirs(workspace, exist_ok=True)
+
+    fog_volume_vdb = workspace / fog_volume_vdb
+    fog_volume_image = workspace / fog_volume_image
+    fog_volume_mesh = workspace / fog_volume_mesh
+    level_set_vdb = workspace / level_set_vdb
+    level_set_image = workspace / level_set_image
+    level_set_mesh = workspace / level_set_mesh
+
+    if input_image is None:
+        # download input image
+        ds = pve.download_head_2()
+        origin = np.array(ds.origin)
+        spacing = np.array(ds.spacing)
+
+        _ = ds.point_data.keys()[0]
+        array = ds.point_data[_].reshape(ds.dimensions, order='F')
+        array = np.ascontiguousarray(array)[:, ::-1, ::-1].copy().astype(np.float32)
+    else:
+        # read input image
+        array, origin, spacing = imvdb.array_from_imread(input_image)
+
+    iso_value = (iso_value - threshold_min) / (threshold_max - threshold_min)
+    array = imvdb.array_normalized(array, (threshold_min, threshold_max))
+
+    # fog volume vdb
+    fog_volume = imvdb.fog_volume_from_array(array, origin, spacing)
+    fog_volume.name = fog_volume_name
+    fog_volume.creator = creator
+    imvdb.write(fog_volume, fog_volume_vdb.as_posix())
+
+    # fog volume image
+    array, origin, spacing = imvdb.array_from_grid(fog_volume)
+    itk_image = itk.image_from_array(array)
+    itk_image.SetOrigin(origin)
+    itk_image.SetSpacing(spacing)
+    itk.imwrite(itk_image, fog_volume_image.as_posix())
+
+    # fog volume mesh
+    grid = pv.UniformGrid(itk.vtk_image_from_image(itk_image))
+    mesh = grid.contour(1, None, True, False, False, [iso_value, iso_value], 'point', 'flying_edges')
+    mesh.save(fog_volume_mesh.as_posix())
+
+    # level set vdb
+    level_set = imvdb.fog_to_sdf(fog_volume, iso_value)
+    level_set.name = level_set_name
+    level_set.creator = creator
+    imvdb.write(level_set, level_set_vdb.as_posix())
+
+    # level set image
+    array, origin, spacing = imvdb.array_from_grid(level_set)
+    itk_image = itk.image_from_array(array)
+    itk_image.SetOrigin(origin)
+    itk_image.SetSpacing(spacing)
+    itk.imwrite(itk_image, level_set_image.as_posix())
+
+    # level set mesh
+    grid = pv.UniformGrid(itk.vtk_image_from_image(itk_image))
+    mesh = grid.contour(1, None, True, False, False, [0, 0], 'point', 'flying_edges')
+    mesh.save(level_set_mesh.as_posix())
+
+    # plot
+    pl = pv.Plotter(shape=(2, 2))
+    camera = pv.Camera()
+
+    pl.subplot(0, 0)
+    pl.add_axes()
+    pl.add_text('Fog Volume Image', 'upper_edge', 9)
+    pl.camera = camera
+    pl.camera_position = 'xz'
+    read = pv.get_reader(fog_volume_image.as_posix()).read()
+    pl.add_volume(read, clim=[-1, 1], opacity='linear', cmap='magma', show_scalar_bar=False)
+    pl.reset_camera()
+
+    pl.subplot(0, 1)
+    pl.add_axes()
+    pl.add_text('Level Set Image', 'upper_edge', 9)
+    pl.camera = camera
+    read = pv.get_reader(level_set_image.as_posix()).read()
+    pl.add_volume(read, clim=[-1, 1], opacity='linear_r', cmap='magma_r', show_scalar_bar=False)
+    pl.reset_camera()
+
+    pl.subplot(1, 0)
+    pl.add_axes()
+    pl.add_text('Fog Volume Mesh', 'upper_edge', 9)
+    pl.camera = camera
+    pl.camera_position = 'xz'
+    pl.add_mesh(pv.get_reader(fog_volume_mesh.as_posix()).read())
+    pl.reset_camera()
+
+    pl.subplot(1, 1)
+    pl.add_axes()
+    pl.add_text('Level Set Mesh', 'upper_edge', 9)
+    pl.camera = camera
+    pl.add_mesh(pv.get_reader(level_set_mesh.as_posix()).read())
+    pl.reset_camera()
+
+    pl.show()
 
 
 if __name__ == '__main__':
     main()
```

## imvdb/grid.py

```diff
@@ -3,14 +3,18 @@
 import numpy as np
 
 from . import vdb  # noqa
 
 Grid = vdb.Grid
 
 
+def probe(grid: Grid, ijk: list) -> float:
+    return vdb.probe(grid, list(ijk))
+
+
 def fog_volume_from_array(array: np.ndarray, origin: np.ndarray = np.zeros(3), spacing: np.ndarray = np.ones(3),
                           background: float = 0.0, tolerance: float = 0.0) -> Grid:
     grid = vdb.from_array(array, origin.tolist(), spacing.tolist(), background, tolerance)
     grid.grid_class = 'fog volume'
     return grid
 
 
@@ -43,10 +47,18 @@
 def write(grids: list | Grid, filename: str) -> None:
     if not isinstance(grids, list):
         grids = [grids]
     return vdb.write(grids, filename)
 
 
 def fog_to_sdf(grid: Grid, iso_value: float) -> Grid:
-    grid = vdb.fog_to_sdf(grid, iso_value)
+    grid = vdb.fog_to_sdf(grid, float(iso_value))
     grid.grid_class = 'level set'
     return grid
+
+
+def volume_to_mesh(grid: Grid, iso_value: float, adaptivity: float = 0.0) -> (np.ndarray, np.ndarray, np.ndarray):
+    return vdb.volume_to_mesh(grid, float(iso_value), float(adaptivity))
+
+
+def volume_to_quad_mesh(grid: Grid, iso_value: float) -> (np.ndarray, np.ndarray):
+    return vdb.volume_to_quad_mesh(grid, float(iso_value))
```

## imvdb/image.py

```diff
@@ -2,27 +2,30 @@
 import numpy as np
 
 
 def _normalize(v, r):
     return (v - r[0]) / (r[1] - r[0])
 
 
-def array_from_imread(input_image: str, threshold=(-np.inf, np.inf)):
+def array_from_imread(input_image: str) -> (np.ndarray, np.ndarray, np.ndarray):
     image = itk.imread(input_image)
     origin = np.array(itk.origin(image))
     spacing = np.array(itk.spacing(image))
+    array = itk.array_from_image(image)
+    array = np.swapaxes(array, 0, 2).copy().astype(np.float32)
+    return array, origin, spacing
+
+
+def array_normalized(array: np.ndarray, minmax=(-np.inf, np.inf)) -> np.ndarray:
+    if array.ndim == 1:
+        array = array[:, np.newaxis, np.newaxis]
+    elif array.ndim == 2:
+        array = array[:, np.newaxis]
+    elif array.ndim > 3:
+        raise RuntimeError(f'input array has {array.ndim} > 3 dimensions')
+
+    minmax = (np.max([minmax[0], np.min(array)]), np.min([minmax[1], np.max(array)]))
+    array = _normalize(array, minmax)
+    array[np.where(array < 0)] = 0
+    array[np.where(array > 1)] = 1
 
-    image = itk.array_from_image(image)
-    image = np.swapaxes(image, 0, 2).copy().astype(np.float32)
-    if image.ndim == 1:
-        image = image[:, np.newaxis, np.newaxis]
-    elif image.ndim == 2:
-        image = image[:, np.newaxis]
-    elif image.ndim > 3:
-        raise RuntimeError(f'input image has {image.ndim} > 3 dimensions')
-
-    threshold = (np.max([threshold[0], np.min(image)]), np.min([threshold[1], np.max(image)]))
-    image = _normalize(image, threshold)
-    image[np.where(image < 0)] = 0
-    image[np.where(image > 1)] = 1
-
-    return image, origin, spacing
+    return array
```

## Comparing `imvdb-0.1.1.dist-info/RECORD` & `imvdb-1.0.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 imvdb/Imath-3_1.dll,sha256=3BKAHdSIBVsX0rU8j9GgWcIfBkcL_Z7Wfmm0vnapZPc,335360
-imvdb/__init__.py,sha256=YzZ_Qhh0QplvmMB-fUhXSaQ7UMzaxA4nWDJsJpmlxUk,68
-imvdb/__main__.py,sha256=U03FobS__W19JbTT7AuetcjU2lZC6U-H8B9D5PLE-EQ,2545
+imvdb/__init__.py,sha256=2QplP_Ry1RLpCdDMNZHaFoY0z7stzY9EIaOtw8ARACE,68
+imvdb/__main__.py,sha256=7O4vMnE58-KArs0CsBpe0GBPt45i2A00l4kWskSUzoQ,5065
 imvdb/blosc.dll,sha256=4EUTAeqsrUtUR1IEzJvMa1Pd7etY3n-_8lLVbK8dRrY,56320
-imvdb/grid.py,sha256=HCPGCSnnBMRDQuCK9tz4BkTXCral0T50vwzZvVAb-Ys,1608
-imvdb/image.py,sha256=TxLpCv8BVf1m1rahILnOtEC34ISgBeqMbbpga9CmHNw,894
+imvdb/grid.py,sha256=KTYFWukaASCPo4cw1BO99sMXbYzdaWCVqef2mr1LFQY,2044
+imvdb/image.py,sha256=owkgyZtSmWyJqjUjPWPh9ogfOx29ZbCa49kykpeizb4,995
 imvdb/lz4.dll,sha256=Aw5Gyv9ASezphkxf9BYlakxkLgqsFfSHkutitYbe2WE,121344
 imvdb/openvdb.dll,sha256=YgXi0tpTSbh1VSZTre64e0DhaWfgPaFRvzU2B1T7pkE,24425984
 imvdb/tbb12.dll,sha256=V6MKyrSVwoeDlcTZ61Nt1GuwcLBSlLgrr0VcxFKzOrI,313856
-imvdb/vdb.cp310-win_amd64.pyd,sha256=zfc_Hhu-kEH0dm11M2z8ujF9daFR2LapNNd8KggaW2g,466944
+imvdb/vdb.cp310-win_amd64.pyd,sha256=UkmBFnLs7GuicWSq4zKblvnQpuoTpTB2net4nYlI528,492032
 imvdb/zlib1.dll,sha256=RX5PDb4Bz7LSkoe1VwKPu7TQAYaYXi89dUgGqaisYzA,89600
 imvdb/zstd.dll,sha256=sSKJ2maR9P60_yyFptIcMRzXVC6X0C7e2hOC3tbD95I,647680
-imvdb-0.1.1.dist-info/METADATA,sha256=F7mXq3np0W5twHY7RfjuEyHaZuy87ijlTEaJKxpd6Jg,522
-imvdb-0.1.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-imvdb-0.1.1.dist-info/top_level.txt,sha256=MtcExZYAYSRbAYb9aoAppo_aGrRaUnKcig1Ovxdhaeg,6
-imvdb-0.1.1.dist-info/RECORD,,
+imvdb-1.0.0.dist-info/METADATA,sha256=DjjsZhHvMU9s-uCXTq4YjHYxsyzxnTDtmrJKDUiMFNs,661
+imvdb-1.0.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+imvdb-1.0.0.dist-info/top_level.txt,sha256=MtcExZYAYSRbAYb9aoAppo_aGrRaUnKcig1Ovxdhaeg,6
+imvdb-1.0.0.dist-info/RECORD,,
```


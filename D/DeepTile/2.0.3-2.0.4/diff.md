# Comparing `tmp/DeepTile-2.0.3.tar.gz` & `tmp/DeepTile-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DeepTile-2.0.3.tar", last modified: Sun Jan 29 06:45:10 2023, max compression
+gzip compressed data, was "DeepTile-2.0.4.tar", last modified: Mon May 29 19:04:18 2023, max compression
```

## Comparing `DeepTile-2.0.3.tar` & `DeepTile-2.0.4.tar`

### file list

```diff
@@ -1,37 +1,41 @@
-drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-01-29 06:45:10.378806 DeepTile-2.0.3/
-drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-01-29 06:45:10.378806 DeepTile-2.0.3/DeepTile.egg-info/
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     1134 2023-01-29 06:45:10.000000 DeepTile-2.0.3/DeepTile.egg-info/PKG-INFO
--rw-rw-r--   0 wniu      (1000) wniu      (1000)      727 2023-01-29 06:45:10.000000 DeepTile-2.0.3/DeepTile.egg-info/SOURCES.txt
--rw-rw-r--   0 wniu      (1000) wniu      (1000)        1 2023-01-29 06:45:10.000000 DeepTile-2.0.3/DeepTile.egg-info/dependency_links.txt
--rw-rw-r--   0 wniu      (1000) wniu      (1000)       37 2023-01-29 06:45:10.000000 DeepTile-2.0.3/DeepTile.egg-info/requires.txt
--rw-rw-r--   0 wniu      (1000) wniu      (1000)        9 2023-01-29 06:45:10.000000 DeepTile-2.0.3/DeepTile.egg-info/top_level.txt
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     1068 2022-10-16 00:41:51.000000 DeepTile-2.0.3/LICENSE
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     1134 2023-01-29 06:45:10.378806 DeepTile-2.0.3/PKG-INFO
--rw-rw-r--   0 wniu      (1000) wniu      (1000)      664 2023-01-29 06:27:36.000000 DeepTile-2.0.3/README.md
-drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-01-29 06:45:10.378806 DeepTile-2.0.3/deeptile/
--rw-rw-r--   0 wniu      (1000) wniu      (1000)      103 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/__init__.py
-drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-01-29 06:45:10.378806 DeepTile-2.0.3/deeptile/core/
--rw-rw-r--   0 wniu      (1000) wniu      (1000)        0 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/core/__init__.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)    24644 2023-01-27 17:43:28.000000 DeepTile-2.0.3/deeptile/core/data.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     3229 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/core/iterators.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)      923 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/core/jobs.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     7954 2023-01-28 23:31:20.000000 DeepTile-2.0.3/deeptile/core/lift.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)    12939 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/core/process.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     1660 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/core/profiles.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     5018 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/core/trees.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     4351 2023-01-27 17:43:28.000000 DeepTile-2.0.3/deeptile/core/utils.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     6947 2023-01-28 21:45:35.000000 DeepTile-2.0.3/deeptile/deeptile.py
-drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-01-29 06:45:10.378806 DeepTile-2.0.3/deeptile/extensions/
--rw-rw-r--   0 wniu      (1000) wniu      (1000)       53 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/extensions/__init__.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     3560 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/extensions/segmentation.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)    11186 2023-01-28 08:00:48.000000 DeepTile-2.0.3/deeptile/extensions/stitch.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     3213 2023-01-28 21:45:35.000000 DeepTile-2.0.3/deeptile/io.py
-drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-01-29 06:45:10.378806 DeepTile-2.0.3/deeptile/sources/
--rw-rw-r--   0 wniu      (1000) wniu      (1000)        0 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/sources/__init__.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)      156 2022-12-13 08:16:08.000000 DeepTile-2.0.3/deeptile/sources/array.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)      894 2023-01-27 17:43:28.000000 DeepTile-2.0.3/deeptile/sources/function.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     2135 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/sources/large_image.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)     3742 2023-01-28 23:16:20.000000 DeepTile-2.0.3/deeptile/sources/nd2.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)      353 2022-10-16 00:41:51.000000 DeepTile-2.0.3/deeptile/sources/tiff.py
--rw-rw-r--   0 wniu      (1000) wniu      (1000)      752 2023-01-29 06:43:49.000000 DeepTile-2.0.3/pyproject.toml
--rw-rw-r--   0 wniu      (1000) wniu      (1000)       38 2023-01-29 06:45:10.378806 DeepTile-2.0.3/setup.cfg
+drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-05-29 19:04:18.655462 DeepTile-2.0.4/
+drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-05-29 19:04:18.655462 DeepTile-2.0.4/DeepTile.egg-info/
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     1134 2023-05-29 19:04:18.000000 DeepTile-2.0.4/DeepTile.egg-info/PKG-INFO
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)      787 2023-05-29 19:04:18.000000 DeepTile-2.0.4/DeepTile.egg-info/SOURCES.txt
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)        1 2023-05-29 19:04:18.000000 DeepTile-2.0.4/DeepTile.egg-info/dependency_links.txt
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)       37 2023-05-29 19:04:18.000000 DeepTile-2.0.4/DeepTile.egg-info/requires.txt
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)        9 2023-05-29 19:04:18.000000 DeepTile-2.0.4/DeepTile.egg-info/top_level.txt
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     1068 2022-10-16 00:41:51.000000 DeepTile-2.0.4/LICENSE
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     1134 2023-05-29 19:04:18.655462 DeepTile-2.0.4/PKG-INFO
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)      664 2023-01-29 06:27:36.000000 DeepTile-2.0.4/README.md
+drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-05-29 19:04:18.655462 DeepTile-2.0.4/deeptile/
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)      103 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/__init__.py
+drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-05-29 19:04:18.655462 DeepTile-2.0.4/deeptile/core/
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)        0 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/core/__init__.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)    26519 2023-05-29 17:15:47.000000 DeepTile-2.0.4/deeptile/core/data.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     3229 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/core/iterators.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)      923 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/core/jobs.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     7954 2023-01-28 23:31:20.000000 DeepTile-2.0.4/deeptile/core/lift.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)    12939 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/core/process.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     1660 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/core/profiles.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     5018 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/core/trees.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     4375 2023-02-23 08:42:53.000000 DeepTile-2.0.4/deeptile/core/utils.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     6947 2023-01-28 21:45:35.000000 DeepTile-2.0.4/deeptile/deeptile.py
+drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-05-29 19:04:18.655462 DeepTile-2.0.4/deeptile/extensions/
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)       53 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/extensions/__init__.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     3560 2023-05-29 16:45:32.000000 DeepTile-2.0.4/deeptile/extensions/segmentation.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)    11186 2023-01-28 08:00:48.000000 DeepTile-2.0.4/deeptile/extensions/stitch.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     3213 2023-01-28 21:45:35.000000 DeepTile-2.0.4/deeptile/io.py
+drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-05-29 19:04:18.655462 DeepTile-2.0.4/deeptile/sources/
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)        0 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/sources/__init__.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)      156 2022-12-13 08:16:08.000000 DeepTile-2.0.4/deeptile/sources/array.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)      894 2023-01-27 17:43:28.000000 DeepTile-2.0.4/deeptile/sources/function.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     2135 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/sources/large_image.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     3742 2023-01-28 23:16:20.000000 DeepTile-2.0.4/deeptile/sources/nd2.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)      353 2022-10-16 00:41:51.000000 DeepTile-2.0.4/deeptile/sources/tiff.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)      752 2023-05-29 19:02:06.000000 DeepTile-2.0.4/pyproject.toml
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)       38 2023-05-29 19:04:18.655462 DeepTile-2.0.4/setup.cfg
+drwxrwxr-x   0 wniu      (1000) wniu      (1000)        0 2023-05-29 19:04:18.655462 DeepTile-2.0.4/tests/
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)      217 2022-12-27 08:25:09.000000 DeepTile-2.0.4/tests/test_imports.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     3449 2023-01-28 23:13:10.000000 DeepTile-2.0.4/tests/test_io.py
+-rw-rw-r--   0 wniu      (1000) wniu      (1000)     1668 2022-12-29 00:57:38.000000 DeepTile-2.0.4/tests/test_stitch.py
```

### Comparing `DeepTile-2.0.3/DeepTile.egg-info/PKG-INFO` & `DeepTile-2.0.4/DeepTile.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepTile
-Version: 2.0.3
+Version: 2.0.4
 Summary: Large image tiling and stitching library for scaling Python functions to arbitrary input image sizes.
 Author: William Niu
 Author-email: wniu721@gmail.com
 Keywords: machine learning,deep learning,image tiling,image stitching
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
```

### Comparing `DeepTile-2.0.3/LICENSE` & `DeepTile-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/PKG-INFO` & `DeepTile-2.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DeepTile
-Version: 2.0.3
+Version: 2.0.4
 Summary: Large image tiling and stitching library for scaling Python functions to arbitrary input image sizes.
 Author: William Niu
 Author-email: wniu721@gmail.com
 Keywords: machine learning,deep learning,image tiling,image stitching
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
```

### Comparing `DeepTile-2.0.3/README.md` & `DeepTile-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/core/data.py` & `DeepTile-2.0.4/deeptile/core/data.py`

 * *Files 9% similar despite different names*

```diff
@@ -318,15 +318,18 @@
         ------
         NotImplementedError
             If padding ``mode`` is not supported.
     """
 
         mode = kwargs.get('mode', 'constant')
 
-        if mode not in ['constant', 'edge', 'linear_ramp', 'reflect', 'symmetric']:
+        if mode not in ['constant', 'edge', 'linear_ramp',
+                        'maximum', 'mean', 'median', 'minimum',
+                        'tile_maximum', 'tile_mean', 'tile_median', 'tile_minimum',
+                        'reflect', 'symmetric']:
 
             raise NotImplementedError('Padding mode is not supported.')
 
         if self.metadata['isimage'] and not self.metadata['stackable']:
 
             tiles = np.array(self)
 
@@ -343,14 +346,28 @@
                                 extension = self.profile.tile_indices[0][-1, 0] - self.profile.tile_indices[0][-2, 0]
                                 extended_tile = np.concatenate((inner_tile[..., :extension, :], edge_tile), axis=-2)
                                 padded_tile = utils.array_pad(extended_tile, tile_padding[0], -2, **kwargs)
                                 padded_tile = padded_tile[..., -tile_size[0]:, :]
                             else:
                                 padded_tile = utils.array_pad(edge_tile, tile_padding[0], -2, **kwargs)
                             tiles[-1, i] = padded_tile
+                elif mode in ['tile_maximum', 'tile_mean', 'tile_median', 'tile_minimum']:
+                    for i, tile in enumerate(tiles[-1]):
+                        if tile is not None:
+                            constant = None
+                            if mode == 'tile_maximum':
+                                constant = np.max(tile)
+                            elif mode == 'tile_mean':
+                                constant = np.mean(tile)
+                            elif mode == 'tile_median':
+                                constant = np.median(tile)
+                            elif mode == 'tile_minimum':
+                                constant = np.min(tile)
+                            tiles[-1, i] = \
+                                utils.array_pad(tile, tile_padding[0], -2, mode='constant', constant_values=constant)
                 else:
                     for i, tile in enumerate(tiles[-1]):
                         if tile is not None:
                             tiles[-1, i] = utils.array_pad(tile, tile_padding[0], -2, **kwargs)
 
             if tile_padding[1] > 0:
                 if (mode in ['reflect', 'symmetric']) and (tiles.shape[1] > 1):
@@ -360,14 +377,28 @@
                                 extension = self.profile.tile_indices[1][-1, 0] - self.profile.tile_indices[1][-2, 0]
                                 extended_tile = np.concatenate((inner_tile[..., :extension], edge_tile), axis=-1)
                                 padded_tile = utils.array_pad(extended_tile, tile_padding[1], -1, **kwargs)
                                 padded_tile = padded_tile[..., -tile_size[1]:]
                             else:
                                 padded_tile = utils.array_pad(edge_tile, tile_padding[0], -1, **kwargs)
                             tiles[i, -1] = padded_tile
+                elif mode in ['tile_maximum', 'tile_mean', 'tile_median', 'tile_minimum']:
+                    for i, tile in enumerate(tiles[:, -1]):
+                        if tile is not None:
+                            constant = None
+                            if mode == 'tile_maximum':
+                                constant = np.max(tile)
+                            elif mode == 'tile_mean':
+                                constant = np.mean(tile)
+                            elif mode == 'tile_median':
+                                constant = np.median(tile)
+                            elif mode == 'tile_minimum':
+                                constant = np.min(tile)
+                            tiles[i, -1] = \
+                                utils.array_pad(tile, tile_padding[1], -1, mode='constant', constant_values=constant)
                 else:
                     for i, tile in enumerate(tiles[:, -1]):
                         if tile is not None:
                             tiles[i, -1] = utils.array_pad(tile, tile_padding[1], -1, **kwargs)
 
             job = Job(self, 'pad_tiles', kwargs)
```

### Comparing `DeepTile-2.0.3/deeptile/core/iterators.py` & `DeepTile-2.0.4/deeptile/core/iterators.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/core/jobs.py` & `DeepTile-2.0.4/deeptile/core/jobs.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/core/lift.py` & `DeepTile-2.0.4/deeptile/core/lift.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/core/process.py` & `DeepTile-2.0.4/deeptile/core/process.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/core/profiles.py` & `DeepTile-2.0.4/deeptile/core/profiles.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/core/trees.py` & `DeepTile-2.0.4/deeptile/core/trees.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/core/utils.py` & `DeepTile-2.0.4/deeptile/core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
     tiled_coords = np.empty(n_batches, dtype=object)
 
     for n in range(n_batches):
 
         coord = coords[n]
 
-        s = (tile_index[0, 0] < coord[:, 0]) & (coord[:, 0] < tile_index[0, 1]) & \
-            (tile_index[1, 0] < coord[:, 1]) & (coord[:, 1] < tile_index[1, 1])
+        s = (tile_index[0, 0] - 0.5 < coord[:, 0]) & (coord[:, 0] < tile_index[0, 1] - 0.5) & \
+            (tile_index[1, 0] - 0.5 < coord[:, 1]) & (coord[:, 1] < tile_index[1, 1] - 0.5)
         tiled_coords[n] = coord[s] - tile_index[:, 0]
 
     if not batch_axis:
         tiled_coords = tiled_coords[0]
 
     return tiled_coords
```

### Comparing `DeepTile-2.0.3/deeptile/deeptile.py` & `DeepTile-2.0.4/deeptile/deeptile.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/extensions/segmentation.py` & `DeepTile-2.0.4/deeptile/extensions/segmentation.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/extensions/stitch.py` & `DeepTile-2.0.4/deeptile/extensions/stitch.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/io.py` & `DeepTile-2.0.4/deeptile/io.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/sources/function.py` & `DeepTile-2.0.4/deeptile/sources/function.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/sources/large_image.py` & `DeepTile-2.0.4/deeptile/sources/large_image.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/deeptile/sources/nd2.py` & `DeepTile-2.0.4/deeptile/sources/nd2.py`

 * *Files identical despite different names*

### Comparing `DeepTile-2.0.3/pyproject.toml` & `DeepTile-2.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DeepTile"
-version = "2.0.3"
+version = "2.0.4"
 description = "Large image tiling and stitching library for scaling Python functions to arbitrary input image sizes."
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [
     {email = "wniu721@gmail.com"},
     {name = "William Niu"}
 ]
```


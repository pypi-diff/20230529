# Comparing `tmp/prose-3.1.0.tar.gz` & `tmp/prose-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prose-3.1.0.tar", max compression
+gzip compressed data, was "prose-3.1.1.tar", max compression
```

## Comparing `prose-3.1.0.tar` & `prose-3.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     1097 2023-05-18 14:50:31.358570 prose-3.1.0/LICENSE
--rw-r--r--   0        0        0     3752 2023-05-18 14:50:31.358570 prose-3.1.0/README.md
--rw-r--r--   0        0        0      651 2023-05-18 14:50:31.462571 prose-3.1.0/prose/__init__.py
--rw-r--r--   0        0        0       84 2023-05-18 14:50:31.462571 prose-3.1.0/prose/archive/__init__.py
--rw-r--r--   0        0        0     2397 2023-05-18 14:50:31.462571 prose-3.1.0/prose/archive/pos1.py
--rw-r--r--   0        0        0     2071 2023-05-18 14:50:31.462571 prose-3.1.0/prose/archive/sdss.py
--rw-r--r--   0        0        0      254 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/__init__.py
--rw-r--r--   0        0        0     3970 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/alignment.py
--rw-r--r--   0        0        0     3680 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/background.py
--rw-r--r--   0        0        0     8982 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/catalogs.py
--rw-r--r--   0        0        0     8768 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/centroids.py
--rw-r--r--   0        0        0    13494 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/detection.py
--rw-r--r--   0        0        0     6717 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/geometry.py
--rw-r--r--   0        0        0     4135 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/photometry.py
--rw-r--r--   0        0        0    13998 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/psf.py
--rw-r--r--   0        0        0     3703 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/shepard.py
--rw-r--r--   0        0        0    20531 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/utils.py
--rw-r--r--   0        0        0     4034 2023-05-18 14:50:31.462571 prose-3.1.0/prose/blocks/visualization.py
--rw-r--r--   0        0        0     4069 2023-05-18 14:50:31.462571 prose-3.1.0/prose/builtins.py
--rw-r--r--   0        0        0    10678 2023-05-18 14:50:31.462571 prose-3.1.0/prose/citations.py
--rw-r--r--   0        0        0     5933 2023-05-18 14:50:31.462571 prose-3.1.0/prose/config.py
--rw-r--r--   0        0        0     3733 2023-05-18 14:50:31.462571 prose-3.1.0/prose/console_utils.py
--rw-r--r--   0        0        0      120 2023-05-18 14:50:31.462571 prose-3.1.0/prose/core/__init__.py
--rw-r--r--   0        0        0     3651 2023-05-18 14:50:31.462571 prose-3.1.0/prose/core/block.py
--rw-r--r--   0        0        0    24631 2023-05-18 14:50:31.462571 prose-3.1.0/prose/core/image.py
--rw-r--r--   0        0        0     9842 2023-05-18 14:50:31.462571 prose-3.1.0/prose/core/sequence.py
--rw-r--r--   0        0        0    16435 2023-05-18 14:50:31.462571 prose-3.1.0/prose/core/source.py
--rw-r--r--   0        0        0    17451 2023-05-18 14:50:31.462571 prose-3.1.0/prose/fluxes.py
--rw-r--r--   0        0        0      137 2023-05-18 14:50:31.462571 prose-3.1.0/prose/io/__init__.py
--rw-r--r--   0        0        0      686 2023-05-18 14:50:31.462571 prose-3.1.0/prose/io/create_fm_db.sql
--rw-r--r--   0        0        0    25095 2023-05-18 14:50:31.462571 prose-3.1.0/prose/io/fitsmanager.py
--rw-r--r--   0        0        0     6374 2023-05-18 14:50:31.462571 prose-3.1.0/prose/io/io.py
--rw-r--r--   0        0        0    15085 2023-05-18 14:50:31.462571 prose-3.1.0/prose/simulations.py
--rw-r--r--   0        0        0     7901 2023-05-18 14:50:31.462571 prose-3.1.0/prose/telescope.py
--rw-r--r--   0        0        0    14447 2023-05-18 14:50:31.462571 prose-3.1.0/prose/utils.py
--rw-r--r--   0        0        0    29851 2023-05-18 14:50:31.462571 prose-3.1.0/prose/visualization.py
--rw-r--r--   0        0        0     1007 2023-05-18 14:50:31.462571 prose-3.1.0/pyproject.toml
--rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 prose-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-29 12:33:24.642265 prose-3.1.1/LICENSE
+-rw-r--r--   0        0        0     3752 2023-05-29 12:33:24.642265 prose-3.1.1/README.md
+-rw-r--r--   0        0        0      651 2023-05-29 12:33:24.746264 prose-3.1.1/prose/__init__.py
+-rw-r--r--   0        0        0       84 2023-05-29 12:33:24.746264 prose-3.1.1/prose/archive/__init__.py
+-rw-r--r--   0        0        0     2397 2023-05-29 12:33:24.750264 prose-3.1.1/prose/archive/pos1.py
+-rw-r--r--   0        0        0     2071 2023-05-29 12:33:24.750264 prose-3.1.1/prose/archive/sdss.py
+-rw-r--r--   0        0        0      254 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/__init__.py
+-rw-r--r--   0        0        0     3970 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/alignment.py
+-rw-r--r--   0        0        0     3680 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/background.py
+-rw-r--r--   0        0        0     9026 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/catalogs.py
+-rw-r--r--   0        0        0     8768 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/centroids.py
+-rw-r--r--   0        0        0    13494 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/detection.py
+-rw-r--r--   0        0        0     6717 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/geometry.py
+-rw-r--r--   0        0        0     4135 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/photometry.py
+-rw-r--r--   0        0        0    13998 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/psf.py
+-rw-r--r--   0        0        0     3703 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/shepard.py
+-rw-r--r--   0        0        0    20531 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/utils.py
+-rw-r--r--   0        0        0     4034 2023-05-29 12:33:24.750264 prose-3.1.1/prose/blocks/visualization.py
+-rw-r--r--   0        0        0     4069 2023-05-29 12:33:24.750264 prose-3.1.1/prose/builtins.py
+-rw-r--r--   0        0        0    10673 2023-05-29 12:33:24.750264 prose-3.1.1/prose/citations.py
+-rw-r--r--   0        0        0     5933 2023-05-29 12:33:24.750264 prose-3.1.1/prose/config.py
+-rw-r--r--   0        0        0     3733 2023-05-29 12:33:24.750264 prose-3.1.1/prose/console_utils.py
+-rw-r--r--   0        0        0      120 2023-05-29 12:33:24.750264 prose-3.1.1/prose/core/__init__.py
+-rw-r--r--   0        0        0     3651 2023-05-29 12:33:24.750264 prose-3.1.1/prose/core/block.py
+-rw-r--r--   0        0        0    24769 2023-05-29 12:33:24.750264 prose-3.1.1/prose/core/image.py
+-rw-r--r--   0        0        0     9842 2023-05-29 12:33:24.750264 prose-3.1.1/prose/core/sequence.py
+-rw-r--r--   0        0        0    16539 2023-05-29 12:33:24.750264 prose-3.1.1/prose/core/source.py
+-rw-r--r--   0        0        0    17451 2023-05-29 12:33:24.750264 prose-3.1.1/prose/fluxes.py
+-rw-r--r--   0        0        0      137 2023-05-29 12:33:24.750264 prose-3.1.1/prose/io/__init__.py
+-rw-r--r--   0        0        0      686 2023-05-29 12:33:24.750264 prose-3.1.1/prose/io/create_fm_db.sql
+-rw-r--r--   0        0        0    25095 2023-05-29 12:33:24.750264 prose-3.1.1/prose/io/fitsmanager.py
+-rw-r--r--   0        0        0     6374 2023-05-29 12:33:24.750264 prose-3.1.1/prose/io/io.py
+-rw-r--r--   0        0        0    15085 2023-05-29 12:33:24.750264 prose-3.1.1/prose/simulations.py
+-rw-r--r--   0        0        0     7901 2023-05-29 12:33:24.750264 prose-3.1.1/prose/telescope.py
+-rw-r--r--   0        0        0    14447 2023-05-29 12:33:24.750264 prose-3.1.1/prose/utils.py
+-rw-r--r--   0        0        0    29851 2023-05-29 12:33:24.750264 prose-3.1.1/prose/visualization.py
+-rw-r--r--   0        0        0     1024 2023-05-29 12:33:24.750264 prose-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4821 1970-01-01 00:00:00.000000 prose-3.1.1/PKG-INFO
```

### Comparing `prose-3.1.0/LICENSE` & `prose-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/README.md` & `prose-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/__init__.py` & `prose-3.1.1/prose/__init__.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/archive/pos1.py` & `prose-3.1.1/prose/archive/pos1.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/archive/sdss.py` & `prose-3.1.1/prose/archive/sdss.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/blocks/alignment.py` & `prose-3.1.1/prose/blocks/alignment.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/blocks/background.py` & `prose-3.1.1/prose/blocks/background.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/blocks/catalogs.py` & `prose-3.1.1/prose/blocks/catalogs.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,16 @@
                 stars_coords > 0, 1
             )
             mask = mask & ~np.any(np.isnan(stars_coords), 1)
             image.sources = Sources(
                 [
                     PointSource(coords=s, i=i)
                     for i, s in enumerate(stars_coords[mask][0 : self.limit])
-                ]
+                ],
+                source_type="PointSource",
             )
             catalog = catalog.iloc[np.flatnonzero(mask)].reset_index()
 
         elif self.mode == "crossmatch":
             coords_1 = image.sources.coords
             coords_2 = catalog[["x", "y"]].values
```

### Comparing `prose-3.1.0/prose/blocks/centroids.py` & `prose-3.1.1/prose/blocks/centroids.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/blocks/detection.py` & `prose-3.1.1/prose/blocks/detection.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/blocks/geometry.py` & `prose-3.1.1/prose/blocks/geometry.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/blocks/photometry.py` & `prose-3.1.1/prose/blocks/photometry.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/blocks/psf.py` & `prose-3.1.1/prose/blocks/psf.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/blocks/shepard.py` & `prose-3.1.1/prose/blocks/shepard.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/blocks/utils.py` & `prose-3.1.1/prose/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/blocks/visualization.py` & `prose-3.1.1/prose/blocks/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/builtins.py` & `prose-3.1.1/prose/builtins.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/citations.py` & `prose-3.1.1/prose/citations.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  pages = {357--362},
  doi = {10.1038/s41586-020-2649-2},
  publisher = {Springer Science and Business Media {LLC}},
  url = {https://doi.org/10.1038/s41586-020-2649-2}
 }
 """,
     "astropy": """
-    @ARTICLE{astropy:2022,
+    @ARTICLE{astropy,
        author = {{Astropy Collaboration} and {Price-Whelan}, Adrian M. and {Lim}, Pey
        Lian and {Earl}, Nicholas and {Starkman}, Nathaniel and {Bradley}, Larry and
        {Shupe}, David L. and {Patil}, Aarya A. and {Corrales}, Lia and {Brasseur}, C.~E.
        and {N{\"o}the}, Maximilian and {Donath}, Axel and {Tollerud}, Erik and {Morris},
        Brett M. and {Ginsburg}, Adam and {Vaher}, Eero and {Weaver}, Benjamin A. and
        {Tocknell}, James and {Jamieson}, William and {van Kerkwijk}, Marten H. and
        {Robitaille}, Thomas P. and {Merry}, Bruce and {Bachetti}, Matteo and
```

### Comparing `prose-3.1.0/prose/config.py` & `prose-3.1.1/prose/config.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/console_utils.py` & `prose-3.1.1/prose/console_utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/core/block.py` & `prose-3.1.1/prose/core/block.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/core/image.py` & `prose-3.1.1/prose/core/image.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,15 +503,15 @@
         im_dict = asdict(self.copy())
         if low_data:
             im_dict["data"] = utils.z_scale(im_dict["data"]) * (2**7 - 1)
             image_dtype = "int8"
         im_dict["data"] = im_dict["data"].astype(image_dtype)
         return im_dict
 
-    def save(self, filepath, image_dtype="float64", low_data=True):
+    def save(self, filepath, image_dtype="float64", low_data=False):
         """
         Save the image to a file using pickle.
 
         Note that the pickle will hold the Image dataclass dict attributes.
 
         Parameters
         ----------
@@ -646,27 +646,30 @@
 
 def FITSImage(
     filepath_or_hdu: Union[str, Path, _BaseHDU],
     verbose: bool = False,
     load_units: bool = True,
     load_data: bool = True,
     telescope: Telescope = None,
+    skip_wcs: bool = False,
 ) -> Image:
     """Create an image from a FITS file
 
     Parameters
     ----------
     filepath_or_hdu : str
         path of fits file of HDU object
     verbose : bool, optional
         whether to be verbose, by default False
     load_units : bool, optional
         whether to load metadata units, by default True
     load_data : bool, optional
         whether to load image data, by default True
+    skip_wcs : bool, optional
+        whether to skip WCS loading, by default False
 
     Returns
     -------
     :py:class:`~prose.Image`
     """
     if isinstance(filepath_or_hdu, (str, Path)):
         values = fits.getdata(filepath_or_hdu).astype(float) if load_data else None
@@ -711,15 +714,16 @@
             }
         )
 
     image = Image(values, metadata, {})
     if image.metadata["jd"] is None:
         image.metadata["jd"] = Time(image.date).jd
     image.fits_header = header
-    image.wcs = WCS(header)
+    if not skip_wcs:
+        image.wcs = WCS(header)
     image.telescope = telescope
 
     return image
 
 
 class Buffer:
     def __init__(self, size: int, loader: callable = None):
```

### Comparing `prose-3.1.0/prose/core/sequence.py` & `prose-3.1.1/prose/core/sequence.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/core/source.py` & `prose-3.1.1/prose/core/source.py`

 * *Files 1% similar despite different names*

```diff
@@ -301,14 +301,19 @@
     def rectangular_annulus(self, r0, r1, scale=False):
         if scale:
             a0 = 2 * r0 * self.a
             a1, b1 = 2 * r1 * self.a, 2 * r1 * self.b
         else:
             a0 = r0
             a1, b1 = r1, r1 * self.eccentricity
+
+        a0 = np.max([0.01, a0])
+        a1 = np.max([a0 + 0.001, a1])
+        b1 = np.max([0.01, b1])
+
         return RectangularAnnulus(self.coords, a0, a1, b1, theta=self.orientation)
 
     def fit_isophotes(self, debug=False):
         """Fit a photutils.isophote.Ellipse to the source. Requires the source to be instantiated from a skimage RegionProperties
 
         Parameters
         ----------
```

### Comparing `prose-3.1.0/prose/fluxes.py` & `prose-3.1.1/prose/fluxes.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/io/create_fm_db.sql` & `prose-3.1.1/prose/io/create_fm_db.sql`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/io/fitsmanager.py` & `prose-3.1.1/prose/io/fitsmanager.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/io/io.py` & `prose-3.1.1/prose/io/io.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/simulations.py` & `prose-3.1.1/prose/simulations.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/telescope.py` & `prose-3.1.1/prose/telescope.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/utils.py` & `prose-3.1.1/prose/utils.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/prose/visualization.py` & `prose-3.1.1/prose/visualization.py`

 * *Files identical despite different names*

### Comparing `prose-3.1.0/pyproject.toml` & `prose-3.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "prose"
-version = "3.1.0"
+version = "3.1.1"
 description = "Modular image processing pipelines for Astronomy"
 authors = ["Lionel Garcia"]
 license = "MIT"
 readme = "README.md"
 include = ["prose/io/*.sql"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
 numpy = "^1.23.5"
 astropy = "^5.1.1"
 astroquery = "^0.4.6"
-requests = "^2.28.1"
+requests = "^2.31.0"
 ipython = "*"
 scipy = "*"
 matplotlib = "*"
 scikit-image = "*"
 pandas = ">1.1"
 tqdm = "*"
 photutils = "^1.6.0"
@@ -43,11 +43,12 @@
 jupyterlab = "*"
 myst-parser = "*"
 sphinx-book-theme = "^1.0.0"
 myst-nb = "*"
 sphinx-copybutton = "*"
 sphinx-design = "*"
 toml = "*"
+ipywidgets = "*"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `prose-3.1.0/PKG-INFO` & `prose-3.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prose
-Version: 3.1.0
+Version: 3.1.1
 Summary: Modular image processing pipelines for Astronomy
 License: MIT
 Author: Lionel Garcia
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -19,15 +19,15 @@
 Requires-Dist: matplotlib
 Requires-Dist: multiprocess
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>1.1)
 Requires-Dist: photutils (>=1.6.0,<2.0.0)
 Requires-Dist: pytest
 Requires-Dist: pyyaml
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scikit-image
 Requires-Dist: scipy
 Requires-Dist: sep
 Requires-Dist: tabulate
 Requires-Dist: tqdm
 Requires-Dist: twirl (==0.1.3)
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-Metadata-Version: 2.1 Name: prose Version: 3.1.0 Summary: Modular image
+Metadata-Version: 2.1 Name: prose Version: 3.1.1 Summary: Modular image
 processing pipelines for Astronomy License: MIT Author: Lionel Garcia Requires-
 Python: >=3.8,<3.12 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: astropy (>=5.1.1,<6.0.0) Requires-
 Dist: astroquery (>=0.4.6,<0.5.0) Requires-Dist: celerite2 Requires-Dist:
 imageio[ffmpeg] Requires-Dist: ipython Requires-Dist: matplotlib Requires-Dist:
 multiprocess Requires-Dist: numpy (>=1.23.5,<2.0.0) Requires-Dist: pandas
 (>1.1) Requires-Dist: photutils (>=1.6.0,<2.0.0) Requires-Dist: pytest
-Requires-Dist: pyyaml Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-Dist:
+Requires-Dist: pyyaml Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-Dist:
 scikit-image Requires-Dist: scipy Requires-Dist: sep Requires-Dist: tabulate
 Requires-Dist: tqdm Requires-Dist: twirl (==0.1.3) Description-Content-Type:
 text/markdown # prose
                            [docs/_static/prose3.png]
                Modular image processing pipelines for Astronomy
                   [github] [license] [paper] [documentation]
 *prose* is a Python package to build image processing pipelines for Astronomy.
```


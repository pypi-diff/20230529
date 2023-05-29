# Comparing `tmp/raster2dggs-0.2.2.tar.gz` & `tmp/raster2dggs-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raster2dggs-0.2.2.tar", max compression
+gzip compressed data, was "raster2dggs-0.2.3.tar", max compression
```

## Comparing `raster2dggs-0.2.2.tar` & `raster2dggs-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     8424 2023-05-22 23:16:34.972155 raster2dggs-0.2.2/README.md
--rw-r--r--   0        0        0     1091 2023-05-22 23:16:41.480189 raster2dggs-0.2.2/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-03 02:59:48.530270 raster2dggs-0.2.2/raster2dggs/__init__.py
--rw-r--r--   0        0        0      599 2023-05-03 02:59:13.750096 raster2dggs-0.2.2/raster2dggs/cli.py
--rw-r--r--   0        0        0    16047 2023-05-22 23:16:08.684017 raster2dggs-0.2.2/raster2dggs/h3.py
--rw-r--r--   0        0        0     9843 1970-01-01 00:00:00.000000 raster2dggs-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     8424 2023-05-29 04:53:57.799276 raster2dggs-0.2.3/README.md
+-rw-r--r--   0        0        0     1091 2023-05-29 04:53:48.071226 raster2dggs-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-03 02:59:48.530270 raster2dggs-0.2.3/raster2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-03 02:59:13.750096 raster2dggs-0.2.3/raster2dggs/cli.py
+-rw-r--r--   0        0        0    16113 2023-05-29 04:51:21.506487 raster2dggs-0.2.3/raster2dggs/h3.py
+-rw-r--r--   0        0        0     9843 1970-01-01 00:00:00.000000 raster2dggs-0.2.3/PKG-INFO
```

### Comparing `raster2dggs-0.2.2/README.md` & `raster2dggs-0.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -148,17 +148,17 @@
 ## Citation
 
 ```bibtex
 @software{raster2dggs,
   title={{raster2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/raster2dggs},
-  version={0.2.2},
+  version={0.2.3},
   date={2023-02-09}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). raster2dggs (0.2.2) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
+> Ardo, J., & Law, R. (2023). raster2dggs (0.2.3) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/raster2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `raster2dggs-0.2.2/pyproject.toml` & `raster2dggs-0.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "raster2dggs"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/raster2dggs"
 keywords = ["dggs", "raster", "h3", "cli"]
```

### Comparing `raster2dggs-0.2.2/raster2dggs/cli.py` & `raster2dggs-0.2.3/raster2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `raster2dggs-0.2.2/raster2dggs/h3.py` & `raster2dggs-0.2.3/raster2dggs/h3.py`

 * *Files 1% similar despite different names*

```diff
@@ -284,14 +284,15 @@
             )
             .to_parquet(
                 output,
                 overwrite=kwargs["overwrite"],
                 engine="pyarrow",
                 write_index=True,
                 append=False,
+                name_function=lambda i: f'{uniqueh3[i]}.parquet',
                 compression=kwargs["compression"],
             )
         )
 
     LOGGER.debug(
         "Stage 2 (parent cell repartioning) and Stage 3 (aggregation) complete"
     )
```

### Comparing `raster2dggs-0.2.2/PKG-INFO` & `raster2dggs-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raster2dggs
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Home-page: https://github.com/manaakiwhenua/raster2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,raster,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -183,18 +183,18 @@
 ## Citation
 
 ```bibtex
 @software{raster2dggs,
   title={{raster2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/raster2dggs},
-  version={0.2.2},
+  version={0.2.3},
   date={2023-02-09}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). raster2dggs (0.2.2) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
+> Ardo, J., & Law, R. (2023). raster2dggs (0.2.3) [Computer software]. https://github.com/manaakiwhenua/raster2dggs 
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/raster2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```


# Comparing `tmp/ssb_sgis-0.2.2.tar.gz` & `tmp/ssb_sgis-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.2.2.tar", max compression
+gzip compressed data, was "ssb_sgis-0.2.3.tar", max compression
```

## Comparing `ssb_sgis-0.2.2.tar` & `ssb_sgis-0.2.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1074 2023-05-23 20:38:37.915335 ssb_sgis-0.2.2/LICENSE
--rw-r--r--   0        0        0     7543 2023-05-23 20:38:37.915335 ssb_sgis-0.2.2/README.md
--rw-r--r--   0        0        0     2539 2023-05-23 20:38:52.283685 ssb_sgis-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2230 2023-05-23 20:38:37.943336 ssb_sgis-0.2.2/src/sgis/__init__.py
--rw-r--r--   0        0        0     3243 2023-05-23 20:38:37.943336 ssb_sgis-0.2.2/src/sgis/dapla.py
--rw-r--r--   0        0        0      576 2023-05-23 20:38:37.943336 ssb_sgis-0.2.2/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-23 20:38:37.943336 ssb_sgis-0.2.2/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8028 2023-05-23 20:38:37.943336 ssb_sgis-0.2.2/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    23937 2023-05-23 20:38:37.943336 ssb_sgis-0.2.2/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5480 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    14520 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    11815 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6888 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0    13161 2023-05-23 20:38:52.283685 ssb_sgis-0.2.2/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     9722 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/geopandas_tools/to_geodataframe.py
--rw-r--r--   0        0        0     2674 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0    20484 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/maps/explore.py
--rw-r--r--   0        0        0     1938 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/maps/httpserver.py
--rw-r--r--   0        0        0    20499 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    17448 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/maps/map.py
--rw-r--r--   0        0        0    16009 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    14132 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6218 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2017 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4206 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4487 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    12433 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/closing_network_holes.py
--rw-r--r--   0        0        0    11984 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/cutting_lines.py
--rw-r--r--   0        0        0     9375 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0     3359 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/finding_isolated_networks.py
--rw-r--r--   0        0        0     7686 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0    66761 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12643 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0     6740 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/networkanalysis/nodes.py
--rw-r--r--   0        0        0        0 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/py.typed
--rw-r--r--   0        0        0     3774 2023-05-23 20:38:37.947336 ssb_sgis-0.2.2/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-29 21:43:46.710242 ssb_sgis-0.2.3/LICENSE
+-rw-r--r--   0        0        0     7543 2023-05-29 21:43:46.710242 ssb_sgis-0.2.3/README.md
+-rw-r--r--   0        0        0     2539 2023-05-29 21:44:06.034292 ssb_sgis-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     2309 2023-05-29 21:44:06.034292 ssb_sgis-0.2.3/src/sgis/__init__.py
+-rw-r--r--   0        0        0     3243 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/dapla.py
+-rw-r--r--   0        0        0      576 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8028 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    23937 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5480 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    14520 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    11815 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6888 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0    18319 2023-05-29 21:44:06.034292 ssb_sgis-0.2.3/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     9722 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/geopandas_tools/to_geodataframe.py
+-rw-r--r--   0        0        0     2674 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0    20484 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0     1938 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/maps/httpserver.py
+-rw-r--r--   0        0        0    20499 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    17448 2023-05-29 21:43:46.750243 ssb_sgis-0.2.3/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    16009 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14132 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6218 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2017 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4206 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4487 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    12433 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    11984 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0     9375 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3359 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     7686 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    66761 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12643 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6740 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0        0 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/py.typed
+-rw-r--r--   0        0        0     3774 2023-05-29 21:43:46.754243 ssb_sgis-0.2.3/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.3/PKG-INFO
```

### Comparing `ssb_sgis-0.2.2/LICENSE` & `ssb_sgis-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/README.md` & `ssb_sgis-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/pyproject.toml` & `ssb_sgis-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.2.2"
+version = "0.2.3"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
```

### Comparing `ssb_sgis-0.2.2/src/sgis/__init__.py` & `ssb_sgis-0.2.3/src/sgis/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     k_nearest_neighbors,
 )
 from .geopandas_tools.overlay import clean_overlay, overlay_update
 from .geopandas_tools.point_operations import snap_all, snap_within_distance
 from .geopandas_tools.polygon_operations import (
     close_all_holes,
     close_small_holes,
+    eliminate_by_largest,
+    eliminate_by_longest,
+    eliminate_by_smallest,
     get_overlapping_polygon_indices,
     get_overlapping_polygon_product,
     get_overlapping_polygons,
     get_polygon_clusters,
 )
 from .geopandas_tools.to_geodataframe import to_gdf
 from .maps.explore import Explore
```

### Comparing `ssb_sgis-0.2.2/src/sgis/dapla.py` & `ssb_sgis-0.2.3/src/sgis/dapla.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/exceptions.py` & `ssb_sgis-0.2.3/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.2.3/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.2.3/src/sgis/geopandas_tools/general.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.2.3/src/sgis/geopandas_tools/geometry_types.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.2.3/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.2.3/src/sgis/geopandas_tools/overlay.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.2.3/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.2.3/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,19 +11,181 @@
     get_interior_ring,
     get_num_interior_rings,
     get_parts,
     polygons,
 )
 from shapely.ops import unary_union
 
-from .general import _push_geom_col
+from .general import _push_geom_col, to_lines
 from .neighbors import get_neighbor_indices
 from .overlay import clean_overlay
 
 
+def eliminate_by_longest(
+    gdf: GeoDataFrame,
+    min_area: int | float,
+    ignore_index: bool = False,
+    aggfunc: str | dict | list = "first",
+    **kwargs,
+) -> GeoDataFrame:
+    """Dissolves small polygons with the longest bordering neighbor polygon.
+
+    Eliminates small geometries by dissolving them with the neighboring
+    polygon with the longest shared border. The index and column values of the
+    large polygons will be kept, unless else is specified.
+
+    Args:
+        gdf: GeoDataFrame with polygon geometries.
+        min_area: minimum area for the polygons to be eliminated.
+        ignore_index: If False (default), the resulting GeoDataFrame will keep the
+            index of the large polygons. If True, the resulting axis will be labeled
+            0, 1, …, n - 1.
+        aggfunc: Aggregation function(s) to use when dissolving. Defaults to 'first',
+            meaning the column values of the large polygons are kept.
+        kwargs: Keyword arguments passed to the dissolve method.
+
+    Returns:
+        The GeoDataFrame with the small polygons dissolved into the large polygons.
+    """
+    if not ignore_index:
+        idx_mapper = {i: idx for i, idx in enumerate(gdf.index)}
+        idx_name = gdf.index.name
+
+    gdf = gdf.reset_index(drop=True)
+
+    small = gdf.loc[gdf.area <= min_area].assign(small_idx=lambda x: x.index)
+    large = gdf.loc[gdf.area > min_area].assign(large_idx=lambda x: x.index)
+
+    lines = to_lines(small[["small_idx", "geometry"]], large[["large_idx", "geometry"]])
+    lines = lines[lines["small_idx"].notna()]
+    lines["length__"] = lines.length
+
+    longest = lines.sort_values("length__", ascending=False).drop_duplicates(
+        "small_idx"
+    )
+
+    small_to_large = longest.set_index("small_idx")["large_idx"]
+    small["dissolve_idx"] = small["small_idx"].map(small_to_large)
+    large["dissolve_idx"] = large["large_idx"]
+
+    kwargs.pop("as_index", None)
+    eliminated = (
+        pd.concat([large, small])
+        .dissolve("dissolve_idx", aggfunc=aggfunc, **kwargs)
+        .drop(
+            ["length__", "small_idx", "large_idx"],
+            axis=1,
+            errors="ignore",
+        )
+    )
+
+    if ignore_index:
+        return eliminated.reset_index(drop=True)
+
+    eliminated.index = eliminated.index.map(idx_mapper)
+    eliminated.index.name = idx_name
+
+    return eliminated
+
+
+def eliminate_by_largest(
+    gdf: GeoDataFrame,
+    min_area: int | float,
+    ignore_index: bool = False,
+    aggfunc: str | dict | list = "first",
+    **kwargs,
+) -> GeoDataFrame:
+    """Dissolves small polygons with the largest neighbor polygon.
+
+    Eliminates small geometries by dissolving them with the neighboring
+    polygon with the largest area. The index and column values of the
+    large polygons will be kept, unless else is specified.
+
+    Args:
+        gdf: GeoDataFrame with polygon geometries.
+        min_area: minimum area for the polygons to be eliminated.
+        ignore_index: If False (default), the resulting GeoDataFrame will keep the
+            index of the large polygons. If True, the resulting axis will be labeled
+            0, 1, …, n - 1.
+        aggfunc: Aggregation function(s) to use when dissolving. Defaults to 'first',
+            meaning the column values of the large polygons are kept.
+        kwargs: Keyword arguments passed to the dissolve method.
+
+    Returns:
+        The GeoDataFrame with the small polygons dissolved into the large polygons.
+    """
+    return _eliminate_by_area(
+        gdf,
+        min_area=min_area,
+        ignore_index=ignore_index,
+        sort_ascending=False,
+        aggfunc=aggfunc,
+        **kwargs,
+    )
+
+
+def eliminate_by_smallest(
+    gdf: GeoDataFrame,
+    min_area: int | float,
+    ignore_index: bool = False,
+    aggfunc: str | dict | list = "first",
+    **kwargs,
+) -> GeoDataFrame:
+    return _eliminate_by_area(
+        gdf,
+        min_area=min_area,
+        ignore_index=ignore_index,
+        sort_ascending=True,
+        aggfunc=aggfunc,
+        **kwargs,
+    )
+
+
+def _eliminate_by_area(
+    gdf: GeoDataFrame,
+    min_area: int | float,
+    sort_ascending: bool,
+    ignore_index: bool = False,
+    aggfunc="first",
+    **kwargs,
+) -> GeoDataFrame:
+    if not ignore_index:
+        idx_mapper = {i: idx for i, idx in enumerate(gdf.index)}
+        idx_name = gdf.index.name
+
+    gdf = gdf.reset_index(drop=True)
+
+    small = gdf.loc[gdf.area <= min_area]
+    large = gdf.loc[gdf.area > min_area]
+    large["area__"] = large.area
+
+    joined = small.sjoin(
+        large[["area__", "geometry"]], predicate="touches"
+    ).sort_values("area__", ascending=sort_ascending)
+
+    largest = joined[~joined.index.duplicated()]
+
+    large = large.assign(index_right=lambda x: x.index)
+
+    kwargs.pop("as_index", None)
+    eliminated = (
+        pd.concat([large, largest])
+        .dissolve("index_right", aggfunc=aggfunc, **kwargs)
+        .drop(["area__"], axis=1, errors="ignore")
+    )
+
+    if ignore_index:
+        return eliminated.reset_index(drop=True)
+
+    eliminated.index = eliminated.index.map(idx_mapper)
+    eliminated.index.name = idx_name
+
+    return eliminated
+
+
 def get_polygon_clusters(
     *gdfs: GeoDataFrame | GeoSeries,
     cluster_col: str = "cluster",
     allow_multipart: bool = False,
 ) -> GeoDataFrame | tuple[GeoDataFrame]:
     """Find which polygons overlap without dissolving.
 
@@ -157,15 +319,15 @@
         gdf = gdf.drop(["i__"], axis=1)
         unconcated = unconcated + (gdf,)
 
     return unconcated
 
 
 def get_overlapping_polygons(
-    gdf: GeoDataFrame | GeoSeries, ignore_index=False
+    gdf: GeoDataFrame | GeoSeries, ignore_index: bool = False
 ) -> GeoDataFrame | GeoSeries:
     """Find the areas that overlap.
 
     Does an intersection with itself and keeps only the duplicated geometries. The
     index of 'gdf' is preserved.
 
     Args:
```

### Comparing `ssb_sgis-0.2.2/src/sgis/geopandas_tools/to_geodataframe.py` & `ssb_sgis-0.2.3/src/sgis/geopandas_tools/to_geodataframe.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/helpers.py` & `ssb_sgis-0.2.3/src/sgis/helpers.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/maps/explore.py` & `ssb_sgis-0.2.3/src/sgis/maps/explore.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/maps/httpserver.py` & `ssb_sgis-0.2.3/src/sgis/maps/httpserver.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/maps/legend.py` & `ssb_sgis-0.2.3/src/sgis/maps/legend.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/maps/map.py` & `ssb_sgis-0.2.3/src/sgis/maps/map.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/maps/maps.py` & `ssb_sgis-0.2.3/src/sgis/maps/maps.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.2.3/src/sgis/maps/thematicmap.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/_get_route.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/closing_network_holes.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/closing_network_holes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/cutting_lines.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/cutting_lines.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/directednetwork.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/finding_isolated_networks.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/finding_isolated_networks.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/network.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/networkanalysis.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/networkanalysis/nodes.py` & `ssb_sgis-0.2.3/src/sgis/networkanalysis/nodes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/src/sgis/read_parquet.py` & `ssb_sgis-0.2.3/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.2/PKG-INFO` & `ssb_sgis-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.2.2
+Version: 0.2.3
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
```


# Comparing `tmp/timor_locations-0.0.2.tar.gz` & `tmp/timor_locations-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timor_locations-0.0.2.tar", max compression
+gzip compressed data, was "timor_locations-0.0.3.tar", max compression
```

## Comparing `timor_locations-0.0.2.tar` & `timor_locations-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,25 @@
--rw-r--r--   0        0        0     1029 2023-05-24 16:20:08.175041 timor_locations-0.0.2/README.md
--rw-r--r--   0        0        0     1734 2023-05-26 10:04:34.088710 timor_locations-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/__init__.py
--rw-r--r--   0        0        0      279 2023-05-26 06:37:53.703110 timor_locations-0.0.2/timor_locations/admin.py
--rw-r--r--   0        0        0      125 2023-05-26 06:37:53.699110 timor_locations-0.0.2/timor_locations/api.py
--rw-r--r--   0        0        0     1011 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/gis_functions.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/management/commands/__init__.py
--rw-r--r--   0        0        0     1273 2023-05-26 09:50:10.256772 timor_locations-0.0.2/timor_locations/management/commands/create_topology.py
--rw-r--r--   0        0        0     2726 2023-05-26 09:51:35.426460 timor_locations-0.0.2/timor_locations/management/commands/import_timor_geo_data.py
--rw-r--r--   0        0        0     3014 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1131 2023-05-24 16:14:01.023615 timor_locations-0.0.2/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py
--rw-r--r--   0        0        0     1401 2023-05-24 16:14:01.023615 timor_locations-0.0.2/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py
--rw-r--r--   0        0        0      887 2023-05-24 16:14:01.023615 timor_locations-0.0.2/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py
--rw-r--r--   0        0        0      783 2023-05-26 09:15:33.722459 timor_locations-0.0.2/timor_locations/migrations/0005_topojson.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/migrations/__init__.py
--rw-r--r--   0        0        0     4719 2023-05-26 09:55:46.818367 timor_locations-0.0.2/timor_locations/models.py
--rw-r--r--   0        0        0     1610 2023-05-26 09:50:10.276774 timor_locations-0.0.2/timor_locations/router.py
--rw-r--r--   0        0        0      983 2023-05-26 09:50:10.248771 timor_locations-0.0.2/timor_locations/schemas.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/settings.py
--rw-r--r--   0        0        0      213 2023-05-26 06:37:53.707110 timor_locations-0.0.2/timor_locations/urls.py
--rw-r--r--   0        0        0      414 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/wsgi.py
--rw-r--r--   0        0        0     1739 1970-01-01 00:00:00.000000 timor_locations-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1029 2023-05-24 16:20:08.175041 timor_locations-0.0.3/README.md
+-rw-r--r--   0        0        0     1808 2023-05-29 05:37:48.959199 timor_locations-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.3/timor_locations/__init__.py
+-rw-r--r--   0        0        0      279 2023-05-26 06:37:53.703110 timor_locations-0.0.3/timor_locations/admin.py
+-rw-r--r--   0        0        0      125 2023-05-26 06:37:53.699110 timor_locations-0.0.3/timor_locations/api.py
+-rw-r--r--   0        0        0     1011 2023-05-24 16:14:01.019615 timor_locations-0.0.3/timor_locations/gis_functions.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.3/timor_locations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.3/timor_locations/management/commands/__init__.py
+-rw-r--r--   0        0        0     1273 2023-05-26 09:50:10.256772 timor_locations-0.0.3/timor_locations/management/commands/create_topology.py
+-rw-r--r--   0        0        0     2726 2023-05-26 09:51:35.426460 timor_locations-0.0.3/timor_locations/management/commands/import_timor_geo_data.py
+-rw-r--r--   0        0        0     2285 2023-05-29 00:25:54.388811 timor_locations-0.0.3/timor_locations/management/commands/suco_to_topology.sql
+-rw-r--r--   0        0        0      801 2023-05-28 23:46:58.069787 timor_locations-0.0.3/timor_locations/management/commands/timor_topology.py
+-rw-r--r--   0        0        0     3014 2023-05-24 16:14:01.019615 timor_locations-0.0.3/timor_locations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1131 2023-05-24 16:14:01.023615 timor_locations-0.0.3/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py
+-rw-r--r--   0        0        0     1401 2023-05-24 16:14:01.023615 timor_locations-0.0.3/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py
+-rw-r--r--   0        0        0      887 2023-05-24 16:14:01.023615 timor_locations-0.0.3/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py
+-rw-r--r--   0        0        0      783 2023-05-26 09:15:33.722459 timor_locations-0.0.3/timor_locations/migrations/0005_topojson.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.3/timor_locations/migrations/__init__.py
+-rw-r--r--   0        0        0     4734 2023-05-29 05:04:41.005512 timor_locations-0.0.3/timor_locations/models.py
+-rw-r--r--   0        0        0     1610 2023-05-29 05:01:43.145478 timor_locations-0.0.3/timor_locations/router.py
+-rw-r--r--   0        0        0      977 2023-05-29 05:00:30.661276 timor_locations-0.0.3/timor_locations/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.3/timor_locations/settings.py
+-rw-r--r--   0        0        0      213 2023-05-26 06:37:53.707110 timor_locations-0.0.3/timor_locations/urls.py
+-rw-r--r--   0        0        0      414 2023-05-24 16:14:01.019615 timor_locations-0.0.3/timor_locations/wsgi.py
+-rw-r--r--   0        0        0     1739 1970-01-01 00:00:00.000000 timor_locations-0.0.3/PKG-INFO
```

### Comparing `timor_locations-0.0.2/README.md` & `timor_locations-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.2/pyproject.toml` & `timor_locations-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [tool.ruff]
 line-length = 119
 exclude = ['migrations']
 
 [tool.poetry]
 name = "timor-locations"
-version = "0.0.2"
+version = "0.0.3"
 description = "Timor-Leste geographic datasets"
 authors = [
   "Joshua Brooks <josh@catalpa.io>",
   "Anders Hofstee <anders@catalpa.io>",
 ]
 exclude = ["tests", "sl_tests", "timor_locations/data", "docs"]
 license = "GPLv3"
@@ -61,14 +61,15 @@
 django-extensions = "^3.2.1"
 
 [tool.poetry.group.topology]
 optional = true
 
 [tool.poetry.group.topology.dependencies]
 topojson = "^1.5"
+geojson = {git = "https://github.com/jazzband/geojson.git", rev = "main"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 plugins = ["mypy_django_plugin.main"]
```

### Comparing `timor_locations-0.0.2/timor_locations/gis_functions.py` & `timor_locations-0.0.3/timor_locations/gis_functions.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.2/timor_locations/management/commands/create_topology.py` & `timor_locations-0.0.3/timor_locations/management/commands/create_topology.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.2/timor_locations/management/commands/import_timor_geo_data.py` & `timor_locations-0.0.3/timor_locations/management/commands/import_timor_geo_data.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.2/timor_locations/migrations/0001_initial.py` & `timor_locations-0.0.3/timor_locations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.2/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py` & `timor_locations-0.0.3/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.2/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py` & `timor_locations-0.0.3/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.2/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py` & `timor_locations-0.0.3/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.2/timor_locations/migrations/0005_topojson.py` & `timor_locations-0.0.3/timor_locations/migrations/0005_topojson.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.2/timor_locations/models.py` & `timor_locations-0.0.3/timor_locations/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
         to fetch the GeoJSON.
         """
         if not hasattr(self, "geojson"):
             return MultiPolygon.construct(**json.loads(self.geom.json))
         return MultiPolygon.construct(**json.loads(self.geojson))
 
     def as_feature(self):
-        properties = dict(name = self.name, kind=self._meta.model_name)
+        properties = dict(name = self.name, id=self.pcode, kind=self._meta.model_name)
 
         for optional in ("adminpost_id", "municipality_id"):
             if hasattr(self, optional):
                 properties[optional] = getattr(self, optional)
             
         return Feature.construct(
             type="Feature", id=self.pcode, properties=properties, geometry=self.as_multipolygon()
```

### Comparing `timor_locations-0.0.2/timor_locations/router.py` & `timor_locations-0.0.3/timor_locations/router.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.2/timor_locations/schemas.py` & `timor_locations-0.0.3/timor_locations/schemas.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class Transform(BaseModel):
     scale: tuple[float, float]
     translate: tuple[float, float]
 
 
 class Topology(BaseModel):
-    type: str = Literal[
+    type: Literal[
         "Topology",
         "Point",
         "MultiPoint",
         "LineString",
         "MultiLineString",
         "Polygon",
         "MultiPolygon",
```

### Comparing `timor_locations-0.0.2/PKG-INFO` & `timor_locations-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timor-locations
-Version: 0.0.2
+Version: 0.0.3
 Summary: Timor-Leste geographic datasets
 Home-page: https://github.com/catalpainternational/timor_locations
 License: GPLv3
 Author: Joshua Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```


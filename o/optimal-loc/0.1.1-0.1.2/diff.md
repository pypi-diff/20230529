# Comparing `tmp/optimal_loc-0.1.1.tar.gz` & `tmp/optimal_loc-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.1.1.tar", max compression
+gzip compressed data, was "optimal_loc-0.1.2.tar", max compression
```

## Comparing `optimal_loc-0.1.1.tar` & `optimal_loc-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.1/LICENSE
--rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.1.1/README.md
--rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.1/optimal_loc/Modelling Algorithm.png
--rw-r--r--   0        0        0       87 2023-05-28 23:14:06.666468 optimal_loc-0.1.1/optimal_loc/__init__.py
--rw-r--r--   0        0        0    18104 2023-05-28 22:39:51.260202 optimal_loc-0.1.1/optimal_loc/app.py
--rw-r--r--   0        0        0      696 2023-05-28 22:37:44.186978 optimal_loc-0.1.1/optimal_loc/app_constants.py
--rw-r--r--   0        0        0      399 2023-05-28 22:39:51.274769 optimal_loc-0.1.1/optimal_loc/bash_command.py
--rw-r--r--   0        0        0     2680 2023-05-28 22:39:51.272259 optimal_loc-0.1.1/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-05-28 23:14:06.670872 optimal_loc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.2/LICENSE
+-rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.1.2/README.md
+-rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.2/optimal_loc/Modelling Algorithm.png
+-rw-r--r--   0        0        0       87 2023-05-28 23:21:52.311668 optimal_loc-0.1.2/optimal_loc/__init__.py
+-rw-r--r--   0        0        0    18115 2023-05-28 23:21:12.583110 optimal_loc-0.1.2/optimal_loc/app.py
+-rw-r--r--   0        0        0      696 2023-05-28 22:37:44.186978 optimal_loc-0.1.2/optimal_loc/app_constants.py
+-rw-r--r--   0        0        0      410 2023-05-28 23:21:17.917732 optimal_loc-0.1.2/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0     2691 2023-05-28 23:21:12.587249 optimal_loc-0.1.2/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-05-28 23:21:56.009013 optimal_loc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.1.2/PKG-INFO
```

### Comparing `optimal_loc-0.1.1/LICENSE` & `optimal_loc-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.1/README.md` & `optimal_loc-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.1/optimal_loc/Modelling Algorithm.png` & `optimal_loc-0.1.2/optimal_loc/Modelling Algorithm.png`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.1/optimal_loc/app.py` & `optimal_loc-0.1.2/optimal_loc/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from numpy import array, meshgrid, nan
 from pandas import DataFrame, pivot_table
 from pymongo.mongo_client import MongoClient
 from h3 import geo_to_h3, h3_to_geo, edge_length
 import pickle
 from pulp import LpProblem, LpMinimize, LpVariable, lpSum, PULP_CBC_CMD
 
-from .app_constants import (
+from optimal_loc.app_constants import (
     HEX_LAT, FROMHEX, TOHEX, HEX_LOCATION, SUPPLY_HEXAGON_ID, TOTAL_EVENT, HEX_ID, HEX_LON, HEXAGON_ID, LATITUDE,
     LONGITUDE, FROMHEX_LAT, FROMHEX_LON, HEXAGON, FILENAME, DISTANCE, SUPPLY_DATA_COLUMN, OPTIMAL_DATA_COLUMN, INDEX
 )
 
 
 def set_resolution(raw_data: DataFrame, hex_size: str):
     if hex_size == 'medium':
```

### Comparing `optimal_loc-0.1.1/optimal_loc/app_constants.py` & `optimal_loc-0.1.2/optimal_loc/app_constants.py`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.1/optimal_loc/st_app.py` & `optimal_loc-0.1.2/optimal_loc/st_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import streamlit as st
 from pandas import DataFrame
 from streamlit_folium import folium_static
 from pickle import load as pickle_load
 from folium import plugins, Map, CircleMarker, Marker, Icon
 from PIL import Image
 
-from .app_constants import COLOURS_LIST, FILENAME, OPTIMAL_DATA_COLUMN, SUPPLY_DATA_COLUMN, HEX_LAT, HEX_LON
+from optimal_loc.app_constants import COLOURS_LIST, FILENAME, OPTIMAL_DATA_COLUMN, SUPPLY_DATA_COLUMN, HEX_LAT, HEX_LON
 
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
 my_algorithm = Image.open(os.path.join(PACKAGE_DIR, 'Modelling Algorithm.png'))
 
 st.set_page_config(layout="wide")
```

### Comparing `optimal_loc-0.1.1/pyproject.toml` & `optimal_loc-0.1.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.1.1"
+version = "0.1.2"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.1.1/PKG-INFO` & `optimal_loc-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.1.1
+Version: 0.1.2
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
```


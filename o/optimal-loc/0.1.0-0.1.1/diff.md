# Comparing `tmp/optimal_loc-0.1.0.tar.gz` & `tmp/optimal_loc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimal_loc-0.1.0.tar", max compression
+gzip compressed data, was "optimal_loc-0.1.1.tar", max compression
```

## Comparing `optimal_loc-0.1.0.tar` & `optimal_loc-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.0/LICENSE
--rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.1.0/README.md
--rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.0/optimal_loc/Modelling Algorithm.png
--rw-r--r--   0        0        0       87 2023-05-28 22:20:04.958787 optimal_loc-0.1.0/optimal_loc/__init__.py
--rw-r--r--   0        0        0    18111 2023-05-27 14:15:21.582817 optimal_loc-0.1.0/optimal_loc/app.py
--rw-r--r--   0        0        0      406 2023-05-27 13:51:08.122984 optimal_loc-0.1.0/optimal_loc/bash_command.py
--rw-r--r--   0        0        0      731 2023-05-26 02:09:22.791228 optimal_loc-0.1.0/optimal_loc/constants.py
--rw-r--r--   0        0        0     2688 2023-05-27 13:51:08.119920 optimal_loc-0.1.0/optimal_loc/st_app.py
--rw-r--r--   0        0        0      857 2023-05-28 22:20:16.429528 optimal_loc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-04-30 23:15:49.879885 optimal_loc-0.1.1/LICENSE
+-rw-r--r--   0        0        0      552 2023-05-01 00:14:15.114286 optimal_loc-0.1.1/README.md
+-rw-r--r--   0        0        0   125580 2023-05-07 13:18:02.614960 optimal_loc-0.1.1/optimal_loc/Modelling Algorithm.png
+-rw-r--r--   0        0        0       87 2023-05-28 23:14:06.666468 optimal_loc-0.1.1/optimal_loc/__init__.py
+-rw-r--r--   0        0        0    18104 2023-05-28 22:39:51.260202 optimal_loc-0.1.1/optimal_loc/app.py
+-rw-r--r--   0        0        0      696 2023-05-28 22:37:44.186978 optimal_loc-0.1.1/optimal_loc/app_constants.py
+-rw-r--r--   0        0        0      399 2023-05-28 22:39:51.274769 optimal_loc-0.1.1/optimal_loc/bash_command.py
+-rw-r--r--   0        0        0     2680 2023-05-28 22:39:51.272259 optimal_loc-0.1.1/optimal_loc/st_app.py
+-rw-r--r--   0        0        0      857 2023-05-28 23:14:06.670872 optimal_loc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1772 1970-01-01 00:00:00.000000 optimal_loc-0.1.1/PKG-INFO
```

### Comparing `optimal_loc-0.1.0/LICENSE` & `optimal_loc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.0/README.md` & `optimal_loc-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.0/optimal_loc/Modelling Algorithm.png` & `optimal_loc-0.1.1/optimal_loc/Modelling Algorithm.png`

 * *Files identical despite different names*

### Comparing `optimal_loc-0.1.0/optimal_loc/app.py` & `optimal_loc-0.1.1/optimal_loc/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from numpy import array, meshgrid, nan
 from pandas import DataFrame, pivot_table
 from pymongo.mongo_client import MongoClient
 from h3 import geo_to_h3, h3_to_geo, edge_length
 import pickle
 from pulp import LpProblem, LpMinimize, LpVariable, lpSum, PULP_CBC_CMD
 
-from optimal_loc.constants import (
+from .app_constants import (
     HEX_LAT, FROMHEX, TOHEX, HEX_LOCATION, SUPPLY_HEXAGON_ID, TOTAL_EVENT, HEX_ID, HEX_LON, HEXAGON_ID, LATITUDE,
     LONGITUDE, FROMHEX_LAT, FROMHEX_LON, HEXAGON, FILENAME, DISTANCE, SUPPLY_DATA_COLUMN, OPTIMAL_DATA_COLUMN, INDEX
 )
 
 
 def set_resolution(raw_data: DataFrame, hex_size: str):
     if hex_size == 'medium':
```

### Comparing `optimal_loc-0.1.0/optimal_loc/constants.py` & `optimal_loc-0.1.1/optimal_loc/app_constants.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 00000000: 434f 4c4f 5552 535f 4c49 5354 203d 205b  COLOURS_LIST = [
 00000010: 0a20 2020 2027 6461 726b 7265 6427 2c0a  .    'darkred',.
 00000020: 2020 2020 276f 7261 6e67 6527 2c0a 2020      'orange',.  
 00000030: 2020 2764 6172 6b67 7265 656e 272c 0a20    'darkgreen',. 
 00000040: 2020 2027 6461 726b 626c 7565 272c 0a20     'darkblue',. 
 00000050: 2020 2027 7075 7270 6c65 272c 0a20 2020     'purple',.   
-00000060: 2027 6c69 6768 7467 7265 656e 272c 0a20   'lightgreen',. 
-00000070: 2020 2027 7069 6e6b 272c 0a20 2020 2027     'pink',.    '
-00000080: 6c69 6768 7462 6c75 6527 2c0a 2020 2020  lightblue',.    
-00000090: 2762 6c61 636b 270a 5d0a 0a44 4953 5441  'black'.]..DISTA
-000000a0: 4e43 4520 3d20 2764 6973 7461 6e63 6527  NCE = 'distance'
-000000b0: 0a46 494c 454e 414d 4520 3d20 276f 7074  .FILENAME = 'opt
-000000c0: 696d 616c 5f6c 6f63 6174 696f 6e73 2e70  imal_locations.p
-000000d0: 6963 6b6c 6527 0a46 524f 4d48 4558 203d  ickle'.FROMHEX =
-000000e0: 2027 6672 6f6d 6865 7827 0a54 4f48 4558   'fromhex'.TOHEX
-000000f0: 203d 2027 746f 6865 7827 0a0a 4652 4f4d   = 'tohex'..FROM
-00000100: 4845 585f 4c41 5420 3d20 2766 726f 6d68  HEX_LAT = 'fromh
-00000110: 6578 5f6c 6174 270a 4652 4f4d 4845 585f  ex_lat'.FROMHEX_
-00000120: 4c4f 4e20 3d20 2766 726f 6d68 6578 5f6c  LON = 'fromhex_l
-00000130: 6f6e 270a 0a54 4f48 4558 5f4c 4154 203d  on'..TOHEX_LAT =
-00000140: 2027 746f 6865 785f 6c61 7427 0a54 4f48   'tohex_lat'.TOH
-00000150: 4558 5f4c 4f4e 203d 2027 746f 6865 785f  EX_LON = 'tohex_
-00000160: 6c6f 6e27 0a0a 4841 5645 5349 4e45 5f44  lon'..HAVESINE_D
-00000170: 4953 5420 3d20 2768 6176 6572 7369 6e65  IST = 'haversine
-00000180: 5f64 6973 7427 0a48 4558 4147 4f4e 203d  _dist'.HEXAGON =
-00000190: 2022 6865 7861 676f 6e22 0a48 4558 4147   "hexagon".HEXAG
-000001a0: 4f4e 5f49 4420 3d20 2268 6578 6167 6f6e  ON_ID = "hexagon
-000001b0: 5f69 6422 0a48 4558 5f49 4420 3d20 2268  _id".HEX_ID = "h
-000001c0: 6578 5f69 6422 0a0a 4845 585f 4c41 5420  ex_id"..HEX_LAT 
-000001d0: 3d20 2268 6578 5f6c 6174 220a 4845 585f  = "hex_lat".HEX_
-000001e0: 4c4f 4e20 3d20 2268 6578 5f6c 6f6e 220a  LON = "hex_lon".
-000001f0: 4845 585f 4c4f 4341 5449 4f4e 203d 2022  HEX_LOCATION = "
-00000200: 6865 785f 6c6f 6361 7469 6f6e 220a 0a49  hex_location"..I
-00000210: 4e44 4558 203d 2022 696e 6465 7822 0a4c  NDEX = "index".L
-00000220: 4154 4954 5544 4520 3d20 226c 6174 6974  ATITUDE = "latit
-00000230: 7564 6522 0a4c 4f4e 4749 5455 4445 203d  ude".LONGITUDE =
-00000240: 2022 6c6f 6e67 6974 7564 6522 0a0a 4f50   "longitude"..OP
-00000250: 5449 4d41 4c5f 4441 5441 5f43 4f4c 554d  TIMAL_DATA_COLUM
-00000260: 4e20 3d20 226f 7074 696d 616c 5f64 6174  N = "optimal_dat
-00000270: 6122 0a53 5550 504c 595f 4441 5441 5f43  a".SUPPLY_DATA_C
-00000280: 4f4c 554d 4e20 3d20 2273 7570 706c 795f  OLUMN = "supply_
-00000290: 6461 7461 220a 5355 5050 4c59 5f48 4558  data".SUPPLY_HEX
-000002a0: 4147 4f4e 5f49 4420 3d20 2273 7570 706c  AGON_ID = "suppl
-000002b0: 795f 6865 7861 676f 6e5f 6964 220a 0a54  y_hexagon_id"..T
-000002c0: 4f54 414c 5f45 5645 4e54 203d 2022 746f  OTAL_EVENT = "to
-000002d0: 7461 6c5f 6576 656e 7422 0a              tal_event".
+00000060: 2027 7069 6e6b 272c 0a20 2020 2027 626c   'pink',.    'bl
+00000070: 6163 6b27 0a5d 0a0a 4449 5354 414e 4345  ack'.]..DISTANCE
+00000080: 203d 2027 6469 7374 616e 6365 270a 4649   = 'distance'.FI
+00000090: 4c45 4e41 4d45 203d 2027 6f70 7469 6d61  LENAME = 'optima
+000000a0: 6c5f 6c6f 6361 7469 6f6e 732e 7069 636b  l_locations.pick
+000000b0: 6c65 270a 4652 4f4d 4845 5820 3d20 2766  le'.FROMHEX = 'f
+000000c0: 726f 6d68 6578 270a 544f 4845 5820 3d20  romhex'.TOHEX = 
+000000d0: 2774 6f68 6578 270a 0a46 524f 4d48 4558  'tohex'..FROMHEX
+000000e0: 5f4c 4154 203d 2027 6672 6f6d 6865 785f  _LAT = 'fromhex_
+000000f0: 6c61 7427 0a46 524f 4d48 4558 5f4c 4f4e  lat'.FROMHEX_LON
+00000100: 203d 2027 6672 6f6d 6865 785f 6c6f 6e27   = 'fromhex_lon'
+00000110: 0a0a 544f 4845 585f 4c41 5420 3d20 2774  ..TOHEX_LAT = 't
+00000120: 6f68 6578 5f6c 6174 270a 544f 4845 585f  ohex_lat'.TOHEX_
+00000130: 4c4f 4e20 3d20 2774 6f68 6578 5f6c 6f6e  LON = 'tohex_lon
+00000140: 270a 0a48 4156 4553 494e 455f 4449 5354  '..HAVESINE_DIST
+00000150: 203d 2027 6861 7665 7273 696e 655f 6469   = 'haversine_di
+00000160: 7374 270a 4845 5841 474f 4e20 3d20 2268  st'.HEXAGON = "h
+00000170: 6578 6167 6f6e 220a 4845 5841 474f 4e5f  exagon".HEXAGON_
+00000180: 4944 203d 2022 6865 7861 676f 6e5f 6964  ID = "hexagon_id
+00000190: 220a 4845 585f 4944 203d 2022 6865 785f  ".HEX_ID = "hex_
+000001a0: 6964 220a 0a48 4558 5f4c 4154 203d 2022  id"..HEX_LAT = "
+000001b0: 6865 785f 6c61 7422 0a48 4558 5f4c 4f4e  hex_lat".HEX_LON
+000001c0: 203d 2022 6865 785f 6c6f 6e22 0a48 4558   = "hex_lon".HEX
+000001d0: 5f4c 4f43 4154 494f 4e20 3d20 2268 6578  _LOCATION = "hex
+000001e0: 5f6c 6f63 6174 696f 6e22 0a0a 494e 4445  _location"..INDE
+000001f0: 5820 3d20 2269 6e64 6578 220a 4c41 5449  X = "index".LATI
+00000200: 5455 4445 203d 2022 6c61 7469 7475 6465  TUDE = "latitude
+00000210: 220a 4c4f 4e47 4954 5544 4520 3d20 226c  ".LONGITUDE = "l
+00000220: 6f6e 6769 7475 6465 220a 0a4f 5054 494d  ongitude"..OPTIM
+00000230: 414c 5f44 4154 415f 434f 4c55 4d4e 203d  AL_DATA_COLUMN =
+00000240: 2022 6f70 7469 6d61 6c5f 6461 7461 220a   "optimal_data".
+00000250: 5355 5050 4c59 5f44 4154 415f 434f 4c55  SUPPLY_DATA_COLU
+00000260: 4d4e 203d 2022 7375 7070 6c79 5f64 6174  MN = "supply_dat
+00000270: 6122 0a53 5550 504c 595f 4845 5841 474f  a".SUPPLY_HEXAGO
+00000280: 4e5f 4944 203d 2022 7375 7070 6c79 5f68  N_ID = "supply_h
+00000290: 6578 6167 6f6e 5f69 6422 0a0a 544f 5441  exagon_id"..TOTA
+000002a0: 4c5f 4556 454e 5420 3d20 2274 6f74 616c  L_EVENT = "total
+000002b0: 5f65 7665 6e74 220a                      _event".
```

### Comparing `optimal_loc-0.1.0/optimal_loc/st_app.py` & `optimal_loc-0.1.1/optimal_loc/st_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import streamlit as st
 from pandas import DataFrame
 from streamlit_folium import folium_static
 from pickle import load as pickle_load
 from folium import plugins, Map, CircleMarker, Marker, Icon
 from PIL import Image
 
-from optimal_loc.constants import COLOURS_LIST, FILENAME, OPTIMAL_DATA_COLUMN, SUPPLY_DATA_COLUMN, HEX_LAT, HEX_LON
-
+from .app_constants import COLOURS_LIST, FILENAME, OPTIMAL_DATA_COLUMN, SUPPLY_DATA_COLUMN, HEX_LAT, HEX_LON
 
 PACKAGE_DIR = os.path.dirname(os.path.abspath(__file__))
 my_algorithm = Image.open(os.path.join(PACKAGE_DIR, 'Modelling Algorithm.png'))
 
 st.set_page_config(layout="wide")
```

### Comparing `optimal_loc-0.1.0/pyproject.toml` & `optimal_loc-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "optimal-loc"
-version = "0.1.0"
+version = "0.1.1"
 description = "A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs."
 
 authors = ["Sinan Demirhan <sdemirhan1320@gmail.com>"]
 readme = "README.md"
 packages = [{include = "optimal_loc"}]
 license = "MIT"
 homepage = "https://github.com/sinan-demirhan/optimal-loc"
```

### Comparing `optimal_loc-0.1.0/PKG-INFO` & `optimal_loc-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optimal-loc
-Version: 0.1.0
+Version: 0.1.1
 Summary: A python project which finds the optimal N locations in a given area according to the given location inputs. This package can be used for business or individual needs.
 Home-page: https://github.com/sinan-demirhan/optimal-loc
 License: MIT
 Keywords: optimalLoc,optimal_loc,optimal-loc,optimal,optimal location,optimal location finder
 Author: Sinan Demirhan
 Author-email: sdemirhan1320@gmail.com
 Requires-Python: >=3.7,<4.0
```


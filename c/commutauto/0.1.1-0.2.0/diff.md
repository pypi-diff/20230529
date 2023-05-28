# Comparing `tmp/commutauto-0.1.1.tar.gz` & `tmp/commutauto-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commutauto-0.1.1.tar", last modified: Sun Mar 19 17:44:52 2023, max compression
+gzip compressed data, was "commutauto-0.2.0.tar", last modified: Sun May 28 23:13:53 2023, max compression
```

## Comparing `commutauto-0.1.1.tar` & `commutauto-0.2.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 17:44:52.598864 commutauto-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-19 17:44:52.598864 commutauto-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-03-19 17:44:44.000000 commutauto-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 17:44:52.590864 commutauto-0.1.1/commutauto/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 17:44:52.594864 commutauto-0.1.1/commutauto/booking_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/booking_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/booking_service/date_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/booking_service/flex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/booking_service/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/booking_service/retriers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13002 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/booking_service/station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 17:44:52.594864 commutauto-0.1.1/commutauto/client/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/client/auth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 17:44:52.594864 commutauto-0.1.1/commutauto/model/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/model/flex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/model/flex_booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/model/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-19 17:44:44.000000 commutauto-0.1.1/commutauto/model/station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-19 17:44:52.590864 commutauto-0.1.1/commutauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-03-19 17:44:52.000000 commutauto-0.1.1/commutauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-19 17:44:52.000000 commutauto-0.1.1/commutauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-19 17:44:52.000000 commutauto-0.1.1/commutauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-19 17:44:52.000000 commutauto-0.1.1/commutauto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-19 17:44:52.000000 commutauto-0.1.1/commutauto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-19 17:44:52.000000 commutauto-0.1.1/commutauto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-19 17:44:52.598864 commutauto-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-03-19 17:44:44.000000 commutauto-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.403109 commutauto-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-28 23:13:53.403109 commutauto-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-28 23:13:41.000000 commutauto-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.399109 commutauto-0.2.0/commutauto/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.403109 commutauto-0.2.0/commutauto/booking_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/date_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/flex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/retriers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.403109 commutauto-0.2.0/commutauto/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/client/auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.403109 commutauto-0.2.0/commutauto/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/model/flex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/model/flex_booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/model/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/model/station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.399109 commutauto-0.2.0/commutauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 23:13:53.403109 commutauto-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-28 23:13:41.000000 commutauto-0.2.0/setup.py
```

### Comparing `commutauto-0.1.1/PKG-INFO` & `commutauto-0.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutauto
-Version: 0.1.1
+Version: 0.2.0
 Summary: CLI to interact with your car sharing service API. Search for available vehicles, manage your bookings and more...
 Home-page: https://github.com/elbuco1/commutauto
 Author: Laurent Boucaud
 Author-email: lrtboucaud@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
```

### Comparing `commutauto-0.1.1/README.md` & `commutauto-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto/__main__.py` & `commutauto-0.2.0/commutauto/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,57 @@
 import argparse
 from datetime import datetime
 import logging
+from typing import Set
 
 import commutauto.booking_service.station as bs_station
 import commutauto.booking_service.flex as bs_flex
 from commutauto.client import CommutautoClient
 from commutauto.constants import (CITIES_MAPPING_STR_ENUM, Cities, 
                                              MAX_STATION_EXPIRATION_TIME_SECOND,
                                              MAX_FLEX_EXPIRATION_TIME_SECOND,
-                                             CitiesToBranchesMapping)
+                                             CitiesToBranchesMapping,
+                                             SIZES_MAPPING_STR_ENUM)
 
 logger = logging.getLogger(__name__)
 
 def parse_date(date: str) -> datetime:
     date = datetime.strptime(date, '%Y-%m-%dT%H:%M:%S')
     return date
 
 def search_station(city: str, latitude: float, longitude: float, radius: float, start_date: datetime, 
-                   end_date: datetime, search_duration: int=None, book: bool=False):
+                   end_date: datetime, search_duration: int=None, book: bool=False, sizes: Set[str]=None):
     city = CITIES_MAPPING_STR_ENUM[city]
+    sizes = {SIZES_MAPPING_STR_ENUM[x] for x in sizes}
 
     client = CommutautoClient(authenticated=False)
     if book:
         client = CommutautoClient(authenticated=True)
 
     available_station = None
     if not search_duration:
         available_station = bs_station.get_available_stations_whithin_radius(client, 
                                 start_date=start_date,
                                 end_date=end_date,
                                 latitude=latitude,
                                 longitude=longitude,
                                 city_id=city,
                                 radius=radius,
+                                allowed_sizes=sizes,
                                 k=1)[0]
     else:
         available_station = bs_station.available_station_search_with_retries(
             client, 
             start_date=start_date, 
             end_date=end_date, 
             latitude=latitude, 
             longitude=longitude, 
             radius=radius,
             city_id=city,
+            allowed_sizes=sizes,
             expiration_time_second=search_duration*24*60*60
         )
     
     if not available_station:
         logger.info(f"No station found stopping search.")
         return
     logger.info(f"Station found: {available_station}. Ending search.")
@@ -215,14 +220,20 @@
                                                 Date format must be 'YYYY-MM-DDTHH:mm:ss'.""")
     
     station_search_parser.add_argument('--search_duration', type=float, required=False,
                                        help=f"""Duration of the search in days. If specified, the search will continue until a car is found or 
                                                 the search duration is greater than the specified value. If not specified, only one search will be conducted. 
                                                 If after this time no car is found, the search will stop. Maximum value is {int(MAX_STATION_EXPIRATION_TIME_SECOND/(24*60*60))} days.""")
 
+    station_search_parser.add_argument('--sizes',
+                                       choices=SIZES_MAPPING_STR_ENUM.keys(),
+                                       default=None,
+                                       nargs='+',
+                                       help='What car sizes to allow. Possible values are: compact, midsize and family. If not specified, all sizes are allowed.')
+    
     station_search_parser.add_argument('--book', action='store_true', 
                                        help='If the flag is set then if a station is found during the search it will be booked automatically.')
     
     ### BOOK ###
     station_book_parser = station_parsers.add_parser('book', help="Book a station.")
     station_book_parser.set_defaults(func=book_station)
     station_book_parser.add_argument('--city',
```

### Comparing `commutauto-0.1.1/commutauto/booking_service/date_manager.py` & `commutauto-0.2.0/commutauto/booking_service/date_manager.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto/booking_service/flex.py` & `commutauto-0.2.0/commutauto/booking_service/flex.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto/booking_service/payload.py` & `commutauto-0.2.0/commutauto/booking_service/payload.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         return True
     
 class GetFlexDisponibilityUrlParameter(Payload):
     def __init__(
             self, 
             BranchID: int,
             CityID: int,
-            LanguageID: int = 1 
+            LanguageID: int = 2
         ):
         self.BranchID = BranchID
         self.CityID = CityID
         self.LanguageID = LanguageID
     def to_dict(self):
         return self.__dict__
```

### Comparing `commutauto-0.1.1/commutauto/booking_service/retriers.py` & `commutauto-0.2.0/commutauto/booking_service/retriers.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto/booking_service/station.py` & `commutauto-0.2.0/commutauto/booking_service/station.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import datetime as dt
-from typing import List, Dict, Union
+from typing import List, Dict, Union, Set
 import heapq
 import logging
-import traceback
 from tenacity import RetryError
 import logging
 
 from commutauto.client import CommutautoClient
 from commutauto.model import Station, Reservation, ReservationShort, Flex
 from commutauto.booking_service.payload import get_payload
 from commutauto.constants import (AspScript, 
                                              MAP_ROUTE_ENDPOINT, 
                                              Cities, 
                                              MINIMUM_SEARCH_RADIUS_KM,
                                              STATION_BASE_WAIT_TIME_SECOND,
                                              STATION_WAIT_TIME_JITTER_SECOND,
                                              STATION_EXPIRATION_TIME_SECOND,
-                                             MAX_STATION_EXPIRATION_TIME_SECOND
+                                             MAX_STATION_EXPIRATION_TIME_SECOND,
+                                             CarSizes,
+                                             CAR_MODELS_MAPPING_STR_ENUM,
+                                             CAR_MODELS_TO_SIZE_MAPPING
                                             )
 from commutauto.booking_service.retriers import get_available_station_search_retryer
 import commutauto.booking_service.date_manager as dm
 from commutauto.exceptions import AuthenticatedClientRequiredException, NoStationsWhithinRadiusException
 
 logger = logging.getLogger(__name__)
 
@@ -34,21 +36,31 @@
     available_stations = []
     for station in stations:
         if station.NbrRes == 0 or station.NbrRes == "0":
             available_stations.append(station)
     return available_stations
 
 def filter_closest_station(stations: List[Station]) -> Station:
-        min_distance = float("inf")
-        closest_station = None
-        for s in stations:
-            if s.Distance < min_distance:
-                min_distance = s.Distance
-                closest_station = s
-        return closest_station     
+    min_distance = float("inf")
+    closest_station = None
+    for s in stations:
+        if s.Distance < min_distance:
+            min_distance = s.Distance
+            closest_station = s
+    return closest_station
+
+def filter_car_size_station(stations: List[Station], allowed_sizes: Set[CarSizes]) -> Station:
+    logger.info(f"Filter vehicles based on vehice size. Allowed sizes are: {allowed_sizes}.")
+    allowed_stations = []
+    for station in stations:
+        model = CAR_MODELS_MAPPING_STR_ENUM[(station.Brand, station.Model)]
+        car_size = CAR_MODELS_TO_SIZE_MAPPING[model]
+        if car_size in allowed_sizes:
+            allowed_stations.append(station)
+    return allowed_stations
 
 def check_stations_whithin_radius(stations: List[Station], radius: float):
     closest_station = filter_closest_station(stations)
     if closest_station and closest_station.Distance > radius:
         err_msg = f"Closest station is located at {closest_station.Distance} kilometers from the provided "
         err_msg += f"GPS coordinates. The specified search radius '{radius} kilometers' is lower than this distance."
         raise NoStationsWhithinRadiusException(err_msg)
@@ -120,27 +132,31 @@
     
     stations = parse_stations(response["Stations"])
     logger.debug(f"Stations found: {stations}.")
     return stations
 
 def get_available_stations_whithin_radius(client: CommutautoClient, start_date: dt.datetime, 
                                 end_date: dt.datetime, latitude: float, longitude: float, city_id: Cities,
-                                radius: float, k: int = -1)-> List[Station]:
+                                radius: float, k: int = -1, allowed_sizes: Set[CarSizes] = None)-> List[Station]:
     """
     Args:
         start_date (dt.datetime): UTC time
         end_date (dt.datetime): UTC time
         radius (float): kilometers
     """
     logger.info(f"Get available stations whithin radius {radius}.")
 
     stations = get_stations(client, start_date, end_date, latitude, longitude, city_id=city_id)
     check_stations_whithin_radius(stations, radius)
     available_stations = filter_available_stations(stations)
     stations_whithin_radius = filter_vehicles_whithin_radius(available_stations, radius, k)
+
+    if allowed_sizes:
+        stations_whithin_radius = filter_car_size_station(stations_whithin_radius, allowed_sizes)
+
     if stations_whithin_radius:
         logger.info("Found stations:")
         for station in stations_whithin_radius:
             logger.info(station)
     return stations_whithin_radius
 
 def book_car_from_id(client: CommutautoClient, start_date: dt.datetime, 
@@ -266,15 +282,15 @@
         logger.info("Found station bookings:")
         for res in reservations:
             logger.info(res)
     return reservations
 
 def available_station_search_with_retries(client: CommutautoClient, start_date: dt.datetime, 
                                 end_date: dt.datetime, latitude: float, longitude: float, city_id: Cities, 
-                                radius: float, base_wait_time_second: int=STATION_BASE_WAIT_TIME_SECOND, 
+                                radius: float, allowed_sizes: Set[CarSizes] = None, base_wait_time_second: int=STATION_BASE_WAIT_TIME_SECOND, 
                                 wait_time_jitter_second: int=STATION_WAIT_TIME_JITTER_SECOND, 
                                 expiration_time_second: int=STATION_EXPIRATION_TIME_SECOND, 
                                 longer_pause_after_second: int=None, 
                                 longer_pause_max_duration_second: int=None):
     logger.info(f"Search stations with retries. Wait time: {base_wait_time_second}s, Jitter: {wait_time_jitter_second}s, Expiration time: {expiration_time_second}.")
     
     if expiration_time_second > MAX_STATION_EXPIRATION_TIME_SECOND:
@@ -285,13 +301,13 @@
                                                    expiration_time_second,
                                                    longer_pause_after_second,
                                                    longer_pause_max_duration_second)
         
     station = None
     try:
         stations = retryer(get_available_stations_whithin_radius, client, start_date=start_date, 
-                           end_date=end_date, latitude=latitude, longitude=longitude, radius=radius, city_id=city_id)
+                           end_date=end_date, latitude=latitude, longitude=longitude, radius=radius, city_id=city_id, allowed_sizes=allowed_sizes)
         if stations:
             station = stations[0]
     except RetryError:
         logging.exception("Ending retry loop.")
     return station
```

### Comparing `commutauto-0.1.1/commutauto/client/auth_token.py` & `commutauto-0.2.0/commutauto/client/auth_token.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto/client/client.py` & `commutauto-0.2.0/commutauto/client/client.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto/exceptions.py` & `commutauto-0.2.0/commutauto/exceptions.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto/model/flex.py` & `commutauto-0.2.0/commutauto/model/flex.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto/model/flex_booking.py` & `commutauto-0.2.0/commutauto/model/flex_booking.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto/model/reservation.py` & `commutauto-0.2.0/commutauto/model/reservation.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto/model/station.py` & `commutauto-0.2.0/commutauto/model/station.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/commutauto.egg-info/PKG-INFO` & `commutauto-0.2.0/commutauto.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutauto
-Version: 0.1.1
+Version: 0.2.0
 Summary: CLI to interact with your car sharing service API. Search for available vehicles, manage your bookings and more...
 Home-page: https://github.com/elbuco1/commutauto
 Author: Laurent Boucaud
 Author-email: lrtboucaud@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
```

### Comparing `commutauto-0.1.1/commutauto.egg-info/SOURCES.txt` & `commutauto-0.2.0/commutauto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commutauto-0.1.1/setup.py` & `commutauto-0.2.0/setup.py`

 * *Files identical despite different names*


# Comparing `tmp/commutauto-0.2.0.tar.gz` & `tmp/commutauto-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commutauto-0.2.0.tar", last modified: Sun May 28 23:13:53 2023, max compression
+gzip compressed data, was "commutauto-0.3.0.tar", last modified: Mon May 29 00:54:23 2023, max compression
```

## Comparing `commutauto-0.2.0.tar` & `commutauto-0.3.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.403109 commutauto-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-28 23:13:53.403109 commutauto-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-28 23:13:41.000000 commutauto-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.399109 commutauto-0.2.0/commutauto/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16412 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.403109 commutauto-0.2.0/commutauto/booking_service/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/date_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/flex.py
--rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/retriers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13869 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/booking_service/station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.403109 commutauto-0.2.0/commutauto/client/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/client/auth_token.py
--rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.403109 commutauto-0.2.0/commutauto/model/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/model/flex.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/model/flex_booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/model/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-28 23:13:41.000000 commutauto-0.2.0/commutauto/model/station.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 23:13:53.399109 commutauto-0.2.0/commutauto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-28 23:13:53.000000 commutauto-0.2.0/commutauto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 23:13:53.403109 commutauto-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-28 23:13:41.000000 commutauto-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 00:54:23.971437 commutauto-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8765 2023-05-29 00:54:07.000000 commutauto-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/commutauto/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/commutauto/booking_service/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/date_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8388 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/flex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7803 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/retriers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15016 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/booking_service/station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/commutauto/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/client/auth_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12738 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/commutauto/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/model/flex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/model/flex_booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/model/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-29 00:54:07.000000 commutauto-0.3.0/commutauto/model/station.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 00:54:23.971437 commutauto-0.3.0/commutauto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 00:54:23.000000 commutauto-0.3.0/commutauto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 00:54:23.971437 commutauto-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-05-29 00:54:07.000000 commutauto-0.3.0/setup.py
```

### Comparing `commutauto-0.2.0/PKG-INFO` & `commutauto-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutauto
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI to interact with your car sharing service API. Search for available vehicles, manage your bookings and more...
 Home-page: https://github.com/elbuco1/commutauto
 Author: Laurent Boucaud
 Author-email: lrtboucaud@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
```

### Comparing `commutauto-0.2.0/README.md` & `commutauto-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/__main__.py` & `commutauto-0.3.0/commutauto/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 logger = logging.getLogger(__name__)
 
 def parse_date(date: str) -> datetime:
     date = datetime.strptime(date, '%Y-%m-%dT%H:%M:%S')
     return date
 
 def search_station(city: str, latitude: float, longitude: float, radius: float, start_date: datetime, 
-                   end_date: datetime, search_duration: int=None, book: bool=False, sizes: Set[str]=None):
+                   end_date: datetime, search_duration: int=None, book: bool=False, sizes: Set[str]=None, swap: bool = False):
     city = CITIES_MAPPING_STR_ENUM[city]
-    sizes = {SIZES_MAPPING_STR_ENUM[x] for x in sizes}
+
+    if sizes:
+        sizes = {SIZES_MAPPING_STR_ENUM[x] for x in sizes}
 
     client = CommutautoClient(authenticated=False)
     if book:
         client = CommutautoClient(authenticated=True)
 
     available_station = None
     if not search_duration:
@@ -33,25 +35,27 @@
                                 start_date=start_date,
                                 end_date=end_date,
                                 latitude=latitude,
                                 longitude=longitude,
                                 city_id=city,
                                 radius=radius,
                                 allowed_sizes=sizes,
+                                swap_bookings=swap,
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
             allowed_sizes=sizes,
+            swap_bookings=swap,
             expiration_time_second=search_duration*24*60*60
         )
     
     if not available_station:
         logger.info(f"No station found stopping search.")
         return
     logger.info(f"Station found: {available_station}. Ending search.")
@@ -61,30 +65,32 @@
     
     reservation_id = bs_station.book_car_from_id(client, 
                                     start_date=start_date, 
                                     end_date=end_date, 
                                     car_id=available_station.CarID, 
                                     latitude=latitude, 
                                     longitude=longitude,
-                                    city_id=city)
+                                    city_id=city,
+                                    swap_bookings=swap)
     if reservation_id:
         logger.info(f"Successfull station booking. Reservation id: {reservation_id}.")
             
 def book_station(city: str, latitude: float, longitude: float, start_date: datetime, 
-                   end_date: datetime, car_id: str):
+                   end_date: datetime, car_id: str, swap: bool = False):
     city = CITIES_MAPPING_STR_ENUM[city]
     client = CommutautoClient(authenticated=True)
 
     reservation_id = bs_station.book_car_from_id(client, 
                                     start_date=start_date, 
                                     end_date=end_date, 
                                     car_id=car_id, 
                                     latitude=latitude, 
                                     longitude=longitude,
-                                    city_id=city)
+                                    city_id=city,
+                                    swap_bookings=swap)
     if reservation_id:
         logger.info(f"Successfull station booking. Reservation id: {reservation_id}.")
 
 def list_station_bookings():
     client = CommutautoClient(authenticated=True)
     reservations = bs_station.get_car_booking_list(client)
 
@@ -229,14 +235,17 @@
                                        default=None,
                                        nargs='+',
                                        help='What car sizes to allow. Possible values are: compact, midsize and family. If not specified, all sizes are allowed.')
     
     station_search_parser.add_argument('--book', action='store_true', 
                                        help='If the flag is set then if a station is found during the search it will be booked automatically.')
     
+    station_search_parser.add_argument('--swap', action='store_true', 
+                                       help='If the flag is set and an overlapping booking already exists the search will be enabled. And in the event where a new booking is found, the old one will be deleted.')
+    
     ### BOOK ###
     station_book_parser = station_parsers.add_parser('book', help="Book a station.")
     station_book_parser.set_defaults(func=book_station)
     station_book_parser.add_argument('--city',
                                        choices=CITIES_MAPPING_STR_ENUM.keys(), 
                                        help='In which city to search for a station car.')
     
@@ -256,14 +265,18 @@
     station_book_parser.add_argument('--end_date',
                                        type=parse_date, 
                                        help="""Date at which the car booking will end. Time must be expressed in the timezone of the specified city.
                                                Time will be rounded to closest 15 minutes. end_date must be at least 30 minutes more than start_date.
                                                 Date format must be 'YYYY-MM-DDTHH:mm:ss'.""")
     station_book_parser.add_argument('--car_id',
                                        help='Station car id (like 1234).')
+
+    station_book_parser.add_argument('--swap', action='store_true', 
+                                       help='If the flag is set and an overlapping booking already exists it will be canceled before creating the new one.')
+    
     
     ### CANCEL BOOKING ###
     station_cancel_parser = station_parsers.add_parser('cancel_booking', help="Cancel a station booking.")
     station_cancel_parser.set_defaults(func=cancel_station_booking)
     station_cancel_parser.add_argument('--reservation_id',
                                        help='Station reservation id (like 39762132).')
```

### Comparing `commutauto-0.2.0/commutauto/booking_service/date_manager.py` & `commutauto-0.3.0/commutauto/booking_service/date_manager.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/booking_service/flex.py` & `commutauto-0.3.0/commutauto/booking_service/flex.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/booking_service/payload.py` & `commutauto-0.3.0/commutauto/booking_service/payload.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/booking_service/retriers.py` & `commutauto-0.3.0/commutauto/booking_service/retriers.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/booking_service/station.py` & `commutauto-0.3.0/commutauto/booking_service/station.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,15 @@
                                              MAX_STATION_EXPIRATION_TIME_SECOND,
                                              CarSizes,
                                              CAR_MODELS_MAPPING_STR_ENUM,
                                              CAR_MODELS_TO_SIZE_MAPPING
                                             )
 from commutauto.booking_service.retriers import get_available_station_search_retryer
 import commutauto.booking_service.date_manager as dm
-from commutauto.exceptions import AuthenticatedClientRequiredException, NoStationsWhithinRadiusException
+from commutauto.exceptions import AuthenticatedClientRequiredException, NoStationsWhithinRadiusException, OverlappingWithBookingsWindow
 
 logger = logging.getLogger(__name__)
 
 def parse_stations(station_dicts: List[Dict])-> List[Station]:
     stations = []
     for station_dict in station_dicts:
         stations.append(Station(**station_dict))
@@ -81,39 +81,44 @@
             break
         vehicle = heapq.heappop(minheap)
         if vehicle.Distance > radius:
             break
         vehicles_whithin_radius.append(vehicle)
     return vehicles_whithin_radius
 
-def prepare_and_validate_time_window(client: CommutautoClient, start_date: dt.datetime, 
+def prepare_and_validate_time_window(start_date: dt.datetime, 
                                 end_date: dt.datetime, latitude: float, longitude: float):
     start_date = dm.convert_datetime_to_utc(start_date, latitude, longitude)
     end_date = dm.convert_datetime_to_utc(end_date, latitude, longitude)
     start_date, end_date = dm.round_booking_time_window(start_date, end_date)
     dm.validate_booking_request_time_window(start_date, end_date)
     dm.check_start_date_greater_than_quarter_hour_from_now(start_date)
     dm.check_start_date_sooner_than_one_month(start_date)
-
-    if client.authenticated:
-        reservations = get_car_booking_list(client)
-        overlapping_reservations = dm.check_no_booking_intersection_with_search_window(start_date, end_date, reservations)
-
-        if overlapping_reservations:
-            err_msg = f"Provided search time window '[{start_date};{end_date}]' overlaps with the following reservations: \n"
-            for res in overlapping_reservations:
-                err_msg += f"{res} \n"
-            raise dm.OverlappingWithBookingsWindow(err_msg)
     return start_date, end_date
 
+def check_existing_booking_overlap(client: CommutautoClient, start_date: dt.datetime, end_date: dt.datetime) -> List[ReservationShort]:
+    reservations = get_car_booking_list(client)
+    overlapping_reservations = dm.check_no_booking_intersection_with_search_window(start_date, end_date, reservations)
+    return overlapping_reservations
+
+def raise_reservation_overlap_error(overlapping_reservations: List[ReservationShort], start_date: dt.datetime, end_date: dt.datetime):
+    err_msg = f"Provided search time window '[{start_date};{end_date}]' overlaps with the following reservations: \n"
+    for res in overlapping_reservations:
+        err_msg += f"{res} \n"
+    raise OverlappingWithBookingsWindow(err_msg)
+
 def get_stations(client: CommutautoClient, start_date: dt.datetime, 
-                                end_date: dt.datetime, latitude: float, longitude: float, city_id: Cities):
+                                end_date: dt.datetime, latitude: float, longitude: float, city_id: Cities, swap_bookings: bool = False):
     logger.info(f"Get available stations. City id: {city_id}, Latitude: {latitude}, Longitude: {longitude}, Start: {start_date}, End: {end_date}.")
-    
-    start_date, end_date = prepare_and_validate_time_window(client, start_date, end_date, latitude, longitude)
+    start_date, end_date = prepare_and_validate_time_window(start_date, end_date, latitude, longitude)
+
+    if client.authenticated:
+        overlaping_res = check_existing_booking_overlap(client, start_date, end_date)
+        if overlaping_res and not swap_bookings:
+            raise_reservation_overlap_error(overlaping_res, start_date, end_date)
 
     payload = get_payload(
         script_name=AspScript.GET_CAR_DISPONIBILITY,
         payload_args={
             "StartDateUTC": start_date, 
             "EndDateUTC": end_date, 
             "Latitude": latitude,
@@ -132,45 +137,55 @@
     
     stations = parse_stations(response["Stations"])
     logger.debug(f"Stations found: {stations}.")
     return stations
 
 def get_available_stations_whithin_radius(client: CommutautoClient, start_date: dt.datetime, 
                                 end_date: dt.datetime, latitude: float, longitude: float, city_id: Cities,
-                                radius: float, k: int = -1, allowed_sizes: Set[CarSizes] = None)-> List[Station]:
+                                radius: float, k: int = -1, allowed_sizes: Set[CarSizes] = None, swap_bookings: bool = False)-> List[Station]:
     """
     Args:
         start_date (dt.datetime): UTC time
         end_date (dt.datetime): UTC time
         radius (float): kilometers
     """
     logger.info(f"Get available stations whithin radius {radius}.")
 
-    stations = get_stations(client, start_date, end_date, latitude, longitude, city_id=city_id)
+    stations = get_stations(client, start_date, end_date, latitude, longitude, city_id=city_id, swap_bookings=swap_bookings)
     check_stations_whithin_radius(stations, radius)
     available_stations = filter_available_stations(stations)
     stations_whithin_radius = filter_vehicles_whithin_radius(available_stations, radius, k)
 
     if allowed_sizes:
         stations_whithin_radius = filter_car_size_station(stations_whithin_radius, allowed_sizes)
 
     if stations_whithin_radius:
         logger.info("Found stations:")
         for station in stations_whithin_radius:
             logger.info(station)
     return stations_whithin_radius
 
 def book_car_from_id(client: CommutautoClient, start_date: dt.datetime, 
-                                end_date: dt.datetime, car_id: int, latitude: float, longitude: float, city_id: Cities) -> int:
+                                end_date: dt.datetime, car_id: int, latitude: float, longitude: float, city_id: Cities, swap_bookings: bool = False) -> int:
     logger.info(f"Book station from id. Car id: {car_id}, City id: {city_id}, Latitude: {latitude}, Longitude: {longitude}, Start: {start_date}, End: {end_date}.")
     
     if not client.authenticated:
         raise AuthenticatedClientRequiredException()
     
-    start_date, end_date = prepare_and_validate_time_window(client, start_date, end_date, latitude, longitude)
+    start_date, end_date = prepare_and_validate_time_window(start_date, end_date, latitude, longitude)
+
+    if client.authenticated:
+        overlaping_res = check_existing_booking_overlap(client, start_date, end_date)
+        if overlaping_res:
+            if not swap_bookings:
+                raise_reservation_overlap_error(overlaping_res, start_date, end_date)
+            else:
+                for res in overlaping_res:
+                    complete_res = get_car_booking(client, res.ReservationID)
+                    cancel_car_booking(client, complete_res, latitude, longitude)
         
     payload = get_payload(
         script_name=AspScript.BOOK_CAR,
         payload_args={
             "StartDateUTC": start_date, 
             "EndDateUTC": end_date, 
             "CarId": car_id,
@@ -282,15 +297,16 @@
         logger.info("Found station bookings:")
         for res in reservations:
             logger.info(res)
     return reservations
 
 def available_station_search_with_retries(client: CommutautoClient, start_date: dt.datetime, 
                                 end_date: dt.datetime, latitude: float, longitude: float, city_id: Cities, 
-                                radius: float, allowed_sizes: Set[CarSizes] = None, base_wait_time_second: int=STATION_BASE_WAIT_TIME_SECOND, 
+                                radius: float, allowed_sizes: Set[CarSizes] = None, swap_bookings: bool = False,
+                                base_wait_time_second: int=STATION_BASE_WAIT_TIME_SECOND, 
                                 wait_time_jitter_second: int=STATION_WAIT_TIME_JITTER_SECOND, 
                                 expiration_time_second: int=STATION_EXPIRATION_TIME_SECOND, 
                                 longer_pause_after_second: int=None, 
                                 longer_pause_max_duration_second: int=None):
     logger.info(f"Search stations with retries. Wait time: {base_wait_time_second}s, Jitter: {wait_time_jitter_second}s, Expiration time: {expiration_time_second}.")
     
     if expiration_time_second > MAX_STATION_EXPIRATION_TIME_SECOND:
@@ -301,13 +317,14 @@
                                                    expiration_time_second,
                                                    longer_pause_after_second,
                                                    longer_pause_max_duration_second)
         
     station = None
     try:
         stations = retryer(get_available_stations_whithin_radius, client, start_date=start_date, 
-                           end_date=end_date, latitude=latitude, longitude=longitude, radius=radius, city_id=city_id, allowed_sizes=allowed_sizes)
+                           end_date=end_date, latitude=latitude, longitude=longitude, radius=radius, city_id=city_id, 
+                           allowed_sizes=allowed_sizes, swap_bookings=swap_bookings)
         if stations:
             station = stations[0]
     except RetryError:
         logging.exception("Ending retry loop.")
     return station
```

### Comparing `commutauto-0.2.0/commutauto/client/auth_token.py` & `commutauto-0.3.0/commutauto/client/auth_token.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/client/client.py` & `commutauto-0.3.0/commutauto/client/client.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/constants.py` & `commutauto-0.3.0/commutauto/constants.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/exceptions.py` & `commutauto-0.3.0/commutauto/exceptions.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/model/flex.py` & `commutauto-0.3.0/commutauto/model/flex.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/model/flex_booking.py` & `commutauto-0.3.0/commutauto/model/flex_booking.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/model/reservation.py` & `commutauto-0.3.0/commutauto/model/reservation.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto/model/station.py` & `commutauto-0.3.0/commutauto/model/station.py`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/commutauto.egg-info/PKG-INFO` & `commutauto-0.3.0/commutauto.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commutauto
-Version: 0.2.0
+Version: 0.3.0
 Summary: CLI to interact with your car sharing service API. Search for available vehicles, manage your bookings and more...
 Home-page: https://github.com/elbuco1/commutauto
 Author: Laurent Boucaud
 Author-email: lrtboucaud@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
```

### Comparing `commutauto-0.2.0/commutauto.egg-info/SOURCES.txt` & `commutauto-0.3.0/commutauto.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commutauto-0.2.0/setup.py` & `commutauto-0.3.0/setup.py`

 * *Files identical despite different names*


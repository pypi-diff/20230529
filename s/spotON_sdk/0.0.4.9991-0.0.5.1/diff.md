# Comparing `tmp/spotON_sdk-0.0.4.9991.tar.gz` & `tmp/spotON_sdk-0.0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.4.9991.tar", last modified: Tue May 23 19:10:49 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.5.1.tar", last modified: Mon May 29 06:08:03 2023, max compression
```

## Comparing `spotON_sdk-0.0.4.9991.tar` & `spotON_sdk-0.0.5.1.tar`

### file list

```diff
@@ -1,23 +1,34 @@
--rw-r--r--   0        0        0     6184 2023-05-21 14:30:18.248848 spotON_sdk-0.0.4.9991/.gitignore
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.4.9991/LICENSE
--rw-r--r--   0        0        0      355 2023-05-21 15:19:16.024161 spotON_sdk-0.0.4.9991/pyproject.toml
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0     2095 2023-05-23 19:10:38.297633 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      208 2023-05-23 09:21:46.713502 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4709 2023-05-22 09:10:42.883983 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0     2248 2023-05-23 14:09:38.854446 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     6957 2023-05-17 21:52:50.903007 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0     1728 2023-05-23 19:09:26.840241 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/timeframes.py
--rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.4.9991/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      462 2023-05-23 19:10:44.497974 spotON_sdk-0.0.4.9991/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.4.9991/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.4.9991/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.4.9991/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.4.9991/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      253 1970-01-01 00:00:00.000000 spotON_sdk-0.0.4.9991/PKG-INFO
+-rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.1/.gitignore
+-rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.1/.gitmodules
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.1/LICENSE
+-rw-r--r--   0        0        0      405 2023-05-29 06:03:48.378147 spotON_sdk-0.0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0      165 2023-05-28 20:03:24.891372 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/API_Call.py
+-rw-r--r--   0        0        0     2303 2023-05-28 16:41:31.459722 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      263 2023-05-28 19:44:31.805887 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/customBaseModel.py
+-rw-r--r--   0        0        0     2806 2023-05-28 17:11:51.233618 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     8210 2023-05-28 16:32:06.404713 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/timeframes.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.5.1/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      459 2023-05-29 06:05:35.172801 spotON_sdk-0.0.5.1/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.1/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.5.1/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.1/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0     1753 2023-05-23 14:27:13.601664 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/Sensor_Device_test.py
+-rw-r--r--   0        0        0     8258 2023-05-28 15:42:11.428221 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/_test.py
+-rw-r--r--   0        0        0      452 2023-05-28 20:00:58.125992 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/api_call.py
+-rw-r--r--   0        0        0     7199 2023-05-28 15:39:01.607110 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/create_spotON_Areas.py
+-rw-r--r--   0        0        0     2051 2023-05-28 09:52:03.472090 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/create_token.py
+-rw-r--r--   0        0        0     1964 2023-05-28 14:25:22.033622 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/make_json.py
+-rw-r--r--   0        0        0      798 2023-05-28 18:21:21.497039 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/pricelogic_Test.py
+-rw-r--r--   0        0        0     2930 2023-05-23 16:32:56.748640 spotON_sdk-0.0.5.1/spotON_sdk/private_tests/userstate_test.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.1/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      250 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.1/PKG-INFO
```

### Comparing `spotON_sdk-0.0.4.9991/.gitignore` & `spotON_sdk-0.0.5.1/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 spotOn-venv/
+private_tests/
 tests/
 .venv
 
 # Byte-compiled / optimized / DLL files
 __pycache__/
 *.py[cod]
 *$py.class
```

### Comparing `spotON_sdk-0.0.4.9991/LICENSE` & `spotON_sdk-0.0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,45 @@
 from math import e
 from mimetypes import init
 from os import name
 from typing import List, Union
-from pydantic import BaseModel, Field, validator, root_validator
+from pydantic import  Field, validator, root_validator
 from .timeframes import Timeframes,Timeframe
 from .markets import Market, Markets
+from .customBaseModel import CustomBaseModel
 
+import json
 
-
-class Interrupted_On_Time(BaseModel):
+class Interrupted_On_Time(CustomBaseModel):
     name: str = Field(default="Interrupted_On_Time",init = False)
     pass
 
 
-class Continuous_On_Time(BaseModel):
+class Continuous_On_Time(CustomBaseModel):
     name: str = Field(default="Continuous_On_Time",init = False)
     week: int = Field(default=None)
     best_hour: int = Field(default=None)
 
-
-class Price_Logic(BaseModel):
+class Price_Logic(CustomBaseModel):
     nr_of_hours_on: int
-    market: Union[str, Market]
+    market: Market | str
     timeframes: Timeframes = Timeframes()
     pricefinding: Continuous_On_Time | Interrupted_On_Time = Interrupted_On_Time()
     resolution: float = Field(default=1)
     timeframe_shorter_than_nr_of_hours_on: bool = Field(default=False)
     
     def update_pricefinding(self, pricefinding: Union[Continuous_On_Time, Interrupted_On_Time]):
             self.pricefinding = pricefinding
 
+    def to_json(self) -> str:
+        switch_pattern_dict = self.to_dict()
+        json_str = json.dumps(switch_pattern_dict)
+
+        return json_str
+
     @root_validator(pre=True)
     def set_market_to_market_object(cls, values):
         if isinstance(values["market"], str):
             result = Markets.get_market_by_name(values["market"])
             result = Markets.get_market_by_code(values["market"])
             if result is None:
                 raise ValueError("Market is not valid")
@@ -52,8 +58,8 @@
         nr_of_hours_on = values.get('nr_of_hours_on')
         if timeframes and nr_of_hours_on:
             possible_hours = timeframes.possible_hours
             if nr_of_hours_on > len(possible_hours):
                 values['timeframe_shorter_than_nr_of_hours_on'] = True
             else:
                 values['timeframe_shorter_than_nr_of_hours_on'] = False
-        return values
+        return values
```

### Comparing `spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/countries.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from dataclasses import dataclass, field
 
 from typing import Any,Optional,List
 from .spotON_Areas import spotON_Area
+from .customBaseModel import CustomBaseModel
 from typing import Tuple
 
 import pandas as pd
 import pytz
 
 def _country_code_to_emoji(country_code):
     OFFSET = 127397
     return ''.join(chr(ord(c) + OFFSET) for c in country_code.upper())
 
-@dataclass
-class Country:
+class Country(CustomBaseModel):
     capital: str
     country_code: str
     country_name: str
-    UTC_time_difference: float = field(init=False)
-    
+    UTC_time_difference: float = 0
+
+    @property
     def calculate_utc_time_difference(self) -> Tuple[pd.Timedelta,float]:
         try:
             timezone = f"Europe/{self.capital}"
             local_tz = pytz.timezone(timezone)
             utc_dt = pd.Timestamp.utcnow().to_pydatetime()
             local_dt = utc_dt.astimezone(local_tz)
             local_dt_Offset = local_dt.utcoffset()
@@ -33,19 +34,18 @@
                 raise Exception
 
         except:
             print(f"{self.capital} not found in European capitals.")
             default_delta = pd.Timedelta(hours=0)
             default_UTC_time_difference = 0
             return default_delta, default_UTC_time_difference
-
-    def __post_init__(self) -> None:
-        self.delta,self.UTC_time_difference = self.calculate_utc_time_difference()
-        self.emoji = _country_code_to_emoji(self.country_code)
         
+
+
+
 def get_country_by_code(countries: List[Country], country_code: str) -> Optional[Country]:
     """
     Returns the country object that matches the given country code.
     If no such object is found, returns None.
     """
     for country in countries:
         if country.country_code == country_code:
```

### Comparing `spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/markets.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,60 +3,80 @@
 from dataclasses import dataclass, field
 from typing import Optional, Dict,Any
 
 from typing import List
 from .countries import *
 from .bidding_zones import bidding_zones
 
-@dataclass
-class Market():
-    area:Area_details
-    country :Country
-    alias : str | None = None
-    area_code :str = field(init=False)
-    country_code : str = field(init=False)
-    region_code : str | None = field(init=False,default=None)
-    cities : str = field(init=False)
-
-    def __post_init__(self):
-        self.area_code = self.area.name
-        country_region = self.area_code.split("_")
-        self.country_code = country_region[0]
+from .customBaseModel import CustomBaseModel
+
+from pydantic import Field, root_validator
+
+class Market(CustomBaseModel):
+    area: Area_details
+    country: Country
+    alias: Optional[str] = None
+    area_code: str = Field(default="")
+    country_code: str = Field(default="")
+    region_code: Optional[str] = None
+    cities: str = Field(default="")
+    name: str = Field(default="")
+    @root_validator(pre=True)
+    def set_codes(cls, values):
+        area = values.get('area')
+        area_code = area.name
+        values['area_code'] = area_code
+
+        country_region = area_code.split("_")
+        values['country_code'] = country_region[0]
         if len(country_region) >=2:
-            self.region_code = country_region[1]
+            values['region_code'] = country_region[1]
 
         try:
-            city_List = bidding_zones[self.area_code]["cities"]
+            city_List = bidding_zones[area_code]["cities"]
             my_string = ', '.join(city_List)
-            self.cities = my_string
+            values['cities'] = my_string
         except:
-            self.cities = ""
+            values['cities'] = ""
+
+        values["name"] = f"{values['country'].country_name} {values['area_code']} {values['cities']}"
+        return values
+
 
+        #TODO: Add emoji to name
+        self.name = f"{self.country.country_name} {self.area_code} {self.cities}"
+        self.name = f" {self.country.country_name}"
 
-        self.name = f"{self.country.emoji} {self.country.country_name} {self.area_code} {self.cities}"
-        self.name = f"{self.country.emoji} {self.country.country_name}"
+        '''self.name = f"{self.country.emoji} {self.country.country_name} {self.area_code} {self.cities}"
+        self.name = f"{self.country.emoji} {self.country.country_name}"'''
 
         #self.get_Market_by_area_code(self.area.name)
 
+
+
+
+
+
 @dataclass
 class Markets():
-    austria = Market(spotON_Area.AT,all_Countries.Austria)
-    germany = Market(spotON_Area.DE_LU,all_Countries.Germany,alias="DE_LU")
+    austria = Market(area=spotON_Area.AT,country=all_Countries.Austria)
+    germany = Market(area=spotON_Area.DE,country=all_Countries.Germany)
+    sweden1 = Market(area=spotON_Area.SE_1,country=all_Countries.Sweden)    
     #luxembourg = Market(Area.DE_LU,Luxembourg)
-    sweden1 = Market(spotON_Area.SE_1,all_Countries.Sweden)
+
     #sweden2 = Market(Area.SE_2,Sweden)
     #sweden3 = Market(Area.SE_3,Sweden)
     #sweden4 = Market(Area.SE_4,Sweden)
     markets_List = [value for key, value in vars().items() if isinstance(value, Market)]
     merged_Markets = []
 
     @staticmethod
     def get_market_by_name(name: str) -> Optional[Market]:
         for market in Markets.markets_List:
-            if market.name == name:
+            if market.name == name: # type: ignore
                 return market
 
         return None
 
     @staticmethod
     def get_market_by_code(area_code: str) -> Optional[Market]:
         for market in Markets.markets_List:
```

### Comparing `spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.5.1/spotON_sdk/private_tests/create_spotON_Areas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
+from entsoe import Area 
 from dataclasses import dataclass
 from enum import Enum
 
 @dataclass
-class Area_details():
-    name:str
+class Area_details:
+    name: str
     code: str
     tz: str
-    # How can i add a name: str with the Object name example : name :str = AL
 
 @dataclass
 class spotON_Area():
     AL = Area_details('AL','10YAL-KESH-----5','Europe/Tirane')
     AT = Area_details('AT','10YAT-APG------L','Europe/Vienna')
     BA = Area_details('BA','10YBA-JPCC-----D','Europe/Sarajevo')
     BE = Area_details('BE','10YBE----------2','Europe/Brussels')
@@ -104,8 +104,19 @@
     TR = Area_details('TR','10YTR-TEIAS----W','Europe/Istanbul')
     UA = Area_details('UA','10Y1001C--00003F','Europe/Kiev')
     UA_BEI = Area_details('UA_BEI','10YUA-WEPS-----0','Europe/Kiev')
     UA_DOBTPP = Area_details('UA_DOBTPP','10Y1001A1001A869','Europe/Kiev')
     UA_IPS = Area_details('UA_IPS','10Y1001C--000182','Europe/Kiev')
     UK = Area_details('UK','10Y1001A1001A92E','Europe/London')
     XK = Area_details('XK','10Y1001C--00100H','Europe/Rome')
-    pass
+    pass
+
+def create():
+    # Create a list of all bidding zones
+    bidding_zones = [f"{area.name} = Area_details(name='{area.name}',code='{area.code}',tz='{area.tz}')" for area in Area]
+
+    bidding_zones.sort()
+    # Print all bidding zones
+    for zone in bidding_zones:
+        print(zone)
+
+create()
```

### Comparing `spotON_sdk-0.0.4.9991/spotON_sdk/Logic/Price/timeframes.py` & `spotON_sdk-0.0.5.1/spotON_sdk/Logic/Price/timeframes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from re import L
-from pydantic import BaseModel, validator
+from pydantic import validator
 from typing import List, Tuple
 from datetime import datetime, time
 
+from .customBaseModel import CustomBaseModel
 
 
-class Timeframe(BaseModel):
+class Timeframe(CustomBaseModel):
     start: int
     end: int
 
     @validator('*')
     def validate_hours(cls, value):
         if not 0 <= value < 24:
             raise ValueError("hours should be in range 0-23")
         return value
 
 
-class Timeframes(BaseModel):
+class Timeframes(CustomBaseModel):
     timeframes: List[Timeframe] =  [Timeframe(start=0, end=23)]
 
     @property
-    def possible_hours(self):
+    def possible_hours(self) -> List[int]:
         hours = set()
         for timeframe in self.timeframes:
             start, end = timeframe.start, timeframe.end
             end += 1
             if start <= end:
                 hours.update(range(start, end))
             else:  # the timeframe goes over midnight
```

### Comparing `spotON_sdk-0.0.4.9991/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.5.1/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.4.9991/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.5.1/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*


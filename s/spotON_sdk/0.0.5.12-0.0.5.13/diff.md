# Comparing `tmp/spotON_sdk-0.0.5.12.tar.gz` & `tmp/spotON_sdk-0.0.5.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotON_sdk-0.0.5.12.tar", last modified: Mon May 29 07:21:35 2023, max compression
+gzip compressed data, was "spotON_sdk-0.0.5.13.tar", last modified: Mon May 29 08:09:29 2023, max compression
```

## Comparing `spotON_sdk-0.0.5.12.tar` & `spotON_sdk-0.0.5.13.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.12/.gitignore
--rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.12/.gitmodules
--rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.12/LICENSE
--rw-r--r--   0        0        0      416 2023-05-29 06:36:38.819802 spotON_sdk-0.0.5.12/pyproject.toml
--rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Feedback/Feedback.py
--rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Feedback/Sensors.py
--rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Feedback/Units.py
--rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Feedback/__init__.py
--rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Output/Switchtypes.py
--rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Output/__init__.py
--rw-r--r--   0        0        0      385 2023-05-29 07:16:45.063497 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/API_Call.py
--rw-r--r--   0        0        0     2303 2023-05-28 16:41:31.459722 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/Price_Logic.py
--rw-r--r--   0        0        0      263 2023-05-28 19:44:31.805887 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/__init__.py
--rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/bidding_zones.py
--rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/countries.py
--rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/customBaseModel.py
--rw-r--r--   0        0        0     2806 2023-05-28 17:11:51.233618 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/markets.py
--rw-r--r--   0        0        0     8210 2023-05-28 16:32:06.404713 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/spotON_Areas.py
--rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/timeframes.py
--rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.5.12/spotON_sdk/Logic/__init__.py
--rw-r--r--   0        0        0      460 2023-05-29 07:21:26.348679 spotON_sdk-0.0.5.12/spotON_sdk/__init__.py
--rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.12/spotON_sdk/data_helpers/BestHour.py
--rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.5.12/spotON_sdk/data_helpers/__init__.py
--rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.12/spotON_sdk/data_helpers/dataframe_modifier.py
--rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.12/spotON_sdk/spotON_controller.py
--rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.12/PKG-INFO
+-rw-r--r--   0        0        0     6199 2023-05-29 06:07:03.308491 spotON_sdk-0.0.5.13/.gitignore
+-rw-r--r--   0        0        0      137 2023-05-28 19:57:55.289605 spotON_sdk-0.0.5.13/.gitmodules
+-rw-r--r--   0        0        0     1085 2023-05-06 14:04:24.538041 spotON_sdk-0.0.5.13/LICENSE
+-rw-r--r--   0        0        0      416 2023-05-29 06:36:38.819802 spotON_sdk-0.0.5.13/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-05-22 17:37:16.929836 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Feedback/Feedback.py
+-rw-r--r--   0        0        0      122 2023-05-13 12:18:00.893425 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Feedback/Sensors.py
+-rw-r--r--   0        0        0      429 2023-05-13 11:38:31.810517 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Feedback/Units.py
+-rw-r--r--   0        0        0      145 2023-05-22 08:52:45.547083 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Feedback/__init__.py
+-rw-r--r--   0        0        0       93 2023-05-22 16:38:29.648297 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Output/Switchtypes.py
+-rw-r--r--   0        0        0      104 2023-05-22 08:52:50.913401 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Output/__init__.py
+-rw-r--r--   0        0        0      385 2023-05-29 07:16:45.063497 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/API_Call.py
+-rw-r--r--   0        0        0     2303 2023-05-28 16:41:31.459722 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/Price_Logic.py
+-rw-r--r--   0        0        0      263 2023-05-28 19:44:31.805887 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/__init__.py
+-rw-r--r--   0        0        0      745 2023-05-08 10:18:24.622068 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/bidding_zones.py
+-rw-r--r--   0        0        0     4573 2023-05-28 16:48:16.706625 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/countries.py
+-rw-r--r--   0        0        0      156 2023-05-28 14:56:08.706388 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/customBaseModel.py
+-rw-r--r--   0        0        0     2872 2023-05-29 08:01:30.571565 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/markets.py
+-rw-r--r--   0        0        0     8239 2023-05-29 07:59:04.654185 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/spotON_Areas.py
+-rw-r--r--   0        0        0     1787 2023-05-28 14:59:11.652808 spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/timeframes.py
+-rw-r--r--   0        0        0      144 2023-05-22 18:00:58.368103 spotON_sdk-0.0.5.13/spotON_sdk/Logic/__init__.py
+-rw-r--r--   0        0        0      460 2023-05-29 08:09:26.884242 spotON_sdk-0.0.5.13/spotON_sdk/__init__.py
+-rw-r--r--   0        0        0      714 2023-05-22 18:11:54.358565 spotON_sdk-0.0.5.13/spotON_sdk/data_helpers/BestHour.py
+-rw-r--r--   0        0        0      136 2023-05-22 08:52:16.359432 spotON_sdk-0.0.5.13/spotON_sdk/data_helpers/__init__.py
+-rw-r--r--   0        0        0     1378 2023-05-22 08:52:33.315148 spotON_sdk-0.0.5.13/spotON_sdk/data_helpers/dataframe_modifier.py
+-rw-r--r--   0        0        0      336 2023-05-22 18:01:04.746198 spotON_sdk-0.0.5.13/spotON_sdk/spotON_controller.py
+-rw-r--r--   0        0        0      251 1970-01-01 00:00:00.000000 spotON_sdk-0.0.5.13/PKG-INFO
```

### Comparing `spotON_sdk-0.0.5.12/.gitignore` & `spotON_sdk-0.0.5.13/.gitignore`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.12/LICENSE` & `spotON_sdk-0.0.5.13/LICENSE`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/Price_Logic.py` & `spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/Price_Logic.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/bidding_zones.py` & `spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/bidding_zones.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/countries.py` & `spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/countries.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/markets.py` & `spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/markets.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,21 @@
     country: Country
     alias: Optional[str] = None
     area_code: str = Field(default="")
     country_code: str = Field(default="")
     region_code: Optional[str] = None
     cities: str = Field(default="")
     name: str = Field(default="")
-    @root_validator(pre=True)
+
+    '''@root_validator(pre=True)
     def set_codes(cls, values):
         area = values.get('area')
+        print(type(area))
         area_code = area.name
+        print(type(area_code))
         values['area_code'] = area_code
 
         country_region = area_code.split("_")
         values['country_code'] = country_region[0]
         if len(country_region) >=2:
             values['region_code'] = country_region[1]
 
@@ -42,29 +45,29 @@
         return values
 
 
         #TODO: Add emoji to name
         self.name = f"{self.country.country_name} {self.area_code} {self.cities}"
         self.name = f" {self.country.country_name}"
 
-        '''self.name = f"{self.country.emoji} {self.country.country_name} {self.area_code} {self.cities}"
+        self.name = f"{self.country.emoji} {self.country.country_name} {self.area_code} {self.cities}"
         self.name = f"{self.country.emoji} {self.country.country_name}"'''
 
         #self.get_Market_by_area_code(self.area.name)
 
 
 
 
 
 
-@dataclass
 class Markets():
-    austria = Market(area=spotON_Area.AT,country=all_Countries.Austria)
-    germany = Market(area=spotON_Area.DE,country=all_Countries.Germany)
-    sweden1 = Market(area=spotON_Area.SE_1,country=all_Countries.Sweden)    
+
+    austria = Market(area=spotON_Area.AT.value,country=all_Countries.Austria)
+    germany = Market(area=spotON_Area.DE.value,country=all_Countries.Germany)
+    sweden1 = Market(area=spotON_Area.SE_1.value,country=all_Countries.Sweden)    
     #luxembourg = Market(Area.DE_LU,Luxembourg)
 
     #sweden2 = Market(Area.SE_2,Sweden)
     #sweden3 = Market(Area.SE_3,Sweden)
     #sweden4 = Market(Area.SE_4,Sweden)
     markets_List = [value for key, value in vars().items() if isinstance(value, Market)]
     merged_Markets = []
```

### Comparing `spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/spotON_Areas.py` & `spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/spotON_Areas.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from dataclasses import dataclass
 from enum import Enum
+
+from pydantic import BaseModel
 from .customBaseModel import CustomBaseModel
 
-class Area_details(CustomBaseModel):
+class Area_details(BaseModel):
     name: str
     code: str
     tz: str
 
 
 
-@dataclass(frozen=True)
-class spotON_Area():
+from enum import Enum
+
+class spotON_Area(Enum):
     AL = Area_details(name='AL',code='10YAL-KESH-----5',tz='Europe/Tirane')
     AT = Area_details(name='AT',code='10YAT-APG------L',tz='Europe/Vienna')
     BA = Area_details(name='BA',code='10YBA-JPCC-----D',tz='Europe/Sarajevo')
     BE = Area_details(name='BE',code='10YBE----------2',tz='Europe/Brussels')
     BG = Area_details(name='BG',code='10YCA-BULGARIA-R',tz='Europe/Sofia')
     BY = Area_details(name='BY',code='10Y1001A1001A51S',tz='Europe/Minsk')
     CH = Area_details(name='CH',code='10YCH-SWISSGRIDZ',tz='Europe/Zurich')
```

### Comparing `spotON_sdk-0.0.5.12/spotON_sdk/Logic/Price/timeframes.py` & `spotON_sdk-0.0.5.13/spotON_sdk/Logic/Price/timeframes.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.12/spotON_sdk/data_helpers/BestHour.py` & `spotON_sdk-0.0.5.13/spotON_sdk/data_helpers/BestHour.py`

 * *Files identical despite different names*

### Comparing `spotON_sdk-0.0.5.12/spotON_sdk/data_helpers/dataframe_modifier.py` & `spotON_sdk-0.0.5.13/spotON_sdk/data_helpers/dataframe_modifier.py`

 * *Files identical despite different names*


# Comparing `tmp/iotcore_api-1.1.0.tar.gz` & `tmp/iotcore_api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotcore_api-1.1.0.tar", max compression
+gzip compressed data, was "iotcore_api-1.1.1.tar", max compression
```

## Comparing `iotcore_api-1.1.0.tar` & `iotcore_api-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.0/iotcoreapi/__init__.py
--rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.0/iotcoreapi/exceptions.py
--rw-r--r--   0        0        0    55577 2023-05-16 09:02:50.068030 iotcore_api-1.1.0/iotcoreapi/iotcoreapi.py
--rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.0/iotcoreapi/nan_treatment.py
--rw-r--r--   0        0        0      782 2023-05-15 16:04:32.304013 iotcore_api-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    34114 2023-05-16 10:19:21.723415 iotcore_api-1.1.0/README.md
--rw-r--r--   0        0        0    33711 1970-01-01 00:00:00.000000 iotcore_api-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.1/iotcoreapi/__init__.py
+-rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.1/iotcoreapi/exceptions.py
+-rw-r--r--   0        0        0    56470 2023-05-29 09:35:28.774184 iotcore_api-1.1.1/iotcoreapi/iotcoreapi.py
+-rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.1/iotcoreapi/nan_treatment.py
+-rw-r--r--   0        0        0      678 2023-05-29 09:47:13.685795 iotcore_api-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    34478 2023-05-29 09:40:36.225358 iotcore_api-1.1.1/README.md
+-rw-r--r--   0        0        0    33951 1970-01-01 00:00:00.000000 iotcore_api-1.1.1/PKG-INFO
```

### Comparing `iotcore_api-1.1.0/iotcoreapi/exceptions.py` & `iotcore_api-1.1.1/iotcoreapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.0/iotcoreapi/iotcoreapi.py` & `iotcore_api-1.1.1/iotcoreapi/iotcoreapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,81 +13,59 @@
 import urllib3
 from pandas import json_normalize
 from iotcoreapi.exceptions import IotCoreAPIException
 import warnings
 import re
 
 from iotcoreapi.nan_treatment import nan_treatment
+import typing
 
 
-class IoTCoreAPI:
-    @staticmethod
-    def _warnings_and_json_wrapper(func):
-        """Decorator including InsecureRequestWarning and then JSON() format"""
-
-        def f(*args, **kwargs):
-            urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-            rv = func(*args, **kwargs)
-            if rv.status_code == 200:
-                return rv.json()
-            else:
-                raise IotCoreAPIException(rv)
+def _warnings_and_json_wrapper(func):
+    """Decorator including InsecureRequestWarning and then JSON() format"""
 
-        return f
+    def f(*args, **kwargs):
+        urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
+        rv = func(*args, **kwargs)
+        if rv.status_code == 200:
+            return rv.json()
+        else:
+            raise IotCoreAPIException(rv)
 
-    @staticmethod
-    def _no_row_limit_decorator(fnc):
-        """Decorator to remove row limit in post methods"""
-
-        @wraps(fnc)
-        def wrapper(*args, **kwargs):
-            NX = args[0]
-            df_nexus = args[1]
-            n = len(df_nexus)
-            if n > 49999:
-                iter = round(n / 49999)
-                for j in range(iter):
-                    ini = j * 49999
-                    fin = (j + 1) * 49999
-                    if fin < n:
-                        df_nexus_write = df_nexus[ini:fin]
-                    else:
-                        df_nexus_write = df_nexus[ini:n]
-                    response = fnc(NX, df_nexus_write)
-            else:
-                response = fnc(NX, df_nexus)
-            return response
+    return f
 
-        return wrapper
 
-    def _convert_response(self, response: dict | list[dict], output_format: str,
-                          time_format: str = None, nan_method: str = None) -> pd.DataFrame | dict | list[dict]:
-        """
-        Auxiliary function to transform response in json format to dataframe if indicated in output_format arg.
-        Args:
-            response: json
-            output_format: 'dataframe' or 'json'
-            time_format: 'datetime' or 'unix'
-            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+def _no_row_limit_decorator(fnc):
+    """Decorator to remove row limit in post methods"""
 
-        Returns:
-            response: json or dataframe
-        """
-        if output_format == 'dataframe':
-            if response:
-                response = self._json_normalize_check(response)
-                if time_format == 'datetime':
-                    response['timeStamp'] = pd.to_datetime(response.timeStamp, unit='s', utc=True)
-                if nan_method is not None:
-                    response = nan_treatment(response, nan_method)
-            else:
-                response = pd.DataFrame(columns=['timeStamp', 'uid', 'name', 'value'])
+    @wraps(fnc)
+    def wrapper(*args, **kwargs):
+        NX = args[0]
+        df_nexus = args[1]
+        n = len(df_nexus)
+        if n > 49999:
+            iter = round(n / 49999)
+            for j in range(iter):
+                ini = j * 49999
+                fin = (j + 1) * 49999
+                if fin < n:
+                    df_nexus_write = df_nexus[ini:fin]
+                else:
+                    df_nexus_write = df_nexus[ini:n]
+                response = fnc(NX, df_nexus_write)
+        else:
+            response = fnc(NX, df_nexus)
         return response
 
-    def __init__(self, ip: str = "localhost", port: int = 56000, token: str = "", version: str | int = "3.0",
+    return wrapper
+
+
+class IoTCoreAPI:
+
+    def __init__(self, ip: str = "localhost", port: int = 56000, token: str = "", version: typing.Union[str, int] = "3.0",
                  logger: logging.Logger = None):
         """
         Init method for iotcoreapi. Needs API configuration parameters
 
         Args:
             ip: IoT Core base endpoint
             port: API Port. Defaults to 56000
@@ -111,14 +89,38 @@
             "nexustoken": self.token,
             "nexusapiversion": self.version,
             "Content-Type": "application/json",
         }
         self.logger = logger
         self._log_print("Created new instance of IoTCoreAPI")
 
+    def _convert_response(self, response: typing.Union[dict, typing.List[dict]], output_format: str,
+                          time_format: str = None, nan_method: str = None) -> typing.Union[pd.DataFrame, dict, typing.List[dict]]:
+        """
+        Auxiliary function to transform response in json format to dataframe if indicated in output_format arg.
+        Args:
+            response: json
+            output_format: 'dataframe' or 'json'
+            time_format: 'datetime' or 'unix'
+            nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
+
+        Returns:
+            response: json or dataframe
+        """
+        if output_format == 'dataframe':
+            if response:
+                response = self._json_normalize_check(response)
+                if time_format == 'datetime':
+                    response['timeStamp'] = pd.to_datetime(response.timeStamp, unit='s', utc=True)
+                if nan_method is not None:
+                    response = nan_treatment(response, nan_method)
+            else:
+                response = pd.DataFrame(columns=['timeStamp', 'uid', 'name', 'value'])
+        return response
+
     def _log_print(self, message, severity='info'):
         if self.logger is not None:
             if severity == 'info':
                 self.logger.info(message)
             elif severity == 'error':
                 self.logger.error(message)
             elif severity == 'debug':
@@ -126,15 +128,15 @@
             elif severity == 'warning':
                 self.logger.warning(message)
             else:
                 raise ValueError('Severity not supported')
         else:
             print(message)
 
-    def _json_normalize_check(self, response: dict | list[dict]) -> pd.DataFrame:
+    def _json_normalize_check(self, response: typing.Union[dict, typing.List[dict]]) -> pd.DataFrame:
         """
         Intenta convertir a DataFrame la respuesta en json de la API. Si no es posible, es que ha habido un fallo (la respuesta no sigue el formato establecido)
 
         Args:
             response: json con valor de la llamada a NexusAPI
         """
         try:
@@ -151,15 +153,16 @@
     @_warnings_and_json_wrapper
     def _postResponse(self, url, body):
         """POST method using Request"""
         return requests.post(url, verify=False, headers=self.header, data=body)
 
     # --------- CATALOGUE METHODS -----------------
 
-    def catalogue_tags(self, include_attributes: bool = True, output_format: str = 'dataframe') -> dict | pd.DataFrame:
+    def catalogue_tags(self, include_attributes: bool = True, output_format: str = 'dataframe') -> typing.Union[
+        dict, pd.DataFrame]:
         """Return all tags available for the token
 
         Args:
             include_attributes (optional): if version >3.0, bool to return attributes or not
             output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 
         Returns:
@@ -171,18 +174,18 @@
         url = self.url_NX + "/api/Tags"
         if self._version_number >= 3.0:
             params = {"IncludeAttributes": include_attributes}
         else:
             params = None
         return self._convert_response(self._getResponse(url, params), output_format)
 
-    def catalogue_tags_filtered(self, installations: list | str = None, drivers: list | str = None,
-                                tags: list | str = None,
-                                attributes: list | str = None,
-                                output_format: str = 'dataframe') -> dict | pd.DataFrame:
+    def catalogue_tags_filtered(self, installations: typing.Union[list, str] = None, drivers: typing.Union[list, str] = None,
+                                tags: typing.Union[list, str] = None,
+                                attributes: typing.Union[list, str] = None,
+                                output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]:
         """Searching for tags that comply with a certain criteria can be achieved with the filtered route. If fields are empty, all tags are returned.
 
         Args:
             installations: name of the installations
             drivers: name of drivers
             tags: name of tags
             attributes: not implemented yet
@@ -209,15 +212,15 @@
         body = json.dumps(
             {"SearchByInstallationName": parameters['installations'], "SearchByDriverName": parameters['drivers'],
              "SearchByTagName": parameters['tags']})
         url = self.url_NX + "/api/Tags/filtered"
         response = self._postResponse(url, body)
         return self._convert_response(response, output_format)
 
-    def catalogue_tags_attributes(self, output_format: str = 'dataframe') -> dict | pd.DataFrame:
+    def catalogue_tags_attributes(self, output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]:
         """Obtaining the list of possible attributes within the system and, when limited to a set of values, the list of possible values
 
         Args:
             output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 
         Returns:
             response in json or dataframe
@@ -227,15 +230,15 @@
             raise ValueError(f'output_format must be in {self._output_formats}')
         if self._version_number < 3:
             raise NotImplementedError('Nexus API version must be greater than 3.0')
         url = self.url_NX + "/api/Tags/Attributes"
         response = self._getResponse(url)
         return self._convert_response(response, output_format)
 
-    def catalogue_tags_writable(self, output_format: str = 'dataframe') -> dict | pd.DataFrame:
+    def catalogue_tags_writable(self, output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]:
         """Return tags available for writing. If version is under 3.0, returned array does not have attribute information
 
         Args:
             output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 
         Returns:
             response in json
@@ -243,15 +246,15 @@
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
         url = self.url_NX + "/api/Tags/writable"
         response = self._getResponse(url)
         return self._convert_response(response, output_format)
 
-    def catalogue_documents(self, output_format: str = 'dataframe') -> dict | pd.DataFrame:
+    def catalogue_documents(self, output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]:
         """Returns all tagviews shared in the token
 
         Args:
             output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 
         Returns:
             response in json
@@ -259,15 +262,15 @@
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
         url_completa = self.url_NX + "/api/Documents"
         response = self._getResponse(url_completa)
         return self._convert_response(response, output_format)
 
-    def catalogue_tagview_detail(self, uid: str, output_format: str = 'dataframe') -> dict | pd.DataFrame:
+    def catalogue_tagview_detail(self, uid: str, output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]:
         """Return all variables from a given tagview
 
         Args:
             uid: uid of the tagview
             output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 
         Returns:
@@ -279,15 +282,16 @@
         url = self.url_NX + "/api/Documents/tagviews/" + uid
         response = self._getResponse(url)
         if output_format == 'dataframe':
             if response:
                 response = self._json_normalize_check(response['columns'])
         return response
 
-    def catalogue_alarms(self, group_uid: str = None, output_format: str = 'dataframe') -> list[dict] | pd.DataFrame:
+    def catalogue_alarms(self, group_uid: str = None, output_format: str = 'dataframe') -> typing.Union[
+        typing.List[dict], pd.DataFrame]:
         """Returns information of the alarms in the token
 
         Args:
             group_uid : Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 
         Returns:
@@ -299,15 +303,15 @@
         if self._version_number < 2:
             raise NotImplementedError('Version 1.0 does not support alarm methods')
         params = {'GroupUid': group_uid}
         url_completa = self.url_NX + "/api/Alarms"
         response = self._getResponse(url_completa, params)
         return self._convert_response(response, output_format)
 
-    def catalogue_alarm_groups(self, output_format: str = 'dataframe') -> list[dict] | pd.DataFrame:
+    def catalogue_alarm_groups(self, output_format: str = 'dataframe') -> typing.Union[typing.List[dict], pd.DataFrame]:
         """Returns information of the alarm groups in the token
 
         Args:
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 
         Returns:
             response in json
@@ -319,16 +323,16 @@
             raise NotImplementedError('Version 1.0 does not support alarm methods')
         url_completa = self.url_NX + "/api/Alarms/Groups"
         response = self._getResponse(url_completa)
         return self._convert_response(response, output_format)
 
     # -------- READING OPERATIONS --------
 
-    def read_tags_realtime(self, tags_uids: list[str], output_format: str = 'dataframe',
-                           time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
+    def read_tags_realtime(self, tags_uids: typing.List[str], output_format: str = 'dataframe',
+                           time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """Reads real time value of the tags provided in the array tags_uids
 
         Args:
             tags_uids : list with uids of the tags
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
@@ -343,17 +347,17 @@
             raise ValueError(f'time_format must be in {self._time_formats}')
         body = json.dumps(tags_uids)
         url = self.url_NX + "/api/Tags/realtime"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
-    def read_tagview_realtime(self, uid: str, uids_tags: list[str] = None,
+    def read_tagview_realtime(self, uid: str, uids_tags: typing.List[str] = None,
                               output_format: str = 'dataframe',
-                              time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
+                              time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """Returns real time value for the uids variables provided in a given tagview
 
         Args:
             uid : uid of the tagview
             uids_tags : list of uids
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
@@ -371,18 +375,18 @@
             uids_tags = []
         body = json.dumps(uids_tags)
         url = self.url_NX + "/api/Documents/tagviews/" + uid + "/realtime"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
-    def read_tags_historic(self, uids: list[str], start_ts: int | float, end_ts: int | float,
-                           data_source: str | int = 'RAW', resolution: str | int = 'RES_1_HOUR',
-                           agg_operation: str | int = "LAST_VALUE", output_format: str = 'dataframe',
-                           time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
+    def read_tags_historic(self, uids: typing.List[str], start_ts: typing.Union[int, float], end_ts: typing.Union[int, float],
+                           data_source: typing.Union[str, int] = 'RAW', resolution: typing.Union[str, int] = 'RES_1_HOUR',
+                           agg_operation: typing.Union[str, int] = "LAST_VALUE", output_format: str = 'dataframe',
+                           time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """Obtain historic data of the specified tags
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
             start_ts: start time in unix time or datetime
             end_ts: end time in unix time or datetime
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
@@ -414,15 +418,15 @@
              "aggOperation": agg_operation})
         url = self.url_NX + "/api/Tags/historic"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tags_rawhistoric(self, uids, start_ts, end_ts, output_format: str = 'dataframe',
-                              time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
+                              time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """To obtain raw data with no aggregation or normalization applied
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
             start_ts: start time in unix time or datetime
             end_ts: end time in unix time or datetime
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
@@ -446,19 +450,19 @@
             end_ts = end_ts.timestamp()
         body = json.dumps({"uids": uids, "startTs": start_ts, "endTs": end_ts})
         url = self.url_NX + "/api/Tags/rawhistoric"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
-    def read_tags_transient(self, uids: list[str], start_ts: int | float, end_ts: int | float,
-                            data_source: str | int = None,
-                            resolution: str | int = 'RES_1_SEC',
+    def read_tags_transient(self, uids: typing.List[str], start_ts: typing.Union[int, float], end_ts: typing.Union[int, float],
+                            data_source: typing.Union[str, int] = None,
+                            resolution: typing.Union[str, int] = 'RES_1_SEC',
                             output_format: str = 'dataframe',
-                            time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
+                            time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """
         This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
         aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
         please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
         for historic.
 
         Args:
@@ -491,18 +495,19 @@
         body = json.dumps(
             {"uids": uids, "startTs": start_ts, "endTs": end_ts, "resolution": resolution})
         url = self.url_NX + "/api/Tags/transient"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
-    def read_tagview_historic(self, uid: str, start_ts: datetime.datetime | float | int,
-                              end_ts: datetime.datetime | float | int, tags_uids: list[str] = None, data_source='RAW',
+    def read_tagview_historic(self, uid: str, start_ts: typing.Union[datetime.datetime, float, int],
+                              end_ts: typing.Union[datetime.datetime, float, int], tags_uids: typing.List[str] = None,
+                              data_source='RAW',
                               resolution='RES_1_HOUR', output_format: str = 'dataframe',
-                              time_format='datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
+                              time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
 
         Args:
             uid: uid of the tagview
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
             tags_uids (optional): list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
@@ -531,27 +536,28 @@
             {"uids": tags_uids, "startTs": start_ts, "endTs": end_ts, "dataSource": data_source,
              "resolution": resolution})
         url = self.url_NX + "/api/Documents/tagviews/" + uid + "/historic"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
-    def read_tagview_historic_text_filters(self, uid_tagview: str, start_ts: datetime.datetime | float | int,
-                                           end_ts: datetime.datetime | float | int,
-                                           filter_txt: str | list[str] = None, data_source: str = 'RAW',
+    def read_tagview_historic_text_filters(self, uid_tagview: str, start_ts: typing.Union[datetime.datetime, float, int],
+                                           end_ts: typing.Union[datetime.datetime, float, int],
+                                           filter_txt: typing.Union[str, typing.List[str]] = None, data_source: str = 'RAW',
                                            resolution: str = 'RES_1_HOUR', output_format: str = 'dataframe',
-                                           time_format: str = 'datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
+                                           time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, \
+                                                                                                     typing.List[dict]]:
         """
         Read dataview historic data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             uid_tagview: uid of the tagview
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
-            filter_txt): text filters to search tags in tagviews. If None, will take all tags in tagview
+            filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
@@ -589,18 +595,18 @@
             filtered_hist['name'] = filtered_hist['uid'].map(diccio)
         else:
             for item in filtered_hist:
                 item['name'] = diccio[item['uid']]
         return filtered_hist
 
     def read_tagview_realtime_text_filters(self, uid_tagview: str,
-                                           filter_txt: str | list[str] = None,
+                                           filter_txt: typing.Union[str, typing.List[str]] = None,
                                            output_format: str = 'dataframe',
                                            time_format: str = 'datetime',
-                                           nan_method: str = None) -> pd.DataFrame | list[dict]:
+                                           nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """
         Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             uid_tagview: uid of the tagview
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
@@ -635,20 +641,21 @@
         if isinstance(filtered_hist, pd.DataFrame):
             filtered_hist['name'] = filtered_hist['uid'].map(diccio)
         else:
             for item in filtered_hist:
                 item['name'] = diccio[item['uid']]
         return filtered_hist
 
-    def read_tags_historic_text_filters(self, uids: list[str], start_ts: datetime.datetime | int | float,
-                                        end_ts: datetime.datetime | int | float,
-                                        filter_txt: str | list[str] = None, data_source: str | int = 'RAW',
-                                        resolution: str | int = 'RES_1_HOUR',
-                                        agg_operation: str | int = "LAST_VALUE", output_format: str = 'dataframe',
-                                        time_format: str = 'datetime', nan_method: str = None) -> pd.DataFrame | list[dict]:
+    def read_tags_historic_text_filters(self, uids: typing.List[str], start_ts: typing.Union[datetime.datetime, int, float],
+                                        end_ts: typing.Union[datetime.datetime, int, float],
+                                        filter_txt: typing.Union[str, typing.List[str]] = None, data_source: typing.Union[str, int] = 'RAW',
+                                        resolution: typing.Union[str, int] = 'RES_1_HOUR',
+                                        agg_operation: typing.Union[str, int] = "LAST_VALUE", output_format: str = 'dataframe',
+                                        time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[
+        dict]]:
         """Obtain historic data of the specified tags by name
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
@@ -692,18 +699,18 @@
             filtered_hist['name'] = filtered_hist['uid'].map(diccio)
         else:
             for item in filtered_hist:
                 item['name'] = diccio[item['uid']]
         return filtered_hist
 
     def read_tags_realtime_text_filters(self,
-                                        filter_txt: str | list[str] = None,
+                                        filter_txt: typing.Union[str, typing.List[str]] = None,
                                         output_format: str = 'dataframe',
                                         time_format: str = 'datetime',
-                                        nan_method: str = None) -> pd.DataFrame | list[dict]:
+                                        nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """
         Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
             output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
             time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
@@ -770,15 +777,15 @@
         if self._version_number < 3:
             raise NotImplementedError('Nexus API version must be greater than 3.0')
         url = self.url_NX + "/api/Alarms/Status/" + alarm_guid
         return self._getResponse(url)
 
     # -------- WRITING OPERATIONS -------------
 
-    def write_tags_insert(self, tags: str | list[str]) -> list[dict]:
+    def write_tags_insert(self, tags: typing.Union[str, typing.List[str]]) -> typing.List[dict]:
         """
         Check if provided tag names exist, then create them if not
 
         Args:
             tags: tags name or names to be created
 
         Returns:
@@ -805,15 +812,15 @@
         if isinstance(tags, str):
             tags = [tags]
         body = json.dumps(tags)
         self._log_print(f'Tags to be created: {body}')
         url_post = self.url_NX + "/api/Tags/Insert"
         return self._postResponse(url_post, body)
 
-    def write_tag_insert_or_update(self, tagname, **attributes) -> list[dict]:
+    def write_tag_insert_or_update(self, tagname, **attributes) -> typing.List[dict]:
         """This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
         Args:
             tagname: name of the new tag
             **attributes: dictionary of attributes and their values
 
         Returns:
@@ -826,15 +833,15 @@
         if self._version_number < 3:
             raise NotImplementedError('Nexus API version must be greater than 3.0')
         attribute_list = [{"attributeName": name, "value": value} for name, value in attributes.items()]
         body = json.dumps([{"Name": tagname, "Attributes": attribute_list}])
         url = self.url_NX + "/api/Tags/InsertOrUpdate"
         return self._postResponse(url, body)
 
-    def write_tags_insert_or_update_by_json(self, tags_and_attributes: list[dict]):
+    def write_tags_insert_or_update_by_json(self, tags_and_attributes: typing.List[dict]):
         """This method creates the tags with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
         Args:
             tags_and_attributes: json list containing info for each tag:
                 [
                     {
                     "Name": "name of the new tag",
@@ -855,24 +862,24 @@
         if self._version_number < 3:
             raise NotImplementedError('Nexus API version must be greater than 3.0')
         body = json.dumps(tags_and_attributes)
         url = self.url_NX + "/api/Tags/InsertOrUpdate"
         return self._postResponse(url, body)
 
     @_no_row_limit_decorator
-    def write_tags_historic_insert(self, df: pd.DataFrame, skip_errors: bool = True) -> list[dict]:
+    def write_tags_historic_insert(self, df: pd.DataFrame, skip_errors: bool = True) -> typing.List[dict]:
         """Update historical data for tags. Tags need to be created with write_tags_insert first.
 
         Args:
             df: dataframe
                 columns:
                     name: name of the tag
                     value : value of the tag
                     timeStamp: timeStamp in unix
-            skip_errors = True: If true, not created tags will be dropped from dataframe
+            skip_errors: True: If true, not created tags will be dropped from dataframe
 
         Returns:
             response in json format
         """
         # la funcion mira cuantas variables diferentes contiene el dataframe y comprueba si todas ellas existen
         vbles = list(df.name.unique())
         n_tags = len(vbles)
@@ -910,15 +917,15 @@
 
         Args:
             df: dataframe
                 columns:
                     name: name of the tag
                     value : value of the tag
                     timeStamp (optional): timeStamp in unix. If not provided, will take current time
-            skip_errors  = True: If true, not created tags will be dropped from dataframe
+            skip_errors: True: If true, not created tags will be dropped from dataframe
 
         Returns:
             response text (None if OK)
         """
         vbles = list(df.name.unique())
         n_tags = len(vbles)
         # Check if tags exists
@@ -945,15 +952,15 @@
             df2['timeStamp'] = df2['timeStamp'].astype('int64') / 1e9
         payload = pandas.DataFrame.to_json(df2, date_format="epoch", orient="records")
         url_completa = self.url_NX + "/api/Tags/realtime/insert"
         response = self._postResponse(url_completa, payload)
         self._log_print(f'Successfully written {n_tags} tags')
         return response
 
-    def write_tag_realtime_insert(self, name: str, value: float | int, timeStamp=None):
+    def write_tag_realtime_insert(self, name: str, value: typing.Union[float, int], timeStamp=None):
         """Update realtime data for a single tag. Tag needs to be created with write_tags_insert first.
 
         Args:
             name: tag name
             value: value of the tag
             timeStamp (optional): time in unix time. If None, will take current time
 
@@ -993,15 +1000,15 @@
 
         url_completa = self.url_NX + "/api/Tags/realtime/insert"
         response = self._postResponse(url_completa, payload)
         self._log_print(f'Successfully written {name}: {value}')
         return response
 
     @_no_row_limit_decorator
-    def write_tags_transient_insert(self, df: pd.DataFrame, skip_errors: bool = True) -> list[dict]:
+    def write_tags_transient_insert(self, df: pd.DataFrame, skip_errors: bool = True) -> typing.List[dict]:
         """Update transient data for tags. Tags need to be created with write_tags_insert first.
 
         Args:
             df: dataframe
                 columns:
                     name: name of the tag
                     value : value of the tag
@@ -1089,15 +1096,15 @@
         url_completa = self.url_NX + "/api/Tags/operate"
         df = df[['uid', 'value']]
         payload = df.to_json(orient='records')
         response = self._postResponse(url_completa, payload)
         self._log_print(response)
         return response
 
-    def operate_tag_single(self, tag_uid: str, value: int | float):
+    def operate_tag_single(self, tag_uid: str, value: typing.Union[int, float]):
         """If the token has access to operate against a Conector associated with a PLC, this method can be used to write values to the actual Plc's tags.
 
         Args:
             tag_uid: nombre de la variable a escribir en el PLC
             value: valor de la variable a escribir
         """
         url_completa = self.url_NX + "/api/Tags/operate"
```

### Comparing `iotcore_api-1.1.0/iotcoreapi/nan_treatment.py` & `iotcore_api-1.1.1/iotcoreapi/nan_treatment.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.0/README.md` & `iotcore_api-1.1.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -222,15 +222,15 @@
 
 #### \_\_init\_\_
 
 ```python
 def __init__(ip: str = "localhost",
              port: int = 56000,
              token: str = "",
-             version: str | int = "3.0",
+             version: typing.Union[str, int] = "3.0",
              logger: logging.Logger = None)
 ```
 
 Init method for iotcoreapi. Needs API configuration parameters
 
 **Arguments**:
 
@@ -241,16 +241,17 @@
 - `logger` - Optional. Logger object to output log messages. If not provided, logger messages will be printed to console
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags"></a>
 
 #### catalogue\_tags
 
 ```python
-def catalogue_tags(include_attributes: bool = True,
-                   output_format: str = 'dataframe') -> dict | pd.DataFrame
+def catalogue_tags(
+        include_attributes: bool = True,
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Return all tags available for the token
 
 **Arguments**:
 
 - `include_attributes` _optional_ - if version >3.0, bool to return attributes or not
@@ -263,19 +264,19 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_filtered"></a>
 
 #### catalogue\_tags\_filtered
 
 ```python
 def catalogue_tags_filtered(
-        installations: list | str = None,
-        drivers: list | str = None,
-        tags: list | str = None,
-        attributes: list | str = None,
-        output_format: str = 'dataframe') -> dict | pd.DataFrame
+        installations: typing.Union[list, str] = None,
+        drivers: typing.Union[list, str] = None,
+        tags: typing.Union[list, str] = None,
+        attributes: typing.Union[list, str] = None,
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Searching for tags that comply with a certain criteria can be achieved with the filtered route. If fields are empty, all tags are returned.
 
 **Arguments**:
 
 - `installations` - name of the installations
@@ -291,15 +292,15 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_attributes"></a>
 
 #### catalogue\_tags\_attributes
 
 ```python
 def catalogue_tags_attributes(
-        output_format: str = 'dataframe') -> dict | pd.DataFrame
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Obtaining the list of possible attributes within the system and, when limited to a set of values, the list of possible values
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
@@ -311,15 +312,15 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_writable"></a>
 
 #### catalogue\_tags\_writable
 
 ```python
 def catalogue_tags_writable(
-        output_format: str = 'dataframe') -> dict | pd.DataFrame
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Return tags available for writing. If version is under 3.0, returned array does not have attribute information
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
@@ -331,15 +332,15 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_documents"></a>
 
 #### catalogue\_documents
 
 ```python
 def catalogue_documents(
-        output_format: str = 'dataframe') -> dict | pd.DataFrame
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Returns all tagviews shared in the token
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
@@ -350,17 +351,17 @@
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tagview_detail"></a>
 
 #### catalogue\_tagview\_detail
 
 ```python
-def catalogue_tagview_detail(uid: str,
-                             output_format: str = 'dataframe'
-                             ) -> dict | pd.DataFrame
+def catalogue_tagview_detail(
+        uid: str,
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Return all variables from a given tagview
 
 **Arguments**:
 
 - `uid` - uid of the tagview
@@ -373,16 +374,17 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarms"></a>
 
 #### catalogue\_alarms
 
 ```python
 def catalogue_alarms(
-        group_uid: str = None,
-        output_format: str = 'dataframe') -> list[dict] | pd.DataFrame
+    group_uid: str = None,
+    output_format: str = 'dataframe'
+) -> typing.Union[typing.List[dict], pd.DataFrame]
 ```
 
 Returns information of the alarms in the token
 
 **Arguments**:
 
   group_uid : Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
@@ -395,15 +397,16 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarm_groups"></a>
 
 #### catalogue\_alarm\_groups
 
 ```python
 def catalogue_alarm_groups(
-        output_format: str = 'dataframe') -> list[dict] | pd.DataFrame
+    output_format: str = 'dataframe'
+) -> typing.Union[typing.List[dict], pd.DataFrame]
 ```
 
 Returns information of the alarm groups in the token
 
 **Arguments**:
 
   output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
@@ -414,18 +417,20 @@
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime"></a>
 
 #### read\_tags\_realtime
 
 ```python
-def read_tags_realtime(tags_uids: list[str],
-                       output_format: str = 'dataframe',
-                       time_format='datetime',
-                       nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tags_realtime(
+        tags_uids: typing.List[str],
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Reads real time value of the tags provided in the array tags_uids
 
 **Arguments**:
 
   tags_uids : list with uids of the tags
@@ -439,19 +444,21 @@
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_realtime"></a>
 
 #### read\_tagview\_realtime
 
 ```python
-def read_tagview_realtime(uid: str,
-                          uids_tags: list[str] = None,
-                          output_format: str = 'dataframe',
-                          time_format='datetime',
-                          nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tagview_realtime(
+        uid: str,
+        uids_tags: typing.List[str] = None,
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Returns real time value for the uids variables provided in a given tagview
 
 **Arguments**:
 
   uid : uid of the tagview
@@ -466,23 +473,25 @@
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_historic"></a>
 
 #### read\_tags\_historic
 
 ```python
-def read_tags_historic(uids: list[str],
-                       start_ts: int | float,
-                       end_ts: int | float,
-                       data_source: str | int = 'RAW',
-                       resolution: str | int = 'RES_1_HOUR',
-                       agg_operation: str | int = "LAST_VALUE",
-                       output_format: str = 'dataframe',
-                       time_format='datetime',
-                       nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tags_historic(
+        uids: typing.List[str],
+        start_ts: typing.Union[int, float],
+        end_ts: typing.Union[int, float],
+        data_source: typing.Union[str, int] = 'RAW',
+        resolution: typing.Union[str, int] = 'RES_1_HOUR',
+        agg_operation: typing.Union[str, int] = "LAST_VALUE",
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Obtain historic data of the specified tags
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
@@ -501,20 +510,22 @@
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_rawhistoric"></a>
 
 #### read\_tags\_rawhistoric
 
 ```python
-def read_tags_rawhistoric(uids,
-                          start_ts,
-                          end_ts,
-                          output_format: str = 'dataframe',
-                          time_format='datetime',
-                          nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tags_rawhistoric(
+        uids,
+        start_ts,
+        end_ts,
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 To obtain raw data with no aggregation or normalization applied
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
@@ -530,22 +541,24 @@
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_transient"></a>
 
 #### read\_tags\_transient
 
 ```python
-def read_tags_transient(uids: list[str],
-                        start_ts: int | float,
-                        end_ts: int | float,
-                        data_source: str | int = None,
-                        resolution: str | int = 'RES_1_SEC',
-                        output_format: str = 'dataframe',
-                        time_format='datetime',
-                        nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tags_transient(
+        uids: typing.List[str],
+        start_ts: typing.Union[int, float],
+        end_ts: typing.Union[int, float],
+        data_source: typing.Union[str, int] = None,
+        resolution: typing.Union[str, int] = 'RES_1_SEC',
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
 aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
 please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
 for historic.
 
@@ -566,23 +579,25 @@
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_historic"></a>
 
 #### read\_tagview\_historic
 
 ```python
-def read_tagview_historic(uid: str,
-                          start_ts: datetime.datetime | float | int,
-                          end_ts: datetime.datetime | float | int,
-                          tags_uids: list[str] = None,
-                          data_source='RAW',
-                          resolution='RES_1_HOUR',
-                          output_format: str = 'dataframe',
-                          time_format='datetime',
-                          nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tagview_historic(
+        uid: str,
+        start_ts: typing.Union[datetime.datetime, float, int],
+        end_ts: typing.Union[datetime.datetime, float, int],
+        tags_uids: typing.List[str] = None,
+        data_source='RAW',
+        resolution='RES_1_HOUR',
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
 
 **Arguments**:
 
 - `uid` - uid of the tagview
@@ -601,34 +616,26 @@
   A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_historic_text_filters"></a>
 
 #### read\_tagview\_historic\_text\_filters
 
 ```python
-def read_tagview_historic_text_filters(
-        uid_tagview: str,
-        start_ts: datetime.datetime | float | int,
-        end_ts: datetime.datetime | float | int,
-        filter_txt: str | list[str] = None,
-        data_source: str = 'RAW',
-        resolution: str = 'RES_1_HOUR',
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tagview_historic_text_filters(uid_tagview: str, start_ts: typing.Union[datetime.datetime, float, int], end_ts: typing.Union[datetime.datetime, float, int], filter_txt: typing.Union[str, typing.List[str]] = None, data_source: str = 'RAW', resolution: str = 'RES_1_HOUR', output_format: str = 'dataframe', time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, \
+                                                                                                     typing.List[dict]]
 ```
 
 Read dataview historic data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `uid_tagview` - uid of the tagview
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
-- `filter_txt)` - text filters to search tags in tagviews. If None, will take all tags in tagview
+- `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
   output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
   time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
@@ -643,18 +650,19 @@
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_realtime_text_filters"></a>
 
 #### read\_tagview\_realtime\_text\_filters
 
 ```python
 def read_tagview_realtime_text_filters(
         uid_tagview: str,
-        filter_txt: str | list[str] = None,
+        filter_txt: typing.Union[str, typing.List[str]] = None,
         output_format: str = 'dataframe',
         time_format: str = 'datetime',
-        nan_method: str = None) -> pd.DataFrame | list[dict]
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `uid_tagview` - uid of the tagview
@@ -674,24 +682,25 @@
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_historic_text_filters"></a>
 
 #### read\_tags\_historic\_text\_filters
 
 ```python
 def read_tags_historic_text_filters(
-        uids: list[str],
-        start_ts: datetime.datetime | int | float,
-        end_ts: datetime.datetime | int | float,
-        filter_txt: str | list[str] = None,
-        data_source: str | int = 'RAW',
-        resolution: str | int = 'RES_1_HOUR',
-        agg_operation: str | int = "LAST_VALUE",
+        uids: typing.List[str],
+        start_ts: typing.Union[datetime.datetime, int, float],
+        end_ts: typing.Union[datetime.datetime, int, float],
+        filter_txt: typing.Union[str, typing.List[str]] = None,
+        data_source: typing.Union[str, int] = 'RAW',
+        resolution: typing.Union[str, int] = 'RES_1_HOUR',
+        agg_operation: typing.Union[str, int] = "LAST_VALUE",
         output_format: str = 'dataframe',
         time_format: str = 'datetime',
-        nan_method: str = None) -> pd.DataFrame | list[dict]
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Obtain historic data of the specified tags by name
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
@@ -712,18 +721,19 @@
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime_text_filters"></a>
 
 #### read\_tags\_realtime\_text\_filters
 
 ```python
 def read_tags_realtime_text_filters(
-        filter_txt: str | list[str] = None,
+        filter_txt: typing.Union[str, typing.List[str]] = None,
         output_format: str = 'dataframe',
         time_format: str = 'datetime',
-        nan_method: str = None) -> pd.DataFrame | list[dict]
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
@@ -776,15 +786,16 @@
   }
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_insert"></a>
 
 #### write\_tags\_insert
 
 ```python
-def write_tags_insert(tags: str | list[str]) -> list[dict]
+def write_tags_insert(
+        tags: typing.Union[str, typing.List[str]]) -> typing.List[dict]
 ```
 
 Check if provided tag names exist, then create them if not
 
 **Arguments**:
 
 - `tags` - tags name or names to be created
@@ -811,15 +822,15 @@
   ]
 
 <a id="iotcoreapi.IoTCoreAPI.write_tag_insert_or_update"></a>
 
 #### write\_tag\_insert\_or\_update
 
 ```python
-def write_tag_insert_or_update(tagname, **attributes) -> list[dict]
+def write_tag_insert_or_update(tagname, **attributes) -> typing.List[dict]
 ```
 
 This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
 **Arguments**:
 
 - `tagname` - name of the new tag
@@ -837,15 +848,16 @@
   response = write_tag_insert_or_update(tagname="mytag", attribute1="value1", attribute2="value2", attribute3="value3")
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_insert_or_update_by_json"></a>
 
 #### write\_tags\_insert\_or\_update\_by\_json
 
 ```python
-def write_tags_insert_or_update_by_json(tags_and_attributes: list[dict])
+def write_tags_insert_or_update_by_json(
+        tags_and_attributes: typing.List[dict])
 ```
 
 This method creates the tags with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
 **Arguments**:
 
 - `tags_and_attributes` - json list containing info for each tag:
@@ -871,27 +883,27 @@
 <a id="iotcoreapi.IoTCoreAPI.write_tags_historic_insert"></a>
 
 #### write\_tags\_historic\_insert
 
 ```python
 @_no_row_limit_decorator
 def write_tags_historic_insert(df: pd.DataFrame,
-                               skip_errors: bool = True) -> list[dict]
+                               skip_errors: bool = True) -> typing.List[dict]
 ```
 
 Update historical data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
   value : value of the tag
 - `timeStamp` - timeStamp in unix
-  skip_errors = True: If true, not created tags will be dropped from dataframe
+- `skip_errors` - True: If true, not created tags will be dropped from dataframe
   
 
 **Returns**:
 
   response in json format
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_realtime_insert"></a>
@@ -908,27 +920,29 @@
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
   value : value of the tag
 - `timeStamp` _optional_ - timeStamp in unix. If not provided, will take current time
-  skip_errors  = True: If true, not created tags will be dropped from dataframe
+- `skip_errors` - True: If true, not created tags will be dropped from dataframe
   
 
 **Returns**:
 
   response text (None if OK)
 
 <a id="iotcoreapi.IoTCoreAPI.write_tag_realtime_insert"></a>
 
 #### write\_tag\_realtime\_insert
 
 ```python
-def write_tag_realtime_insert(name: str, value: float | int, timeStamp=None)
+def write_tag_realtime_insert(name: str,
+                              value: typing.Union[float, int],
+                              timeStamp=None)
 ```
 
 Update realtime data for a single tag. Tag needs to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `name` - tag name
@@ -943,15 +957,15 @@
 <a id="iotcoreapi.IoTCoreAPI.write_tags_transient_insert"></a>
 
 #### write\_tags\_transient\_insert
 
 ```python
 @_no_row_limit_decorator
 def write_tags_transient_insert(df: pd.DataFrame,
-                                skip_errors: bool = True) -> list[dict]
+                                skip_errors: bool = True) -> typing.List[dict]
 ```
 
 Update transient data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
@@ -1019,15 +1033,15 @@
 - `value` - value to write
 
 <a id="iotcoreapi.IoTCoreAPI.operate_tag_single"></a>
 
 #### operate\_tag\_single
 
 ```python
-def operate_tag_single(tag_uid: str, value: int | float)
+def operate_tag_single(tag_uid: str, value: typing.Union[int, float])
 ```
 
 If the token has access to operate against a Conector associated with a PLC, this method can be used to write values to the actual Plc's tags.
 
 **Arguments**:
 
 - `tag_uid` - nombre de la variable a escribir en el PLC
```

### Comparing `iotcore_api-1.1.0/PKG-INFO` & `iotcore_api-1.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: iotcore-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: IoT core connection methods and utilities
-Home-page: https://nexusintegra.io
-Author: Nexus Integra
+Author: Idrica
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pandas (>=2.0.1,<3.0.0)
 Requires-Dist: requests (>=2.30.0,<3.0.0)
-Project-URL: Repository, https://github.com/NexusIntegra/iotcoreAPI
 Description-Content-Type: text/markdown
 
 # IoTCoreAPI
 
 Library to interact with IoTCoreAPI in Python
 
 ## Table Of Contents
@@ -239,15 +237,15 @@
 
 #### \_\_init\_\_
 
 ```python
 def __init__(ip: str = "localhost",
              port: int = 56000,
              token: str = "",
-             version: str | int = "3.0",
+             version: typing.Union[str, int] = "3.0",
              logger: logging.Logger = None)
 ```
 
 Init method for iotcoreapi. Needs API configuration parameters
 
 **Arguments**:
 
@@ -258,16 +256,17 @@
 - `logger` - Optional. Logger object to output log messages. If not provided, logger messages will be printed to console
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags"></a>
 
 #### catalogue\_tags
 
 ```python
-def catalogue_tags(include_attributes: bool = True,
-                   output_format: str = 'dataframe') -> dict | pd.DataFrame
+def catalogue_tags(
+        include_attributes: bool = True,
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Return all tags available for the token
 
 **Arguments**:
 
 - `include_attributes` _optional_ - if version >3.0, bool to return attributes or not
@@ -280,19 +279,19 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_filtered"></a>
 
 #### catalogue\_tags\_filtered
 
 ```python
 def catalogue_tags_filtered(
-        installations: list | str = None,
-        drivers: list | str = None,
-        tags: list | str = None,
-        attributes: list | str = None,
-        output_format: str = 'dataframe') -> dict | pd.DataFrame
+        installations: typing.Union[list, str] = None,
+        drivers: typing.Union[list, str] = None,
+        tags: typing.Union[list, str] = None,
+        attributes: typing.Union[list, str] = None,
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Searching for tags that comply with a certain criteria can be achieved with the filtered route. If fields are empty, all tags are returned.
 
 **Arguments**:
 
 - `installations` - name of the installations
@@ -308,15 +307,15 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_attributes"></a>
 
 #### catalogue\_tags\_attributes
 
 ```python
 def catalogue_tags_attributes(
-        output_format: str = 'dataframe') -> dict | pd.DataFrame
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Obtaining the list of possible attributes within the system and, when limited to a set of values, the list of possible values
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
@@ -328,15 +327,15 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tags_writable"></a>
 
 #### catalogue\_tags\_writable
 
 ```python
 def catalogue_tags_writable(
-        output_format: str = 'dataframe') -> dict | pd.DataFrame
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Return tags available for writing. If version is under 3.0, returned array does not have attribute information
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
@@ -348,15 +347,15 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_documents"></a>
 
 #### catalogue\_documents
 
 ```python
 def catalogue_documents(
-        output_format: str = 'dataframe') -> dict | pd.DataFrame
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Returns all tagviews shared in the token
 
 **Arguments**:
 
 - `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
@@ -367,17 +366,17 @@
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_tagview_detail"></a>
 
 #### catalogue\_tagview\_detail
 
 ```python
-def catalogue_tagview_detail(uid: str,
-                             output_format: str = 'dataframe'
-                             ) -> dict | pd.DataFrame
+def catalogue_tagview_detail(
+        uid: str,
+        output_format: str = 'dataframe') -> typing.Union[dict, pd.DataFrame]
 ```
 
 Return all variables from a given tagview
 
 **Arguments**:
 
 - `uid` - uid of the tagview
@@ -390,16 +389,17 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarms"></a>
 
 #### catalogue\_alarms
 
 ```python
 def catalogue_alarms(
-        group_uid: str = None,
-        output_format: str = 'dataframe') -> list[dict] | pd.DataFrame
+    group_uid: str = None,
+    output_format: str = 'dataframe'
+) -> typing.Union[typing.List[dict], pd.DataFrame]
 ```
 
 Returns information of the alarms in the token
 
 **Arguments**:
 
   group_uid : Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
@@ -412,15 +412,16 @@
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarm_groups"></a>
 
 #### catalogue\_alarm\_groups
 
 ```python
 def catalogue_alarm_groups(
-        output_format: str = 'dataframe') -> list[dict] | pd.DataFrame
+    output_format: str = 'dataframe'
+) -> typing.Union[typing.List[dict], pd.DataFrame]
 ```
 
 Returns information of the alarm groups in the token
 
 **Arguments**:
 
   output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
@@ -431,18 +432,20 @@
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime"></a>
 
 #### read\_tags\_realtime
 
 ```python
-def read_tags_realtime(tags_uids: list[str],
-                       output_format: str = 'dataframe',
-                       time_format='datetime',
-                       nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tags_realtime(
+        tags_uids: typing.List[str],
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Reads real time value of the tags provided in the array tags_uids
 
 **Arguments**:
 
   tags_uids : list with uids of the tags
@@ -456,19 +459,21 @@
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_realtime"></a>
 
 #### read\_tagview\_realtime
 
 ```python
-def read_tagview_realtime(uid: str,
-                          uids_tags: list[str] = None,
-                          output_format: str = 'dataframe',
-                          time_format='datetime',
-                          nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tagview_realtime(
+        uid: str,
+        uids_tags: typing.List[str] = None,
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Returns real time value for the uids variables provided in a given tagview
 
 **Arguments**:
 
   uid : uid of the tagview
@@ -483,23 +488,25 @@
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_historic"></a>
 
 #### read\_tags\_historic
 
 ```python
-def read_tags_historic(uids: list[str],
-                       start_ts: int | float,
-                       end_ts: int | float,
-                       data_source: str | int = 'RAW',
-                       resolution: str | int = 'RES_1_HOUR',
-                       agg_operation: str | int = "LAST_VALUE",
-                       output_format: str = 'dataframe',
-                       time_format='datetime',
-                       nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tags_historic(
+        uids: typing.List[str],
+        start_ts: typing.Union[int, float],
+        end_ts: typing.Union[int, float],
+        data_source: typing.Union[str, int] = 'RAW',
+        resolution: typing.Union[str, int] = 'RES_1_HOUR',
+        agg_operation: typing.Union[str, int] = "LAST_VALUE",
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Obtain historic data of the specified tags
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
@@ -518,20 +525,22 @@
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_rawhistoric"></a>
 
 #### read\_tags\_rawhistoric
 
 ```python
-def read_tags_rawhistoric(uids,
-                          start_ts,
-                          end_ts,
-                          output_format: str = 'dataframe',
-                          time_format='datetime',
-                          nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tags_rawhistoric(
+        uids,
+        start_ts,
+        end_ts,
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 To obtain raw data with no aggregation or normalization applied
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
@@ -547,22 +556,24 @@
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_transient"></a>
 
 #### read\_tags\_transient
 
 ```python
-def read_tags_transient(uids: list[str],
-                        start_ts: int | float,
-                        end_ts: int | float,
-                        data_source: str | int = None,
-                        resolution: str | int = 'RES_1_SEC',
-                        output_format: str = 'dataframe',
-                        time_format='datetime',
-                        nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tags_transient(
+        uids: typing.List[str],
+        start_ts: typing.Union[int, float],
+        end_ts: typing.Union[int, float],
+        data_source: typing.Union[str, int] = None,
+        resolution: typing.Union[str, int] = 'RES_1_SEC',
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
 aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
 please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
 for historic.
 
@@ -583,23 +594,25 @@
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_historic"></a>
 
 #### read\_tagview\_historic
 
 ```python
-def read_tagview_historic(uid: str,
-                          start_ts: datetime.datetime | float | int,
-                          end_ts: datetime.datetime | float | int,
-                          tags_uids: list[str] = None,
-                          data_source='RAW',
-                          resolution='RES_1_HOUR',
-                          output_format: str = 'dataframe',
-                          time_format='datetime',
-                          nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tagview_historic(
+        uid: str,
+        start_ts: typing.Union[datetime.datetime, float, int],
+        end_ts: typing.Union[datetime.datetime, float, int],
+        tags_uids: typing.List[str] = None,
+        data_source='RAW',
+        resolution='RES_1_HOUR',
+        output_format: str = 'dataframe',
+        time_format='datetime',
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
 
 **Arguments**:
 
 - `uid` - uid of the tagview
@@ -618,34 +631,26 @@
   A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
 
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_historic_text_filters"></a>
 
 #### read\_tagview\_historic\_text\_filters
 
 ```python
-def read_tagview_historic_text_filters(
-        uid_tagview: str,
-        start_ts: datetime.datetime | float | int,
-        end_ts: datetime.datetime | float | int,
-        filter_txt: str | list[str] = None,
-        data_source: str = 'RAW',
-        resolution: str = 'RES_1_HOUR',
-        output_format: str = 'dataframe',
-        time_format: str = 'datetime',
-        nan_method: str = None) -> pd.DataFrame | list[dict]
+def read_tagview_historic_text_filters(uid_tagview: str, start_ts: typing.Union[datetime.datetime, float, int], end_ts: typing.Union[datetime.datetime, float, int], filter_txt: typing.Union[str, typing.List[str]] = None, data_source: str = 'RAW', resolution: str = 'RES_1_HOUR', output_format: str = 'dataframe', time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, \
+                                                                                                     typing.List[dict]]
 ```
 
 Read dataview historic data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `uid_tagview` - uid of the tagview
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
-- `filter_txt)` - text filters to search tags in tagviews. If None, will take all tags in tagview
+- `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
   output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
   time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
@@ -660,18 +665,19 @@
 <a id="iotcoreapi.IoTCoreAPI.read_tagview_realtime_text_filters"></a>
 
 #### read\_tagview\_realtime\_text\_filters
 
 ```python
 def read_tagview_realtime_text_filters(
         uid_tagview: str,
-        filter_txt: str | list[str] = None,
+        filter_txt: typing.Union[str, typing.List[str]] = None,
         output_format: str = 'dataframe',
         time_format: str = 'datetime',
-        nan_method: str = None) -> pd.DataFrame | list[dict]
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `uid_tagview` - uid of the tagview
@@ -691,24 +697,25 @@
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_historic_text_filters"></a>
 
 #### read\_tags\_historic\_text\_filters
 
 ```python
 def read_tags_historic_text_filters(
-        uids: list[str],
-        start_ts: datetime.datetime | int | float,
-        end_ts: datetime.datetime | int | float,
-        filter_txt: str | list[str] = None,
-        data_source: str | int = 'RAW',
-        resolution: str | int = 'RES_1_HOUR',
-        agg_operation: str | int = "LAST_VALUE",
+        uids: typing.List[str],
+        start_ts: typing.Union[datetime.datetime, int, float],
+        end_ts: typing.Union[datetime.datetime, int, float],
+        filter_txt: typing.Union[str, typing.List[str]] = None,
+        data_source: typing.Union[str, int] = 'RAW',
+        resolution: typing.Union[str, int] = 'RES_1_HOUR',
+        agg_operation: typing.Union[str, int] = "LAST_VALUE",
         output_format: str = 'dataframe',
         time_format: str = 'datetime',
-        nan_method: str = None) -> pd.DataFrame | list[dict]
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Obtain historic data of the specified tags by name
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
@@ -729,18 +736,19 @@
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime_text_filters"></a>
 
 #### read\_tags\_realtime\_text\_filters
 
 ```python
 def read_tags_realtime_text_filters(
-        filter_txt: str | list[str] = None,
+        filter_txt: typing.Union[str, typing.List[str]] = None,
         output_format: str = 'dataframe',
         time_format: str = 'datetime',
-        nan_method: str = None) -> pd.DataFrame | list[dict]
+        nan_method: str = None
+) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
@@ -793,15 +801,16 @@
   }
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_insert"></a>
 
 #### write\_tags\_insert
 
 ```python
-def write_tags_insert(tags: str | list[str]) -> list[dict]
+def write_tags_insert(
+        tags: typing.Union[str, typing.List[str]]) -> typing.List[dict]
 ```
 
 Check if provided tag names exist, then create them if not
 
 **Arguments**:
 
 - `tags` - tags name or names to be created
@@ -828,15 +837,15 @@
   ]
 
 <a id="iotcoreapi.IoTCoreAPI.write_tag_insert_or_update"></a>
 
 #### write\_tag\_insert\_or\_update
 
 ```python
-def write_tag_insert_or_update(tagname, **attributes) -> list[dict]
+def write_tag_insert_or_update(tagname, **attributes) -> typing.List[dict]
 ```
 
 This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
 **Arguments**:
 
 - `tagname` - name of the new tag
@@ -854,15 +863,16 @@
   response = write_tag_insert_or_update(tagname="mytag", attribute1="value1", attribute2="value2", attribute3="value3")
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_insert_or_update_by_json"></a>
 
 #### write\_tags\_insert\_or\_update\_by\_json
 
 ```python
-def write_tags_insert_or_update_by_json(tags_and_attributes: list[dict])
+def write_tags_insert_or_update_by_json(
+        tags_and_attributes: typing.List[dict])
 ```
 
 This method creates the tags with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
 **Arguments**:
 
 - `tags_and_attributes` - json list containing info for each tag:
@@ -888,27 +898,27 @@
 <a id="iotcoreapi.IoTCoreAPI.write_tags_historic_insert"></a>
 
 #### write\_tags\_historic\_insert
 
 ```python
 @_no_row_limit_decorator
 def write_tags_historic_insert(df: pd.DataFrame,
-                               skip_errors: bool = True) -> list[dict]
+                               skip_errors: bool = True) -> typing.List[dict]
 ```
 
 Update historical data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
   value : value of the tag
 - `timeStamp` - timeStamp in unix
-  skip_errors = True: If true, not created tags will be dropped from dataframe
+- `skip_errors` - True: If true, not created tags will be dropped from dataframe
   
 
 **Returns**:
 
   response in json format
 
 <a id="iotcoreapi.IoTCoreAPI.write_tags_realtime_insert"></a>
@@ -925,27 +935,29 @@
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
   value : value of the tag
 - `timeStamp` _optional_ - timeStamp in unix. If not provided, will take current time
-  skip_errors  = True: If true, not created tags will be dropped from dataframe
+- `skip_errors` - True: If true, not created tags will be dropped from dataframe
   
 
 **Returns**:
 
   response text (None if OK)
 
 <a id="iotcoreapi.IoTCoreAPI.write_tag_realtime_insert"></a>
 
 #### write\_tag\_realtime\_insert
 
 ```python
-def write_tag_realtime_insert(name: str, value: float | int, timeStamp=None)
+def write_tag_realtime_insert(name: str,
+                              value: typing.Union[float, int],
+                              timeStamp=None)
 ```
 
 Update realtime data for a single tag. Tag needs to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `name` - tag name
@@ -960,15 +972,15 @@
 <a id="iotcoreapi.IoTCoreAPI.write_tags_transient_insert"></a>
 
 #### write\_tags\_transient\_insert
 
 ```python
 @_no_row_limit_decorator
 def write_tags_transient_insert(df: pd.DataFrame,
-                                skip_errors: bool = True) -> list[dict]
+                                skip_errors: bool = True) -> typing.List[dict]
 ```
 
 Update transient data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
@@ -1036,15 +1048,15 @@
 - `value` - value to write
 
 <a id="iotcoreapi.IoTCoreAPI.operate_tag_single"></a>
 
 #### operate\_tag\_single
 
 ```python
-def operate_tag_single(tag_uid: str, value: int | float)
+def operate_tag_single(tag_uid: str, value: typing.Union[int, float])
 ```
 
 If the token has access to operate against a Conector associated with a PLC, this method can be used to write values to the actual Plc's tags.
 
 **Arguments**:
 
 - `tag_uid` - nombre de la variable a escribir en el PLC
```


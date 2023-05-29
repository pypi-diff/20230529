# Comparing `tmp/iotcore_api-1.1.1.tar.gz` & `tmp/iotcore_api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iotcore_api-1.1.1.tar", max compression
+gzip compressed data, was "iotcore_api-1.1.2.tar", max compression
```

## Comparing `iotcore_api-1.1.1.tar` & `iotcore_api-1.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.1/iotcoreapi/__init__.py
--rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.1/iotcoreapi/exceptions.py
--rw-r--r--   0        0        0    56470 2023-05-29 09:35:28.774184 iotcore_api-1.1.1/iotcoreapi/iotcoreapi.py
--rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.1/iotcoreapi/nan_treatment.py
--rw-r--r--   0        0        0      678 2023-05-29 09:47:13.685795 iotcore_api-1.1.1/pyproject.toml
--rw-r--r--   0        0        0    34478 2023-05-29 09:40:36.225358 iotcore_api-1.1.1/README.md
--rw-r--r--   0        0        0    33951 1970-01-01 00:00:00.000000 iotcore_api-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0      483 2023-03-15 03:19:14.000000 iotcore_api-1.1.2/iotcoreapi/__init__.py
+-rw-r--r--   0        0        0      963 2023-03-13 08:36:48.000000 iotcore_api-1.1.2/iotcoreapi/exceptions.py
+-rw-r--r--   0        0        0    56483 2023-05-29 14:54:04.396063 iotcore_api-1.1.2/iotcoreapi/iotcoreapi.py
+-rw-r--r--   0        0        0     1734 2023-05-16 07:36:12.815682 iotcore_api-1.1.2/iotcoreapi/nan_treatment.py
+-rw-r--r--   0        0        0      678 2023-05-29 14:46:52.907219 iotcore_api-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0    34546 2023-05-29 14:44:23.253425 iotcore_api-1.1.2/README.md
+-rw-r--r--   0        0        0    34019 1970-01-01 00:00:00.000000 iotcore_api-1.1.2/PKG-INFO
```

### Comparing `iotcore_api-1.1.1/iotcoreapi/exceptions.py` & `iotcore_api-1.1.2/iotcoreapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.1/iotcoreapi/iotcoreapi.py` & `iotcore_api-1.1.2/iotcoreapi/iotcoreapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -287,16 +287,16 @@
         return response
 
     def catalogue_alarms(self, group_uid: str = None, output_format: str = 'dataframe') -> typing.Union[
         typing.List[dict], pd.DataFrame]:
         """Returns information of the alarms in the token
 
         Args:
-            group_uid : Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            group_uid: Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 
         Returns:
             response in json or dataframe
             """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
@@ -307,15 +307,15 @@
         response = self._getResponse(url_completa, params)
         return self._convert_response(response, output_format)
 
     def catalogue_alarm_groups(self, output_format: str = 'dataframe') -> typing.Union[typing.List[dict], pd.DataFrame]:
         """Returns information of the alarm groups in the token
 
         Args:
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
 
         Returns:
             response in json
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
             raise ValueError(f'output_format must be in {self._output_formats}')
@@ -324,21 +324,21 @@
         url_completa = self.url_NX + "/api/Alarms/Groups"
         response = self._getResponse(url_completa)
         return self._convert_response(response, output_format)
 
     # -------- READING OPERATIONS --------
 
     def read_tags_realtime(self, tags_uids: typing.List[str], output_format: str = 'dataframe',
-                           time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                           time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """Reads real time value of the tags provided in the array tags_uids
 
         Args:
-            tags_uids : list with uids of the tags
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            tags_uids: list with uids of the tags
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -349,22 +349,22 @@
         url = self.url_NX + "/api/Tags/realtime"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tagview_realtime(self, uid: str, uids_tags: typing.List[str] = None,
                               output_format: str = 'dataframe',
-                              time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                              time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """Returns real time value for the uids variables provided in a given tagview
 
         Args:
-            uid : uid of the tagview
-            uids_tags : list of uids
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            uid: uid of the tagview
+            uids_tags: list of uids
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -378,26 +378,26 @@
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tags_historic(self, uids: typing.List[str], start_ts: typing.Union[int, float], end_ts: typing.Union[int, float],
                            data_source: typing.Union[str, int] = 'RAW', resolution: typing.Union[str, int] = 'RES_1_HOUR',
                            agg_operation: typing.Union[str, int] = "LAST_VALUE", output_format: str = 'dataframe',
-                           time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                           time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """Obtain historic data of the specified tags
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
             start_ts: start time in unix time or datetime
             end_ts: end time in unix time or datetime
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
             agg_operation: MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -418,23 +418,23 @@
              "aggOperation": agg_operation})
         url = self.url_NX + "/api/Tags/historic"
         response = self._postResponse(url, body)
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tags_rawhistoric(self, uids, start_ts, end_ts, output_format: str = 'dataframe',
-                              time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                              time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """To obtain raw data with no aggregation or normalization applied
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained.
             start_ts: start time in unix time or datetime
             end_ts: end time in unix time or datetime
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -454,29 +454,29 @@
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tags_transient(self, uids: typing.List[str], start_ts: typing.Union[int, float], end_ts: typing.Union[int, float],
                             data_source: typing.Union[str, int] = None,
                             resolution: typing.Union[str, int] = 'RES_1_SEC',
                             output_format: str = 'dataframe',
-                            time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                            time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """
         This method works like "Tags in historical mode", but forces the dataSource to be the transient space. Be
         aware that the maximum period (endTs - startTs) than can be asked for in transient mode is 15 min. Also
         please note that resolutions should be according to the span of time (max 15 mins) so there are new options not available
         for historic.
 
         Args:
             uids: list of unique identifiers of the tags whose values must be obtained. start_ts:
             start_ts: time in unix time or datetime
             end_ts: end time in unix time or datetime. Timespan must be smaller than 15 mins
             data_source: Can be set to null or empty. Not needed
             resolution: RES_1_SEC, RES_200_MIL, RES_500_MIL, any other option makes no sense with the transient data pool.
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json or dataframe
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -499,26 +499,26 @@
         response = self._convert_response(response, output_format, time_format, nan_method)
         return response
 
     def read_tagview_historic(self, uid: str, start_ts: typing.Union[datetime.datetime, float, int],
                               end_ts: typing.Union[datetime.datetime, float, int], tags_uids: typing.List[str] = None,
                               data_source='RAW',
                               resolution='RES_1_HOUR', output_format: str = 'dataframe',
-                              time_format='datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
+                              time_format: str = 'datetime', nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """Read dataview historic data. It is recommended to use read_dataview_history_text_filters instead.
 
         Args:
             uid: uid of the tagview
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
             tags_uids (optional): list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            time_format: 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
             """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -552,16 +552,16 @@
         Args:
             uid_tagview: uid of the tagview
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            time_format: Optional. 'datetime' or 'unix'. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             filtered_hist (dataframe):
                 columns:
                     name: name of tag
                     value: value of tag
@@ -605,16 +605,16 @@
                                            nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """
         Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             uid_tagview: uid of the tagview
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            time_format: Optional. 'datetime' or 'unix'. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             filtered_hist (dataframe):
                 columns:
                     name: name of tag
                     value: value of tag
@@ -658,16 +658,16 @@
             uids: list of unique identifiers of the tags whose values must be obtained.
             start_ts: start time in unix or datetime
             end_ts: end time in unix or datetime
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
             data_source: RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
             resolution: RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
             agg_operation: MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            time_format: Optional. 'datetime' or 'unix'. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             response in json
         """
         # Check for valid parameters
         if output_format not in self._output_formats:
@@ -708,16 +708,16 @@
                                         time_format: str = 'datetime',
                                         nan_method: str = None) -> typing.Union[pd.DataFrame, typing.List[dict]]:
         """
         Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
 
         Args:
             filter_txt: text filters to search tags in tagviews. If None, will take all tags in tagview
-            output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-            time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+            output_format: Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+            time_format: Optional. 'datetime' or 'unix'. Defaults to datetime
             nan_method: method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
 
         Returns:
             dataframe or json:
                 columns:
                     name: name of tag
                     value: value of tag
@@ -749,15 +749,15 @@
         return filtered_hist
 
     def read_alarm_status(self, alarm_guid: str) -> dict:
         """
         Reads alarm status for a given alarm
 
         Args:
-            alarm_guid : guid of the alarm
+            alarm_guid: guid of the alarm
 
         Returns:
             Dictionary with following data:
             {
                 "name": "BasicAlarm1",
                 "uid": "b926bfb0-3f2f-49df-a2eb-138452296903",
                 "status": "ARE",
@@ -788,18 +788,18 @@
         Args:
             tags: tags name or names to be created
 
         Returns:
             response object in json format:
                 [
                    {
-                     "Uid" : "unique tag identifier",
-                     "Name" : "name of the tag",
-                     "Installation" : "name of the installation",
-                     "Driver" : "name of the driver",
+                     "Uid": "unique tag identifier",
+                     "Name": "name of the tag",
+                     "Installation": "name of the installation",
+                     "Driver": "name of the driver",
                      "Attributes": [
                        {
                          "AttributeName":"name of the attribute",
                          "Value":"value of the attribute for this tag"
                        },
                        ...
                      ]
@@ -812,15 +812,15 @@
         if isinstance(tags, str):
             tags = [tags]
         body = json.dumps(tags)
         self._log_print(f'Tags to be created: {body}')
         url_post = self.url_NX + "/api/Tags/Insert"
         return self._postResponse(url_post, body)
 
-    def write_tag_insert_or_update(self, tagname, **attributes) -> typing.List[dict]:
+    def write_tag_insert_or_update(self, tagname: str, **attributes) -> typing.List[dict]:
         """This method updates a tag with the complete model that may include attributes or modifies the existing tags changing their attributes to the ones indicated in the query.
 
         Args:
             tagname: name of the new tag
             **attributes: dictionary of attributes and their values
 
         Returns:
@@ -869,15 +869,15 @@
     def write_tags_historic_insert(self, df: pd.DataFrame, skip_errors: bool = True) -> typing.List[dict]:
         """Update historical data for tags. Tags need to be created with write_tags_insert first.
 
         Args:
             df: dataframe
                 columns:
                     name: name of the tag
-                    value : value of the tag
+                    value: value of the tag
                     timeStamp: timeStamp in unix
             skip_errors: True: If true, not created tags will be dropped from dataframe
 
         Returns:
             response in json format
         """
         # la funcion mira cuantas variables diferentes contiene el dataframe y comprueba si todas ellas existen
@@ -915,15 +915,15 @@
     def write_tags_realtime_insert(self, df: pd.DataFrame, skip_errors: bool = True):
         """Update realtime data for tags. Tags need to be created with write_tags_insert first.
 
         Args:
             df: dataframe
                 columns:
                     name: name of the tag
-                    value : value of the tag
+                    value: value of the tag
                     timeStamp (optional): timeStamp in unix. If not provided, will take current time
             skip_errors: True: If true, not created tags will be dropped from dataframe
 
         Returns:
             response text (None if OK)
         """
         vbles = list(df.name.unique())
@@ -1007,15 +1007,15 @@
     def write_tags_transient_insert(self, df: pd.DataFrame, skip_errors: bool = True) -> typing.List[dict]:
         """Update transient data for tags. Tags need to be created with write_tags_insert first.
 
         Args:
             df: dataframe
                 columns:
                     name: name of the tag
-                    value : value of the tag
+                    value: value of the tag
                     timeStamp: timeStamp in unix
             skip_errors  = True: If true, not created tags will be dropped from dataframe
 
         Returns:
             response in json format
         """
         # la funcion mira cuantas variables diferentes contiene el dataframe y comprueba si todas ellas existen
```

### Comparing `iotcore_api-1.1.1/iotcoreapi/nan_treatment.py` & `iotcore_api-1.1.2/iotcoreapi/nan_treatment.py`

 * *Files identical despite different names*

### Comparing `iotcore_api-1.1.1/pyproject.toml` & `iotcore_api-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iotcore-api"
-version = "1.1.1"
+version = "1.1.2"
 authors = ["Idrica"]
 description ="IoT core connection methods and utilities"
 readme = "README.md"
 packages = [
     {include = 'iotcoreapi/*.py'}
 ]
```

### Comparing `iotcore_api-1.1.1/README.md` & `iotcore_api-1.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -383,16 +383,16 @@
 ) -> typing.Union[typing.List[dict], pd.DataFrame]
 ```
 
 Returns information of the alarms in the token
 
 **Arguments**:
 
-  group_uid : Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `group_uid` - Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
   
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarm_groups"></a>
@@ -405,15 +405,15 @@
 ) -> typing.Union[typing.List[dict], pd.DataFrame]
 ```
 
 Returns information of the alarm groups in the token
 
 **Arguments**:
 
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
   
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime"></a>
@@ -429,17 +429,17 @@
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Reads real time value of the tags provided in the array tags_uids
 
 **Arguments**:
 
-  tags_uids : list with uids of the tags
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `tags_uids` - list with uids of the tags
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json or dataframe
 
@@ -457,18 +457,18 @@
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Returns real time value for the uids variables provided in a given tagview
 
 **Arguments**:
 
-  uid : uid of the tagview
-  uids_tags : list of uids
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `uid` - uid of the tagview
+- `uids_tags` - list of uids
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json or dataframe
 
@@ -496,16 +496,16 @@
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix time or datetime
 - `end_ts` - end time in unix time or datetime
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json or dataframe
 
@@ -527,16 +527,16 @@
 To obtain raw data with no aggregation or normalization applied
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix time or datetime
 - `end_ts` - end time in unix time or datetime
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json or dataframe
 
@@ -565,16 +565,16 @@
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained. start_ts:
 - `start_ts` - time in unix time or datetime
 - `end_ts` - end time in unix time or datetime. Timespan must be smaller than 15 mins
 - `data_source` - Can be set to null or empty. Not needed
 - `resolution` - RES_1_SEC, RES_200_MIL, RES_500_MIL, any other option makes no sense with the transient data pool.
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json or dataframe
 
@@ -602,16 +602,16 @@
 
 - `uid` - uid of the tagview
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
 - `tags_uids` _optional_ - list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
 
@@ -630,16 +630,16 @@
 
 - `uid_tagview` - uid of the tagview
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   filtered_hist (dataframe):
   columns:
@@ -663,16 +663,16 @@
 
 Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `uid_tagview` - uid of the tagview
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   filtered_hist (dataframe):
   columns:
@@ -706,16 +706,16 @@
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json
 
@@ -733,16 +733,16 @@
 ```
 
 Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   dataframe or json:
   columns:
@@ -758,15 +758,15 @@
 def read_alarm_status(alarm_guid: str) -> dict
 ```
 
 Reads alarm status for a given alarm
 
 **Arguments**:
 
-  alarm_guid : guid of the alarm
+- `alarm_guid` - guid of the alarm
   
 
 **Returns**:
 
   Dictionary with following data:
   {
 - `"name"` - "BasicAlarm1",
@@ -802,18 +802,18 @@
   
 
 **Returns**:
 
   response object in json format:
   [
   {
-  "Uid" : "unique tag identifier",
-  "Name" : "name of the tag",
-  "Installation" : "name of the installation",
-  "Driver" : "name of the driver",
+- `"Uid"` - "unique tag identifier",
+- `"Name"` - "name of the tag",
+- `"Installation"` - "name of the installation",
+- `"Driver"` - "name of the driver",
 - `"Attributes"` - [
   {
   "AttributeName":"name of the attribute",
   "Value":"value of the attribute for this tag"
   },
   ...
   ]
@@ -893,15 +893,15 @@
 Update historical data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
-  value : value of the tag
+- `value` - value of the tag
 - `timeStamp` - timeStamp in unix
 - `skip_errors` - True: If true, not created tags will be dropped from dataframe
   
 
 **Returns**:
 
   response in json format
@@ -918,15 +918,15 @@
 Update realtime data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
-  value : value of the tag
+- `value` - value of the tag
 - `timeStamp` _optional_ - timeStamp in unix. If not provided, will take current time
 - `skip_errors` - True: If true, not created tags will be dropped from dataframe
   
 
 **Returns**:
 
   response text (None if OK)
@@ -967,15 +967,15 @@
 Update transient data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
-  value : value of the tag
+- `value` - value of the tag
 - `timeStamp` - timeStamp in unix
   skip_errors  = True: If true, not created tags will be dropped from dataframe
   
 
 **Returns**:
 
   response in json format
```

### Comparing `iotcore_api-1.1.1/PKG-INFO` & `iotcore_api-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iotcore-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: IoT core connection methods and utilities
 Author: Idrica
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -398,16 +398,16 @@
 ) -> typing.Union[typing.List[dict], pd.DataFrame]
 ```
 
 Returns information of the alarms in the token
 
 **Arguments**:
 
-  group_uid : Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `group_uid` - Optional. Uid of the group to list. If the group uid is indicated, the list only contains the alarms that belong directly to the group (no digging down in the hierarchy)
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
   
 
 **Returns**:
 
   response in json or dataframe
 
 <a id="iotcoreapi.IoTCoreAPI.catalogue_alarm_groups"></a>
@@ -420,15 +420,15 @@
 ) -> typing.Union[typing.List[dict], pd.DataFrame]
 ```
 
 Returns information of the alarm groups in the token
 
 **Arguments**:
 
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
   
 
 **Returns**:
 
   response in json
 
 <a id="iotcoreapi.IoTCoreAPI.read_tags_realtime"></a>
@@ -444,17 +444,17 @@
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Reads real time value of the tags provided in the array tags_uids
 
 **Arguments**:
 
-  tags_uids : list with uids of the tags
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `tags_uids` - list with uids of the tags
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json or dataframe
 
@@ -472,18 +472,18 @@
 ) -> typing.Union[pd.DataFrame, typing.List[dict]]
 ```
 
 Returns real time value for the uids variables provided in a given tagview
 
 **Arguments**:
 
-  uid : uid of the tagview
-  uids_tags : list of uids
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `uid` - uid of the tagview
+- `uids_tags` - list of uids
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json or dataframe
 
@@ -511,16 +511,16 @@
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix time or datetime
 - `end_ts` - end time in unix time or datetime
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json or dataframe
 
@@ -542,16 +542,16 @@
 To obtain raw data with no aggregation or normalization applied
 
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix time or datetime
 - `end_ts` - end time in unix time or datetime
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json or dataframe
 
@@ -580,16 +580,16 @@
 **Arguments**:
 
 - `uids` - list of unique identifiers of the tags whose values must be obtained. start_ts:
 - `start_ts` - time in unix time or datetime
 - `end_ts` - end time in unix time or datetime. Timespan must be smaller than 15 mins
 - `data_source` - Can be set to null or empty. Not needed
 - `resolution` - RES_1_SEC, RES_200_MIL, RES_500_MIL, any other option makes no sense with the transient data pool.
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json or dataframe
 
@@ -617,16 +617,16 @@
 
 - `uid` - uid of the tagview
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
 - `tags_uids` _optional_ - list of unique identifier of the tags whose values must be obtained. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - 'datetime' or 'unix' if output_format is dataframe. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   A list of objects or dataframe providing information for the requested tags. Every element in the array corresponds to one of the requested tags associated with one timestamp between the startTs and the endTs.
 
@@ -645,16 +645,16 @@
 
 - `uid_tagview` - uid of the tagview
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   filtered_hist (dataframe):
   columns:
@@ -678,16 +678,16 @@
 
 Read dataview realtime data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `uid_tagview` - uid of the tagview
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   filtered_hist (dataframe):
   columns:
@@ -721,16 +721,16 @@
 - `uids` - list of unique identifiers of the tags whose values must be obtained.
 - `start_ts` - start time in unix or datetime
 - `end_ts` - end time in unix or datetime
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
 - `data_source` - RAW, STATS_PER_HOUR, STATS_PER_DAY o STATS_PER_MONTH. This parameter indicates the historian section to get the information from, being "RAW" the finest data storage available.
 - `resolution` - RES_10_SEC, RES_30_SEC, RES_1_MIN, RES_5_MIN, RES_15_MIN, RES_1_HOUR, RES_1_DAY, RES_1_MONTH o RES_1_YEAR, this parameter only applies if the datasource is RAW.
 - `agg_operation` - MIN, MAX, AVG, LAST_VALUE, SUM. The operation to be applied to obtain the resolution required. Not mandatory, can be null or empty, then applies LAST_VALUE by default.
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   response in json
 
@@ -748,16 +748,16 @@
 ```
 
 Read tags realtime data but use text filters instead of uids. Also returns data in dataframe format
 
 **Arguments**:
 
 - `filter_txt` - text filters to search tags in tagviews. If None, will take all tags in tagview
-  output_format : Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
-  time_format : Optional. 'datetime' or 'unix'. Defaults to datetime
+- `output_format` - Result given in 'dataframe' or 'json'. Defaults to 'dataframe'
+- `time_format` - Optional. 'datetime' or 'unix'. Defaults to datetime
 - `nan_method` - method used to drop NaNs. None or 'interpolate', 'bfill', 'ffill', 'mean', 'zerofill'. Only valid for 'dataframe' output_format
   
 
 **Returns**:
 
   dataframe or json:
   columns:
@@ -773,15 +773,15 @@
 def read_alarm_status(alarm_guid: str) -> dict
 ```
 
 Reads alarm status for a given alarm
 
 **Arguments**:
 
-  alarm_guid : guid of the alarm
+- `alarm_guid` - guid of the alarm
   
 
 **Returns**:
 
   Dictionary with following data:
   {
 - `"name"` - "BasicAlarm1",
@@ -817,18 +817,18 @@
   
 
 **Returns**:
 
   response object in json format:
   [
   {
-  "Uid" : "unique tag identifier",
-  "Name" : "name of the tag",
-  "Installation" : "name of the installation",
-  "Driver" : "name of the driver",
+- `"Uid"` - "unique tag identifier",
+- `"Name"` - "name of the tag",
+- `"Installation"` - "name of the installation",
+- `"Driver"` - "name of the driver",
 - `"Attributes"` - [
   {
   "AttributeName":"name of the attribute",
   "Value":"value of the attribute for this tag"
   },
   ...
   ]
@@ -908,15 +908,15 @@
 Update historical data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
-  value : value of the tag
+- `value` - value of the tag
 - `timeStamp` - timeStamp in unix
 - `skip_errors` - True: If true, not created tags will be dropped from dataframe
   
 
 **Returns**:
 
   response in json format
@@ -933,15 +933,15 @@
 Update realtime data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
-  value : value of the tag
+- `value` - value of the tag
 - `timeStamp` _optional_ - timeStamp in unix. If not provided, will take current time
 - `skip_errors` - True: If true, not created tags will be dropped from dataframe
   
 
 **Returns**:
 
   response text (None if OK)
@@ -982,15 +982,15 @@
 Update transient data for tags. Tags need to be created with write_tags_insert first.
 
 **Arguments**:
 
 - `df` - dataframe
   columns:
 - `name` - name of the tag
-  value : value of the tag
+- `value` - value of the tag
 - `timeStamp` - timeStamp in unix
   skip_errors  = True: If true, not created tags will be dropped from dataframe
   
 
 **Returns**:
 
   response in json format
```


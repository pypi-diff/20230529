# Comparing `tmp/python_omnilogic_local-0.4.1.tar.gz` & `tmp/python_omnilogic_local-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_omnilogic_local-0.4.1.tar", max compression
+gzip compressed data, was "python_omnilogic_local-0.4.2.tar", max compression
```

## Comparing `python_omnilogic_local-0.4.1.tar` & `python_omnilogic_local-0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1696 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/__init__.py
--rwxr-xr-x   0        0        0    20177 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/api.py
--rwxr-xr-x   0        0        0     3931 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/cli.py
--rw-r--r--   0        0        0        0 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/__init__.py
--rw-r--r--   0        0        0       51 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/const.py
--rw-r--r--   0        0        0     1532 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/filter_diagnostics.py
--rw-r--r--   0        0        0      407 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/leadmessage.py
--rw-r--r--   0        0        0     7864 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/mspconfig.py
--rw-r--r--   0        0        0     9619 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/telemetry.py
--rw-r--r--   0        0        0     1476 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/models/util.py
--rw-r--r--   0        0        0     9040 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/protocol.py
--rw-r--r--   0        0        0     6304 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/types.py
--rw-r--r--   0        0        0      359 2023-05-28 14:15:07.953240 python_omnilogic_local-0.4.1/pyomnilogic_local/util.py
--rw-r--r--   0        0        0     5227 2023-05-28 14:15:08.841250 python_omnilogic_local-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1696 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/__init__.py
+-rwxr-xr-x   0        0        0    21535 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/api.py
+-rwxr-xr-x   0        0        0     3921 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/cli.py
+-rw-r--r--   0        0        0        0 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/__init__.py
+-rw-r--r--   0        0        0       51 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/const.py
+-rw-r--r--   0        0        0     1532 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/filter_diagnostics.py
+-rw-r--r--   0        0        0      407 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/leadmessage.py
+-rw-r--r--   0        0        0     7871 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/mspconfig.py
+-rw-r--r--   0        0        0     9619 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/telemetry.py
+-rw-r--r--   0        0        0     1476 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/models/util.py
+-rw-r--r--   0        0        0     9040 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/protocol.py
+-rw-r--r--   0        0        0     6304 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/types.py
+-rw-r--r--   0        0        0      359 2023-05-29 20:55:47.922797 python_omnilogic_local-0.4.2/pyomnilogic_local/util.py
+-rw-r--r--   0        0        0     5227 2023-05-29 20:55:49.086857 python_omnilogic_local-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0     2727 1970-01-01 00:00:00.000000 python_omnilogic_local-0.4.2/PKG-INFO
```

### Comparing `python_omnilogic_local-0.4.1/README.md` & `python_omnilogic_local-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.1/pyomnilogic_local/api.py` & `python_omnilogic_local-0.4.2/pyomnilogic_local/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,24 @@
         ...
 
     @overload
     async def async_send_message(self, message_type: MessageType, message: str | None, need_response: Literal[False]) -> None:
         ...
 
     async def async_send_message(self, message_type: MessageType, message: str | None, need_response: bool = False) -> str | None:
+        """Send a message via the Hayward Omni UDP protocol along with properly handling timeouts and responses.
+
+        Args:
+            message_type (MessageType): A selection from MessageType indicating what type of communication you are sending
+            message (str | None): The XML body of the message to deliver
+            need_response (bool, optional): Should a response be received and returned to the caller. Defaults to False.
+
+        Returns:
+            str | None: The response body sent from the Omni if need_response indicates that a response will be sent
+        """
         loop = asyncio.get_running_loop()
         transport, protocol = await loop.create_datagram_endpoint(OmniLogicProtocol, remote_addr=(self.controller_ip, self.controller_port))
 
         resp: str | None = None
         try:
             if need_response:
                 resp = await asyncio.wait_for(protocol.send_and_receive(message_type, message), self.response_timeout)
@@ -49,44 +59,57 @@
                 await asyncio.wait_for(protocol.send_message(message_type, message), self.response_timeout)
         finally:
             transport.close()
 
         return resp
 
     async def async_get_alarm_list(self) -> str:
+        """Retrieve a list of alarms from the Omni.
+
+        Returns:
+            str: An XML body indicating any alarms that are present
+        """
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
 
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "GetAllAlarmList"
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.GET_ALARM_LIST, req_body, True)
 
     @to_pydantic(pydantic_type=MSPConfig)
     async def async_get_config(self) -> str:
+        """Retrieve the MSPConfig from the Omni, optionally parse it into a pydantic model.
+
+        Args:
+            raw (bool): Do not parse the response into a Pydantic model, just return the raw XML. Defaults to False.
+
+        Returns:
+            MSPConfig|str: Either a parsed .models.mspconfig.MSPConfig object or a str depending on arg raw
+        """
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
 
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "RequestConfiguration"
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.REQUEST_CONFIGURATION, req_body, True)
 
     @to_pydantic(pydantic_type=FilterDiagnostics)
     async def async_get_filter_diagnostics(self, pool_id: int, equipment_id: int) -> str:
-        """async_get_filter_diagnostics handles sending a GetUIFilterDiagnosticInfo XML API call to the Hayward Omni pool controller
+        """Retrieve filter diagnostics from the Omni, optionally parse it into a pydantic model.
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
 
         Returns:
-            _type_: _description_
+            FilterDiagnostics|str: Either a parsed .models.mspconfig.FilterDiagnostics object or a str depending on arg raw
         """
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
 
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "GetUIFilterDiagnosticInfo"
 
         parameters_element = ET.SubElement(body_element, "Parameters")
@@ -96,38 +119,48 @@
         parameter.text = str(equipment_id)
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.GET_FILTER_DIAGNOSTIC_INFO, req_body, True)
 
     async def async_get_log_config(self) -> str:
+        """Retrieve the logging configuration from the Omni.
+
+        Returns:
+            str: An XML body describing the logging configuration
+        """
         return await self.async_send_message(MessageType.REQUEST_LOG_CONFIG, None, True)
 
     @to_pydantic(pydantic_type=Telemetry)
     async def async_get_telemetry(self) -> str:
+        """Retrieve the current telemetry data from the Omni, optionally parse it into a pydantic model.
+
+        Returns:
+            Telemetry|str: Either a parsed .models.telemetry.Telemetry object or a str depending on arg raw
+        """
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
 
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "RequestTelemetryData"
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.GET_TELEMETRY, req_body, True)
 
     async def async_set_heater(self, pool_id: int, equipment_id: int, temperature: int, unit: str) -> None:
-        """async_set_heater handles sending a SetUIHeaterCmd XML API call to the Hayward Omni pool controller
+        """Set the temperature for a heater on the Omni
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
             temperature (int): What temperature to request
             unit (str): The temperature unit to use (either F or C)
 
         Returns:
-            _type_: _description_
+            None
         """
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
 
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "SetUIHeaterCmd"
 
         parameters_element = ET.SubElement(body_element, "Parameters")
@@ -139,24 +172,24 @@
         parameter.text = str(temperature)
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.SET_HEATER_COMMAND, req_body, False)
 
     async def async_set_solar_heater(self, pool_id: int, equipment_id: int, temperature: int, unit: str) -> None:
-        """async_set_heater handles sending a SetUIHeaterCmd XML API call to the Hayward Omni pool controller
+        """Set the solar set point for a heater on the Omni.
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
             temperature (int): What temperature to request
             unit (str): The temperature unit to use (either F or C)
 
         Returns:
-            _type_: _description_
+            None
         """
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
 
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "SetUISolarSetPointCmd"
 
         parameters_element = ET.SubElement(body_element, "Parameters")
@@ -168,23 +201,23 @@
         parameter.text = str(temperature)
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.SET_SOLAR_SET_POINT_COMMAND, req_body, False)
 
     async def async_set_heater_mode(self, pool_id: int, equipment_id: int, mode: HeaterMode) -> None:
-        """async_set_heater_enable handles sending a SetHeaterEnable XML API call to the Hayward Omni pool controller
+        """Set what mode (Heat/Cool/Auto) the heater should use.
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
-            enabled (bool, optional): Turn the heater on (True) or off (False)
+            mode (HeaterMode): What mode should the heater operate under
 
         Returns:
-            _type_: _description_
+            None
         """
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
 
         name_element = ET.SubElement(body_element, "Name")
         name_element.text = "SetUIHeaterModeCmd"
 
         parameters_element = ET.SubElement(body_element, "Parameters")
@@ -236,21 +269,22 @@
         start_time_hours: int = 0,
         start_time_minutes: int = 0,
         end_time_hours: int = 0,
         end_time_minutes: int = 0,
         days_active: int = 0,
         recurring: bool = False,
     ) -> None:
-        """async_set_equipment handles sending a SetUIEquipmentCmd XML API call to the Hayward Omni pool controller
+        """Control a piece of equipment, turning it on/off or setting a value (E.g.: filter speed), optionally scheduling it.
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
             is_on (Union[int,bool]): For most equipment items, True/False to turn on/off.
                 For Variable Speed Pumps, you can optionally provide an int from 0-100 to set the speed percentage with 0 being Off.
+                The interpretation of value depends on the piece of equipment being targeted.
             is_countdown_timer (bool, optional): For potential future use, included to be "API complete". Defaults to False.
             startTimeHours (int, optional): For potential future use, included to be "API complete". Defaults to 0.
             startTimeMinutes (int, optional): For potential future use, included to be "API complete". Defaults to 0.
             endTimeHours (int, optional): For potential future use, included to be "API complete". Defaults to 0.
             endTimeMinutes (int, optional): For potential future use, included to be "API complete". Defaults to 0.
             daysActive (int, optional): For potential future use, included to be "API complete". Defaults to 0.
             recurring (bool, optional): For potential future use, included to be "API complete". Defaults to False.
@@ -261,15 +295,15 @@
         name_element.text = "SetUIEquipmentCmd"
 
         parameters_element = ET.SubElement(body_element, "Parameters")
         parameter = ET.SubElement(parameters_element, "Parameter", name="poolId", dataType="int")
         parameter.text = str(pool_id)
         parameter = ET.SubElement(parameters_element, "Parameter", name="equipmentId", dataType="int")
         parameter.text = str(equipment_id)
-        parameter = ET.SubElement(parameters_element, "Parameter", name="isOn", dataType="int")
+        parameter = ET.SubElement(parameters_element, "Parameter", name="isOn", dataType="int", alias="Data")
         parameter.text = str(int(is_on))
         parameter = ET.SubElement(parameters_element, "Parameter", name="IsCountDownTimer", dataType="bool")
         parameter.text = str(int(is_countdown_timer))
         parameter = ET.SubElement(parameters_element, "Parameter", name="StartTimeHours", dataType="int")
         parameter.text = str(start_time_hours)
         parameter = ET.SubElement(parameters_element, "Parameter", name="StartTimeMinutes", dataType="int")
         parameter.text = str(start_time_minutes)
@@ -283,15 +317,15 @@
         parameter.text = str(int(recurring))
 
         req_body = ET.tostring(body_element, xml_declaration=True, encoding="unicode")
 
         return await self.async_send_message(MessageType.SET_EQUIPMENT, req_body, False)
 
     async def async_set_filter_speed(self, pool_id: int, equipment_id: int, speed: int) -> None:
-        """async_set_filter_speed handles sending a SetUIFilterSpeedCmd XML API call to the Hayward Omni pool controller
+        """Set the speed for a variable speed filter/pump.
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
             speed (int): Speed value from 0-100 to set the filter to.  A value of 0 will turn the filter off.
         """
         body_element = ET.Element("Request", {"xmlns": "http://nextgen.hayward.com/api"})
@@ -324,15 +358,15 @@
         start_time_hours: int = 0,
         start_time_minutes: int = 0,
         end_time_hours: int = 0,
         end_time_minutes: int = 0,
         days_active: int = 0,
         recurring: bool = False,
     ) -> None:
-        """async_set_light_show handles sending a SetStandAloneLightShow XML API call to the Hayward Omni pool controller
+        """Set the desired light show/speed/brightness for a ColorLogic light.
 
         Args:
             pool_id (int): The Pool/BodyOfWater ID that you want to address
             equipment_id (int): Which equipment_id within that Pool to address
             show (ColorLogicShow): ColorLogicShow to set the light to
             speed (ColorLogicSpeed, optional): Speed to animate the show. Defaults to 4.  0-8 which map to:
             brightness (ColorLogicBrightness, optional): How bright should the light be. Defaults to 4. 0-4 which map to:
```

### Comparing `python_omnilogic_local-0.4.1/pyomnilogic_local/cli.py` & `python_omnilogic_local-0.4.2/pyomnilogic_local/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,22 +45,22 @@
     diags = await omni.async_get_filter_diagnostics(POOL_ID, PUMP_EQUIPMENT_ID)
     print(diags)
     # Decode the filter display revision
     # b1=chr(diags.get_param_by_name("DisplayFWRevisionB1"))
     # b2=chr(diags.get_param_by_name("DisplayFWRevisionB2"))
     # b3=chr(diags.get_param_by_name("DisplayFWRevisionB3"))
     # b4=chr(diags.get_param_by_name("DisplayFWRevisionB4"))
-    # # b5 and b6 are whitespace and a null terminator
-    # # b5=chr(diags.get_param_by_name("DisplayFWRevisionB5"))
-    # # b6=chr(diags.get_param_by_name("DisplayFWRevisionB6"))
+    # b5 and b6 are whitespace and a null terminator
+    # b5=chr(diags.get_param_by_name("DisplayFWRevisionB5"))
+    # b6=chr(diags.get_param_by_name("DisplayFWRevisionB6"))
     # print(f"{b1}{b2}.{b3}.{b4}")
-    # # Decode the filter power consumption (don't do this, it's returned already decoded in the telemetry)
+    # Decode the filter power consumption (don't do this, it's returned already decoded in the telemetry)
     # p1=diags.get_param_by_name("PowerMSB")
     # p2=diags.get_param_by_name("PowerLSB")
-    # # The f-string below converts the bytes to hex and displays them.  Just get this value from the telemetry, it's easier
+    # The f-string below converts the bytes to hex and displays them.  Just get this value from the telemetry, it's easier
     # print(f"{p1:x}{p2:x}")
 
     # Fetch logging configuration
     # print(await omni.async_get_log_config())
 
     # Adjust the heater temperature
     # await omni.async_set_heater(POOL_ID, HEATER_EQUIPMENT_ID, 85, "F")
```

### Comparing `python_omnilogic_local-0.4.1/pyomnilogic_local/models/filter_diagnostics.py` & `python_omnilogic_local-0.4.2/pyomnilogic_local/models/filter_diagnostics.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.1/pyomnilogic_local/models/mspconfig.py` & `python_omnilogic_local-0.4.2/pyomnilogic_local/models/mspconfig.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         heater_equip_data = [op for op in data.get("Operation", {}) if OmniType.HEATER_EQUIP in op][0]
         self.heater_equipment = [MSPHeaterEquip.parse_obj(equip) for equip in heater_equip_data[OmniType.HEATER_EQUIP]]
 
 
 class MSPColorLogicLight(OmniBase):
     omni_type: OmniType = OmniType.CL_LIGHT
     type: ColorLogicLightType | str = Field(alias="Type")
-    v2_active: Literal["yes", "no"] = Field(alias="V2-Active")
+    v2_active: Literal["yes", "no"] | None = Field(alias="V2-Active")
 
 
 class MSPBoW(OmniBase):
     _sub_devices = {"filter", "relay", "heater", "sensor", "colorlogic_light"}
 
     omni_type: OmniType = OmniType.BOW
     type: BodyOfWaterType | str = Field(alias="Type")
```

### Comparing `python_omnilogic_local-0.4.1/pyomnilogic_local/models/telemetry.py` & `python_omnilogic_local-0.4.2/pyomnilogic_local/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.1/pyomnilogic_local/models/util.py` & `python_omnilogic_local-0.4.2/pyomnilogic_local/models/util.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.1/pyomnilogic_local/protocol.py` & `python_omnilogic_local-0.4.2/pyomnilogic_local/protocol.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.1/pyomnilogic_local/types.py` & `python_omnilogic_local-0.4.2/pyomnilogic_local/types.py`

 * *Files identical despite different names*

### Comparing `python_omnilogic_local-0.4.1/pyproject.toml` & `python_omnilogic_local-0.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-omnilogic-local"
-version = "0.4.1"
+version = "0.4.2"
 description = "A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API"
 authors = ["cryptk <cryptk@users.noreply.github.com>", "djtimca", "garionphx"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/cryptk/python-omnilogic-local"
 classifiers = [
     "Development Status :: 3 - Alpha",
```

### Comparing `python_omnilogic_local-0.4.1/PKG-INFO` & `python_omnilogic_local-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-omnilogic-local
-Version: 0.4.1
+Version: 0.4.2
 Summary: A library for local control of Hayward OmniHub/OmniLogic pool controllers using their local API
 Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0
 Author: cryptk
 Author-email: cryptk@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.4.1 Summary: A
+Metadata-Version: 2.1 Name: python-omnilogic-local Version: 0.4.2 Summary: A
 library for local control of Hayward OmniHub/OmniLogic pool controllers using
 their local API Home-page: https://github.com/cryptk/python-omnilogic-local
 License: Apache-2.0 Author: cryptk Author-email:
 cryptk@users.noreply.github.com Requires-Python: >=3.10,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Natural Language :: English Classifier: Operating System :: OS Independent
```


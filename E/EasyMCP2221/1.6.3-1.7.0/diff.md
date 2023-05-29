# Comparing `tmp/EasyMCP2221-1.6.3.tar.gz` & `tmp/easymcp2221-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EasyMCP2221-1.6.3.tar", last modified: Fri Mar  3 21:05:16 2023, max compression
+gzip compressed data, was "easymcp2221-1.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `EasyMCP2221-1.6.3.tar` & `easymcp2221-1.7.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     7312 2023-03-03 21:05:08.841355 EasyMCP2221-1.6.3/EasyMCP2221/Constants.py
--rw-r--r--   0        0        0     6681 2023-03-03 21:05:08.841355 EasyMCP2221-1.6.3/EasyMCP2221/I2C_Slave.py
--rw-r--r--   0        0        0    69495 2023-03-03 21:05:08.845355 EasyMCP2221-1.6.3/EasyMCP2221/MCP2221.py
--rw-r--r--   0        0        0     1482 2023-03-03 21:05:08.845355 EasyMCP2221-1.6.3/EasyMCP2221/__init__.py
--rw-r--r--   0        0        0     1867 2023-03-03 21:05:08.845355 EasyMCP2221-1.6.3/EasyMCP2221/exceptions.py
--rw-r--r--   0        0        0     9305 2023-03-03 21:05:08.845355 EasyMCP2221-1.6.3/EasyMCP2221/smbus.py
--rw-r--r--   0        0        0     1036 2023-03-03 21:05:08.845355 EasyMCP2221-1.6.3/LICENSE
--rw-r--r--   0        0        0     1698 2023-03-03 21:05:08.845355 EasyMCP2221-1.6.3/README.rst
--rw-r--r--   0        0        0      768 2023-03-03 21:05:09.125356 EasyMCP2221-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 EasyMCP2221-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     7558 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/Constants.py
+-rw-r--r--   0        0        0     6681 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/I2C_Slave.py
+-rw-r--r--   0        0        0    73577 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/MCP2221.py
+-rw-r--r--   0        0        0     1482 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/__init__.py
+-rw-r--r--   0        0        0     1867 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/exceptions.py
+-rw-r--r--   0        0        0     9305 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/EasyMCP2221/smbus.py
+-rw-r--r--   0        0        0     1036 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/LICENSE
+-rw-r--r--   0        0        0     1698 2023-05-29 14:53:58.897451 easymcp2221-1.7.0/README.rst
+-rw-r--r--   0        0        0      768 2023-05-29 14:53:59.177453 easymcp2221-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2339 1970-01-01 00:00:00.000000 easymcp2221-1.7.0/PKG-INFO
```

### Comparing `EasyMCP2221-1.6.3/EasyMCP2221/Constants.py` & `easymcp2221-1.7.0/EasyMCP2221/Constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -225,7 +225,15 @@
 I2C_POLL_RESP_TX_LEN_H        = 12
 I2C_POLL_RESP_CLKDIV          = 14
 I2C_POLL_RESP_UNDOCUMENTED_18 = 18
 I2C_POLL_RESP_ACK             = 20
 I2C_POLL_RESP_UNDOCUMENTED_21 = 21
 I2C_POLL_RESP_SCL             = 22
 I2C_POLL_RESP_SDA             = 23
+I2C_POLL_RESP_INT_FLAG        = 24
+
+I2C_POLL_RESP_ADC_CH0_LSB     = 50
+I2C_POLL_RESP_ADC_CH0_MSB     = 51
+I2C_POLL_RESP_ADC_CH1_LSB     = 52
+I2C_POLL_RESP_ADC_CH1_MSB     = 53
+I2C_POLL_RESP_ADC_CH2_LSB     = 54
+I2C_POLL_RESP_ADC_CH2_MSB     = 55
```

### Comparing `EasyMCP2221-1.6.3/EasyMCP2221/I2C_Slave.py` & `easymcp2221-1.7.0/EasyMCP2221/I2C_Slave.py`

 * *Files identical despite different names*

### Comparing `EasyMCP2221-1.6.3/EasyMCP2221/MCP2221.py` & `easymcp2221-1.7.0/EasyMCP2221/MCP2221.py`

 * *Files 7% similar despite different names*

```diff
@@ -42,14 +42,20 @@
 
     trace_packets = False
     """bool: Print all binary commands and responses."""
 
     debug_messages = False
     """bool: Print debugging messages."""
 
+    unsaved_SRAM = {}
+    """Some options, like USB power attributes, are read from Flash into SRAM at start-up
+    and cannot be changed in SRAM at run time. So we must store them somewhere to save
+    then in save_config.
+    """
+
     status = {
         # 4   -> output value
         # 3   -> direction
         # 2:0 -> designation
         "GPIO": {
             "gp0": None,
             "gp1": None,
@@ -115,34 +121,27 @@
 
         # Initialize current DAC/ADC Vref (not the same for Get SRAM and for Set SRAM)
         self.status["dac_ref"]   = (settings[6] >> 5) & 0b00000111
         self.status["dac_value"] = (settings[6])      & 0b00011111
         self.status["adc_ref"]   = (settings[7] >> 2) & 0b00000111
 
         ## After power-up, Vrm may be set-up but not working, it's like when you apply new GPIO in SRAM
-        self.SRAM_config(
-            dac_ref    = self.status["dac_ref"],
-            dac_value  = self.status["dac_value"],
-            adc_ref    = self.status["adc_ref"],
-            gp0        = self.status["GPIO"]["gp0"],
-            gp1        = self.status["GPIO"]["gp1"],
-            gp2        = self.status["GPIO"]["gp2"],
-            gp3        = self.status["GPIO"]["gp3"])
+        self._reinforce_SRAM()
 
         # Read I2C status and try to release the bus if needed.
         # (i2c lines might not be up right now)
         try:
             self._i2c_release()
         except:
             pass
 
 
     def __repr__(self):
         import json
-        data = self._read_flash_info(raw = False)
+        data = self.read_flash_info(human=True)
         return json.dumps(data, indent=4, sort_keys=True)
 
 
     def __del__(self):
         """ Releases the device. """
         self.hidhandler.close()
         del self.hidhandler
@@ -305,19 +304,23 @@
         chip[FLASH_CHIP_SETTINGS_PWD7]    = sram[SRAM_CHIP_SETTINGS_PWD7]
         chip[FLASH_CHIP_SETTINGS_PWD8]    = sram[SRAM_CHIP_SETTINGS_PWD8]
 
         if self.debug_messages:
             print("NEW CHIP:", " ".join("%02x" % i for i in chip))
             print("OLD GP:", " ".join("%02x" % i for i in gp))
 
+        # Take status instead of SRAM variables because GPIO_write command won't alter SRAM
         gp[FLASH_GP_SETTINGS_GP0]         = self.status["GPIO"]["gp0"]
         gp[FLASH_GP_SETTINGS_GP1]         = self.status["GPIO"]["gp1"]
         gp[FLASH_GP_SETTINGS_GP2]         = self.status["GPIO"]["gp2"]
         gp[FLASH_GP_SETTINGS_GP3]         = self.status["GPIO"]["gp3"]
 
+        for k in self.unsaved_SRAM:
+            chip[k] = self.unsaved_SRAM[k]
+
         if self.debug_messages:
             print("NEW GP:", " ".join("%02x" % i for i in gp))
 
         self._write_flash_raw(FLASH_DATA_CHIP_SETTINGS, chip)
         self._write_flash_raw(FLASH_DATA_GP_SETTINGS,   gp)
 
 
@@ -345,57 +348,100 @@
 
         if rbuf[RESPONSE_STATUS_BYTE] != RESPONSE_RESULT_OK:
             raise RuntimeError("Write flash data command failed.")
 
         return rbuf[0:64]
 
 
-    def _read_flash_info(self, raw = False):
+    def read_flash_info(self, raw=False, human=False):
         """ Read flash data.
 
         Return USB enumeration strings, power-up GPIO settings and internal chip configuration.
 
         Parameters:
             raw (bool, optional):
                 If ``False``, return only parsed data (this is the default).
                 If ``True``, return all data unparsed.
+            human (bool, optional):
+                If ``False``, return variable names untranslated, for API (this is the default).
+                If ``True``, return variable names in readable text.
 
         Return:
             dict: Flash data (parsed or raw)
 
+        Example:
+            >>> mcp.read_flash_info()
+            {
+                "CHIP_SETTINGS": {
+                    "adc_ref": "VDD",
+                    "clk_duty": 50,
+                    "clk_freq": "12MHz",
+                    "dac_ref": "VDD",
+                    "dac_val": 0,
+                    "ioc": "both",
+                    "ma": 100,
+                    "pid": "0x00DD",
+                    "pwr": "disabled",
+                    "vid": "0x04D8"
+                },
+                "GP_SETTINGS": {
+                    "GP0": {
+                        "func": "GPIO_IN",
+                        "outval": 0
+                    },
+                    "GP1": {
+                        "func": "GPIO_IN",
+                        "outval": 0
+                    },
+                    "GP2": {
+                        "func": "GPIO_IN",
+                        "outval": 0
+                    },
+                    "GP3": {
+                        "func": "GPIO_IN",
+                        "outval": 0
+                    }
+                },
+                "USB_FACT_SERIAL": "01234567",
+                "USB_PRODUCT": "MCP2221 USB-I2C/UART Combo",
+                "USB_SERIAL": "0000033333",
+                "USB_VENDOR": "Microchip Technology Inc."
+            }
+
+
         Hint:
-            This is the function used to stringfy the object.
+            When called with `human = true` parameter, this is the function used to
+            stringfy the object.
         """
-        CHIP_SETTINGS_STR   = "Chip settings"
-        GP_SETTINGS_STR     = "GP settings"
-        USB_VENDOR_STR      = "USB Manufacturer"
-        USB_PRODUCT_STR     = "USB Product"
-        USB_SERIAL_STR      = "USB Serial"
-        USB_FACT_SERIAL_STR = "Factory Serial"
+
 
         data = {
-            CHIP_SETTINGS_STR:    self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_CHIP_SETTINGS]),
-            GP_SETTINGS_STR:      self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_GP_SETTINGS]),
-            USB_VENDOR_STR:       self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_USB_MANUFACTURER]),
-            USB_PRODUCT_STR:      self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_USB_PRODUCT]),
-            USB_SERIAL_STR:       self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_USB_SERIALNUM]),
-            USB_FACT_SERIAL_STR:  self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_CHIP_SERIALNUM]),
+            "CHIP_SETTINGS"   : self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_CHIP_SETTINGS]),
+            "GP_SETTINGS"     : self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_GP_SETTINGS]),
+            "USB_VENDOR"      : self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_USB_MANUFACTURER]),
+            "USB_PRODUCT"     : self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_USB_PRODUCT]),
+            "USB_SERIAL"      : self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_USB_SERIALNUM]),
+            "USB_FACT_SERIAL" : self.send_cmd([CMD_READ_FLASH_DATA, FLASH_DATA_CHIP_SERIALNUM]),
         }
 
         if raw:
             return data
 
-        data[USB_VENDOR_STR]      = self._parse_wchar_structure(data[USB_VENDOR_STR])
-        data[USB_PRODUCT_STR]     = self._parse_wchar_structure(data[USB_PRODUCT_STR])
-        data[USB_SERIAL_STR]      = self._parse_wchar_structure(data[USB_SERIAL_STR])
-        data[USB_FACT_SERIAL_STR] = self._parse_factory_serial(data[USB_FACT_SERIAL_STR])
-        data[CHIP_SETTINGS_STR]   = self._parse_chip_settings_struct(data[CHIP_SETTINGS_STR])
-        data[GP_SETTINGS_STR]     = self._parse_gp_settings_struct(data[GP_SETTINGS_STR])
+        data["USB_VENDOR"]      = self._parse_wchar_structure(data["USB_VENDOR"])
+        data["USB_PRODUCT"]     = self._parse_wchar_structure(data["USB_PRODUCT"])
+        data["USB_SERIAL"]      = self._parse_wchar_structure(data["USB_SERIAL"])
+        data["USB_FACT_SERIAL"] = self._parse_factory_serial(data["USB_FACT_SERIAL"])
+        data["CHIP_SETTINGS"]   = self._parse_chip_settings_struct(data["CHIP_SETTINGS"])
+        data["GP_SETTINGS"]     = self._parse_gp_settings_struct(data["GP_SETTINGS"])
+
+        if not human:
+            return data
+
+        return self._humanify(data)
 
-        return data
 
     def _parse_wchar_structure(self, buf):
         cmd_echo  = buf[RESPONSE_ECHO_BYTE]
         cmd_error = buf[RESPONSE_STATUS_BYTE]
         strlen    = buf[2] - 2
         three     = buf[3]
         w_str     = buf[4:4+strlen]
@@ -408,37 +454,177 @@
         strlen    = buf[2]
         three     = buf[3]
         str       = buf[4:4+strlen]
         str = bytes(str).decode('ascii')
         return str
 
     def _parse_chip_settings_struct(self, buf):
-        vid = (buf[9] << 8) +  buf[8]
-        pid = (buf[11] << 8) +  buf[10]
-        mA = buf[13] * 2
-        pmo_str = "enabled" if buf[12] & 0b00100000 else "disabled"
-        ide_bits = (buf[7] & 0b1100000) >> 5
-        ide_str = ("both"   if ide_bits == 3 else
-                  "falling" if ide_bits == 2 else
-                  "raising" if ide_bits == 1 else
-                  "none")
+        vid = (buf[FLASH_CHIP_SETTINGS_HVID + FLASH_OFFSET_READ] << 8) \
+            +  buf[FLASH_CHIP_SETTINGS_LVID + FLASH_OFFSET_READ]
+
+        pid = (buf[FLASH_CHIP_SETTINGS_HPID + FLASH_OFFSET_READ] << 8) \
+            +  buf[FLASH_CHIP_SETTINGS_LPID + FLASH_OFFSET_READ]
+
+        mA = buf[FLASH_CHIP_SETTINGS_USBMA + FLASH_OFFSET_READ] * 2
+
+        if buf[FLASH_CHIP_SETTINGS_USBPWR + FLASH_OFFSET_READ] & 0b00100000:
+            pmo_str = "enabled"
+        else:
+            pmo_str = "disabled"
+
+        ide_bits = (buf[FLASH_CHIP_SETTINGS_INT_ADC + FLASH_OFFSET_READ] & 0b01100000) >> 5
+        ide_str = ("both"    if ide_bits == 3 else
+                   "falling" if ide_bits == 2 else
+                   "rising"  if ide_bits == 1 else
+                   "none")
+
+        ADCREF = (buf[FLASH_CHIP_SETTINGS_INT_ADC + FLASH_OFFSET_READ] & 0b00000100) >> 2
+        ADCVRM = (buf[FLASH_CHIP_SETTINGS_INT_ADC + FLASH_OFFSET_READ] & 0b00011000) >> 3
+        adc_ref_str = ("VDD"    if ADCREF == 0 else
+                       "1.024V" if ADCVRM == 0b01 else
+                       "2.048V" if ADCVRM == 0b10 else
+                       "4.096V" if ADCVRM == 0b11 else
+                       "OFF")
+
+        CLKDC  = (buf[FLASH_CHIP_SETTINGS_CLOCK + FLASH_OFFSET_READ] & 0b00011000) >> 3
+        clk_dc_str = (75 if CLKDC == 0b11 else
+                      50 if CLKDC == 0b10 else
+                      25 if CLKDC == 0b01 else
+                      0)
+
+        CLKDIV = (buf[FLASH_CHIP_SETTINGS_CLOCK + FLASH_OFFSET_READ] & 0b00000111) >> 0
+        clk_freq_str = ("375kHz" if CLKDIV == 0b111 else
+                        "750kHz" if CLKDIV == 0b110 else
+                        "1.5MHz" if CLKDIV == 0b101 else
+                        "3MHz"   if CLKDIV == 0b100 else
+                        "6MHz"   if CLKDIV == 0b011 else
+                        "12MHz"  if CLKDIV == 0b010 else
+                        "24MHz"  if CLKDIV == 0b001 else
+                        "reserved")
+
+        DACREF = (buf[FLASH_CHIP_SETTINGS_DAC + FLASH_OFFSET_READ] & 0b00100000) >> 5
+        DACVRM = (buf[FLASH_CHIP_SETTINGS_DAC + FLASH_OFFSET_READ] & 0b11000000) >> 6
+        dac_ref_str = ("VDD"    if DACREF == 0 else
+                       "1.024V" if DACVRM == 0b01 else
+                       "2.048V" if DACVRM == 0b10 else
+                       "4.096V" if DACVRM == 0b11 else
+                       "OFF")
+
+        DACVAL = (buf[FLASH_CHIP_SETTINGS_DAC + FLASH_OFFSET_READ] & 0b00011111) >> 0
 
         data = {
-            "USB VID": "0x{:04X}".format(vid),
-            "USB PID": "0x{:04X}".format(pid),
-            "USB requested number of mA": mA,
-            "Power management options": pmo_str,
-            "Interrupt detection edge": ide_str,
+            "vid": "0x{:04X}".format(vid),
+            "pid": "0x{:04X}".format(pid),
+            "ma": mA,
+            "pwr": pmo_str,
+            "ioc": ide_str,
+            "clk_duty": clk_dc_str,
+            "clk_freq": clk_freq_str,
+            "adc_ref": adc_ref_str,
+            "dac_ref": dac_ref_str,
+            "dac_val": DACVAL,
         }
+
         return data
 
     def _parse_gp_settings_struct(self, buf):
-        data = { }
+        GPSETTING0 = buf[FLASH_GP_SETTINGS_GP0 + FLASH_OFFSET_READ]
+        GPSETTING1 = buf[FLASH_GP_SETTINGS_GP1 + FLASH_OFFSET_READ]
+        GPSETTING2 = buf[FLASH_GP_SETTINGS_GP2 + FLASH_OFFSET_READ]
+        GPSETTING3 = buf[FLASH_GP_SETTINGS_GP3 + FLASH_OFFSET_READ]
+
+        data = {}
+        data["GP0"] = self._parse_gp_settings_register(GPSETTING0, 0)
+        data["GP1"] = self._parse_gp_settings_register(GPSETTING1, 1)
+        data["GP2"] = self._parse_gp_settings_register(GPSETTING2, 2)
+        data["GP3"] = self._parse_gp_settings_register(GPSETTING3, 3)
+
         return data
 
+    def _parse_gp_settings_register(self, GPSETTING, pin):
+        GPIOOUTVAL = (GPSETTING & 0b00010000) >> 4
+        GPIODIR    = (GPSETTING & 0b00001000) >> 3
+        GPDES      = (GPSETTING & 0b00000111)
+
+        data = {}
+        data["outval"] = GPIOOUTVAL
+
+        # GPIO operation
+        if GPDES == 0:
+            if GPIODIR == 0: data["func"] = "GPIO_OUT"
+            else: data["func"] = "GPIO_IN"
+
+        #  Dedicated function operation
+        elif GPDES == 1:
+            if pin == 0: data["func"] = "SSPND"
+            if pin == 1: data["func"] = "CLK_OUT"
+            if pin == 2: data["func"] = "USBCFG"
+            if pin == 3: data["func"] = "LED_I2C"
+
+        #  Alternate function 0
+        elif GPDES == 2:
+            if pin == 0: data["func"] = "LED_URX"
+            if pin == 1: data["func"] = "ADC"
+            if pin == 2: data["func"] = "ADC"
+            if pin == 3: data["func"] = "ADC"
+
+        #  Alternate function 1
+        elif GPDES == 3:
+            if pin == 0: data["func"] = "reserved"
+            if pin == 1: data["func"] = "LED_UTX"
+            if pin == 2: data["func"] = "DAC"
+            if pin == 3: data["func"] = "DAC"
+
+        #  Alternate function 2
+        elif GPDES == 4:
+            if pin == 0: data["func"] = "reserved"
+            if pin == 1: data["func"] = "IOC"
+            if pin == 2: data["func"] = "reserved"
+            if pin == 3: data["func"] = "reserved"
+
+        else:
+            data["func"] == "reserved"
+
+        return data
+
+    def _humanify(self, data):
+        """Convert variable names into human strings recursively."""
+        h = {}
+        for k,v in data.items():
+            if isinstance(v, dict):
+                h[self._var2str(k)] = self._humanify(v)
+            else:
+                h[self._var2str(k)] = v
+        return h
+
+    def _var2str(self, varname):
+        """Convert variable names into human strings."""
+        strings = {
+            "vid"             : "USB VID",
+            "pid"             : "USB PID",
+            "ma"              : "USB requested number of mA",
+            "pwr"             : "Power management options",
+            "ioc"             : "Interrupt detection edge",
+            "adc_ref"         : "ADC reference value",
+            "clk_duty"        : "Clock output duty cycle",
+            "clk_freq"        : "Clock output frequency",
+            "dac_ref"         : "DAC reference value",
+            "dac_val"         : "DAC output value",
+            "CHIP_SETTINGS"   : "Chip settings",
+            "GP_SETTINGS"     : "General Purpose IO settings",
+            "USB_VENDOR"      : "USB Manufacturer",
+            "USB_PRODUCT"     : "USB Product",
+            "USB_SERIAL"      : "USB Serial Number",
+            "USB_FACT_SERIAL" : "Factory Serial Number",
+            "func"            : "Pin designated operation",
+            "outval"          : "Default output value",
+        }
+
+        return strings.get(varname, varname)
+
 
     #######################################################################
     # SRAM
     #######################################################################
     def SRAM_config(self,
         clk_output = None,
         dac_ref    = None,
@@ -573,14 +759,27 @@
         cmd[4]  = self.status["dac_value"] | ALTER_DAC_VALUE
         cmd[5]  = self.status["adc_ref"]   | ALTER_ADC_REF
         r = self.send_cmd(cmd)
         if r[RESPONSE_STATUS_BYTE] != RESPONSE_RESULT_OK:
             raise RuntimeError("SRAM write error.")
 
 
+    def _reinforce_SRAM(self):
+        """ The only purpose of this function is to solve some weird bugs on MCP2221. """
+        self.SRAM_config(
+            dac_ref    = self.status["dac_ref"],
+            dac_value  = self.status["dac_value"],
+            adc_ref    = self.status["adc_ref"],
+            gp0        = self.status["GPIO"]["gp0"],
+            gp1        = self.status["GPIO"]["gp1"],
+            gp2        = self.status["GPIO"]["gp2"],
+            gp3        = self.status["GPIO"]["gp3"])
+
+
+
     #######################################################################
     # GPIO
     #######################################################################
     def GPIO_write(self, gp0 = None, gp1 = None, gp2 = None, gp3 = None):
         """ Set pin output values.
 
         If a pin is omitted, it will preserve the value.
@@ -941,14 +1140,17 @@
             ref = ADC_REF_VDD
             vrm = ADC_VRM_OFF
         else:
             raise ValueError("Accepted values for ref are 'OFF', '1.024V', '2.048V', '4.096V' and 'VDD'.")
 
         self.SRAM_config(adc_ref = ref | vrm)
 
+        # When GP1, 2 and 3 are ADC and ADC_REF is Vdd. If Vrm ref is selected, ADC stop working.
+        self._reinforce_SRAM()
+
 
     def ADC_read(self):
         """ Read all Analog to Digital Converter (ADC) channels.
 
         Analog value is always available regardless of pin function (see :func:`set_pin_function`).
         If pin is configured as output (GPIO_OUT or LED_I2C), the read value is always the output state.
 
@@ -974,17 +1176,17 @@
             >>> mcp.set_pin_function(
             ...    gp1 = "GPIO_OUT", out1 = True,
             ...    gp2 = "GPIO_OUT", out2 = False)
             >>> mcp.ADC_read()
             (1023, 0, 198)
         """
         buf = self.send_cmd([CMD_POLL_STATUS_SET_PARAMETERS])
-        adc1 = buf[50] + 256*buf[51]
-        adc2 = buf[52] + 256*buf[53]
-        adc3 = buf[54] + 256*buf[55]
+        adc1 = buf[I2C_POLL_RESP_ADC_CH0_LSB] + 256*buf[I2C_POLL_RESP_ADC_CH0_MSB]
+        adc2 = buf[I2C_POLL_RESP_ADC_CH1_LSB] + 256*buf[I2C_POLL_RESP_ADC_CH1_MSB]
+        adc3 = buf[I2C_POLL_RESP_ADC_CH2_LSB] + 256*buf[I2C_POLL_RESP_ADC_CH2_MSB]
         return (adc1, adc2, adc3)
 
 
     #######################################################################
     # DAC
     #######################################################################
     def DAC_config(self, ref = "VDD", out = None):
@@ -1075,14 +1277,89 @@
         if out not in range(0, 32):
             raise ValueError("Accepted values for out are from 0 to 31.")
 
         self.SRAM_config(dac_value = out)
 
 
     #######################################################################
+    # Interrupt On Change
+    #######################################################################
+
+    def IOC_read(self):
+        """ Read Interruption On Change flag.
+
+        To enable Interruption Detection mechanism, pin designation must be *IOC*. See :func:`set_pin_function`.
+
+        Return:
+            int: Value of interrupt flag.
+
+        Example:
+            >>> mcp.IOC_read()
+            1
+
+        """
+        rbuf = self.send_cmd([CMD_POLL_STATUS_SET_PARAMETERS])
+        intflag = rbuf[I2C_POLL_RESP_INT_FLAG]
+        return intflag
+
+
+    def IOC_clear(self):
+        """ Clear Interruption On Change flag.
+
+        Example:
+            >>> mcp.IOC_read()
+            1
+            >>> mcp.IOC_clear()
+            >>> mcp.IOC_read()
+            0
+            >>>
+        """
+        self.SRAM_config(int_conf = INT_FLAG_CLEAR)
+
+
+    def IOC_config(self, edge = "both"):
+        """ Configure Interruption On Change edge.
+
+        Valid values for ``edge``:
+            - **none**: disable interrupt detection
+            - **rising**: fire interruption on rising edge (i.e. when GP1 goes from Low to High).
+            - **falling**: fire interruption on falling edge (i.e. when GP1 goes from High to Low).
+            - **both**: fire interruption on both (i.e. when GP1 state changes).
+
+        Remember to call :func:`save_config` to persist this configuration when reset the chip.
+
+        Parameters:
+            edge (str): which edge triggers the interruption (see description).
+
+        Raises:
+            ValueError: if edge detection value is not valid.
+
+        Example:
+            >>> mcp.IOC_config(edge = "rising")
+            >>>
+
+        See also:
+            :func:`set_pin_function`, :func:`IOC_clear`, :func:`IOC_read`.
+        """
+        if edge == "none":
+            edge = INT_POS_EDGE_DISABLE | INT_NEG_EDGE_DISABLE
+        elif edge == "rising":
+            edge = INT_POS_EDGE_ENABLE  | INT_NEG_EDGE_DISABLE
+        elif edge == "falling":
+            edge = INT_POS_EDGE_DISABLE | INT_NEG_EDGE_ENABLE
+        elif edge == "both":
+            edge = INT_POS_EDGE_ENABLE  | INT_NEG_EDGE_ENABLE
+        else:
+            raise ValueError("Invalid edge detection. Allowed: 'rising', 'falling', 'both' or 'none'.")
+
+        self.SRAM_config(int_conf = edge | INT_FLAG_CLEAR)
+
+
+
+    #######################################################################
     # I2C
     #######################################################################
     def I2C_speed(self, speed=100000):
         """ Set I2C bus speed.
 
         Acceptable values for speed are between 47kHz and 400kHz.
 
@@ -1615,235 +1892,56 @@
             "initialized" : rbuf[I2C_POLL_RESP_UNDOCUMENTED_21] != 0
         }
 
         return i2c_status
 
 
     #######################################################################
-    # I2C deprecated
-    #######################################################################
-
-    def I2C_is_idle(self):
-        """ Check if the I2C engine is idle.
-
-        Warning:
-            **Deprecated.**
-
-            There is no need for this method anymore. The bus is managed automatically.
-            You can use :func:`_i2c_status` function to know the I2C internal status details.
-
-        Returns:
-            bool: True if idle, False if engine is in the middle of a transfer or busy.
-
-        Raises:
-            LowSDAError: if **SCL** line is down (read exception description).
-            LowSCLError: if **SDA** line is down (read exception description).
-
-        Example:
-            >>> mcp.I2C_is_idle()
-            True
-            >>>
-        """
-        import warnings
-        warnings.warn("This method is deprecated and will be removed in the next release.",
-            DeprecationWarning,
-            stacklevel=2)
-
-        rbuf = self.send_cmd([CMD_POLL_STATUS_SET_PARAMETERS])
-
-        if rbuf[I2C_POLL_RESP_SCL] == 0:
-            self.status["i2c_dirty"] = True
-            raise LowSCLError("SCL is low. I2C bus is busy or missing pull-up resistor.")
-
-        if rbuf[I2C_POLL_RESP_SDA] == 0:
-            self.status["i2c_dirty"] = True
-            raise LowSDAError("SDA is low. Missing pull-up resistor, I2C bus is busy or slave device in the middle of sending data.")
-
-        if rbuf[I2C_POLL_RESP_STATUS]:
-            self.status["i2c_dirty"] = True
-            return False
-        else:
-            self.status["i2c_dirty"] = False
-            return True
-
-
-    def I2C_cancel(self):
-        """ Try to cancel an active I2C read or write command.
-
-        Warning:
-            **Deprecated.**
-
-            There is no need for this method anymore. The bus is managed automatically.
-            You can use :func:`_i2c_release` function to manually cancel a transfer.
-
-        Return:
-            bool: True if device is now ready to go. False if the engine is not idle.
-
-        Raises:
-            LowSDAError: if I2C engine detects the **SCL** line does not go up (read exception description).
-            LowSCLError: if I2C engine detects the **SDA** line does not go up (read exception description).
-
-        Examples:
-
-            Last transfer was cancel, and engine is ready for the next operation:
-
-            >>> mcp.I2C_cancel()
-            True
-
-            Last transfer failed, and cancel failed too because I2C bus seems busy:
-
-            >>> mcp.I2C_cancel()
-            Traceback (most recent call last):
-            ...
-            EasyMCP2221.exceptions.LowSCLError: SCL is low. I2C bus is busy or missing pull-up resistor.
-
-        Note:
-            Do not call this function without issuing a :func:`I2C_read` or
-            :func:`I2C_write` first. It could render I2C engine inoperative until
-            the next reset.
-
-            >>> mcp.reset()
-            >>> mcp.I2C_is_idle()
-            True
-            >>> mcp.I2C_cancel()
-            False
-
-            Now the bus is busy until the next reset.
-
-            >>> mcp.I2C_speed(100000)
-            Traceback (most recent call last):
-            ...
-            RuntimeError: I2C speed is not valid or bus is busy.
-            >>> mcp.I2C_cancel()
-            False
-            >>> mcp.I2C_is_idle()
-            False
-            >>> mcp.I2C_cancel()
-            False
-
-            After a reset, it will work again.
-
-            >>> mcp.reset()
-            >>> mcp.I2C_is_idle()
-            True
-        """
-        import warnings
-        warnings.warn("This method is deprecated and will be removed in the next release.",
-            DeprecationWarning,
-            stacklevel=2)
-
-        buf = [0] * 3
-        buf[0] = CMD_POLL_STATUS_SET_PARAMETERS
-        buf[1] = 0
-        buf[2] = I2C_CMD_CANCEL_CURRENT_TRANSFER
-
-        rbuf = self.send_cmd(buf)
-
-        # Return idle if the first cancel attempt worked
-        if rbuf[I2C_POLL_RESP_STATUS] == I2C_ST_IDLE:
-            self.status["i2c_dirty"] = False
-            return True
-
-        # Otherwise, sleep, try again and confirm.
-        time.sleep(10/1000)
-        rbuf = self.send_cmd(buf)
-
-        if rbuf[I2C_POLL_RESP_SCL] == 0:
-            self.status["i2c_dirty"] = True
-            raise LowSCLError("SCL is low. I2C bus is busy or missing pull-up resistor.")
-
-        if rbuf[I2C_POLL_RESP_SDA] == 0:
-            self.status["i2c_dirty"] = True
-            raise LowSDAError("SDA is low. Missing pull-up resistor, I2C bus is busy or slave device in the middle of sending data.")
-
-        return self.I2C_is_idle()
-
-
-
-
-    #######################################################################
     # Wake-up
     #######################################################################
-    def enable_power_management(self, enable = False):
+    def enable_power_management(self, enable=True):
         """ Enable or disable USB Power Management options for this device.
 
-        Set or clear Remote Wake-up Capability bit in flash configuration.
+        Set or clear Remote Wake-up Capability bit.
+        Remember to call :func:`save_config` after this function to save the new settings.
+
+        Remote wake-up is triggered by Interrupt detection on GP1
+        (see :func:`set_pin_function` and :func:`IOC_config`).
 
-        If enabled, Power Management Tab is available for this device in the Device Manager (Windows).
-        So you can mark *"Allow this device to wake the computer"* option.
+        When enabled, Power Management Tab is available for this device in the Device Manager (Windows).
+        To wake-up the computer *"Allow this device to wake the computer"* option must be set in Device Manager.
 
-        A device :func:`reset` (or power supply cycle) is needed in order for changes to take effect.
+        USB power attributes are only read while USB device enumeration. So :func:`reset`
+        (or power supply cycle) is needed in order for changes to take effect.
 
         Parameters:
             enable (bool): Enable or disable Power Management.
 
         Raises:
-            RuntimeError: If write to flash command failed.
-            AssertionError: In rare cases, when some bug might have inadvertently activated Flash protection or permanent chip lock.
+            RuntimeError: If flash read command failed.
 
         Example:
             >>> mcp.enable_power_management(True)
+            >>> mcp.save_config()
             >>> print(mcp)
             ...
                 "Chip settings": {
                     "Power management options": "enabled",
             ...
             >>> mcp.reset()
-            >>>
         """
         chip_settings = self._read_flash_raw(FLASH_DATA_CHIP_SETTINGS)
-        USBPWRATTR = chip_settings[12]
+        USBPWRATTR = chip_settings[FLASH_CHIP_SETTINGS_USBPWR + FLASH_OFFSET_READ]
 
         if enable:
             USBPWRATTR |= 0b00100000
         else:
             USBPWRATTR &= 0b11011111
 
-        chip_settings[12] = USBPWRATTR
-        self._write_flash_raw(FLASH_DATA_CHIP_SETTINGS, chip_settings[4:64])
-
-
-    def wake_up_config(self, edge = "none"):
-        """ Configure interruption edge.
-
-        Valid values for ``edge``:
-            - **none**: disable interrupt detection
-            - **raising**: fire interruption in raising edge (i.e. when GP1 goes from Low to High).
-            - **falling**: fire interruption in falling edge (i.e. when GP1 goes from High to Low).
-            - **both**: fire interruption in both (i.e. when GP1 state changes).
-
-        In order to trigger, GP1 must be assigned to IOC function (see :func:`set_pin_function`).
-
-        To wake-up the computer, Power Management options must be enabled (see :func:`enable_power_management`).
-        And *"Allow this device to wake the computer"* option must be set in Device Manager.
-
-        Remember to call :func:`save_config` to persist this configuration when the chip resets
-
-        Parameters:
-            edge (str): which edge triggers the interruption (see description).
-
-        Raises:
-            ValueError: if edge detection given.
-
-        Example:
-            >>> mcp.wake_up_config("both")
-            >>>
-        """
-        if edge == "none":
-            edge = INT_POS_EDGE_DISABLE | INT_NEG_EDGE_DISABLE
-        elif edge == "raising":
-            edge = INT_POS_EDGE_ENABLE  | INT_NEG_EDGE_DISABLE
-        elif edge == "falling":
-            edge = INT_POS_EDGE_DISABLE | INT_NEG_EDGE_ENABLE
-        elif edge == "both":
-            edge = INT_POS_EDGE_ENABLE  | INT_NEG_EDGE_ENABLE
-        else:
-            raise ValueError("Invalid edge detection. Allowed: 'raising', 'falling', 'both' or 'none'.")
-
-        self.SRAM_config(int_conf = edge | INT_FLAG_CLEAR)
+        self.unsaved_SRAM[FLASH_CHIP_SETTINGS_USBPWR] = USBPWRATTR
 
 
     #######################################################################
     # Reset
     #######################################################################
     def reset(self):
         """ Reset MCP2221.
```

### Comparing `EasyMCP2221-1.6.3/EasyMCP2221/__init__.py` & `easymcp2221-1.7.0/EasyMCP2221/__init__.py`

 * *Files identical despite different names*

### Comparing `EasyMCP2221-1.6.3/EasyMCP2221/exceptions.py` & `easymcp2221-1.7.0/EasyMCP2221/exceptions.py`

 * *Files identical despite different names*

### Comparing `EasyMCP2221-1.6.3/EasyMCP2221/smbus.py` & `easymcp2221-1.7.0/EasyMCP2221/smbus.py`

 * *Files identical despite different names*

### Comparing `EasyMCP2221-1.6.3/LICENSE` & `easymcp2221-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `EasyMCP2221-1.6.3/README.rst` & `easymcp2221-1.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `EasyMCP2221-1.6.3/pyproject.toml` & `easymcp2221-1.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "EasyMCP2221"
-version = "1.6.3"
+version = "1.7.0"
 authors = [
   { name="Reinoso Guzman", email="electronicayciencia@gmail.com" },
 ]
 description = "Python module to interface with MCP2221 focused on ease of use."
 readme = "README.rst"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `EasyMCP2221-1.6.3/PKG-INFO` & `easymcp2221-1.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EasyMCP2221
-Version: 1.6.3
+Version: 1.7.0
 Summary: Python module to interface with MCP2221 focused on ease of use.
 Author-email: Reinoso Guzman <electronicayciencia@gmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```


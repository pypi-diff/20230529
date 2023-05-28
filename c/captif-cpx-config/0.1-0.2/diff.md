# Comparing `tmp/captif_cpx_config-0.1.tar.gz` & `tmp/captif_cpx_config-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_config-0.1.tar", max compression
+gzip compressed data, was "captif_cpx_config-0.2.tar", max compression
```

## Comparing `captif_cpx_config-0.1.tar` & `captif_cpx_config-0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-05-28 21:48:04.921696 captif_cpx_config-0.1/LICENSE
--rw-r--r--   0        0        0       19 2023-05-28 21:48:04.921696 captif_cpx_config-0.1/README.md
--rw-r--r--   0        0        0       44 2023-05-28 21:48:04.921696 captif_cpx_config-0.1/captif_cpx_config/__init__.py
--rw-r--r--   0        0        0     3860 2023-05-28 21:48:04.921696 captif_cpx_config-0.1/captif_cpx_config/metadata.py
--rw-r--r--   0        0        0      498 2023-05-28 21:48:04.921696 captif_cpx_config-0.1/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-28 23:25:46.113794 captif_cpx_config-0.2/LICENSE
+-rw-r--r--   0        0        0       19 2023-05-28 23:25:46.113794 captif_cpx_config-0.2/README.md
+-rw-r--r--   0        0        0       44 2023-05-28 23:25:46.113794 captif_cpx_config-0.2/captif_cpx_config/__init__.py
+-rw-r--r--   0        0        0     3855 2023-05-28 23:25:46.113794 captif_cpx_config-0.2/captif_cpx_config/metadata.py
+-rw-r--r--   0        0        0      498 2023-05-28 23:25:46.113794 captif_cpx_config-0.2/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.2/PKG-INFO
```

### Comparing `captif_cpx_config-0.1/LICENSE` & `captif_cpx_config-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_config-0.1/captif_cpx_config/metadata.py` & `captif_cpx_config-0.2/captif_cpx_config/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     wheel_bay_configuration_details: str = Field(
         description="description of the wheel bay configuration",
     )
     wheel_bay_calibration_date: date_ = Field(
         description="wheel bay / device correction calibration date"
     )
     microphone_details: list["MicrophoneDetails"]
-    accelerometer_details: Optional[list["AccelerometerDetails"]]
+    accelerometer_details: list["AccelerometerDetails"] = []
     tyre_details: "TyreDetails"
     device_corrections: "DeviceCorrections"
 
 
 class Metadata(BaseModel):
     measurement_details: "MeasurementDetails"
     wheel_bay_details: list["WheelBayDetails"]
```

### Comparing `captif_cpx_config-0.1/PKG-INFO` & `captif_cpx_config-0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-cpx-config
-Version: 0.1
+Version: 0.2
 Summary: 
 License: MIT
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


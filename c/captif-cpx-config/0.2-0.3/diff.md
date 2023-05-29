# Comparing `tmp/captif_cpx_config-0.2.tar.gz` & `tmp/captif_cpx_config-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "captif_cpx_config-0.2.tar", max compression
+gzip compressed data, was "captif_cpx_config-0.3.tar", max compression
```

## Comparing `captif_cpx_config-0.2.tar` & `captif_cpx_config-0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1084 2023-05-28 23:25:46.113794 captif_cpx_config-0.2/LICENSE
--rw-r--r--   0        0        0       19 2023-05-28 23:25:46.113794 captif_cpx_config-0.2/README.md
--rw-r--r--   0        0        0       44 2023-05-28 23:25:46.113794 captif_cpx_config-0.2/captif_cpx_config/__init__.py
--rw-r--r--   0        0        0     3855 2023-05-28 23:25:46.113794 captif_cpx_config-0.2/captif_cpx_config/metadata.py
--rw-r--r--   0        0        0      498 2023-05-28 23:25:46.113794 captif_cpx_config-0.2/pyproject.toml
--rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1084 2023-05-29 00:00:45.690899 captif_cpx_config-0.3/LICENSE
+-rw-r--r--   0        0        0       19 2023-05-29 00:00:45.690899 captif_cpx_config-0.3/README.md
+-rw-r--r--   0        0        0       44 2023-05-29 00:00:45.690899 captif_cpx_config-0.3/captif_cpx_config/__init__.py
+-rw-r--r--   0        0        0     3959 2023-05-29 00:00:45.690899 captif_cpx_config-0.3/captif_cpx_config/metadata.py
+-rw-r--r--   0        0        0      498 2023-05-29 00:00:45.690899 captif_cpx_config-0.3/pyproject.toml
+-rw-r--r--   0        0        0      519 1970-01-01 00:00:00.000000 captif_cpx_config-0.3/PKG-INFO
```

### Comparing `captif_cpx_config-0.2/LICENSE` & `captif_cpx_config-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `captif_cpx_config-0.2/captif_cpx_config/metadata.py` & `captif_cpx_config-0.3/captif_cpx_config/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     )
 
 
 class AccelerometerDetails(BaseModel):
     accelerometer_position: Literal["chassis", "axle"] = Field(
         description="accelerometer position ('chassis' or 'axle')",
     )
+    accelerometer_serial_number: str = Field(
+        description="accelerometer serial number",
+    ),
     accelerometer_sensitivity_mv_g: float = Field(
         description="accelerometer sensitivity in mV/g",
     )
     wav_file_channel_number: int = Field(
         description=(
             "channel number in the wav file corresponding to the accelerometer"
         ),
```

### Comparing `captif_cpx_config-0.2/PKG-INFO` & `captif_cpx_config-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: captif-cpx-config
-Version: 0.2
+Version: 0.3
 Summary: 
 License: MIT
 Author: John Bull
 Author-email: john.bull@nzta.govt.nz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```


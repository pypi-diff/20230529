# Comparing `tmp/aioapcaccess-0.2.1-py3-none-any.whl.zip` & `tmp/aioapcaccess-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4687 bytes, number of entries: 6
--rw-r--r--  2.0 unx     3466 b- defN 23-Mar-26 00:29 aioapcaccess/__init__.py
--rw-r--r--  2.0 unx     1067 b- defN 23-Mar-26 00:29 aioapcaccess-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     3241 b- defN 23-Mar-26 00:29 aioapcaccess-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Mar-26 00:29 aioapcaccess-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       13 b- defN 23-Mar-26 00:29 aioapcaccess-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      492 b- defN 23-Mar-26 00:29 aioapcaccess-0.2.1.dist-info/RECORD
-6 files, 8371 bytes uncompressed, 3793 bytes compressed:  54.7%
+Zip file size: 4701 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     3488 b- defN 23-May-29 03:00 aioapcaccess/__init__.py
+-rw-r--r--  2.0 unx     1067 b- defN 23-May-29 03:00 aioapcaccess-0.3.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3241 b- defN 23-May-29 03:00 aioapcaccess-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 03:00 aioapcaccess-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       13 b- defN 23-May-29 03:00 aioapcaccess-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      492 b- defN 23-May-29 03:00 aioapcaccess-0.3.0.dist-info/RECORD
+6 files, 8393 bytes uncompressed, 3807 bytes compressed:  54.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: aioapcaccess/__init__.py
 Comment: 
 
-Filename: aioapcaccess-0.2.1.dist-info/LICENSE
+Filename: aioapcaccess-0.3.0.dist-info/LICENSE
 Comment: 
 
-Filename: aioapcaccess-0.2.1.dist-info/METADATA
+Filename: aioapcaccess-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: aioapcaccess-0.2.1.dist-info/WHEEL
+Filename: aioapcaccess-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: aioapcaccess-0.2.1.dist-info/top_level.txt
+Filename: aioapcaccess-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: aioapcaccess-0.2.1.dist-info/RECORD
+Filename: aioapcaccess-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## aioapcaccess/__init__.py

```diff
@@ -12,38 +12,39 @@
     "Seconds",
     "Percent",
     "Volts",
     "Watts",
     "Amps",
     "Hz",
     "C",
+    "C Internal",
     "VA",
     "Percent Load Capacity",
 }
 
 
 async def request_status(
     host: str = "localhost",
     port: int = 3551,
 ) -> OrderedDict[str, str]:
     """Connect to the APCUPSd NIS and request its status and return the parsed dict.
 
     :param host: the host which apcupsd is listening on.
     :param port: the port which apcupsd is listening on.
-    :return an ordered dict, where key is the field (e.g., "NOMINV") and value is the
+    :return: an ordered dict, where key is the field (e.g., "NOMINV") and value is the
     value. For example, {"NOMINV": "12.0 Volts", ..., "SERIALNO": "XXXXXXX"}
     """
     return parse_raw_status(await request_raw_status(host, port))
 
 
 def parse_raw_status(raw_status: bytes) -> OrderedDict[str, str]:
     """Parse the raw status and return an ordered dict.
 
     :param raw_status: raw status string retrieved from apcupsd.
-    :return an ordered dict, where key is the field (e.g., "NOMINV") and value is the
+    :return: an ordered dict, where key is the field (e.g., "NOMINV") and value is the
     value. For example, {"NOMINV": "12.0 Volts", ..., "SERIALNO": "XXXXXXX"}
     """
     result = OrderedDict()
 
     # Strip EOF from the status and decode to string.
     if not raw_status.endswith(_EOF):
         raise ValueError("raw status does not end with EOF")
@@ -76,15 +77,15 @@
 
 
 async def request_raw_status(host: str = "localhost", port: int = 3551) -> bytes:
     """Connect to the APCUPSd NIS and request its status in raw format.
 
     :param host: the host which apcupsd is listening on.
     :param port: the port which apcupsd is listening on.
-    :return a bytes object containing raw status obtained from apcupsd.
+    :return: a bytes object containing raw status obtained from apcupsd.
     """
 
     reader, writer = await asyncio.open_connection(host, port)
     try:
         writer.write(_STATUS_CMD)
         await writer.drain()
 
@@ -97,15 +98,15 @@
 
 def split_unit(value: str) -> tuple[str, str | None]:
     """Split the unit suffix from the value (if available).
 
     For the set of supported unit suffixes, see aioapcaccess.UNITS.
 
     :param value: the retrieved value string.
-    :return a tuple consisting of the value and the unit (None if not found).
+    :return: a tuple consisting of the value and the unit (None if not found).
     """
     for unit in UNITS:
         if not value.endswith(unit):
             continue
         return value[: -len(unit)].strip(), unit
 
     return value, None
```

## Comparing `aioapcaccess-0.2.1.dist-info/LICENSE` & `aioapcaccess-0.3.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `aioapcaccess-0.2.1.dist-info/METADATA` & `aioapcaccess-0.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioapcaccess
-Version: 0.2.1
+Version: 0.3.0
 Summary: Async version of apcaccess library implemented in python.
 Author-email: Yuxin Wang <yuxinwang.dev@gmail.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```


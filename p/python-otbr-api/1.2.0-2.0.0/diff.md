# Comparing `tmp/python-otbr-api-1.2.0.tar.gz` & `tmp/python-otbr-api-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-otbr-api-1.2.0.tar", last modified: Thu May 25 07:56:15 2023, max compression
+gzip compressed data, was "python-otbr-api-2.0.0.tar", last modified: Mon May 29 07:03:15 2023, max compression
```

## Comparing `python-otbr-api-1.2.0.tar` & `python-otbr-api-2.0.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:56:15.204285 python-otbr-api-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 07:56:15.204285 python-otbr-api-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:56:15.200285 python-otbr-api-1.2.0/python_otbr_api/
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/mdns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/pskc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-25 07:55:54.000000 python-otbr-api-1.2.0/python_otbr_api/tlv_parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 07:56:15.204285 python-otbr-api-1.2.0/python_otbr_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-25 07:56:15.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-25 07:56:15.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:56:15.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-25 07:56:15.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 07:56:15.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 07:56:14.000000 python-otbr-api-1.2.0/python_otbr_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 07:56:15.204285 python-otbr-api-1.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:03:15.862037 python-otbr-api-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-29 07:03:15.862037 python-otbr-api-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:03:15.858037 python-otbr-api-2.0.0/python_otbr_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     6988 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/mdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8565 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/pskc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-05-29 07:02:49.000000 python-otbr-api-2.0.0/python_otbr_api/tlv_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:03:15.862037 python-otbr-api-2.0.0/python_otbr_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:03:15.000000 python-otbr-api-2.0.0/python_otbr_api.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 07:03:15.862037 python-otbr-api-2.0.0/setup.cfg
```

### Comparing `python-otbr-api-1.2.0/LICENSE` & `python-otbr-api-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.2.0/pyproject.toml` & `python-otbr-api-2.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=65.6", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name         = "python-otbr-api"
-version      = "1.2.0"
+version      = "2.0.0"
 license      = {text = "MIT"}
 description  = "API to interact with an OTBR via its REST API"
 readme       = "README.md"
 authors      = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
 requires-python = ">=3.9.0"
```

### Comparing `python-otbr-api-1.2.0/python_otbr_api/__init__.py` & `python-otbr-api-2.0.0/python_otbr_api/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 """API to interact with the Open Thread Border Router REST API."""
 from __future__ import annotations
 from http import HTTPStatus
 import json
-from typing import Literal
 
 import aiohttp
 import voluptuous as vol  # type:ignore[import]
 
-from .models import OperationalDataSet, Timestamp
+from .models import ActiveDataSet, PendingDataSet, Timestamp
 
 # 5 minutes as recommended by
 # https://github.com/openthread/openthread/discussions/8567#discussioncomment-4468920
 PENDING_DATASET_DELAY_TIMER = 5 * 60 * 1000
 
 
 class OTBRError(Exception):
@@ -32,24 +31,24 @@
         self._session = session
         self._url = url
         self._timeout = timeout
 
     async def set_enabled(self, enabled: bool) -> None:
         """Enable or disable the router."""
 
-        response = await self._session.post(
+        response = await self._session.put(
             f"{self._url}/node/state",
             json="enable" if enabled else "disable",
             timeout=aiohttp.ClientTimeout(total=10),
         )
 
         if response.status != HTTPStatus.OK:
             raise OTBRError(f"unexpected http status {response.status}")
 
-    async def get_active_dataset(self) -> OperationalDataSet | None:
+    async def get_active_dataset(self) -> ActiveDataSet | None:
         """Get current active operational dataset.
 
         Returns None if there is no active operational dataset.
         Raises if the http status is 400 or higher or if the response is invalid.
         """
         response = await self._session.get(
             f"{self._url}/node/dataset/active",
@@ -59,15 +58,15 @@
         if response.status == HTTPStatus.NO_CONTENT:
             return None
 
         if response.status != HTTPStatus.OK:
             raise OTBRError(f"unexpected http status {response.status}")
 
         try:
-            return OperationalDataSet.from_json(await response.json())
+            return ActiveDataSet.from_json(await response.json())
         except (json.JSONDecodeError, vol.Error) as exc:
             raise OTBRError("unexpected API response") from exc
 
     async def get_active_dataset_tlvs(self) -> bytes | None:
         """Get current active operational dataset in TLVS format, or None.
 
         Returns None if there is no active operational dataset.
@@ -86,51 +85,49 @@
             raise OTBRError(f"unexpected http status {response.status}")
 
         try:
             return bytes.fromhex(await response.text("ASCII"))
         except ValueError as exc:
             raise OTBRError("unexpected API response") from exc
 
-    async def _create_dataset(
-        self, dataset: OperationalDataSet, dataset_type: Literal["active", "pending"]
-    ) -> None:
-        """Create active or pending operational dataset.
+    async def create_active_dataset(self, dataset: ActiveDataSet) -> None:
+        """Create active operational dataset.
 
-        The passed in OperationalDataSet does not need to be fully populated, any fields
+        The passed in ActiveDataSet does not need to be fully populated, any fields
         not set will be automatically set by the open thread border router.
         Raises if the http status is 400 or higher or if the response is invalid.
         """
-        response = await self._session.post(
-            f"{self._url}/node/dataset/{dataset_type}",
+        response = await self._session.put(
+            f"{self._url}/node/dataset/active",
             json=dataset.as_json(),
             timeout=aiohttp.ClientTimeout(total=self._timeout),
         )
 
         if response.status == HTTPStatus.CONFLICT:
             raise ThreadNetworkActiveError
-        if response.status != HTTPStatus.ACCEPTED:
+        if response.status not in (HTTPStatus.CREATED, HTTPStatus.OK):
             raise OTBRError(f"unexpected http status {response.status}")
 
-    async def create_active_dataset(self, dataset: OperationalDataSet) -> None:
-        """Create active operational dataset.
-
-        The passed in OperationalDataSet does not need to be fully populated, any fields
-        not set will be automatically set by the open thread border router.
-        Raises if the http status is 400 or higher or if the response is invalid.
-        """
-        await self._create_dataset(dataset, "active")
-
-    async def create_pending_dataset(self, dataset: OperationalDataSet) -> None:
+    async def create_pending_dataset(self, dataset: PendingDataSet) -> None:
         """Create pending operational dataset.
 
-        The passed in OperationalDataSet does not need to be fully populated, any fields
+        The passed in PendingDataSet does not need to be fully populated, any fields
         not set will be automatically set by the open thread border router.
         Raises if the http status is 400 or higher or if the response is invalid.
         """
-        await self._create_dataset(dataset, "pending")
+        response = await self._session.put(
+            f"{self._url}/node/dataset/pending",
+            json=dataset.as_json(),
+            timeout=aiohttp.ClientTimeout(total=self._timeout),
+        )
+
+        if response.status == HTTPStatus.CONFLICT:
+            raise ThreadNetworkActiveError
+        if response.status not in (HTTPStatus.CREATED, HTTPStatus.OK):
+            raise OTBRError(f"unexpected http status {response.status}")
 
     async def set_active_dataset_tlvs(self, dataset: bytes) -> None:
         """Set current active operational dataset.
 
         Raises if the http status is 400 or higher or if the response is invalid.
         """
 
@@ -139,15 +136,15 @@
             data=dataset.hex(),
             headers={"Content-Type": "text/plain"},
             timeout=aiohttp.ClientTimeout(total=10),
         )
 
         if response.status == HTTPStatus.CONFLICT:
             raise ThreadNetworkActiveError
-        if response.status != HTTPStatus.ACCEPTED:
+        if response.status not in (HTTPStatus.CREATED, HTTPStatus.OK):
             raise OTBRError(f"unexpected http status {response.status}")
 
     async def set_channel(
         self, channel: int, delay: int = PENDING_DATASET_DELAY_TIMER
     ) -> None:
         """Change the channel
 
@@ -160,17 +157,17 @@
             raise OTBRError("router has no active dataset")
 
         if dataset.active_timestamp and dataset.active_timestamp.seconds is not None:
             dataset.active_timestamp.seconds += 1
         else:
             dataset.active_timestamp = Timestamp(False, 1, 0)
         dataset.channel = channel
-        dataset.delay = delay
+        pending_dataset = PendingDataSet(active_dataset=dataset, delay=delay)
 
-        await self.create_pending_dataset(dataset)
+        await self.create_pending_dataset(pending_dataset)
 
     async def get_extended_address(self) -> bytes:
         """Get extended address (EUI-64).
 
         Raises if the http status is not 200 or if the response is invalid.
         """
         response = await self._session.get(
```

### Comparing `python-otbr-api-1.2.0/python_otbr_api/mdns.py` & `python-otbr-api-2.0.0/python_otbr_api/mdns.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.2.0/python_otbr_api/models.py` & `python-otbr-api-2.0.0/python_otbr_api/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -115,97 +115,129 @@
             json_data.get("RotationTime"),
             json_data.get("Routers"),
             json_data.get("TobleLink"),
         )
 
 
 @dataclass
-class OperationalDataSet:  # pylint: disable=too-many-instance-attributes
+class ActiveDataSet:  # pylint: disable=too-many-instance-attributes
     """Operational dataset."""
 
     SCHEMA = vol.Schema(
         {
             vol.Optional("ActiveTimestamp"): dict,
             vol.Optional("ChannelMask"): int,
             vol.Optional("Channel"): int,
-            vol.Optional("Delay"): int,
             vol.Optional("ExtPanId"): str,
             vol.Optional("MeshLocalPrefix"): str,
             vol.Optional("NetworkKey"): str,
             vol.Optional("NetworkName"): str,
             vol.Optional("PanId"): int,
-            vol.Optional("PendingTimestamp"): dict,
             vol.Optional("PSKc"): str,
             vol.Optional("SecurityPolicy"): dict,
         }
     )
 
     active_timestamp: Timestamp | None = None
     channel_mask: int | None = None
     channel: int | None = None
-    delay: int | None = None
     extended_pan_id: str | None = None
     mesh_local_prefix: str | None = None
     network_key: str | None = None
     network_name: str | None = None
     pan_id: int | None = None
-    pending_timestamp: Timestamp | None = None
     psk_c: str | None = None
     security_policy: SecurityPolicy | None = None
 
     def as_json(self) -> dict:
         """Serialize to JSON."""
         result: dict[str, Any] = {}
         if self.active_timestamp is not None:
             result["ActiveTimestamp"] = self.active_timestamp.as_json()
         if self.channel_mask is not None:
             result["ChannelMask"] = self.channel_mask
         if self.channel is not None:
             result["Channel"] = self.channel
-        if self.delay is not None:
-            result["Delay"] = self.delay
         if self.extended_pan_id is not None:
             result["ExtPanId"] = self.extended_pan_id
         if self.mesh_local_prefix is not None:
             result["MeshLocalPrefix"] = self.mesh_local_prefix
         if self.network_key is not None:
             result["NetworkKey"] = self.network_key
         if self.network_name is not None:
             result["NetworkName"] = self.network_name
         if self.pan_id is not None:
             result["PanId"] = self.pan_id
-        if self.pending_timestamp is not None:
-            result["PendingTimestamp"] = self.pending_timestamp.as_json()
         if self.psk_c is not None:
             result["PSKc"] = self.psk_c
         if self.security_policy is not None:
             result["SecurityPolicy"] = self.security_policy.as_json()
         return result
 
     @classmethod
-    def from_json(cls, json_data: Any) -> OperationalDataSet:
+    def from_json(cls, json_data: Any) -> ActiveDataSet:
         """Deserialize from JSON."""
         cls.SCHEMA(json_data)
         active_timestamp = None
-        pending_timestamp = None
         security_policy = None
         if "ActiveTimestamp" in json_data:
             active_timestamp = Timestamp.from_json(json_data["ActiveTimestamp"])
-        if "PendingTimestamp" in json_data:
-            pending_timestamp = Timestamp.from_json(json_data["PendingTimestamp"])
         if "SecurityPolicy" in json_data:
             security_policy = SecurityPolicy.from_json(json_data["SecurityPolicy"])
 
-        return OperationalDataSet(
+        return ActiveDataSet(
             active_timestamp,
             json_data.get("ChannelMask"),
             json_data.get("Channel"),
-            json_data.get("Delay"),
             json_data.get("ExtPanId"),
             json_data.get("MeshLocalPrefix"),
             json_data.get("NetworkKey"),
             json_data.get("NetworkName"),
             json_data.get("PanId"),
-            pending_timestamp,
             json_data.get("PSKc"),
             security_policy,
         )
+
+
+@dataclass
+class PendingDataSet:  # pylint: disable=too-many-instance-attributes
+    """Operational dataset."""
+
+    SCHEMA = vol.Schema(
+        {
+            vol.Optional("ActiveDataset"): dict,
+            vol.Optional("Delay"): int,
+            vol.Optional("PendingTimestamp"): dict,
+        }
+    )
+
+    active_dataset: ActiveDataSet | None = None
+    delay: int | None = None
+    pending_timestamp: Timestamp | None = None
+
+    def as_json(self) -> dict:
+        """Serialize to JSON."""
+        result: dict[str, Any] = {}
+        if self.active_dataset is not None:
+            result["ActiveDataset"] = self.active_dataset.as_json()
+        if self.delay is not None:
+            result["Delay"] = self.delay
+        if self.pending_timestamp is not None:
+            result["PendingTimestamp"] = self.pending_timestamp.as_json()
+        return result
+
+    @classmethod
+    def from_json(cls, json_data: Any) -> PendingDataSet:
+        """Deserialize from JSON."""
+        cls.SCHEMA(json_data)
+        active_dataset = None
+        pending_timestamp = None
+        if "ActiveDataset" in json_data:
+            active_dataset = ActiveDataSet.from_json(json_data["ActiveDataset"])
+        if "PendingTimestamp" in json_data:
+            pending_timestamp = Timestamp.from_json(json_data["PendingTimestamp"])
+
+        return PendingDataSet(
+            active_dataset,
+            json_data.get("Delay"),
+            pending_timestamp,
+        )
```

### Comparing `python-otbr-api-1.2.0/python_otbr_api/pskc.py` & `python-otbr-api-2.0.0/python_otbr_api/pskc.py`

 * *Files identical despite different names*

### Comparing `python-otbr-api-1.2.0/python_otbr_api/tlv_parser.py` & `python-otbr-api-2.0.0/python_otbr_api/tlv_parser.py`

 * *Files identical despite different names*


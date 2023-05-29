# Comparing `tmp/aioslimproto-2.2.0.tar.gz` & `tmp/aioslimproto-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioslimproto-2.2.0.tar", last modified: Tue Mar  7 21:41:11 2023, max compression
+gzip compressed data, was "aioslimproto-2.2.1.tar", last modified: Mon May 29 21:37:27 2023, max compression
```

## Comparing `aioslimproto-2.2.0.tar` & `aioslimproto-2.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:41:11.139468 aioslimproto-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-07 21:41:11.139468 aioslimproto-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:41:11.139468 aioslimproto-2.2.0/aioslimproto/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/aioslimproto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/aioslimproto/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30389 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/aioslimproto/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/aioslimproto/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/aioslimproto/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/aioslimproto/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/aioslimproto/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/aioslimproto/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 21:41:11.139468 aioslimproto-2.2.0/aioslimproto.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-03-07 21:41:11.000000 aioslimproto-2.2.0/aioslimproto.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-07 21:41:11.000000 aioslimproto-2.2.0/aioslimproto.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 21:41:11.000000 aioslimproto-2.2.0/aioslimproto.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-07 21:41:11.000000 aioslimproto-2.2.0/aioslimproto.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 21:41:11.000000 aioslimproto-2.2.0/aioslimproto.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-07 21:41:11.139468 aioslimproto-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-07 21:41:00.000000 aioslimproto-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:37:27.813711 aioslimproto-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-29 21:37:27.813711 aioslimproto-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:37:27.813711 aioslimproto-2.2.1/aioslimproto/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22638 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30608 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7385 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6000 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/aioslimproto/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 21:37:27.813711 aioslimproto-2.2.1/aioslimproto.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 21:37:27.000000 aioslimproto-2.2.1/aioslimproto.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-29 21:37:27.813711 aioslimproto-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-29 21:37:14.000000 aioslimproto-2.2.1/setup.py
```

### Comparing `aioslimproto-2.2.0/LICENSE` & `aioslimproto-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.0/PKG-INFO` & `aioslimproto-2.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslimproto
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python module to talk to Logitech Squeezebox players directly (without Logitech server).
 Home-page: https://github.com/music-assistant/aioslimproto
 Author: Marcel van der Veldt
 Author-email: marcelveldt@users.noreply.github.com
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioslimproto-2.2.0/aioslimproto/cli.py` & `aioslimproto-2.2.1/aioslimproto/cli.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.0/aioslimproto/client.py` & `aioslimproto-2.2.1/aioslimproto/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import time
 from asyncio import StreamReader, StreamWriter, create_task
 from collections import deque
 from enum import Enum
 from typing import Callable, Dict, List, TypedDict
 from urllib.parse import parse_qsl, urlparse
 
+from async_timeout import timeout
+
 from .const import EventType
 from .errors import UnsupportedContentType
 from .util import parse_capabilities, parse_headers
 
 # from http://wiki.slimdevices.com/index.php/SlimProtoTCPProtocol#HELO
 DEVICE_TYPE = {
     2: "squeezebox",
@@ -121,14 +123,15 @@
     "aif": b"p",
 }
 
 FALLBACK_MODEL = "Squeezebox"
 FALLLBACK_FIRMWARE = "Unknown"
 FALLBACK_CODECS = ["pcm"]
 FALLBACK_SAMPLE_RATE = 96000
+HEARTBEAT_INTERVAL = 5
 
 
 class Metadata(TypedDict):
     """Optional metadata for playback."""
 
     item_id: str  # optional
     artist: str  # optional
@@ -168,24 +171,23 @@
         self._connected: bool = False
         self._last_heartbeat = (0, 0)
         self._packet_latency = deque(maxlen=10)
         self._reader_task = create_task(self._socket_reader())
         self._send_heartbeat()
 
     def disconnect(self) -> None:
-        """Disconnect socket client."""
-        if self._reader_task and not self._reader_task.cancelled():
+        """Disconnect and/or cleanup socket client."""
+        if self._reader_task and not self._reader_task.done():
             self._reader_task.cancel()
 
         if self._connected:
             self._connected = False
             if self._writer.can_write_eof():
                 self._writer.write_eof()
             self._writer.close()
-            self.callback(EventType.PLAYER_DISCONNECTED, self)
 
     @property
     def connected(self) -> bool:
         """Return connection state of the socket."""
         return self._connected
 
     @property
@@ -309,15 +311,15 @@
         )
         self.callback(EventType.PLAYER_UPDATED, self)
 
     async def mute(self, muted: bool = False) -> None:
         """Send mute command to player."""
         muted_int = 0 if muted else 1
         await self._send_frame(b"aude", struct.pack("2B", muted_int, 0))
-        self.muted = muted
+        self._muted = muted
         self.callback(EventType.PLAYER_UPDATED, self)
 
     async def play_url(
         self,
         url: str,
         mime_type: str | None = None,
         metadata: Metadata | None = None,
@@ -404,15 +406,15 @@
             trans_duration=transition_duration,
             trans_type=transition.value,
             flags=0x20 if scheme == "https" else 0x00,
             httpreq=httpreq,
         )
 
     def _send_heartbeat(self) -> None:
-        """Send (periodic) heartbeat message to player."""
+        """Send heartbeat message to player."""
 
         async def async_send_heartbeat():
             heartbeat_id = self._last_heartbeat[0] + 1
             self._last_heartbeat = (heartbeat_id, time.time())
             await self.send_strm(b"t", flags=0, replay_gain=heartbeat_id)
 
         asyncio.create_task(async_send_heartbeat())
@@ -431,15 +433,19 @@
             self.disconnect()
 
     async def _socket_reader(self) -> None:
         """Handle incoming data from socket."""
         buffer = b""
         # keep reading bytes from the socket
         while not (self._reader.at_eof() or self._writer.is_closing()):
-            data = await self._reader.read(64)
+            try:
+                async with timeout(HEARTBEAT_INTERVAL * 2):
+                    data = await self._reader.read(64)
+            except asyncio.TimeoutError:
+                break
             # handle incoming data from socket
             buffer = buffer + data
             del data
             if len(buffer) > 8:
                 # construct operation and
                 operation, length = buffer[:4], buffer[4:8]
                 plen = struct.unpack("!I", length)[0] + 8
@@ -453,14 +459,15 @@
                         create_task(handler(packet))
                     else:
                         asyncio.get_running_loop().call_soon(handler, packet)
         # EOF reached: socket is disconnected
         self.logger.debug(
             "Socket disconnected: %s", self._writer.get_extra_info("peername")
         )
+        self.callback(EventType.PLAYER_DISCONNECTED, self)
         self.disconnect()
 
     async def send_strm(
         self,
         command=b"q",
         formatbyte=b"?",
         autostart=b"0",
@@ -635,15 +642,15 @@
             # if playback busy we want high accuracy
             # but otherwise every 5 seconds is good enough
             if self.state == PlayerState.PLAYING:
                 heartbeat_delay = 0.1
             elif self.powered:
                 heartbeat_delay = 1
             else:
-                heartbeat_delay = 5
+                heartbeat_delay = HEARTBEAT_INTERVAL
             asyncio.get_event_loop().call_later(heartbeat_delay, self._send_heartbeat)
 
         self._elapsed_milliseconds = elapsed_milliseconds
         # consider latency when calculating the elapsed time
         self._last_timestamp = time.time() - self.packet_latency
         self.callback(EventType.PLAYER_HEARTBEAT, self)
```

### Comparing `aioslimproto-2.2.0/aioslimproto/const.py` & `aioslimproto-2.2.1/aioslimproto/const.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.0/aioslimproto/discovery.py` & `aioslimproto-2.2.1/aioslimproto/discovery.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.0/aioslimproto/server.py` & `aioslimproto-2.2.1/aioslimproto/server.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.0/aioslimproto/util.py` & `aioslimproto-2.2.1/aioslimproto/util.py`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.0/aioslimproto.egg-info/PKG-INFO` & `aioslimproto-2.2.1/aioslimproto.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioslimproto
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python module to talk to Logitech Squeezebox players directly (without Logitech server).
 Home-page: https://github.com/music-assistant/aioslimproto
 Author: Marcel van der Veldt
 Author-email: marcelveldt@users.noreply.github.com
 License: Apache License 2.0
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `aioslimproto-2.2.0/setup.cfg` & `aioslimproto-2.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `aioslimproto-2.2.0/setup.py` & `aioslimproto-2.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README_FILE = PROJECT_DIR / "README.md"
 REQUIREMENTS_FILE = PROJECT_DIR / "requirements.txt"
 PACKAGES = find_packages(exclude=["tests", "tests.*"])
 PROJECT_REQ_PYTHON_VERSION = "3.9"
 
 setup(
     name="aioslimproto",
-    version="2.2.0",
+    version="2.2.1",
     license="Apache License 2.0",
     url="https://github.com/music-assistant/aioslimproto",
     author="Marcel van der Veldt",
     author_email="marcelveldt@users.noreply.github.com",
     description="Python module to talk to Logitech Squeezebox players directly (without Logitech server).",
     long_description=README_FILE.read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
```


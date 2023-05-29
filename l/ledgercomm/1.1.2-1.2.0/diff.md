# Comparing `tmp/ledgercomm-1.1.2.tar.gz` & `tmp/ledgercomm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledgercomm-1.1.2.tar", last modified: Mon Nov 21 13:58:50 2022, max compression
+gzip compressed data, was "ledgercomm-1.2.0.tar", last modified: Mon May 29 16:09:59 2023, max compression
```

## Comparing `ledgercomm-1.1.2.tar` & `ledgercomm-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:58:50.652577 ledgercomm-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)     4594 2022-11-21 13:58:50.652577 ledgercomm-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3094 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:58:50.652577 ledgercomm-1.1.2/ledgercomm/
--rw-r--r--   0 runner    (1001) docker     (121)      117 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/ledgercomm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:58:50.652577 ledgercomm-1.1.2/ledgercomm/cli/
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/ledgercomm/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2921 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/ledgercomm/cli/send.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:58:50.652577 ledgercomm-1.1.2/ledgercomm/interfaces/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/ledgercomm/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      922 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/ledgercomm/interfaces/comm.py
--rw-r--r--   0 runner    (1001) docker     (121)     5074 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/ledgercomm/interfaces/hid_device.py
--rw-r--r--   0 runner    (1001) docker     (121)     3027 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/ledgercomm/interfaces/tcp_client.py
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/ledgercomm/log.py
--rw-r--r--   0 runner    (1001) docker     (121)     7377 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/ledgercomm/transport.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 13:58:50.652577 ledgercomm-1.1.2/ledgercomm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4594 2022-11-21 13:58:50.000000 ledgercomm-1.1.2/ledgercomm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-11-21 13:58:50.000000 ledgercomm-1.1.2/ledgercomm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 13:58:50.000000 ledgercomm-1.1.2/ledgercomm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-11-21 13:58:50.000000 ledgercomm-1.1.2/ledgercomm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-21 13:58:50.000000 ledgercomm-1.1.2/ledgercomm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-21 13:58:50.000000 ledgercomm-1.1.2/ledgercomm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 13:58:50.000000 ledgercomm-1.1.2/ledgercomm.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-21 13:58:50.652577 ledgercomm-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1178 2022-11-21 13:58:39.000000 ledgercomm-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:09:59.335935 ledgercomm-1.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:09:59.331935 ledgercomm-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:09:59.331935 ledgercomm-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/.github/workflows/python-fast-checks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-29 16:09:59.335935 ledgercomm-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:09:59.331935 ledgercomm-1.2.0/ledgercomm/
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/ledgercomm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 16:09:59.000000 ledgercomm-1.2.0/ledgercomm/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:09:59.335935 ledgercomm-1.2.0/ledgercomm/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/ledgercomm/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2964 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/ledgercomm/cli/send.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:09:59.335935 ledgercomm-1.2.0/ledgercomm/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/ledgercomm/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/ledgercomm/interfaces/comm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/ledgercomm/interfaces/hid_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/ledgercomm/interfaces/tcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/ledgercomm/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/ledgercomm/transport.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:09:59.335935 ledgercomm-1.2.0/ledgercomm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-29 16:09:59.000000 ledgercomm-1.2.0/ledgercomm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-29 16:09:59.000000 ledgercomm-1.2.0/ledgercomm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:09:59.000000 ledgercomm-1.2.0/ledgercomm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-29 16:09:59.000000 ledgercomm-1.2.0/ledgercomm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-29 16:09:59.000000 ledgercomm-1.2.0/ledgercomm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 16:09:59.000000 ledgercomm-1.2.0/ledgercomm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:09:59.000000 ledgercomm-1.2.0/ledgercomm.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-29 16:09:45.000000 ledgercomm-1.2.0/requirements-opt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 16:09:59.335935 ledgercomm-1.2.0/setup.cfg
```

### Comparing `ledgercomm-1.1.2/LICENCE` & `ledgercomm-1.2.0/LICENCE`

 * *Files identical despite different names*

### Comparing `ledgercomm-1.1.2/README.md` & `ledgercomm-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `ledgercomm-1.1.2/ledgercomm/cli/send.py` & `ledgercomm-1.2.0/ledgercomm/cli/send.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ledgercomm.cli.send module."""
 
 import argparse
 from pathlib import Path
 import re
 from typing import Iterator, Optional
 
-from ledgercomm import Transport
+from ledgercomm import Transport, __version__
 
 
 def parse_file(filepath: Path, condition: Optional[str]) -> Iterator[str]:
     """Filter with `condition` and yield line of `filepath`."""
     with open(filepath, "r", encoding="utf-8") as f:
         for line in f:
             if condition and line.startswith(condition):
@@ -17,70 +17,46 @@
             else:
                 yield line.strip()
 
 
 def main():
     """Entrypoint of ledgercomm-parse binary."""
     parser = argparse.ArgumentParser()
-    subparsers = parser.add_subparsers(
-        help="sub-command help",
-        dest="command"
-    )
+    subparsers = parser.add_subparsers(help="sub-command help", dest="command")
     # file subparser
-    parser_file = subparsers.add_parser(
-        "file",
-        help="send APDUs from file"
-    )
-    parser_file.add_argument(
-        "filepath",
-        help="path of the file within APDUs"
-    )
+    parser_file = subparsers.add_parser("file", help="send APDUs from file")
+    parser_file.add_argument("filepath", help="path of the file within APDUs")
     # stdin subparser
-    _ = subparsers.add_parser(
-        "stdin",
-        help="send APDUs from stdin"
-    )
+    _ = subparsers.add_parser("stdin", help="send APDUs from stdin")
     # stdin subparser
-    parser_log = subparsers.add_parser(
-        "log",
-        help="send APDUs from Ledger Live log file"
-    )
-    parser_log.add_argument(
-        "filepath",
-        help="path of the Ledger Live log file within APDUs"
-    )
+    parser_log = subparsers.add_parser("log", help="send APDUs from Ledger Live log file")
+    parser_log.add_argument("filepath", help="path of the Ledger Live log file within APDUs")
     # args for main parser
-    parser.add_argument(
-        "--hid",
-        help="Use HID instead of TCP client",
-        action="store_true"
-    )
-    parser.add_argument(
-        "--server",
-        help="IP server of the TCP client (default: 127.0.0.1)",
-        default="127.0.0.1"
-    )
-    parser.add_argument(
-        "--port",
-        help="Port of the TCP client (default: 9999)",
-        default=9999
-    )
-    parser.add_argument(
-        "--startswith",
-        help="Only send APDUs which starts with STARTSWITH (default: None)",
-        default=None
-    )
+    parser.add_argument("--hid", help="Use HID instead of TCP client", action="store_true")
+    parser.add_argument("--server",
+                        help="IP server of the TCP client (default: 127.0.0.1)",
+                        default="127.0.0.1")
+    parser.add_argument("--port", help="Port of the TCP client (default: 9999)", default=9999)
+    parser.add_argument("--startswith",
+                        help="Only send APDUs which starts with STARTSWITH (default: None)",
+                        default=None)
+    parser.add_argument("--version",
+                        "-v",
+                        help="Print LedgerComm package current version",
+                        default=False,
+                        action="store_true")
 
     args = parser.parse_args()
 
-    transport = (Transport(interface="hid", debug=True) if args.hid
-                 else Transport(interface="tcp",
-                                server=args.server,
-                                port=args.port,
-                                debug=True))
+    if args.version:
+        print(__version__)
+        return 0
+
+    transport = (Transport(interface="hid", debug=True) if args.hid else Transport(
+        interface="tcp", server=args.server, port=args.port, debug=True))
 
     if args.command == "file":
         filepath: Path = Path(args.filepath)
 
         for apdu in parse_file(filepath, args.startswith):  # type: str
             if apdu:
                 transport.exchange_raw(re.sub(r"[^a-fA-F0-9]", "", apdu))
```

### Comparing `ledgercomm-1.1.2/ledgercomm/interfaces/comm.py` & `ledgercomm-1.2.0/ledgercomm/interfaces/comm.py`

 * *Files identical despite different names*

### Comparing `ledgercomm-1.1.2/ledgercomm/interfaces/hid_device.py` & `ledgercomm-1.2.0/ledgercomm/interfaces/hid_device.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,16 +77,15 @@
 
         for hid_device in hid.enumerate(vendor_id, 0):
             if (hid_device.get("interface_number") == 0 or
                     # MacOS specific
                     hid_device.get("usage_page") == 0xffa0):
                 devices.append(hid_device["path"])
 
-        assert len(devices) != 0, (
-            f"Can't find Ledger device with vendor_id {hex(vendor_id)}")
+        assert len(devices) != 0, f"Can't find Ledger device with vendor_id {hex(vendor_id)}"
 
         return devices
 
     def send(self, data: bytes) -> int:
         """Send `data` through HID device `self.device`.
 
         Parameters
@@ -97,28 +96,27 @@
         Returns
         -------
         int
             Total length of data sent to the device.
 
         """
         if not data:
-            raise Exception("Can't send empty data!")
+            raise ValueError("Can't send empty data!")
 
         LOG.debug("=> %s", data.hex())
 
         data = int.to_bytes(len(data), 2, byteorder="big") + data
         offset: int = 0
         seq_idx: int = 0
         length: int = 0
 
         while offset < len(data):
             # Header: channel (0x0101), tag (0x05), sequence index
             header: bytes = b"\x01\x01\x05" + seq_idx.to_bytes(2, byteorder="big")
-            data_chunk: bytes = (header +
-                                 data[offset:offset + 64 - len(header)])
+            data_chunk: bytes = header + data[offset:offset + 64 - len(header)]
 
             self.device.write(b"\x00" + data_chunk)
             length += len(data_chunk) + 1
             offset += 64 - len(header)
             seq_idx += 1
 
         return length
```

### Comparing `ledgercomm-1.1.2/ledgercomm/interfaces/tcp_client.py` & `ledgercomm-1.2.0/ledgercomm/interfaces/tcp_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,15 @@
         Returns
         -------
         int
             Total lenght of data sent through TCP socket.
 
         """
         if not data:
-            raise Exception("Can't send empty data!")
+            raise ValueError("Can't send empty data!")
 
         LOG.debug("=> %s", data.hex())
         data_len: bytes = int.to_bytes(len(data), 4, byteorder="big")
 
         return self.socket.send(data_len + data)
 
     def recv(self) -> Tuple[int, bytes]:
```

### Comparing `ledgercomm-1.1.2/ledgercomm/transport.py` & `ledgercomm-1.2.0/ledgercomm/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,19 +65,18 @@
             LOG.addHandler(ch)
 
         self.interface: TransportType
 
         try:
             self.interface = TransportType[interface.upper()]
         except KeyError as exc:
-            raise Exception(f"Unknown interface '{interface}'!") from exc
+            raise KeyError(f"Unknown interface '{interface}'!") from exc
 
         self.com: Union[TCPClient, HID] = (TCPClient(server=server, port=port)
-                                           if self.interface == TransportType.TCP
-                                           else HID())
+                                           if self.interface == TransportType.TCP else HID())
 
         self.com.open()
 
     @staticmethod
     def apdu_header(cla: int,
                     ins: Union[int, enum.IntEnum],
                     p1: int = 0,
@@ -106,28 +105,24 @@
         bytes
             APDU header packed with parameters.
 
         """
         ins = cast(int, ins.value) if isinstance(ins, enum.IntEnum) else cast(int, ins)
 
         if opt:
-            return struct.pack("BBBBBB",
-                               cla,
-                               ins,
-                               p1,
-                               p2,
-                               1 + lc,  # add option to length
-                               opt)
-
-        return struct.pack("BBBBB",
-                           cla,
-                           ins,
-                           p1,
-                           p2,
-                           lc)
+            return struct.pack(
+                "BBBBBB",
+                cla,
+                ins,
+                p1,
+                p2,
+                1 + lc,  # add option to length
+                opt)
+
+        return struct.pack("BBBBB", cla, ins, p1, p2, lc)
 
     def send(self,
              cla: int,
              ins: Union[int, enum.IntEnum],
              p1: int = 0,
              p2: int = 0,
              option: Optional[int] = None,
```

### Comparing `ledgercomm-1.1.2/ledgercomm.egg-info/SOURCES.txt` & `ledgercomm-1.2.0/ledgercomm.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,18 @@
+.gitignore
+CHANGELOG.md
 LICENCE
 README.md
+pyproject.toml
+requirements-dev.txt
+requirements-opt.txt
 setup.cfg
-setup.py
+.github/workflows/python-fast-checks.yml
 ledgercomm/__init__.py
+ledgercomm/__version__.py
 ledgercomm/log.py
 ledgercomm/transport.py
 ledgercomm.egg-info/PKG-INFO
 ledgercomm.egg-info/SOURCES.txt
 ledgercomm.egg-info/dependency_links.txt
 ledgercomm.egg-info/entry_points.txt
 ledgercomm.egg-info/requires.txt
```


# Comparing `tmp/ledgerwallet-0.1.4.tar.gz` & `tmp/ledgerwallet-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ledgerwallet-0.1.4.tar", last modified: Mon Sep 26 12:20:09 2022, max compression
+gzip compressed data, was "ledgerwallet-0.3.0.tar", last modified: Mon May 29 16:10:22 2023, max compression
```

## Comparing `ledgerwallet-0.1.4.tar` & `ledgerwallet-0.3.0.tar`

### file list

```diff
@@ -1,38 +1,76 @@
-drwxrwxrwx   0        0        0        0 2022-09-26 12:20:09.383597 ledgerwallet-0.1.4/
--rw-rw-rw-   0        0        0     1063 2022-06-30 11:21:42.000000 ledgerwallet-0.1.4/LICENSE
--rw-rw-rw-   0        0        0     6193 2022-09-26 12:20:09.384584 ledgerwallet-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     5345 2022-09-12 12:33:08.000000 ledgerwallet-0.1.4/README.md
--rw-rw-rw-   0        0        0    10634 2022-09-12 12:33:08.000000 ledgerwallet-0.1.4/ledgerctl.py
-drwxrwxrwx   0        0        0        0 2022-09-26 12:20:09.264620 ledgerwallet-0.1.4/ledgerwallet/
--rw-rw-rw-   0        0        0       22 2022-07-01 07:39:27.000000 ledgerwallet-0.1.4/ledgerwallet/__init__.py
--rw-rw-rw-   0        0        0    16055 2022-09-12 12:33:08.000000 ledgerwallet-0.1.4/ledgerwallet/client.py
-drwxrwxrwx   0        0        0        0 2022-09-26 12:20:09.320583 ledgerwallet-0.1.4/ledgerwallet/crypto/
--rw-rw-rw-   0        0        0        0 2022-06-30 11:21:42.000000 ledgerwallet-0.1.4/ledgerwallet/crypto/__init__.py
--rw-rw-rw-   0        0        0     2214 2022-07-01 07:39:27.000000 ledgerwallet-0.1.4/ledgerwallet/crypto/ecc.py
--rw-rw-rw-   0        0        0     4097 2022-06-30 11:21:42.000000 ledgerwallet-0.1.4/ledgerwallet/crypto/scp.py
--rw-rw-rw-   0        0        0      374 2022-06-30 11:21:42.000000 ledgerwallet-0.1.4/ledgerwallet/hsmscript.py
--rw-rw-rw-   0        0        0     2629 2022-09-12 12:33:08.000000 ledgerwallet-0.1.4/ledgerwallet/hsmserver.py
--rw-rw-rw-   0        0        0      412 2022-09-12 12:33:08.000000 ledgerwallet-0.1.4/ledgerwallet/ledgerserver.py
--rw-rw-rw-   0        0        0     5468 2022-09-12 12:33:08.000000 ledgerwallet-0.1.4/ledgerwallet/manifest.py
--rw-rw-rw-   0        0        0     4910 2022-09-12 12:33:08.000000 ledgerwallet-0.1.4/ledgerwallet/params.py
-drwxrwxrwx   0        0        0        0 2022-09-26 12:20:09.341583 ledgerwallet-0.1.4/ledgerwallet/proto/
--rw-rw-rw-   0        0        0     1659 2022-07-01 07:39:27.000000 ledgerwallet-0.1.4/ledgerwallet/proto/LedgerHSMServer_pb2.py
--rw-rw-rw-   0        0        0        0 2022-06-30 11:21:42.000000 ledgerwallet-0.1.4/ledgerwallet/proto/__init__.py
--rw-rw-rw-   0        0        0     1188 2022-07-01 07:39:27.000000 ledgerwallet-0.1.4/ledgerwallet/proto/listApps_pb2.py
--rw-rw-rw-   0        0        0     3969 2022-09-12 12:33:08.000000 ledgerwallet-0.1.4/ledgerwallet/simpleserver.py
-drwxrwxrwx   0        0        0        0 2022-09-26 12:20:09.381585 ledgerwallet-0.1.4/ledgerwallet/transport/
--rw-rw-rw-   0        0        0      237 2022-07-22 09:30:37.000000 ledgerwallet-0.1.4/ledgerwallet/transport/__init__.py
--rw-rw-rw-   0        0        0      621 2022-09-12 12:33:08.000000 ledgerwallet-0.1.4/ledgerwallet/transport/device.py
--rw-rw-rw-   0        0        0     2854 2022-07-22 09:30:37.000000 ledgerwallet-0.1.4/ledgerwallet/transport/hid.py
--rw-rw-rw-   0        0        0     1362 2022-07-22 09:30:37.000000 ledgerwallet-0.1.4/ledgerwallet/transport/tcp.py
--rw-rw-rw-   0        0        0     1900 2022-09-12 12:33:08.000000 ledgerwallet-0.1.4/ledgerwallet/utils.py
-drwxrwxrwx   0        0        0        0 2022-09-26 12:20:09.299585 ledgerwallet-0.1.4/ledgerwallet.egg-info/
--rw-rw-rw-   0        0        0     6193 2022-09-26 12:20:09.000000 ledgerwallet-0.1.4/ledgerwallet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      832 2022-09-26 12:20:09.000000 ledgerwallet-0.1.4/ledgerwallet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-26 12:20:09.000000 ledgerwallet-0.1.4/ledgerwallet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2022-09-26 12:20:09.000000 ledgerwallet-0.1.4/ledgerwallet.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      107 2022-09-26 12:20:09.000000 ledgerwallet-0.1.4/ledgerwallet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2022-09-26 12:20:09.000000 ledgerwallet-0.1.4/ledgerwallet.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-01 07:39:27.000000 ledgerwallet-0.1.4/pyproject.toml
--rw-rw-rw-   0        0        0      126 2022-09-26 12:20:09.390584 ledgerwallet-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1833 2022-09-26 12:12:56.000000 ledgerwallet-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.893453 ledgerwallet-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.885453 ledgerwallet-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.889454 ledgerwallet-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-29 16:10:22.893453 ledgerwallet-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5432 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.889454 ledgerwallet-0.3.0/ledgerwallet/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-29 16:10:22.000000 ledgerwallet-0.3.0/ledgerwallet/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.889454 ledgerwallet-0.3.0/ledgerwallet/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/crypto/ecc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/crypto/scp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/hsmscript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/hsmserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11717 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/ledgerctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/ledgerserver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/manifest_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/manifest_toml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/params.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.889454 ledgerwallet-0.3.0/ledgerwallet/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/proto/LedgerHSMServer.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/proto/LedgerHSMServer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/proto/LedgerHSMServer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/proto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/proto/listApps.proto
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/proto/listApps_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/proto/listApps_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/simpleserver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.893453 ledgerwallet-0.3.0/ledgerwallet/transport/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/transport/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/transport/hid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/transport/tcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/ledgerwallet/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.889454 ledgerwallet-0.3.0/ledgerwallet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7378 2023-05-29 16:10:22.000000 ledgerwallet-0.3.0/ledgerwallet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-05-29 16:10:22.000000 ledgerwallet-0.3.0/ledgerwallet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 16:10:22.000000 ledgerwallet-0.3.0/ledgerwallet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-29 16:10:22.000000 ledgerwallet-0.3.0/ledgerwallet.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-29 16:10:22.000000 ledgerwallet-0.3.0/ledgerwallet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 16:10:22.000000 ledgerwallet-0.3.0/ledgerwallet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-29 16:10:22.893453 ledgerwallet-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.885453 ledgerwallet-0.3.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.893453 ledgerwallet-0.3.0/tests/app/
+-rw-r--r--   0 runner    (1001) docker     (123)    53376 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/app/app.hex
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/app/app.json
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/app/app.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/app/nanos_app_ssh.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.893453 ledgerwallet-0.3.0/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.893453 ledgerwallet-0.3.0/tests/unit/crypto/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/crypto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/crypto/test_ecc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:22.893453 ledgerwallet-0.3.0/tests/unit/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/data/empty_manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/data/empty_manifest.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/data/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/data/manifest.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/data/minimal_manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/data/minimal_manifest.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/data/missing_binary_manifest.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/test_manifest_ManifestJSON.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/test_manifest_ManifestTOML.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6288 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-29 16:10:10.000000 ledgerwallet-0.3.0/tests/unit/test_utils.py
```

### Comparing `ledgerwallet-0.1.4/LICENSE` & `ledgerwallet-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/README.md` & `ledgerwallet-0.3.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -97,29 +97,33 @@
 ```shell
 python3 -m ledgerblue.loadApp --curve secp256k1 --tlv --targetId 0x31100004 --targetVersion="1.6.0" --delete --fileName bin/app.hex --appName "Bitcoin" --appVersion 1.3.13 --dataSize $((0x`cat debug/app.map |grep _envram_data | tr -s ' ' | cut -f2 -d' '|cut -f2 -d'x'` - 0x`cat debug/app.map |grep _nvram_data | tr -s ' ' | cut -f2 -d' '|cut -f2 -d'x'`)) `ICONHEX=\`python3 /home/dev/sdk/icon3.py --hexbitmaponly nanos_app_bitcoin.gif  2>/dev/null\` ; [ ! -z "$ICONHEX" ] && echo "--icon $ICONHEX"`  --path "" --appFlags 0xa50 --offline bin/app.apdu | grep "Application" | cut -f5 -d' ' > bin/app.sha256
 ```
 
 To install it with ledgerctl:
 
 1. Retrieve `dataSize` using the above one-liner.
-2. Create a manifest file app.json in the ledger-app-btc directory:
+2. Create a manifest file app.toml in the ledger-app-btc directory:
 
-```json
-{
-    "name": "Bitcoin",
-    "version": "1.3.13",
-    "icon": "nanos_app_bitcoin.gif",
-    "targetId": "0x31100004",
-    "flags": "0xA50",
-    "derivationPath": {
-        "curves": ["secp256k1"]
-    },
-    "binary": "bin/app.hex",
-    "dataSize": 64
-}
+```toml
+name = "Bitcoin"
+version = "1.3.13"
+
+[0x31100004] #NanoS
+icon = "nanos_app_bitcoin.gif"
+flags = "0xA50"
+derivationPath = {curves = ["secp256k1"]}
+binary = "bin/app.hex"
+dataSize = 64
+
+[0x33100004] #NanoSP
+icon = "nanosp_app_bitcoin.gif"
+flags = "0xA50"
+derivationPath = {curves = ["secp256k1"]}
+binary = "bin/app_nanosp.hex"
+dataSize = 64
 ```
 
 3. Install with `ledgerctl install app.json`.
 
 If you want to force the deletion of the previous version, run the previous command with the `-f` flag.
 
 ### Viewing APDUs
```

### Comparing `ledgerwallet-0.1.4/ledgerctl.py` & `ledgerwallet-0.3.0/ledgerwallet/ledgerctl.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,48 @@
 import configparser
 import os
 import re
 import sys
+from json import JSONDecodeError
 
 import click
 from tabulate import tabulate
 
+if sys.version_info >= (3, 11):
+    from tomllib import TOMLDecodeError
+else:
+    from toml.decoder import TomlDecodeError as TOMLDecodeError
+
 from ledgerwallet import utils
 from ledgerwallet.client import (
     LEDGER_HSM_KEY,
     LEDGER_HSM_URL,
     CommException,
     LedgerClient,
     LedgerIns,
     NoLedgerDeviceException,
 )
 from ledgerwallet.crypto.ecc import PrivateKey
 from ledgerwallet.manifest import AppManifest
+from ledgerwallet.manifest_json import AppManifestJson
+from ledgerwallet.manifest_toml import AppManifestToml
+
+
+class ManifestFormatError(Exception):
+    def __init__(
+        self, toml_error: TOMLDecodeError, json_error: JSONDecodeError
+    ) -> None:
+        self.toml = toml_error
+        self.json = json_error
+
+    def __str__(self) -> str:
+        return "TOML or JSON is expected\nTOML error : {}\nJSON error : {}".format(
+            self.toml, self.json
+        )
+
 
 _remote_options = [
     click.option("--url", type=str, default=LEDGER_HSM_URL, help="Server URL."),
     click.option(
         "--key",
         "-k",
         type=str,
@@ -139,18 +161,30 @@
     "--force",
     help="Delete using application hash instead of application name",
     is_flag=True,
 )
 @click.pass_obj
 def install_app(get_client, manifest: AppManifest, force):
     client = get_client()
-    app_manifest = AppManifest(manifest)
+    try:
+        app_manifest: AppManifest = AppManifestToml(manifest)
+    except TOMLDecodeError as toml_error:
+        try:
+            app_manifest = AppManifestJson(manifest)
+            click.echo(
+                "[WARNING] JSON files will be deprecated in future version", err=True
+            )
+        except JSONDecodeError as json_error:
+            raise ManifestFormatError(toml_error, json_error)
+
     try:
         if force:
             client.delete_app(app_manifest.app_name)
+            client.close()
+            client = get_client()
         client.install_app(app_manifest)
     except CommException as e:
         if e.sw == 0x6985:
             click.echo("Operation has been canceled by the user.")
         elif e.sw == 0x6A80:
             click.echo("An application with the same name is already installed.")
         elif e.sw == 0x6A81:
```

### Comparing `ledgerwallet-0.1.4/ledgerwallet/client.py` & `ledgerwallet-0.3.0/ledgerwallet/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -297,29 +297,46 @@
     def _load_segment(self, hex_file: IntelHex, segment):
         start_addr, end_addr = segment
         # Load each segment by chunks of 64kB
         for offset in range(0, end_addr - start_addr, MAX_CHUNK_SIZE):
             self._load_chunk(hex_file, segment, offset)
 
     def install_app(self, app_manifest: AppManifest):
-        hex_file = IntelHex(app_manifest.get_binary())
+        version_info = self.get_version_info()
+        device = str(version_info.target_id)
+
+        app_manifest.assert_compatible_device(version_info.target_id)
+
+        hex_file = IntelHex(app_manifest.get_binary(device))
         code_length = hex_file.maxaddr() - hex_file.minaddr() + 1
-        data_length = app_manifest.data_size
+        data_length = app_manifest.data_size(device)
 
         code_length -= data_length
         assert code_length % 64 == 0  # code length must be aligned
 
-        flags = app_manifest.get_application_flags()  # not handled yet
+        flags = app_manifest.get_application_flags(device)  # not handled yet
 
-        params = app_manifest.serialize_parameters()
+        params = app_manifest.serialize_parameters(device)
         main_address = hex_file.start_addr["EIP"] - hex_file.minaddr()
 
-        data = struct.pack(
-            ">IIIII", code_length, data_length, len(params), flags, main_address
-        )
+        level = app_manifest.get_api_level(device)
+        if level:
+            data = struct.pack(
+                ">BIIIII",
+                level,
+                code_length,
+                data_length,
+                len(params),
+                flags,
+                main_address,
+            )
+        else:
+            data = struct.pack(
+                ">IIIII", code_length, data_length, len(params), flags, main_address
+            )
         self.apdu_secure_exchange(LedgerSecureIns.CREATE_APP, data)
 
         hex_file.puts(hex_file.maxaddr() + 1, params)
         for segment in hex_file.segments():
             self._load_segment(hex_file, segment)
         self.apdu_secure_exchange(LedgerSecureIns.COMMIT)
```

### Comparing `ledgerwallet-0.1.4/ledgerwallet/crypto/ecc.py` & `ledgerwallet-0.3.0/ledgerwallet/crypto/ecc.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/ledgerwallet/crypto/scp.py` & `ledgerwallet-0.3.0/ledgerwallet/crypto/scp.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/ledgerwallet/hsmserver.py` & `ledgerwallet-0.3.0/ledgerwallet/hsmserver.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/ledgerwallet/manifest.py` & `ledgerwallet-0.3.0/ledgerwallet/manifest.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import collections
 import colorsys
-import json
 import math
-import os
+from abc import ABC, abstractmethod
 from typing import Dict, List, Optional
 
 from PIL import Image
 
 from ledgerwallet import params
 
 MAX_COLORS = 16
@@ -95,72 +94,59 @@
     for i in range(num_colors):
         header += new_palette[i].to_bytes(4, "big")
 
     image_data = _image_to_packed_buffer(im, new_indices, bits_per_pixel)
     return header + image_data
 
 
-class AppManifest(object):
-    def __init__(self, filename):
-        with open(filename) as f:
-            self.path = os.path.dirname(filename)
-            self.json = json.load(f)
-            assert "targetId" in self.json and "binary" in self.json
+class AppManifest(ABC):
+    dic: Dict = {}
 
     @property
     def app_name(self) -> str:
-        return self.json["name"]
+        return self.dic.get("name", "")
 
-    @property
-    def data_size(self) -> int:
-        if "dataSize" not in self.json:
-            return 0
-        else:
-            return self.json["dataSize"]
-
-    def get_application_flags(self) -> int:
-        if "flags" not in self.json:
-            return 0
-        else:
-            return int(self.json["flags"], 16)
-
-    def get_binary(self) -> str:
-        return os.path.join(self.path, self.json["binary"])
-
-    def get_target_id(self) -> int:
-        return int(self.json["targetId"], 16)
-
-    def serialize_parameters(self) -> bytes:
-        parameters = []
-        for entry, value in self.json.items():
-            if entry == "name":
-                parameters.append({"type_": "BOLOS_TAG_APPNAME", "value": value})
-            elif entry == "version":
-                parameters.append({"type_": "BOLOS_TAG_APPVERSION", "value": value})
-            elif entry == "icon":
-                parameters.append(
-                    {"type_": "BOLOS_TAG_ICON", "value": icon_from_file(value)}
-                )
-            elif entry == "derivationPath":
-                derivation_paths: Dict[str, Optional[int]] = {
-                    "paths": None,
-                    "curve": None,
-                }
-                for derivation_entry in value:
-                    if derivation_entry == "curves":
-                        curves = 0
-                        for curve in value["curves"]:
-                            if curve == "secp256k1":
-                                curves |= params.CURVE_SECP256K1
-                            elif curve == "prime256r1":
-                                curves |= params.CURVE_PRIME256R1
-                            elif curve == "ed25519":
-                                curves |= params.CURVE_ED25519
-                            elif curve == "bls12381g1":
-                                curves |= params.CURVE_BLS12381G1
-                            derivation_paths["curve"] = curves
-                    elif derivation_entry == "paths":
-                        derivation_paths["paths"] = value["paths"]
-                parameters.append(
-                    {"type_": "BOLOS_TAG_DERIVEPATH", "value": derivation_paths}
-                )
-        return params.AppParams.build(parameters)
+    @abstractmethod
+    def data_size(self, device: str) -> int:
+        pass
+
+    @abstractmethod
+    def get_application_flags(self, device: str) -> int:
+        pass
+
+    @abstractmethod
+    def get_api_level(self, device: str) -> Optional[int]:
+        pass
+
+    @abstractmethod
+    def get_binary(self, device: str) -> str:
+        pass
+
+    @abstractmethod
+    def serialize_parameters(self, device: str) -> bytes:
+        pass
+
+    @abstractmethod
+    def assert_compatible_device(self, device_id: int):
+        pass
+
+    def serialize_derivation_path(self, value):
+        derivation_paths: Dict[str, Optional[int]] = {
+            "paths": None,
+            "curve": None,
+        }
+        for derivation_entry in value:
+            if derivation_entry == "curves":
+                curves = 0
+                for curve in value["curves"]:
+                    if curve == "secp256k1":
+                        curves |= params.CURVE_SECP256K1
+                    elif curve == "prime256r1":
+                        curves |= params.CURVE_PRIME256R1
+                    elif curve == "ed25519":
+                        curves |= params.CURVE_ED25519
+                    elif curve == "bls12381g1":
+                        curves |= params.CURVE_BLS12381G1
+                    derivation_paths["curve"] = curves
+            elif derivation_entry == "paths":
+                derivation_paths["paths"] = value["paths"]
+        return derivation_paths
```

### Comparing `ledgerwallet-0.1.4/ledgerwallet/params.py` & `ledgerwallet-0.3.0/ledgerwallet/params.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/ledgerwallet/proto/LedgerHSMServer_pb2.py` & `ledgerwallet-0.3.0/ledgerwallet/proto/LedgerHSMServer_pb2.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/ledgerwallet/proto/listApps_pb2.py` & `ledgerwallet-0.3.0/ledgerwallet/proto/listApps_pb2.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/ledgerwallet/simpleserver.py` & `ledgerwallet-0.3.0/ledgerwallet/simpleserver.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/ledgerwallet/transport/device.py` & `ledgerwallet-0.3.0/ledgerwallet/transport/device.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/ledgerwallet/transport/hid.py` & `ledgerwallet-0.3.0/ledgerwallet/transport/hid.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/ledgerwallet/transport/tcp.py` & `ledgerwallet-0.3.0/ledgerwallet/transport/tcp.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/ledgerwallet/utils.py` & `ledgerwallet-0.3.0/ledgerwallet/utils.py`

 * *Files identical despite different names*

### Comparing `ledgerwallet-0.1.4/setup.py` & `ledgerwallet-0.3.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,60 +1,60 @@
-import codecs
-from os import path
+[build-system]
+requires = [
+    "setuptools>=45",
+    "setuptools_scm[toml]>=6.2",
+    "wheel"
+]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "ledgerwallet"
+authors = [
+    {name = "Ledger", email = "hello@ledger.fr" }
+]
+description = "Library to communicate with Ledger Nano S/X and Speculos"
+readme = {file = "README.md", content-type = "text/markdown"}
+license = { file = "LICENSE" }
+classifiers = [
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Operating System :: POSIX :: Linux",
+    "Operating System :: Microsoft :: Windows",
+    "Operating System :: MacOS :: MacOS X",
+]
+dynamic = ["version"]
+requires-python = ">=3.7"
+dependencies = [
+    "click >=8.0",
+    "construct >=2.10",
+    "cryptography >=2.5",
+    "ecdsa",
+    "hidapi",
+    "intelhex",
+    "Pillow",
+    "protobuf >=3.20,<4",
+    "requests",
+    "tabulate",
+    "toml",
+]
+
+[project.urls]
+Home = "https://github.com/LedgerHQ/ledgerctl"
+
+[project.scripts]
+ledgerctl = "ledgerwallet.ledgerctl:cli"
+
+[tool.setuptools_scm]
+write_to = "ledgerwallet/__version__.py"
+local_scheme = "no-local-version"
 
-from setuptools import find_packages, setup
+[tool.isort]
+profile = "black"
 
+[tool.black]
+preview = true
 
-def read(rel_path):
-    here = path.abspath(path.dirname(__file__))
-    with codecs.open(path.join(here, rel_path), "r") as fp:
-        return fp.read()
-
-
-def get_version(rel_path):
-    for line in read(rel_path).splitlines():
-        if line.startswith("__version__"):
-            delimiter = '"' if '"' in line else "'"
-            return line.split(delimiter)[1]
-    raise RuntimeError("Unable to find version string.")
-
-
-this_dir = path.abspath(path.dirname(__file__))
-with open(path.join(this_dir, "README.md"), encoding="utf-8") as f:
-    long_description = f.read()
-
-setup(
-    name="ledgerwallet",
-    version=get_version("ledgerwallet/__init__.py"),
-    url="https://github.com/LedgerHQ/ledgerctl/",
-    python_requires=">=3.7",
-    license="MIT",
-    description="Python client and library to communicate with Ledger devices",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    install_requires=[
-        "click>=8.0",
-        "construct>=2.10",
-        "cryptography>=2.5",
-        "ecdsa",
-        "hidapi",
-        "intelhex",
-        "Pillow",
-        "protobuf>=3.20",
-        "requests",
-        "tabulate",
-    ],
-    packages=find_packages(),
-    include_package_data=True,
-    entry_points={"console_scripts": "ledgerctl = ledgerctl:cli"},
-    py_modules=["ledgerctl"],
-    classifiers=[
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Operating System :: POSIX :: Linux",
-        "Operating System :: Microsoft :: Windows",
-        "Operating System :: MacOS :: MacOS X",
-    ],
-)
+[tool.bandit]
+skips = ["B101"]
```


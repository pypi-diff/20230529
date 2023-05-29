# Comparing `tmp/genie.libs.robot-3.1.7-py3-none-any.whl.zip` & `tmp/genie.libs.robot-3.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 10774 bytes, number of entries: 8
--rw-r--r--  2.0 unx     1676 b- defN 19-Jan-23 21:51 genie.libs.robot-3.1.7-py3.6-nspkg.pth
--rw-r--r--  2.0 unx    34319 b- defN 19-Jan-23 21:51 genie/libs/robot/GenieRobot.py
--rw-r--r--  2.0 unx     1132 b- defN 19-Jan-23 21:51 genie/libs/robot/__init__.py
--rw-r--r--  2.0 unx     3345 b- defN 19-Jan-23 21:51 genie.libs.robot-3.1.7.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 19-Jan-23 21:51 genie.libs.robot-3.1.7.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 19-Jan-23 21:51 genie.libs.robot-3.1.7.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx        6 b- defN 19-Jan-23 21:51 genie.libs.robot-3.1.7.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      711 b- defN 19-Jan-23 21:51 genie.libs.robot-3.1.7.dist-info/RECORD
-8 files, 41298 bytes uncompressed, 9514 bytes compressed:  77.0%
+Zip file size: 10767 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     1676 b- defN 19-Feb-14 21:06 genie.libs.robot-3.1.8-py3.5-nspkg.pth
+-rw-r--r--  2.0 unx    34311 b- defN 19-Feb-14 21:06 genie/libs/robot/GenieRobot.py
+-rw-r--r--  2.0 unx     1132 b- defN 19-Feb-14 21:06 genie/libs/robot/__init__.py
+-rw-r--r--  2.0 unx     3345 b- defN 19-Feb-14 21:06 genie.libs.robot-3.1.8.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 19-Feb-14 21:06 genie.libs.robot-3.1.8.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 19-Feb-14 21:06 genie.libs.robot-3.1.8.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        6 b- defN 19-Feb-14 21:06 genie.libs.robot-3.1.8.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      711 b- defN 19-Feb-14 21:06 genie.libs.robot-3.1.8.dist-info/RECORD
+8 files, 41290 bytes uncompressed, 9507 bytes compressed:  77.0%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: genie.libs.robot-3.1.7-py3.6-nspkg.pth
+Filename: genie.libs.robot-3.1.8-py3.5-nspkg.pth
 Comment: 
 
 Filename: genie/libs/robot/GenieRobot.py
 Comment: 
 
 Filename: genie/libs/robot/__init__.py
 Comment: 
 
-Filename: genie.libs.robot-3.1.7.dist-info/METADATA
+Filename: genie.libs.robot-3.1.8.dist-info/METADATA
 Comment: 
 
-Filename: genie.libs.robot-3.1.7.dist-info/WHEEL
+Filename: genie.libs.robot-3.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: genie.libs.robot-3.1.7.dist-info/namespace_packages.txt
+Filename: genie.libs.robot-3.1.8.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: genie.libs.robot-3.1.7.dist-info/top_level.txt
+Filename: genie.libs.robot-3.1.8.dist-info/top_level.txt
 Comment: 
 
-Filename: genie.libs.robot-3.1.7.dist-info/RECORD
+Filename: genie.libs.robot-3.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## genie/libs/robot/GenieRobot.py

```diff
@@ -22,15 +22,15 @@
 from genie.conf import Genie
 from genie.utils.diff import Diff
 from genie.conf.base import loader
 from genie.conf.base import Testbed
 from genie.utils.config import Config
 from genie.harness.script import TestScript
 from genie.utils.loadattr import load_attribute
-from genie.harness._commons_internal import pickle, unpickle
+from genie.utils.profile import unpickle, pickle
 from genie.harness.discovery import GenieScriptDiscover
 from genie.harness.datafile.loader import TriggerdatafileLoader,\
                                           VerificationdatafileLoader,\
                                           PtsdatafileLoader
 
 log = logging.getLogger(__name__)
 
@@ -543,15 +543,15 @@
                         feature=fet.strip(), alias=None, device=dev)
 
                     profiled[fet][dev] = learnt_feature
 
 
         if os.path.isdir(os.path.dirname(name)):
             # the user provided a file to save as pickle
-            pickle_file = pickle(profiled, file = name)
+            pickle_file = pickle(profiled, pts_name = name)
             log.info('Saved system profile as file: %s' % pickle_file)
         else:
             self.testscript.parameters[name] = profiled
             log.info('Saved system profile as variable %s' % name)
 
     def _profile_config(self, device):
         device_handle = self._search_device(device)
```

## genie/libs/robot/__init__.py

```diff
@@ -4,15 +4,15 @@
 
     Description:
         This is the library sub-component of Genie for `genie.robot`.
 
 '''
 
 # metadata
-__version__ = '3.1.7'
+__version__ = '3.1.8'
 __author__ = 'Cisco Systems Inc.'
 __contact__ = ['pyats-support@cisco.com', 'pyats-support-ext@cisco.com']
 __copyright__ = 'Copyright (c) 2018, Cisco Systems Inc.'
 
 from genie import abstract
 abstract.declare_package(__name__)
```

## Comparing `genie.libs.robot-3.1.7-py3.6-nspkg.pth` & `genie.libs.robot-3.1.8-py3.5-nspkg.pth`

 * *Files identical despite different names*

## Comparing `genie.libs.robot-3.1.7.dist-info/METADATA` & `genie.libs.robot-3.1.8.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genie.libs.robot
-Version: 3.1.7
+Version: 3.1.8
 Summary: Genie libs Robot: RobotFramework libraries to interact with Genie
 Home-page: https://developer.cisco.com/site/pyats/
 Author: Cisco Systems Inc.
 Author-email: pyats-support-ext@cisco.com
 License: Apache 2.0
 Keywords: genie pyats test automation robot
 Platform: UNKNOWN
```

## Comparing `genie.libs.robot-3.1.7.dist-info/RECORD` & `genie.libs.robot-3.1.8.dist-info/RECORD`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-genie.libs.robot-3.1.7-py3.6-nspkg.pth,sha256=ObYoD8sL3pc4avNcQOL6mdv2IdNlOmFr3c3nD1iDADQ,1676
-genie/libs/robot/GenieRobot.py,sha256=l9pjIWoD4uL7srgZML_oeCryUFEnnJbtnnXtdSeLEc8,34319
-genie/libs/robot/__init__.py,sha256=2fQVZgUlH46EmEQGdRzk7trZQ_BAn7uyD3klrv1L9Bo,1132
-genie.libs.robot-3.1.7.dist-info/METADATA,sha256=lhB3U6bvQiasb9_nRdYLEJK_-g6na0G5KX9mgZiw8FE,3345
-genie.libs.robot-3.1.7.dist-info/WHEEL,sha256=_NOXIqFgOaYmlm9RJLPQZ13BJuEIrp5jx5ptRD5uh3Y,92
-genie.libs.robot-3.1.7.dist-info/namespace_packages.txt,sha256=k0OxVAETbf7Ou2EqqjuxO-JdrIdJtxZsUDHdrIkrOFE,17
-genie.libs.robot-3.1.7.dist-info/top_level.txt,sha256=EW4swMMBmuGW5VFCUGsl828kVUhrmMZJGHXfzmOidSg,6
-genie.libs.robot-3.1.7.dist-info/RECORD,,
+genie.libs.robot-3.1.8-py3.5-nspkg.pth,sha256=ObYoD8sL3pc4avNcQOL6mdv2IdNlOmFr3c3nD1iDADQ,1676
+genie/libs/robot/GenieRobot.py,sha256=fVkbLCTyAsUMD4q1GV5E7Xxo_tPHgBOIlxMF6IN45Fo,34311
+genie/libs/robot/__init__.py,sha256=vHE-pOLQa5mrJBQJXbv5U8K3pDxHxt7QYDt3TsING5o,1132
+genie.libs.robot-3.1.8.dist-info/METADATA,sha256=Zl_XExC1ph772mv_LbIVxWwVXbartZMRwdJFHGTq8y8,3345
+genie.libs.robot-3.1.8.dist-info/WHEEL,sha256=_NOXIqFgOaYmlm9RJLPQZ13BJuEIrp5jx5ptRD5uh3Y,92
+genie.libs.robot-3.1.8.dist-info/namespace_packages.txt,sha256=k0OxVAETbf7Ou2EqqjuxO-JdrIdJtxZsUDHdrIkrOFE,17
+genie.libs.robot-3.1.8.dist-info/top_level.txt,sha256=EW4swMMBmuGW5VFCUGsl828kVUhrmMZJGHXfzmOidSg,6
+genie.libs.robot-3.1.8.dist-info/RECORD,,
```


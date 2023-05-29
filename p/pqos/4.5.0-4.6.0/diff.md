# Comparing `tmp/pqos-4.5.0.tar.gz` & `tmp/pqos-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pqos-4.5.0.tar", last modified: Thu Dec 15 12:34:14 2022, max compression
+gzip compressed data, was "pqos-4.6.0.tar", last modified: Mon May 29 11:39:03 2023, max compression
```

## Comparing `pqos-4.5.0.tar` & `pqos-4.6.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)        0 2022-12-15 12:34:14.411811 pqos-4.5.0/
--rw-r--r--   0 aleksinx (11722229) cigccusr (22537)     1527 2022-12-15 12:30:28.000000 pqos-4.5.0/LICENSE
--rw-r--r--   0 aleksinx (11722229) cigccusr (22537)     4686 2022-12-15 12:34:14.409811 pqos-4.5.0/PKG-INFO
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)     1972 2022-12-15 12:30:28.000000 pqos-4.5.0/README.md
-drwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)        0 2022-12-15 12:34:14.332807 pqos-4.5.0/pqos/
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)     1871 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/__init__.py
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)     9496 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/allocation.py
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)    14602 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/capability.py
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)     5313 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/common.py
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)    11808 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/cpuinfo.py
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)     3019 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/error.py
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)     4786 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/l2ca.py
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)     4793 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/l3ca.py
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)     4819 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/mba.py
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)     8015 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/monitoring.py
--rwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)     7018 2022-12-15 12:30:28.000000 pqos-4.5.0/pqos/pqos.py
-drwxr-xr-x   0 aleksinx (11722229) cigccusr (22537)        0 2022-12-15 12:34:14.403810 pqos-4.5.0/pqos.egg-info/
--rw-r--r--   0 aleksinx (11722229) cigccusr (22537)     4686 2022-12-15 12:34:14.000000 pqos-4.5.0/pqos.egg-info/PKG-INFO
--rw-r--r--   0 aleksinx (11722229) cigccusr (22537)      350 2022-12-15 12:34:14.000000 pqos-4.5.0/pqos.egg-info/SOURCES.txt
--rw-r--r--   0 aleksinx (11722229) cigccusr (22537)        1 2022-12-15 12:34:14.000000 pqos-4.5.0/pqos.egg-info/dependency_links.txt
--rw-r--r--   0 aleksinx (11722229) cigccusr (22537)       52 2022-12-15 12:34:14.000000 pqos-4.5.0/pqos.egg-info/requires.txt
--rw-r--r--   0 aleksinx (11722229) cigccusr (22537)        5 2022-12-15 12:34:14.000000 pqos-4.5.0/pqos.egg-info/top_level.txt
--rw-r--r--   0 aleksinx (11722229) cigccusr (22537)     1318 2022-12-15 12:30:28.000000 pqos-4.5.0/pyproject.toml
--rw-r--r--   0 aleksinx (11722229) cigccusr (22537)       38 2022-12-15 12:34:14.412810 pqos-4.5.0/setup.cfg
--rw-r--r--   0 aleksinx (11722229) cigccusr (22537)      113 2022-12-15 12:30:28.000000 pqos-4.5.0/setup.py
+drwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)        0 2023-05-29 11:39:03.438513 pqos-4.6.0/
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)     1527 2023-05-29 10:01:18.000000 pqos-4.6.0/LICENSE
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)     4686 2023-05-29 11:39:03.436513 pqos-4.6.0/PKG-INFO
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)     1972 2023-05-29 10:01:18.000000 pqos-4.6.0/README.md
+drwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)        0 2023-05-29 11:39:03.381514 pqos-4.6.0/pqos/
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)     1871 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/__init__.py
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)     9851 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/allocation.py
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)    12644 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/capability.py
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)     5311 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/common.py
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)    10180 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/cpuinfo.py
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)     3019 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/error.py
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)     3852 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/l2ca.py
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)     3859 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/l3ca.py
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)     4284 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/mba.py
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)     8068 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/monitoring.py
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)    14148 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/native_struct.py
+-rwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)     6363 2023-05-29 10:01:18.000000 pqos-4.6.0/pqos/pqos.py
+drwxr-xr-x   0 rkanagar (12148013) cigccusr (22537)        0 2023-05-29 11:39:03.420515 pqos-4.6.0/pqos.egg-info/
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)     4686 2023-05-29 11:39:03.000000 pqos-4.6.0/pqos.egg-info/PKG-INFO
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)      372 2023-05-29 11:39:03.000000 pqos-4.6.0/pqos.egg-info/SOURCES.txt
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)        1 2023-05-29 11:39:03.000000 pqos-4.6.0/pqos.egg-info/dependency_links.txt
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)       52 2023-05-29 11:39:03.000000 pqos-4.6.0/pqos.egg-info/requires.txt
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)        5 2023-05-29 11:39:03.000000 pqos-4.6.0/pqos.egg-info/top_level.txt
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)     1318 2023-05-29 10:01:18.000000 pqos-4.6.0/pyproject.toml
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)       38 2023-05-29 11:39:03.439511 pqos-4.6.0/setup.cfg
+-rw-r--r--   0 rkanagar (12148013) cigccusr (22537)      113 2023-05-29 10:01:18.000000 pqos-4.6.0/setup.py
```

### Comparing `pqos-4.5.0/LICENSE` & `pqos-4.6.0/LICENSE`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD LICENSE
 
-Copyright(c) 2020-2022 Intel Corporation. All rights reserved.
+Copyright(c) 2020-2023 Intel Corporation. All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions
 are met:
 
   * Redistributions of source code must retain the above copyright
     notice, this list of conditions and the following disclaimer.
```

### Comparing `pqos-4.5.0/PKG-INFO` & `pqos-4.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pqos
-Version: 4.5.0
+Version: 4.6.0
 Summary: Python interface for Intel(R) RDT PQoS library
 Home-page: https://github.com/intel/intel-cmt-cat
 Author-email: Michal Aleksinski <michalx.aleksinski@intel.com>, Wojciech Andralojc <wojciechx.andralojc@intel.com>, Adrian Boczkowski <adrianx.boczkowski@intel.com>, Khawar Abbasi <khawar.abbasi@intel.com>
 Maintainer-email: Michal Aleksinski <michalx.aleksinski@intel.com>
 License: BSD LICENSE
         
-        Copyright(c) 2020-2022 Intel Corporation. All rights reserved.
+        Copyright(c) 2020-2023 Intel Corporation. All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
         are met:
         
           * Redistributions of source code must retain the above copyright
             notice, this list of conditions and the following disclaimer.
```

### Comparing `pqos-4.5.0/README.md` & `pqos-4.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pqos-4.5.0/pqos/__init__.py` & `pqos-4.6.0/pqos/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # BSD LICENSE
 #
-# Copyright(c) 2019-2022 Intel Corporation. All rights reserved.
+# Copyright(c) 2019-2023 Intel Corporation. All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 #   * Redistributions of source code must retain the above copyright
 #     notice, this list of conditions and the following disclaimer.
```

### Comparing `pqos-4.5.0/pqos/allocation.py` & `pqos-4.6.0/pqos/allocation.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # BSD LICENSE
 #
-# Copyright(c) 2019-2022 Intel Corporation. All rights reserved.
+# Copyright(c) 2019-2023 Intel Corporation. All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 #   * Redistributions of source code must retain the above copyright
 #     notice, this list of conditions and the following disclaimer.
@@ -285,7 +285,19 @@
         l3_cdp_cfg_enum = _get_cdp_config(l3_cdp_cfg)
         l2_cdp_cfg_enum = _get_cdp_config(l2_cdp_cfg)
         mba_cfg_enum = _get_mba_config(mba_cfg)
 
         ret = self.pqos.lib.pqos_alloc_reset(l3_cdp_cfg_enum, l2_cdp_cfg_enum,
                                              mba_cfg_enum)
         pqos_handle_error('pqos_alloc_reset', ret)
+
+    def reset_config(self, cfg):
+        """
+        Resets configuration of allocation technologies.
+
+        Parameters:
+            cfg: allocation configuration (CPqosAllocConfig)
+        """
+
+        cfg_ptr = ctypes.pointer(cfg)
+        ret = self.pqos.lib.pqos_alloc_reset_config(cfg_ptr)
+        pqos_handle_error('pqos_alloc_reset_config', ret)
```

### Comparing `pqos-4.5.0/pqos/capability.py` & `pqos-4.6.0/pqos/capability.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # BSD LICENSE
 #
-# Copyright(c) 2019-2022 Intel Corporation. All rights reserved.
+# Copyright(c) 2019-2023 Intel Corporation. All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 #   * Redistributions of source code must retain the above copyright
 #     notice, this list of conditions and the following disclaimer.
@@ -35,173 +35,55 @@
 """
 
 from __future__ import absolute_import, division, print_function
 import ctypes
 
 from pqos.common import pqos_handle_error
 from pqos.pqos import Pqos
-
-
-class CPqosCapabilityL3(ctypes.Structure):
-    "pqos_cap_l3ca structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('mem_size', ctypes.c_uint),
-        ('num_classes', ctypes.c_uint),
-        ('num_ways', ctypes.c_uint),
-        ('way_size', ctypes.c_uint),
-        ('way_contention', ctypes.c_uint64),
-        ('cdp', ctypes.c_int),
-        ('cdp_on', ctypes.c_int),
-    ]
-
-
-class CPqosCapabilityL2(ctypes.Structure):
-    "pqos_cap_l2ca structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('mem_size', ctypes.c_uint),
-        ('num_classes', ctypes.c_uint),
-        ('num_ways', ctypes.c_uint),
-        ('way_size', ctypes.c_uint),
-        ('way_contention', ctypes.c_uint64),
-        ('cdp', ctypes.c_int),
-        ('cdp_on', ctypes.c_int),
-    ]
-
-
-class CPqosCapabilityMBA(ctypes.Structure):
-    "pqos_cap_mba structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('mem_size', ctypes.c_uint),
-        ('num_classes', ctypes.c_uint),
-        ('throttle_max', ctypes.c_uint),
-        ('throttle_step', ctypes.c_uint),
-        ('is_linear', ctypes.c_int),
-        ('ctrl', ctypes.c_int),
-        ('ctrl_on', ctypes.c_int),
-    ]
-
-
-class CPqosMonitor(ctypes.Structure):
-    "pqos_monitor structure"
-    # pylint: disable=too-few-public-methods
-
-    PQOS_MON_EVENT_L3_OCCUP = 1
-    PQOS_MON_EVENT_LMEM_BW = 2
-    PQOS_MON_EVENT_TMEM_BW = 4
-    PQOS_MON_EVENT_RMEM_BW = 8
-    RESERVED1 = 0x1000
-    RESERVED2 = 0x2000
-    PQOS_PERF_EVENT_LLC_MISS = 0x4000
-    PQOS_PERF_EVENT_IPC = 0x8000
-
-    _fields_ = [
-        ('type', ctypes.c_int),
-        ('max_rmid', ctypes.c_uint),
-        ('scale_factor', ctypes.c_uint32),
-        ('counter_length', ctypes.c_uint),
-    ]
-
-
-class CPqosCapabilityMonitoring(ctypes.Structure):
-    "pqos_cap_mon structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('mem_size', ctypes.c_uint),
-        ('max_rmid', ctypes.c_uint),
-        ('l3_size', ctypes.c_uint),
-        ('num_events', ctypes.c_uint),
-        ('events', CPqosMonitor * 0),
-    ]
-
-
-class CPqosCapabilityUnion(ctypes.Union):
-    "Union from pqos_capability structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('mon', ctypes.POINTER(CPqosCapabilityMonitoring)),
-        ('l3ca', ctypes.POINTER(CPqosCapabilityL3)),
-        ('l2ca', ctypes.POINTER(CPqosCapabilityL2)),
-        ('mba', ctypes.POINTER(CPqosCapabilityMBA)),
-        ('generic_ptr', ctypes.c_void_p),
-    ]
-
-
-class CPqosCapability(ctypes.Structure):
-    "pqos_capability structure"
-    # pylint: disable=too-few-public-methods
-
-    PQOS_CAP_TYPE_MON = 0
-    PQOS_CAP_TYPE_L3CA = 1
-    PQOS_CAP_TYPE_L2CA = 2
-    PQOS_CAP_TYPE_MBA = 3
-    PQOS_CAP_TYPE_NUMOF = 4
-
-    _fields_ = [
-        ('type', ctypes.c_int),
-        ('u', CPqosCapabilityUnion)
-    ]
-
-
-class CPqosCap(ctypes.Structure):
-    "pqos_cap structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('mem_size', ctypes.c_uint),
-        ('version', ctypes.c_uint),
-        ('num_cap', ctypes.c_uint),
-        ('capabilities', CPqosCapability * 0)
-    ]
-
+from pqos.native_struct import CPqosCap, CPqosCapability, CPqosMonitor
 
 class PqosCapabilityMonitoring(object):
     "PQoS monitoring capability"
     # pylint: disable=too-few-public-methods
 
     def __init__(self):
         self.mem_size = 0    # byte size of the structure
         self.max_rmid = 0    # max RMID supported by socket
         self.l3_size = 0     # L3 cache size in bytes
         self.events = []     # a list of supported events
 
 
 class PqosCapabilityL3Ca(object):
     "PQoS L3 cache allocation capability"
-    # pylint: disable=too-few-public-methods
+    # pylint: disable=too-few-public-methods,too-many-instance-attributes
 
     def __init__(self):
-        self.mem_size = 0           # byte size of the structure
-        self.num_classes = 0        # number of classes of service
-        self.num_ways = 0           # number of cache ways
-        self.way_size = 0           # way size in bytes
-        self.way_contention = 0     # ways contention bit mask
-        self.cdp = False            # code data prioritization feature support
-        self.cdp_on = False         # code data prioritization on or off
+        self.mem_size = 0               # byte size of the structure
+        self.num_classes = 0            # number of classes of service
+        self.num_ways = 0               # number of cache ways
+        self.way_size = 0               # way size in bytes
+        self.way_contention = 0         # ways contention bit mask
+        self.cdp = False                # code data prioritization feature support
+        self.cdp_on = False             # code data prioritization on or off
+        self.non_contiguous_cbm = False # Non-Contiguous CBM support
 
 
 class PqosCapabilityL2Ca(object):
     "PQoS L2 cache allocation capability"
-    # pylint: disable=too-few-public-methods
+    # pylint: disable=too-few-public-methods,too-many-instance-attributes
 
     def __init__(self):
-        self.mem_size = 0           # byte size of the structure
-        self.num_classes = 0        # number of classes of service
-        self.num_ways = 0           # number of cache ways
-        self.way_size = 0           # way size in bytes
-        self.way_contention = 0     # ways contention bit mask
-        self.cdp = False            # code data prioritization feature support
-        self.cdp_on = False         # code data prioritization on or off
+        self.mem_size = 0               # byte size of the structure
+        self.num_classes = 0            # number of classes of service
+        self.num_ways = 0               # number of cache ways
+        self.way_size = 0               # way size in bytes
+        self.way_contention = 0         # ways contention bit mask
+        self.cdp = False                # code data prioritization feature support
+        self.cdp_on = False             # code data prioritization on or off
+        self.non_contiguous_cbm = False # Non-Contiguous CBM support
 
 
 class PqosCapabilityMba(object):
     "PQoS memory bandwidth allocation capability"
     # pylint: disable=too-few-public-methods
 
     def __init__(self):
@@ -254,14 +136,15 @@
     capability.mem_size = c_capability.mem_size
     capability.num_classes = c_capability.num_classes
     capability.num_ways = c_capability.num_ways
     capability.way_size = c_capability.way_size
     capability.way_contention = c_capability.way_contention
     capability.cdp = _get_tristate_bool(c_capability.cdp)
     capability.cdp_on = _get_tristate_bool(c_capability.cdp_on)
+    capability.non_contiguous_cbm = c_capability.non_contiguous_cbm
     return capability
 
 
 def _get_cap_l2ca(p_capability):
     """
     Converts low-level pqos_cap_l2ca structure to
     high-level PqosCapabilityL2Ca object.
@@ -271,14 +154,15 @@
     capability.mem_size = c_capability.mem_size
     capability.num_classes = c_capability.num_classes
     capability.num_ways = c_capability.num_ways
     capability.way_size = c_capability.way_size
     capability.way_contention = c_capability.way_contention
     capability.cdp = _get_tristate_bool(c_capability.cdp)
     capability.cdp_on = _get_tristate_bool(c_capability.cdp_on)
+    capability.non_contiguous_cbm = c_capability.non_contiguous_cbm
     return capability
 
 
 def _get_cap_mba(p_capability):
     """
     Converts low-level pqos_cap_mba structure to
     high-level PqosCapabilityMba object.
@@ -320,93 +204,132 @@
 
 
 class PqosCap(object):
     "PQoS capabilities"
 
     def __init__(self):
         "Initializes capabilities, calls pqos_cap_get."
+
         self.pqos = Pqos()
         self.p_cap = ctypes.POINTER(CPqosCap)()
         ret = self.pqos.lib.pqos_cap_get(ctypes.byref(self.p_cap), None)
         pqos_handle_error('pqos_cap_get', ret)
 
     def get_type(self, type_str):
-        """Retrieves a type of capability from a cap structure.
+        """
+        Retrieves a type of capability from a cap structure.
 
         Parameters:
             type_str: a string indicating a type of capability, available
                       options: mon, l3ca, l2ca and mba
+
+        Returns:
+            capabilities
         """
+
         type_enum = pqos_get_type_enum(type_str)
         p_cap_item = ctypes.POINTER(CPqosCapability)()
         ret = self.pqos.lib.pqos_cap_get_type(self.p_cap, type_enum,
                                               ctypes.byref(p_cap_item))
         pqos_handle_error('pqos_cap_get_type', ret)
 
         cap_item = p_cap_item.contents
         capability = _get_capability(cap_item, type_str)
         return capability
 
     def get_l3ca_cos_num(self):
         """
         Retrieves number of L3 allocation classes of service from
         a cap structure.
+
+        Returns:
+            a number of L3 allocation classes
         """
+
         cos_num = ctypes.c_uint(0)
         ret = self.pqos.lib.pqos_l3ca_get_cos_num(self.p_cap,
                                                   ctypes.byref(cos_num))
         pqos_handle_error('pqos_l3ca_get_cos_num', ret)
         return cos_num.value
 
     def get_l2ca_cos_num(self):
         """
         Retrieves number of L2 allocation classes of service from
         a cap structure.
+
+        Returns:
+            a number of L2 allocation classes
         """
+
         cos_num = ctypes.c_uint(0)
         ret = self.pqos.lib.pqos_l2ca_get_cos_num(self.p_cap,
                                                   ctypes.byref(cos_num))
         pqos_handle_error('pqos_l2ca_get_cos_num', ret)
         return cos_num.value
 
     def get_mba_cos_num(self):
         """
         Retrieves number of memory B/W allocation classes of service from
         a cap structure.
+
+        Returns:
+            a number of memory B/W allocation classes
         """
+
         cos_num = ctypes.c_uint(0)
         ret = self.pqos.lib.pqos_mba_get_cos_num(self.p_cap,
                                                  ctypes.byref(cos_num))
         pqos_handle_error('pqos_mba_get_cos_num', ret)
         return cos_num.value
 
     def is_l3ca_cdp_enabled(self):
-        "Retrieves L3 CDP status."
+        """
+        Retrieves L3 CDP status.
+
+        Returns:
+            a tuple of two values: supported (True, False or None)
+              and enabled (True, False or None)
+        """
+
         supported = ctypes.c_int(0)
         enabled = ctypes.c_int(0)
         ret = self.pqos.lib.pqos_l3ca_cdp_enabled(self.p_cap,
                                                   ctypes.byref(supported),
                                                   ctypes.byref(enabled))
         pqos_handle_error('pqos_l3ca_cdp_enabled', ret)
         return (_get_tristate_bool(supported.value),
                 _get_tristate_bool(enabled.value))
 
     def is_l2ca_cdp_enabled(self):
-        "Retrieves L2 CDP status."
+        """
+        Retrieves L2 CDP status.
+
+        Returns:
+            a tuple of two values: supported (True, False or None)
+              and enabled (True, False or None)
+        """
+
         supported = ctypes.c_int(0)
         enabled = ctypes.c_int(0)
         ret = self.pqos.lib.pqos_l2ca_cdp_enabled(self.p_cap,
                                                   ctypes.byref(supported),
                                                   ctypes.byref(enabled))
         pqos_handle_error('pqos_l2ca_cdp_enabled', ret)
         return (_get_tristate_bool(supported.value),
                 _get_tristate_bool(enabled.value))
 
     def is_mba_ctrl_enabled(self):
-        "Retrieves MBA CTRL status."
+        """
+        Retrieves MBA CTRL status.
+
+        Returns:
+            a tuple of two values: supported (True, False or None)
+              and enabled (True, False or None)
+        """
+
         supported = ctypes.c_int(0)
         enabled = ctypes.c_int(0)
         ret = self.pqos.lib.pqos_mba_ctrl_enabled(self.p_cap,
                                                   ctypes.byref(supported),
                                                   ctypes.byref(enabled))
         pqos_handle_error('pqos_mba_ctrl_enabled', ret)
         return (_get_tristate_bool(supported.value),
```

### Comparing `pqos-4.5.0/pqos/common.py` & `pqos-4.6.0/pqos/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # BSD LICENSE
 #
-# Copyright(c) 2019-2022 Intel Corporation. All rights reserved.
+# Copyright(c) 2019-2023 Intel Corporation. All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 #   * Redistributions of source code must retain the above copyright
 #     notice, this list of conditions and the following disclaimer.
@@ -142,11 +142,11 @@
 
 def free_memory(ptr):
     "Releases memory allocated by the library."
 
     libc_path = ctypes.util.find_library('c')
 
     if not libc_path:
-        raise Exception('Cannot find libc')
+        raise OSError('Cannot find libc')
 
     libc = ctypes.cdll.LoadLibrary(libc_path)
     libc.free(ptr)
```

### Comparing `pqos-4.5.0/pqos/cpuinfo.py` & `pqos-4.6.0/pqos/cpuinfo.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # BSD LICENSE
 #
-# Copyright(c) 2019-2022 Intel Corporation. All rights reserved.
+# Copyright(c) 2019-2023 Intel Corporation. All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 #   * Redistributions of source code must retain the above copyright
 #     notice, this list of conditions and the following disclaimer.
@@ -35,65 +35,18 @@
 like number of cores, L2/L3 cache ID etc.
 """
 
 from __future__ import absolute_import, division, print_function
 import ctypes
 
 from pqos.common import pqos_handle_error, free_memory
-from pqos.error import PqosError, PqosErrorParam, PqosErrorResource
+from pqos.error import PqosError, PqosErrorResource, PqosErrorParam
+from pqos.native_struct import CPqosCpuInfo, CPqosCoreInfo
 from pqos.pqos import Pqos
 
-
-class CPqosCoreInfo(ctypes.Structure):
-    "pqos_coreinfo structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('lcore', ctypes.c_uint),    # Logical core id
-        ('socket', ctypes.c_uint),   # Socket id in the system
-        ('l3_id', ctypes.c_uint),    # L3/LLC cluster id
-        ('l2_id', ctypes.c_uint),    # L2 cluster id
-        ('l3cat_id', ctypes.c_uint), # L3 CAT classes id
-        ('mba_id', ctypes.c_uint),   # MBA id
-    ]
-
-
-class CPqosCacheInfo(ctypes.Structure):
-    "pqos_cacheinfo structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ("detected", ctypes.c_int),         # Indicates cache detected & valid
-        ("num_ways", ctypes.c_uint),        # Number of cache ways
-        ("num_sets", ctypes.c_uint),        # Number of sets
-        ("num_partitions", ctypes.c_uint),  # Number of partitions
-        ("line_size", ctypes.c_uint),       # Cache line size in bytes
-        ("total_size", ctypes.c_uint),      # Total cache size in bytes
-        ("way_size", ctypes.c_uint),        # Cache way size in bytes
-    ]
-
-
-class CPqosCpuInfo(ctypes.Structure):
-    "pqos_cpuinfo structure"
-    # pylint: disable=too-few-public-methods
-
-    PQOS_VENDOR_UNKNOWN = 0
-    PQOS_VENDOR_INTEL = 1
-    PQOS_VENDOR_AMD = 2
-
-    _fields_ = [
-        ("mem_size", ctypes.c_uint),   # Byte size of the structure
-        ("l2", CPqosCacheInfo),        # L2 cache information
-        ("l3", CPqosCacheInfo),        # L3 cache information
-        ("vendor", ctypes.c_int),      # CPU vendor
-        ("num_cores", ctypes.c_uint),  # Number of cores in the system
-        ("cores", CPqosCoreInfo * 0)   # Core information
-    ]
-
-
 class PqosCoreInfo(object):
     "Core information"
     # pylint: disable=too-few-public-methods, too-many-arguments
 
     def __init__(self, core, socket, l3_id, l2_id, l3cat_id, mba_id):
         self.core = core
         self.socket = socket
@@ -168,15 +121,15 @@
             p_items = func(self.p_cpu, arg, count_ref)
         else:
             p_items = func(self.p_cpu, count_ref)
 
         if not p_items:
             return []
 
-        items = [p_items[i] for i in range(count.value)] if count.value else []
+        items = [p_items[i] for i in range(count.value)] if count.value > 0 else []
         free_memory(p_items)
         return items
 
     def _call_func_ref(self, func, arg):
         """
         Calls a function from PQoS library, handles errors and returns
         an integer set by the called function.
```

### Comparing `pqos-4.5.0/pqos/error.py` & `pqos-4.6.0/pqos/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # BSD LICENSE
 #
-# Copyright(c) 2019-2022 Intel Corporation. All rights reserved.
+# Copyright(c) 2019-2023 Intel Corporation. All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 #   * Redistributions of source code must retain the above copyright
 #     notice, this list of conditions and the following disclaimer.
```

### Comparing `pqos-4.5.0/pqos/l2ca.py` & `pqos-4.6.0/pqos/mba.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # BSD LICENSE
 #
-# Copyright(c) 2019-2022 Intel Corporation. All rights reserved.
+# Copyright(c) 2019-2023 Intel Corporation. All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 #   * Redistributions of source code must retain the above copyright
 #     notice, this list of conditions and the following disclaimer.
@@ -27,116 +27,84 @@
 # DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 # THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 # (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 ################################################################################
 
 """
-The module defines PqosCatL2 which can be used to read or write L2 CAT
-configuration.
+The module defines PqosMba which can be used to read or write Memory Bandwidth
+Allocation configuration.
 """
 
 from __future__ import absolute_import, division, print_function
 import ctypes
 
 from pqos.capability import PqosCap
-from pqos.common import (
-    pqos_handle_error, convert_from_cos, convert_to_cos, COSBase
-)
+from pqos.common import pqos_handle_error
+from pqos.native_struct import CPqosMba
 from pqos.pqos import Pqos
 
+class PqosMba(object):
+    "PQoS Memory Bandwidth Allocation"
 
-class CPqosL2CaMaskCDP(ctypes.Structure):
-    "CDP structure from union from pqos_l2ca structure"
-    # pylint: disable=too-few-public-methods
+    class COS:  # pylint: disable=too-few-public-methods
+        "MBA class of service configuration"
 
-    _fields_ = [
-        ('data_mask', ctypes.c_uint64),
-        ('code_mask', ctypes.c_uint64),
-    ]
-
-
-class CPqosL2CaMask(ctypes.Union):
-    "Union from pqos_l2ca structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('ways_mask', ctypes.c_uint64),
-        ('s', CPqosL2CaMaskCDP)
-    ]
-
-
-class CPqosL2Ca(ctypes.Structure):
-    "pqos_l2ca structure"
-
-    _fields_ = [
-        ('class_id', ctypes.c_uint),
-        ('cdp', ctypes.c_int),
-        ('u', CPqosL2CaMask),
-    ]
-
-    @classmethod
-    def from_cos(cls, cos):
-        "Creates CPqosL2Ca object from PqosCatL2.COS object."
-
-        return convert_from_cos(cos, cls)
-
-    def to_cos(self, cls):
-        "Creates PqosCatL2.COS object from CPqosL2Ca object."
-
-        return convert_to_cos(self, cls)
-
-
-class PqosCatL2(object):
-    "PQoS L2 Cache Allocation Technology"
-
-    class COS(COSBase):  # pylint: disable=too-few-public-methods
-        "L2 class of service configuration"
+        def __init__(self, class_id, mb_max, ctrl=False):
+            self.class_id = class_id  # class of service
+            self.mb_max = mb_max      # maximum available bandwidth
+                                      # in percentage (without MBA controller)
+                                      # or in MBps (with MBA controller),
+                                      # depending on ctrl flag
+            self.ctrl = ctrl          # MBA controller flag
 
     def __init__(self):
         self.pqos = Pqos()
 
-    def set(self, l2id, coses):
+    def set(self, socket, requested):
         """
-        Sets class of service on a specified l2id.
+        Sets classes of service defined by requested configuration on a socket.
 
         Parameters:
-            l2id: L2 cache identifier
-            coses: a list of PqosCatL2.COS objects, class of service
-                   configuration
+            socket: socket ID
+            requested: a list of PqosMba.COS objects that define requested MBA
+                       configuration
+
+        Returns:
+            a list of PqosMba.COS object with actual MBA configuration
         """
 
-        pqos_l2_cas = [CPqosL2Ca.from_cos(cos) for cos in coses]
-        pqos_l2_ca_arr = (CPqosL2Ca * len(pqos_l2_cas))(*pqos_l2_cas)
-        ret = self.pqos.lib.pqos_l2ca_set(l2id, len(pqos_l2_cas),
-                                          pqos_l2_ca_arr)
-        pqos_handle_error('pqos_l2ca_set', ret)
+        requested_coses = [CPqosMba.from_cos(req) for req in requested]
+        num_cos = len(requested_coses)
+        cos_arr = (CPqosMba * num_cos)(*requested_coses)
+        actual_arr = (CPqosMba * num_cos)()
+
+        ret = self.pqos.lib.pqos_mba_set(socket, num_cos, cos_arr, actual_arr)
+        pqos_handle_error('pqos_mba_set', ret)
 
-    def get(self, l2id):
+        actual = [cos.to_cos(self.COS) for cos in actual_arr]
+        return actual
+
+    def get(self, socket):
         """
-        Reads classes of service from a L2 ID.
+        Reads MBA configuration for a socket.
 
         Parameters:
-            l2id: L2 cache identifier
+            socket: socket ID
+
+        Returns:
+            a list of PqosMba.COS object with actual MBA configuration
+            for a given socket
         """
 
         cap = PqosCap()
-        cos_num = cap.get_l2ca_cos_num()
+        max_num_cos = cap.get_mba_cos_num()
 
-        l2cas = (CPqosL2Ca * cos_num)()
-        num_ca = ctypes.c_uint(0)
-        num_ca_ref = ctypes.byref(num_ca)
-        ret = self.pqos.lib.pqos_l2ca_get(l2id, cos_num, num_ca_ref, l2cas)
-        pqos_handle_error('pqos_l2ca_get', ret)
+        num_cos = ctypes.c_uint(0)
+        cos_arr = (CPqosMba * max_num_cos)()
 
-        coses = [l2ca.to_cos(self.COS) for l2ca in l2cas[:num_ca.value]]
-        return coses
+        ret = self.pqos.lib.pqos_mba_get(socket, max_num_cos,
+                                         ctypes.byref(num_cos), cos_arr)
+        pqos_handle_error('pqos_mba_get', ret)
 
-    def get_min_cbm_bits(self):
-        """Gets minimum number of bits which must be set in L2 way mask when
-        updating a class of service."""
-
-        min_cbm_bits = ctypes.c_uint(0)
-        min_cbm_bits_ref = ctypes.byref(min_cbm_bits)
-        ret = self.pqos.lib.pqos_l2ca_get_min_cbm_bits(min_cbm_bits_ref)
-        pqos_handle_error('pqos_l2ca_get_min_cbm_bits', ret)
-        return min_cbm_bits.value
+        coses = [cos_arr[i].to_cos(self.COS) for i in range(num_cos.value)]
+        return coses
```

### Comparing `pqos-4.5.0/pqos/l3ca.py` & `pqos-4.6.0/pqos/l3ca.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # BSD LICENSE
 #
-# Copyright(c) 2019-2022 Intel Corporation. All rights reserved.
+# Copyright(c) 2019-2023 Intel Corporation. All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 #   * Redistributions of source code must retain the above copyright
 #     notice, this list of conditions and the following disclaimer.
@@ -35,61 +35,18 @@
 configuration.
 """
 
 from __future__ import absolute_import, division, print_function
 import ctypes
 
 from pqos.capability import PqosCap
-from pqos.common import (
-    pqos_handle_error, convert_from_cos, convert_to_cos, COSBase
-)
+from pqos.common import pqos_handle_error, COSBase
+from pqos.native_struct import CPqosL3Ca
 from pqos.pqos import Pqos
 
-
-class CPqosL3CaMaskCDP(ctypes.Structure):
-    "CDP structure from union from pqos_l3ca structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('data_mask', ctypes.c_uint64),
-        ('code_mask', ctypes.c_uint64),
-    ]
-
-
-class CPqosL3CaMask(ctypes.Union):
-    "Union from pqos_l3ca structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('ways_mask', ctypes.c_uint64),
-        ('s', CPqosL3CaMaskCDP)
-    ]
-
-
-class CPqosL3Ca(ctypes.Structure):
-    "pqos_l3ca structure"
-
-    _fields_ = [
-        ('class_id', ctypes.c_uint),
-        ('cdp', ctypes.c_int),
-        ('u', CPqosL3CaMask),
-    ]
-
-    @classmethod
-    def from_cos(cls, cos):
-        "Creates CPqosL3Ca object from PqosCatL3.COS object."
-
-        return convert_from_cos(cos, cls)
-
-    def to_cos(self, cls):
-        "Creates PqosCatL3.COS object from CPqosL3Ca object."
-
-        return convert_to_cos(self, cls)
-
-
 class PqosCatL3(object):
     "PQoS L3 Cache Allocation Technology"
 
     class COS(COSBase):  # pylint: disable=too-few-public-methods
         "L3 class of service configuration"
 
     def __init__(self):
```

### Comparing `pqos-4.5.0/pqos/monitoring.py` & `pqos-4.6.0/pqos/monitoring.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # BSD LICENSE
 #
-# Copyright(c) 2019-2022 Intel Corporation. All rights reserved.
+# Copyright(c) 2019-2023 Intel Corporation. All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 #   * Redistributions of source code must retain the above copyright
 #     notice, this list of conditions and the following disclaimer.
@@ -35,45 +35,25 @@
 bandwidth.
 """
 
 from __future__ import absolute_import, division, print_function
 import ctypes
 
 from pqos.common import pqos_handle_error
+from pqos.native_struct import (
+    CPqosEventValues, CPqosMonitor, RmidT
+)
 from pqos.pqos import Pqos
-from pqos.capability import CPqosMonitor
-
-
-RmidT = ctypes.c_uint32
-
-
-class CPqosEventValues(ctypes.Structure):
-    "pqos_event_values structure"
-    # pylint: disable=too-few-public-methods
-
-    _fields_ = [
-        ('llc', ctypes.c_uint64),
-        ('mbm_local', ctypes.c_uint64),
-        ('mbm_total', ctypes.c_uint64),
-        ('mbm_remote', ctypes.c_uint64),
-        ('mbm_local_delta', ctypes.c_uint64),
-        ('mbm_total_delta', ctypes.c_uint64),
-        ('mbm_remote_delta', ctypes.c_uint64),
-        ('ipc_retired', ctypes.c_uint64),
-        ('ipc_retired_delta', ctypes.c_uint64),
-        ('ipc_unhalted', ctypes.c_uint64),
-        ('ipc_unhalted_delta', ctypes.c_uint64),
-        ('ipc', ctypes.c_double),
-        ('llc_misses', ctypes.c_uint64),
-        ('llc_misses_delta', ctypes.c_uint64),
-    ]
-
 
 class CPqosMonData(ctypes.Structure):
-    "pqos_mon_data structure"
+    """
+    pqos_mon_data structure
+    This class is not in native_struct.py because it has additional methods
+    that requires Pqos() - avoiding circular dependency.
+    """
 
     _fields_ = [
         ('valid', ctypes.c_int),
         ('event', ctypes.c_uint),
         ('context', ctypes.c_void_p),
         ('values', CPqosEventValues),
         ('num_pids', ctypes.c_uint),
@@ -124,14 +104,40 @@
 
         Returns:
             a pointer to a monitoring data
         """
 
         return ctypes.pointer(self)
 
+    def get_event_value(self, event):
+        """
+        Returns counter value for a given event.
+
+        Parameters:
+            event: an event identifier
+
+        Returns:
+            counter value
+        """
+
+        event_counter_map = {
+            'l3_occup': 'llc',
+            'lmem_bw': 'mbm_local_delta',
+            'tmem_bw': 'mbm_total_delta',
+            'rmem_bw': 'mbm_remote_delta',
+            'perf_ipc': 'ipc',
+            'perf_llc_miss': 'llc_misses_delta'
+        }
+
+        counter = event_counter_map.get(event)
+        if not counter:
+            return None
+
+        return getattr(self.values, counter, None)
+
 
 def _get_event_mask(events):
     "Converts a list of events into a binary mask accepted by PQoS library."
 
     event_map = {
         'l3_occup': CPqosMonitor.PQOS_MON_EVENT_L3_OCCUP,
         'lmem_bw': CPqosMonitor.PQOS_MON_EVENT_LMEM_BW,
```

### Comparing `pqos-4.5.0/pqos/pqos.py` & `pqos-4.6.0/pqos/pqos.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ################################################################################
 # BSD LICENSE
 #
-# Copyright(c) 2019-2022 Intel Corporation. All rights reserved.
+# Copyright(c) 2019-2023 Intel Corporation. All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
 # modification, are permitted provided that the following conditions
 # are met:
 #
 #   * Redistributions of source code must retain the above copyright
 #     notice, this list of conditions and the following disclaimer.
@@ -37,42 +37,15 @@
 """
 
 from __future__ import absolute_import, division, print_function
 import ctypes
 import sys
 
 from pqos.common import pqos_handle_error
-
-
-class CPqosConfig(ctypes.Structure):
-    "pqos_config structure"
-    # pylint: disable=too-few-public-methods
-
-    PQOS_INTER_MSR = 0
-    PQOS_INTER_OS = 1
-    PQOS_INTER_OS_RESCTRL_MON = 2
-    PQOS_INTER_AUTO = 3
-
-    LOG_VER_SILENT = -1
-    LOG_VER_DEFAULT = 0
-    LOG_VER_VERBOSE = 1
-    LOG_VER_SUPER_VERBOSE = 2
-
-    LOG_CALLBACK = ctypes.CFUNCTYPE(None, ctypes.c_void_p, ctypes.c_size_t,
-                                    ctypes.c_char_p)
-
-    _fields_ = [
-        ('fd_log', ctypes.c_int),
-        ('callback_log', LOG_CALLBACK),
-        ('context_log', ctypes.c_void_p),
-        ('verbose', ctypes.c_int),
-        ('interface', ctypes.c_int),
-        ('reserved', ctypes.c_int),
-    ]
-
+from pqos.native_struct import CPqosConfig
 
 class Pqos(object):
     """
     The main class that is responsible for PQoS library initialization
     and finalization. It implements singleton pattern.
     """
```

### Comparing `pqos-4.5.0/pqos.egg-info/PKG-INFO` & `pqos-4.6.0/pqos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: pqos
-Version: 4.5.0
+Version: 4.6.0
 Summary: Python interface for Intel(R) RDT PQoS library
 Home-page: https://github.com/intel/intel-cmt-cat
 Author-email: Michal Aleksinski <michalx.aleksinski@intel.com>, Wojciech Andralojc <wojciechx.andralojc@intel.com>, Adrian Boczkowski <adrianx.boczkowski@intel.com>, Khawar Abbasi <khawar.abbasi@intel.com>
 Maintainer-email: Michal Aleksinski <michalx.aleksinski@intel.com>
 License: BSD LICENSE
         
-        Copyright(c) 2020-2022 Intel Corporation. All rights reserved.
+        Copyright(c) 2020-2023 Intel Corporation. All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions
         are met:
         
           * Redistributions of source code must retain the above copyright
             notice, this list of conditions and the following disclaimer.
```

### Comparing `pqos-4.5.0/pyproject.toml` & `pqos-4.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "pqos"
-version = "4.5.0"
+version = "4.6.0"
 description = "Python interface for Intel(R) RDT PQoS library"
 authors = [
     { name = "Michal Aleksinski", email = "michalx.aleksinski@intel.com"},
     { name = "Wojciech Andralojc", email = "wojciechx.andralojc@intel.com"},
     { name = "Adrian Boczkowski", email = "adrianx.boczkowski@intel.com"},
     { name = "Khawar Abbasi", email = "khawar.abbasi@intel.com"}
 ]
```


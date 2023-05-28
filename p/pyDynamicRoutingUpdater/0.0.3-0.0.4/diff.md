# Comparing `tmp/pyDynamicRoutingUpdater-0.0.3.tar.gz` & `tmp/pyDynamicRoutingUpdater-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyDynamicRoutingUpdater-0.0.3.tar", last modified: Mon Mar 13 22:32:52 2023, max compression
+gzip compressed data, was "pyDynamicRoutingUpdater-0.0.4.tar", last modified: Sun May 28 22:10:50 2023, max compression
```

## Comparing `pyDynamicRoutingUpdater-0.0.3.tar` & `pyDynamicRoutingUpdater-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 22:32:52.875296 pyDynamicRoutingUpdater-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 22:32:52.875296 pyDynamicRoutingUpdater-0.0.3/DynamicRoutingUpdater/
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-03-13 22:32:40.000000 pyDynamicRoutingUpdater-0.0.3/DynamicRoutingUpdater/DynamicRoutingUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)     6875 2023-03-13 22:32:40.000000 pyDynamicRoutingUpdater-0.0.3/DynamicRoutingUpdater/NetworkHookHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-03-13 22:32:40.000000 pyDynamicRoutingUpdater-0.0.3/DynamicRoutingUpdater/NetworkInfoWatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-13 22:32:40.000000 pyDynamicRoutingUpdater-0.0.3/DynamicRoutingUpdater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13319 2023-03-13 22:32:40.000000 pyDynamicRoutingUpdater-0.0.3/DynamicRoutingUpdater/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-13 22:32:40.000000 pyDynamicRoutingUpdater-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-03-13 22:32:52.875296 pyDynamicRoutingUpdater-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-03-13 22:32:40.000000 pyDynamicRoutingUpdater-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 22:32:52.875296 pyDynamicRoutingUpdater-0.0.3/pyDynamicRoutingUpdater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-03-13 22:32:52.000000 pyDynamicRoutingUpdater-0.0.3/pyDynamicRoutingUpdater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-03-13 22:32:52.000000 pyDynamicRoutingUpdater-0.0.3/pyDynamicRoutingUpdater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 22:32:52.000000 pyDynamicRoutingUpdater-0.0.3/pyDynamicRoutingUpdater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-13 22:32:52.000000 pyDynamicRoutingUpdater-0.0.3/pyDynamicRoutingUpdater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-13 22:32:52.000000 pyDynamicRoutingUpdater-0.0.3/pyDynamicRoutingUpdater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 22:32:52.875296 pyDynamicRoutingUpdater-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-03-13 22:32:40.000000 pyDynamicRoutingUpdater-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:10:50.380599 pyDynamicRoutingUpdater-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:10:50.380599 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/AddressInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/DynamicRoutingUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/NetworkAdapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6968 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/NetworkHookHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/NetworkInfoWatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/Routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3322 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/RoutingTable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/Rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3112 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-28 22:10:50.380599 pyDynamicRoutingUpdater-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 22:10:50.380599 pyDynamicRoutingUpdater-0.0.4/pyDynamicRoutingUpdater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2880 2023-05-28 22:10:50.000000 pyDynamicRoutingUpdater-0.0.4/pyDynamicRoutingUpdater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-28 22:10:50.000000 pyDynamicRoutingUpdater-0.0.4/pyDynamicRoutingUpdater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 22:10:50.000000 pyDynamicRoutingUpdater-0.0.4/pyDynamicRoutingUpdater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 22:10:50.000000 pyDynamicRoutingUpdater-0.0.4/pyDynamicRoutingUpdater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-28 22:10:50.000000 pyDynamicRoutingUpdater-0.0.4/pyDynamicRoutingUpdater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-28 22:10:50.380599 pyDynamicRoutingUpdater-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-28 22:10:38.000000 pyDynamicRoutingUpdater-0.0.4/setup.py
```

### Comparing `pyDynamicRoutingUpdater-0.0.3/DynamicRoutingUpdater/NetworkHookHandler.py` & `pyDynamicRoutingUpdater-0.0.4/DynamicRoutingUpdater/NetworkHookHandler.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 from io import TextIOWrapper
 import json, random
 from threading import Thread
 import threading
 import queue
 from typing import List
-from .objects import NetworkAdapter, RoutingManager
 import os, sys, time, re, errno
 import netifaces 
+from .objects import IpData
+from .Routing import Routing
+from .Rules import Rules
+from .NetworkAdapter import NetworkAdapter
 
 
 class NetworkHookHandler:
     """
     """
     __mainThread = threading.current_thread
     
@@ -126,35 +129,37 @@
                 else:
                     self.message_queue.put(message)
                 
                  
     
     def __processMessage(self, nic: str) -> None:
         adapter = NetworkAdapter(nic)
-        if (adapter.isValid()):
+        if (adapter.getIpData().isValid()):
             self.__routingTable_modify(adapter)
         else:
             self.stdout(f"Adding puller on {nic}")
             self.__puller_add(nic)
                 
             
     def __routingTable_modify(self, adapter: NetworkAdapter) -> None:
         """_summary_
         """
         nic_rt_table = self.nics_rt[adapter.name]
         self.stdout(f"Modifying routing for {adapter.name} on table {nic_rt_table}")
         
-        route_manager = RoutingManager()
-        route_manager.flushTable(tableName=nic_rt_table)
-        #route_manager.deleteRoute(adapter=adapter)
-        #route_manager.deleteRoute(adapter=adapter, tableName=nic_rt_table)
+        Routing.flushRoutes(table=nic_rt_table) 
+        ipData = adapter.getIpData()
+        Routing("main").deleteRoutes(ipData=ipData)
+        
+        rt = Routing(nic_rt_table)
+        rt.deleteRoutes(ipData=ipData)
+        rt.addRoutes(ipData=ipData)
         
-
-        route_manager.addRoute(adapter=adapter, tableName=nic_rt_table)
-        route_manager.addRule(adapter=adapter, tableName=nic_rt_table)
+        Rules().deleteRule(table=nic_rt_table)
+        Rules().addRule(table=nic_rt_table, source=ipData.ip)
         
             
     nicsPullerThreads: List[Thread] = []
 
     def __puller_add(self, nic: str) -> None:
         """Pulls on network adapter in seperate thread
         """
@@ -181,15 +186,15 @@
         """Thread for pulling on adapter
         """
         self.stdout(f"Starting pulling on {nic}")
         
         isInInvalidState: bool = True
         while isInInvalidState:
             time.sleep(waitTime)
-            adapter = NetworkAdapter(nic)
+            adapter = NetworkAdapter(nic).getIpData()
             isInInvalidState = not adapter.isValid()
             print(adapter)
             if (isInInvalidState == False):
                 self.__puller_remove(nic)
                 self.__routingTable_modify(adapter)
             else:
                 self.stdout(f"Pulling on {nic} in {waitTime}s")
```

### Comparing `pyDynamicRoutingUpdater-0.0.3/LICENSE` & `pyDynamicRoutingUpdater-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyDynamicRoutingUpdater-0.0.3/PKG-INFO` & `pyDynamicRoutingUpdater-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyDynamicRoutingUpdater
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library to modify and alter the routing table in according to configuration passed
-Home-page: https://github.com/bskjon/DynamicRoutingUpdater
+Home-page: https://github.com/iktdev-no/DynamicRoutingUpdater
 Author: Brage Skjønborg
 Author-email: bskjon@outlook.com
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Networking
```

### Comparing `pyDynamicRoutingUpdater-0.0.3/README.md` & `pyDynamicRoutingUpdater-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyDynamicRoutingUpdater-0.0.3/pyDynamicRoutingUpdater.egg-info/PKG-INFO` & `pyDynamicRoutingUpdater-0.0.4/pyDynamicRoutingUpdater.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pyDynamicRoutingUpdater
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library to modify and alter the routing table in according to configuration passed
-Home-page: https://github.com/bskjon/DynamicRoutingUpdater
+Home-page: https://github.com/iktdev-no/DynamicRoutingUpdater
 Author: Brage Skjønborg
 Author-email: bskjon@outlook.com
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Networking
```

### Comparing `pyDynamicRoutingUpdater-0.0.3/setup.py` & `pyDynamicRoutingUpdater-0.0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,22 +11,22 @@
     long_description_content_type='text/markdown',
     long_description=readme(),
     packages=["DynamicRoutingUpdater"],
     install_requires=[
         "netifaces>=0.11.0",
         "netaddr>=0.8.0"
     ],
-    version="0.0.3",
+    version="0.0.4",
     description="""
     A Python library to modify and alter the routing table in according to configuration passed
     """,
     python_requires=">=3.9.0",
     author="Brage Skjønborg",
     author_email="bskjon@outlook.com",
-    url="https://github.com/bskjon/DynamicRoutingUpdater",
+    url="https://github.com/iktdev-no/DynamicRoutingUpdater",
     classifiers=[
         "Intended Audience :: Developers",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Topic :: System :: Networking",
         "Topic :: Software Development :: Libraries :: Python Modules",
```


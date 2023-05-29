# Comparing `tmp/temporaluuid64-0.1.3.tar.gz` & `tmp/temporaluuid64-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/temporaluuid64-0.1.3.tar", last modified: Tue Sep 10 07:11:14 2019, max compression
+gzip compressed data, was "temporaluuid64-0.2.0.tar", last modified: Mon May 29 08:37:02 2023, max compression
```

## Comparing `temporaluuid64-0.1.3.tar` & `temporaluuid64-0.2.0.tar`

### file list

```diff
@@ -1,5 +1,13 @@
-drwxr-xr-x   0 sb         (501) staff       (20)        0 2019-09-10 07:11:14.000000 temporaluuid64-0.1.3/
--rw-r--r--   0 sb         (501) staff       (20)     1607 2019-09-10 07:11:14.000000 temporaluuid64-0.1.3/PKG-INFO
--rw-r--r--   0 sb         (501) staff       (20)     1057 2019-09-10 07:08:13.000000 temporaluuid64-0.1.3/README.rst
--rw-r--r--   0 sb         (501) staff       (20)      551 2019-09-10 07:08:13.000000 temporaluuid64-0.1.3/setup.py
--rw-r--r--   0 sb         (501) staff       (20)     1096 2019-09-10 07:09:59.000000 temporaluuid64-0.1.3/uuid64.py
+drwxr-xr-x   0 sb         (501) staff       (20)        0 2023-05-29 08:37:02.239749 temporaluuid64-0.2.0/
+-rw-r--r--   0 sb         (501) staff       (20)     1263 2023-05-29 08:37:02.239566 temporaluuid64-0.2.0/PKG-INFO
+-rw-r--r--   0 sb         (501) staff       (20)     1057 2023-05-29 07:57:13.000000 temporaluuid64-0.2.0/README.rst
+-rw-r--r--   0 sb         (501) staff       (20)       38 2023-05-29 08:37:02.239808 temporaluuid64-0.2.0/setup.cfg
+-rw-r--r--   0 sb         (501) staff       (20)      540 2023-05-29 08:32:52.000000 temporaluuid64-0.2.0/setup.py
+drwxr-xr-x   0 sb         (501) staff       (20)        0 2023-05-29 08:37:02.238860 temporaluuid64-0.2.0/temporaluuid64.egg-info/
+-rw-r--r--   0 sb         (501) staff       (20)     1263 2023-05-29 08:37:02.000000 temporaluuid64-0.2.0/temporaluuid64.egg-info/PKG-INFO
+-rw-r--r--   0 sb         (501) staff       (20)      203 2023-05-29 08:37:02.000000 temporaluuid64-0.2.0/temporaluuid64.egg-info/SOURCES.txt
+-rw-r--r--   0 sb         (501) staff       (20)        1 2023-05-29 08:37:02.000000 temporaluuid64-0.2.0/temporaluuid64.egg-info/dependency_links.txt
+-rw-r--r--   0 sb         (501) staff       (20)        7 2023-05-29 08:37:02.000000 temporaluuid64-0.2.0/temporaluuid64.egg-info/top_level.txt
+drwxr-xr-x   0 sb         (501) staff       (20)        0 2023-05-29 08:37:02.239105 temporaluuid64-0.2.0/tests/
+-rw-r--r--   0 sb         (501) staff       (20)      690 2023-05-29 08:32:52.000000 temporaluuid64-0.2.0/tests/test_overall.py
+-rw-r--r--   0 sb         (501) staff       (20)     1294 2023-05-29 08:32:56.000000 temporaluuid64-0.2.0/uuid64.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `temporaluuid64-0.1.3/README.rst` & `temporaluuid64-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `temporaluuid64-0.1.3/uuid64.py` & `temporaluuid64-0.2.0/uuid64.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,47 +6,51 @@
 
 from datetime import datetime
 import os
 import struct
 import socket
 import time
 
-__author__ = 'Sumin Byeon'
-__email__ = 'suminb@gmail.com'
-__version__ = '0.1.3'
+from typing import Optional
+
+__author__ = "Sumin Byeon"
+__email__ = "suminb@gmail.com"
+__version__ = "0.2.0"
 
 
 EPOCH = datetime(2015, 8, 1)
 
 
 def ipv4_to_int(addr):
     """Converts an IPv4 address in a string format to a 32-bit integer."""
     return struct.unpack("!I", socket.inet_aton(addr))[0]
 
 
 def uuid64_fields(uuid64):
     """
     :type uuid64: int
     """
-    return (uuid64 >> 48, uuid64 & 0xFFFF)
+    return ((uuid64 >> 16) / 10000, uuid64 & 0xFFFF)
 
 
-class UUID64(object):
+class UUID64:
     def __init__(self, node_id):
         self.node_id = node_id
 
-    def issue(self):
-        time_seq = int(time.time() * 10000)
+    def issue(self, current_time: Optional[datetime] = None) -> int:
+        if current_time is None:
+            current_time = datetime.utcnow()
+        time_seq = int(current_time.timestamp() * 10000)
 
-        return int(time_seq << 16 | (self.node_id & 0xFFFF) )
+        return int(time_seq << 16 | (self.node_id & 0xFFFF))
 
 
-def issue(node_id=None):
+def issue(current_time=None, node_id=None):
     if node_id is None:
         try:
             host = socket.gethostbyname(socket.gethostname())
         except socket.gaierror:
-            host = '127.0.0.1'
-        local_ip = os.environ.get('IPV4_ADDR', host)
-        node_id = ipv4_to_int(local_ip) % (2 ** 16)
+            host = "127.0.0.1"
+        local_ip = os.environ.get("IPV4_ADDR", host)
+        node_id = ipv4_to_int(local_ip) % (2**16)
     uuid = UUID64(node_id)
-    return uuid.issue()
+    return uuid.issue(current_time)
```


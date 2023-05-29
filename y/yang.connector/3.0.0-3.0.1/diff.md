# Comparing `tmp/yang.connector-3.0.0-py3-none-any.whl.zip` & `tmp/yang.connector-3.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,13 @@
-Zip file size: 9464 bytes, number of entries: 9
--rw-r--r--  2.0 unx      529 b- defN 18-Dec-04 18:52 yang.connector-3.0.0-py3.5-nspkg.pth
--rw-r--r--  2.0 unx    18469 b- defN 18-Dec-04 16:50 yang/connector/__init__.py
--rw-r--r--  2.0 unx       99 b- defN 18-Nov-13 15:24 yang/connector/tests/__init__.py
--rw-r--r--  2.0 unx     8352 b- defN 18-Dec-03 19:49 yang/connector/tests/test_yang.py
--rw-r--r--  2.0 unx     1319 b- defN 18-Dec-04 18:52 yang.connector-3.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 18-Dec-04 18:52 yang.connector-3.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 18-Dec-04 18:52 yang.connector-3.0.0.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx        5 b- defN 18-Dec-04 18:52 yang.connector-3.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      785 b- defN 18-Dec-04 18:47 yang.connector-3.0.0.dist-info/RECORD
-9 files, 29655 bytes uncompressed, 8086 bytes compressed:  72.7%
+Zip file size: 10662 bytes, number of entries: 11
+-rw-r--r--  2.0 unx      529 b- defN 19-May-31 22:08 yang.connector-3.0.1-py3.6-nspkg.pth
+-rw-r--r--  2.0 unx    18849 b- defN 19-May-31 22:02 yang/connector/__init__.py
+-rw-r--r--  2.0 unx       99 b- defN 19-May-31 21:36 yang/connector/tests/__init__.py
+-rw-r--r--  2.0 unx     8352 b- defN 19-May-31 21:36 yang/connector/tests/test_yang.py
+-rw-r--r--  2.0 unx       40 b- defN 19-May-31 22:08 yang.connector-3.0.1.dist-info/DESCRIPTION.rst
+-rw-r--r--  2.0 unx     1195 b- defN 19-May-31 22:08 yang.connector-3.0.1.dist-info/metadata.json
+-rw-r--r--  2.0 unx        5 b- defN 19-May-31 22:08 yang.connector-3.0.1.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx        5 b- defN 19-May-31 22:08 yang.connector-3.0.1.dist-info/top_level.txt
+-rw-r--r--  2.0 unx       92 b- defN 19-May-31 22:08 yang.connector-3.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx     1195 b- defN 19-May-31 22:08 yang.connector-3.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx      998 b- defN 19-May-31 22:08 yang.connector-3.0.1.dist-info/RECORD
+11 files, 31359 bytes uncompressed, 8952 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -1,28 +1,34 @@
-Filename: yang.connector-3.0.0-py3.5-nspkg.pth
+Filename: yang.connector-3.0.1-py3.6-nspkg.pth
 Comment: 
 
 Filename: yang/connector/__init__.py
 Comment: 
 
 Filename: yang/connector/tests/__init__.py
 Comment: 
 
 Filename: yang/connector/tests/test_yang.py
 Comment: 
 
-Filename: yang.connector-3.0.0.dist-info/METADATA
+Filename: yang.connector-3.0.1.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: yang.connector-3.0.0.dist-info/WHEEL
+Filename: yang.connector-3.0.1.dist-info/metadata.json
 Comment: 
 
-Filename: yang.connector-3.0.0.dist-info/namespace_packages.txt
+Filename: yang.connector-3.0.1.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: yang.connector-3.0.0.dist-info/top_level.txt
+Filename: yang.connector-3.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: yang.connector-3.0.0.dist-info/RECORD
+Filename: yang.connector-3.0.1.dist-info/WHEEL
+Comment: 
+
+Filename: yang.connector-3.0.1.dist-info/METADATA
+Comment: 
+
+Filename: yang.connector-3.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## yang/connector/__init__.py

```diff
@@ -1,13 +1,13 @@
 """yang.connector module defines a set of classes that connect to Data Model
 Interfaces (DMI), in particular, an implementation of Netconf client by
 wrapping up ncclient package. Restconf implementation is coming next."""
 
 # metadata
-__version__ = '3.0.0'
+__version__ = '3.0.1'
 __author__ = ('Jonathan Yang <yuekyang@cisco.com>',
               'Siming Yuan <siyuan@cisco.com',)
 __contact__ = 'yang-python@cisco.com'
 __copyright__ = 'Cisco Systems, Inc.'
 
 
 import re
@@ -16,30 +16,36 @@
 import logging
 from ncclient import manager
 from ncclient import operations
 from ncclient import transport
 from ncclient.devices.default import DefaultDeviceHandler
 from ncclient.operations.errors import TimeoutExpiredError
 
-from pyats.connections import BaseConnection
+try:
+    from pyats.connections import BaseConnection
+except ImportError:
+    try:
+        from ats.connections import BaseConnection
+    except ImportError:
+        raise ImportError('Cannot import pyATS - make sure pyATS is installed ' 
+                          'in your environment') from None
 
 # try to record usage statistics
 #  - only internal cisco users will have stats.CesMonitor module
 #  - below code does nothing for DevNet users -  we DO NOT track usage stats
 #    for PyPI/public/customer users
 try:
     # new internal cisco-only pkg since devnet release
     from ats.cisco.stats import CesMonitor
 except Exception:
     try:
         # legacy pyats version, stats was inside utils module
         from ats.utils.stats import CesMonitor
     except Exception:
         CesMonitor = None
-
 finally:
     if CesMonitor is not None:
         # CesMonitor exists -> this is an internal cisco user
         CesMonitor(action = __name__, application='pyATS Packages').post()
 
 # create a logger for this module
 logger = logging.getLogger(__name__)
@@ -130,45 +136,36 @@
         synchronously (False). The default value is False.
     '''
 
     def __init__(self, *args, **kwargs):
         '''
         __init__ instantiates a single connection instance.
         '''
+        # set defaults
+        kwargs.setdefault('timeout', 30)
 
         # instanciate BaseConnection
         # (could use super...)
         BaseConnection.__init__(self, *args, **kwargs)
 
-        # default values
-        defaults = {
-            'async_mode': False,
-            'raise_mode': 0,
-            'timeout': 30,
-            }
-        defaults = {k: self.connection_info.get(k, v) for k, v in defaults.items()}
-        defaults = {k: kwargs.get(k, v) for k, v in defaults.items()}
-
         # shortwire Ncclient device handling portion
         # and create just the DeviceHandler
         device_handler = DefaultDeviceHandler()
 
         # create the session instance
         session = transport.SSHSession(device_handler)
 
         # load known_hosts file (if available)
         session.load_known_hosts()
 
         # instanciate ncclient Manager
         # (can't use super due to mro change)
         manager.Manager.__init__(self, session = session,
                                        device_handler = device_handler,
-                                       *args, **defaults)
-        for item in ['async_mode', 'raise_mode']:
-            setattr(self, item, defaults[item])
+                                       timeout = self.timeout)
 
     @property
     def session(self):
         '''session
 
         High-level api: return the SSH session object.
 
@@ -303,25 +300,37 @@
             'hostkey_verify': False,
             'look_for_keys': False,
             'ssh_config': None,
             }
         defaults.update(self.connection_info)
 
         # remove items
-        disregards = ['class', 'model', 'protocol', 'async_mode', 'raise_mode']
+        disregards = ['class', 'model', 'protocol', 
+                      'async_mode', 'raise_mode', 'credentials']
         defaults = {k: v for k, v in defaults.items() if k not in disregards}
 
         # rename ip -> host, cast to str type
         if 'ip' in defaults:
             defaults['host'] = str(defaults.pop('ip'))
 
         # rename user -> username
         if 'user' in defaults:
             defaults['username'] = str(defaults.pop('user'))
 
+        # check credentials
+        if self.connection_info.get('credentials'):
+            try:
+                defaults['username'] = str(self.connection_info['credentials']['netconf']['username'])
+            except Exception:
+                pass
+            try:
+                defaults['password'] = str(self.connection_info['credentials']['netconf']['password'])
+            except Exception:
+                pass
+
         defaults = {k: getattr(self, k, v) for k, v in defaults.items()}
 
         try:
             self.session.connect(**defaults)
         except Exception:
             if self.session.transport:
                 self.session.close()
```

## Comparing `yang.connector-3.0.0-py3.5-nspkg.pth` & `yang.connector-3.0.1-py3.6-nspkg.pth`

 * *Files identical despite different names*

## Comparing `yang.connector-3.0.0.dist-info/METADATA` & `yang.connector-3.0.1.dist-info/METADATA`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,34 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.0
 Name: yang.connector
-Version: 3.0.0
+Version: 3.0.1
 Summary: A NETCONF connector
 Home-page: https://github.com/CiscoTestAutomation/yang.git
 Author: Jonathan Yang
-Author-email: yuekyang@cisco.com
-Maintainer-email: yang-python@cisco.com
+Author-email: yang-python@cisco.com
 License: Apache 2.0
+Description-Content-Type: UNKNOWN
 Keywords: pyats cisco-shared
-Platform: CEL
+Platform: Linux
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Telecommunications Industry
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Testing
 Requires-Dist: paramiko (>=1.15.1)
 Requires-Dist: lxml (>=3.3.0)
-Requires-Dist: ncclient (>=0.5.2)
-Requires-Dist: pyats.log (>=5.0.0)
-Requires-Dist: pyats.connections (>=5.0.0)
-Requires-Dist: pyats.topology (>=5.0.0)
+Requires-Dist: ncclient (>=0.6.6)
 Provides-Extra: dev
-Requires-Dist: coverage ; extra == 'dev'
-Requires-Dist: restview ; extra == 'dev'
-Requires-Dist: Sphinx ; extra == 'dev'
-Requires-Dist: sphinxcontrib-napoleon ; extra == 'dev'
-Requires-Dist: sphinx-rtd-theme ; extra == 'dev'
+Requires-Dist: coverage; extra == 'dev'
+Requires-Dist: restview; extra == 'dev'
+Requires-Dist: Sphinx; extra == 'dev'
+Requires-Dist: sphinxcontrib-napoleon; extra == 'dev'
+Requires-Dist: sphinx-rtd-theme; extra == 'dev'
 
 A NETCONF connector based on ncclient
```


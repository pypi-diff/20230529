# Comparing `tmp/Mopiqtt-1.0.8.tar.gz` & `tmp/Mopiqtt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Mopiqtt-1.0.8.tar", last modified: Wed Jun 29 11:24:36 2022, max compression
+gzip compressed data, was "dist/Mopiqtt-1.0.9.tar", last modified: Fri Jul  1 10:01:59 2022, max compression
```

## Comparing `Mopiqtt-1.0.8.tar` & `Mopiqtt-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwx------   0 fabio      (501) staff       (20)        0 2022-06-29 11:24:36.000000 Mopiqtt-1.0.8/
--rwx------   0 fabio      (501) staff       (20)     1207 2022-06-29 11:22:13.000000 Mopiqtt-1.0.8/CHANGELOG.md
--rwx------   0 fabio      (501) staff       (20)    11324 2022-05-27 12:07:31.000000 Mopiqtt-1.0.8/LICENSE
--rwx------   0 fabio      (501) staff       (20)      133 2022-05-27 12:10:38.000000 Mopiqtt-1.0.8/MANIFEST.in
-drwx------   0 fabio      (501) staff       (20)        0 2022-06-29 11:24:35.000000 Mopiqtt-1.0.8/Mopiqtt.egg-info/
--rwx------   0 fabio      (501) staff       (20)     7044 2022-06-29 11:24:35.000000 Mopiqtt-1.0.8/Mopiqtt.egg-info/PKG-INFO
--rwx------   0 fabio      (501) staff       (20)      445 2022-06-29 11:24:35.000000 Mopiqtt-1.0.8/Mopiqtt.egg-info/SOURCES.txt
--rwx------   0 fabio      (501) staff       (20)        1 2022-06-29 11:24:35.000000 Mopiqtt-1.0.8/Mopiqtt.egg-info/dependency_links.txt
--rwx------   0 fabio      (501) staff       (20)       42 2022-06-29 11:24:35.000000 Mopiqtt-1.0.8/Mopiqtt.egg-info/entry_points.txt
--rwx------   0 fabio      (501) staff       (20)        1 2022-05-28 09:38:06.000000 Mopiqtt-1.0.8/Mopiqtt.egg-info/not-zip-safe
--rwx------   0 fabio      (501) staff       (20)       44 2022-06-29 11:24:35.000000 Mopiqtt-1.0.8/Mopiqtt.egg-info/requires.txt
--rwx------   0 fabio      (501) staff       (20)        8 2022-06-29 11:24:35.000000 Mopiqtt-1.0.8/Mopiqtt.egg-info/top_level.txt
--rwx------   0 fabio      (501) staff       (20)     7044 2022-06-29 11:24:36.000000 Mopiqtt-1.0.8/PKG-INFO
--rwx------   0 fabio      (501) staff       (20)     5242 2022-06-29 11:22:13.000000 Mopiqtt-1.0.8/README.md
-drwx------   0 fabio      (501) staff       (20)        0 2022-06-29 11:24:36.000000 Mopiqtt-1.0.8/mopiqtt/
--rwx------   0 fabio      (501) staff       (20)      962 2022-06-29 11:22:13.000000 Mopiqtt-1.0.8/mopiqtt/__init__.py
--rwx------   0 fabio      (501) staff       (20)       98 2022-05-27 12:16:29.000000 Mopiqtt-1.0.8/mopiqtt/ext.conf
--rwx------   0 fabio      (501) staff       (20)    10882 2022-06-29 11:22:13.000000 Mopiqtt-1.0.8/mopiqtt/frontend.py
--rwx------   0 fabio      (501) staff       (20)     2873 2022-06-06 08:24:45.000000 Mopiqtt-1.0.8/mopiqtt/mqtt.py
--rwx------   0 fabio      (501) staff       (20)     1462 2022-06-29 11:22:13.000000 Mopiqtt-1.0.8/mopiqtt/utils.py
--rwx------   0 fabio      (501) staff       (20)     2230 2022-06-11 08:12:33.000000 Mopiqtt-1.0.8/mynotes.txt
--rwx------   0 fabio      (501) staff       (20)      132 2022-06-29 11:24:36.000000 Mopiqtt-1.0.8/setup.cfg
--rwx------   0 fabio      (501) staff       (20)     1509 2022-05-28 11:27:17.000000 Mopiqtt-1.0.8/setup.py
-drwx------   0 fabio      (501) staff       (20)        0 2022-06-29 11:24:36.000000 Mopiqtt-1.0.8/tests/
--rwx------   0 fabio      (501) staff       (20)        0 2022-01-01 18:29:13.000000 Mopiqtt-1.0.8/tests/__init__.py
--rwx------   0 fabio      (501) staff       (20)      410 2022-01-01 18:29:13.000000 Mopiqtt-1.0.8/tests/conftest.py
--rwx------   0 fabio      (501) staff       (20)      367 2022-06-06 08:24:45.000000 Mopiqtt-1.0.8/tests/test_smoke.py
--rwx------   0 fabio      (501) staff       (20)      294 2022-05-27 12:10:12.000000 Mopiqtt-1.0.8/tox.ini
+drwx------   0 fabio      (501) staff       (20)        0 2022-07-01 10:01:59.000000 Mopiqtt-1.0.9/
+-rwx------   0 fabio      (501) staff       (20)     1327 2022-07-01 10:00:13.000000 Mopiqtt-1.0.9/CHANGELOG.md
+-rwx------   0 fabio      (501) staff       (20)    11324 2022-05-27 12:07:31.000000 Mopiqtt-1.0.9/LICENSE
+-rwx------   0 fabio      (501) staff       (20)      133 2022-05-27 12:10:38.000000 Mopiqtt-1.0.9/MANIFEST.in
+drwx------   0 fabio      (501) staff       (20)        0 2022-07-01 10:01:59.000000 Mopiqtt-1.0.9/Mopiqtt.egg-info/
+-rwx------   0 fabio      (501) staff       (20)     7044 2022-07-01 10:01:58.000000 Mopiqtt-1.0.9/Mopiqtt.egg-info/PKG-INFO
+-rwx------   0 fabio      (501) staff       (20)      445 2022-07-01 10:01:59.000000 Mopiqtt-1.0.9/Mopiqtt.egg-info/SOURCES.txt
+-rwx------   0 fabio      (501) staff       (20)        1 2022-07-01 10:01:58.000000 Mopiqtt-1.0.9/Mopiqtt.egg-info/dependency_links.txt
+-rwx------   0 fabio      (501) staff       (20)       42 2022-07-01 10:01:58.000000 Mopiqtt-1.0.9/Mopiqtt.egg-info/entry_points.txt
+-rwx------   0 fabio      (501) staff       (20)        1 2022-05-28 09:38:06.000000 Mopiqtt-1.0.9/Mopiqtt.egg-info/not-zip-safe
+-rwx------   0 fabio      (501) staff       (20)       44 2022-07-01 10:01:58.000000 Mopiqtt-1.0.9/Mopiqtt.egg-info/requires.txt
+-rwx------   0 fabio      (501) staff       (20)        8 2022-07-01 10:01:58.000000 Mopiqtt-1.0.9/Mopiqtt.egg-info/top_level.txt
+-rwx------   0 fabio      (501) staff       (20)     7044 2022-07-01 10:01:59.000000 Mopiqtt-1.0.9/PKG-INFO
+-rwx------   0 fabio      (501) staff       (20)     5242 2022-06-29 11:22:13.000000 Mopiqtt-1.0.9/README.md
+drwx------   0 fabio      (501) staff       (20)        0 2022-07-01 10:01:59.000000 Mopiqtt-1.0.9/mopiqtt/
+-rwx------   0 fabio      (501) staff       (20)      962 2022-07-01 09:57:08.000000 Mopiqtt-1.0.9/mopiqtt/__init__.py
+-rwx------   0 fabio      (501) staff       (20)       98 2022-05-27 12:16:29.000000 Mopiqtt-1.0.9/mopiqtt/ext.conf
+-rwx------   0 fabio      (501) staff       (20)    10882 2022-06-29 11:22:13.000000 Mopiqtt-1.0.9/mopiqtt/frontend.py
+-rwx------   0 fabio      (501) staff       (20)     2881 2022-07-01 09:52:26.000000 Mopiqtt-1.0.9/mopiqtt/mqtt.py
+-rwx------   0 fabio      (501) staff       (20)     1462 2022-06-29 11:22:13.000000 Mopiqtt-1.0.9/mopiqtt/utils.py
+-rwx------   0 fabio      (501) staff       (20)     2253 2022-06-29 11:25:22.000000 Mopiqtt-1.0.9/mynotes.txt
+-rwx------   0 fabio      (501) staff       (20)      132 2022-07-01 10:01:59.000000 Mopiqtt-1.0.9/setup.cfg
+-rwx------   0 fabio      (501) staff       (20)     1509 2022-05-28 11:27:17.000000 Mopiqtt-1.0.9/setup.py
+drwx------   0 fabio      (501) staff       (20)        0 2022-07-01 10:01:59.000000 Mopiqtt-1.0.9/tests/
+-rwx------   0 fabio      (501) staff       (20)        0 2022-01-01 18:29:13.000000 Mopiqtt-1.0.9/tests/__init__.py
+-rwx------   0 fabio      (501) staff       (20)      410 2022-01-01 18:29:13.000000 Mopiqtt-1.0.9/tests/conftest.py
+-rwx------   0 fabio      (501) staff       (20)      367 2022-06-06 08:24:45.000000 Mopiqtt-1.0.9/tests/test_smoke.py
+-rwx------   0 fabio      (501) staff       (20)      294 2022-05-27 12:10:12.000000 Mopiqtt-1.0.9/tox.ini
```

### Comparing `Mopiqtt-1.0.8/CHANGELOG.md` & `Mopiqtt-1.0.9/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Changelog
 
+## 1.0.9
+* Bugfix on mqtt username (Credit: @hirschharald) Closes [#2](https://github.com/fmarzocca/Mopiqtt/issues/2) 
+
 ## 1.0.8
 * Local artwork is not supported
 
 ## 1.0.7
 * Added `mopidy/cmnd/queryschemes` to request a list of uri-schemes Mopidy can handle in searches
 * Added `mopidy/stat/uri_schemes` to get a list of uri-schemes Mopidy can handle in searches
 * Added `mopidy/cmnd/search` to search libraries for any string (artist, album, track)
```

### Comparing `Mopiqtt-1.0.8/LICENSE` & `Mopiqtt-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `Mopiqtt-1.0.8/Mopiqtt.egg-info/PKG-INFO` & `Mopiqtt-1.0.9/Mopiqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopiqtt
-Version: 1.0.8
+Version: 1.0.9
 Summary: Control mopidy music server through MQTT broker
 Home-page: https://github.com/fmarzocca/mopiqtt
 Author: Fabio Marzocca
 Author-email: marzoccafabio@gmail.com
 License: Apache License, Version 2.0
 Description: Based on [mopidy-mqtt](https://github.com/odiroot/mopidy-mqtt)
```

### Comparing `Mopiqtt-1.0.8/PKG-INFO` & `Mopiqtt-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Mopiqtt
-Version: 1.0.8
+Version: 1.0.9
 Summary: Control mopidy music server through MQTT broker
 Home-page: https://github.com/fmarzocca/mopiqtt
 Author: Fabio Marzocca
 Author-email: marzoccafabio@gmail.com
 License: Apache License, Version 2.0
 Description: Based on [mopidy-mqtt](https://github.com/odiroot/mopidy-mqtt)
```

### Comparing `Mopiqtt-1.0.8/README.md` & `Mopiqtt-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `Mopiqtt-1.0.8/mopiqtt/__init__.py` & `Mopiqtt-1.0.9/mopiqtt/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import absolute_import
 import logging
 import os
 
 from mopidy import config, ext
 
 
-__version__ = '1.0.8'
+__version__ = '1.0.9'
 logger = logging.getLogger(__name__)
 
 
 class Extension(ext.Extension):
 
     dist_name = 'Mopiqtt'
     ext_name = 'mopiqtt'
```

### Comparing `Mopiqtt-1.0.8/mopiqtt/frontend.py` & `Mopiqtt-1.0.9/mopiqtt/frontend.py`

 * *Files identical despite different names*

### Comparing `Mopiqtt-1.0.8/mopiqtt/mqtt.py` & `Mopiqtt-1.0.9/mopiqtt/mqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,24 +9,24 @@
 
 HANDLER_PREFIX = 'on_action_'
 
 
 class Comms:
     def __init__(
             self, frontend, host='localhost', port=1883, topic='mopidy',
-            user=None, password=None, **kwargs):
+            username=None, password=None, **kwargs):
         """
         Configure MQTT communication client.
         frontend (MopiqttFrontend): Instance of extension's frontend.
         """
         self.frontend = frontend
         self.host = host
         self.port = port
         self.topic = topic
-        self.user = user
+        self.user = username
         self.password = password
 
         self.client = mqtt.Client(
             client_id='mopidy-{}'.format(getpid()), clean_session=True)
         self.client.on_connect = self._on_connect
         self.client.on_message = self._on_message
```

### Comparing `Mopiqtt-1.0.8/mopiqtt/utils.py` & `Mopiqtt-1.0.9/mopiqtt/utils.py`

 * *Files identical despite different names*

### Comparing `Mopiqtt-1.0.8/mynotes.txt` & `Mopiqtt-1.0.9/mynotes.txt`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - Fai il merge di Development in main su GitHub
 
 
 prima genera un sdist:
 
 python3 setup.py sdist
 
-poiTest Pypi: (https://test.pypi.org/)
+poiTest Pypi: (https://test.pypi.org/) (ut: fm... pwd: Eg...)
 
 twine upload --repository testpypi dist/* 
 
 Pubblicazione su PyPi:
 twine upload dist/*
 
 Release su GitHub web
```

### Comparing `Mopiqtt-1.0.8/setup.py` & `Mopiqtt-1.0.9/setup.py`

 * *Files identical despite different names*


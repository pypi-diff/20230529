# Comparing `tmp/cs-eventsender-0.0.1.tar.gz` & `tmp/cs-eventsender-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-eventsender-0.0.1.tar", last modified: Mon May 29 07:45:20 2023, max compression
+gzip compressed data, was "cs-eventsender-0.0.2.tar", last modified: Mon May 29 10:41:37 2023, max compression
```

## Comparing `cs-eventsender-0.0.1.tar` & `cs-eventsender-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:45:20.808050 cs-eventsender-0.0.1/
--rw-rw-rw-   0        0        0      509 2023-05-29 07:45:20.808050 cs-eventsender-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 07:45:20.794049 cs-eventsender-0.0.1/cs_eventsender.egg-info/
--rw-rw-rw-   0        0        0      509 2023-05-29 07:45:20.000000 cs-eventsender-0.0.1/cs_eventsender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-29 07:45:20.000000 cs-eventsender-0.0.1/cs_eventsender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:45:20.000000 cs-eventsender-0.0.1/cs_eventsender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-29 07:45:20.000000 cs-eventsender-0.0.1/cs_eventsender.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 07:45:20.000000 cs-eventsender-0.0.1/cs_eventsender.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 07:45:20.806133 cs-eventsender-0.0.1/eventsender/
--rw-rw-rw-   0        0        0       37 2023-05-29 07:36:13.000000 cs-eventsender-0.0.1/eventsender/__init__.py
--rw-rw-rw-   0        0        0     2176 2023-05-29 07:41:27.000000 cs-eventsender-0.0.1/eventsender/event_sender.py
--rw-rw-rw-   0        0        0       42 2023-05-29 07:45:20.809048 cs-eventsender-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-05-29 07:45:01.000000 cs-eventsender-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 10:41:37.739871 cs-eventsender-0.0.2/
+-rw-rw-rw-   0        0        0      509 2023-05-29 10:41:37.738865 cs-eventsender-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-29 10:41:37.721276 cs-eventsender-0.0.2/cs_eventsender.egg-info/
+-rw-rw-rw-   0        0        0      509 2023-05-29 10:41:37.000000 cs-eventsender-0.0.2/cs_eventsender.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2023-05-29 10:41:37.000000 cs-eventsender-0.0.2/cs_eventsender.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 10:41:37.000000 cs-eventsender-0.0.2/cs_eventsender.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-05-29 10:41:37.000000 cs-eventsender-0.0.2/cs_eventsender.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-29 10:41:37.000000 cs-eventsender-0.0.2/cs_eventsender.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-29 10:41:37.736359 cs-eventsender-0.0.2/eventsender/
+-rw-rw-rw-   0        0        0       37 2023-05-29 07:36:13.000000 cs-eventsender-0.0.2/eventsender/__init__.py
+-rw-rw-rw-   0        0        0     2178 2023-05-29 10:39:33.000000 cs-eventsender-0.0.2/eventsender/event_sender.py
+-rw-rw-rw-   0        0        0       42 2023-05-29 10:41:37.739871 cs-eventsender-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      846 2023-05-29 10:41:18.000000 cs-eventsender-0.0.2/setup.py
```

### Comparing `cs-eventsender-0.0.1/eventsender/event_sender.py` & `cs-eventsender-0.0.2/eventsender/event_sender.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 
         if response.status_code != 200:
             logging.error(
                 f"Failed to send data to server. Status code: {response.status_code}. Response: {response.text}")
             return False
         return True
 
-    def _send_to_telegram(self, data_type, message):
+    def _send_to_telegram(self, chat_id, message):
         try:
-            self.telegram_client.send_message(data_type, message)
+            self.telegram_client.send_message(chat_id, message)
         except Exception as e:
             logging.error(
                 f"Failed to send message to telegram. Exception: {e}")
             return False
         return True
 
     def send_data(self, status, data):
@@ -50,10 +50,10 @@
         data_type = data.__tablename__
         event_type = f"{status}_{data_type}"
 
         message = data.generate_new_message(
         ) if status == "new" else data.generate_update_message()
 
         server_success = self._send_to_server(event_type, data)
-        telegram_success = self._send_to_telegram(data_type, message)
+        telegram_success = self._send_to_telegram(data.__chatid__, message)
 
         return server_success and telegram_success
```

### Comparing `cs-eventsender-0.0.1/setup.py` & `cs-eventsender-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'A package for sending event notifications.'
 
 # Setting up
 setup(
     name="cs-eventsender",
     version=VERSION,
     author="Richard",
```


# Comparing `tmp/cs-eventsender-0.0.2.tar.gz` & `tmp/cs-eventsender-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-eventsender-0.0.2.tar", last modified: Mon May 29 10:41:37 2023, max compression
+gzip compressed data, was "cs-eventsender-0.0.4.tar", last modified: Mon May 29 19:01:51 2023, max compression
```

## Comparing `cs-eventsender-0.0.2.tar` & `cs-eventsender-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 10:41:37.739871 cs-eventsender-0.0.2/
--rw-rw-rw-   0        0        0      509 2023-05-29 10:41:37.738865 cs-eventsender-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-29 10:41:37.721276 cs-eventsender-0.0.2/cs_eventsender.egg-info/
--rw-rw-rw-   0        0        0      509 2023-05-29 10:41:37.000000 cs-eventsender-0.0.2/cs_eventsender.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2023-05-29 10:41:37.000000 cs-eventsender-0.0.2/cs_eventsender.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 10:41:37.000000 cs-eventsender-0.0.2/cs_eventsender.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-05-29 10:41:37.000000 cs-eventsender-0.0.2/cs_eventsender.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-29 10:41:37.000000 cs-eventsender-0.0.2/cs_eventsender.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 10:41:37.736359 cs-eventsender-0.0.2/eventsender/
--rw-rw-rw-   0        0        0       37 2023-05-29 07:36:13.000000 cs-eventsender-0.0.2/eventsender/__init__.py
--rw-rw-rw-   0        0        0     2178 2023-05-29 10:39:33.000000 cs-eventsender-0.0.2/eventsender/event_sender.py
--rw-rw-rw-   0        0        0       42 2023-05-29 10:41:37.739871 cs-eventsender-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      846 2023-05-29 10:41:18.000000 cs-eventsender-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:01:51.935941 cs-eventsender-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-29 19:01:51.935941 cs-eventsender-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 19:01:34.000000 cs-eventsender-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:01:51.935941 cs-eventsender-0.0.4/cs_eventsender.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-29 19:01:51.000000 cs-eventsender-0.0.4/cs_eventsender.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-29 19:01:51.000000 cs-eventsender-0.0.4/cs_eventsender.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:01:51.000000 cs-eventsender-0.0.4/cs_eventsender.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-29 19:01:51.000000 cs-eventsender-0.0.4/cs_eventsender.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-29 19:01:51.000000 cs-eventsender-0.0.4/cs_eventsender.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:01:51.935941 cs-eventsender-0.0.4/eventsender/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-29 19:01:34.000000 cs-eventsender-0.0.4/eventsender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-29 19:01:34.000000 cs-eventsender-0.0.4/eventsender/event_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:01:51.935941 cs-eventsender-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-29 19:01:34.000000 cs-eventsender-0.0.4/setup.py
```

### Comparing `cs-eventsender-0.0.2/eventsender/event_sender.py` & `cs-eventsender-0.0.4/eventsender/event_sender.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,59 +1,63 @@
-import logging
-import os
-import requests
-from cs_telegram_bot import TelegramClient
-
-
-class EventSender:
-    def __init__(self, server_url=None, api_key=None):
-        self.server_url = server_url or os.getenv("REACT_APP_API_URL")
-        if not self.server_url:
-            raise ValueError(
-                "Server URL is not set. It must be provided during initialization or set in the environment variables.")
-
-        self.api_key = api_key or os.getenv("FLASK_APP_API_KEY")
-        if not self.api_key:
-            raise ValueError(
-                "API key is not set. It must be provided during initialization or set in the environment variables.")
-
-        self.telegram_client = TelegramClient()
-
-    def _send_to_server(self, event_type, data):
-        payload = {
-            "event_type": event_type,
-            "data": data.to_dict()
-        }
-        headers = {'X-Api-Key': self.api_key}
-        response = requests.post(
-            f"{self.server_url}/events/send", json=payload, headers=headers)
-
-        if response.status_code != 200:
-            logging.error(
-                f"Failed to send data to server. Status code: {response.status_code}. Response: {response.text}")
-            return False
-        return True
-
-    def _send_to_telegram(self, chat_id, message):
-        try:
-            self.telegram_client.send_message(chat_id, message)
-        except Exception as e:
-            logging.error(
-                f"Failed to send message to telegram. Exception: {e}")
-            return False
-        return True
-
-    def send_data(self, status, data):
-        if status not in ["new", "update"]:
-            raise ValueError(
-                "Invalid status. It must be either 'new' or 'update'.")
-
-        data_type = data.__tablename__
-        event_type = f"{status}_{data_type}"
-
-        message = data.generate_new_message(
-        ) if status == "new" else data.generate_update_message()
-
-        server_success = self._send_to_server(event_type, data)
-        telegram_success = self._send_to_telegram(data.__chatid__, message)
-
+import logging
+import os
+import requests
+from cs_telegram_bot import TelegramClient
+
+
+class EventSender:
+    def __init__(self, server_url=None, api_key=None):
+        self.server_url = server_url or os.getenv("REACT_APP_API_URL")
+        if not self.server_url:
+            raise ValueError(
+                "Server URL is not set. It must be provided during initialization or set in the environment variables.")
+
+        self.api_key = api_key or os.getenv("FLASK_APP_API_KEY")
+        if not self.api_key:
+            raise ValueError(
+                "API key is not set. It must be provided during initialization or set in the environment variables.")
+
+        self.telegram_client = TelegramClient()
+
+    def _send_to_server(self, event_type, data):
+        payload = {
+            "event_type": event_type,
+            "data": data.to_dict()
+        }
+        headers = {'X-Api-Key': self.api_key}
+        
+        try:
+            response = requests.post(
+                f"{self.server_url}/events/send", json=payload, headers=headers)
+            
+            response.raise_for_status()  # Raise an exception for non-200 status codes
+            
+            return True
+        
+        except requests.exceptions.RequestException as e:
+            logging.error(f"Failed to send data to server. Error: {str(e)}")
+            return False
+
+    def _send_to_telegram(self, chat_id, message):
+        try:
+            self.telegram_client.send_message(chat_id, message)
+        except Exception as e:
+            logging.error(
+                f"Failed to send message to telegram. Exception: {e}")
+            return False
+        return True
+
+    def send_data(self, status, data):
+        if status not in ["new", "update"]:
+            raise ValueError(
+                "Invalid status. It must be either 'new' or 'update'.")
+
+        data_type = data.__tablename__
+        event_type = f"{status}_{data_type}"
+
+        message = data.generate_new_message(
+        ) if status == "new" else data.generate_update_message()
+
+        server_success = self._send_to_server(event_type, data)
+        telegram_success = self._send_to_telegram(data.__chatid__, message)
+
         return server_success and telegram_success
```

### Comparing `cs-eventsender-0.0.2/setup.py` & `cs-eventsender-0.0.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from setuptools import setup, find_packages
-import codecs
-import os
-
-here = os.path.abspath(os.path.dirname(__file__))
-
-VERSION = '0.0.2'
-DESCRIPTION = 'A package for sending event notifications.'
-
-# Setting up
-setup(
-    name="cs-eventsender",
-    version=VERSION,
-    author="Richard",
-    author_email="<rich_swainson@hotmail.co.uk>",
-    description=DESCRIPTION,
-    packages=find_packages(),
-    install_requires=['requests','cs-telegram-bot-api'],
-    keywords=['binance', 'api', 'wrapper', 'c2c', 'sapi'],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Developers",
-        "Programming Language :: Python :: 3",
-        "Operating System :: Unix",
-        "Operating System :: MacOS :: MacOS X",
-        "Operating System :: Microsoft :: Windows",
-    ]
+from setuptools import setup, find_packages
+import codecs
+import os
+
+here = os.path.abspath(os.path.dirname(__file__))
+
+VERSION = '0.0.4'
+DESCRIPTION = 'A package for sending event notifications.'
+LONG_DESCRIPTION = 'A package for sending event notifications.'
+
+# Setting up
+setup(
+    name="cs-eventsender",
+    version=VERSION,
+    author="Richard",
+    author_email="<rich_swainson@hotmail.co.uk>",
+    description=DESCRIPTION,
+    long_description=LONG_DESCRIPTION,
+    packages=find_packages(),
+    install_requires=['requests','cs-telegram-bot-api'],
+    keywords=['binance', 'api', 'wrapper', 'c2c', 'sapi'],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Intended Audience :: Developers",
+        "Programming Language :: Python :: 3",
+        "Operating System :: Unix",
+        "Operating System :: MacOS :: MacOS X",
+        "Operating System :: Microsoft :: Windows",
+    ]
 )
```


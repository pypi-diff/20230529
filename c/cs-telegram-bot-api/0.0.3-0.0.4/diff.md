# Comparing `tmp/cs-telegram-bot-api-0.0.3.tar.gz` & `tmp/cs-telegram-bot-api-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-telegram-bot-api-0.0.3.tar", last modified: Mon May 29 07:03:29 2023, max compression
+gzip compressed data, was "cs-telegram-bot-api-0.0.4.tar", last modified: Mon May 29 19:06:17 2023, max compression
```

## Comparing `cs-telegram-bot-api-0.0.3.tar` & `cs-telegram-bot-api-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:03:29.271723 cs-telegram-bot-api-0.0.3/
--rw-rw-rw-   0        0        0      501 2023-05-29 07:03:29.271723 cs-telegram-bot-api-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-05-28 19:29:01.000000 cs-telegram-bot-api-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 07:03:29.230859 cs-telegram-bot-api-0.0.3/cs_telegram_bot/
--rw-rw-rw-   0        0        0       31 2023-05-29 06:59:14.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot/__init__.py
--rw-rw-rw-   0        0        0     2089 2023-05-28 19:25:37.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot/api.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:03:29.263704 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/
--rw-rw-rw-   0        0        0      501 2023-05-29 07:03:29.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      283 2023-05-29 07:03:29.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:03:29.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 07:03:29.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-29 07:03:29.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 07:03:29.271723 cs-telegram-bot-api-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1006 2023-05-29 07:03:06.000000 cs-telegram-bot-api-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:06:17.545194 cs-telegram-bot-api-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 19:06:17.541194 cs-telegram-bot-api-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-29 19:06:05.000000 cs-telegram-bot-api-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:06:17.541194 cs-telegram-bot-api-0.0.4/cs_telegram_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-29 19:06:05.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-29 19:06:05.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:06:17.541194 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 19:06:17.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-29 19:06:17.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:06:17.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 19:06:17.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 19:06:17.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:06:17.545194 cs-telegram-bot-api-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-29 19:06:05.000000 cs-telegram-bot-api-0.0.4/setup.py
```

### Comparing `cs-telegram-bot-api-0.0.3/README.md` & `cs-telegram-bot-api-0.0.4/README.md`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,30 +1,30 @@
-# Telegram Bot API Wrapper
-This is a Python wrapper for interacting with the Telegram Bot API. It provides a convenient way to send messages and receive updates from Telegram bots.
-
-## Installation
-To use this wrapper, you'll need Python 3.6 or above. You can install it using pip:
-
-`pip install telegram-bot-api-wrapper`
-## Usage
-1. Import the TelegramClient class:
-
-`from telegram_client import TelegramClient`
-2. Create an instance of the TelegramClient class by providing your bot token:
-```python
-bot_token = 'YOUR_BOT_TOKEN'
-client = TelegramClient(bot_token)
-```
-
-3. Use the available methods to interact with the Telegram Bot API. For example, to send a message:
-```python
-chat_id = 'TARGET_CHAT_ID'
-message = 'Hello, world!'
-client.send_message(chat_id, message)
-```
-4. To receive new messages, use the get_new_messages method:
-```python
-new_messages = client.get_new_messages()
-for message in new_messages:
-    print(message)
-```
+# Telegram Bot API Wrapper
+This is a Python wrapper for interacting with the Telegram Bot API. It provides a convenient way to send messages and receive updates from Telegram bots.
+
+## Installation
+To use this wrapper, you'll need Python 3.6 or above. You can install it using pip:
+
+`pip install telegram-bot-api-wrapper`
+## Usage
+1. Import the TelegramClient class:
+
+`from telegram_client import TelegramClient`
+2. Create an instance of the TelegramClient class by providing your bot token:
+```python
+bot_token = 'YOUR_BOT_TOKEN'
+client = TelegramClient(bot_token)
+```
+
+3. Use the available methods to interact with the Telegram Bot API. For example, to send a message:
+```python
+chat_id = 'TARGET_CHAT_ID'
+message = 'Hello, world!'
+client.send_message(chat_id, message)
+```
+4. To receive new messages, use the get_new_messages method:
+```python
+new_messages = client.get_new_messages()
+for message in new_messages:
+    print(message)
+```
 Refer to the docstrings in the code for more information about each method and its parameters.
```

### Comparing `cs-telegram-bot-api-0.0.3/cs_telegram_bot/api.py` & `cs-telegram-bot-api-0.0.4/cs_telegram_bot/api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,72 +1,73 @@
-"""
-A Python module for interacting with the Telegram Bot API.
-"""
-import requests
-import os
-
-
-class TelegramClient:
-    """
-    A client for the Telegram Bot API.
-    """
-
-    def __init__(self, bot_token=None):
-        """
-        Create a new TelegramClient.
-        """
-        self.bot_token = bot_token or os.getenv("TELEGRAM_TOKEN")
-        self.offset = 0
-
-    def get_new_messages(self):
-        """
-        Get new messages from the API.
-        """
-        try:
-            response = requests.get(
-                f"https://api.telegram.org/bot{self.bot_token}/getUpdates",
-                params={
-                    "offset": self.offset  # Only get updates with higher offsets
-                }
-            )
-            response.raise_for_status()
-        except requests.exceptions.RequestException as e:
-            raise SystemExit(e)
-
-        result = response.json()["result"]
-
-        # Get the messages from the updates
-        messages = []
-        for update in result:
-            if "message" in update:
-                messages.append(update["message"])
-
-        # Update the offset
-        if result:
-            self.offset = result[-1]["update_id"] + 1
-
-        return messages
-
-    def send_message(self, chat_id, message):
-        """
-        Send a message to a chat.
-        """
-        try:
-            # Make the API call
-            response = requests.post(
-                "https://api.telegram.org/bot{}/sendMessage".format(
-                    self.bot_token),
-                json={
-                    "chat_id": chat_id,
-                    "text": message,
-                    'parse_mode': 'Markdown'
-                }
-            )
-            response.raise_for_status()
-        except requests.exceptions.RequestException as e:
-            raise SystemExit(e)
-
-        # If the API call was successful, the response will contain
-        # the sent message in the "result" field
-        result = response.json()["result"]
-        print(message)
-        return result
+"""
+A Python module for interacting with the Telegram Bot API.
+"""
+import requests
+import os
+
+
+class TelegramClient:
+    """
+    A client for the Telegram Bot API.
+    """
+
+    def __init__(self, bot_token=None):
+        """
+        Create a new TelegramClient.
+        """
+        self.bot_token = bot_token or os.getenv("TELEGRAM_TOKEN")
+        self.offset = 0
+
+    def get_new_messages(self):
+        """
+        Get new messages from the API.
+        """
+        try:
+            response = requests.get(
+                f"https://api.telegram.org/bot{self.bot_token}/getUpdates",
+                params={
+                    "offset": self.offset  # Only get updates with higher offsets
+                }
+            )
+            response.raise_for_status()
+        except requests.exceptions.RequestException as e:
+            raise SystemExit(e)
+
+        result = response.json()["result"]
+
+        # Get the messages from the updates
+        messages = []
+        for update in result:
+            if "message" in update:
+                messages.append(update["message"])
+
+        # Update the offset
+        if result:
+            self.offset = result[-1]["update_id"] + 1
+
+        return messages
+
+    def send_message(self, chat_id, message):
+        """
+        Send a message to a chat.
+        """
+        try:
+            response = requests.post(
+                "https://api.telegram.org/bot{}/sendMessage".format(
+                    self.bot_token),
+                json={
+                    "chat_id": chat_id,
+                    "text": message
+                }
+            )
+            response.raise_for_status()
+        except requests.exceptions.RequestException as e:
+            raise SystemExit(e)
+
+        # If the API call was successful, the response will contain
+        # the sent message in the "result" field
+        result = response.json()["result"]
+        print(message)
+        return result
+
+
+if __name__ == "__main__":
```


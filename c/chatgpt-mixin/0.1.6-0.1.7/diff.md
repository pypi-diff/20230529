# Comparing `tmp/chatgpt-mixin-0.1.6.tar.gz` & `tmp/chatgpt-mixin-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatgpt-mixin-0.1.6.tar", last modified: Tue Mar 21 01:50:44 2023, max compression
+gzip compressed data, was "chatgpt-mixin-0.1.7.tar", last modified: Mon May 29 12:27:12 2023, max compression
```

## Comparing `chatgpt-mixin-0.1.6.tar` & `chatgpt-mixin-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 01:50:44.948634 chatgpt-mixin-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (116)     1073 2023-03-21 01:50:39.000000 chatgpt-mixin-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)     3863 2023-03-21 01:50:44.948634 chatgpt-mixin-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     3582 2023-03-21 01:50:39.000000 chatgpt-mixin-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 01:50:44.948634 chatgpt-mixin-0.1.6/chatgpt_mixin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3863 2023-03-21 01:50:44.000000 chatgpt-mixin-0.1.6/chatgpt_mixin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      365 2023-03-21 01:50:44.000000 chatgpt-mixin-0.1.6/chatgpt_mixin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-21 01:50:44.000000 chatgpt-mixin-0.1.6/chatgpt_mixin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       59 2023-03-21 01:50:44.000000 chatgpt-mixin-0.1.6/chatgpt_mixin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)       79 2023-03-21 01:50:44.000000 chatgpt-mixin-0.1.6/chatgpt_mixin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       14 2023-03-21 01:50:44.000000 chatgpt-mixin-0.1.6/chatgpt_mixin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      357 2023-03-21 01:50:44.948634 chatgpt-mixin-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      385 2023-03-21 01:50:39.000000 chatgpt-mixin-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-21 01:50:44.948634 chatgpt-mixin-0.1.6/src/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-21 01:50:39.000000 chatgpt-mixin-0.1.6/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)       70 2023-03-21 01:50:39.000000 chatgpt-mixin-0.1.6/src/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15266 2023-03-21 01:50:39.000000 chatgpt-mixin-0.1.6/src/chatgpt_browser.py
--rw-r--r--   0 runner    (1001) docker     (116)     9166 2023-03-21 01:50:39.000000 chatgpt-mixin-0.1.6/src/chatgpt_openai.py
--rw-r--r--   0 runner    (1001) docker     (116)    17234 2023-03-21 01:50:39.000000 chatgpt-mixin-0.1.6/src/mixinbot.py
--rw-r--r--   0 runner    (1001) docker     (116)     1983 2023-03-21 01:50:39.000000 chatgpt-mixin-0.1.6/src/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 12:27:12.928991 chatgpt-mixin-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-29 12:27:12.928991 chatgpt-mixin-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     3555 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 12:27:12.928991 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3836 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      365 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       79 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-29 12:27:12.000000 chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      357 2023-05-29 12:27:12.932991 chatgpt-mixin-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      385 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-29 12:27:12.928991 chatgpt-mixin-0.1.7/src/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       70 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15472 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/chatgpt_browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10453 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/chatgpt_openai.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17336 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/mixinbot.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1983 2023-05-29 12:27:06.000000 chatgpt-mixin-0.1.7/src/test.py
```

### Comparing `chatgpt-mixin-0.1.6/LICENSE` & `chatgpt-mixin-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chatgpt-mixin-0.1.6/PKG-INFO` & `chatgpt-mixin-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatgpt-mixin
-Version: 0.1.6
+Version: 0.1.7
 Summary: ChatGPT Bot For Mixin
 Home-page: https://github.com/learnforpractice/chatgpt-mixin
 Author: learnforpractice
 License: Apache 2.0
 Description-Content-Type: text/markdown
 Provides-Extra: browser
 License-File: LICENSE
@@ -20,28 +20,27 @@
 
 # Installation
 
 on unix like platform, install `chatgpt-mixin` with the following command:
 
 ```bash
 python3 -m pip install -U chatgpt-mixin
-playwright install firefox
 ```
 
 on the Windows platform, use the following command to install `chatgpt-mixin`:
 
 ```bash
 python -m pip install -U chatgpt-mixin
-playwright install firefox
 ```
 
 Install chatgpt-mixin with the support of accessing openai model in a browser:
 
 ```bash
 python3 -m pip install -U chatgpt-mixin[browser]
+playwright install firefox
 ```
 
 # configuration
 
 First, you need to create a mixin bot from [developers.mixin.one](https://developers.mixin.one/dashboard).
 And then under the `Secret` tab, click `Ed25519 session` to generate an App Session configuration.
```

### Comparing `chatgpt-mixin-0.1.6/README.md` & `chatgpt-mixin-0.1.7/chatgpt_mixin.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: chatgpt-mixin
+Version: 0.1.7
+Summary: ChatGPT Bot For Mixin
+Home-page: https://github.com/learnforpractice/chatgpt-mixin
+Author: learnforpractice
+License: Apache 2.0
+Description-Content-Type: text/markdown
+Provides-Extra: browser
+License-File: LICENSE
+
 [![PyPi](https://img.shields.io/pypi/v/chatgpt-mixin.svg)](https://pypi.org/project/chatgpt-mixin)
 [![PyPi](https://img.shields.io/pypi/dm/chatgpt-mixin.svg)](https://pypi.org/project/chatgpt-mixin)
 
 # chatgpt-mixin
 
 ![Demo](./images/demo.png)
 
@@ -9,28 +20,27 @@
 
 # Installation
 
 on unix like platform, install `chatgpt-mixin` with the following command:
 
 ```bash
 python3 -m pip install -U chatgpt-mixin
-playwright install firefox
 ```
 
 on the Windows platform, use the following command to install `chatgpt-mixin`:
 
 ```bash
 python -m pip install -U chatgpt-mixin
-playwright install firefox
 ```
 
 Install chatgpt-mixin with the support of accessing openai model in a browser:
 
 ```bash
 python3 -m pip install -U chatgpt-mixin[browser]
+playwright install firefox
 ```
 
 # configuration
 
 First, you need to create a mixin bot from [developers.mixin.one](https://developers.mixin.one/dashboard).
 And then under the `Secret` tab, click `Ed25519 session` to generate an App Session configuration.
```

### Comparing `chatgpt-mixin-0.1.6/chatgpt_mixin.egg-info/PKG-INFO` & `chatgpt-mixin-0.1.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: chatgpt-mixin
-Version: 0.1.6
-Summary: ChatGPT Bot For Mixin
-Home-page: https://github.com/learnforpractice/chatgpt-mixin
-Author: learnforpractice
-License: Apache 2.0
-Description-Content-Type: text/markdown
-Provides-Extra: browser
-License-File: LICENSE
-
 [![PyPi](https://img.shields.io/pypi/v/chatgpt-mixin.svg)](https://pypi.org/project/chatgpt-mixin)
 [![PyPi](https://img.shields.io/pypi/dm/chatgpt-mixin.svg)](https://pypi.org/project/chatgpt-mixin)
 
 # chatgpt-mixin
 
 ![Demo](./images/demo.png)
 
@@ -20,28 +9,27 @@
 
 # Installation
 
 on unix like platform, install `chatgpt-mixin` with the following command:
 
 ```bash
 python3 -m pip install -U chatgpt-mixin
-playwright install firefox
 ```
 
 on the Windows platform, use the following command to install `chatgpt-mixin`:
 
 ```bash
 python -m pip install -U chatgpt-mixin
-playwright install firefox
 ```
 
 Install chatgpt-mixin with the support of accessing openai model in a browser:
 
 ```bash
 python3 -m pip install -U chatgpt-mixin[browser]
+playwright install firefox
 ```
 
 # configuration
 
 First, you need to create a mixin bot from [developers.mixin.one](https://developers.mixin.one/dashboard).
 And then under the `Secret` tab, click `Ed25519 session` to generate an App Session configuration.
```

### Comparing `chatgpt-mixin-0.1.6/src/chatgpt_browser.py` & `chatgpt-mixin-0.1.7/src/chatgpt_browser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # -*- coding: utf-8 -*-
 
+import asyncio
+import json
+import logging
 import os
+import random
 import re
-import json
+import shelve
 import time
 import uuid
-import random
-import asyncio
-import logging
-import shelve
+from typing import Any, Dict, Optional, Tuple, Union
 
-from typing import Optional, Dict, Tuple, Any, Union
+from cf_clearance import StealthConfig
 from playwright.async_api import BrowserContext as AsyncContext
 from playwright.async_api import Page as AsyncPage
-from cf_clearance import StealthConfig
-
-
 from pymixin import log
+
 logger = log.get_logger(__name__)
 logger.addHandler(log.handler)
 
 async def async_stealth(
     page_or_context: Union[AsyncContext, AsyncPage],
     config: StealthConfig = None,
     pure: bool = True,
@@ -95,15 +94,15 @@
         self.expiration = time.time() + 15*60.0
 
     def is_expired(self):
         return self.expiration < time.time()
 
 class ChatGPTBot:
 
-    def __init__(self, PLAY: Any, user: str, password: str):
+    def __init__(self, PLAY: Any, user: str, password: str, model='gpt-4'):
         self.page: Optional[Any] = None
         self.access_token: Optional[str] = None
 
         self.PLAY = PLAY
         self.user = user
         self.password = password
         self._standby: bool = False
@@ -116,14 +115,15 @@
 
         if not os.path.exists('.db'):
             os.mkdir('.db')
         self.users = shelve.open(f".db/{user}-1")
         self.expired_user = shelve.open(f".db/{user}-2")
 
         self.alive_counter = 0
+        self.model = model #'text-davinci-002-render',
 
     @property
     def standby(self):
         return self._standby
 
     @standby.setter
     def standby(self, value):
@@ -314,14 +314,19 @@
     def reset_conversation_id(self, user_id):
         assert user_id in self.users
         user = self.users[user_id]
         user.conversation_id = None
         self.users[user_id] = user
 
     async def send_message(self, user_id, message):
+        if message == '/reset':
+            self.reset_conversation_id(user_id)
+            yield '[BEGIN]'
+            yield 'Done'
+            return
         try:
             async with self.lock:
                 user = self.get_user(user_id)
                 self.busy = True
                 async for msg in self._send_message(user, message):
                     yield msg
         finally:
@@ -344,15 +349,15 @@
                     "role": 'user',
                     "content": {
                         "content_type": 'text',
                         "parts": [message]
                     }
                 }
             ],
-            "model": 'text-davinci-002-render',
+            "model": self.model,
             "parent_message_id": user.parent_message_id
         }
 
         if user.conversation_id:
             body['conversation_id'] = user.conversation_id
 
         url = "https://chat.openai.com/backend-api/conversation"
```

### Comparing `chatgpt-mixin-0.1.6/src/mixinbot.py` & `chatgpt-mixin-0.1.7/src/mixinbot.py`

 * *Files 2% similar despite different names*

```diff
@@ -275,15 +275,15 @@
                     continue
             for question in handled_question:
                 del self.saved_questions[question]
 
     def save_question(self, conversation_id, user_id, data):
         self.saved_questions[user_id] = SavedQuestion(conversation_id, user_id, data)
 
-    async def handle_message(self, conversation_id, user_id, message):
+    async def handle_user_message(self, conversation_id, user_id, message):
         try:
             await self.send_message_to_chat_gpt(conversation_id, user_id, message)
         except Exception as e:
             logger.exception(e)
             if self.developer_user_id:
                 await self.sendUserText(self.developer_conversation_id, self.developer_user_id, f"exception occur at:{time.time()}: {traceback.format_exc()}")
 
@@ -360,29 +360,32 @@
             reply = sayhi[data]
             await self.sendUserText(msg.conversation_id, msg.user_id, reply)
             return
         except KeyError:
             pass
 
         if utils.unique_conversation_id(msg.user_id, self.client_id) == msg.conversation_id:
-            asyncio.create_task(self.handle_message(msg.conversation_id, msg.user_id, data))
+            asyncio.create_task(self.handle_user_message(msg.conversation_id, msg.user_id, data))
         else:
             asyncio.create_task(self.handle_group_message(msg.conversation_id, msg.user_id, data))
 
     async def run(self):
         try:
             while not self.paused:
                 try:
                     await super().run()
                 except websockets.exceptions.ConnectionClosedError as e:
                     logger.exception(e)
+                    await asyncio.sleep(3.0)
                     self.ws = None
                 #asyncio.exceptions.TimeoutError
                 except Exception as e:
+#
                     logger.exception(e)
+                    await asyncio.sleep(3.0)
                     self.ws = None
         except asyncio.CancelledError:
             if self.ws:
                 await self.ws.close()
             if self.web_client:
                 await self.web_client.aclose()
             logger.info("mixin websocket was cancelled!")
```

### Comparing `chatgpt-mixin-0.1.6/src/test.py` & `chatgpt-mixin-0.1.7/src/test.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import shutil
 from dataclasses import dataclass
 from typing import List
 
+import openai
 import pytest
 
-import openai
 from chatgpt_openai import ChatGPTBot
 
 file_dir = os.path.dirname(os.path.realpath(__file__))
 
 def test_save_message_id():
     bot = ChatGPTBot('test')
     bot.save_last_message_id('conversation_id', 'message_id')
```


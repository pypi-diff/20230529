# Comparing `tmp/omniunibot-0.0.5.tar.gz` & `tmp/omniunibot-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omniunibot-0.0.5.tar", last modified: Sun Apr 16 09:13:31 2023, max compression
+gzip compressed data, was "omniunibot-0.0.6.tar", last modified: Mon May 29 12:13:32 2023, max compression
```

## Comparing `omniunibot-0.0.5.tar` & `omniunibot-0.0.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:31.303208 omniunibot-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-16 09:13:19.000000 omniunibot-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-16 09:13:31.303208 omniunibot-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-04-16 09:13:19.000000 omniunibot-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:31.303208 omniunibot-0.0.5/omniunibot/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4584 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/server.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:31.303208 omniunibot-0.0.5/omniunibot/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/dingtalk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/feishu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/slack.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-16 09:13:19.000000 omniunibot-0.0.5/omniunibot/wrapper/wecom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-16 09:13:31.303208 omniunibot-0.0.5/omniunibot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-16 09:13:31.000000 omniunibot-0.0.5/omniunibot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-16 09:13:31.303208 omniunibot-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-16 09:13:19.000000 omniunibot-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:32.832872 omniunibot-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-29 12:13:15.000000 omniunibot-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-29 12:13:32.832872 omniunibot-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2520 2023-05-29 12:13:15.000000 omniunibot-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:32.832872 omniunibot-0.0.6/omniunibot/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1566 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:32.832872 omniunibot-0.0.6/omniunibot/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/dingtalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/feishu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/slack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2844 2023-05-29 12:13:15.000000 omniunibot-0.0.6/omniunibot/wrapper/wecom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:13:32.832872 omniunibot-0.0.6/omniunibot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 12:13:32.000000 omniunibot-0.0.6/omniunibot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:13:32.832872 omniunibot-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-29 12:13:15.000000 omniunibot-0.0.6/setup.py
```

### Comparing `omniunibot-0.0.5/LICENSE` & `omniunibot-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.5/PKG-INFO` & `omniunibot-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniunibot
-Version: 0.0.5
+Version: 0.0.6
 Summary: A universal multiplatform message bot
 Home-page: https://github.com/yttty/omniunibot
 Author: yttty
 Author-email: yttty@noreply.com
 License: MIT
 Keywords: bots
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `omniunibot-0.0.5/README.md` & `omniunibot-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.5/omniunibot/__main__.py` & `omniunibot-0.0.6/omniunibot/__main__.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.5/omniunibot/client.py` & `omniunibot-0.0.6/omniunibot/client.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.5/omniunibot/server.py` & `omniunibot-0.0.6/omniunibot/server.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import zmq
 import json
 import asyncio
 from loguru import logger
 from zmq.asyncio import Context
-
+from traceback import format_exc
 
 from concurrent.futures import ThreadPoolExecutor
 
 from .wrapper.dingtalk import DingTalkBot
 from .wrapper.wecom import WeComBot
 from .wrapper.feishu import FeishuBot
 from .wrapper.slack import SlackBot
@@ -91,20 +91,22 @@
         executors = []
         with ThreadPoolExecutor(max_workers=len(self.bots[channel])) as executor:
             for bot in self.bots[channel]:
                 executors.append(executor.submit(bot.sendQuickMessage, msg))
 
     async def _startServer(self):
         self._socket.bind(self._addr)
-        logger.debug(f"Server bind to {self._addr}")
+        logger.info(f"Server bind to {self._addr}")
         while True:
             try:
                 mtPart = await self._socket.recv_multipart()
                 info = json.loads(mtPart[1].decode('utf-8'))
 
+                logger.debug(f"Server receive: {info}")
+
                 if info['msgType'] not in ['text']:
                     raise NotImplementedError(
                         f"Unsupported message type {info['msgType']}")
 
                 if info['channel'] not in self.bots.keys():
                     raise ValueError(f"No such channel {self.bots}")
 
@@ -116,13 +118,13 @@
                 self._bulkSend(channel=info['channel'],
                                msg=msgStr,
                                msgType=info['msgType'])
             except KeyboardInterrupt:
                 logger.info('Bye')
                 exit(0)
             except Exception as e:
-                logger.error(str(e))
+                logger.error(format_exc())
                 pass
 
     def run(self):
         asyncio.ensure_future(self._startServer(), loop=self.loop)
         self.loop.run_forever()
```

### Comparing `omniunibot-0.0.5/omniunibot/wrapper/base.py` & `omniunibot-0.0.6/omniunibot/wrapper/base.py`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.5/omniunibot/wrapper/dingtalk.py` & `omniunibot-0.0.6/omniunibot/wrapper/dingtalk.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     def _onErrorResponse(self, response) -> int:
         logger.error(
             f"Code = {response['errcode']}. Message = {response['errmsg']}."
         )
         return response['errcode']
 
     def _onSuccessResponse(self, response=None) -> int:
-        logger.info("Successully sent message to DingTalk.")
+        logger.debug("Successully sent message to DingTalk.")
         return 0
 
     def generatePayload(self,
                         text: str,
                         atMobiles: Optional[List[str]] = None,
                         atAll: bool = False):
         payload = {
@@ -61,28 +61,28 @@
             }
         }
         if atMobiles is not None:
             payload['at']['atMobiles'] = atMobiles
         return payload
 
     def sendMessage(self, payload: dict):
-        logger.info(f"Get message: {payload}")
+        logger.debug(f"Get message: {payload}")
         try:
             r = requests.post(self._getSignedUrlForDingDing(),
                               json=payload)
             response = r.json()
             if response['errcode'] == 0:
                 self._onSuccessResponse()
             else:
                 self._onErrorResponse(response)
         except Exception as e:
             logger.error(f"Caught Exception {str(e)}")
 
     def sendQuickMessage(self, msg: str):
-        logger.info(f"Get text message: {msg}")
+        logger.debug(f"Get text message: {msg}")
         try:
             r = requests.post(self._getSignedUrlForDingDing(),
                               json=self.generatePayload(msg))
             response = r.json()
             if response['errcode'] == 0:
                 self._onSuccessResponse()
             else:
```

### Comparing `omniunibot-0.0.5/omniunibot/wrapper/feishu.py` & `omniunibot-0.0.6/omniunibot/wrapper/feishu.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     def _onErrorResponse(self, response) -> int:
         logger.error(
             f"Code = {response['code']}. Message = {response['msg']}."
         )
         return response['code']
 
     def _onSuccessResponse(self, response=None) -> int:
-        logger.info("Successully sent message to Feishu.")
+        logger.debug("Successully sent message to Feishu.")
         return 0
 
     def generatePayload(self,
                         text: str,
                         title: Optional[str] = None):
         """Generate payload to send, using message type `post`, see the document for details
 
@@ -83,15 +83,15 @@
                         "zh_cn": post_zh_cn
                 }
             }
         }
         return payload
 
     def sendQuickMessage(self, msg: str):
-        logger.info(f"Get text message: {msg}")
+        logger.debug(f"Get text message: {msg}")
         try:
             r = requests.post(self.webhook,
                               json=self.generatePayload(msg))
             response = r.json()
             if "code" in response.keys() and response['code'] != 0:
                 self._onErrorResponse(response)
             else:
```

### Comparing `omniunibot-0.0.5/omniunibot/wrapper/slack.py` & `omniunibot-0.0.6/omniunibot/wrapper/slack.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         """
         logger.error(
             f"Code = {response.status_code}. Message = {response.body}."
         )
         return response.status_code
 
     def _onSuccessResponse(self, response=None) -> int:
-        logger.info("Successully sent message to Slack.")
+        logger.debug("Successully sent message to Slack.")
         return 0
 
     def generatePayload(self, text: str) -> Dict:
         payload = {
             'channel': "what-channel",
             'blocks': [
                 # {
@@ -71,15 +71,15 @@
                     ]
                 }
             ]
         }
         return payload
 
     def sendQuickMessage(self, msg: str):
-        logger.info(f"Get text message: {msg}")
+        logger.debug(f"Get text message: {msg}")
         try:
             response = self.slack_client.send_dict(self.generatePayload(msg))
             if response.status_code != 200:
                 self._onErrorResponse(response)
             else:
                 self._onSuccessResponse()
         except Exception as e:
```

### Comparing `omniunibot-0.0.5/omniunibot/wrapper/wecom.py` & `omniunibot-0.0.6/omniunibot/wrapper/wecom.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     def _onErrorResponse(self, response) -> int:
         logger.error(
             f"Code = {response['errcode']}. Message = {response['errmsg']}."
         )
         return response['errcode']
 
     def _onSuccessResponse(self, response=None) -> int:
-        logger.info("Successully sent message to WeCom.")
+        logger.debug("Successully sent message to WeCom.")
         return 0
 
     def generatePayload(self, msgtype: str, **kwargs):
         assert msgtype in ["markdown", "text", "image"], "Unsupported msgtype"
         payload = {"msgtype": msgtype, msgtype: {}}
 
         if msgtype == "text" or msgtype == "markdown":
@@ -54,27 +54,27 @@
                 payload[msgtype]["md5"] = kwargs["md5"]
             except KeyError:
                 raise KeyError("Missing image args")
 
         return payload
 
     def sendMessage(self, payload: dict):
-        logger.info(f"Get message: {payload}")
+        logger.debug(f"Get message: {payload}")
         try:
             r = requests.post(self.webhook, json=payload)
             response = r.json()
             if response['errcode'] == 0:
                 self._onSuccessResponse()
             else:
                 self._onErrorResponse(response)
         except Exception as e:
             logger.error(f"Caught Exception {str(e)}")
 
     def sendQuickMessage(self, text: str):
-        logger.info(f"Get text Message: {text}")
+        logger.debug(f"Get text Message: {text}")
         try:
             r = requests.post(self.webhook,
                               json=self.generatePayload(msgtype="text",
                                                         content=text))
             response = r.json()
             if response['errcode'] == 0:
                 self._onSuccessResponse()
```

### Comparing `omniunibot-0.0.5/omniunibot.egg-info/PKG-INFO` & `omniunibot-0.0.6/omniunibot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omniunibot
-Version: 0.0.5
+Version: 0.0.6
 Summary: A universal multiplatform message bot
 Home-page: https://github.com/yttty/omniunibot
 Author: yttty
 Author-email: yttty@noreply.com
 License: MIT
 Keywords: bots
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `omniunibot-0.0.5/omniunibot.egg-info/SOURCES.txt` & `omniunibot-0.0.6/omniunibot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omniunibot-0.0.5/setup.py` & `omniunibot-0.0.6/setup.py`

 * *Files identical despite different names*


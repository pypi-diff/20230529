# Comparing `tmp/whochat-1.3.3.tar.gz` & `tmp/whochat-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whochat-1.3.3.tar", last modified: Tue May 23 03:09:23 2023, max compression
+gzip compressed data, was "whochat-1.3.4.tar", last modified: Mon May 29 15:57:29 2023, max compression
```

## Comparing `whochat-1.3.3.tar` & `whochat-1.3.4.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.927396 whochat-1.3.3/
--rw-r--r--   0 luming     (501) staff       (20)     1514 2023-01-29 06:35:29.000000 whochat-1.3.3/LICENSE
--rw-r--r--   0 luming     (501) staff       (20)       55 2023-01-29 06:35:29.000000 whochat-1.3.3/MANIFEST.in
--rw-r--r--   0 luming     (501) staff       (20)     7460 2023-05-23 03:09:23.927528 whochat-1.3.3/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)     6807 2023-05-23 03:09:03.000000 whochat-1.3.3/README.md
--rw-r--r--   0 luming     (501) staff       (20)     1292 2023-05-23 03:09:23.928126 whochat-1.3.3/setup.cfg
--rw-r--r--   0 luming     (501) staff       (20)       38 2023-03-09 09:22:00.000000 whochat-1.3.3/setup.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.921625 whochat-1.3.3/whochat/
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.924437 whochat-1.3.3/whochat/ComWeChatRobot/
--rw-r--r--   0 luming     (501) staff       (20)   165376 2023-02-13 09:38:48.000000 whochat-1.3.3/whochat/ComWeChatRobot/CWeChatRobot.exe
--rw-r--r--   0 luming     (501) staff       (20)   293888 2023-02-13 09:38:48.000000 whochat-1.3.3/whochat/ComWeChatRobot/DWeChatRobot.dll
--rw-r--r--   0 luming     (501) staff       (20)      472 2023-02-13 09:38:48.000000 whochat-1.3.3/whochat/ComWeChatRobot/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)       65 2023-05-23 03:06:59.000000 whochat-1.3.3/whochat/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      107 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/__main__.py
--rw-r--r--   0 luming     (501) staff       (20)      608 2023-02-13 09:38:48.000000 whochat-1.3.3/whochat/_comtypes.py
--rw-r--r--   0 luming     (501) staff       (20)     6413 2023-02-13 09:38:48.000000 whochat-1.3.3/whochat/abc.py
--rw-r--r--   0 luming     (501) staff       (20)    18091 2023-05-23 03:05:16.000000 whochat-1.3.3/whochat/bot.py
--rw-r--r--   0 luming     (501) staff       (20)     4952 2023-05-11 01:43:21.000000 whochat-1.3.3/whochat/cli.py
--rw-r--r--   0 luming     (501) staff       (20)      762 2023-05-11 01:43:21.000000 whochat-1.3.3/whochat/logger.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.925272 whochat-1.3.3/whochat/messages/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/messages/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      447 2023-03-09 10:27:55.000000 whochat-1.3.3/whochat/messages/constants.py
--rw-r--r--   0 luming     (501) staff       (20)     6875 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/messages/tcp.py
--rw-r--r--   0 luming     (501) staff       (20)     7055 2023-05-23 03:05:36.000000 whochat-1.3.3/whochat/messages/websocket.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.926343 whochat-1.3.3/whochat/rpc/
--rw-r--r--   0 luming     (501) staff       (20)       22 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/rpc/__init__.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.926706 whochat-1.3.3/whochat/rpc/clients/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-03-09 10:27:55.000000 whochat-1.3.3/whochat/rpc/clients/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)     4314 2023-05-11 01:43:21.000000 whochat-1.3.3/whochat/rpc/clients/websocket.py
--rw-r--r--   0 luming     (501) staff       (20)     1823 2023-03-09 10:27:55.000000 whochat-1.3.3/whochat/rpc/docs.py
--rw-r--r--   0 luming     (501) staff       (20)     9767 2023-03-09 10:27:55.000000 whochat-1.3.3/whochat/rpc/handlers.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.927239 whochat-1.3.3/whochat/rpc/servers/
--rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/rpc/servers/__init__.py
--rw-r--r--   0 luming     (501) staff       (20)      930 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/rpc/servers/http.py
--rw-r--r--   0 luming     (501) staff       (20)     1138 2023-05-11 01:43:21.000000 whochat-1.3.3/whochat/rpc/servers/websocket.py
--rw-r--r--   0 luming     (501) staff       (20)      315 2023-05-11 01:43:21.000000 whochat-1.3.3/whochat/settings.py
--rw-r--r--   0 luming     (501) staff       (20)     1108 2023-01-29 06:35:29.000000 whochat-1.3.3/whochat/signals.py
--rw-r--r--   0 luming     (501) staff       (20)     3091 2023-03-09 10:27:55.000000 whochat-1.3.3/whochat/utils.py
-drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-23 03:09:23.922787 whochat-1.3.3/whochat.egg-info/
--rw-r--r--   0 luming     (501) staff       (20)     7460 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/PKG-INFO
--rw-r--r--   0 luming     (501) staff       (20)      870 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/SOURCES.txt
--rw-r--r--   0 luming     (501) staff       (20)        1 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/dependency_links.txt
--rw-r--r--   0 luming     (501) staff       (20)       50 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/entry_points.txt
--rw-r--r--   0 luming     (501) staff       (20)      115 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/requires.txt
--rw-r--r--   0 luming     (501) staff       (20)        8 2023-05-23 03:09:23.000000 whochat-1.3.3/whochat.egg-info/top_level.txt
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.773577 whochat-1.3.4/
+-rw-r--r--   0 luming     (501) staff       (20)     1514 2023-01-29 06:35:29.000000 whochat-1.3.4/LICENSE
+-rw-r--r--   0 luming     (501) staff       (20)       55 2023-01-29 06:35:29.000000 whochat-1.3.4/MANIFEST.in
+-rw-r--r--   0 luming     (501) staff       (20)     7644 2023-05-29 15:57:29.773753 whochat-1.3.4/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)     6991 2023-05-29 15:57:17.000000 whochat-1.3.4/README.md
+-rw-r--r--   0 luming     (501) staff       (20)     1292 2023-05-29 15:57:29.774164 whochat-1.3.4/setup.cfg
+-rw-r--r--   0 luming     (501) staff       (20)       38 2023-03-09 09:22:00.000000 whochat-1.3.4/setup.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.766218 whochat-1.3.4/whochat/
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.768285 whochat-1.3.4/whochat/ComWeChatRobot/
+-rw-r--r--   0 luming     (501) staff       (20)   165376 2023-02-13 09:38:48.000000 whochat-1.3.4/whochat/ComWeChatRobot/CWeChatRobot.exe
+-rw-r--r--   0 luming     (501) staff       (20)   293888 2023-02-13 09:38:48.000000 whochat-1.3.4/whochat/ComWeChatRobot/DWeChatRobot.dll
+-rw-r--r--   0 luming     (501) staff       (20)      472 2023-02-13 09:38:48.000000 whochat-1.3.4/whochat/ComWeChatRobot/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)       65 2023-05-29 15:50:44.000000 whochat-1.3.4/whochat/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      107 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/__main__.py
+-rw-r--r--   0 luming     (501) staff       (20)      608 2023-02-13 09:38:48.000000 whochat-1.3.4/whochat/_comtypes.py
+-rw-r--r--   0 luming     (501) staff       (20)     6413 2023-02-13 09:38:48.000000 whochat-1.3.4/whochat/abc.py
+-rw-r--r--   0 luming     (501) staff       (20)    22043 2023-05-26 16:24:36.000000 whochat-1.3.4/whochat/bot.py
+-rw-r--r--   0 luming     (501) staff       (20)     4952 2023-05-11 01:43:21.000000 whochat-1.3.4/whochat/cli.py
+-rw-r--r--   0 luming     (501) staff       (20)      762 2023-05-11 01:43:21.000000 whochat-1.3.4/whochat/logger.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.771566 whochat-1.3.4/whochat/messages/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/messages/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      447 2023-03-09 10:27:55.000000 whochat-1.3.4/whochat/messages/constants.py
+-rw-r--r--   0 luming     (501) staff       (20)     6875 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/messages/tcp.py
+-rw-r--r--   0 luming     (501) staff       (20)     7210 2023-05-26 16:02:21.000000 whochat-1.3.4/whochat/messages/websocket.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.772353 whochat-1.3.4/whochat/rpc/
+-rw-r--r--   0 luming     (501) staff       (20)       22 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/rpc/__init__.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.772696 whochat-1.3.4/whochat/rpc/clients/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-03-09 10:27:55.000000 whochat-1.3.4/whochat/rpc/clients/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)     4824 2023-05-29 14:29:26.000000 whochat-1.3.4/whochat/rpc/clients/websocket.py
+-rw-r--r--   0 luming     (501) staff       (20)     1823 2023-03-09 10:27:55.000000 whochat-1.3.4/whochat/rpc/docs.py
+-rw-r--r--   0 luming     (501) staff       (20)    10159 2023-05-26 15:23:50.000000 whochat-1.3.4/whochat/rpc/handlers.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.773251 whochat-1.3.4/whochat/rpc/servers/
+-rw-r--r--   0 luming     (501) staff       (20)        0 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/rpc/servers/__init__.py
+-rw-r--r--   0 luming     (501) staff       (20)      930 2023-01-29 06:35:29.000000 whochat-1.3.4/whochat/rpc/servers/http.py
+-rw-r--r--   0 luming     (501) staff       (20)     1138 2023-05-26 10:13:13.000000 whochat-1.3.4/whochat/rpc/servers/websocket.py
+-rw-r--r--   0 luming     (501) staff       (20)      315 2023-05-11 01:43:21.000000 whochat-1.3.4/whochat/settings.py
+-rw-r--r--   0 luming     (501) staff       (20)     1108 2023-05-29 10:26:50.000000 whochat-1.3.4/whochat/signals.py
+-rw-r--r--   0 luming     (501) staff       (20)     3091 2023-03-09 10:27:55.000000 whochat-1.3.4/whochat/utils.py
+drwxr-xr-x   0 luming     (501) staff       (20)        0 2023-05-29 15:57:29.767129 whochat-1.3.4/whochat.egg-info/
+-rw-r--r--   0 luming     (501) staff       (20)     7644 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/PKG-INFO
+-rw-r--r--   0 luming     (501) staff       (20)      870 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/SOURCES.txt
+-rw-r--r--   0 luming     (501) staff       (20)        1 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/dependency_links.txt
+-rw-r--r--   0 luming     (501) staff       (20)       50 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/entry_points.txt
+-rw-r--r--   0 luming     (501) staff       (20)      115 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/requires.txt
+-rw-r--r--   0 luming     (501) staff       (20)        8 2023-05-29 15:57:29.000000 whochat-1.3.4/whochat.egg-info/top_level.txt
```

### Comparing `whochat-1.3.3/LICENSE` & `whochat-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/PKG-INFO` & `whochat-1.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whochat
-Version: 1.3.3
+Version: 1.3.4
 Summary: 一个命令就可启用的微信机器人
 Home-page: https://github.com/amchii/whochat
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/whochat
 Classifier: Intended Audience :: Developers
@@ -189,14 +189,19 @@
     "id": 4
 }
 ```
 
 [CHANGELOG](https://github.com/amchii/whochat/blob/main/CHANGELOG.md)
 
 [Tags](https://github.com/amchii/whochat/tags)
+## v1.3.4
+* 自动设置微信版本号避免更新
+* 增加环境变量`WHOCHAT_WECHAT_VERSION`自定义微信版本号
+* 尝试使`BotWebsocketRPCClient.rpc_call`更正确地运行
+
 ## v1.3.3
 * 增加获取微信最新版本号的方法
 * 修复Mac用户发送@消息无法正确解析的问题
 
 ## v1.3.2
 * 修改日志级别，增加日志文件记录
```

### Comparing `whochat-1.3.3/README.md` & `whochat-1.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -170,14 +170,19 @@
     "id": 4
 }
 ```
 
 [CHANGELOG](https://github.com/amchii/whochat/blob/main/CHANGELOG.md)
 
 [Tags](https://github.com/amchii/whochat/tags)
+## v1.3.4
+* 自动设置微信版本号避免更新
+* 增加环境变量`WHOCHAT_WECHAT_VERSION`自定义微信版本号
+* 尝试使`BotWebsocketRPCClient.rpc_call`更正确地运行
+
 ## v1.3.3
 * 增加获取微信最新版本号的方法
 * 修复Mac用户发送@消息无法正确解析的问题
 
 ## v1.3.2
 * 修改日志级别，增加日志文件记录
```

### Comparing `whochat-1.3.3/setup.cfg` & `whochat-1.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/ComWeChatRobot/CWeChatRobot.exe` & `whochat-1.3.4/whochat/ComWeChatRobot/CWeChatRobot.exe`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/ComWeChatRobot/DWeChatRobot.dll` & `whochat-1.3.4/whochat/ComWeChatRobot/DWeChatRobot.dll`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/_comtypes.py` & `whochat-1.3.4/whochat/_comtypes.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/abc.py` & `whochat-1.3.4/whochat/abc.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/bot.py` & `whochat-1.3.4/whochat/bot.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pathlib
 import re
 import shutil
 import tempfile
 import threading
 import time
 from datetime import datetime
-from typing import Dict, List, Union
+from typing import Dict, List, Union, overload
 from urllib import request
 
 import psutil
 
 from ._comtypes import client as com_client
 from .abc import CWechatRobotABC, RobotEventABC, RobotEventSinkABC
 from .logger import logger
@@ -43,25 +43,32 @@
         except Exception as e:
             logger.exception(e)
 
     return wrapper
 
 
 class WechatBot:
-    def __init__(self, wx_pid, robot_object_id: str, robot_event_id: str = None):
+    def __init__(
+        self,
+        wx_pid,
+        robot_object_id: str,
+        robot_event_id: str = None,
+        wechat_version=None,
+    ):
         self.wx_pid = int(wx_pid)
         self._robot_object_id = robot_object_id
         self._robot_event_id = robot_event_id
         self.started = False
         self.user_info = {}
         self.event_connection = None
 
         self._base_directory = None
         self.image_hook_path = None
         self.voice_hook_path = None
+        self.wechat_version = wechat_version
 
     @property
     def robot(self):
         return get_robot_object(self._robot_object_id)
 
     @property
     def robot_event(self):
@@ -78,14 +85,17 @@
         if self.started:
             return True
         result = self.robot.CStartRobotService(
             self.wx_pid,
         )
         if result == 0:
             self.started = True
+            if self.wechat_version:
+                self.change_wechat_ver(self.wechat_version)
+                logger.info(f"更改微信版本号为: {self.wechat_version}")
         return not result
 
     def stop_robot_service(self):
         if not self.started:
             return True
         result = self.robot.CStopRobotService(
             self.wx_pid,
@@ -102,14 +112,18 @@
 
     def get_base_directory(self):
         p = psutil.Process(pid=self.wx_pid)
         base_directory = guess_wechat_base_directory([f.path for f in p.open_files()])
         self._base_directory = base_directory
         return base_directory
 
+    @overload
+    def send_image(self, wx_id, img_path) -> int:
+        ...
+
     @auto_start
     def send_image(self, wx_id, img_path):
         path = pathlib.Path(img_path)
         if not path.is_absolute():
             base_dir = self.image_hook_path or self.base_directory
             path = pathlib.Path(base_dir).joinpath(path)
 
@@ -118,112 +132,176 @@
             with tempfile.TemporaryDirectory() as td:
                 temp_path = os.path.join(td, os.urandom(5).hex() + path.suffix)
                 shutil.copy(path, temp_path)
                 return self.robot.CSendImage(self.wx_pid, wx_id, temp_path)
 
         return self.robot.CSendImage(self.wx_pid, wx_id, str(path))
 
+    @overload
+    def send_text(self, wx_id, text) -> int:
+        ...
+
     @auto_start
     def send_text(self, wx_id, text):
         return self.robot.CSendText(self.wx_pid, wx_id, text)
 
+    @overload
+    def send_file(self, wx_id, filepath) -> int:
+        ...
+
     @auto_start
     def send_file(self, wx_id, filepath):
         path = pathlib.Path(filepath)
         if not path.is_absolute():
             path = pathlib.Path(self.base_directory).joinpath(path)
 
         return self.robot.CSendFile(self.wx_pid, wx_id, str(path))
 
+    @overload
+    def send_article(
+        self, wxid: str, title: str, abstract: str, url: str, imgpath: str
+    ):
+        ...
+
     @auto_start
     def send_article(
         self, wxid: str, title: str, abstract: str, url: str, imgpath: str
     ):
         return self.robot.CSendArticle(self.wx_pid, wxid, title, abstract, url, imgpath)
 
+    @overload
+    def send_card(self, wxid: str, shared_wxid: str, nickname: str) -> int:
+        ...
+
     @auto_start
     def send_card(self, wxid: str, shared_wxid: str, nickname: str):
         return self.robot.CSendCard(self.wx_pid, wxid, shared_wxid, nickname)
 
+    @overload
+    def send_at_text(
+        self,
+        chatroom_id: str,
+        at_wxids: Union[str, List[str]],
+        text: str,
+        auto_nickname: bool = True,
+    ) -> int:
+        ...
+
     @auto_start
     def send_at_text(
         self,
         chatroom_id: str,
         at_wxids: Union[str, List[str]],
         text: str,
         auto_nickname: bool = True,
     ):
         return self.robot.CSendAtText(
             self.wx_pid, chatroom_id, at_wxids, text, auto_nickname
         )
 
+    @overload
+    def get_friend_list(self) -> List[Dict]:
+        ...
+
     @auto_start
     def get_friend_list(self):
         return [
             dict(item)
             for item in (
                 self.robot.CGetFriendList(
                     self.wx_pid,
                 )
                 or []
             )
         ]
 
+    @overload
+    def get_wx_user_info(self, wxid: str):
+        ...
+
     @auto_start
     def get_wx_user_info(self, wxid: str):
         return json.loads(self.robot.CGetWxUserInfo(self.wx_pid, wxid))
 
     @property
     def wxid(self):
         return self.get_self_info()["wxId"]
 
     @property
     def self_path(self):
         return os.path.join(self.base_directory, str(self.wx_pid))
 
+    @overload
+    def get_self_info(self, refresh=False) -> Dict:
+        ...
+
     @auto_start
     def get_self_info(self, refresh=False):
         if refresh or not self.user_info:
             self.user_info = json.loads(
                 self.robot.CGetSelfInfo(
                     self.wx_pid,
                 )
             )
         return self.user_info
 
+    @overload
+    def check_friend_status(self, wxid: str) -> int:
+        ...
+
     @auto_start
     def check_friend_status(self, wxid: str):
         return self.robot.CCheckFriendStatus(self.wx_pid, wxid)
 
+    @overload
+    def get_com_work_path(self) -> int:
+        ...
+
     @auto_start
     def get_com_work_path(self):
         return self.robot.CGetComWorkPath(
             self.wx_pid,
         )
 
+    @overload
+    def start_receive_message(self, port: int) -> int:
+        ...
+
     @auto_start
     def start_receive_message(self, port: int):
         """
         开始接收消息
         :param port: 端口， port为0则使用COM Event推送
         """
         return self.robot.CStartReceiveMessage(self.wx_pid, port)
 
+    @overload
+    def stop_receive_message(self) -> int:
+        ...
+
     @auto_start
     def stop_receive_message(self):
         return self.robot.CStopReceiveMessage(
             self.wx_pid,
         )
 
+    @overload
+    def get_chat_room_member_ids(self, chatroom_id: str) -> List:
+        ...
+
     @auto_start
     def get_chat_room_member_ids(self, chatroom_id: str):
         wx_ids_str: str = self.robot.CGetChatRoomMembers(self.wx_pid, chatroom_id)[1][1]
         wx_ids = wx_ids_str.split("^G")
         return wx_ids
 
+    @overload
+    def get_chat_room_member_nickname(self, chatroom_id: str, wxid: str) -> str:
+        ...
+
     @auto_start
     def get_chat_room_member_nickname(self, chatroom_id: str, wxid: str):
         return self.robot.CGetChatRoomMemberNickname(self.wx_pid, chatroom_id, wxid)
 
     def get_chat_room_members(self, chatroom_id: str) -> List[dict]:
         """
         获取群成员id及昵称信息
@@ -241,97 +319,161 @@
                 {
                     "wx_id": wx_id,
                     "nickname": self.get_chat_room_member_nickname(chatroom_id, wx_id),
                 }
             )
         return results
 
+    @overload
+    def add_friend_by_wxid(self, wxid: str, message: str) -> int:
+        ...
+
     @auto_start
     def add_friend_by_wxid(self, wxid: str, message: str):
         return self.robot.CAddFriendByWxid(self.wx_pid, wxid, message)
 
+    @overload
+    def search_contact_by_net(self, keyword: str) -> List[Dict]:
+        ...
+
     @auto_start
     def search_contact_by_net(self, keyword: str):
         return [
             dict(item) for item in self.robot.CSearchContactByNet(self.wx_pid, keyword)
         ]
 
+    @overload
+    def add_brand_contact(self, public_id: str) -> int:
+        ...
+
     @auto_start
     def add_brand_contact(self, public_id: str):
         return self.robot.CAddBrandContact(self.wx_pid, public_id)
 
+    @overload
+    def change_wechat_ver(self, version: str) -> int:
+        ...
+
     @auto_start
-    def change_we_chat_ver(self, version: str):
+    def change_wechat_ver(self, version: str):
         return self.robot.CChangeWeChatVer(self.wx_pid, version)
 
+    @overload
+    def send_app_msg(self, wxid: str, app_id: str) -> int:
+        ...
+
     @auto_start
     def send_app_msg(self, wxid: str, app_id: str):
         return self.robot.CSendAppMsg(self.wx_pid, wxid, app_id)
 
+    @overload
+    def delete_user(self, wxid: str) -> int:
+        ...
+
     @auto_start
     def delete_user(self, wxid: str):
         return self.robot.CDeleteUser(self.wx_pid, wxid)
 
+    @overload
+    def is_wx_login(self) -> int:
+        ...
+
     @auto_start
     def is_wx_login(self) -> int:
         return self.robot.CIsWxLogin(
             self.wx_pid,
         )
 
+    @overload
+    def get_db_handles(self) -> List[Dict]:
+        ...
+
     @auto_start
     def get_db_handles(self):
         return [dict(item) for item in self.robot.CGetDbHandles(self.wx_pid)]
 
+    @overload
+    def register_event(self, event_sink: RobotEventSinkABC) -> int:
+        ...
+
     @auto_start
     def register_event(self, event_sink: RobotEventSinkABC):
         if self.event_connection:
             self.event_connection.__del__()
         self.event_connection = com_client.GetEvents(self.robot_event, event_sink)
         self.robot_event.CRegisterWxPidWithCookie(
             self.wx_pid, self.event_connection.cookie
         )
 
+    @overload
+    def get_wechat_ver(self) -> str:
+        ...
+
     @auto_start
-    def get_we_chat_ver(self) -> str:
+    def get_wechat_ver(self) -> str:
         return self.robot.CGetWeChatVer()
 
+    @overload
+    def hook_voice_msg(self, savepath: str) -> Union[int, str]:
+        ...
+
     @auto_start
     def hook_voice_msg(self, savepath: str) -> Union[int, str]:
         p = pathlib.Path(savepath)
         if not p.is_absolute():
             p = pathlib.Path.home().joinpath(p)
         result = self.robot.CHookVoiceMsg(self.wx_pid, str(p))
         if result == 0:
             self.voice_hook_path = str(p)
             return self.voice_hook_path
         return result
 
+    @overload
+    def unhook_voice_msg(self) -> int:
+        ...
+
     @auto_start
     def unhook_voice_msg(self):
         return self.robot.CUnHookVoiceMsg(self.wx_pid)
 
+    @overload
+    def hook_image_msg(self, savepath: str) -> Union[int, str]:
+        ...
+
     @auto_start
     def hook_image_msg(self, savepath: str) -> Union[int, str]:
         p = pathlib.Path(savepath)
         if not p.is_absolute():
             p = pathlib.Path.home().joinpath(p)
         result = self.robot.CHookImageMsg(self.wx_pid, str(p))
         if result == 0:
             self.image_hook_path = str(p)
             return self.image_hook_path
         return result
 
+    @overload
+    def unhook_image_msg(self) -> int:
+        ...
+
     @auto_start
     def unhook_image_msg(self):
         return self.robot.CUnHookImageMsg(self.wx_pid)
 
+    @overload
+    def open_browser(self, url: str) -> int:
+        ...
+
     @auto_start
     def open_browser(self, url: str):
         return self.robot.COpenBrowser(self.wx_pid, url)
 
+    @overload
+    def get_history_public_msg(self, public_id: str, offset: str = "") -> List:
+        ...
+
     @auto_start
     def get_history_public_msg(self, public_id: str, offset: str = ""):
         """
         获取公众号历史消息
 
         Args:
             offset (str, optional): 起始偏移，为空的话则从新到久获取十条，该值可从返回数据中取得
@@ -340,25 +482,35 @@
         try:
             msgs = json.loads(r[0])
         except (IndexError, json.JSONDecodeError) as e:
             logger.exception(e)
             return []
         return msgs
 
+    @overload
+    def forward_message(self, wxid: str, msgid: int) -> int:
+        ...
+
     @auto_start
     def forward_message(self, wxid: str, msgid: int):
         """
         转发消息
 
         Args:
             wxid (str): 消息接收人
             msgid (int): 消息id
         """
         return self.robot.CForwardMessage(self.wx_pid, wxid, msgid)
 
+    @overload
+    def get_qrcode_image(
+        self,
+    ) -> bytes:
+        ...
+
     @auto_start
     def get_qrcode_image(
         self,
     ) -> bytes:
         """
         获取二维码，同时切换到扫码登陆
 
@@ -370,14 +522,18 @@
         >>> from PIL import Image
         >>> buf = wx.GetQrcodeImage()
         >>> image = Image.open(BytesIO(buf)).convert("L")
         >>> image.save('./qrcode.png')
         """
         return self.robot.CGetQrcodeImage(self.wx_pid)
 
+    @overload
+    def get_a8_key(self, url: str) -> str:
+        ...
+
     @auto_start
     def get_a8_key(self, url: str):
         """
         获取A8Key
 
         Args:
             url (str): 公众号文章链接
@@ -386,34 +542,46 @@
         try:
             result = json.loads(r[0])
         except (IndexError, json.JSONDecodeError) as e:
             logger.exception(e)
             return ""
         return result
 
+    @overload
+    def send_xml_msg(self, wxid: str, xml: str, img_path: str) -> int:
+        ...
+
     @auto_start
     def send_xml_msg(self, wxid: str, xml: str, img_path: str) -> int:
         """
         发送原始xml消息
 
         Returns:
             int: 0表示成功
         """
         return self.robot.CSendXmlMsg(self.wx_pid, wxid, xml, img_path)
 
+    @overload
+    def logout(self) -> int:
+        ...
+
     @auto_start
     def logout(self) -> int:
         """
         登出
 
         Returns:
             int: 0表示成功
         """
         return self.robot.CLogout(self.wx_pid)
 
+    @overload
+    def get_transfer(self, wxid: str, transactionid: str, transferid: int) -> int:
+        ...
+
     @auto_start
     def get_transfer(self, wxid: str, transactionid: str, transferid: int) -> int:
         """
         收款
 
         Args:
             wxid : str
@@ -425,18 +593,26 @@
 
         Returns:
             int
                 成功返回0，失败返回非0值.
         """
         return self.robot.CGetTransfer(self.wx_pid, wxid, transactionid, transferid)
 
+    @overload
+    def send_emotion(self, wxid: str, img_path: str) -> int:
+        ...
+
     @auto_start
     def send_emotion(self, wxid: str, img_path: str) -> int:
         return self.robot.CSendEmotion(self.wx_pid, wxid, img_path)
 
+    @overload
+    def get_msg_cdn(self, msgid: int) -> str:
+        ...
+
     @auto_start
     def get_msg_cdn(self, msgid: int) -> str:
         """
         下载图片、视频、文件等
 
         Returns:
             str
@@ -509,17 +685,24 @@
     _instances: Dict[int, "WechatBot"] = {}
     _robot_object_id = "WeChatRobot.CWeChatRobot"
     _robot_event_id = "WeChatRobot.RobotEvent"
 
     @classmethod
     def get(cls, wx_pid) -> "WechatBot":
         if wx_pid not in cls._instances:
-            cls._instances[wx_pid] = WechatBot(
-                wx_pid, cls._robot_object_id, cls._robot_event_id
+            wechat_version = os.environ.get(
+                "WHOCHAT_WECHAT_VERSION"
+            ) or cls.get_latest_wechat_version(fill=".99")
+            bot = WechatBot(
+                wx_pid,
+                cls._robot_object_id,
+                cls._robot_event_id,
+                wechat_version=wechat_version,
             )
+            cls._instances[wx_pid] = bot
         return cls._instances[wx_pid]
 
     @classmethod
     def exit(cls):
         logger.info("卸载注入的dll...")
         for instance in cls._instances.values():
             instance.stop_robot_service()
@@ -572,15 +755,15 @@
             cls.robot_event.CRegisterWxPidWithCookie(wx_pid, connection.cookie)
 
     @classmethod
     def get_current_dir(cls):
         return os.getcwd()
 
     @classmethod
-    def get_latest_wechat_version(cls):
+    def get_latest_wechat_version(cls, fill: str = None):
         logger.info("获取微信最新版本号...")
         with request.urlopen(
             request.Request(
                 "https://pc.weixin.qq.com/?lang=zh_CN",
                 headers={
                     "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/113.0.0.0 Safari/537.36"
                 },
@@ -589,9 +772,11 @@
         ) as fp:
             html = fp.read().decode()
         m = re.search(r"download-version\">(.*?)</span>", html)
         if not m:
             logger.warning("获取微信最新版本号异常")
             return
         version = m.group(1)
+        if fill:
+            version = version + fill
         logger.info(f"微信最新版本号：{version}")
         return version
```

### Comparing `whochat-1.3.3/whochat/cli.py` & `whochat-1.3.4/whochat/cli.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/logger.py` & `whochat-1.3.4/whochat/logger.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/messages/tcp.py` & `whochat-1.3.4/whochat/messages/tcp.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/messages/websocket.py` & `whochat-1.3.4/whochat/messages/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
 
         self.ws_server = None
         self.clients = set()
         self._deque = deque(maxlen=self.queue.maxsize)
         self._event_waiter = EventWaiter(2)
 
         self._stop_broadcast = False
+        self._stop_receive_msg = False
         self._stop_websocket = asyncio.Event()
         Signal.register_sigint(self.shutdown)
 
     async def handler(self, websocket):
         if websocket not in self.clients:
             logger.info(f"Accept connection from {websocket.remote_address}")
             self.clients.add(websocket)
@@ -117,15 +118,15 @@
                 bot.register_event(sink)
             self._event_waiter.create_handle()
             self._event_waiter.wait_forever()
         finally:
             comtypes.CoUninitialize()
 
     async def deque_to_queue(self):
-        while True:
+        while not self._stop_receive_msg:
             try:
                 e = self._deque.popleft()
                 await self.queue.put(e)
             except IndexError:
                 await asyncio.sleep(0.1)
 
     async def start_receive_msg(self):
@@ -136,14 +137,15 @@
         logger.info("微信消息接收服务已停止")
 
     def stop_websocket(self):
         self._stop_websocket.set()
 
     def stop_receive_msg(self):
         self._event_waiter.stop()
+        self._stop_receive_msg = True
         for wx_pid in self.wx_pids:
             bot = WechatBotFactory.get(wx_pid)
             bot.stop_receive_message()
             bot.stop_robot_service()
 
     def stop_broadcast(self):
         self._stop_broadcast = True
@@ -167,23 +169,25 @@
     def shutdown(self):
         logger.info("停止服务中...")
         self.stop_websocket()
         self.stop_broadcast()
         self.stop_receive_msg()
 
     async def serve(self):
-        websocket_task = asyncio.create_task(self.serve_websocket())
-        receive_msg_task = asyncio.create_task(self.start_receive_msg())
-        broadcast_task = asyncio.create_task(self.broadcast_received_msg())
-
-        await websocket_task
-        self.stop_broadcast()
-        self.stop_receive_msg()
-        await receive_msg_task
-        await broadcast_task
+        try:
+            websocket_task = asyncio.create_task(self.serve_websocket())
+            receive_msg_task = asyncio.create_task(self.start_receive_msg())
+            broadcast_task = asyncio.create_task(self.broadcast_received_msg())
+
+            await websocket_task
+            await receive_msg_task
+            await broadcast_task
+        except Exception as e:
+            logger.exception(e)
+            raise
 
 
 class WechatWebsocketServer(WechatMessageWebsocketServer):
     def __init__(self, *args, **kwargs):
         warnings.warn(" 'WechatWebsocketServer' 已更名为 'WechatMessageWebsocketServer'")
         super().__init__(*args, **kwargs)
```

### Comparing `whochat-1.3.3/whochat/rpc/clients/websocket.py` & `whochat-1.3.4/whochat/rpc/clients/websocket.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 import asyncio
 import json
 import logging
-import time
 from collections import defaultdict
 from functools import partial
 from typing import Any, Dict
 
 import websockets
 import websockets.client
 from jsonrpcclient import request as req
 
 from whochat.rpc.handlers import make_rpc_methods
 
 logger = logging.getLogger("whochat")
 
-
-class unset:  # noqa
-    pass
+unset = object()
 
 
 class Timeout(Exception):
     pass
 
 
 class BotWebsocketRPCClient:
@@ -43,73 +40,87 @@
 
     async def start_sender(
         self, websocket: "websockets.client.WebSocketClientProtocol"
     ):
         while not websocket.closed:
             request_dict = await self.send_queue.get()
             logger.debug(f"SEND: {request_dict}")
-            await websocket.send(json.dumps(request_dict))
+            try:
+                await websocket.send(json.dumps(request_dict))
+            except websockets.ConnectionClosed:
+                await self.send_queue.put(request_dict)
+                raise
 
     async def start_receiver(
         self, websocket: "websockets.client.WebSocketClientProtocol"
     ):
         async for message in websocket:
             logger.debug(f"RECV: {message}")
             try:
                 response_dict = json.loads(message)
                 if "result" in response_dict:
                     self._results[response_dict["id"]] = response_dict["result"]
                 elif "error" in response_dict:
+                    self._results[response_dict["id"]] = response_dict["error"]
                     logger.error(response_dict["error"])
             except json.JSONDecodeError:
                 continue
 
     async def start_consumer(self):
         logger.info("Starting rpc client consumer")
         async for websocket in websockets.client.connect(self.ws_uri):
             websocket: "websockets.client.WebSocketClientProtocol"
             logger.info(f"Websocket client bind on {websocket.local_address}")
+            gathered = asyncio.gather(
+                self.start_receiver(websocket),
+                self.start_sender(websocket),
+            )
             try:
-                await asyncio.gather(
-                    self.start_receiver(websocket),
-                    self.start_sender(websocket),
-                )
-            except websockets.ConnectionClosed:
+                await gathered
+            except websockets.ConnectionClosedOK:
                 logger.warning(
                     f"Websocket{websocket.local_address} closed",
                 )
+            except websockets.ConnectionClosedError:
+                logger.warning(
+                    f"Websocket{websocket.local_address} closed unexpectedly",
+                )
+            finally:
+                gathered.cancel()
 
     def consume_in_background(self):
         asyncio.create_task(self.start_consumer())
         asyncio.create_task(self.start_result_cleaner())
 
+    async def _send_and_recv(self, request):
+        await self.send_queue.put(request)
+        request_id = request["id"]
+        while True:
+            if self._results[request_id] is unset:
+                await asyncio.sleep(0.1)
+            else:
+                return self._results[request_id]
+
     async def rpc_call(self, name: str, params, timeout):
         request = req(name, params)
         request_id = request["id"]
         self._current_request_id = request_id
-        await self.send_queue.put(request)
         if timeout < 0:
+            asyncio.create_task(self.send_queue.put(request))
             return request_id
-        elif timeout == 0:
-            while True:
-                if self._results[request_id] is unset:
-                    await asyncio.sleep(0.1)
-                else:
-                    return self._results[request_id]
+        if timeout == 0:
+            return await self._send_and_recv(request)
         else:
-            start = time.perf_counter()
-            while time.perf_counter() < start + timeout:
-                if self._results[request_id] is unset:
-                    await asyncio.sleep(0.1)
-                else:
-                    return self._results[request_id]
-            raise Timeout(f"Timeout: rpc call timeout: {name}, params {params}")
+            try:
+                return await asyncio.wait_for(self._send_and_recv(request), timeout)
+            except asyncio.TimeoutError:
+                raise Timeout(f"Timeout: rpc call timeout: {name}, params {params}")
 
     def __getattr__(self, item):
-        def remote_func(*params, timeout=0):
+        def remote_func(*params, timeout=5):
             """
             :param params: 仅支持位置参数
             :param timeout: 超时时间。0: 阻塞等待返回结果, <0: 直接返回不等结果,  >0: 等待超时时间
             """
             return self.rpc_call(item, params, timeout)
 
         return remote_func
```

### Comparing `whochat-1.3.3/whochat/rpc/docs.py` & `whochat-1.3.4/whochat/rpc/docs.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/rpc/handlers.py` & `whochat-1.3.4/whochat/rpc/handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,60 +22,62 @@
 )
 
 
 class BotRpcHelper:
     bot_methods = {
         method.__name__: method
         for method in [
-            WechatBot.start_robot_service,
-            WechatBot.stop_robot_service,
-            WechatBot.start_receive_message,
-            WechatBot.stop_receive_message,
-            WechatBot.get_wx_user_info,
-            WechatBot.send_text,
-            WechatBot.send_image,
-            WechatBot.send_file,
-            WechatBot.send_card,
-            WechatBot.send_article,
-            WechatBot.send_app_msg,
-            WechatBot.send_at_text,
-            WechatBot.search_contact_by_net,
-            WechatBot.get_friend_list,
-            WechatBot.get_self_info,
+            WechatBot.add_brand_contact,
+            WechatBot.add_friend_by_wxid,
+            WechatBot.change_wechat_ver,
+            WechatBot.delete_user,
+            WechatBot.forward_message,
+            WechatBot.get_a8_key,
+            WechatBot.get_base_directory,
             WechatBot.get_chat_room_member_ids,
             WechatBot.get_chat_room_member_nickname,
             WechatBot.get_chat_room_members,
-            WechatBot.add_friend_by_wxid,
-            WechatBot.add_brand_contact,
-            WechatBot.get_we_chat_ver,
-            WechatBot.is_wx_login,
-            WechatBot.delete_user,
             WechatBot.get_db_handles,
-            WechatBot.hook_image_msg,
-            WechatBot.unhook_image_msg,
-            WechatBot.hook_voice_msg,
-            WechatBot.unhook_voice_msg,
-            WechatBot.open_browser,
+            WechatBot.get_friend_list,
             WechatBot.get_history_public_msg,
-            WechatBot.forward_message,
+            WechatBot.get_msg_cdn,
             WechatBot.get_qrcode_image,
-            WechatBot.get_a8_key,
-            WechatBot.send_xml_msg,
-            WechatBot.logout,
+            WechatBot.get_self_info,
             WechatBot.get_transfer,
-            WechatBot.send_emotion,
-            WechatBot.get_msg_cdn,
-            WechatBot.get_base_directory,
+            WechatBot.get_wechat_ver,
+            WechatBot.get_wx_user_info,
+            WechatBot.hook_image_msg,
+            WechatBot.hook_voice_msg,
+            WechatBot.is_wx_login,
+            WechatBot.logout,
+            WechatBot.open_browser,
             WechatBot.prevent_revoke,
-            WechatBotFactory.list_wechat,
-            WechatBotFactory.start_wechat,
-            WechatBotFactory.get_we_chat_ver,
+            WechatBot.search_contact_by_net,
+            WechatBot.send_app_msg,
+            WechatBot.send_article,
+            WechatBot.send_at_text,
+            WechatBot.send_card,
+            WechatBot.send_emotion,
+            WechatBot.send_file,
+            WechatBot.send_image,
+            WechatBot.send_text,
+            WechatBot.send_xml_msg,
+            WechatBot.start_receive_message,
+            WechatBot.start_robot_service,
+            WechatBot.stop_receive_message,
+            WechatBot.stop_robot_service,
+            WechatBot.unhook_image_msg,
+            WechatBot.unhook_voice_msg,
+            WechatBotFactory.get_current_dir,
+            WechatBotFactory.get_latest_wechat_version,
             WechatBotFactory.get_robot_pid,
+            WechatBotFactory.get_we_chat_ver,
             WechatBotFactory.kill_robot,
-            WechatBotFactory.get_current_dir,
+            WechatBotFactory.list_wechat,
+            WechatBotFactory.start_wechat,
         ]
     }
     rpc_methods = {}
     async_rpc_methods = {}
 
     @classmethod
     def make_rpc_methods(cls):
@@ -110,28 +112,36 @@
             return cls.async_rpc_methods
 
         from whochat.bot import WechatBotFactory
 
         def factory(func):
             @functools.wraps(func)
             async def bot_self_func(wx_pid, *args, **kwargs):
-                bot = WechatBotFactory.get(wx_pid)
-                loop = asyncio.get_running_loop()
-                result = await loop.run_in_executor(
-                    bot_executor,
-                    functools.partial(func, bot, *args, **kwargs),
-                )
-                return Success(result)
+                try:
+                    bot = WechatBotFactory.get(wx_pid)
+                    loop = asyncio.get_running_loop()
+                    result = await loop.run_in_executor(
+                        bot_executor,
+                        functools.partial(func, bot, *args, **kwargs),
+                    )
+                    return Success(result)
+                except Exception as e:
+                    logger.exception(e)
+                    raise
 
             @functools.wraps(func)
             async def normal_func(*args, **kwargs):
-                _func = functools.partial(func, *args, **kwargs)
-                loop = asyncio.get_running_loop()
-                result = await loop.run_in_executor(bot_executor, _func)
-                return Success(result)
+                try:
+                    _func = functools.partial(func, *args, **kwargs)
+                    loop = asyncio.get_running_loop()
+                    result = await loop.run_in_executor(bot_executor, _func)
+                    return Success(result)
+                except Exception as e:
+                    logger.exception(e)
+                    raise
 
             if func.__qualname__.split(".", maxsplit=1)[0] == "WechatBot":
                 return bot_self_func
             return normal_func
 
         for name, function in cls.bot_methods.items():
             cls.async_rpc_methods[name] = factory(function)
```

### Comparing `whochat-1.3.3/whochat/rpc/servers/http.py` & `whochat-1.3.4/whochat/rpc/servers/http.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/rpc/servers/websocket.py` & `whochat-1.3.4/whochat/rpc/servers/websocket.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/signals.py` & `whochat-1.3.4/whochat/signals.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat/utils.py` & `whochat-1.3.4/whochat/utils.py`

 * *Files identical despite different names*

### Comparing `whochat-1.3.3/whochat.egg-info/PKG-INFO` & `whochat-1.3.4/whochat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whochat
-Version: 1.3.3
+Version: 1.3.4
 Summary: 一个命令就可启用的微信机器人
 Home-page: https://github.com/amchii/whochat
 Author: Amchii
 Author-email: finethankuandyou@gmail.com
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/amchii/whochat
 Classifier: Intended Audience :: Developers
@@ -189,14 +189,19 @@
     "id": 4
 }
 ```
 
 [CHANGELOG](https://github.com/amchii/whochat/blob/main/CHANGELOG.md)
 
 [Tags](https://github.com/amchii/whochat/tags)
+## v1.3.4
+* 自动设置微信版本号避免更新
+* 增加环境变量`WHOCHAT_WECHAT_VERSION`自定义微信版本号
+* 尝试使`BotWebsocketRPCClient.rpc_call`更正确地运行
+
 ## v1.3.3
 * 增加获取微信最新版本号的方法
 * 修复Mac用户发送@消息无法正确解析的问题
 
 ## v1.3.2
 * 修改日志级别，增加日志文件记录
```

### Comparing `whochat-1.3.3/whochat.egg-info/SOURCES.txt` & `whochat-1.3.4/whochat.egg-info/SOURCES.txt`

 * *Files identical despite different names*


# Comparing `tmp/Twitch_Edog0049a-0.0.31.tar.gz` & `tmp/Twitch_Edog0049a-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Twitch_Edog0049a-0.0.31.tar", last modified: Sun May 28 22:58:05 2023, max compression
+gzip compressed data, was "Twitch_Edog0049a-0.0.32.tar", last modified: Sun May 28 23:03:47 2023, max compression
```

## Comparing `Twitch_Edog0049a-0.0.31.tar` & `Twitch_Edog0049a-0.0.32.tar`

### file list

```diff
@@ -1,77 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.905397 Twitch_Edog0049a-0.0.31/
--rw-rw-rw-   0        0        0     1079 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.31/LICENSE.txt
--rw-rw-rw-   0        0        0     1742 2023-05-28 22:58:05.905397 Twitch_Edog0049a-0.0.31/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.31/README.md
--rw-rw-rw-   0        0        0       82 2023-05-28 21:47:57.000000 Twitch_Edog0049a-0.0.31/pyproject.toml
--rw-rw-rw-   0        0        0      726 2023-05-28 22:58:05.906395 Twitch_Edog0049a-0.0.31/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.749207 Twitch_Edog0049a-0.0.31/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.764688 Twitch_Edog0049a-0.0.31/src/Twitch/
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.773298 Twitch_Edog0049a-0.0.31/src/Twitch/API/
--rw-rw-rw-   0        0        0      355 2023-04-16 12:59:45.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.862396 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/
--rw-rw-rw-   0        0        0      714 2023-05-07 12:32:52.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Ads.py
--rw-rw-rw-   0        0        0     2651 2023-05-07 12:33:14.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Analytics.py
--rw-rw-rw-   0        0        0     3990 2023-05-06 20:34:56.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Bits.py
--rw-rw-rw-   0        0        0     8807 2023-05-07 12:29:11.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/ChannelPoints.py
--rw-rw-rw-   0        0        0     4628 2023-05-06 14:00:30.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Channels.py
--rw-rw-rw-   0        0        0     1762 2023-05-07 12:30:48.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Charity.py
--rw-rw-rw-   0        0        0    10043 2023-05-14 11:39:53.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Chat.py
--rw-rw-rw-   0        0        0     1907 2023-05-21 12:49:05.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Clips.py
--rw-rw-rw-   0        0        0      846 2023-04-23 19:40:21.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Entitlements.py
--rw-rw-rw-   0        0        0     1273 2023-04-23 19:41:04.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/EventSub.py
--rw-rw-rw-   0        0        0     4942 2023-04-23 19:40:49.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Extensions.py
--rw-rw-rw-   0        0        0      800 2023-04-23 19:41:21.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Games.py
--rw-rw-rw-   0        0        0      433 2023-04-23 19:41:40.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Goals.py
--rw-rw-rw-   0        0        0      439 2023-04-23 19:41:56.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/HypeTrain.py
--rw-rw-rw-   0        0        0     7481 2023-04-23 19:42:07.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Moderation.py
--rw-rw-rw-   0        0        0     1259 2023-04-23 19:43:41.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Music.py
--rw-rw-rw-   0        0        0     1171 2023-04-23 19:42:22.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Polls.py
--rw-rw-rw-   0        0        0     1207 2023-04-23 19:42:34.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Predictions.py
--rw-rw-rw-   0        0        0      806 2023-04-23 19:42:46.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Raids.py
--rw-rw-rw-   0        0        0     7229 2023-05-07 12:38:56.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/ResponseTypes.py
--rw-rw-rw-   0        0        0     2542 2023-04-23 19:43:14.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Schedule.py
--rw-rw-rw-   0        0        0      822 2023-04-23 19:43:27.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Search.py
--rw-rw-rw-   0        0        0     1989 2023-04-23 19:43:53.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Streams.py
--rw-rw-rw-   0        0        0      860 2023-04-23 19:44:04.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Subscriptions.py
--rw-rw-rw-   0        0        0      820 2023-04-23 19:44:19.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Tags.py
--rw-rw-rw-   0        0        0      808 2023-04-23 19:44:31.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Teams.py
--rw-rw-rw-   0        0        0     3252 2023-04-30 15:25:37.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Users.py
--rw-rw-rw-   0        0        0     1835 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Utils.py
--rw-rw-rw-   0        0        0     2117 2023-05-06 14:01:27.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Videos.py
--rw-rw-rw-   0        0        0      628 2023-04-29 20:08:34.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/Whispers.py
--rw-rw-rw-   0        0        0      180 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/__imports.py
--rw-rw-rw-   0        0        0    14010 2023-05-28 22:17:32.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/Resources/__init__.py
--rw-rw-rw-   0        0        0    36055 2023-05-14 11:48:59.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/TwitchAPI.py
--rw-rw-rw-   0        0        0     1008 2023-04-30 22:42:20.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/_ApiRequest.py
--rw-rw-rw-   0        0        0      176 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.31/src/Twitch/API/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.872417 Twitch_Edog0049a-0.0.31/src/Twitch/ChatInterface/
--rw-rw-rw-   0        0        0       94 2023-03-26 15:46:11.000000 Twitch_Edog0049a-0.0.31/src/Twitch/ChatInterface/Exceptions.py
--rw-rw-rw-   0        0        0     4368 2023-04-08 23:17:22.000000 Twitch_Edog0049a-0.0.31/src/Twitch/ChatInterface/IrcController.py
--rw-rw-rw-   0        0        0    25655 2023-04-08 21:10:07.000000 Twitch_Edog0049a-0.0.31/src/Twitch/ChatInterface/MessageHandler.py
--rw-rw-rw-   0        0        0     1388 2023-03-11 21:23:16.000000 Twitch_Edog0049a-0.0.31/src/Twitch/ChatInterface/TokenBucket.py
--rw-rw-rw-   0        0        0    22973 2023-04-08 23:31:19.000000 Twitch_Edog0049a-0.0.31/src/Twitch/ChatInterface/TwitchChatInterface.py
--rw-rw-rw-   0        0        0      138 2023-04-23 19:47:57.000000 Twitch_Edog0049a-0.0.31/src/Twitch/ChatInterface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.879911 Twitch_Edog0049a-0.0.31/src/Twitch/EventSub/
--rw-rw-rw-   0        0        0      136 2023-04-01 21:27:54.000000 Twitch_Edog0049a-0.0.31/src/Twitch/EventSub/EventSubConnector.py
--rw-rw-rw-   0        0        0       71 2023-04-09 00:14:32.000000 Twitch_Edog0049a-0.0.31/src/Twitch/EventSub/EventSubInterface.py
--rw-rw-rw-   0        0        0       48 2023-04-09 00:14:11.000000 Twitch_Edog0049a-0.0.31/src/Twitch/EventSub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.885022 Twitch_Edog0049a-0.0.31/src/Twitch/OAuth/
--rw-rw-rw-   0        0        0      573 2023-04-01 19:02:07.000000 Twitch_Edog0049a-0.0.31/src/Twitch/OAuth/Exceptions.py
--rw-rw-rw-   0        0        0     4044 2023-04-30 13:42:07.000000 Twitch_Edog0049a-0.0.31/src/Twitch/OAuth/Oauth.py
--rw-rw-rw-   0        0        0       88 2023-04-23 19:49:34.000000 Twitch_Edog0049a-0.0.31/src/Twitch/OAuth/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.891870 Twitch_Edog0049a-0.0.31/src/Twitch/PubSub/
--rw-rw-rw-   0        0        0      807 2023-04-08 14:06:35.000000 Twitch_Edog0049a-0.0.31/src/Twitch/PubSub/PubSubConnector.py
--rw-rw-rw-   0        0        0       32 2023-04-08 15:26:06.000000 Twitch_Edog0049a-0.0.31/src/Twitch/PubSub/PubSubInterface.py
--rw-rw-rw-   0        0        0       21 2023-04-08 15:31:25.000000 Twitch_Edog0049a-0.0.31/src/Twitch/PubSub/Topics.py
--rw-rw-rw-   0        0        0       91 2023-04-08 17:07:40.000000 Twitch_Edog0049a-0.0.31/src/Twitch/PubSub/__init__.py
--rw-rw-rw-   0        0        0    10296 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.31/src/Twitch/Scope.py
--rw-rw-rw-   0        0        0     1976 2023-05-21 13:26:58.000000 Twitch_Edog0049a-0.0.31/src/Twitch/SubscriptionTypes.py
--rw-rw-rw-   0        0        0      391 2023-05-28 22:56:12.000000 Twitch_Edog0049a-0.0.31/src/Twitch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.902405 Twitch_Edog0049a-0.0.31/src/Twitch_Edog0049a.egg-info/
--rw-rw-rw-   0        0        0     1742 2023-05-28 22:58:05.000000 Twitch_Edog0049a-0.0.31/src/Twitch_Edog0049a.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2222 2023-05-28 22:58:05.000000 Twitch_Edog0049a-0.0.31/src/Twitch_Edog0049a.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 22:58:05.000000 Twitch_Edog0049a-0.0.31/src/Twitch_Edog0049a.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 22:58:05.000000 Twitch_Edog0049a-0.0.31/src/Twitch_Edog0049a.egg-info/namespace_packages.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 22:58:05.000000 Twitch_Edog0049a-0.0.31/src/Twitch_Edog0049a.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 22:58:05.903402 Twitch_Edog0049a-0.0.31/test/
--rw-rw-rw-   0        0        0     1003 2023-04-08 21:18:43.000000 Twitch_Edog0049a-0.0.31/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:03:47.484408 Twitch_Edog0049a-0.0.32/
+-rw-rw-rw-   0        0        0     1079 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.32/LICENSE.txt
+-rw-rw-rw-   0        0        0     1742 2023-05-28 23:03:47.484408 Twitch_Edog0049a-0.0.32/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.32/README.md
+-rw-rw-rw-   0        0        0       82 2023-05-28 21:47:57.000000 Twitch_Edog0049a-0.0.32/pyproject.toml
+-rw-rw-rw-   0        0        0      726 2023-05-28 23:03:47.486402 Twitch_Edog0049a-0.0.32/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 23:03:47.440102 Twitch_Edog0049a-0.0.32/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 23:03:47.470443 Twitch_Edog0049a-0.0.32/src/Twitch/
+-rw-rw-rw-   0        0        0    10296 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.32/src/Twitch/Scope.py
+-rw-rw-rw-   0        0        0     1976 2023-05-21 13:26:58.000000 Twitch_Edog0049a-0.0.32/src/Twitch/SubscriptionTypes.py
+-rw-rw-rw-   0        0        0       76 2023-05-28 23:03:17.000000 Twitch_Edog0049a-0.0.32/src/Twitch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:03:47.480397 Twitch_Edog0049a-0.0.32/src/Twitch_Edog0049a.egg-info/
+-rw-rw-rw-   0        0        0     1742 2023-05-28 23:03:47.000000 Twitch_Edog0049a-0.0.32/src/Twitch_Edog0049a.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2023-05-28 23:03:47.000000 Twitch_Edog0049a-0.0.32/src/Twitch_Edog0049a.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:03:47.000000 Twitch_Edog0049a-0.0.32/src/Twitch_Edog0049a.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 23:03:47.000000 Twitch_Edog0049a-0.0.32/src/Twitch_Edog0049a.egg-info/namespace_packages.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 23:03:47.000000 Twitch_Edog0049a-0.0.32/src/Twitch_Edog0049a.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 23:03:47.482949 Twitch_Edog0049a-0.0.32/test/
+-rw-rw-rw-   0        0        0     1003 2023-04-08 21:18:43.000000 Twitch_Edog0049a-0.0.32/test/test1.py
```

### Comparing `Twitch_Edog0049a-0.0.31/LICENSE.txt` & `Twitch_Edog0049a-0.0.32/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.31/PKG-INFO` & `Twitch_Edog0049a-0.0.32/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Twitch_Edog0049a
-Version: 0.0.31
+Version: 0.0.32
 Summary: Twitch library for chat, api, pubs, and eventsub
 Home-page: https://github.com/eli-reid/twitch
 Author: Eli Reid
 Author-email: EliR@Elireid.com
 Project-URL: Bug Tracker, https://github.com/eli-reid/twitch/-/issues
 Project-URL: repository, https://github.com/eli-reid/twitch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Twitch_Edog0049a-0.0.31/setup.cfg` & `Twitch_Edog0049a-0.0.32/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2054 7769 7463 685f 4564 6f67 3030   = Twitch_Edog00
 00000020: 3439 610d 0a76 6572 7369 6f6e 203d 2030  49a..version = 0
-00000030: 2e30 2e33 310d 0a61 7574 686f 7220 3d20  .0.31..author = 
+00000030: 2e30 2e33 320d 0a61 7574 686f 7220 3d20  .0.32..author = 
 00000040: 456c 6920 5265 6964 0d0a 6175 7468 6f72  Eli Reid..author
 00000050: 5f65 6d61 696c 203d 2045 6c69 5240 456c  _email = EliR@El
 00000060: 6972 6569 642e 636f 6d0d 0a64 6573 6372  ireid.com..descr
 00000070: 6970 7469 6f6e 203d 2054 7769 7463 6820  iption = Twitch 
 00000080: 6c69 6272 6172 7920 666f 7220 6368 6174  library for chat
 00000090: 2c20 6170 692c 2070 7562 732c 2061 6e64  , api, pubs, and
 000000a0: 2065 7665 6e74 7375 620d 0a6c 6f6e 675f   eventsub..long_
```

### Comparing `Twitch_Edog0049a-0.0.31/src/Twitch/Scope.py` & `Twitch_Edog0049a-0.0.32/src/Twitch/Scope.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.31/src/Twitch/SubscriptionTypes.py` & `Twitch_Edog0049a-0.0.32/src/Twitch/SubscriptionTypes.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.31/src/Twitch_Edog0049a.egg-info/PKG-INFO` & `Twitch_Edog0049a-0.0.32/src/Twitch_Edog0049a.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Twitch-Edog0049a
-Version: 0.0.31
+Version: 0.0.32
 Summary: Twitch library for chat, api, pubs, and eventsub
 Home-page: https://github.com/eli-reid/twitch
 Author: Eli Reid
 Author-email: EliR@Elireid.com
 Project-URL: Bug Tracker, https://github.com/eli-reid/twitch/-/issues
 Project-URL: repository, https://github.com/eli-reid/twitch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Twitch_Edog0049a-0.0.31/test/test1.py` & `Twitch_Edog0049a-0.0.32/test/test1.py`

 * *Files identical despite different names*


# Comparing `tmp/Twitch_Edog0049a-0.0.35.tar.gz` & `tmp/Twitch_Edog0049a-0.0.36.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Twitch_Edog0049a-0.0.35.tar", last modified: Sun May 28 23:16:46 2023, max compression
+gzip compressed data, was "Twitch_Edog0049a-0.0.36.tar", last modified: Sun May 28 23:29:47 2023, max compression
```

## Comparing `Twitch_Edog0049a-0.0.35.tar` & `Twitch_Edog0049a-0.0.36.tar`

### file list

```diff
@@ -1,94 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:46.001423 Twitch_Edog0049a-0.0.35/
--rw-rw-rw-   0        0        0     1079 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.35/LICENSE.txt
--rw-rw-rw-   0        0        0     1742 2023-05-28 23:16:46.001423 Twitch_Edog0049a-0.0.35/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.35/README.md
--rw-rw-rw-   0        0        0       82 2023-05-28 21:47:57.000000 Twitch_Edog0049a-0.0.35/pyproject.toml
--rw-rw-rw-   0        0        0      651 2023-05-28 23:16:46.003434 Twitch_Edog0049a-0.0.35/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.865455 Twitch_Edog0049a-0.0.35/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.878514 Twitch_Edog0049a-0.0.35/src/Twitch/
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.885698 Twitch_Edog0049a-0.0.35/src/Twitch/API/
--rw-rw-rw-   0        0        0      355 2023-04-16 12:59:45.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.938875 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/
--rw-rw-rw-   0        0        0      714 2023-05-07 12:32:52.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Ads.py
--rw-rw-rw-   0        0        0     2651 2023-05-07 12:33:14.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Analytics.py
--rw-rw-rw-   0        0        0     3990 2023-05-06 20:34:56.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Bits.py
--rw-rw-rw-   0        0        0     8807 2023-05-07 12:29:11.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/ChannelPoints.py
--rw-rw-rw-   0        0        0     4628 2023-05-06 14:00:30.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Channels.py
--rw-rw-rw-   0        0        0     1762 2023-05-07 12:30:48.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Charity.py
--rw-rw-rw-   0        0        0    10043 2023-05-14 11:39:53.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Chat.py
--rw-rw-rw-   0        0        0     1907 2023-05-21 12:49:05.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Clips.py
--rw-rw-rw-   0        0        0      846 2023-04-23 19:40:21.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Entitlements.py
--rw-rw-rw-   0        0        0     1273 2023-04-23 19:41:04.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/EventSub.py
--rw-rw-rw-   0        0        0     4942 2023-04-23 19:40:49.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Extensions.py
--rw-rw-rw-   0        0        0      800 2023-04-23 19:41:21.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Games.py
--rw-rw-rw-   0        0        0      433 2023-04-23 19:41:40.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Goals.py
--rw-rw-rw-   0        0        0      439 2023-04-23 19:41:56.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/HypeTrain.py
--rw-rw-rw-   0        0        0     7481 2023-04-23 19:42:07.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Moderation.py
--rw-rw-rw-   0        0        0     1259 2023-04-23 19:43:41.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Music.py
--rw-rw-rw-   0        0        0     1171 2023-04-23 19:42:22.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Polls.py
--rw-rw-rw-   0        0        0     1207 2023-04-23 19:42:34.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Predictions.py
--rw-rw-rw-   0        0        0      806 2023-04-23 19:42:46.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Raids.py
--rw-rw-rw-   0        0        0     7229 2023-05-07 12:38:56.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/ResponseTypes.py
--rw-rw-rw-   0        0        0     2542 2023-04-23 19:43:14.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Schedule.py
--rw-rw-rw-   0        0        0      822 2023-04-23 19:43:27.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Search.py
--rw-rw-rw-   0        0        0     1989 2023-04-23 19:43:53.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Streams.py
--rw-rw-rw-   0        0        0      860 2023-04-23 19:44:04.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Subscriptions.py
--rw-rw-rw-   0        0        0      820 2023-04-23 19:44:19.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Tags.py
--rw-rw-rw-   0        0        0      808 2023-04-23 19:44:31.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Teams.py
--rw-rw-rw-   0        0        0     3252 2023-04-30 15:25:37.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Users.py
--rw-rw-rw-   0        0        0     1835 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Utils.py
--rw-rw-rw-   0        0        0     2117 2023-05-06 14:01:27.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Videos.py
--rw-rw-rw-   0        0        0      628 2023-04-29 20:08:34.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/Whispers.py
--rw-rw-rw-   0        0        0      180 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/__imports.py
--rw-rw-rw-   0        0        0    14010 2023-05-28 22:17:32.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/Resources/__init__.py
--rw-rw-rw-   0        0        0    36055 2023-05-14 11:48:59.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/TwitchAPI.py
--rw-rw-rw-   0        0        0     1008 2023-04-30 22:42:20.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/_ApiRequest.py
--rw-rw-rw-   0        0        0      176 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.945624 Twitch_Edog0049a-0.0.35/src/Twitch/API/test/
--rw-rw-rw-   0        0        0      533 2023-02-19 15:59:48.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/test/Ads_test.py
--rw-rw-rw-   0        0        0     1557 2023-02-19 15:48:15.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/test/Bits_Test.py
--rw-rw-rw-   0        0        0      277 2023-02-19 16:03:36.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/test/Utils.py
--rw-rw-rw-   0        0        0        0 2023-02-19 14:23:38.000000 Twitch_Edog0049a-0.0.35/src/Twitch/API/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.956079 Twitch_Edog0049a-0.0.35/src/Twitch/ChatInterface/
--rw-rw-rw-   0        0        0       94 2023-03-26 15:46:11.000000 Twitch_Edog0049a-0.0.35/src/Twitch/ChatInterface/Exceptions.py
--rw-rw-rw-   0        0        0     4368 2023-04-08 23:17:22.000000 Twitch_Edog0049a-0.0.35/src/Twitch/ChatInterface/IrcController.py
--rw-rw-rw-   0        0        0    25655 2023-04-08 21:10:07.000000 Twitch_Edog0049a-0.0.35/src/Twitch/ChatInterface/MessageHandler.py
--rw-rw-rw-   0        0        0     1388 2023-03-11 21:23:16.000000 Twitch_Edog0049a-0.0.35/src/Twitch/ChatInterface/TokenBucket.py
--rw-rw-rw-   0        0        0    22973 2023-04-08 23:31:19.000000 Twitch_Edog0049a-0.0.35/src/Twitch/ChatInterface/TwitchChatInterface.py
--rw-rw-rw-   0        0        0      138 2023-04-23 19:47:57.000000 Twitch_Edog0049a-0.0.35/src/Twitch/ChatInterface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.961600 Twitch_Edog0049a-0.0.35/src/Twitch/EventHandler/
--rw-rw-rw-   0        0        0     7280 2023-04-08 17:39:27.000000 Twitch_Edog0049a-0.0.35/src/Twitch/EventHandler/EventHandler.py
--rw-rw-rw-   0        0        0       38 2023-04-08 23:59:13.000000 Twitch_Edog0049a-0.0.35/src/Twitch/EventHandler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.969072 Twitch_Edog0049a-0.0.35/src/Twitch/EventSub/
--rw-rw-rw-   0        0        0      136 2023-04-01 21:27:54.000000 Twitch_Edog0049a-0.0.35/src/Twitch/EventSub/EventSubConnector.py
--rw-rw-rw-   0        0        0       71 2023-04-09 00:14:32.000000 Twitch_Edog0049a-0.0.35/src/Twitch/EventSub/EventSubInterface.py
--rw-rw-rw-   0        0        0       48 2023-04-09 00:14:11.000000 Twitch_Edog0049a-0.0.35/src/Twitch/EventSub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.973987 Twitch_Edog0049a-0.0.35/src/Twitch/OAuth/
--rw-rw-rw-   0        0        0      573 2023-04-01 19:02:07.000000 Twitch_Edog0049a-0.0.35/src/Twitch/OAuth/Exceptions.py
--rw-rw-rw-   0        0        0     4044 2023-04-30 13:42:07.000000 Twitch_Edog0049a-0.0.35/src/Twitch/OAuth/Oauth.py
--rw-rw-rw-   0        0        0       88 2023-04-23 19:49:34.000000 Twitch_Edog0049a-0.0.35/src/Twitch/OAuth/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.975983 Twitch_Edog0049a-0.0.35/src/Twitch/OAuth/test/
--rw-rw-rw-   0        0        0     1544 2023-04-30 13:09:50.000000 Twitch_Edog0049a-0.0.35/src/Twitch/OAuth/test/oauthtest.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.982548 Twitch_Edog0049a-0.0.35/src/Twitch/PubSub/
--rw-rw-rw-   0        0        0      807 2023-04-08 14:06:35.000000 Twitch_Edog0049a-0.0.35/src/Twitch/PubSub/PubSubConnector.py
--rw-rw-rw-   0        0        0       32 2023-04-08 15:26:06.000000 Twitch_Edog0049a-0.0.35/src/Twitch/PubSub/PubSubInterface.py
--rw-rw-rw-   0        0        0       21 2023-04-08 15:31:25.000000 Twitch_Edog0049a-0.0.35/src/Twitch/PubSub/Topics.py
--rw-rw-rw-   0        0        0       91 2023-05-28 23:12:13.000000 Twitch_Edog0049a-0.0.35/src/Twitch/PubSub/__init__.py
--rw-rw-rw-   0        0        0    10296 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.35/src/Twitch/Scope.py
--rw-rw-rw-   0        0        0     1976 2023-05-21 13:26:58.000000 Twitch_Edog0049a-0.0.35/src/Twitch/SubscriptionTypes.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.986225 Twitch_Edog0049a-0.0.35/src/Twitch/WebsocketClient/
--rw-rw-rw-   0        0        0     3256 2023-05-13 12:45:46.000000 Twitch_Edog0049a-0.0.35/src/Twitch/WebsocketClient/WebsocketClient.py
--rw-rw-rw-   0        0        0       45 2023-04-08 14:38:11.000000 Twitch_Edog0049a-0.0.35/src/Twitch/WebsocketClient/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.990217 Twitch_Edog0049a-0.0.35/src/Twitch/WebsocketClient/tests/
--rw-rw-rw-   0        0        0        0 2023-03-26 19:28:11.000000 Twitch_Edog0049a-0.0.35/src/Twitch/WebsocketClient/tests/__init__.py
--rw-rw-rw-   0        0        0     4089 2023-04-02 20:14:05.000000 Twitch_Edog0049a-0.0.35/src/Twitch/WebsocketClient/tests/client_run_test.py
--rw-rw-rw-   0        0        0      313 2023-05-28 23:06:45.000000 Twitch_Edog0049a-0.0.35/src/Twitch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.990720 Twitch_Edog0049a-0.0.35/src/Twitch/secretkeys/
--rw-rw-rw-   0        0        0      189 2023-04-30 13:24:32.000000 Twitch_Edog0049a-0.0.35/src/Twitch/secretkeys/apikeys.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:45.998840 Twitch_Edog0049a-0.0.35/src/Twitch_Edog0049a.egg-info/
--rw-rw-rw-   0        0        0     1742 2023-05-28 23:16:45.000000 Twitch_Edog0049a-0.0.35/src/Twitch_Edog0049a.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-05-28 23:16:45.000000 Twitch_Edog0049a-0.0.35/src/Twitch_Edog0049a.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 23:16:45.000000 Twitch_Edog0049a-0.0.35/src/Twitch_Edog0049a.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 23:16:45.000000 Twitch_Edog0049a-0.0.35/src/Twitch_Edog0049a.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 23:16:46.000425 Twitch_Edog0049a-0.0.35/test/
--rw-rw-rw-   0        0        0     1003 2023-04-08 21:18:43.000000 Twitch_Edog0049a-0.0.35/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:29:47.797756 Twitch_Edog0049a-0.0.36/
+drwxrwxrwx   0        0        0        0 2023-05-28 23:29:47.778890 Twitch_Edog0049a-0.0.36/CallbackServer/
+-rw-rw-rw-   0        0        0     1657 2023-04-10 00:05:11.000000 Twitch_Edog0049a-0.0.36/CallbackServer/CallbackServer.py
+-rw-rw-rw-   0        0        0       58 2023-04-09 23:38:58.000000 Twitch_Edog0049a-0.0.36/CallbackServer/__init__.py
+-rw-rw-rw-   0        0        0     1079 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.36/LICENSE.txt
+-rw-rw-rw-   0        0        0     1742 2023-05-28 23:29:47.799263 Twitch_Edog0049a-0.0.36/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.36/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 23:29:47.787894 Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/
+-rw-rw-rw-   0        0        0     1742 2023-05-28 23:29:47.000000 Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-28 23:29:47.000000 Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:29:47.000000 Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-05-28 23:29:47.000000 Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       82 2023-05-28 21:47:57.000000 Twitch_Edog0049a-0.0.36/pyproject.toml
+-rw-rw-rw-   0        0        0      669 2023-05-28 23:29:47.800791 Twitch_Edog0049a-0.0.36/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 23:29:47.792770 Twitch_Edog0049a-0.0.36/test/
+-rw-rw-rw-   0        0        0        0 2023-04-08 16:14:59.000000 Twitch_Edog0049a-0.0.36/test/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-04-08 21:18:43.000000 Twitch_Edog0049a-0.0.36/test/test1.py
```

### Comparing `Twitch_Edog0049a-0.0.35/LICENSE.txt` & `Twitch_Edog0049a-0.0.36/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.35/PKG-INFO` & `Twitch_Edog0049a-0.0.36/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Twitch_Edog0049a
-Version: 0.0.35
+Version: 0.0.36
 Summary: Twitch library for chat, api, pubs, and eventsub
 Home-page: https://github.com/eli-reid/twitch
 Author: Eli Reid
 Author-email: EliR@Elireid.com
 Project-URL: Bug Tracker, https://github.com/eli-reid/twitch/-/issues
 Project-URL: repository, https://github.com/eli-reid/twitch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Twitch_Edog0049a-0.0.35/src/Twitch_Edog0049a.egg-info/PKG-INFO` & `Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Twitch-Edog0049a
-Version: 0.0.35
+Version: 0.0.36
 Summary: Twitch library for chat, api, pubs, and eventsub
 Home-page: https://github.com/eli-reid/twitch
 Author: Eli Reid
 Author-email: EliR@Elireid.com
 Project-URL: Bug Tracker, https://github.com/eli-reid/twitch/-/issues
 Project-URL: repository, https://github.com/eli-reid/twitch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Twitch_Edog0049a-0.0.35/test/test1.py` & `Twitch_Edog0049a-0.0.36/test/test1.py`

 * *Files identical despite different names*


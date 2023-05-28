# Comparing `tmp/Twitch_Edog0049a-0.0.33.tar.gz` & `tmp/Twitch_Edog0049a-0.0.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Twitch_Edog0049a-0.0.33.tar", last modified: Sun May 28 23:09:14 2023, max compression
+gzip compressed data, was "Twitch_Edog0049a-0.0.34.tar", last modified: Sun May 28 23:13:43 2023, max compression
```

## Comparing `Twitch_Edog0049a-0.0.33.tar` & `Twitch_Edog0049a-0.0.34.tar`

### file list

```diff
@@ -1,95 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.228627 Twitch_Edog0049a-0.0.33/
--rw-rw-rw-   0        0        0     1079 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.33/LICENSE.txt
--rw-rw-rw-   0        0        0     1742 2023-05-28 23:09:14.229633 Twitch_Edog0049a-0.0.33/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.33/README.md
--rw-rw-rw-   0        0        0       82 2023-05-28 21:47:57.000000 Twitch_Edog0049a-0.0.33/pyproject.toml
--rw-rw-rw-   0        0        0      675 2023-05-28 23:09:14.232623 Twitch_Edog0049a-0.0.33/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.090286 Twitch_Edog0049a-0.0.33/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.095791 Twitch_Edog0049a-0.0.33/src/Twitch/
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.103789 Twitch_Edog0049a-0.0.33/src/Twitch/API/
--rw-rw-rw-   0        0        0      355 2023-04-16 12:59:45.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.166700 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/
--rw-rw-rw-   0        0        0      714 2023-05-07 12:32:52.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Ads.py
--rw-rw-rw-   0        0        0     2651 2023-05-07 12:33:14.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Analytics.py
--rw-rw-rw-   0        0        0     3990 2023-05-06 20:34:56.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Bits.py
--rw-rw-rw-   0        0        0     8807 2023-05-07 12:29:11.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/ChannelPoints.py
--rw-rw-rw-   0        0        0     4628 2023-05-06 14:00:30.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Channels.py
--rw-rw-rw-   0        0        0     1762 2023-05-07 12:30:48.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Charity.py
--rw-rw-rw-   0        0        0    10043 2023-05-14 11:39:53.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Chat.py
--rw-rw-rw-   0        0        0     1907 2023-05-21 12:49:05.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Clips.py
--rw-rw-rw-   0        0        0      846 2023-04-23 19:40:21.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Entitlements.py
--rw-rw-rw-   0        0        0     1273 2023-04-23 19:41:04.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/EventSub.py
--rw-rw-rw-   0        0        0     4942 2023-04-23 19:40:49.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Extensions.py
--rw-rw-rw-   0        0        0      800 2023-04-23 19:41:21.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Games.py
--rw-rw-rw-   0        0        0      433 2023-04-23 19:41:40.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Goals.py
--rw-rw-rw-   0        0        0      439 2023-04-23 19:41:56.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/HypeTrain.py
--rw-rw-rw-   0        0        0     7481 2023-04-23 19:42:07.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Moderation.py
--rw-rw-rw-   0        0        0     1259 2023-04-23 19:43:41.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Music.py
--rw-rw-rw-   0        0        0     1171 2023-04-23 19:42:22.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Polls.py
--rw-rw-rw-   0        0        0     1207 2023-04-23 19:42:34.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Predictions.py
--rw-rw-rw-   0        0        0      806 2023-04-23 19:42:46.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Raids.py
--rw-rw-rw-   0        0        0     7229 2023-05-07 12:38:56.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/ResponseTypes.py
--rw-rw-rw-   0        0        0     2542 2023-04-23 19:43:14.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Schedule.py
--rw-rw-rw-   0        0        0      822 2023-04-23 19:43:27.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Search.py
--rw-rw-rw-   0        0        0     1989 2023-04-23 19:43:53.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Streams.py
--rw-rw-rw-   0        0        0      860 2023-04-23 19:44:04.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Subscriptions.py
--rw-rw-rw-   0        0        0      820 2023-04-23 19:44:19.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Tags.py
--rw-rw-rw-   0        0        0      808 2023-04-23 19:44:31.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Teams.py
--rw-rw-rw-   0        0        0     3252 2023-04-30 15:25:37.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Users.py
--rw-rw-rw-   0        0        0     1835 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Utils.py
--rw-rw-rw-   0        0        0     2117 2023-05-06 14:01:27.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Videos.py
--rw-rw-rw-   0        0        0      628 2023-04-29 20:08:34.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/Whispers.py
--rw-rw-rw-   0        0        0      180 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/__imports.py
--rw-rw-rw-   0        0        0    14010 2023-05-28 22:17:32.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/Resources/__init__.py
--rw-rw-rw-   0        0        0    36055 2023-05-14 11:48:59.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/TwitchAPI.py
--rw-rw-rw-   0        0        0     1008 2023-04-30 22:42:20.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/_ApiRequest.py
--rw-rw-rw-   0        0        0      176 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.173684 Twitch_Edog0049a-0.0.33/src/Twitch/API/test/
--rw-rw-rw-   0        0        0      533 2023-02-19 15:59:48.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/test/Ads_test.py
--rw-rw-rw-   0        0        0     1557 2023-02-19 15:48:15.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/test/Bits_Test.py
--rw-rw-rw-   0        0        0      277 2023-02-19 16:03:36.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/test/Utils.py
--rw-rw-rw-   0        0        0        0 2023-02-19 14:23:38.000000 Twitch_Edog0049a-0.0.33/src/Twitch/API/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.187992 Twitch_Edog0049a-0.0.33/src/Twitch/ChatInterface/
--rw-rw-rw-   0        0        0       94 2023-03-26 15:46:11.000000 Twitch_Edog0049a-0.0.33/src/Twitch/ChatInterface/Exceptions.py
--rw-rw-rw-   0        0        0     4368 2023-04-08 23:17:22.000000 Twitch_Edog0049a-0.0.33/src/Twitch/ChatInterface/IrcController.py
--rw-rw-rw-   0        0        0    25655 2023-04-08 21:10:07.000000 Twitch_Edog0049a-0.0.33/src/Twitch/ChatInterface/MessageHandler.py
--rw-rw-rw-   0        0        0     1388 2023-03-11 21:23:16.000000 Twitch_Edog0049a-0.0.33/src/Twitch/ChatInterface/TokenBucket.py
--rw-rw-rw-   0        0        0    22973 2023-04-08 23:31:19.000000 Twitch_Edog0049a-0.0.33/src/Twitch/ChatInterface/TwitchChatInterface.py
--rw-rw-rw-   0        0        0      138 2023-04-23 19:47:57.000000 Twitch_Edog0049a-0.0.33/src/Twitch/ChatInterface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.190983 Twitch_Edog0049a-0.0.33/src/Twitch/EventHandler/
--rw-rw-rw-   0        0        0     7280 2023-04-08 17:39:27.000000 Twitch_Edog0049a-0.0.33/src/Twitch/EventHandler/EventHandler.py
--rw-rw-rw-   0        0        0       38 2023-04-08 23:59:13.000000 Twitch_Edog0049a-0.0.33/src/Twitch/EventHandler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.196682 Twitch_Edog0049a-0.0.33/src/Twitch/EventSub/
--rw-rw-rw-   0        0        0      136 2023-04-01 21:27:54.000000 Twitch_Edog0049a-0.0.33/src/Twitch/EventSub/EventSubConnector.py
--rw-rw-rw-   0        0        0       71 2023-04-09 00:14:32.000000 Twitch_Edog0049a-0.0.33/src/Twitch/EventSub/EventSubInterface.py
--rw-rw-rw-   0        0        0       48 2023-04-09 00:14:11.000000 Twitch_Edog0049a-0.0.33/src/Twitch/EventSub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.202197 Twitch_Edog0049a-0.0.33/src/Twitch/OAuth/
--rw-rw-rw-   0        0        0      573 2023-04-01 19:02:07.000000 Twitch_Edog0049a-0.0.33/src/Twitch/OAuth/Exceptions.py
--rw-rw-rw-   0        0        0     4044 2023-04-30 13:42:07.000000 Twitch_Edog0049a-0.0.33/src/Twitch/OAuth/Oauth.py
--rw-rw-rw-   0        0        0       88 2023-04-23 19:49:34.000000 Twitch_Edog0049a-0.0.33/src/Twitch/OAuth/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.203204 Twitch_Edog0049a-0.0.33/src/Twitch/OAuth/test/
--rw-rw-rw-   0        0        0     1544 2023-04-30 13:09:50.000000 Twitch_Edog0049a-0.0.33/src/Twitch/OAuth/test/oauthtest.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.209714 Twitch_Edog0049a-0.0.33/src/Twitch/PubSub/
--rw-rw-rw-   0        0        0      807 2023-04-08 14:06:35.000000 Twitch_Edog0049a-0.0.33/src/Twitch/PubSub/PubSubConnector.py
--rw-rw-rw-   0        0        0       32 2023-04-08 15:26:06.000000 Twitch_Edog0049a-0.0.33/src/Twitch/PubSub/PubSubInterface.py
--rw-rw-rw-   0        0        0       21 2023-04-08 15:31:25.000000 Twitch_Edog0049a-0.0.33/src/Twitch/PubSub/Topics.py
--rw-rw-rw-   0        0        0       91 2023-04-08 17:07:40.000000 Twitch_Edog0049a-0.0.33/src/Twitch/PubSub/__init__.py
--rw-rw-rw-   0        0        0    10296 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.33/src/Twitch/Scope.py
--rw-rw-rw-   0        0        0     1976 2023-05-21 13:26:58.000000 Twitch_Edog0049a-0.0.33/src/Twitch/SubscriptionTypes.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.213703 Twitch_Edog0049a-0.0.33/src/Twitch/WebsocketClient/
--rw-rw-rw-   0        0        0     3256 2023-05-13 12:45:46.000000 Twitch_Edog0049a-0.0.33/src/Twitch/WebsocketClient/WebsocketClient.py
--rw-rw-rw-   0        0        0       45 2023-04-08 14:38:11.000000 Twitch_Edog0049a-0.0.33/src/Twitch/WebsocketClient/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.216208 Twitch_Edog0049a-0.0.33/src/Twitch/WebsocketClient/tests/
--rw-rw-rw-   0        0        0        0 2023-03-26 19:28:11.000000 Twitch_Edog0049a-0.0.33/src/Twitch/WebsocketClient/tests/__init__.py
--rw-rw-rw-   0        0        0     4089 2023-04-02 20:14:05.000000 Twitch_Edog0049a-0.0.33/src/Twitch/WebsocketClient/tests/client_run_test.py
--rw-rw-rw-   0        0        0      313 2023-05-28 23:06:45.000000 Twitch_Edog0049a-0.0.33/src/Twitch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.218429 Twitch_Edog0049a-0.0.33/src/Twitch/secretkeys/
--rw-rw-rw-   0        0        0      189 2023-04-30 13:24:32.000000 Twitch_Edog0049a-0.0.33/src/Twitch/secretkeys/apikeys.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.225916 Twitch_Edog0049a-0.0.33/src/Twitch_Edog0049a.egg-info/
--rw-rw-rw-   0        0        0     1742 2023-05-28 23:09:14.000000 Twitch_Edog0049a-0.0.33/src/Twitch_Edog0049a.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2637 2023-05-28 23:09:14.000000 Twitch_Edog0049a-0.0.33/src/Twitch_Edog0049a.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 23:09:14.000000 Twitch_Edog0049a-0.0.33/src/Twitch_Edog0049a.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-28 23:09:14.000000 Twitch_Edog0049a-0.0.33/src/Twitch_Edog0049a.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       72 2023-05-28 23:07:36.000000 Twitch_Edog0049a-0.0.33/src/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 23:09:14.226916 Twitch_Edog0049a-0.0.33/test/
--rw-rw-rw-   0        0        0     1003 2023-04-08 21:18:43.000000 Twitch_Edog0049a-0.0.33/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:13:43.344980 Twitch_Edog0049a-0.0.34/
+-rw-rw-rw-   0        0        0     1079 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.34/LICENSE.txt
+-rw-rw-rw-   0        0        0     1742 2023-05-28 23:13:43.344980 Twitch_Edog0049a-0.0.34/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.34/README.md
+-rw-rw-rw-   0        0        0       82 2023-05-28 21:47:57.000000 Twitch_Edog0049a-0.0.34/pyproject.toml
+-rw-rw-rw-   0        0        0      697 2023-05-28 23:13:43.345978 Twitch_Edog0049a-0.0.34/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 23:13:43.320753 Twitch_Edog0049a-0.0.34/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 23:13:43.334682 Twitch_Edog0049a-0.0.34/src/Twitch/
+-rw-rw-rw-   0        0        0    10296 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.34/src/Twitch/Scope.py
+-rw-rw-rw-   0        0        0     1976 2023-05-21 13:26:58.000000 Twitch_Edog0049a-0.0.34/src/Twitch/SubscriptionTypes.py
+-rw-rw-rw-   0        0        0      313 2023-05-28 23:06:45.000000 Twitch_Edog0049a-0.0.34/src/Twitch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 23:13:43.341995 Twitch_Edog0049a-0.0.34/src/Twitch_Edog0049a.egg-info/
+-rw-rw-rw-   0        0        0     1742 2023-05-28 23:13:43.000000 Twitch_Edog0049a-0.0.34/src/Twitch_Edog0049a.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      311 2023-05-28 23:13:43.000000 Twitch_Edog0049a-0.0.34/src/Twitch_Edog0049a.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 23:13:43.000000 Twitch_Edog0049a-0.0.34/src/Twitch_Edog0049a.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 23:13:43.000000 Twitch_Edog0049a-0.0.34/src/Twitch_Edog0049a.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 23:13:43.342986 Twitch_Edog0049a-0.0.34/test/
+-rw-rw-rw-   0        0        0     1003 2023-04-08 21:18:43.000000 Twitch_Edog0049a-0.0.34/test/test1.py
```

### Comparing `Twitch_Edog0049a-0.0.33/LICENSE.txt` & `Twitch_Edog0049a-0.0.34/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.33/PKG-INFO` & `Twitch_Edog0049a-0.0.34/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Twitch_Edog0049a
-Version: 0.0.33
+Version: 0.0.34
 Summary: Twitch library for chat, api, pubs, and eventsub
 Home-page: https://github.com/eli-reid/twitch
 Author: Eli Reid
 Author-email: EliR@Elireid.com
 Project-URL: Bug Tracker, https://github.com/eli-reid/twitch/-/issues
 Project-URL: repository, https://github.com/eli-reid/twitch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Twitch_Edog0049a-0.0.33/setup.cfg` & `Twitch_Edog0049a-0.0.34/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2054 7769 7463 685f 4564 6f67 3030   = Twitch_Edog00
 00000020: 3439 610d 0a76 6572 7369 6f6e 203d 2030  49a..version = 0
-00000030: 2e30 2e33 330d 0a61 7574 686f 7220 3d20  .0.33..author = 
+00000030: 2e30 2e33 340d 0a61 7574 686f 7220 3d20  .0.34..author = 
 00000040: 456c 6920 5265 6964 0d0a 6175 7468 6f72  Eli Reid..author
 00000050: 5f65 6d61 696c 203d 2045 6c69 5240 456c  _email = EliR@El
 00000060: 6972 6569 642e 636f 6d0d 0a64 6573 6372  ireid.com..descr
 00000070: 6970 7469 6f6e 203d 2054 7769 7463 6820  iption = Twitch 
 00000080: 6c69 6272 6172 7920 666f 7220 6368 6174  library for chat
 00000090: 2c20 6170 692c 2070 7562 732c 2061 6e64  , api, pubs, and
 000000a0: 2065 7665 6e74 7375 620d 0a6c 6f6e 675f   eventsub..long_
@@ -33,11 +33,12 @@
 00000200: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
 00000210: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
 00000220: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
 00000230: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
 00000240: 6e73 5d0d 0a70 6163 6b61 6765 5f64 6972  ns]..package_dir
 00000250: 203d 200d 0a09 3d20 7372 630d 0a70 7974   = ...= src..pyt
 00000260: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000270: 3d33 2e31 300d 0a0d 0a5b 6567 675f 696e  =3.10....[egg_in
-00000280: 666f 5d0d 0a74 6167 5f62 7569 6c64 203d  fo]..tag_build =
-00000290: 200d 0a74 6167 5f64 6174 6520 3d20 300d   ..tag_date = 0.
-000002a0: 0a0d 0a                                  ...
+00000270: 3d33 2e31 300d 0a70 6163 6b61 6765 7320  =3.10..packages 
+00000280: 3d20 0d0a 0954 7769 7463 680d 0a0d 0a5b  = ...Twitch....[
+00000290: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
+000002a0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
+000002b0: 6520 3d20 300d 0a0d 0a                   e = 0....
```

### Comparing `Twitch_Edog0049a-0.0.33/src/Twitch/Scope.py` & `Twitch_Edog0049a-0.0.34/src/Twitch/Scope.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.33/src/Twitch/SubscriptionTypes.py` & `Twitch_Edog0049a-0.0.34/src/Twitch/SubscriptionTypes.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.33/src/Twitch_Edog0049a.egg-info/PKG-INFO` & `Twitch_Edog0049a-0.0.34/src/Twitch_Edog0049a.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Twitch-Edog0049a
-Version: 0.0.33
+Version: 0.0.34
 Summary: Twitch library for chat, api, pubs, and eventsub
 Home-page: https://github.com/eli-reid/twitch
 Author: Eli Reid
 Author-email: EliR@Elireid.com
 Project-URL: Bug Tracker, https://github.com/eli-reid/twitch/-/issues
 Project-URL: repository, https://github.com/eli-reid/twitch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Twitch_Edog0049a-0.0.33/test/test1.py` & `Twitch_Edog0049a-0.0.34/test/test1.py`

 * *Files identical despite different names*


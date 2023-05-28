# Comparing `tmp/Twitch_Edog0049a-0.0.2.tar.gz` & `tmp/Twitch_Edog0049a-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Twitch_Edog0049a-0.0.2.tar", last modified: Sun May 28 22:08:02 2023, max compression
+gzip compressed data, was "Twitch_Edog0049a-0.0.3.tar", last modified: Sun May 28 22:23:19 2023, max compression
```

## Comparing `Twitch_Edog0049a-0.0.2.tar` & `Twitch_Edog0049a-0.0.3.tar`

### file list

```diff
@@ -1,94 +1,76 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.412976 Twitch_Edog0049a-0.0.2/
--rw-rw-rw-   0        0        0     1079 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1741 2023-05-28 22:08:02.412976 Twitch_Edog0049a-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.2/README.md
--rw-rw-rw-   0        0        0       82 2023-05-28 21:47:57.000000 Twitch_Edog0049a-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      714 2023-05-28 22:08:02.414971 Twitch_Edog0049a-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.270247 Twitch_Edog0049a-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.281733 Twitch_Edog0049a-0.0.2/src/Twitch/
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.290236 Twitch_Edog0049a-0.0.2/src/Twitch/API/
--rw-rw-rw-   0        0        0      355 2023-04-16 12:59:45.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.343788 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/
--rw-rw-rw-   0        0        0      714 2023-05-07 12:32:52.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Ads.py
--rw-rw-rw-   0        0        0     2651 2023-05-07 12:33:14.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Analytics.py
--rw-rw-rw-   0        0        0     3990 2023-05-06 20:34:56.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Bits.py
--rw-rw-rw-   0        0        0     8807 2023-05-07 12:29:11.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/ChannelPoints.py
--rw-rw-rw-   0        0        0     4628 2023-05-06 14:00:30.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Channels.py
--rw-rw-rw-   0        0        0     1762 2023-05-07 12:30:48.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Charity.py
--rw-rw-rw-   0        0        0    10043 2023-05-14 11:39:53.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Chat.py
--rw-rw-rw-   0        0        0     1907 2023-05-21 12:49:05.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Clips.py
--rw-rw-rw-   0        0        0      846 2023-04-23 19:40:21.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Entitlements.py
--rw-rw-rw-   0        0        0     1273 2023-04-23 19:41:04.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/EventSub.py
--rw-rw-rw-   0        0        0     4942 2023-04-23 19:40:49.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Extensions.py
--rw-rw-rw-   0        0        0      800 2023-04-23 19:41:21.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Games.py
--rw-rw-rw-   0        0        0      433 2023-04-23 19:41:40.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Goals.py
--rw-rw-rw-   0        0        0      439 2023-04-23 19:41:56.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/HypeTrain.py
--rw-rw-rw-   0        0        0     7481 2023-04-23 19:42:07.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Moderation.py
--rw-rw-rw-   0        0        0     1259 2023-04-23 19:43:41.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Music.py
--rw-rw-rw-   0        0        0     1171 2023-04-23 19:42:22.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Polls.py
--rw-rw-rw-   0        0        0     1207 2023-04-23 19:42:34.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Predictions.py
--rw-rw-rw-   0        0        0      806 2023-04-23 19:42:46.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Raids.py
--rw-rw-rw-   0        0        0     7229 2023-05-07 12:38:56.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/ResponseTypes.py
--rw-rw-rw-   0        0        0     2542 2023-04-23 19:43:14.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Schedule.py
--rw-rw-rw-   0        0        0      822 2023-04-23 19:43:27.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Search.py
--rw-rw-rw-   0        0        0     1989 2023-04-23 19:43:53.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Streams.py
--rw-rw-rw-   0        0        0      860 2023-04-23 19:44:04.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Subscriptions.py
--rw-rw-rw-   0        0        0      820 2023-04-23 19:44:19.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Tags.py
--rw-rw-rw-   0        0        0      808 2023-04-23 19:44:31.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Teams.py
--rw-rw-rw-   0        0        0     3252 2023-04-30 15:25:37.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Users.py
--rw-rw-rw-   0        0        0     1835 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Utils.py
--rw-rw-rw-   0        0        0     2117 2023-05-06 14:01:27.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Videos.py
--rw-rw-rw-   0        0        0      628 2023-04-29 20:08:34.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Whispers.py
--rw-rw-rw-   0        0        0      180 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/__imports.py
--rw-rw-rw-   0        0        0    14010 2023-04-30 13:11:45.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/__init__.py
--rw-rw-rw-   0        0        0    36055 2023-05-14 11:48:59.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/TwitchAPI.py
--rw-rw-rw-   0        0        0     1008 2023-04-30 22:42:20.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/_ApiRequest.py
--rw-rw-rw-   0        0        0      176 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.350551 Twitch_Edog0049a-0.0.2/src/Twitch/API/test/
--rw-rw-rw-   0        0        0      533 2023-02-19 15:59:48.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/test/Ads_test.py
--rw-rw-rw-   0        0        0     1557 2023-02-19 15:48:15.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/test/Bits_Test.py
--rw-rw-rw-   0        0        0      277 2023-02-19 16:03:36.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/test/Utils.py
--rw-rw-rw-   0        0        0        0 2023-02-19 14:23:38.000000 Twitch_Edog0049a-0.0.2/src/Twitch/API/test/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.361108 Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/
--rw-rw-rw-   0        0        0       94 2023-03-26 15:46:11.000000 Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/Exceptions.py
--rw-rw-rw-   0        0        0     4368 2023-04-08 23:17:22.000000 Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/IrcController.py
--rw-rw-rw-   0        0        0    25655 2023-04-08 21:10:07.000000 Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/MessageHandler.py
--rw-rw-rw-   0        0        0     1388 2023-03-11 21:23:16.000000 Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/TokenBucket.py
--rw-rw-rw-   0        0        0    22973 2023-04-08 23:31:19.000000 Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/TwitchChatInterface.py
--rw-rw-rw-   0        0        0      138 2023-04-23 19:47:57.000000 Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.365105 Twitch_Edog0049a-0.0.2/src/Twitch/EventHandler/
--rw-rw-rw-   0        0        0     7280 2023-04-08 17:39:27.000000 Twitch_Edog0049a-0.0.2/src/Twitch/EventHandler/EventHandler.py
--rw-rw-rw-   0        0        0       38 2023-04-08 23:59:13.000000 Twitch_Edog0049a-0.0.2/src/Twitch/EventHandler/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.369087 Twitch_Edog0049a-0.0.2/src/Twitch/EventSub/
--rw-rw-rw-   0        0        0      136 2023-04-01 21:27:54.000000 Twitch_Edog0049a-0.0.2/src/Twitch/EventSub/EventSubConnector.py
--rw-rw-rw-   0        0        0       71 2023-04-09 00:14:32.000000 Twitch_Edog0049a-0.0.2/src/Twitch/EventSub/EventSubInterface.py
--rw-rw-rw-   0        0        0       48 2023-04-09 00:14:11.000000 Twitch_Edog0049a-0.0.2/src/Twitch/EventSub/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.374781 Twitch_Edog0049a-0.0.2/src/Twitch/OAuth/
--rw-rw-rw-   0        0        0      573 2023-04-01 19:02:07.000000 Twitch_Edog0049a-0.0.2/src/Twitch/OAuth/Exceptions.py
--rw-rw-rw-   0        0        0     4044 2023-04-30 13:42:07.000000 Twitch_Edog0049a-0.0.2/src/Twitch/OAuth/Oauth.py
--rw-rw-rw-   0        0        0       88 2023-04-23 19:49:34.000000 Twitch_Edog0049a-0.0.2/src/Twitch/OAuth/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.379300 Twitch_Edog0049a-0.0.2/src/Twitch/OAuth/test/
--rw-rw-rw-   0        0        0     1544 2023-04-30 13:09:50.000000 Twitch_Edog0049a-0.0.2/src/Twitch/OAuth/test/oauthtest.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.395475 Twitch_Edog0049a-0.0.2/src/Twitch/PubSub/
--rw-rw-rw-   0        0        0      807 2023-04-08 14:06:35.000000 Twitch_Edog0049a-0.0.2/src/Twitch/PubSub/PubSubConnector.py
--rw-rw-rw-   0        0        0       32 2023-04-08 15:26:06.000000 Twitch_Edog0049a-0.0.2/src/Twitch/PubSub/PubSubInterface.py
--rw-rw-rw-   0        0        0       21 2023-04-08 15:31:25.000000 Twitch_Edog0049a-0.0.2/src/Twitch/PubSub/Topics.py
--rw-rw-rw-   0        0        0       91 2023-04-08 17:07:40.000000 Twitch_Edog0049a-0.0.2/src/Twitch/PubSub/__init__.py
--rw-rw-rw-   0        0        0    10296 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.2/src/Twitch/Scope.py
--rw-rw-rw-   0        0        0     1976 2023-05-21 13:26:58.000000 Twitch_Edog0049a-0.0.2/src/Twitch/SubscriptionTypes.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.398970 Twitch_Edog0049a-0.0.2/src/Twitch/WebsocketClient/
--rw-rw-rw-   0        0        0     3256 2023-05-13 12:45:46.000000 Twitch_Edog0049a-0.0.2/src/Twitch/WebsocketClient/WebsocketClient.py
--rw-rw-rw-   0        0        0       45 2023-04-08 14:38:11.000000 Twitch_Edog0049a-0.0.2/src/Twitch/WebsocketClient/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.402033 Twitch_Edog0049a-0.0.2/src/Twitch/WebsocketClient/tests/
--rw-rw-rw-   0        0        0        0 2023-03-26 19:28:11.000000 Twitch_Edog0049a-0.0.2/src/Twitch/WebsocketClient/tests/__init__.py
--rw-rw-rw-   0        0        0     4089 2023-04-02 20:14:05.000000 Twitch_Edog0049a-0.0.2/src/Twitch/WebsocketClient/tests/client_run_test.py
--rw-rw-rw-   0        0        0      313 2023-04-30 13:08:44.000000 Twitch_Edog0049a-0.0.2/src/Twitch/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.403031 Twitch_Edog0049a-0.0.2/src/Twitch/secretkeys/
--rw-rw-rw-   0        0        0      189 2023-04-30 13:24:32.000000 Twitch_Edog0049a-0.0.2/src/Twitch/secretkeys/apikeys.py
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.409913 Twitch_Edog0049a-0.0.2/src/Twitch_Edog0049a.egg-info/
--rw-rw-rw-   0        0        0     1741 2023-05-28 22:08:02.000000 Twitch_Edog0049a-0.0.2/src/Twitch_Edog0049a.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-05-28 22:08:02.000000 Twitch_Edog0049a-0.0.2/src/Twitch_Edog0049a.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 22:08:02.000000 Twitch_Edog0049a-0.0.2/src/Twitch_Edog0049a.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-28 22:08:02.000000 Twitch_Edog0049a-0.0.2/src/Twitch_Edog0049a.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-28 22:08:02.410979 Twitch_Edog0049a-0.0.2/test/
--rw-rw-rw-   0        0        0     1003 2023-04-08 21:18:43.000000 Twitch_Edog0049a-0.0.2/test/test1.py
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.840377 Twitch_Edog0049a-0.0.3/
+-rw-rw-rw-   0        0        0     1079 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1741 2023-05-28 22:23:19.840377 Twitch_Edog0049a-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.3/README.md
+-rw-rw-rw-   0        0        0       82 2023-05-28 21:47:57.000000 Twitch_Edog0049a-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      844 2023-05-28 22:23:19.842372 Twitch_Edog0049a-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.718448 Twitch_Edog0049a-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.731531 Twitch_Edog0049a-0.0.3/src/Twitch/
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.739105 Twitch_Edog0049a-0.0.3/src/Twitch/API/
+-rw-rw-rw-   0        0        0      355 2023-04-16 12:59:45.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.798485 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/
+-rw-rw-rw-   0        0        0      714 2023-05-07 12:32:52.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Ads.py
+-rw-rw-rw-   0        0        0     2651 2023-05-07 12:33:14.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Analytics.py
+-rw-rw-rw-   0        0        0     3990 2023-05-06 20:34:56.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Bits.py
+-rw-rw-rw-   0        0        0     8807 2023-05-07 12:29:11.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/ChannelPoints.py
+-rw-rw-rw-   0        0        0     4628 2023-05-06 14:00:30.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Channels.py
+-rw-rw-rw-   0        0        0     1762 2023-05-07 12:30:48.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Charity.py
+-rw-rw-rw-   0        0        0    10043 2023-05-14 11:39:53.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Chat.py
+-rw-rw-rw-   0        0        0     1907 2023-05-21 12:49:05.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Clips.py
+-rw-rw-rw-   0        0        0      846 2023-04-23 19:40:21.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Entitlements.py
+-rw-rw-rw-   0        0        0     1273 2023-04-23 19:41:04.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/EventSub.py
+-rw-rw-rw-   0        0        0     4942 2023-04-23 19:40:49.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Extensions.py
+-rw-rw-rw-   0        0        0      800 2023-04-23 19:41:21.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Games.py
+-rw-rw-rw-   0        0        0      433 2023-04-23 19:41:40.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Goals.py
+-rw-rw-rw-   0        0        0      439 2023-04-23 19:41:56.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/HypeTrain.py
+-rw-rw-rw-   0        0        0     7481 2023-04-23 19:42:07.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Moderation.py
+-rw-rw-rw-   0        0        0     1259 2023-04-23 19:43:41.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Music.py
+-rw-rw-rw-   0        0        0     1171 2023-04-23 19:42:22.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Polls.py
+-rw-rw-rw-   0        0        0     1207 2023-04-23 19:42:34.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Predictions.py
+-rw-rw-rw-   0        0        0      806 2023-04-23 19:42:46.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Raids.py
+-rw-rw-rw-   0        0        0     7229 2023-05-07 12:38:56.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/ResponseTypes.py
+-rw-rw-rw-   0        0        0     2542 2023-04-23 19:43:14.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Schedule.py
+-rw-rw-rw-   0        0        0      822 2023-04-23 19:43:27.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Search.py
+-rw-rw-rw-   0        0        0     1989 2023-04-23 19:43:53.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Streams.py
+-rw-rw-rw-   0        0        0      860 2023-04-23 19:44:04.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Subscriptions.py
+-rw-rw-rw-   0        0        0      820 2023-04-23 19:44:19.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Tags.py
+-rw-rw-rw-   0        0        0      808 2023-04-23 19:44:31.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Teams.py
+-rw-rw-rw-   0        0        0     3252 2023-04-30 15:25:37.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Users.py
+-rw-rw-rw-   0        0        0     1835 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Utils.py
+-rw-rw-rw-   0        0        0     2117 2023-05-06 14:01:27.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Videos.py
+-rw-rw-rw-   0        0        0      628 2023-04-29 20:08:34.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Whispers.py
+-rw-rw-rw-   0        0        0      180 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/__imports.py
+-rw-rw-rw-   0        0        0    14010 2023-05-28 22:17:32.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/__init__.py
+-rw-rw-rw-   0        0        0    36055 2023-05-14 11:48:59.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/TwitchAPI.py
+-rw-rw-rw-   0        0        0     1008 2023-04-30 22:42:20.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/_ApiRequest.py
+-rw-rw-rw-   0        0        0      176 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.3/src/Twitch/API/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.811477 Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/
+-rw-rw-rw-   0        0        0       94 2023-03-26 15:46:11.000000 Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/Exceptions.py
+-rw-rw-rw-   0        0        0     4368 2023-04-08 23:17:22.000000 Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/IrcController.py
+-rw-rw-rw-   0        0        0    25655 2023-04-08 21:10:07.000000 Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/MessageHandler.py
+-rw-rw-rw-   0        0        0     1388 2023-03-11 21:23:16.000000 Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/TokenBucket.py
+-rw-rw-rw-   0        0        0    22973 2023-04-08 23:31:19.000000 Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/TwitchChatInterface.py
+-rw-rw-rw-   0        0        0      138 2023-04-23 19:47:57.000000 Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.817461 Twitch_Edog0049a-0.0.3/src/Twitch/EventSub/
+-rw-rw-rw-   0        0        0      136 2023-04-01 21:27:54.000000 Twitch_Edog0049a-0.0.3/src/Twitch/EventSub/EventSubConnector.py
+-rw-rw-rw-   0        0        0       71 2023-04-09 00:14:32.000000 Twitch_Edog0049a-0.0.3/src/Twitch/EventSub/EventSubInterface.py
+-rw-rw-rw-   0        0        0       48 2023-04-09 00:14:11.000000 Twitch_Edog0049a-0.0.3/src/Twitch/EventSub/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.823512 Twitch_Edog0049a-0.0.3/src/Twitch/OAuth/
+-rw-rw-rw-   0        0        0      573 2023-04-01 19:02:07.000000 Twitch_Edog0049a-0.0.3/src/Twitch/OAuth/Exceptions.py
+-rw-rw-rw-   0        0        0     4044 2023-04-30 13:42:07.000000 Twitch_Edog0049a-0.0.3/src/Twitch/OAuth/Oauth.py
+-rw-rw-rw-   0        0        0       88 2023-04-23 19:49:34.000000 Twitch_Edog0049a-0.0.3/src/Twitch/OAuth/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.830000 Twitch_Edog0049a-0.0.3/src/Twitch/PubSub/
+-rw-rw-rw-   0        0        0      807 2023-04-08 14:06:35.000000 Twitch_Edog0049a-0.0.3/src/Twitch/PubSub/PubSubConnector.py
+-rw-rw-rw-   0        0        0       32 2023-04-08 15:26:06.000000 Twitch_Edog0049a-0.0.3/src/Twitch/PubSub/PubSubInterface.py
+-rw-rw-rw-   0        0        0       21 2023-04-08 15:31:25.000000 Twitch_Edog0049a-0.0.3/src/Twitch/PubSub/Topics.py
+-rw-rw-rw-   0        0        0       91 2023-04-08 17:07:40.000000 Twitch_Edog0049a-0.0.3/src/Twitch/PubSub/__init__.py
+-rw-rw-rw-   0        0        0    10296 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.3/src/Twitch/Scope.py
+-rw-rw-rw-   0        0        0     1976 2023-05-21 13:26:58.000000 Twitch_Edog0049a-0.0.3/src/Twitch/SubscriptionTypes.py
+-rw-rw-rw-   0        0        0      313 2023-04-30 13:08:44.000000 Twitch_Edog0049a-0.0.3/src/Twitch/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.837335 Twitch_Edog0049a-0.0.3/src/Twitch_Edog0049a.egg-info/
+-rw-rw-rw-   0        0        0     1741 2023-05-28 22:23:19.000000 Twitch_Edog0049a-0.0.3/src/Twitch_Edog0049a.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2169 2023-05-28 22:23:19.000000 Twitch_Edog0049a-0.0.3/src/Twitch_Edog0049a.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 22:23:19.000000 Twitch_Edog0049a-0.0.3/src/Twitch_Edog0049a.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 22:23:19.000000 Twitch_Edog0049a-0.0.3/src/Twitch_Edog0049a.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 22:23:19.838334 Twitch_Edog0049a-0.0.3/test/
+-rw-rw-rw-   0        0        0     1003 2023-04-08 21:18:43.000000 Twitch_Edog0049a-0.0.3/test/test1.py
```

### Comparing `Twitch_Edog0049a-0.0.2/LICENSE.txt` & `Twitch_Edog0049a-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/PKG-INFO` & `Twitch_Edog0049a-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Twitch_Edog0049a
-Version: 0.0.2
+Version: 0.0.3
 Summary: Twitch library for chat, api, pubs, and eventsub
 Home-page: https://github.com/eli-reid/twitch
 Author: Eli Reid
 Author-email: EliR@Elireid.com
 Project-URL: Bug Tracker, https://github.com/eli-reid/twitch/-/issues
 Project-URL: repository, https://github.com/eli-reid/twitch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Ads.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Ads.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Analytics.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Analytics.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Bits.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Bits.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/ChannelPoints.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/ChannelPoints.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Channels.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Channels.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Charity.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Charity.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Chat.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Chat.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Clips.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Clips.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Entitlements.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Entitlements.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/EventSub.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/EventSub.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Extensions.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Extensions.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Games.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Games.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Moderation.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Moderation.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Music.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Music.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Polls.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Polls.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Predictions.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Predictions.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Raids.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Raids.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/ResponseTypes.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/ResponseTypes.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Schedule.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Schedule.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Search.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Search.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Streams.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Streams.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Subscriptions.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Subscriptions.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Tags.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Tags.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Teams.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Teams.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Users.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Users.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Utils.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Utils.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Videos.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Videos.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/Whispers.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/Whispers.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/Resources/__init__.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/Resources/__init__.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/TwitchAPI.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/TwitchAPI.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/API/_ApiRequest.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/API/_ApiRequest.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/IrcController.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/IrcController.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/MessageHandler.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/MessageHandler.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/TokenBucket.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/TokenBucket.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/ChatInterface/TwitchChatInterface.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/ChatInterface/TwitchChatInterface.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/OAuth/Exceptions.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/OAuth/Exceptions.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/OAuth/Oauth.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/OAuth/Oauth.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/PubSub/PubSubConnector.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/PubSub/PubSubConnector.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/Scope.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/Scope.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch/SubscriptionTypes.py` & `Twitch_Edog0049a-0.0.3/src/Twitch/SubscriptionTypes.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch_Edog0049a.egg-info/PKG-INFO` & `Twitch_Edog0049a-0.0.3/src/Twitch_Edog0049a.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Twitch-Edog0049a
-Version: 0.0.2
+Version: 0.0.3
 Summary: Twitch library for chat, api, pubs, and eventsub
 Home-page: https://github.com/eli-reid/twitch
 Author: Eli Reid
 Author-email: EliR@Elireid.com
 Project-URL: Bug Tracker, https://github.com/eli-reid/twitch/-/issues
 Project-URL: repository, https://github.com/eli-reid/twitch
 Classifier: Programming Language :: Python :: 3
```

### Comparing `Twitch_Edog0049a-0.0.2/src/Twitch_Edog0049a.egg-info/SOURCES.txt` & `Twitch_Edog0049a-0.0.3/src/Twitch_Edog0049a.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -37,40 +37,28 @@
 src/Twitch/API/Resources/Teams.py
 src/Twitch/API/Resources/Users.py
 src/Twitch/API/Resources/Utils.py
 src/Twitch/API/Resources/Videos.py
 src/Twitch/API/Resources/Whispers.py
 src/Twitch/API/Resources/__imports.py
 src/Twitch/API/Resources/__init__.py
-src/Twitch/API/test/Ads_test.py
-src/Twitch/API/test/Bits_Test.py
-src/Twitch/API/test/Utils.py
-src/Twitch/API/test/__init__.py
 src/Twitch/ChatInterface/Exceptions.py
 src/Twitch/ChatInterface/IrcController.py
 src/Twitch/ChatInterface/MessageHandler.py
 src/Twitch/ChatInterface/TokenBucket.py
 src/Twitch/ChatInterface/TwitchChatInterface.py
 src/Twitch/ChatInterface/__init__.py
-src/Twitch/EventHandler/EventHandler.py
-src/Twitch/EventHandler/__init__.py
 src/Twitch/EventSub/EventSubConnector.py
 src/Twitch/EventSub/EventSubInterface.py
 src/Twitch/EventSub/__init__.py
 src/Twitch/OAuth/Exceptions.py
 src/Twitch/OAuth/Oauth.py
 src/Twitch/OAuth/__init__.py
-src/Twitch/OAuth/test/oauthtest.py
 src/Twitch/PubSub/PubSubConnector.py
 src/Twitch/PubSub/PubSubInterface.py
 src/Twitch/PubSub/Topics.py
 src/Twitch/PubSub/__init__.py
-src/Twitch/WebsocketClient/WebsocketClient.py
-src/Twitch/WebsocketClient/__init__.py
-src/Twitch/WebsocketClient/tests/__init__.py
-src/Twitch/WebsocketClient/tests/client_run_test.py
-src/Twitch/secretkeys/apikeys.py
 src/Twitch_Edog0049a.egg-info/PKG-INFO
 src/Twitch_Edog0049a.egg-info/SOURCES.txt
 src/Twitch_Edog0049a.egg-info/dependency_links.txt
 src/Twitch_Edog0049a.egg-info/top_level.txt
 test/test1.py
```

### Comparing `Twitch_Edog0049a-0.0.2/test/test1.py` & `Twitch_Edog0049a-0.0.3/test/test1.py`

 * *Files identical despite different names*


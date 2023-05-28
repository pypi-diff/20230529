# Comparing `tmp/Twitch_Edog0049a-0.0.36.tar.gz` & `tmp/twitch_edog0049a-0.0.37.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Twitch_Edog0049a-0.0.36.tar", last modified: Sun May 28 23:29:47 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `Twitch_Edog0049a-0.0.36.tar` & `twitch_edog0049a-0.0.37.tar`

### file list

```diff
@@ -1,17 +1,79 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 23:29:47.797756 Twitch_Edog0049a-0.0.36/
-drwxrwxrwx   0        0        0        0 2023-05-28 23:29:47.778890 Twitch_Edog0049a-0.0.36/CallbackServer/
--rw-rw-rw-   0        0        0     1657 2023-04-10 00:05:11.000000 Twitch_Edog0049a-0.0.36/CallbackServer/CallbackServer.py
--rw-rw-rw-   0        0        0       58 2023-04-09 23:38:58.000000 Twitch_Edog0049a-0.0.36/CallbackServer/__init__.py
--rw-rw-rw-   0        0        0     1079 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.36/LICENSE.txt
--rw-rw-rw-   0        0        0     1742 2023-05-28 23:29:47.799263 Twitch_Edog0049a-0.0.36/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-28 17:07:49.000000 Twitch_Edog0049a-0.0.36/README.md
-drwxrwxrwx   0        0        0        0 2023-05-28 23:29:47.787894 Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/
--rw-rw-rw-   0        0        0     1742 2023-05-28 23:29:47.000000 Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-05-28 23:29:47.000000 Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 23:29:47.000000 Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-05-28 23:29:47.000000 Twitch_Edog0049a-0.0.36/Twitch_Edog0049a.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       82 2023-05-28 21:47:57.000000 Twitch_Edog0049a-0.0.36/pyproject.toml
--rw-rw-rw-   0        0        0      669 2023-05-28 23:29:47.800791 Twitch_Edog0049a-0.0.36/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-28 23:29:47.792770 Twitch_Edog0049a-0.0.36/test/
--rw-rw-rw-   0        0        0        0 2023-04-08 16:14:59.000000 Twitch_Edog0049a-0.0.36/test/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-04-08 21:18:43.000000 Twitch_Edog0049a-0.0.36/test/test1.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/Twitch.code-workspace
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/dddd.cfgd
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/CallbackServer/CallbackServer.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/CallbackServer/__init__.py
+-rw-r--r--   0        0        0    10296 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/Scope.py
+-rw-r--r--   0        0        0     1976 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/SubscriptionTypes.py
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/__init__.py
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Exceptions.py
+-rw-r--r--   0        0        0    36055 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/TwitchAPI.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/_ApiRequest.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/__init__.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/api flow.svg
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Ads.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Analytics.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Bits.py
+-rw-r--r--   0        0        0     8807 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/ChannelPoints.py
+-rw-r--r--   0        0        0     4628 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Channels.py
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Charity.py
+-rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Chat.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Clips.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Entitlements.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/EventSub.py
+-rw-r--r--   0        0        0     4942 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Extensions.py
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Games.py
+-rw-r--r--   0        0        0      433 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Goals.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/HypeTrain.py
+-rw-r--r--   0        0        0     7481 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Moderation.py
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Music.py
+-rw-r--r--   0        0        0     1171 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Polls.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Predictions.py
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Raids.py
+-rw-r--r--   0        0        0     7229 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/ResponseTypes.py
+-rw-r--r--   0        0        0     2542 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Schedule.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Search.py
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Streams.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Subscriptions.py
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Tags.py
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Teams.py
+-rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Users.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Utils.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Videos.py
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/Whispers.py
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/__imports.py
+-rw-r--r--   0        0        0    14010 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/Resources/__init__.py
+-rw-r--r--   0        0        0      533 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/test/Ads_test.py
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/test/Bits_Test.py
+-rw-r--r--   0        0        0      277 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/test/Utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/API/test/__init__.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/Exceptions.py
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/IrcController.py
+-rw-r--r--   0        0        0    25655 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/MessageHandler.py
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/TokenBucket.py
+-rw-r--r--   0        0        0    22973 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/TwitchChatInterface.py
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/ChatInterface/__init__.py
+-rw-r--r--   0        0        0     7280 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/EventHandler/EventHandler.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/EventHandler/__init__.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/EventSub/EventSubConnector.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/EventSub/EventSubInterface.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/EventSub/__init__.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/OAuth/Exceptions.py
+-rw-r--r--   0        0        0    39494 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/OAuth/Oauth flow.svg
+-rw-r--r--   0        0        0     4044 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/OAuth/Oauth.py
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/OAuth/__init__.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/OAuth/test/oauthtest.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/PubSub/PubSubConnector.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/PubSub/PubSubInterface.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/PubSub/Topics.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/PubSub/__init__.py
+-rw-r--r--   0        0        0     3256 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/WebsocketClient/WebsocketClient.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/WebsocketClient/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/WebsocketClient/tests/__init__.py
+-rw-r--r--   0        0        0     4089 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/src/Twitch/WebsocketClient/tests/client_run_test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/test/__init__.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/test/test1.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/.gitignore
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/LICENSE.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/README.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/pyproject.toml
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 twitch_edog0049a-0.0.37/PKG-INFO
```

### Comparing `Twitch_Edog0049a-0.0.36/CallbackServer/CallbackServer.py` & `twitch_edog0049a-0.0.37/CallbackServer/CallbackServer.py`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.36/LICENSE.txt` & `twitch_edog0049a-0.0.37/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Twitch_Edog0049a-0.0.36/setup.cfg` & `twitch_edog0049a-0.0.37/dddd.cfgd`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,40 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2054 7769 7463 685f 4564 6f67 3030   = Twitch_Edog00
 00000020: 3439 610d 0a76 6572 7369 6f6e 203d 2030  49a..version = 0
 00000030: 2e30 2e33 360d 0a61 7574 686f 7220 3d20  .0.36..author = 
 00000040: 456c 6920 5265 6964 0d0a 6175 7468 6f72  Eli Reid..author
-00000050: 5f65 6d61 696c 203d 2045 6c69 5240 456c  _email = EliR@El
-00000060: 6972 6569 642e 636f 6d0d 0a64 6573 6372  ireid.com..descr
-00000070: 6970 7469 6f6e 203d 2054 7769 7463 6820  iption = Twitch 
-00000080: 6c69 6272 6172 7920 666f 7220 6368 6174  library for chat
-00000090: 2c20 6170 692c 2070 7562 732c 2061 6e64  , api, pubs, and
-000000a0: 2065 7665 6e74 7375 620d 0a6c 6f6e 675f   eventsub..long_
-000000b0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-000000c0: 6c65 3a20 5245 4144 4d45 2e6d 642c 204c  le: README.md, L
-000000d0: 4943 454e 5345 2e74 7874 0d0a 6c6f 6e67  ICENSE.txt..long
-000000e0: 5f64 6573 6372 6970 7469 6f6e 5f63 6f6e  _description_con
-000000f0: 7465 6e74 5f74 7970 6520 3d20 7465 7874  tent_type = text
-00000100: 2f6d 6172 6b64 6f77 6e0d 0a75 726c 203d  /markdown..url =
-00000110: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-00000120: 636f 6d2f 656c 692d 7265 6964 2f74 7769  com/eli-reid/twi
-00000130: 7463 680d 0a70 726f 6a65 6374 5f75 726c  tch..project_url
-00000140: 7320 3d20 0d0a 0942 7567 2054 7261 636b  s = ...Bug Track
-00000150: 6572 203d 2068 7474 7073 3a2f 2f67 6974  er = https://git
-00000160: 6875 622e 636f 6d2f 656c 692d 7265 6964  hub.com/eli-reid
-00000170: 2f74 7769 7463 682f 2d2f 6973 7375 6573  /twitch/-/issues
-00000180: 0d0a 0972 6570 6f73 6974 6f72 7920 3d20  ...repository = 
-00000190: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000001a0: 6f6d 2f65 6c69 2d72 6569 642f 7477 6974  om/eli-reid/twit
-000001b0: 6368 0d0a 636c 6173 7369 6669 6572 7320  ch..classifiers 
-000001c0: 3d20 0d0a 0950 726f 6772 616d 6d69 6e67  = ...Programming
-000001d0: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
-000001e0: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
-000001f0: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
-00000200: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
-00000210: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
-00000220: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-00000230: 656e 6465 6e74 0d0a 0d0a 5b6f 7074 696f  endent....[optio
-00000240: 6e73 5d0d 0a70 7974 686f 6e5f 7265 7175  ns]..python_requ
-00000250: 6972 6573 203d 203e 3d33 2e31 300d 0a70  ires = >=3.10..p
-00000260: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000270: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000280: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-00000290: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000050: 5f65 6d61 696c 203d 2020 456c 6952 4045  _email =  EliR@E
+00000060: 6c69 7265 6964 2e63 6f6d 0d0a 6465 7363  lireid.com..desc
+00000070: 7269 7074 696f 6e20 3d20 5477 6974 6368  ription = Twitch
+00000080: 206c 6962 7261 7279 2066 6f72 2063 6861   library for cha
+00000090: 742c 2061 7069 2c20 7075 6273 2c20 616e  t, api, pubs, an
+000000a0: 6420 6576 656e 7473 7562 0d0a 6c6f 6e67  d eventsub..long
+000000b0: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
+000000c0: 696c 653a 2052 4541 444d 452e 6d64 2c20  ile: README.md, 
+000000d0: 4c49 4345 4e53 452e 7478 740d 0a6c 6f6e  LICENSE.txt..lon
+000000e0: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
+000000f0: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
+00000100: 742f 6d61 726b 646f 776e 0d0a 7572 6c20  t/markdown..url 
+00000110: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
+00000120: 2e63 6f6d 2f65 6c69 2d72 6569 642f 7477  .com/eli-reid/tw
+00000130: 6974 6368 0d0a 7072 6f6a 6563 745f 7572  itch..project_ur
+00000140: 6c73 203d 0d0a 2020 2020 4275 6720 5472  ls =..    Bug Tr
+00000150: 6163 6b65 7220 3d20 6874 7470 733a 2f2f  acker = https://
+00000160: 6769 7468 7562 2e63 6f6d 2f65 6c69 2d72  github.com/eli-r
+00000170: 6569 642f 7477 6974 6368 2f2d 2f69 7373  eid/twitch/-/iss
+00000180: 7565 730d 0a20 2020 2072 6570 6f73 6974  ues..    reposit
+00000190: 6f72 7920 3d20 6874 7470 733a 2f2f 6769  ory = https://gi
+000001a0: 7468 7562 2e63 6f6d 2f65 6c69 2d72 6569  thub.com/eli-rei
+000001b0: 642f 7477 6974 6368 0d0a 636c 6173 7369  d/twitch..classi
+000001c0: 6669 6572 7320 3d0d 0a20 2020 2050 726f  fiers =..    Pro
+000001d0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
+000001e0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
+000001f0: 0d0a 2020 2020 4c69 6365 6e73 6520 3a3a  ..    License ::
+00000200: 204f 5349 2041 7070 726f 7665 6420 3a3a   OSI Approved ::
+00000210: 204d 4954 204c 6963 656e 7365 0d0a 2020   MIT License..  
+00000220: 2020 4f70 6572 6174 696e 6720 5379 7374    Operating Syst
+00000230: 656d 203a 3a20 4f53 2049 6e64 6570 656e  em :: OS Indepen
+00000240: 6465 6e74 0d0a 0d0a 5b6f 7074 696f 6e73  dent....[options
+00000250: 5d0d 0a70 7974 686f 6e5f 7265 7175 6972  ]..python_requir
+00000260: 6573 203d 203e 3d33 2e31 300d 0a0d 0a70  es = >=3.10....p
+00000270: 6163 6b61 6765 7320 3d20 6669 6e64 3a    ackages = find:
```

### Comparing `Twitch_Edog0049a-0.0.36/test/test1.py` & `twitch_edog0049a-0.0.37/test/test1.py`

 * *Files identical despite different names*


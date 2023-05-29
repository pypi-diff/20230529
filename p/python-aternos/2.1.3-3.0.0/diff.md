# Comparing `tmp/python-aternos-2.1.3.tar.gz` & `tmp/python-aternos-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-aternos-2.1.3.tar", last modified: Mon Oct 31 13:28:28 2022, max compression
+gzip compressed data, was "python-aternos-3.0.0.tar", last modified: Mon May 29 08:07:34 2023, max compression
```

## Comparing `python-aternos-2.1.3.tar` & `python-aternos-3.0.0.tar`

### file list

```diff
@@ -1,26 +1,34 @@
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2022-10-31 13:28:28.783320 python-aternos-2.1.3/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    11357 2022-02-15 14:48:20.000000 python-aternos-2.1.3/LICENSE
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      562 2022-08-23 06:43:33.000000 python-aternos-2.1.3/NOTICE
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6844 2022-10-31 13:28:28.783320 python-aternos-2.1.3/PKG-INFO
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5670 2022-10-05 15:46:49.000000 python-aternos-2.1.3/README.md
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      110 2022-07-01 10:05:05.000000 python-aternos-2.1.3/pyproject.toml
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2022-10-31 13:28:28.783320 python-aternos-2.1.3/python_aternos/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     1616 2022-08-19 12:47:32.000000 python-aternos-2.1.3/python_aternos/__init__.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    13666 2022-10-31 13:26:02.000000 python-aternos-2.1.3/python_aternos/atclient.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10140 2022-10-31 13:26:02.000000 python-aternos-2.1.3/python_aternos/atconf.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9044 2022-10-31 13:26:01.000000 python-aternos-2.1.3/python_aternos/atconnect.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2406 2022-10-31 13:26:01.000000 python-aternos-2.1.3/python_aternos/aterrors.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8697 2022-10-31 13:26:02.000000 python-aternos-2.1.3/python_aternos/atfile.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5261 2022-10-31 13:26:02.000000 python-aternos-2.1.3/python_aternos/atfm.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     1496 2022-10-31 13:26:01.000000 python-aternos-2.1.3/python_aternos/atjsparse.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     3319 2022-10-31 13:26:02.000000 python-aternos-2.1.3/python_aternos/atplayers.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10999 2022-10-31 13:26:02.000000 python-aternos-2.1.3/python_aternos/atserver.py
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9942 2022-10-31 13:26:02.000000 python-aternos-2.1.3/python_aternos/atwss.py
-drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2022-10-31 13:28:28.783320 python-aternos-2.1.3/python_aternos.egg-info/
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6844 2022-10-31 13:28:28.000000 python-aternos-2.1.3/python_aternos.egg-info/PKG-INFO
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      536 2022-10-31 13:28:28.000000 python-aternos-2.1.3/python_aternos.egg-info/SOURCES.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)        1 2022-10-31 13:28:28.000000 python-aternos-2.1.3/python_aternos.egg-info/dependency_links.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       79 2022-10-31 13:28:28.000000 python-aternos-2.1.3/python_aternos.egg-info/requires.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       15 2022-10-31 13:28:28.000000 python-aternos-2.1.3/python_aternos.egg-info/top_level.txt
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      105 2022-10-31 13:28:28.786653 python-aternos-2.1.3/setup.cfg
--rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     1594 2022-10-31 13:27:33.000000 python-aternos-2.1.3/setup.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-05-29 08:07:34.706738 python-aternos-3.0.0/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    11357 2022-02-15 14:48:20.000000 python-aternos-3.0.0/LICENSE
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      562 2022-08-23 06:43:33.000000 python-aternos-3.0.0/NOTICE
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7311 2023-05-29 08:07:34.706738 python-aternos-3.0.0/PKG-INFO
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6137 2023-05-29 08:02:27.000000 python-aternos-3.0.0/README.md
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      110 2022-07-01 10:05:05.000000 python-aternos-3.0.0/pyproject.toml
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-05-29 08:07:34.706738 python-aternos-3.0.0/python_aternos/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      317 2023-05-29 07:28:42.000000 python-aternos-3.0.0/python_aternos/__init__.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6067 2023-05-29 05:43:14.000000 python-aternos-3.0.0/python_aternos/ataccount.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     6857 2023-05-29 08:06:11.000000 python-aternos-3.0.0/python_aternos/atclient.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10133 2023-05-29 07:09:48.000000 python-aternos-3.0.0/python_aternos/atconf.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8868 2023-05-24 17:02:08.000000 python-aternos-3.0.0/python_aternos/atconnect.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     2406 2022-10-31 13:26:01.000000 python-aternos-3.0.0/python_aternos/aterrors.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     8655 2023-05-24 13:38:15.000000 python-aternos-3.0.0/python_aternos/atfile.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5259 2023-05-24 13:39:35.000000 python-aternos-3.0.0/python_aternos/atfm.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     5800 2023-05-24 17:02:44.000000 python-aternos-3.0.0/python_aternos/atjsparse.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      577 2023-05-29 07:41:54.000000 python-aternos-3.0.0/python_aternos/atlog.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      344 2023-05-24 15:59:49.000000 python-aternos-3.0.0/python_aternos/atmd5.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     3311 2023-05-24 15:57:21.000000 python-aternos-3.0.0/python_aternos/atplayers.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)    10912 2023-05-29 08:06:02.000000 python-aternos-3.0.0/python_aternos/atserver.py
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     9942 2023-05-24 15:57:36.000000 python-aternos-3.0.0/python_aternos/atwss.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-05-29 08:07:34.706738 python-aternos-3.0.0/python_aternos.egg-info/
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     7311 2023-05-29 08:07:34.000000 python-aternos-3.0.0/python_aternos.egg-info/PKG-INFO
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      692 2023-05-29 08:07:34.000000 python-aternos-3.0.0/python_aternos.egg-info/SOURCES.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)        1 2023-05-29 08:07:34.000000 python-aternos-3.0.0/python_aternos.egg-info/dependency_links.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       79 2023-05-29 08:07:34.000000 python-aternos-3.0.0/python_aternos.egg-info/requires.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)       15 2023-05-29 08:07:34.000000 python-aternos-3.0.0/python_aternos.egg-info/top_level.txt
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)      131 2023-05-29 08:07:34.706738 python-aternos-3.0.0/setup.cfg
+-rw-r--r--   0 darkcat09  (1000) darkcat09  (1000)     1626 2023-05-29 08:05:32.000000 python-aternos-3.0.0/setup.py
+drwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)        0 2023-05-29 08:07:34.706738 python-aternos-3.0.0/tests/
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      923 2023-05-29 07:11:46.000000 python-aternos-3.0.0/tests/test_http.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1947 2022-12-25 13:47:12.000000 python-aternos-3.0.0/tests/test_js2py.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)      741 2023-01-13 12:15:15.000000 python-aternos-3.0.0/tests/test_jsnode.py
+-rwxr-xr-x   0 darkcat09  (1000) darkcat09  (1000)     1191 2023-05-24 15:32:24.000000 python-aternos-3.0.0/tests/test_login.py
```

### Comparing `python-aternos-2.1.3/LICENSE` & `python-aternos-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-aternos-2.1.3/NOTICE` & `python-aternos-3.0.0/NOTICE`

 * *Files identical despite different names*

### Comparing `python-aternos-2.1.3/PKG-INFO` & `python-aternos-3.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aternos
-Version: 2.1.3
+Version: 3.0.0
 Summary: An unofficial Aternos API
 Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09)
 Author-email: aacd0709@mail.ru
 Project-URL: Documentation, https://python-aternos.codeberg.page
 Project-URL: GitHub, https://github.com/DarkCat09/python-aternos
 Project-URL: Bug Tracker, https://github.com/DarkCat09/python-aternos/issues
@@ -49,22 +49,22 @@
 </div>
 
 An unofficial Aternos API written in Python.  
 It uses [aternos](https://aternos.org/)' private API and html parsing.
 
 Python Aternos supports:
 
- - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value.
- - Saving session to the file and restoring.
- - Changing username, email and password.
- - Parsing Minecraft servers list.
- - Parsing server info by its ID.
- - Starting/stoping server, restarting, confirming/cancelling launch.
- - Updating server info in real-time (view WebSocket API).
- - Changing server subdomain and MOTD (message-of-the-day).
+ - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
+ - Saving session to the file and restoring
+ - Changing username, email and password
+ - Parsing Minecraft servers list
+ - Parsing server info by its ID
+ - Starting/stoping server, restarting, confirming/cancelling launch
+ - Updating server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/websocket))
+ - Changing server subdomain and MOTD (message-of-the-day)
  - Managing files, settings, players (whitelist, operators, etc.)
 
 > **Warning**
 >
 > According to the Aternos' [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
 > you must not use any software or APIs for automated access,
 > beacuse they don't receive money from advertisting in this case.
@@ -93,79 +93,92 @@
 $ git clone https://github.com/DarkCat09/python-aternos.git
 $ cd python-aternos
 $ pip install -e .
 ```
 
 ## Usage
 To use Aternos API in your Python script, import it
-and login with your username and password or MD5.
+and login with your username and password or its MD5 hash.
 
 Then request the servers list using `list_servers()`.  
 You can start/stop your Aternos server, calling `start()` or `stop()`.
 
 Here is an example how to use the API:
 ```python
 # Import
 from python_aternos import Client
 
+# Create object
+aternos = Client()
+
 # Log in
-aternos = Client.from_credentials('example', 'test123')
+# with username and password
+aternos.login('example', 'test123')
 # ----OR----
-aternos = Client.from_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
+# with username and MD5 hashed password
+aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
 # ----OR----
-aternos = Client.restore_session()
+# with session cookie
+aternos.login_with_session('ATERNOS_SESSION cookie value')
 
-# Returns AternosServer list
+# Get servers list
 servs = aternos.list_servers()
 
-# Get the first server by the 0 index
+# Get the first server
 myserv = servs[0]
 
 # Start
 myserv.start()
 # Stop
 myserv.stop()
 
 # You can also find server by IP
 testserv = None
 for serv in servs:
     if serv.address == 'test.aternos.org':
         testserv = serv
 
 if testserv is not None:
-    # Prints a server softaware and its version
+    # Prints the server software and its version
     # (for example, "Vanilla 1.12.2")
     print(testserv.software, testserv.version)
     # Starts server
     testserv.start()
 ```
 
 ## [More examples](https://github.com/DarkCat09/python-aternos/tree/main/examples)
 
-## [Documentation](https://python-aternos.codeberg.page/)
+## [Documentation](https://aternos.dc09.ru)
 
-## [How-To Guide](https://python-aternos.codeberg.page/howto/auth)
+## [How-To Guide](https://aternos.dc09.ru/howto/auth)
 
 ## Changelog
 |Version|Description |
 |:-----:|:-----------|
-|v0.1|The first release.|
-|v0.2|Fixed import problem.|
 |v0.3|Implemented files API, added typization.|
 |v0.4|Implemented configuration API, some bugfixes.|
 |v0.5|The API was updated corresponding to new Aternos security methods. Huge thanks to [lusm554](https://github.com/lusm554).|
 |**v0.6/v1.0.0**|Code refactoring, websockets API and session saving to prevent detecting automation access.|
 |v1.0.x|Lots of bugfixes, changed versioning (SemVer).|
 |v1.1.x|Documentation, unit tests, pylint, bugfixes, changes in atwss.|
 |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/DarkCat09/python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS parser.|
 |v2.0.x|Documentation, automatically saving/restoring session, improvements in Files API.|
-|v2.1.x|Fixes in websockets API, atconnect. Supported captcha solving services (view [#52](https://github.com/DarkCat09/python-aternos/issues/52)).|
-|**v2.2.x**|Using Node.js as a JS interpreter if it's installed.|
-|v3.0.x|Full implementation of config and software API.|
-|v3.1.x|Shared access API and Google Drive backups.|
+|v2.1.x|Fixes in websockets API, atconnect (including cookie refreshing fix). Support for captcha solving services (view [#52](https://github.com/DarkCat09/python-aternos/issues/52)).|
+|v2.2.x|Node.JS interpreter support.|
+|v3.0.0|Partially rewritten, API updates.|
+|v3.1.x|Full implementation of config API.|
+|v3.2.x|Shared access API and maybe Google Drive backups.|
+
+## Reversed API Specification
+Private Aternos API requests were captured into
+[this HAR file](https://github.com/DarkCat09/python-aternos/blob/main/aternos.har)
+and were imported to
+[a Postman Workspace](https://www.postman.com/darkcat09/workspace/aternos-api).  
+You can use both resources to explore the API.  
+Any help with improving this library is welcome.
 
 ## License
 [License Notice:](https://github.com/DarkCat09/python-aternos/blob/main/NOTICE)
 ```
 Copyright 2021-2022 All contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-aternos Version: 2.1.3 Summary: An
+Metadata-Version: 2.1 Name: python-aternos Version: 3.0.0 Summary: An
 unofficial Aternos API Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09) Author-email: aacd0709@mail.ru Project-
 URL: Documentation, https://python-aternos.codeberg.page Project-URL: GitHub,
 https://github.com/DarkCat09/python-aternos Project-URL: Bug Tracker, https://
 github.com/DarkCat09/python-aternos/issues Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -17,67 +17,74 @@
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
 aternos.org/)' private API and html parsing. Python Aternos supports: - Logging
-in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie
-value. - Saving session to the file and restoring. - Changing username, email
-and password. - Parsing Minecraft servers list. - Parsing server info by its
-ID. - Starting/stoping server, restarting, confirming/cancelling launch. -
-Updating server info in real-time (view WebSocket API). - Changing server
-subdomain and MOTD (message-of-the-day). - Managing files, settings, players
-(whitelist, operators, etc.) > **Warning** > > According to the Aternos' [Terms
-of Service Â§5.2e](https://aternos.gmbh/en/aternos/terms#:~:
+in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
+- Saving session to the file and restoring - Changing username, email and
+password - Parsing Minecraft servers list - Parsing server info by its ID -
+Starting/stoping server, restarting, confirming/cancelling launch - Updating
+server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/
+websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
+Managing files, settings, players (whitelist, operators, etc.) > **Warning** >
+> According to the Aternos' [Terms of Service Â§5.2e](https://aternos.gmbh/en/
+aternos/terms#:~:
 text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
 > you must not use any software or APIs for automated access, > beacuse they
 don't receive money from advertisting in this case. > > I always try to hide
 automated python-aternos requests > using browser-specific headers/cookies, >
 but you should make backups to restore your world > if Aternos detects
 violation of ToS and bans your account > (view issues [#16](https://github.com/
 DarkCat09/python-aternos/issues/16) > and [#46](https://github.com/DarkCat09/
 python-aternos/issues/46)). ## Install ### Common ```bash $ pip install python-
 aternos ``` > **Note** for Windows users > > Install `lxml` package from [here]
 (https://www.lfd.uci.edu/~gohlke/pythonlibs/#lxml) > if you have problems with
 it, and then execute: > `pip install --no-deps python-aternos` ### Development
 ```bash $ git clone https://github.com/DarkCat09/python-aternos.git $ cd
 python-aternos $ pip install -e . ``` ## Usage To use Aternos API in your
-Python script, import it and login with your username and password or MD5. Then
-request the servers list using `list_servers()`. You can start/stop your
-Aternos server, calling `start()` or `stop()`. Here is an example how to use
-the API: ```python # Import from python_aternos import Client # Log in aternos
-= Client.from_credentials('example', 'test123') # ----OR---- aternos =
-Client.from_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---
-- aternos = Client.restore_session() # Returns AternosServer list servs =
-aternos.list_servers() # Get the first server by the 0 index myserv = servs[0]
-# Start myserv.start() # Stop myserv.stop() # You can also find server by IP
-testserv = None for serv in servs: if serv.address == 'test.aternos.org':
-testserv = serv if testserv is not None: # Prints a server softaware and its
-version # (for example, "Vanilla 1.12.2") print(testserv.software,
-testserv.version) # Starts server testserv.start() ``` ## [More examples]
-(https://github.com/DarkCat09/python-aternos/tree/main/examples) ##
-[Documentation](https://python-aternos.codeberg.page/) ## [How-To Guide](https:
-//python-aternos.codeberg.page/howto/auth) ## Changelog |Version|Description |
-|:-----:|:-----------| |v0.1|The first release.| |v0.2|Fixed import problem.|
-|v0.3|Implemented files API, added typization.| |v0.4|Implemented configuration
-API, some bugfixes.| |v0.5|The API was updated corresponding to new Aternos
-security methods. Huge thanks to [lusm554](https://github.com/lusm554).|
-|**v0.6/v1.0.0**|Code refactoring, websockets API and session saving to prevent
-detecting automation access.| |v1.0.x|Lots of bugfixes, changed versioning
-(SemVer).| |v1.1.x|Documentation, unit tests, pylint, bugfixes, changes in
-atwss.| |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/DarkCat09/
-python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS parser.|
-|v2.0.x|Documentation, automatically saving/restoring session, improvements in
-Files API.| |v2.1.x|Fixes in websockets API, atconnect. Supported captcha
-solving services (view [#52](https://github.com/DarkCat09/python-aternos/
-issues/52)).| |**v2.2.x**|Using Node.js as a JS interpreter if it's installed.|
-|v3.0.x|Full implementation of config and software API.| |v3.1.x|Shared access
-API and Google Drive backups.| ## License [License Notice:](https://github.com/
-DarkCat09/python-aternos/blob/main/NOTICE) ``` Copyright 2021-2022 All
-contributors Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License. You may obtain
-a copy of the License at http://www.apache.org/licenses/LICENSE-2.0 Unless
-required by applicable law or agreed to in writing, software distributed under
-the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
-CONDITIONS OF ANY KIND, either express or implied. See the License for the
-specific language governing permissions and limitations under the License. ```
+Python script, import it and login with your username and password or its MD5
+hash. Then request the servers list using `list_servers()`. You can start/stop
+your Aternos server, calling `start()` or `stop()`. Here is an example how to
+use the API: ```python # Import from python_aternos import Client # Create
+object aternos = Client() # Log in # with username and password aternos.login
+('example', 'test123') # ----OR---- # with username and MD5 hashed password
+aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---
+- # with session cookie aternos.login_with_session('ATERNOS_SESSION cookie
+value') # Get servers list servs = aternos.list_servers() # Get the first
+server myserv = servs[0] # Start myserv.start() # Stop myserv.stop() # You can
+also find server by IP testserv = None for serv in servs: if serv.address ==
+'test.aternos.org': testserv = serv if testserv is not None: # Prints the
+server software and its version # (for example, "Vanilla 1.12.2") print
+(testserv.software, testserv.version) # Starts server testserv.start() ``` ##
+[More examples](https://github.com/DarkCat09/python-aternos/tree/main/examples)
+## [Documentation](https://aternos.dc09.ru) ## [How-To Guide](https://
+aternos.dc09.ru/howto/auth) ## Changelog |Version|Description | |:-----:|:-----
+------| |v0.3|Implemented files API, added typization.| |v0.4|Implemented
+configuration API, some bugfixes.| |v0.5|The API was updated corresponding to
+new Aternos security methods. Huge thanks to [lusm554](https://github.com/
+lusm554).| |**v0.6/v1.0.0**|Code refactoring, websockets API and session saving
+to prevent detecting automation access.| |v1.0.x|Lots of bugfixes, changed
+versioning (SemVer).| |v1.1.x|Documentation, unit tests, pylint, bugfixes,
+changes in atwss.| |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/
+DarkCat09/python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS
+parser.| |v2.0.x|Documentation, automatically saving/restoring session,
+improvements in Files API.| |v2.1.x|Fixes in websockets API, atconnect
+(including cookie refreshing fix). Support for captcha solving services (view
+[#52](https://github.com/DarkCat09/python-aternos/issues/52)).| |v2.2.x|Node.JS
+interpreter support.| |v3.0.0|Partially rewritten, API updates.| |v3.1.x|Full
+implementation of config API.| |v3.2.x|Shared access API and maybe Google Drive
+backups.| ## Reversed API Specification Private Aternos API requests were
+captured into [this HAR file](https://github.com/DarkCat09/python-aternos/blob/
+main/aternos.har) and were imported to [a Postman Workspace](https://
+www.postman.com/darkcat09/workspace/aternos-api). You can use both resources to
+explore the API. Any help with improving this library is welcome. ## License
+[License Notice:](https://github.com/DarkCat09/python-aternos/blob/main/NOTICE)
+``` Copyright 2021-2022 All contributors Licensed under the Apache License,
+Version 2.0 (the "License"); you may not use this file except in compliance
+with the License. You may obtain a copy of the License at http://
+www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
+to in writing, software distributed under the License is distributed on an "AS
+IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+implied. See the License for the specific language governing permissions and
+limitations under the License. ```
```

### Comparing `python-aternos-2.1.3/README.md` & `python-aternos-3.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -20,22 +20,22 @@
 </div>
 
 An unofficial Aternos API written in Python.  
 It uses [aternos](https://aternos.org/)' private API and html parsing.
 
 Python Aternos supports:
 
- - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value.
- - Saving session to the file and restoring.
- - Changing username, email and password.
- - Parsing Minecraft servers list.
- - Parsing server info by its ID.
- - Starting/stoping server, restarting, confirming/cancelling launch.
- - Updating server info in real-time (view WebSocket API).
- - Changing server subdomain and MOTD (message-of-the-day).
+ - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
+ - Saving session to the file and restoring
+ - Changing username, email and password
+ - Parsing Minecraft servers list
+ - Parsing server info by its ID
+ - Starting/stoping server, restarting, confirming/cancelling launch
+ - Updating server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/websocket))
+ - Changing server subdomain and MOTD (message-of-the-day)
  - Managing files, settings, players (whitelist, operators, etc.)
 
 > **Warning**
 >
 > According to the Aternos' [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
 > you must not use any software or APIs for automated access,
 > beacuse they don't receive money from advertisting in this case.
@@ -64,79 +64,92 @@
 $ git clone https://github.com/DarkCat09/python-aternos.git
 $ cd python-aternos
 $ pip install -e .
 ```
 
 ## Usage
 To use Aternos API in your Python script, import it
-and login with your username and password or MD5.
+and login with your username and password or its MD5 hash.
 
 Then request the servers list using `list_servers()`.  
 You can start/stop your Aternos server, calling `start()` or `stop()`.
 
 Here is an example how to use the API:
 ```python
 # Import
 from python_aternos import Client
 
+# Create object
+aternos = Client()
+
 # Log in
-aternos = Client.from_credentials('example', 'test123')
+# with username and password
+aternos.login('example', 'test123')
 # ----OR----
-aternos = Client.from_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
+# with username and MD5 hashed password
+aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
 # ----OR----
-aternos = Client.restore_session()
+# with session cookie
+aternos.login_with_session('ATERNOS_SESSION cookie value')
 
-# Returns AternosServer list
+# Get servers list
 servs = aternos.list_servers()
 
-# Get the first server by the 0 index
+# Get the first server
 myserv = servs[0]
 
 # Start
 myserv.start()
 # Stop
 myserv.stop()
 
 # You can also find server by IP
 testserv = None
 for serv in servs:
     if serv.address == 'test.aternos.org':
         testserv = serv
 
 if testserv is not None:
-    # Prints a server softaware and its version
+    # Prints the server software and its version
     # (for example, "Vanilla 1.12.2")
     print(testserv.software, testserv.version)
     # Starts server
     testserv.start()
 ```
 
 ## [More examples](https://github.com/DarkCat09/python-aternos/tree/main/examples)
 
-## [Documentation](https://python-aternos.codeberg.page/)
+## [Documentation](https://aternos.dc09.ru)
 
-## [How-To Guide](https://python-aternos.codeberg.page/howto/auth)
+## [How-To Guide](https://aternos.dc09.ru/howto/auth)
 
 ## Changelog
 |Version|Description |
 |:-----:|:-----------|
-|v0.1|The first release.|
-|v0.2|Fixed import problem.|
 |v0.3|Implemented files API, added typization.|
 |v0.4|Implemented configuration API, some bugfixes.|
 |v0.5|The API was updated corresponding to new Aternos security methods. Huge thanks to [lusm554](https://github.com/lusm554).|
 |**v0.6/v1.0.0**|Code refactoring, websockets API and session saving to prevent detecting automation access.|
 |v1.0.x|Lots of bugfixes, changed versioning (SemVer).|
 |v1.1.x|Documentation, unit tests, pylint, bugfixes, changes in atwss.|
 |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/DarkCat09/python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS parser.|
 |v2.0.x|Documentation, automatically saving/restoring session, improvements in Files API.|
-|v2.1.x|Fixes in websockets API, atconnect. Supported captcha solving services (view [#52](https://github.com/DarkCat09/python-aternos/issues/52)).|
-|**v2.2.x**|Using Node.js as a JS interpreter if it's installed.|
-|v3.0.x|Full implementation of config and software API.|
-|v3.1.x|Shared access API and Google Drive backups.|
+|v2.1.x|Fixes in websockets API, atconnect (including cookie refreshing fix). Support for captcha solving services (view [#52](https://github.com/DarkCat09/python-aternos/issues/52)).|
+|v2.2.x|Node.JS interpreter support.|
+|v3.0.0|Partially rewritten, API updates.|
+|v3.1.x|Full implementation of config API.|
+|v3.2.x|Shared access API and maybe Google Drive backups.|
+
+## Reversed API Specification
+Private Aternos API requests were captured into
+[this HAR file](https://github.com/DarkCat09/python-aternos/blob/main/aternos.har)
+and were imported to
+[a Postman Workspace](https://www.postman.com/darkcat09/workspace/aternos-api).  
+You can use both resources to explore the API.  
+Any help with improving this library is welcome.
 
 ## License
 [License Notice:](https://github.com/DarkCat09/python-aternos/blob/main/NOTICE)
 ```
 Copyright 2021-2022 All contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

#### html2text {}

```diff
@@ -1,67 +1,74 @@
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
 aternos.org/)' private API and html parsing. Python Aternos supports: - Logging
-in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie
-value. - Saving session to the file and restoring. - Changing username, email
-and password. - Parsing Minecraft servers list. - Parsing server info by its
-ID. - Starting/stoping server, restarting, confirming/cancelling launch. -
-Updating server info in real-time (view WebSocket API). - Changing server
-subdomain and MOTD (message-of-the-day). - Managing files, settings, players
-(whitelist, operators, etc.) > **Warning** > > According to the Aternos' [Terms
-of Service Â§5.2e](https://aternos.gmbh/en/aternos/terms#:~:
+in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
+- Saving session to the file and restoring - Changing username, email and
+password - Parsing Minecraft servers list - Parsing server info by its ID -
+Starting/stoping server, restarting, confirming/cancelling launch - Updating
+server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/
+websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
+Managing files, settings, players (whitelist, operators, etc.) > **Warning** >
+> According to the Aternos' [Terms of Service Â§5.2e](https://aternos.gmbh/en/
+aternos/terms#:~:
 text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
 > you must not use any software or APIs for automated access, > beacuse they
 don't receive money from advertisting in this case. > > I always try to hide
 automated python-aternos requests > using browser-specific headers/cookies, >
 but you should make backups to restore your world > if Aternos detects
 violation of ToS and bans your account > (view issues [#16](https://github.com/
 DarkCat09/python-aternos/issues/16) > and [#46](https://github.com/DarkCat09/
 python-aternos/issues/46)). ## Install ### Common ```bash $ pip install python-
 aternos ``` > **Note** for Windows users > > Install `lxml` package from [here]
 (https://www.lfd.uci.edu/~gohlke/pythonlibs/#lxml) > if you have problems with
 it, and then execute: > `pip install --no-deps python-aternos` ### Development
 ```bash $ git clone https://github.com/DarkCat09/python-aternos.git $ cd
 python-aternos $ pip install -e . ``` ## Usage To use Aternos API in your
-Python script, import it and login with your username and password or MD5. Then
-request the servers list using `list_servers()`. You can start/stop your
-Aternos server, calling `start()` or `stop()`. Here is an example how to use
-the API: ```python # Import from python_aternos import Client # Log in aternos
-= Client.from_credentials('example', 'test123') # ----OR---- aternos =
-Client.from_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---
-- aternos = Client.restore_session() # Returns AternosServer list servs =
-aternos.list_servers() # Get the first server by the 0 index myserv = servs[0]
-# Start myserv.start() # Stop myserv.stop() # You can also find server by IP
-testserv = None for serv in servs: if serv.address == 'test.aternos.org':
-testserv = serv if testserv is not None: # Prints a server softaware and its
-version # (for example, "Vanilla 1.12.2") print(testserv.software,
-testserv.version) # Starts server testserv.start() ``` ## [More examples]
-(https://github.com/DarkCat09/python-aternos/tree/main/examples) ##
-[Documentation](https://python-aternos.codeberg.page/) ## [How-To Guide](https:
-//python-aternos.codeberg.page/howto/auth) ## Changelog |Version|Description |
-|:-----:|:-----------| |v0.1|The first release.| |v0.2|Fixed import problem.|
-|v0.3|Implemented files API, added typization.| |v0.4|Implemented configuration
-API, some bugfixes.| |v0.5|The API was updated corresponding to new Aternos
-security methods. Huge thanks to [lusm554](https://github.com/lusm554).|
-|**v0.6/v1.0.0**|Code refactoring, websockets API and session saving to prevent
-detecting automation access.| |v1.0.x|Lots of bugfixes, changed versioning
-(SemVer).| |v1.1.x|Documentation, unit tests, pylint, bugfixes, changes in
-atwss.| |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/DarkCat09/
-python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS parser.|
-|v2.0.x|Documentation, automatically saving/restoring session, improvements in
-Files API.| |v2.1.x|Fixes in websockets API, atconnect. Supported captcha
-solving services (view [#52](https://github.com/DarkCat09/python-aternos/
-issues/52)).| |**v2.2.x**|Using Node.js as a JS interpreter if it's installed.|
-|v3.0.x|Full implementation of config and software API.| |v3.1.x|Shared access
-API and Google Drive backups.| ## License [License Notice:](https://github.com/
-DarkCat09/python-aternos/blob/main/NOTICE) ``` Copyright 2021-2022 All
-contributors Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License. You may obtain
-a copy of the License at http://www.apache.org/licenses/LICENSE-2.0 Unless
-required by applicable law or agreed to in writing, software distributed under
-the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
-CONDITIONS OF ANY KIND, either express or implied. See the License for the
-specific language governing permissions and limitations under the License. ```
+Python script, import it and login with your username and password or its MD5
+hash. Then request the servers list using `list_servers()`. You can start/stop
+your Aternos server, calling `start()` or `stop()`. Here is an example how to
+use the API: ```python # Import from python_aternos import Client # Create
+object aternos = Client() # Log in # with username and password aternos.login
+('example', 'test123') # ----OR---- # with username and MD5 hashed password
+aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---
+- # with session cookie aternos.login_with_session('ATERNOS_SESSION cookie
+value') # Get servers list servs = aternos.list_servers() # Get the first
+server myserv = servs[0] # Start myserv.start() # Stop myserv.stop() # You can
+also find server by IP testserv = None for serv in servs: if serv.address ==
+'test.aternos.org': testserv = serv if testserv is not None: # Prints the
+server software and its version # (for example, "Vanilla 1.12.2") print
+(testserv.software, testserv.version) # Starts server testserv.start() ``` ##
+[More examples](https://github.com/DarkCat09/python-aternos/tree/main/examples)
+## [Documentation](https://aternos.dc09.ru) ## [How-To Guide](https://
+aternos.dc09.ru/howto/auth) ## Changelog |Version|Description | |:-----:|:-----
+------| |v0.3|Implemented files API, added typization.| |v0.4|Implemented
+configuration API, some bugfixes.| |v0.5|The API was updated corresponding to
+new Aternos security methods. Huge thanks to [lusm554](https://github.com/
+lusm554).| |**v0.6/v1.0.0**|Code refactoring, websockets API and session saving
+to prevent detecting automation access.| |v1.0.x|Lots of bugfixes, changed
+versioning (SemVer).| |v1.1.x|Documentation, unit tests, pylint, bugfixes,
+changes in atwss.| |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/
+DarkCat09/python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS
+parser.| |v2.0.x|Documentation, automatically saving/restoring session,
+improvements in Files API.| |v2.1.x|Fixes in websockets API, atconnect
+(including cookie refreshing fix). Support for captcha solving services (view
+[#52](https://github.com/DarkCat09/python-aternos/issues/52)).| |v2.2.x|Node.JS
+interpreter support.| |v3.0.0|Partially rewritten, API updates.| |v3.1.x|Full
+implementation of config API.| |v3.2.x|Shared access API and maybe Google Drive
+backups.| ## Reversed API Specification Private Aternos API requests were
+captured into [this HAR file](https://github.com/DarkCat09/python-aternos/blob/
+main/aternos.har) and were imported to [a Postman Workspace](https://
+www.postman.com/darkcat09/workspace/aternos-api). You can use both resources to
+explore the API. Any help with improving this library is welcome. ## License
+[License Notice:](https://github.com/DarkCat09/python-aternos/blob/main/NOTICE)
+``` Copyright 2021-2022 All contributors Licensed under the Apache License,
+Version 2.0 (the "License"); you may not use this file except in compliance
+with the License. You may obtain a copy of the License at http://
+www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
+to in writing, software distributed under the License is distributed on an "AS
+IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+implied. See the License for the specific language governing permissions and
+limitations under the License. ```
```

### Comparing `python-aternos-2.1.3/python_aternos/atconf.py` & `python-aternos-3.0.0/python_aternos/atconf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 """Modifying server and world options"""
 
+# TODO: Still needs refactoring
+
 import enum
 import re
 
 from typing import Any, Dict, List, Union, Optional
 from typing import TYPE_CHECKING
 
 import lxml.html
 
+from .atconnect import BASE_URL, AJAX_URL
 if TYPE_CHECKING:
     from .atserver import AternosServer
 
+
 DAT_PREFIX = 'Data:'
 DAT_GR_PREFIX = 'Data:GameRules:'
 
 
 class ServerOpts(enum.Enum):
 
     """server.options file"""
@@ -107,19 +111,20 @@
     easy = 1
     normal = 2
     hard = 3
 
 
 # checking timezone format
 tzcheck = re.compile(r'(^[A-Z]\w+\/[A-Z]\w+$)|^UTC$')
+
 # options types converting
 convert = {
     'config-option-number': int,
     'config-option-select': int,
-    'config-option-toggle': bool
+    'config-option-toggle': bool,
 }
 
 
 class AternosConfig:
 
     """Class for editing server settings"""
 
@@ -137,15 +142,15 @@
         """Parses timezone from options page
 
         Returns:
             Area/Location
         """
 
         optreq = self.atserv.atserver_request(
-            'https://aternos.org/options', 'GET'
+            f'{BASE_URL}/options', 'GET'
         )
         opttree = lxml.html.fromstring(optreq)
 
         tzopt = opttree.xpath(
             '//div[@class="options-other-input timezone-switch"]'
         )[0]
         tztext = tzopt.xpath('.//div[@class="option current"]')[0].text
@@ -165,28 +170,28 @@
         matches_tz = tzcheck.search(value)
         if not matches_tz:
             raise ValueError(
                 'Timezone must match zoneinfo format: Area/Location'
             )
 
         self.atserv.atserver_request(
-            'https://aternos.org/panel/ajax/timezone.php',
+            f'{AJAX_URL}/timezone.php',
             'POST', data={'timezone': value},
             sendtoken=True
         )
 
     def get_java(self) -> int:
         """Parses Java version from options page
 
         Returns:
             Java image version
         """
 
         optreq = self.atserv.atserver_request(
-            'https://aternos.org/options', 'GET'
+            f'{BASE_URL}/options', 'GET'
         )
         opttree = lxml.html.fromstring(optreq)
         imgopt = opttree.xpath(
             '//div[@class="options-other-input image-switch"]'
         )[0]
         imgver = imgopt.xpath(
             './/div[@class="option current"]/@data-value'
@@ -199,15 +204,15 @@
         """Sets new Java version
 
         Args:
             value (int): New Java image version
         """
 
         self.atserv.atserver_request(
-            'https://aternos.org/panel/ajax/image.php',
+            f'{AJAX_URL}/image.php',
             'POST', data={'image': f'openjdk:{value}'},
             sendtoken=True
         )
 
     #
     # server.properties
     #
@@ -234,15 +239,15 @@
                 property type (e.g. max-players will be int)
                 instead of string
 
         Returns:
             `server.properties` dictionary
         """
 
-        return self.__get_all_props('https://aternos.org/options', proptyping)
+        return self.__get_all_props(f'{BASE_URL}/options', proptyping)
 
     def set_server_props(self, props: Dict[str, Any]) -> None:
         """Updates server.properties options with the given dict
 
         Args:
             props (Dict[str,Any]):
                 Dictionary with `{key:value}` properties
@@ -292,15 +297,15 @@
                 instead of string
 
         Returns:
             `level.dat` options dictionary
         """
 
         return self.__get_all_props(
-            f'https://aternos.org/files/{world}/level.dat',
+            f'{BASE_URL}/files/{world}/level.dat',
             proptyping, [DAT_PREFIX, DAT_GR_PREFIX]
         )
 
     def set_world_props(
             self,
             props: Dict[Union[WorldOpts, WorldRules], Any],
             world: str = 'world') -> None:
@@ -323,15 +328,15 @@
 
     #
     # helpers
     #
     def __set_prop(self, file: str, option: str, value: Any) -> None:
 
         self.atserv.atserver_request(
-            'https://aternos.org/panel/ajax/config.php',
+            f'{AJAX_URL}/config.php',
             'POST', data={
                 'file': file,
                 'option': option,
                 'value': value
             }, sendtoken=True
         )
```

### Comparing `python-aternos-2.1.3/python_aternos/atconnect.py` & `python-aternos-3.0.0/python_aternos/atconnect.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,58 @@
-"""Stores API connection session and sends requests"""
+"""Stores API session and sends requests"""
 
 import re
 import time
+
+import string
 import secrets
-import logging
+
 from functools import partial
 
 from typing import Optional
 from typing import List, Dict, Any
 
 import requests
 
 from cloudscraper import CloudScraper
 
+from .atlog import log, is_debug
+
 from . import atjsparse
 from .aterrors import TokenError
 from .aterrors import CloudflareError
 from .aterrors import AternosPermissionError
 
+
+BASE_URL = 'https://aternos.org'
+AJAX_URL = f'{BASE_URL}/ajax'
+
 REQUA = \
     'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 ' \
     '(KHTML, like Gecko) Chrome/99.0.4844.84 Safari/537.36 OPR/85.0.4341.47'
 
-ARROW_FN_REGEX = r'\(\(\)(.*?)\)\(\);'
+ARROW_FN_REGEX = r'\(\(\).*?\)\(\);'
 SCRIPT_TAG_REGEX = (
     rb'<script type=([\'"]?)text/javascript\1>.+?</script>'
 )
 
+SEC_ALPHABET = string.ascii_lowercase + string.digits
 
-class AternosConnect:
 
+class AternosConnect:
     """Class for sending API requests,
     bypassing Cloudflare and parsing responses"""
 
     def __init__(self) -> None:
 
         self.cf_init = partial(CloudScraper)
         self.session = self.cf_init()
         self.sec = ''
         self.token = ''
-
-    def add_args(self, **kwargs) -> None:
-        """Pass arguments to CloudScarper
-        session object __init__
-        if kwargs is not empty
-
-        Args:
-            **kwargs: Keyword arguments
-        """
-
-        if len(kwargs) < 1:
-            logging.debug('**kwargs is empty')
-            return
-
-        logging.debug('New args for CloudScraper: %s', kwargs)
-        self.cf_init = partial(CloudScraper, **kwargs)
-        self.refresh_session()
-
-    def clear_args(self) -> None:
-        """Clear CloudScarper object __init__ arguments
-        which was set using add_args method"""
-
-        logging.debug('Creating session object with no keywords')
-        self.cf_init = partial(CloudScraper)
-        self.refresh_session()
+        self.atcookie = ''
 
     def refresh_session(self) -> None:
         """Creates a new CloudScraper
         session object and copies all cookies.
         Required for bypassing Cloudflare"""
 
         old_cookies = self.session.cookies
@@ -76,71 +61,71 @@
         del old_cookies
 
     def parse_token(self) -> str:
         """Parses Aternos ajax token that
         is needed for most requests
 
         Raises:
-            RuntimeWarning: If the parser can not
-                find `<head>` tag in HTML response
             TokenError: If the parser is unable
                 to extract ajax token from HTML
 
         Returns:
             Aternos ajax token
         """
 
         loginpage = self.request_cloudflare(
-            'https://aternos.org/go/', 'GET'
+            f'{BASE_URL}/go/', 'GET'
         ).content
 
         # Using the standard string methods
         # instead of the expensive xml parsing
         head = b'<head>'
         headtag = loginpage.find(head)
         headend = loginpage.find(b'</head>', headtag + len(head))
 
         # Some checks
         if headtag < 0 or headend < 0:
             pagehead = loginpage
-            logging.warning(
+            log.warning(
                 'Unable to find <head> tag, parsing the whole page'
             )
 
         else:
             # Extracting <head> content
             headtag = headtag + len(head)
             pagehead = loginpage[headtag:headend]
 
         js_code: Optional[List[Any]] = None
+
         try:
             text = pagehead.decode('utf-8', 'replace')
             js_code = re.findall(ARROW_FN_REGEX, text)
 
             token_func = js_code[0]
             if len(js_code) > 1:
                 token_func = js_code[1]
 
-            ctx = atjsparse.exec_js(token_func)
-            self.token = ctx.window['AJAX_TOKEN']
+            js = atjsparse.get_interpreter()
+            js.exec_js(token_func)
+            self.token = js['AJAX_TOKEN']
 
         except (IndexError, TypeError) as err:
 
-            logging.warning('---')
-            logging.warning('Unable to parse AJAX_TOKEN!')
-            logging.warning('Please, insert the info below')
-            logging.warning('to the GitHub issue description:')
-            logging.warning('---')
+            log.warning('---')
+            log.warning('Unable to parse AJAX_TOKEN!')
+            log.warning('Please, insert the info below')
+            log.warning('to the GitHub issue description:')
+            log.warning('---')
 
-            logging.warning('JavaScript: %s', js_code)
-            logging.warning(
+            log.warning('JavaScript: %s', js_code)
+            log.warning(
                 'All script tags: %s',
                 re.findall(SCRIPT_TAG_REGEX, pagehead)
             )
-            logging.warning('---')
+            log.warning('---')
 
             raise TokenError(
                 'Unable to parse TOKEN from the page'
             ) from err
 
         return self.token
 
@@ -148,59 +133,74 @@
         """Generates Aternos SEC token which
         is also needed for most API requests
 
         Returns:
             Random SEC `key:value` string
         """
 
-        randkey = secrets.token_hex(8)
-        randval = secrets.token_hex(8)
+        randkey = self.generate_sec_part()
+        randval = self.generate_sec_part()
         self.sec = f'{randkey}:{randval}'
         self.session.cookies.set(
             f'ATERNOS_SEC_{randkey}', randval,
             domain='aternos.org'
         )
 
         return self.sec
 
+    def generate_sec_part(self) -> str:
+        """Generates a part for SEC token"""
+
+        return ''.join(
+            secrets.choice(SEC_ALPHABET)
+            for _ in range(11)
+        ) + ('0' * 5)
+
     def request_cloudflare(
             self, url: str, method: str,
             params: Optional[Dict[Any, Any]] = None,
             data: Optional[Dict[Any, Any]] = None,
             headers: Optional[Dict[Any, Any]] = None,
             reqcookies: Optional[Dict[Any, Any]] = None,
             sendtoken: bool = False,
-            retry: int = 5) -> requests.Response:
+            retries: int = 5,
+            timeout: int = 4) -> requests.Response:
         """Sends a request to Aternos API bypass Cloudflare
 
         Args:
             url (str): Request URL
             method (str): Request method, must be GET or POST
             params (Optional[Dict[Any, Any]], optional): URL parameters
             data (Optional[Dict[Any, Any]], optional): POST request data,
                 if the method is GET, this dict will be combined with params
             headers (Optional[Dict[Any, Any]], optional): Custom headers
             reqcookies (Optional[Dict[Any, Any]], optional):
                 Cookies only for this request
             sendtoken (bool, optional): If the ajax and SEC token
                 should be sent
-            retry (int, optional): How many times parser must retry
+            retries (int, optional): How many times parser must retry
                 connection to API bypass Cloudflare
+            timeout (int, optional): Request timeout in seconds
 
         Raises:
             CloudflareError: When the parser has exceeded retries count
             NotImplementedError: When the specified method is not GET or POST
 
         Returns:
             API response
         """
 
-        if retry <= 0:
+        if retries <= 0:
             raise CloudflareError('Unable to bypass Cloudflare protection')
 
+        try:
+            self.atcookie = self.session.cookies['ATERNOS_SESSION']
+        except KeyError:
+            pass
+
         self.refresh_session()
 
         params = params or {}
         data = data or {}
         headers = headers or {}
         reqcookies = reqcookies or {}
 
@@ -211,68 +211,71 @@
 
         if sendtoken:
             params['TOKEN'] = self.token
             params['SEC'] = self.sec
             headers['X-Requested-With'] = 'XMLHttpRequest'
 
         # requests.cookies.CookieConflictError bugfix
-        reqcookies['ATERNOS_SESSION'] = self.atsession
+        reqcookies['ATERNOS_SESSION'] = self.atcookie
         del self.session.cookies['ATERNOS_SESSION']
 
-        reqcookies_dbg = {
-            k: str(v or '')[:3]
-            for k, v in reqcookies.items()
-        }
-
-        session_cookies_dbg = {
-            k: str(v or '')[:3]
-            for k, v in self.session.cookies.items()
-        }
-
-        logging.debug('Requesting(%s)%s', method, url)
-        logging.debug('headers=%s', headers)
-        logging.debug('params=%s', params)
-        logging.debug('data=%s', data)
-        logging.debug('req-cookies=%s', reqcookies_dbg)
-        logging.debug('session-cookies=%s', session_cookies_dbg)
+        if is_debug():
+
+            reqcookies_dbg = {
+                k: str(v or '')[:3]
+                for k, v in reqcookies.items()
+            }
+
+            session_cookies_dbg = {
+                k: str(v or '')[:3]
+                for k, v in self.session.cookies.items()
+            }
+
+            log.debug('Requesting(%s)%s', method, url)
+            log.debug('headers=%s', headers)
+            log.debug('params=%s', params)
+            log.debug('data=%s', data)
+            log.debug('req-cookies=%s', reqcookies_dbg)
+            log.debug('session-cookies=%s', session_cookies_dbg)
 
         if method == 'POST':
             sendreq = partial(
                 self.session.post,
                 params=params,
-                data=data
+                data=data,
             )
         else:
             sendreq = partial(
                 self.session.get,
-                params={**params, **data}
+                params={**params, **data},
             )
 
         req = sendreq(
             url,
             headers=headers,
-            cookies=reqcookies
+            cookies=reqcookies,
+            timeout=timeout,
         )
 
         resp_type = req.headers.get('content-type', '')
         html_type = resp_type.find('text/html') != -1
         cloudflare = req.status_code == 403
 
         if html_type and cloudflare:
-            logging.info('Retrying to bypass Cloudflare')
-            time.sleep(0.2)
+            log.info('Retrying to bypass Cloudflare')
+            time.sleep(0.3)
             return self.request_cloudflare(
                 url, method,
                 params, data,
                 headers, reqcookies,
-                sendtoken, retry - 1
+                sendtoken, retries - 1
             )
 
-        logging.debug('AternosConnect received: %s', req.text[:65])
-        logging.info(
+        log.debug('AternosConnect received: %s', req.text[:65])
+        log.info(
             '%s completed with %s status',
             method, req.status_code
         )
 
         if req.status_code == 402:
             raise AternosPermissionError
```

### Comparing `python-aternos-2.1.3/python_aternos/aterrors.py` & `python-aternos-3.0.0/python_aternos/aterrors.py`

 * *Files identical despite different names*

### Comparing `python-aternos-2.1.3/python_aternos/atfile.py` & `python-aternos-3.0.0/python_aternos/atfile.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import enum
 
 from typing import Union
 from typing import TYPE_CHECKING
 
 import lxml.html
 
+from .atconnect import BASE_URL, AJAX_URL
 from .aterrors import FileError
 
 if TYPE_CHECKING:
     from .atserver import AternosServer
 
 
 class FileType(enum.IntEnum):
@@ -83,15 +84,15 @@
             raise RuntimeWarning(
                 'Creating files only available '
                 'inside directories'
             )
 
         name = name.strip().replace('/', '_')
         req = self.atserv.atserver_request(
-            'https://aternos.org/panel/ajax/files/create.php',
+            f'{AJAX_URL}/files/create.php',
             'POST', data={
                 'file': f'{self._path}/{name}',
                 'type': 'file'
                 if ftype == FileType.file
                 else 'directory'
             }
         )
@@ -110,15 +111,15 @@
         if not self._deleteable:
             raise RuntimeWarning(
                 'The file seems to be protected (undeleteable). '
                 'Always check it before calling delete()'
             )
 
         req = self.atserv.atserver_request(
-            'https://aternos.org/panel/ajax/delete.php',
+            f'{AJAX_URL}/delete.php',
             'POST', data={'file': self._path},
             sendtoken=True
         )
 
         if req.content == b'{"success":false}':
             raise FileError('Unable to delete the file')
 
@@ -136,15 +137,15 @@
         if not self._downloadable:
             raise RuntimeWarning(
                 'The file seems to be undownloadable. '
                 'Always check it before calling get_content()'
             )
 
         file = self.atserv.atserver_request(
-            'https://aternos.org/panel/ajax/files/download.php',
+            f'{AJAX_URL}/files/download.php',
             'GET', params={
                 'file': self._path
             }
         )
 
         if file.content == b'{"success":false}':
             raise FileError(
@@ -161,15 +162,15 @@
             value (bytes): New content
 
         Raises:
             FileError: If Aternos denied file saving
         """
 
         req = self.atserv.atserver_request(
-            'https://aternos.org/panel/ajax/save.php',
+            f'{AJAX_URL}/save.php',
             'POST', data={
                 'file': self._path,
                 'content': value
             }, sendtoken=True
         )
 
         if req.content == b'{"success":false}':
@@ -196,15 +197,15 @@
             raise RuntimeWarning(
                 'Use get_content() to download '
                 'a directory as a ZIP file!'
             )
 
         filepath = self._path.lstrip("/")
         editor = self.atserv.atserver_request(
-            f'https://aternos.org/files/{filepath}', 'GET'
+            f'{BASE_URL}/files/{filepath}', 'GET'
         )
         edittree = lxml.html.fromstring(editor.content)
         editblock = edittree.xpath('//div[@id="editor"]')
 
         if len(editblock) < 1:
             raise FileError(
                 'Unable to open editor. '
```

### Comparing `python-aternos-2.1.3/python_aternos/atfm.py` & `python-aternos-3.0.0/python_aternos/atfm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Exploring files in your server directory"""
 
 from typing import Union, Optional, Any, List
 from typing import TYPE_CHECKING
 
 import lxml.html
 
+from .atconnect import BASE_URL, AJAX_URL
 from .atfile import AternosFile, FileType
+
 if TYPE_CHECKING:
     from .atserver import AternosServer
 
 
 class FileManager:
 
     """Aternos file manager class
@@ -37,15 +39,15 @@
         Returns:
             List of atfile.AternosFile objects
         """
 
         path = path.lstrip('/')
 
         filesreq = self.atserv.atserver_request(
-            f'https://aternos.org/files/{path}', 'GET'
+            f'{BASE_URL}/files/{path}', 'GET'
         )
         filestree = lxml.html.fromstring(filesreq.content)
 
         fileslist = filestree.xpath(
             '//div[@class="file" or @class="file clickable"]'
         )
 
@@ -159,15 +161,15 @@
             path (str): Path to file including its filename
 
         Returns:
             File content
         """
 
         file = self.atserv.atserver_request(  # type: ignore
-            'https://aternos.org/panel/ajax/files/download.php'
+            f'{AJAX_URL}/files/download.php'
             'GET', params={
                 'file': path.replace('/', '%2F')
             }
         )
 
         return file.content
 
@@ -179,14 +181,14 @@
             world (str, optional): Name of world
 
         Returns:
             ZIP file content
         """
 
         resp = self.atserv.atserver_request(  # type: ignore
-            'https://aternos.org/panel/ajax/worlds/download.php'
+            f'{AJAX_URL}/worlds/download.php'
             'GET', params={
                 'world': world.replace('/', '%2F')
             }
         )
 
         return resp.content
```

### Comparing `python-aternos-2.1.3/python_aternos/atplayers.py` & `python-aternos-3.0.0/python_aternos/atplayers.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import enum
 
 from typing import List, Union
 from typing import TYPE_CHECKING
 
 import lxml.html
 
+from .atconnect import BASE_URL, AJAX_URL
 if TYPE_CHECKING:
     from .atserver import AternosServer
 
 
 class Lists(enum.Enum):
 
     """Players list type enum"""
@@ -45,16 +46,16 @@
         self.atserv = atserv
         self.lst = Lists(lst)
 
         # Fix for #30 issue
         # whl_je = whitelist for java
         # whl_be = whitelist for bedrock
         # whl = common whitelist
-        common_whl = (self.lst == Lists.whl)
-        bedrock = (atserv.is_bedrock)
+        common_whl = self.lst == Lists.whl
+        bedrock = atserv.is_bedrock
 
         if common_whl and bedrock:
             self.lst = Lists.whl_be
 
         self.players: List[str] = []
         self.parsed = False
 
@@ -69,15 +70,15 @@
             List of players' nicknames
         """
 
         if cache and self.parsed:
             return self.players
 
         listreq = self.atserv.atserver_request(
-            f'https://aternos.org/players/{self.lst.value}',
+            f'{BASE_URL}/players/{self.lst.value}',
             'GET'
         )
         listtree = lxml.html.fromstring(listreq.content)
         items = listtree.xpath(
             '//div[@class="list-item"]'
         )
 
@@ -94,15 +95,15 @@
         """Appends a player to the list by the nickname
 
         Args:
             name (str): Player's nickname
         """
 
         self.atserv.atserver_request(
-            'https://aternos.org/panel/ajax/players/add.php',
+            f'{AJAX_URL}/players/add.php',
             'POST', data={
                 'list': self.lst.value,
                 'name': name
             }, sendtoken=True
         )
 
         self.players.append(name)
@@ -111,15 +112,15 @@
         """Removes a player from the list by the nickname
 
         Args:
             name (str): Player's nickname
         """
 
         self.atserv.atserver_request(
-            'https://aternos.org/panel/ajax/players/remove.php',
+            f'{AJAX_URL}/players/remove.php',
             'POST', data={
                 'list': self.lst.value,
                 'name': name
             }, sendtoken=True
         )
 
         for i, j in enumerate(self.players):
```

### Comparing `python-aternos-2.1.3/python_aternos/atserver.py` & `python-aternos-3.0.0/python_aternos/atserver.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 """Aternos Minecraft server"""
 
-import enum
+import re
 import json
 
-from typing import Optional
-from typing import List, Dict, Any
-
-import requests
+import enum
+from typing import Any, Dict, List
+from functools import partial
 
+from .atconnect import BASE_URL, AJAX_URL
 from .atconnect import AternosConnect
-from .aterrors import ServerStartError
-from .atfm import FileManager
-from .atconf import AternosConfig
+from .atwss import AternosWss
+
 from .atplayers import PlayersList
 from .atplayers import Lists
-from .atwss import AternosWss
+
+from .atfm import FileManager
+from .atconf import AternosConfig
+
+from .aterrors import AternosError
+from .aterrors import ServerStartError
+
+
+SERVER_URL = f'{AJAX_URL}/server'
+status_re = re.compile(
+    r'<script>\s*var lastStatus\s*?=\s*?(\{.+?\});?\s*<\/script>'
+)
 
 
 class Edition(enum.IntEnum):
 
     """Server edition type enum (java, bedrock)"""
 
     java = 0
@@ -42,44 +52,57 @@
     error = 7
 
     preparing = 10
     confirm = 10
 
 
 class AternosServer:
-
     """Class for controlling your Aternos Minecraft server"""
 
     def __init__(
             self, servid: str,
             atconn: AternosConnect,
-            reqinfo: bool = True) -> None:
+            autofetch: bool = False) -> None:
         """Class for controlling your Aternos Minecraft server
 
         Args:
             servid (str): Unique server IDentifier
             atconn (AternosConnect):
                 AternosConnect instance with initialized Aternos session
-            reqinfo (bool, optional): Automatically call
+            autofetch (bool, optional): Automatically call
                 `fetch()` to get all info
         """
 
         self.servid = servid
         self.atconn = atconn
-        if reqinfo:
+
+        self._info: Dict[str, Any] = {}
+
+        self.atserver_request = partial(
+            self.atconn.request_cloudflare,
+            reqcookies={
+                'ATERNOS_SERVER': self.servid,
+            }
+        )
+
+        if autofetch:
             self.fetch()
 
     def fetch(self) -> None:
-        """Send a request to Aternos API to get all server info"""
+        """Get all server info"""
 
-        servreq = self.atserver_request(
-            'https://aternos.org/panel/ajax/status.php',
-            'GET', sendtoken=True
+        page = self.atserver_request(
+            f'{BASE_URL}/server', 'GET'
         )
-        self._info = json.loads(servreq.content)
+        match = status_re.search(page.text)
+
+        if match is None:
+            raise AternosError('Unable to parse lastStatus object')
+
+        self._info = json.loads(match[1])
 
     def wss(self, autoconfirm: bool = False) -> AternosWss:
         """Returns AternosWss instance for
         listening server streams in real-time
 
         Args:
             autoconfirm (bool, optional):
@@ -92,33 +115,40 @@
         """
 
         return AternosWss(self, autoconfirm)
 
     def start(
             self,
             headstart: bool = False,
+            access_credits: bool = False,
             accepteula: bool = True) -> None:
         """Starts a server
 
         Args:
             headstart (bool, optional): Start a server in
                 the headstart mode which allows
                 you to skip all queue
+            access_credits (bool, optional):
+                Some new parameter in Aternos API,
+                I don't know what it is
             accepteula (bool, optional):
                 Automatically accept the Mojang EULA
 
         Raises:
             ServerStartError: When Aternos
                 is unable to start the server
         """
 
         startreq = self.atserver_request(
-            'https://aternos.org/panel/ajax/start.php',
-            'GET', params={'headstart': int(headstart)},
-            sendtoken=True
+            f'{SERVER_URL}/start',
+            'GET', params={
+                'headstart': int(headstart),
+                'access-credits': int(access_credits),
+            },
+            sendtoken=True,
         )
         startresult = startreq.json()
 
         if startresult['success']:
             return
 
         error = startresult['error']
@@ -130,48 +160,48 @@
 
         raise ServerStartError(error)
 
     def confirm(self) -> None:
         """Confirms server launching"""
 
         self.atserver_request(
-            'https://aternos.org/panel/ajax/confirm.php',
-            'GET', sendtoken=True
+            f'{SERVER_URL}/confirm',
+            'GET', sendtoken=True,
         )
 
     def stop(self) -> None:
         """Stops the server"""
 
         self.atserver_request(
-            'https://aternos.org/panel/ajax/stop.php',
-            'GET', sendtoken=True
+            f'{SERVER_URL}/stop',
+            'GET', sendtoken=True,
         )
 
     def cancel(self) -> None:
         """Cancels server launching"""
 
         self.atserver_request(
-            'https://aternos.org/panel/ajax/cancel.php',
-            'GET', sendtoken=True
+            f'{SERVER_URL}/cancel',
+            'GET', sendtoken=True,
         )
 
     def restart(self) -> None:
         """Restarts the server"""
 
         self.atserver_request(
-            'https://aternos.org/panel/ajax/restart.php',
-            'GET', sendtoken=True
+            f'{SERVER_URL}/restart',
+            'GET', sendtoken=True,
         )
 
     def eula(self) -> None:
-        """Accepts the Mojang EULA"""
+        """Sends a request to accept the Mojang EULA"""
 
         self.atserver_request(
-            'https://aternos.org/panel/ajax/eula.php',
-            'GET', sendtoken=True
+            f'{SERVER_URL}/accept-eula',
+            'GET', sendtoken=True,
         )
 
     def files(self) -> FileManager:
         """Returns FileManager instance
         for file operations
 
         Returns:
@@ -201,109 +231,77 @@
 
         Returns:
             PlayersList object
         """
 
         return PlayersList(lst, self)
 
-    def atserver_request(
-            self, url: str, method: str,
-            params: Optional[Dict[Any, Any]] = None,
-            data: Optional[Dict[Any, Any]] = None,
-            headers: Optional[Dict[Any, Any]] = None,
-            sendtoken: bool = False) -> requests.Response:
-        """Sends a request to Aternos API
-        with server IDenitfier parameter
+    def set_subdomain(self, value: str) -> None:
+        """Set a new subdomain for your server
+        (the part before `.aternos.me`)
 
         Args:
-            url (str): Request URL
-            method (str): Request method, must be GET or POST
-            params (Optional[Dict[Any, Any]], optional): URL parameters
-            data (Optional[Dict[Any, Any]], optional): POST request data,
-                if the method is GET, this dict
-                will be combined with params
-            headers (Optional[Dict[Any, Any]], optional): Custom headers
-            sendtoken (bool, optional): If the ajax and SEC token should be sent
-
-        Returns:
-            API response
-        """
-
-        return self.atconn.request_cloudflare(
-            url=url, method=method,
-            params=params, data=data,
-            headers=headers,
-            reqcookies={
-                'ATERNOS_SERVER': self.servid
-            },
-            sendtoken=sendtoken
+            value (str): Subdomain
+        """
+
+        self.atserver_request(
+            f'{SERVER_URL}/options/set-subdomain',
+            'GET', params={'subdomain': value},
+            sendtoken=True,
+        )
+
+    def set_motd(self, value: str) -> None:
+        """Set new Message of the Day
+        (shown below the name in the Minecraft servers list).
+        Formatting with "paragraph sign + code" is supported,
+        see https://minecraft.tools/color-code.php
+
+        Args:
+            value (str): MOTD
+        """
+
+        self.atserver_request(
+            f'{SERVER_URL}/options/set-motd',
+            'POST', data={'motd': value},
+            sendtoken=True,
         )
 
     @property
     def subdomain(self) -> str:
-        """Server subdomain
-        (the part of domain before `.aternos.me`)
+        """Get the server subdomain
+        (the part before `.aternos.me`)
 
         Returns:
             Subdomain
         """
 
         atdomain = self.domain
         return atdomain[:atdomain.find('.')]
 
-    @subdomain.setter
-    def subdomain(self, value: str) -> None:
-        """Set a new subdomain for your server
-
-        Args:
-            value (str): Subdomain
-        """
-
-        self.atserver_request(
-            'https://aternos.org/panel/ajax/options/subdomain.php',
-            'GET', params={'subdomain': value},
-            sendtoken=True
-        )
-
     @property
     def motd(self) -> str:
-        """Server message of the day
-        which is shown below its name
-        in the Minecraft servers list
+        """Get the server message of the day
+        (shown below its name in Minecraft servers list)
 
         Returns:
             MOTD
         """
 
         return self._info['motd']
 
-    @motd.setter
-    def motd(self, value: str) -> None:
-        """Set a new message of the day
-
-        Args:
-            value (str): New MOTD
-        """
-
-        self.atserver_request(
-            'https://aternos.org/panel/ajax/options/motd.php',
-            'POST', data={'motd': value},
-            sendtoken=True
-        )
-
     @property
     def address(self) -> str:
         """Full server address
         including domain and port
 
         Returns:
             Server address
         """
 
-        return self._info['displayAddress']
+        return f'{self.domain}:{self.port}'
 
     @property
     def domain(self) -> str:
         """Server domain (e.g. `test.aternos.me`).
         In other words, address without port number
 
         Returns:
@@ -371,19 +369,19 @@
             Software version
         """
 
         return self._info['version']
 
     @property
     def css_class(self) -> str:
-        """CSS class for
-        server status block
-        on official web site
-        (offline, loading,
-        loading starting, queueing)
+        """CSS class for the server status element
+        on official web site: offline, online, loading, etc.
+        See https://aternos.dc09.ru/howto/server/#server-info
+
+        In most cases you need `AternosServer.status` instead of this
 
         Returns:
             CSS class
         """
 
         return self._info['class']
 
@@ -446,7 +444,19 @@
         """Server used RAM in MB
 
         Returns:
             Used RAM
         """
 
         return int(self._info['ram'])
+
+    @property
+    def countdown(self) -> int:
+        """Server stop countdown
+        in seconds
+
+        Returns:
+            Stop countdown
+        """
+
+        value = self._info['countdown']
+        return int(value or -1)
```

### Comparing `python-aternos-2.1.3/python_aternos/atwss.py` & `python-aternos-3.0.0/python_aternos/atwss.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """Connects to Aternos WebSocket API
 for real-time information"""
 
 import enum
 import json
 import asyncio
-import logging
 
 from typing import Iterable
 from typing import Union, Any
 from typing import Tuple, List, Dict
 from typing import Callable, Coroutine
 from typing import TYPE_CHECKING
 
 import websockets
 
+from .atlog import log
 from .atconnect import REQUA
+
 if TYPE_CHECKING:
     from .atserver import AternosServer
 
+
 OneArgT = Callable[[Any], Coroutine[Any, Any, None]]
 TwoArgT = Callable[[Any, Tuple[Any, ...]], Coroutine[Any, Any, None]]
 FunctionT = Union[OneArgT, TwoArgT]
 ArgsTuple = Tuple[FunctionT, Tuple[Any, ...]]
 
 
 class Streams(enum.Enum):
@@ -151,16 +153,16 @@
             Args:
                 msg (Dict[str, Any]): Server info dictionary
             """
 
             if not self.autoconfirm:
                 return
 
-            in_queue = (msg['class'] == 'queueing')
-            pending = (msg['queue']['pending'] == 'pending')
+            in_queue = msg['class'] == 'queueing'
+            pending = msg['queue']['pending'] == 'pending'
             confirmation = in_queue and pending
 
             if confirmation and not self.confirmed:
                 await self.confirm()
 
         @self.wssreceiver(Streams.status)
         async def streamsfunc(msg: Dict[str, Any]) -> None:
@@ -192,15 +194,15 @@
                         continue
 
                     # If the handlers list is empty
                     if not self.recv.get(strm):
                         continue
 
                     if strm.stream:
-                        logging.debug('Requesting %s stream', strm.stream)
+                        log.debug('Requesting %s stream', strm.stream)
                         await self.send({
                             'stream': strm.stream,
                             'type': 'start'
                         })
 
         await self.wssworker()
 
@@ -219,15 +221,15 @@
 
         Args:
             obj (Union[Dict[str, Any],str]):
                 Message, may be a string or a dict
         """
 
         if self.socket is None:
-            logging.warning('Did you forget to call socket.connect?')
+            log.warning('Did you forget to call socket.connect?')
             await self.connect()
 
         assert self.socket is not None
 
         if isinstance(obj, dict):
             obj = json.dumps(obj)
```

### Comparing `python-aternos-2.1.3/python_aternos.egg-info/PKG-INFO` & `python-aternos-3.0.0/python_aternos.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-aternos
-Version: 2.1.3
+Version: 3.0.0
 Summary: An unofficial Aternos API
 Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09)
 Author-email: aacd0709@mail.ru
 Project-URL: Documentation, https://python-aternos.codeberg.page
 Project-URL: GitHub, https://github.com/DarkCat09/python-aternos
 Project-URL: Bug Tracker, https://github.com/DarkCat09/python-aternos/issues
@@ -49,22 +49,22 @@
 </div>
 
 An unofficial Aternos API written in Python.  
 It uses [aternos](https://aternos.org/)' private API and html parsing.
 
 Python Aternos supports:
 
- - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value.
- - Saving session to the file and restoring.
- - Changing username, email and password.
- - Parsing Minecraft servers list.
- - Parsing server info by its ID.
- - Starting/stoping server, restarting, confirming/cancelling launch.
- - Updating server info in real-time (view WebSocket API).
- - Changing server subdomain and MOTD (message-of-the-day).
+ - Logging in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
+ - Saving session to the file and restoring
+ - Changing username, email and password
+ - Parsing Minecraft servers list
+ - Parsing server info by its ID
+ - Starting/stoping server, restarting, confirming/cancelling launch
+ - Updating server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/websocket))
+ - Changing server subdomain and MOTD (message-of-the-day)
  - Managing files, settings, players (whitelist, operators, etc.)
 
 > **Warning**
 >
 > According to the Aternos' [Terms of Service §5.2e](https://aternos.gmbh/en/aternos/terms#:~:text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
 > you must not use any software or APIs for automated access,
 > beacuse they don't receive money from advertisting in this case.
@@ -93,79 +93,92 @@
 $ git clone https://github.com/DarkCat09/python-aternos.git
 $ cd python-aternos
 $ pip install -e .
 ```
 
 ## Usage
 To use Aternos API in your Python script, import it
-and login with your username and password or MD5.
+and login with your username and password or its MD5 hash.
 
 Then request the servers list using `list_servers()`.  
 You can start/stop your Aternos server, calling `start()` or `stop()`.
 
 Here is an example how to use the API:
 ```python
 # Import
 from python_aternos import Client
 
+# Create object
+aternos = Client()
+
 # Log in
-aternos = Client.from_credentials('example', 'test123')
+# with username and password
+aternos.login('example', 'test123')
 # ----OR----
-aternos = Client.from_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
+# with username and MD5 hashed password
+aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5')
 # ----OR----
-aternos = Client.restore_session()
+# with session cookie
+aternos.login_with_session('ATERNOS_SESSION cookie value')
 
-# Returns AternosServer list
+# Get servers list
 servs = aternos.list_servers()
 
-# Get the first server by the 0 index
+# Get the first server
 myserv = servs[0]
 
 # Start
 myserv.start()
 # Stop
 myserv.stop()
 
 # You can also find server by IP
 testserv = None
 for serv in servs:
     if serv.address == 'test.aternos.org':
         testserv = serv
 
 if testserv is not None:
-    # Prints a server softaware and its version
+    # Prints the server software and its version
     # (for example, "Vanilla 1.12.2")
     print(testserv.software, testserv.version)
     # Starts server
     testserv.start()
 ```
 
 ## [More examples](https://github.com/DarkCat09/python-aternos/tree/main/examples)
 
-## [Documentation](https://python-aternos.codeberg.page/)
+## [Documentation](https://aternos.dc09.ru)
 
-## [How-To Guide](https://python-aternos.codeberg.page/howto/auth)
+## [How-To Guide](https://aternos.dc09.ru/howto/auth)
 
 ## Changelog
 |Version|Description |
 |:-----:|:-----------|
-|v0.1|The first release.|
-|v0.2|Fixed import problem.|
 |v0.3|Implemented files API, added typization.|
 |v0.4|Implemented configuration API, some bugfixes.|
 |v0.5|The API was updated corresponding to new Aternos security methods. Huge thanks to [lusm554](https://github.com/lusm554).|
 |**v0.6/v1.0.0**|Code refactoring, websockets API and session saving to prevent detecting automation access.|
 |v1.0.x|Lots of bugfixes, changed versioning (SemVer).|
 |v1.1.x|Documentation, unit tests, pylint, bugfixes, changes in atwss.|
 |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/DarkCat09/python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS parser.|
 |v2.0.x|Documentation, automatically saving/restoring session, improvements in Files API.|
-|v2.1.x|Fixes in websockets API, atconnect. Supported captcha solving services (view [#52](https://github.com/DarkCat09/python-aternos/issues/52)).|
-|**v2.2.x**|Using Node.js as a JS interpreter if it's installed.|
-|v3.0.x|Full implementation of config and software API.|
-|v3.1.x|Shared access API and Google Drive backups.|
+|v2.1.x|Fixes in websockets API, atconnect (including cookie refreshing fix). Support for captcha solving services (view [#52](https://github.com/DarkCat09/python-aternos/issues/52)).|
+|v2.2.x|Node.JS interpreter support.|
+|v3.0.0|Partially rewritten, API updates.|
+|v3.1.x|Full implementation of config API.|
+|v3.2.x|Shared access API and maybe Google Drive backups.|
+
+## Reversed API Specification
+Private Aternos API requests were captured into
+[this HAR file](https://github.com/DarkCat09/python-aternos/blob/main/aternos.har)
+and were imported to
+[a Postman Workspace](https://www.postman.com/darkcat09/workspace/aternos-api).  
+You can use both resources to explore the API.  
+Any help with improving this library is welcome.
 
 ## License
 [License Notice:](https://github.com/DarkCat09/python-aternos/blob/main/NOTICE)
 ```
 Copyright 2021-2022 All contributors
 
 Licensed under the Apache License, Version 2.0 (the "License");
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: python-aternos Version: 2.1.3 Summary: An
+Metadata-Version: 2.1 Name: python-aternos Version: 3.0.0 Summary: An
 unofficial Aternos API Home-page: https://github.com/DarkCat09/python-aternos
 Author: Chechkenev Andrey (@DarkCat09) Author-email: aacd0709@mail.ru Project-
 URL: Documentation, https://python-aternos.codeberg.page Project-URL: GitHub,
 https://github.com/DarkCat09/python-aternos Project-URL: Bug Tracker, https://
 github.com/DarkCat09/python-aternos/issues Classifier: Development Status :: 4
 - Beta Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
@@ -17,67 +17,74 @@
                              [Python Aternos Logo]
                                 Python Aternos
 [https://img.shields.io/pypi/v/python-aternos] [https://img.shields.io/pypi/l/
  python-aternos] [https://img.shields.io/github/last-commit/DarkCat09/python-
    aternos] [https://img.shields.io/github/issues/DarkCat09/python-aternos]
 An unofficial Aternos API written in Python. It uses [aternos](https://
 aternos.org/)' private API and html parsing. Python Aternos supports: - Logging
-in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie
-value. - Saving session to the file and restoring. - Changing username, email
-and password. - Parsing Minecraft servers list. - Parsing server info by its
-ID. - Starting/stoping server, restarting, confirming/cancelling launch. -
-Updating server info in real-time (view WebSocket API). - Changing server
-subdomain and MOTD (message-of-the-day). - Managing files, settings, players
-(whitelist, operators, etc.) > **Warning** > > According to the Aternos' [Terms
-of Service Â§5.2e](https://aternos.gmbh/en/aternos/terms#:~:
+in to account with password (plain or hashed) or `ATERNOS_SESSION` cookie value
+- Saving session to the file and restoring - Changing username, email and
+password - Parsing Minecraft servers list - Parsing server info by its ID -
+Starting/stoping server, restarting, confirming/cancelling launch - Updating
+server info in real-time (see [WebSocket API](https://aternos.dc09.ru/howto/
+websocket)) - Changing server subdomain and MOTD (message-of-the-day) -
+Managing files, settings, players (whitelist, operators, etc.) > **Warning** >
+> According to the Aternos' [Terms of Service Â§5.2e](https://aternos.gmbh/en/
+aternos/terms#:~:
 text=Automatically%20accessing%20our%20website%20or%20automating%20actions%20on%20our%20website.),
 > you must not use any software or APIs for automated access, > beacuse they
 don't receive money from advertisting in this case. > > I always try to hide
 automated python-aternos requests > using browser-specific headers/cookies, >
 but you should make backups to restore your world > if Aternos detects
 violation of ToS and bans your account > (view issues [#16](https://github.com/
 DarkCat09/python-aternos/issues/16) > and [#46](https://github.com/DarkCat09/
 python-aternos/issues/46)). ## Install ### Common ```bash $ pip install python-
 aternos ``` > **Note** for Windows users > > Install `lxml` package from [here]
 (https://www.lfd.uci.edu/~gohlke/pythonlibs/#lxml) > if you have problems with
 it, and then execute: > `pip install --no-deps python-aternos` ### Development
 ```bash $ git clone https://github.com/DarkCat09/python-aternos.git $ cd
 python-aternos $ pip install -e . ``` ## Usage To use Aternos API in your
-Python script, import it and login with your username and password or MD5. Then
-request the servers list using `list_servers()`. You can start/stop your
-Aternos server, calling `start()` or `stop()`. Here is an example how to use
-the API: ```python # Import from python_aternos import Client # Log in aternos
-= Client.from_credentials('example', 'test123') # ----OR---- aternos =
-Client.from_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---
-- aternos = Client.restore_session() # Returns AternosServer list servs =
-aternos.list_servers() # Get the first server by the 0 index myserv = servs[0]
-# Start myserv.start() # Stop myserv.stop() # You can also find server by IP
-testserv = None for serv in servs: if serv.address == 'test.aternos.org':
-testserv = serv if testserv is not None: # Prints a server softaware and its
-version # (for example, "Vanilla 1.12.2") print(testserv.software,
-testserv.version) # Starts server testserv.start() ``` ## [More examples]
-(https://github.com/DarkCat09/python-aternos/tree/main/examples) ##
-[Documentation](https://python-aternos.codeberg.page/) ## [How-To Guide](https:
-//python-aternos.codeberg.page/howto/auth) ## Changelog |Version|Description |
-|:-----:|:-----------| |v0.1|The first release.| |v0.2|Fixed import problem.|
-|v0.3|Implemented files API, added typization.| |v0.4|Implemented configuration
-API, some bugfixes.| |v0.5|The API was updated corresponding to new Aternos
-security methods. Huge thanks to [lusm554](https://github.com/lusm554).|
-|**v0.6/v1.0.0**|Code refactoring, websockets API and session saving to prevent
-detecting automation access.| |v1.0.x|Lots of bugfixes, changed versioning
-(SemVer).| |v1.1.x|Documentation, unit tests, pylint, bugfixes, changes in
-atwss.| |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/DarkCat09/
-python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS parser.|
-|v2.0.x|Documentation, automatically saving/restoring session, improvements in
-Files API.| |v2.1.x|Fixes in websockets API, atconnect. Supported captcha
-solving services (view [#52](https://github.com/DarkCat09/python-aternos/
-issues/52)).| |**v2.2.x**|Using Node.js as a JS interpreter if it's installed.|
-|v3.0.x|Full implementation of config and software API.| |v3.1.x|Shared access
-API and Google Drive backups.| ## License [License Notice:](https://github.com/
-DarkCat09/python-aternos/blob/main/NOTICE) ``` Copyright 2021-2022 All
-contributors Licensed under the Apache License, Version 2.0 (the "License");
-you may not use this file except in compliance with the License. You may obtain
-a copy of the License at http://www.apache.org/licenses/LICENSE-2.0 Unless
-required by applicable law or agreed to in writing, software distributed under
-the License is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR
-CONDITIONS OF ANY KIND, either express or implied. See the License for the
-specific language governing permissions and limitations under the License. ```
+Python script, import it and login with your username and password or its MD5
+hash. Then request the servers list using `list_servers()`. You can start/stop
+your Aternos server, calling `start()` or `stop()`. Here is an example how to
+use the API: ```python # Import from python_aternos import Client # Create
+object aternos = Client() # Log in # with username and password aternos.login
+('example', 'test123') # ----OR---- # with username and MD5 hashed password
+aternos.login_hashed('example', 'cc03e747a6afbbcbf8be7668acfebee5') # ----OR---
+- # with session cookie aternos.login_with_session('ATERNOS_SESSION cookie
+value') # Get servers list servs = aternos.list_servers() # Get the first
+server myserv = servs[0] # Start myserv.start() # Stop myserv.stop() # You can
+also find server by IP testserv = None for serv in servs: if serv.address ==
+'test.aternos.org': testserv = serv if testserv is not None: # Prints the
+server software and its version # (for example, "Vanilla 1.12.2") print
+(testserv.software, testserv.version) # Starts server testserv.start() ``` ##
+[More examples](https://github.com/DarkCat09/python-aternos/tree/main/examples)
+## [Documentation](https://aternos.dc09.ru) ## [How-To Guide](https://
+aternos.dc09.ru/howto/auth) ## Changelog |Version|Description | |:-----:|:-----
+------| |v0.3|Implemented files API, added typization.| |v0.4|Implemented
+configuration API, some bugfixes.| |v0.5|The API was updated corresponding to
+new Aternos security methods. Huge thanks to [lusm554](https://github.com/
+lusm554).| |**v0.6/v1.0.0**|Code refactoring, websockets API and session saving
+to prevent detecting automation access.| |v1.0.x|Lots of bugfixes, changed
+versioning (SemVer).| |v1.1.x|Documentation, unit tests, pylint, bugfixes,
+changes in atwss.| |**v1.1.2/v2.0.0**|Solution for [#25](https://github.com/
+DarkCat09/python-aternos/issues/25) (Cloudflare bypassing), bugfixes in JS
+parser.| |v2.0.x|Documentation, automatically saving/restoring session,
+improvements in Files API.| |v2.1.x|Fixes in websockets API, atconnect
+(including cookie refreshing fix). Support for captcha solving services (view
+[#52](https://github.com/DarkCat09/python-aternos/issues/52)).| |v2.2.x|Node.JS
+interpreter support.| |v3.0.0|Partially rewritten, API updates.| |v3.1.x|Full
+implementation of config API.| |v3.2.x|Shared access API and maybe Google Drive
+backups.| ## Reversed API Specification Private Aternos API requests were
+captured into [this HAR file](https://github.com/DarkCat09/python-aternos/blob/
+main/aternos.har) and were imported to [a Postman Workspace](https://
+www.postman.com/darkcat09/workspace/aternos-api). You can use both resources to
+explore the API. Any help with improving this library is welcome. ## License
+[License Notice:](https://github.com/DarkCat09/python-aternos/blob/main/NOTICE)
+``` Copyright 2021-2022 All contributors Licensed under the Apache License,
+Version 2.0 (the "License"); you may not use this file except in compliance
+with the License. You may obtain a copy of the License at http://
+www.apache.org/licenses/LICENSE-2.0 Unless required by applicable law or agreed
+to in writing, software distributed under the License is distributed on an "AS
+IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+implied. See the License for the specific language governing permissions and
+limitations under the License. ```
```

### Comparing `python-aternos-2.1.3/setup.py` & `python-aternos-3.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'rt') as readme:
     long_description = readme.read()
 
 setuptools.setup(
     name='python-aternos',
-    version='2.1.3',
+    version='3.0.0',
     author='Chechkenev Andrey (@DarkCat09)',
     author_email='aacd0709@mail.ru',
     description='An unofficial Aternos API',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/DarkCat09/python-aternos',
     project_urls={
@@ -38,8 +38,9 @@
         'cloudscraper>=1.2.60',
         'js2py>=0.71',
         'websockets>=10.1',
         'regex>=2022.3.15',
     ],
     packages=['python_aternos'],
     python_requires=">=3.7",
+    include_package_data=True,
 )
```


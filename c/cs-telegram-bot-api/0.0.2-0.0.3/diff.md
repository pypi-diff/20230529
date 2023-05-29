# Comparing `tmp/cs-telegram-bot-api-0.0.2.tar.gz` & `tmp/cs-telegram-bot-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-telegram-bot-api-0.0.2.tar", last modified: Mon May 29 07:00:14 2023, max compression
+gzip compressed data, was "cs-telegram-bot-api-0.0.3.tar", last modified: Mon May 29 07:03:29 2023, max compression
```

## Comparing `cs-telegram-bot-api-0.0.2.tar` & `cs-telegram-bot-api-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 07:00:14.385692 cs-telegram-bot-api-0.0.2/
--rw-rw-rw-   0        0        0      501 2023-05-29 07:00:14.377521 cs-telegram-bot-api-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1063 2023-05-28 19:29:01.000000 cs-telegram-bot-api-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 07:00:14.297910 cs-telegram-bot-api-0.0.2/cs-telegram-bot-api/
--rw-rw-rw-   0        0        0       31 2023-05-29 06:59:14.000000 cs-telegram-bot-api-0.0.2/cs-telegram-bot-api/__init__.py
--rw-rw-rw-   0        0        0     2089 2023-05-28 19:25:37.000000 cs-telegram-bot-api-0.0.2/cs-telegram-bot-api/api.py
-drwxrwxrwx   0        0        0        0 2023-05-29 07:00:14.377521 cs-telegram-bot-api-0.0.2/cs_telegram_bot_api.egg-info/
--rw-rw-rw-   0        0        0      501 2023-05-29 07:00:14.000000 cs-telegram-bot-api-0.0.2/cs_telegram_bot_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      291 2023-05-29 07:00:14.000000 cs-telegram-bot-api-0.0.2/cs_telegram_bot_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 07:00:14.000000 cs-telegram-bot-api-0.0.2/cs_telegram_bot_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-29 07:00:14.000000 cs-telegram-bot-api-0.0.2/cs_telegram_bot_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-29 07:00:14.000000 cs-telegram-bot-api-0.0.2/cs_telegram_bot_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-29 07:00:14.386515 cs-telegram-bot-api-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1006 2023-05-29 06:59:48.000000 cs-telegram-bot-api-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:03:29.271723 cs-telegram-bot-api-0.0.3/
+-rw-rw-rw-   0        0        0      501 2023-05-29 07:03:29.271723 cs-telegram-bot-api-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1063 2023-05-28 19:29:01.000000 cs-telegram-bot-api-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 07:03:29.230859 cs-telegram-bot-api-0.0.3/cs_telegram_bot/
+-rw-rw-rw-   0        0        0       31 2023-05-29 06:59:14.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot/__init__.py
+-rw-rw-rw-   0        0        0     2089 2023-05-28 19:25:37.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot/api.py
+drwxrwxrwx   0        0        0        0 2023-05-29 07:03:29.263704 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/
+-rw-rw-rw-   0        0        0      501 2023-05-29 07:03:29.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      283 2023-05-29 07:03:29.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 07:03:29.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-29 07:03:29.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-29 07:03:29.000000 cs-telegram-bot-api-0.0.3/cs_telegram_bot_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-29 07:03:29.271723 cs-telegram-bot-api-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1006 2023-05-29 07:03:06.000000 cs-telegram-bot-api-0.0.3/setup.py
```

### Comparing `cs-telegram-bot-api-0.0.2/README.md` & `cs-telegram-bot-api-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cs-telegram-bot-api-0.0.2/cs-telegram-bot-api/api.py` & `cs-telegram-bot-api-0.0.3/cs_telegram_bot/api.py`

 * *Files identical despite different names*

### Comparing `cs-telegram-bot-api-0.0.2/setup.py` & `cs-telegram-bot-api-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'Telegram Bot API Wrapper'
 LONG_DESCRIPTION = 'A Python module for interacting with the Telegram Bot API.'
 
 # Setting up
 setup(
     name="cs-telegram-bot-api",
     version=VERSION,
```


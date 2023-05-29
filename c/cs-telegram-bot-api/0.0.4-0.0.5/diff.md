# Comparing `tmp/cs-telegram-bot-api-0.0.4.tar.gz` & `tmp/cs-telegram-bot-api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs-telegram-bot-api-0.0.4.tar", last modified: Mon May 29 19:06:17 2023, max compression
+gzip compressed data, was "cs-telegram-bot-api-0.0.5.tar", last modified: Mon May 29 19:13:12 2023, max compression
```

## Comparing `cs-telegram-bot-api-0.0.4.tar` & `cs-telegram-bot-api-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:06:17.545194 cs-telegram-bot-api-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 19:06:17.541194 cs-telegram-bot-api-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-29 19:06:05.000000 cs-telegram-bot-api-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:06:17.541194 cs-telegram-bot-api-0.0.4/cs_telegram_bot/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-29 19:06:05.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-29 19:06:05.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:06:17.541194 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 19:06:17.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-29 19:06:17.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:06:17.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 19:06:17.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 19:06:17.000000 cs-telegram-bot-api-0.0.4/cs_telegram_bot_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:06:17.545194 cs-telegram-bot-api-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-29 19:06:05.000000 cs-telegram-bot-api-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:13:12.281933 cs-telegram-bot-api-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 19:13:12.281933 cs-telegram-bot-api-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-29 19:13:00.000000 cs-telegram-bot-api-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:13:12.281933 cs-telegram-bot-api-0.0.5/cs_telegram_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-29 19:13:00.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-29 19:13:00.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 19:13:12.281933 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-29 19:13:12.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-29 19:13:12.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 19:13:12.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-29 19:13:12.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-29 19:13:12.000000 cs-telegram-bot-api-0.0.5/cs_telegram_bot_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 19:13:12.281933 cs-telegram-bot-api-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-29 19:13:00.000000 cs-telegram-bot-api-0.0.5/setup.py
```

### Comparing `cs-telegram-bot-api-0.0.4/README.md` & `cs-telegram-bot-api-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cs-telegram-bot-api-0.0.4/cs_telegram_bot/api.py` & `cs-telegram-bot-api-0.0.5/cs_telegram_bot/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -65,9 +65,7 @@
 
         # If the API call was successful, the response will contain
         # the sent message in the "result" field
         result = response.json()["result"]
         print(message)
         return result
 
-
-if __name__ == "__main__":
```

### Comparing `cs-telegram-bot-api-0.0.4/setup.py` & `cs-telegram-bot-api-0.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Telegram Bot API Wrapper'
 LONG_DESCRIPTION = 'A Python module for interacting with the Telegram Bot API.'
 
 # Setting up
 setup(
     name="cs-telegram-bot-api",
     version=VERSION,
```


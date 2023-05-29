# Comparing `tmp/optimuslib-0.0.5.tar.gz` & `tmp/optimuslib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimuslib-0.0.5.tar", max compression
+gzip compressed data, was "optimuslib-0.0.6.tar", max compression
```

## Comparing `optimuslib-0.0.5.tar` & `optimuslib-0.0.6.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0    29675 2023-05-29 13:07:32.126990 optimuslib-0.0.5/optimuslib/optimuslib.py
--rw-r--r--   0        0        0      343 2023-05-29 13:13:40.253272 optimuslib-0.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.5/README.md
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 optimuslib-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-29 13:32:12.741001 optimuslib-0.0.6/optimuslib/__init__.py
+-rw-r--r--   0        0        0    30853 2023-05-29 13:43:24.695064 optimuslib-0.0.6/optimuslib/optimuslib.py
+-rw-r--r--   0        0        0      343 2023-05-29 13:44:02.285293 optimuslib-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.6/README.md
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 optimuslib-0.0.6/PKG-INFO
```

### Comparing `optimuslib-0.0.5/optimuslib/optimuslib.py` & `optimuslib-0.0.6/optimuslib/optimuslib.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,22 @@
 
 ### add any filename.py to .gitignore and remove it from cache using below command
 # git rm -r --cached .
 # git add .
 # git commit -m "untrack files contained in the .gitignore file"
 
 #########################################################
+# Local testing on 
+# C:\Users\Admin\AppData\Local\Programs\Python\Python311\Lib\site-packages\optimuslib
+
+### import code
+# import optimuslib
+# from optimuslib.optimuslib import log
+# optimuslib = optimuslib.optimuslib
+
 ### import libraries to file using import sys 
 # import sys
 # import os
 # try:
     # sys.path.append(r'C:/Users/NanwaniS/OneDrive - HP Inc/Python Projects/python-automation-scripts/libraries')
     # print('Fetching libraries from default libraries folder')
     # import optimuslib
@@ -447,15 +455,32 @@
 ########### TELEGRAM BOT NOTIFICATION - BOT DETAILS ##############
 def getTelegramBotInfo(botToken):
     log.info('Fetching BOT Information')
     url = 'https://api.telegram.org/bot'+botToken+'/getMe'
     response = sendRequest('get', url)
     responseJson = response.result().json()
     if responseJson['ok']==True:
-        return True
+        if responseJson['result']:
+            id = responseJson['result']['id']
+            is_bot = responseJson['result']['is_bot']
+            first_name = responseJson['result']['first_name']
+            username = responseJson['result']['username']
+            can_join_groups = responseJson['result']['can_join_groups']
+            can_read_all_group_messages = responseJson['result']['can_read_all_group_messages']
+            supports_inline_queries = responseJson['result']['supports_inline_queries']
+            getVarInfo('id',id)
+            getVarInfo('is_bot',is_bot)
+            getVarInfo('first_name',first_name)
+            getVarInfo('username',username)
+            getVarInfo('can_join_groups',can_join_groups)
+            getVarInfo('can_read_all_group_messages',can_read_all_group_messages)
+            getVarInfo('supports_inline_queries',supports_inline_queries)
+            return True
+        else:
+            return False
     else:
         getVarInfo('responseJson',responseJson)
         return False
 
 ########### TELEGRAM BOT NOTIFICATION - FETCH RECEIVED MESSAGES ##############
 def getTelegramBotUpdates(botToken, update_id):
     log.info('Checking new messages...')
```


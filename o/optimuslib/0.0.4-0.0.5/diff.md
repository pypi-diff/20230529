# Comparing `tmp/optimuslib-0.0.4.tar.gz` & `tmp/optimuslib-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimuslib-0.0.4.tar", max compression
+gzip compressed data, was "optimuslib-0.0.5.tar", max compression
```

## Comparing `optimuslib-0.0.4.tar` & `optimuslib-0.0.5.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.4/optimuslib/__init__.py
--rw-r--r--   0        0        0    29675 2023-05-29 12:48:48.451666 optimuslib-0.0.4/optimuslib/optimuslib.py
--rw-r--r--   0        0        0      343 2023-05-29 12:52:51.415597 optimuslib-0.0.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.4/README.md
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 optimuslib-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    29675 2023-05-29 13:07:32.126990 optimuslib-0.0.5/optimuslib/optimuslib.py
+-rw-r--r--   0        0        0      343 2023-05-29 13:13:40.253272 optimuslib-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.5/README.md
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 optimuslib-0.0.5/PKG-INFO
```

### Comparing `optimuslib-0.0.4/optimuslib/optimuslib.py` & `optimuslib-0.0.5/optimuslib/optimuslib.py`

 * *Files 0% similar despite different names*

```diff
@@ -446,27 +446,27 @@
 
 ########### TELEGRAM BOT NOTIFICATION - BOT DETAILS ##############
 def getTelegramBotInfo(botToken):
     log.info('Fetching BOT Information')
     url = 'https://api.telegram.org/bot'+botToken+'/getMe'
     response = sendRequest('get', url)
     responseJson = response.result().json()
-    if responseJson['ok']==true:
+    if responseJson['ok']==True:
         return True
     else:
         getVarInfo('responseJson',responseJson)
         return False
 
 ########### TELEGRAM BOT NOTIFICATION - FETCH RECEIVED MESSAGES ##############
 def getTelegramBotUpdates(botToken, update_id):
     log.info('Checking new messages...')
     url = 'https://api.telegram.org/bot'+botToken+'/getUpdates?offset='+str(update_id+1)
     response = sendRequest('get', url)
     responseJson = response.result().json()
-    if responseJson['ok']==true:
+    if responseJson['ok']==True:
         if responseJson['result']:
             for result in responseJson['result']:
                 update_id = result['update_id']
                 message_id = result['message']['message_id']
                 fromId = result['message']['from']['id']
                 fromFirstName = result['message']['from']['first_name']
                 fromUsername = result['message']['from']['username']
@@ -498,15 +498,15 @@
     '''
     
     url = 'https://api.telegram.org/bot'+botToken+'/sendMessage'
     data = {'chat_id': chatId, 'text': message}
 
     response = sendRequest('post', url, json=data)
     responseJson = response.result().json()
-    if responseJson['ok']==true:
+    if responseJson['ok']==True:
         return True
     else:
         getVarInfo('responseJson',responseJson)
         return False
         
         
 # if(optimuslib.sendTelegramNotification('5772623603:AAFNcED4WEKWGOzIp5l0BHNHsf_JdPiEV0o','79928065',output)):
```


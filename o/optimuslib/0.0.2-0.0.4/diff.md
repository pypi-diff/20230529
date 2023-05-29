# Comparing `tmp/optimuslib-0.0.2.tar.gz` & `tmp/optimuslib-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimuslib-0.0.2.tar", max compression
+gzip compressed data, was "optimuslib-0.0.4.tar", max compression
```

## Comparing `optimuslib-0.0.2.tar` & `optimuslib-0.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.2/optimuslib/__init__.py
--rw-r--r--   0        0        0    29886 2023-05-29 11:55:26.750370 optimuslib-0.0.2/optimuslib/optimuslib.py
--rw-r--r--   0        0        0      343 2023-05-29 12:23:08.824248 optimuslib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.2/README.md
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 optimuslib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.4/optimuslib/__init__.py
+-rw-r--r--   0        0        0    29675 2023-05-29 12:48:48.451666 optimuslib-0.0.4/optimuslib/optimuslib.py
+-rw-r--r--   0        0        0      343 2023-05-29 12:52:51.415597 optimuslib-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.4/README.md
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 optimuslib-0.0.4/PKG-INFO
```

### Comparing `optimuslib-0.0.2/optimuslib/optimuslib.py` & `optimuslib-0.0.4/optimuslib/optimuslib.py`

 * *Files 3% similar despite different names*

```diff
@@ -444,71 +444,72 @@
 
 
 
 ########### TELEGRAM BOT NOTIFICATION - BOT DETAILS ##############
 def getTelegramBotInfo(botToken):
     log.info('Fetching BOT Information')
     url = 'https://api.telegram.org/bot'+botToken+'/getMe'
-    response = optimuslib.sendRequest('get', url, proxyhost=proxyhost)
+    response = sendRequest('get', url)
     responseJson = response.result().json()
     if responseJson['ok']==true:
         return True
     else:
-        optimuslib.getVarInfo('responseJson',responseJson)
+        getVarInfo('responseJson',responseJson)
         return False
 
 ########### TELEGRAM BOT NOTIFICATION - FETCH RECEIVED MESSAGES ##############
 def getTelegramBotUpdates(botToken, update_id):
     log.info('Checking new messages...')
     url = 'https://api.telegram.org/bot'+botToken+'/getUpdates?offset='+str(update_id+1)
-    response = optimuslib.sendRequest('get', url, proxyhost=proxyhost)
+    response = sendRequest('get', url)
     responseJson = response.result().json()
     if responseJson['ok']==true:
         if responseJson['result']:
             for result in responseJson['result']:
                 update_id = result['update_id']
                 message_id = result['message']['message_id']
                 fromId = result['message']['from']['id']
                 fromFirstName = result['message']['from']['first_name']
                 fromUsername = result['message']['from']['username']
                 chatId = result['message']['chat']['id']
                 date = result['message']['date']
                 text = result['message']['text']
-                optimuslib.getVarInfo('update_id',update_id)
-                optimuslib.getVarInfo('message_id',message_id)
-                optimuslib.getVarInfo('fromId',fromId)
-                optimuslib.getVarInfo('fromFirstName',fromFirstName)
-                optimuslib.getVarInfo('fromUsername',fromUsername)
-                optimuslib.getVarInfo('chatId',chatId)
-                optimuslib.getVarInfo('date',date)
-                optimuslib.getVarInfo('text',text)
+                getVarInfo('update_id',update_id)
+                getVarInfo('message_id',message_id)
+                getVarInfo('fromId',fromId)
+                getVarInfo('fromFirstName',fromFirstName)
+                getVarInfo('fromUsername',fromUsername)
+                getVarInfo('chatId',chatId)
+                getVarInfo('date',date)
+                getVarInfo('text',text)
                 # return update_id, message_id, fromId, fromFirstName, fromUsername, chatId, date, text
                 return update_id, text
         else:
             return False, False
     else:
-        optimuslib.getVarInfo('responseJson',responseJson)
+        getVarInfo('responseJson',responseJson)
         return False, False
         
 ########### TELEGRAM BOT NOTIFICATION - SEND ##############
 def sendTelegramBotNotification(botToken,chatId,message):
     log.info('Sending Message via BOT')
     '''
     url = 'https://api.telegram.org/bot'+botToken+'/sendMessage?chat_id='+chatId+'&text='+message
     data = ''
     '''
+    
     url = 'https://api.telegram.org/bot'+botToken+'/sendMessage'
     data = {'chat_id': chatId, 'text': message}
 
-    response = optimuslib.sendRequest('post', url, json=data, proxyhost=proxyhost)
+    response = sendRequest('post', url, json=data)
     responseJson = response.result().json()
     if responseJson['ok']==true:
         return True
     else:
-        optimuslib.getVarInfo('responseJson',responseJson)
+        getVarInfo('responseJson',responseJson)
         return False
         
         
 # if(optimuslib.sendTelegramNotification('5772623603:AAFNcED4WEKWGOzIp5l0BHNHsf_JdPiEV0o','79928065',output)):
     # print('Telegram Notification Sent.')
 
 ########## TWILIO SMS ALERT ###############
```


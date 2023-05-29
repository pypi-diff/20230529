# Comparing `tmp/optimuslib-0.0.1.tar.gz` & `tmp/optimuslib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimuslib-0.0.1.tar", last modified: Fri May  5 08:19:07 2023, max compression
+gzip compressed data, was "optimuslib-0.0.2.tar", max compression
```

## Comparing `optimuslib-0.0.1.tar` & `optimuslib-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,5 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:19:07.807870 optimuslib-0.0.1/
--rw-rw-rw-   0        0        0      377 2023-05-05 08:19:07.804869 optimuslib-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 08:19:07.740870 optimuslib-0.0.1/optimuslib/
-drwxrwxrwx   0        0        0        0 2023-05-05 08:19:07.789870 optimuslib-0.0.1/optimuslib/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 08:19:07.782870 optimuslib-0.0.1/optimuslib/src/optimuslib.egg-info/
--rw-rw-rw-   0        0        0      377 2023-05-05 08:19:07.000000 optimuslib-0.0.1/optimuslib/src/optimuslib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      525 2023-05-05 08:19:07.000000 optimuslib-0.0.1/optimuslib/src/optimuslib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:19:07.000000 optimuslib-0.0.1/optimuslib/src/optimuslib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 08:19:07.000000 optimuslib-0.0.1/optimuslib/src/optimuslib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-05 08:19:07.000000 optimuslib-0.0.1/optimuslib/src/optimuslib.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    27494 2023-05-05 08:09:51.000000 optimuslib-0.0.1/optimuslib/src/optimuslib.py
--rw-rw-rw-   0        0        0       42 2023-05-05 08:19:07.808873 optimuslib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1244 2023-05-05 08:13:47.000000 optimuslib-0.0.1/setup.py
+-rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.2/optimuslib/__init__.py
+-rw-r--r--   0        0        0    29886 2023-05-29 11:55:26.750370 optimuslib-0.0.2/optimuslib/optimuslib.py
+-rw-r--r--   0        0        0      343 2023-05-29 12:23:08.824248 optimuslib-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.2/README.md
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 optimuslib-0.0.2/PKG-INFO
```

### Comparing `optimuslib-0.0.1/optimuslib/src/optimuslib.py` & `optimuslib-0.0.2/optimuslib/optimuslib.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # https://peps.python.org/pep-0008/
 # https://google.github.io/styleguide/pyguide.html
 
 
 ############ IMPORT THIS FILE USING BELOW COMMAND #############
 
 ### update github submodule (libraries) before pushing the latest update to github
-# git submodule add https://github.azc.ext.hp.com/shomi-nanwani/libraries
+# git submodule add https://github.com/optimus/libraries
 # git submodule update --remote
 
 # git submodule update
 
 # git submodule update --init
 # git add {submodule}
 
@@ -438,29 +438,80 @@
 
     # move file
     shutil.move(file_path, destination)
 
 def renameFile(current_file_name, new_file_name):
     os.rename(current_file_name, new_file_name)
 
-########### TELEGRAM BOT NOTIFICATION ##############
-def sendTelegramNotification(botToken,chatId,message):
+
+
+########### TELEGRAM BOT NOTIFICATION - BOT DETAILS ##############
+def getTelegramBotInfo(botToken):
+    log.info('Fetching BOT Information')
+    url = 'https://api.telegram.org/bot'+botToken+'/getMe'
+    response = optimuslib.sendRequest('get', url, proxyhost=proxyhost)
+    responseJson = response.result().json()
+    if responseJson['ok']==true:
+        return True
+    else:
+        optimuslib.getVarInfo('responseJson',responseJson)
+        return False
+
+########### TELEGRAM BOT NOTIFICATION - FETCH RECEIVED MESSAGES ##############
+def getTelegramBotUpdates(botToken, update_id):
+    log.info('Checking new messages...')
+    url = 'https://api.telegram.org/bot'+botToken+'/getUpdates?offset='+str(update_id+1)
+    response = optimuslib.sendRequest('get', url, proxyhost=proxyhost)
+    responseJson = response.result().json()
+    if responseJson['ok']==true:
+        if responseJson['result']:
+            for result in responseJson['result']:
+                update_id = result['update_id']
+                message_id = result['message']['message_id']
+                fromId = result['message']['from']['id']
+                fromFirstName = result['message']['from']['first_name']
+                fromUsername = result['message']['from']['username']
+                chatId = result['message']['chat']['id']
+                date = result['message']['date']
+                text = result['message']['text']
+                optimuslib.getVarInfo('update_id',update_id)
+                optimuslib.getVarInfo('message_id',message_id)
+                optimuslib.getVarInfo('fromId',fromId)
+                optimuslib.getVarInfo('fromFirstName',fromFirstName)
+                optimuslib.getVarInfo('fromUsername',fromUsername)
+                optimuslib.getVarInfo('chatId',chatId)
+                optimuslib.getVarInfo('date',date)
+                optimuslib.getVarInfo('text',text)
+                # return update_id, message_id, fromId, fromFirstName, fromUsername, chatId, date, text
+                return update_id, text
+        else:
+            return False, False
+    else:
+        optimuslib.getVarInfo('responseJson',responseJson)
+        return False, False
+        
+########### TELEGRAM BOT NOTIFICATION - SEND ##############
+def sendTelegramBotNotification(botToken,chatId,message):
+    log.info('Sending Message via BOT')
     '''
     url = 'https://api.telegram.org/bot'+botToken+'/sendMessage?chat_id='+chatId+'&text='+message
     data = ''
     '''
     url = 'https://api.telegram.org/bot'+botToken+'/sendMessage'
     data = {'chat_id': chatId, 'text': message}
 
-    response = sendRequest('post', url, json=data)
-    if 'true' in response.result().text:
+    response = optimuslib.sendRequest('post', url, json=data, proxyhost=proxyhost)
+    responseJson = response.result().json()
+    if responseJson['ok']==true:
         return True
     else:
-        return response.result().text
-
+        optimuslib.getVarInfo('responseJson',responseJson)
+        return False
+        
+        
 # if(optimuslib.sendTelegramNotification('5772623603:AAFNcED4WEKWGOzIp5l0BHNHsf_JdPiEV0o','79928065',output)):
     # print('Telegram Notification Sent.')
 
 ########## TWILIO SMS ALERT ###############
 '''
 from twilio.rest import Client
 def sendTwilioSMS(account_sid,auth_token,messagingServiceSid,toNumber,message):
```


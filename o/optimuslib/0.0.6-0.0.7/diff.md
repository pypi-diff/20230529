# Comparing `tmp/optimuslib-0.0.6.tar.gz` & `tmp/optimuslib-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optimuslib-0.0.6.tar", max compression
+gzip compressed data, was "optimuslib-0.0.7.tar", max compression
```

## Comparing `optimuslib-0.0.6.tar` & `optimuslib-0.0.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2023-05-29 13:32:12.741001 optimuslib-0.0.6/optimuslib/__init__.py
--rw-r--r--   0        0        0    30853 2023-05-29 13:43:24.695064 optimuslib-0.0.6/optimuslib/optimuslib.py
--rw-r--r--   0        0        0      343 2023-05-29 13:44:02.285293 optimuslib-0.0.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.6/README.md
--rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 optimuslib-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-29 13:32:12.741001 optimuslib-0.0.7/optimuslib/__init__.py
+-rw-r--r--   0        0        0    31065 2023-05-29 17:23:26.114807 optimuslib-0.0.7/optimuslib/optimuslib.py
+-rw-r--r--   0        0        0      343 2023-05-29 17:29:11.320109 optimuslib-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-29 12:14:49.714718 optimuslib-0.0.7/README.md
+-rw-r--r--   0        0        0      378 1970-01-01 00:00:00.000000 optimuslib-0.0.7/PKG-INFO
```

### Comparing `optimuslib-0.0.6/optimuslib/optimuslib.py` & `optimuslib-0.0.7/optimuslib/optimuslib.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Style Guide for python code
 # https://peps.python.org/pep-0008/
 # https://google.github.io/styleguide/pyguide.html
 
-
+proxyhost = None
+# proxyhost = 'http://127.0.0.1:8080'
 ############ IMPORT THIS FILE USING BELOW COMMAND #############
 
 ### update github submodule (libraries) before pushing the latest update to github
 # git submodule add https://github.com/optimus/libraries
 # git submodule update --remote
 
 # git submodule update
@@ -389,15 +390,15 @@
         pass
 
 # WRITE ANYTHING TO FILE
 def writeOutput(filename,output,end='\n'):
     # log.info('Writing file: `%s`', filename)
     f = open(filename, 'w')
     # f.write(output+'\n')
-    f.write(output+end)
+    f.write(str(output)+end)
     f.close()
 
 # READ TO FILE
 def readFile(filename):
     # log.info('Reading file: `%s`', filename)
     try:
         f = open(filename, 'r')
@@ -452,15 +453,15 @@
 
 
 
 ########### TELEGRAM BOT NOTIFICATION - BOT DETAILS ##############
 def getTelegramBotInfo(botToken):
     log.info('Fetching BOT Information')
     url = 'https://api.telegram.org/bot'+botToken+'/getMe'
-    response = sendRequest('get', url)
+    response = sendRequest('get', url, proxyhost=proxyhost)
     responseJson = response.result().json()
     if responseJson['ok']==True:
         if responseJson['result']:
             id = responseJson['result']['id']
             is_bot = responseJson['result']['is_bot']
             first_name = responseJson['result']['first_name']
             username = responseJson['result']['username']
@@ -481,15 +482,15 @@
         getVarInfo('responseJson',responseJson)
         return False
 
 ########### TELEGRAM BOT NOTIFICATION - FETCH RECEIVED MESSAGES ##############
 def getTelegramBotUpdates(botToken, update_id):
     log.info('Checking new messages...')
     url = 'https://api.telegram.org/bot'+botToken+'/getUpdates?offset='+str(update_id+1)
-    response = sendRequest('get', url)
+    response = sendRequest('get', url, proxyhost=proxyhost)
     responseJson = response.result().json()
     if responseJson['ok']==True:
         if responseJson['result']:
             for result in responseJson['result']:
                 update_id = result['update_id']
                 message_id = result['message']['message_id']
                 fromId = result['message']['from']['id']
@@ -503,33 +504,35 @@
                 getVarInfo('fromId',fromId)
                 getVarInfo('fromFirstName',fromFirstName)
                 getVarInfo('fromUsername',fromUsername)
                 getVarInfo('chatId',chatId)
                 getVarInfo('date',date)
                 getVarInfo('text',text)
                 # return update_id, message_id, fromId, fromFirstName, fromUsername, chatId, date, text
-                return update_id, text
+                return update_id, text, chatId
         else:
-            return False, False
+            return False, False, False
     else:
         getVarInfo('responseJson',responseJson)
         return False, False
         
 ########### TELEGRAM BOT NOTIFICATION - SEND ##############
 def sendTelegramBotNotification(botToken,chatId,message):
     log.info('Sending Message via BOT')
     '''
     url = 'https://api.telegram.org/bot'+botToken+'/sendMessage?chat_id='+chatId+'&text='+message
     data = ''
     '''
     
     url = 'https://api.telegram.org/bot'+botToken+'/sendMessage'
     data = {'chat_id': chatId, 'text': message}
-
-    response = sendRequest('post', url, json=data)
+    
+    # proxyhost = locals()
+    # proxyhost= 'http://127.0.0.1:8080'
+    response = sendRequest('post', url, json=data, proxyhost=proxyhost)
     responseJson = response.result().json()
     if responseJson['ok']==True:
         return True
     else:
         getVarInfo('responseJson',responseJson)
         return False
```


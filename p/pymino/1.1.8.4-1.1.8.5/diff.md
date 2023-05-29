# Comparing `tmp/pymino-1.1.8.4.tar.gz` & `tmp/pymino-1.1.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.8.3\dist\.tmp-_g53xax8\pymino-1.1.8.4.tar", last modified: Mon May 29 00:37:41 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.8.3\dist\.tmp-fitrcryk\pymino-1.1.8.5.tar", last modified: Mon May 29 04:02:43 2023, max compression
```

## Comparing `pymino-1.1.8.4.tar` & `pymino-1.1.8.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.656715 pymino-1.1.8.4/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.4/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-05-29 00:37:41.656715 pymino-1.1.8.4/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.613563 pymino-1.1.8.4/pymino/
--rw-rw-rw-   0        0        0      721 2023-05-29 00:12:00.000000 pymino-1.1.8.4/pymino/__init__.py
--rw-rw-rw-   0        0        0     8112 2023-05-29 00:01:55.000000 pymino-1.1.8.4/pymino/async_bot.py
--rw-rw-rw-   0        0        0    27542 2023-05-29 00:04:00.000000 pymino-1.1.8.4/pymino/bot.py
--rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.8.4/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.637867 pymino-1.1.8.4/pymino/ext/
--rw-rw-rw-   0        0        0      469 2023-05-28 22:44:43.000000 pymino-1.1.8.4/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.8.4/pymino/ext/account.py
--rw-rw-rw-   0        0        0   273924 2023-05-29 00:08:42.000000 pymino-1.1.8.4/pymino/ext/async_community.py
--rw-rw-rw-   0        0        0    18163 2023-05-28 22:59:05.000000 pymino-1.1.8.4/pymino/ext/async_context.py
--rw-rw-rw-   0        0        0    24194 2023-05-28 22:29:38.000000 pymino-1.1.8.4/pymino/ext/async_event_handler.py
--rw-rw-rw-   0        0        0     7299 2023-05-29 00:25:30.000000 pymino-1.1.8.4/pymino/ext/async_socket.py
--rw-rw-rw-   0        0        0   271224 2023-05-25 22:50:46.000000 pymino-1.1.8.4/pymino/ext/community.py
--rw-rw-rw-   0        0        0    44587 2023-05-29 00:03:54.000000 pymino-1.1.8.4/pymino/ext/context.py
--rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.8.4/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.648779 pymino-1.1.8.4/pymino/ext/entities/
--rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.8.4/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.4/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    14847 2023-05-28 23:41:49.000000 pymino-1.1.8.4/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    52847 2023-05-27 20:44:10.000000 pymino-1.1.8.4/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     4763 2023-05-29 00:33:12.000000 pymino-1.1.8.4/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.8.4/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     6185 2023-05-25 23:01:02.000000 pymino-1.1.8.4/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.4/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.4/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.8.4/pymino/ext/handle_queue.py
--rw-rw-rw-   0        0        0     7088 2023-05-29 00:33:01.000000 pymino-1.1.8.4/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.655723 pymino-1.1.8.4/pymino/ext/utilities/
--rw-rw-rw-   0        0        0      118 2023-05-28 22:35:54.000000 pymino-1.1.8.4/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0    11330 2023-05-28 22:35:37.000000 pymino-1.1.8.4/pymino/ext/utilities/async_request_handler.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.4/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.4/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.8.4/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-29 00:37:41.623483 pymino-1.1.8.4/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-05-29 00:37:41.000000 pymino-1.1.8.4/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1011 2023-05-29 00:37:41.000000 pymino-1.1.8.4/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 00:37:41.000000 pymino-1.1.8.4/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      102 2023-05-29 00:37:41.000000 pymino-1.1.8.4/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-29 00:37:41.000000 pymino-1.1.8.4/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-05-29 00:37:41.663163 pymino-1.1.8.4/setup.cfg
--rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.8.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.438526 pymino-1.1.8.5/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.8.5/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-05-29 04:02:43.439022 pymino-1.1.8.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.8.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.170687 pymino-1.1.8.5/pymino/
+-rw-rw-rw-   0        0        0      721 2023-05-29 04:00:48.000000 pymino-1.1.8.5/pymino/__init__.py
+-rw-rw-rw-   0        0        0     8112 2023-05-29 00:01:55.000000 pymino-1.1.8.5/pymino/async_bot.py
+-rw-rw-rw-   0        0        0    27542 2023-05-29 00:04:00.000000 pymino-1.1.8.5/pymino/bot.py
+-rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.8.5/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.205407 pymino-1.1.8.5/pymino/ext/
+-rw-rw-rw-   0        0        0      469 2023-05-28 22:44:43.000000 pymino-1.1.8.5/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.8.5/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   273903 2023-05-29 04:01:53.000000 pymino-1.1.8.5/pymino/ext/async_community.py
+-rw-rw-rw-   0        0        0    18163 2023-05-28 22:59:05.000000 pymino-1.1.8.5/pymino/ext/async_context.py
+-rw-rw-rw-   0        0        0    24302 2023-05-29 04:00:13.000000 pymino-1.1.8.5/pymino/ext/async_event_handler.py
+-rw-rw-rw-   0        0        0     7299 2023-05-29 00:25:30.000000 pymino-1.1.8.5/pymino/ext/async_socket.py
+-rw-rw-rw-   0        0        0   271224 2023-05-25 22:50:46.000000 pymino-1.1.8.5/pymino/ext/community.py
+-rw-rw-rw-   0        0        0    44587 2023-05-29 00:03:54.000000 pymino-1.1.8.5/pymino/ext/context.py
+-rw-rw-rw-   0        0        0     1758 2023-05-28 22:00:16.000000 pymino-1.1.8.5/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.352719 pymino-1.1.8.5/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.8.5/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.8.5/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    14847 2023-05-28 23:41:49.000000 pymino-1.1.8.5/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    52847 2023-05-27 20:44:10.000000 pymino-1.1.8.5/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     4763 2023-05-29 00:33:12.000000 pymino-1.1.8.5/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0    44257 2023-05-17 02:59:21.000000 pymino-1.1.8.5/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     6185 2023-05-25 23:01:02.000000 pymino-1.1.8.5/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.8.5/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2451 2023-05-17 03:04:06.000000 pymino-1.1.8.5/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0      543 2023-05-28 22:01:44.000000 pymino-1.1.8.5/pymino/ext/handle_queue.py
+-rw-rw-rw-   0        0        0     7088 2023-05-29 00:33:01.000000 pymino-1.1.8.5/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.437534 pymino-1.1.8.5/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0      118 2023-05-28 22:35:54.000000 pymino-1.1.8.5/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0    11320 2023-05-29 04:02:19.000000 pymino-1.1.8.5/pymino/ext/utilities/async_request_handler.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.8.5/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.8.5/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.8.5/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-29 04:02:43.191023 pymino-1.1.8.5/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-05-29 04:02:43.000000 pymino-1.1.8.5/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1011 2023-05-29 04:02:43.000000 pymino-1.1.8.5/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-29 04:02:43.000000 pymino-1.1.8.5/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      102 2023-05-29 04:02:43.000000 pymino-1.1.8.5/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-29 04:02:43.000000 pymino-1.1.8.5/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-05-29 04:02:43.450430 pymino-1.1.8.5/setup.cfg
+-rw-rw-rw-   0        0        0     1367 2023-05-29 00:20:50.000000 pymino-1.1.8.5/setup.py
```

### Comparing `pymino-1.1.8.4/LICENSE` & `pymino-1.1.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/PKG-INFO` & `pymino-1.1.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.4
+Version: 1.1.8.5
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.4 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.5 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.4/README.md` & `pymino-1.1.8.5/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/__init__.py` & `pymino-1.1.8.5/pymino/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.8.4'
+__version__ = '1.1.8.5'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .async_bot import AsyncBot as AsyncBot
 from .client import Client as Client
 
 from requests import get
```

### Comparing `pymino-1.1.8.4/pymino/async_bot.py` & `pymino-1.1.8.5/pymino/async_bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/bot.py` & `pymino-1.1.8.5/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/client.py` & `pymino-1.1.8.5/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/account.py` & `pymino-1.1.8.5/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/async_community.py` & `pymino-1.1.8.5/pymino/ext/async_community.py`

 * *Files 0% similar despite different names*

```diff
@@ -251,25 +251,25 @@
         >>> link_info = client.community.fetch_object(objectId="0000-00000-00000-0000", objectType=ObjectTypes.BLOG, comId=123456)
         >>> print(link_info.fullPath)
         """
         if "object_type" in kwargs: #TODO: Remove this in the near future.
             objectType = kwargs["object_type"]
             print("Warning: The 'object_type' parameter is deprecated. Please use 'objectType' instead.")
 
-        return LinkInfo(
-            await self.session.handler(
-                method="POST",
-                url=f"/g/s-x{self.community_id if comId is None else comId}/link-resolution",
-                data={
-                    "objectId": objectId,
-                    "targetCode": 1,
-                    "objectType": objectType.value if isinstance(objectType, ObjectTypes) else objectType,
-                    "timestamp": int(time() * 1000)
-                    }
-                ))
+        response = await self.session.handler(
+            method="POST",
+            url=f"/g/s-x{self.community_id if comId is None else comId}/link-resolution",
+            data={
+                "objectId": objectId,
+                "targetCode": 1,
+                "objectType": objectType.value if isinstance(objectType, ObjectTypes) else objectType,
+                "timestamp": int(time() * 1000)
+                }
+            )
+        return LinkInfo(response)
     
 
     def fetch_object_id(self, link: str) -> str:
         """
         Fetches the object ID given a link to the object.
 
         :param link: The link to the object.
```

### Comparing `pymino-1.1.8.4/pymino/ext/async_context.py` & `pymino-1.1.8.5/pymino/ext/async_context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/async_event_handler.py` & `pymino-1.1.8.5/pymino/ext/async_event_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,35 +220,40 @@
 
         if data.content[:len(self.command_prefix)] != self.command_prefix:
             return None
 
         message = data.content[len(self.command_prefix) + len(command_name) + 1:]
         command_name = dict(self._commands.__command_aliases__().copy()).get(command_name, command_name)
         
-        await self._check_cooldown(command_name, data, context)
-        func = self._commands.fetch_command(command_name).func
-        return await func(*await self._set_parameters(context=context, func=func, message=message))
+        response = await self._check_cooldown(command_name, data, context)
+
+        if response  != 403:
+            func = self._commands.fetch_command(command_name).func
+            return await func(*await self._set_parameters(context=context, func=func, message=message))
+        
+        return None
 
         
     async def _check_cooldown(self, command_name: str, data: Message, context: AsyncContext) -> None:
         """`_check_cooldown` is a function that checks if a command is on cooldown."""
         if self._commands.fetch_command(command_name).cooldown > 0:
             if self._commands.fetch_cooldown(command_name, data.author.userId) > time():
 
-                return context.reply(
+                await context.reply(
                     content=f"You are on cooldown for {int(self._commands.fetch_cooldown(command_name, data.author.userId) - time())} seconds."
                     )
+                return 403
             
             self._commands.set_cooldown(
                 command_name=command_name,
                 cooldown=self._commands.fetch_command(command_name).cooldown,
                 userId=data.author.userId
                 )
 
-        return None
+        return 200
 
 
     def on_error(self):
         def decorator(func: Callable) -> Callable:
             self._events["error"] = func
             return func
         return decorator
```

### Comparing `pymino-1.1.8.4/pymino/ext/async_socket.py` & `pymino-1.1.8.5/pymino/ext/async_socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/community.py` & `pymino-1.1.8.5/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/context.py` & `pymino-1.1.8.5/pymino/ext/context.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/dispatcher.py` & `pymino-1.1.8.5/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/entities/enums.py` & `pymino-1.1.8.5/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/entities/exceptions.py` & `pymino-1.1.8.5/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/entities/general.py` & `pymino-1.1.8.5/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/entities/handlers.py` & `pymino-1.1.8.5/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/entities/messages.py` & `pymino-1.1.8.5/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/entities/threads.py` & `pymino-1.1.8.5/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/entities/userprofile.py` & `pymino-1.1.8.5/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/entities/wsevents.py` & `pymino-1.1.8.5/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/handle_queue.py` & `pymino-1.1.8.5/pymino/ext/handle_queue.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/socket.py` & `pymino-1.1.8.5/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/utilities/async_request_handler.py` & `pymino-1.1.8.5/pymino/ext/utilities/async_request_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,641 +69,640 @@
 00000440: 6c66 2e73 6964 3a20 2020 2020 2020 4f70  lf.sid:       Op
 00000450: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
 00000460: 6e65 0d0a 2020 2020 2020 2020 7365 6c66  ne..        self
 00000470: 2e75 7365 7249 643a 2020 2020 4f70 7469  .userId:    Opti
 00000480: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
 00000490: 0d0a 2020 2020 2020 2020 7365 6c66 2e6f  ..        self.o
 000004a0: 726a 736f 6e3a 2020 2020 626f 6f6c 203d  rjson:    bool =
-000004b0: 206f 726a 736f 6e5f 6578 6973 7473 2829   orjson_exists()
-000004c0: 0d0a 0d0a 2020 2020 2020 2020 7365 6c66  ....        self
-000004d0: 2e70 726f 7879 203d 2070 726f 7879 2069  .proxy = proxy i
-000004e0: 6620 7072 6f78 7920 6973 206e 6f74 204e  f proxy is not N
-000004f0: 6f6e 6520 656c 7365 204e 6f6e 650d 0a0d  one else None...
-00000500: 0a20 2020 2020 2020 2073 656c 662e 7265  .        self.re
-00000510: 7370 6f6e 7365 5f6d 6170 203d 207b 0d0a  sponse_map = {..
-00000520: 2020 2020 2020 2020 2020 2020 3430 333a              403:
-00000530: 2046 6f72 6269 6464 656e 2c0d 0a20 2020   Forbidden,..   
-00000540: 2020 2020 2020 2020 2035 3032 3a20 4261           502: Ba
-00000550: 6447 6174 6577 6179 2c0d 0a20 2020 2020  dGateway,..     
-00000560: 2020 2020 2020 2035 3033 3a20 5365 7276         503: Serv
-00000570: 6963 6555 6e61 7661 696c 6162 6c65 0d0a  iceUnavailable..
-00000580: 2020 2020 2020 2020 7d0d 0a0d 0a0d 0a20          }...... 
-00000590: 2020 2061 7379 6e63 2064 6566 2069 6e69     async def ini
-000005a0: 7469 616c 697a 655f 7365 7373 696f 6e28  tialize_session(
-000005b0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-000005c0: 7365 6c66 2e73 6573 7369 6f6e 203d 2043  self.session = C
-000005d0: 6c69 656e 7453 6573 7369 6f6e 2829 0d0a  lientSession()..
-000005e0: 0d0a 0d0a 2020 2020 6173 796e 6320 6465  ....    async de
-000005f0: 6620 636c 6f73 655f 7365 7373 696f 6e28  f close_session(
-00000600: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00000610: 6966 2073 656c 662e 7365 7373 696f 6e20  if self.session 
-00000620: 6973 206e 6f74 204e 6f6e 653a 0d0a 2020  is not None:..  
-00000630: 2020 2020 2020 2020 2020 6177 6169 7420            await 
-00000640: 7365 6c66 2e73 6573 7369 6f6e 2e63 6c6f  self.session.clo
-00000650: 7365 2829 0d0a 0d0a 0d0a 2020 2020 6465  se()......    de
-00000660: 6620 7365 7276 6963 655f 7572 6c28 7365  f service_url(se
-00000670: 6c66 2c20 7572 6c3a 2073 7472 2920 2d3e  lf, url: str) ->
-00000680: 2073 7472 3a0d 0a20 2020 2020 2020 2022   str:..        "
-00000690: 2222 0d0a 2020 2020 2020 2020 6073 6572  ""..        `ser
-000006a0: 7669 6365 5f75 726c 6020 2d20 4170 7065  vice_url` - Appe
-000006b0: 6e64 7320 7468 6520 656e 6470 6f69 6e74  nds the endpoint
-000006c0: 2074 6f20 7468 6520 7365 7276 6963 6520   to the service 
-000006d0: 7572 6c0d 0a0d 0a20 2020 2020 2020 2060  url....        `
-000006e0: 2a2a 5061 7261 6d65 7465 7273 2a2a 6060  **Parameters**``
-000006f0: 0d0a 2020 2020 2020 2020 2d20 6075 726c  ..        - `url
-00000700: 6020 2d20 5468 6520 656e 6470 6f69 6e74  ` - The endpoint
-00000710: 2074 6f20 6170 7065 6e64 2074 6f20 7468   to append to th
-00000720: 6520 7365 7276 6963 6520 7572 6c2e 0d0a  e service url...
-00000730: 0d0a 2020 2020 2020 2020 602a 2a52 6574  ..        `**Ret
-00000740: 7572 6e73 2a2a 6060 0d0a 2020 2020 2020  urns**``..      
-00000750: 2020 2d20 6073 7472 6020 2d20 5468 6520    - `str` - The 
-00000760: 7365 7276 6963 6520 7572 6c2e 0d0a 0d0a  service url.....
-00000770: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00000780: 2020 2020 2072 6574 7572 6e20 6622 6874       return f"ht
-00000790: 7470 3a2f 2f73 6572 7669 6365 2e61 6d69  tp://service.ami
-000007a0: 6e6f 6170 7073 2e63 6f6d 2f61 7069 2f76  noapps.com/api/v
-000007b0: 317b 7572 6c7d 2220 6966 2075 726c 2e73  1{url}" if url.s
-000007c0: 7461 7274 7377 6974 6828 222f 2229 2065  tartswith("/") e
-000007d0: 6c73 6520 7572 6c0d 0a0d 0a20 2020 2061  lse url....    a
-000007e0: 7379 6e63 2064 6566 2073 6572 7669 6365  sync def service
-000007f0: 5f68 6561 6465 7273 2873 656c 6629 202d  _headers(self) -
-00000800: 3e20 6469 6374 3a0d 0a20 2020 2020 2020  > dict:..       
-00000810: 2022 2222 5265 7475 726e 7320 7468 6520   """Returns the 
-00000820: 7365 7276 6963 6520 6865 6164 6572 7322  service headers"
-00000830: 2222 0d0a 2020 2020 2020 2020 7265 7475  ""..        retu
-00000840: 726e 207b 0d0a 2020 2020 2020 2020 2020  rn {..          
-00000850: 2020 224e 4443 4c41 4e47 223a 2022 656e    "NDCLANG": "en
-00000860: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-00000870: 2241 4343 4550 542d 4c41 4e47 5541 4745  "ACCEPT-LANGUAGE
-00000880: 223a 2022 656e 2d55 5322 2c0d 0a20 2020  ": "en-US",..   
-00000890: 2020 2020 2020 2020 2022 5553 4552 2d41           "USER-A
-000008a0: 4745 4e54 223a 2022 4170 706c 6520 6950  GENT": "Apple iP
-000008b0: 686f 6e65 3133 2c34 2069 4f53 2076 3135  hone13,4 iOS v15
-000008c0: 2e36 2e31 204d 6169 6e2f 332e 3132 2e39  .6.1 Main/3.12.9
-000008d0: 222c 0d0a 2020 2020 2020 2020 2020 2020  ",..            
-000008e0: 2248 4f53 5422 3a20 2273 6572 7669 6365  "HOST": "service
-000008f0: 2e61 6d69 6e6f 6170 7073 2e63 6f6d 222c  .aminoapps.com",
-00000900: 0d0a 2020 2020 2020 2020 2020 2020 2243  ..            "C
-00000910: 4f4e 4e45 4354 494f 4e22 3a20 224b 6565  ONNECTION": "Kee
-00000920: 702d 416c 6976 6522 2c0d 0a20 2020 2020  p-Alive",..     
-00000930: 2020 2020 2020 2022 4143 4345 5054 2d45         "ACCEPT-E
-00000940: 4e43 4f44 494e 4722 3a20 2267 7a69 702c  NCODING": "gzip,
-00000950: 2064 6566 6c61 7465 2c20 6272 222c 0d0a   deflate, br",..
-00000960: 2020 2020 2020 2020 2020 2020 224e 4443              "NDC
-00000970: 4155 5448 223a 2066 2273 6964 3d7b 7365  AUTH": f"sid={se
-00000980: 6c66 2e73 6964 7d22 2c0d 0a20 2020 2020  lf.sid}",..     
-00000990: 2020 2020 2020 2022 4155 4944 223a 2073         "AUID": s
-000009a0: 656c 662e 7573 6572 4964 206f 7220 7374  elf.userId or st
-000009b0: 7228 7575 6964 3428 2929 0d0a 2020 2020  r(uuid4())..    
-000009c0: 2020 2020 7d0d 0a0d 0a0d 0a20 2020 2061      }......    a
-000009d0: 7379 6e63 2064 6566 2066 6574 6368 5f72  sync def fetch_r
-000009e0: 6571 7565 7374 2873 656c 662c 206d 6574  equest(self, met
-000009f0: 686f 643a 2073 7472 2920 2d3e 2043 616c  hod: str) -> Cal
-00000a00: 6c61 626c 653a 0d0a 2020 2020 2020 2020  lable:..        
-00000a10: 2222 220d 0a20 2020 2020 2020 2060 6665  """..        `fe
-00000a20: 7463 685f 7265 7175 6573 7460 202d 2052  tch_request` - R
-00000a30: 6574 7572 6e73 2074 6865 2072 6571 7565  eturns the reque
-00000a40: 7374 206d 6574 686f 640d 0a0d 0a20 2020  st method....   
-00000a50: 2020 2020 2060 2a2a 5061 7261 6d65 7465       `**Paramete
-00000a60: 7273 2a2a 6060 0d0a 2020 2020 2020 2020  rs**``..        
-00000a70: 2d20 606d 6574 686f 6460 202d 2054 6865  - `method` - The
-00000a80: 2072 6571 7565 7374 206d 6574 686f 6420   request method 
-00000a90: 746f 2072 6574 7572 6e2e 0d0a 0d0a 2020  to return.....  
-00000aa0: 2020 2020 2020 602a 2a52 6574 7572 6e73        `**Returns
-00000ab0: 2a2a 6060 0d0a 2020 2020 2020 2020 2d20  **``..        - 
-00000ac0: 6043 616c 6c61 626c 6560 202d 2054 6865  `Callable` - The
-00000ad0: 2072 6571 7565 7374 206d 6574 686f 642e   request method.
-00000ae0: 0d0a 0d0a 2020 2020 2020 2020 2222 220d  ....        """.
-00000af0: 0a20 2020 2020 2020 2072 6571 7565 7374  .        request
-00000b00: 5f6d 6574 686f 6473 203d 207b 0d0a 2020  _methods = {..  
-00000b10: 2020 2020 2020 2020 2020 2247 4554 223a            "GET":
-00000b20: 2073 656c 662e 7365 7373 696f 6e2e 6765   self.session.ge
-00000b30: 742c 0d0a 2020 2020 2020 2020 2020 2020  t,..            
-00000b40: 2250 4f53 5422 3a20 7365 6c66 2e73 6573  "POST": self.ses
-00000b50: 7369 6f6e 2e70 6f73 742c 0d0a 2020 2020  sion.post,..    
-00000b60: 2020 2020 2020 2020 2244 454c 4554 4522          "DELETE"
-00000b70: 3a20 7365 6c66 2e73 6573 7369 6f6e 2e64  : self.session.d
-00000b80: 656c 6574 652c 0d0a 2020 2020 2020 2020  elete,..        
-00000b90: 7d0d 0a20 2020 2020 2020 2072 6574 7572  }..        retur
-00000ba0: 6e20 7265 7175 6573 745f 6d65 7468 6f64  n request_method
-00000bb0: 735b 6d65 7468 6f64 5d0d 0a0d 0a0d 0a20  s[method]...... 
-00000bc0: 2020 2061 7379 6e63 2064 6566 2073 656e     async def sen
-00000bd0: 645f 7265 7175 6573 7428 0d0a 2020 2020  d_request(..    
-00000be0: 2020 2020 2020 2020 7365 6c66 2c0d 0a20          self,.. 
-00000bf0: 2020 2020 2020 2020 2020 206d 6574 686f             metho
-00000c00: 643a 2073 7472 2c0d 0a20 2020 2020 2020  d: str,..       
-00000c10: 2020 2020 2075 726c 3a20 7374 722c 0d0a       url: str,..
-00000c20: 2020 2020 2020 2020 2020 2020 6461 7461              data
-00000c30: 3a20 556e 696f 6e5b 6469 6374 2c20 6279  : Union[dict, by
-00000c40: 7465 732c 204e 6f6e 655d 2c0d 0a20 2020  tes, None],..   
-00000c50: 2020 2020 2020 2020 2068 6561 6465 7273           headers
-00000c60: 3a20 6469 6374 2c0d 0a20 2020 2020 2020  : dict,..       
-00000c70: 2020 2020 2063 6f6e 7465 6e74 5f74 7970       content_typ
-00000c80: 653a 204f 7074 696f 6e61 6c5b 7374 725d  e: Optional[str]
-00000c90: 0d0a 2020 2020 2920 2d3e 2055 6e69 6f6e  ..    ) -> Union
-00000ca0: 5b69 6e74 2c20 7374 725d 3a0d 0a20 2020  [int, str]:..   
-00000cb0: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00000cc0: 2020 6073 656e 645f 7265 7175 6573 7460    `send_request`
-00000cd0: 202d 2053 656e 6473 2061 2072 6571 7565   - Sends a reque
-00000ce0: 7374 0d0a 0d0a 2020 2020 2020 2020 602a  st....        `*
-00000cf0: 2a50 6172 616d 6574 6572 732a 2a60 600d  *Parameters**``.
-00000d00: 0a20 2020 2020 2020 202d 2060 6d65 7468  .        - `meth
-00000d10: 6f64 6020 2d20 5468 6520 7265 7175 6573  od` - The reques
-00000d20: 7420 6d65 7468 6f64 2074 6f20 7573 652e  t method to use.
-00000d30: 0d0a 2020 2020 2020 2020 2d20 6075 726c  ..        - `url
-00000d40: 6020 2d20 5468 6520 7572 6c20 746f 2073  ` - The url to s
-00000d50: 656e 6420 7468 6520 7265 7175 6573 7420  end the request 
-00000d60: 746f 2e0d 0a20 2020 2020 2020 202d 2060  to...        - `
-00000d70: 6461 7461 6020 2d20 5468 6520 6461 7461  data` - The data
-00000d80: 2074 6f20 7365 6e64 2077 6974 6820 7468   to send with th
-00000d90: 6520 7265 7175 6573 742e 0d0a 2020 2020  e request...    
-00000da0: 2020 2020 2d20 6068 6561 6465 7273 6020      - `headers` 
-00000db0: 2d20 5468 6520 6865 6164 6572 7320 746f  - The headers to
-00000dc0: 2073 656e 6420 7769 7468 2074 6865 2072   send with the r
-00000dd0: 6571 7565 7374 2e0d 0a20 2020 2020 2020  equest...       
-00000de0: 202d 2060 636f 6e74 656e 745f 7479 7065   - `content_type
-00000df0: 6020 2d20 5468 6520 636f 6e74 656e 7420  ` - The content 
-00000e00: 7479 7065 206f 6620 7468 6520 6461 7461  type of the data
-00000e10: 2e0d 0a0d 0a20 2020 2020 2020 2060 2a2a  .....        `**
-00000e20: 5265 7475 726e 732a 2a60 600d 0a20 2020  Returns**``..   
-00000e30: 2020 2020 202d 2060 556e 696f 6e5b 696e       - `Union[in
-00000e40: 742c 2073 7472 5d60 202d 2054 6865 2073  t, str]` - The s
-00000e50: 7461 7475 7320 636f 6465 2061 6e64 2072  tatus code and r
-00000e60: 6573 706f 6e73 6520 6672 6f6d 2074 6865  esponse from the
-00000e70: 2072 6571 7565 7374 2e0d 0a0d 0a20 2020   request.....   
-00000e80: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
-00000e90: 2020 6966 2073 656c 662e 7365 7373 696f    if self.sessio
-00000ea0: 6e20 6973 204e 6f6e 653a 0d0a 2020 2020  n is None:..    
-00000eb0: 2020 2020 2020 2020 6177 6169 7420 7365          await se
-00000ec0: 6c66 2e69 6e69 7469 616c 697a 655f 7365  lf.initialize_se
-00000ed0: 7373 696f 6e28 290d 0a0d 0a20 2020 2020  ssion()....     
-00000ee0: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00000ef0: 2020 2020 2061 7379 6e63 2077 6974 6820       async with 
-00000f00: 7365 6c66 2e73 6573 7369 6f6e 2e72 6571  self.session.req
-00000f10: 7565 7374 280d 0a20 2020 2020 2020 2020  uest(..         
-00000f20: 2020 2020 2020 206d 6574 686f 642c 2075         method, u
-00000f30: 726c 2c20 6461 7461 3d64 6174 612c 2068  rl, data=data, h
-00000f40: 6561 6465 7273 3d68 6561 6465 7273 2c20  eaders=headers, 
-00000f50: 7072 6f78 793d 7365 6c66 2e70 726f 7879  proxy=self.proxy
-00000f60: 0d0a 2020 2020 2020 2020 2020 2020 2920  ..            ) 
-00000f70: 6173 2072 6573 706f 6e73 653a 0d0a 2020  as response:..  
-00000f80: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00000f90: 7475 726e 2072 6573 706f 6e73 652e 7374  turn response.st
-00000fa0: 6174 7573 2c20 6177 6169 7420 7265 7370  atus, await resp
-00000fb0: 6f6e 7365 2e74 6578 7428 290d 0a20 2020  onse.text()..   
-00000fc0: 2020 2020 2065 7863 6570 7420 280d 0a20       except (.. 
-00000fd0: 2020 2020 2020 2020 2020 2054 7970 6545             TypeE
-00000fe0: 7272 6f72 2c0d 0a20 2020 2020 2020 2020  rror,..         
-00000ff0: 2020 2043 6c69 656e 7445 7272 6f72 2c0d     ClientError,.
-00001000: 0a20 2020 2020 2020 2020 2020 2043 6c69  .            Cli
-00001010: 656e 7443 6f6e 6e65 6374 696f 6e45 7272  entConnectionErr
-00001020: 6f72 2c0d 0a20 2020 2020 2020 2020 2020  or,..           
-00001030: 2043 6c69 656e 744f 5345 7272 6f72 2c0d   ClientOSError,.
-00001040: 0a20 2020 2020 2020 2020 2020 2043 6c69  .            Cli
-00001050: 656e 7443 6f6e 6e65 6374 6f72 4572 726f  entConnectorErro
-00001060: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
-00001070: 436c 6965 6e74 5072 6f78 7943 6f6e 6e65  ClientProxyConne
-00001080: 6374 696f 6e45 7272 6f72 2c0d 0a20 2020  ctionError,..   
-00001090: 2020 2020 2020 2020 2043 6c69 656e 7453           ClientS
-000010a0: 534c 4572 726f 722c 0d0a 2020 2020 2020  SLError,..      
-000010b0: 2020 2020 2020 436c 6965 6e74 436f 6e6e        ClientConn
-000010c0: 6563 746f 7253 534c 4572 726f 722c 0d0a  ectorSSLError,..
-000010d0: 2020 2020 2020 2020 2020 2020 436c 6965              Clie
-000010e0: 6e74 436f 6e6e 6563 746f 7243 6572 7469  ntConnectorCerti
-000010f0: 6669 6361 7465 4572 726f 722c 0d0a 2020  ficateError,..  
-00001100: 2020 2020 2020 2020 2020 5365 7276 6572            Server
-00001110: 436f 6e6e 6563 7469 6f6e 4572 726f 722c  ConnectionError,
-00001120: 0d0a 2020 2020 2020 2020 2020 2020 5365  ..            Se
-00001130: 7276 6572 5469 6d65 6f75 7445 7272 6f72  rverTimeoutError
-00001140: 2c0d 0a20 2020 2020 2020 2020 2020 2053  ,..            S
-00001150: 6572 7665 7244 6973 636f 6e6e 6563 7465  erverDisconnecte
-00001160: 6445 7272 6f72 2c0d 0a20 2020 2020 2020  dError,..       
-00001170: 2020 2020 2053 6572 7665 7246 696e 6765       ServerFinge
-00001180: 7270 7269 6e74 4d69 736d 6174 6368 2c0d  rprintMismatch,.
-00001190: 0a20 2020 2020 2020 2020 2020 2043 6c69  .            Cli
-000011a0: 656e 7452 6573 706f 6e73 6545 7272 6f72  entResponseError
-000011b0: 2c0d 0a20 2020 2020 2020 2020 2020 2043  ,..            C
-000011c0: 6c69 656e 7448 7474 7050 726f 7879 4572  lientHttpProxyEr
-000011d0: 726f 722c 0d0a 2020 2020 2020 2020 2020  ror,..          
-000011e0: 2020 5753 5365 7276 6572 4861 6e64 7368    WSServerHandsh
-000011f0: 616b 6545 7272 6f72 2c0d 0a20 2020 2020  akeError,..     
-00001200: 2020 2029 3a0d 0a20 2020 2020 2020 2020     ):..         
-00001210: 2020 2061 7761 6974 2073 656c 662e 6861     await self.ha
-00001220: 6e64 6c65 7228 6d65 7468 6f64 2c20 7572  ndler(method, ur
-00001230: 6c2c 2064 6174 612c 2063 6f6e 7465 6e74  l, data, content
-00001240: 5f74 7970 6529 0d0a 0d0a 0d0a 2020 2020  _type)......    
-00001250: 6173 796e 6320 6465 6620 6861 6e64 6c65  async def handle
-00001260: 7228 0d0a 2020 2020 2020 2020 2020 2020  r(..            
-00001270: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-00001280: 2020 206d 6574 686f 643a 2073 7472 2c0d     method: str,.
-00001290: 0a20 2020 2020 2020 2020 2020 2075 726c  .            url
-000012a0: 3a20 7374 722c 0d0a 2020 2020 2020 2020  : str,..        
-000012b0: 2020 2020 6461 7461 3a20 556e 696f 6e5b      data: Union[
-000012c0: 6469 6374 2c20 6279 7465 732c 204e 6f6e  dict, bytes, Non
-000012d0: 655d 203d 204e 6f6e 652c 0d0a 2020 2020  e] = None,..    
-000012e0: 2020 2020 2020 2020 636f 6e74 656e 745f          content_
-000012f0: 7479 7065 3a20 4f70 7469 6f6e 616c 5b73  type: Optional[s
-00001300: 7472 5d20 3d20 4e6f 6e65 0d0a 2020 2020  tr] = None..    
-00001310: 2920 2d3e 2064 6963 743a 0d0a 2020 2020  ) -> dict:..    
-00001320: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-00001330: 2060 6861 6e64 6c65 7260 202d 2048 616e   `handler` - Han
-00001340: 646c 6573 2061 6c6c 2072 6571 7565 7374  dles all request
-00001350: 730d 0a0d 0a20 2020 2020 2020 2060 2a2a  s....        `**
-00001360: 5061 7261 6d65 7465 7273 2a2a 6060 0d0a  Parameters**``..
-00001370: 2020 2020 2020 2020 2d20 606d 6574 686f          - `metho
-00001380: 6460 202d 2054 6865 2072 6571 7565 7374  d` - The request
-00001390: 206d 6574 686f 6420 746f 2075 7365 2e0d   method to use..
-000013a0: 0a20 2020 2020 2020 202d 2060 7572 6c60  .        - `url`
-000013b0: 202d 2054 6865 2075 726c 2074 6f20 7365   - The url to se
-000013c0: 6e64 2074 6865 2072 6571 7565 7374 2074  nd the request t
-000013d0: 6f2e 0d0a 2020 2020 2020 2020 2d20 6064  o...        - `d
-000013e0: 6174 6160 202d 2054 6865 2064 6174 6120  ata` - The data 
-000013f0: 746f 2073 656e 6420 7769 7468 2074 6865  to send with the
-00001400: 2072 6571 7565 7374 2e0d 0a20 2020 2020   request...     
-00001410: 2020 202d 2060 636f 6e74 656e 745f 7479     - `content_ty
-00001420: 7065 6020 2d20 5468 6520 636f 6e74 656e  pe` - The conten
-00001430: 7420 7479 7065 206f 6620 7468 6520 6461  t type of the da
-00001440: 7461 2e0d 0a0d 0a20 2020 2020 2020 2060  ta.....        `
-00001450: 2a2a 5265 7475 726e 732a 2a60 600d 0a20  **Returns**``.. 
-00001460: 2020 2020 2020 202d 2060 6469 6374 6020         - `dict` 
-00001470: 2d20 5468 6520 7265 7370 6f6e 7365 2066  - The response f
-00001480: 726f 6d20 7468 6520 7265 7175 6573 742e  rom the request.
-00001490: 0d0a 0d0a 2020 2020 2020 2020 2222 220d  ....        """.
-000014a0: 0a20 2020 2020 2020 2075 726c 203d 2073  .        url = s
-000014b0: 656c 662e 7365 7276 6963 655f 7572 6c28  elf.service_url(
-000014c0: 7572 6c29 0d0a 0d0a 2020 2020 2020 2020  url)....        
-000014d0: 7572 6c2c 2068 6561 6465 7273 2c20 6269  url, headers, bi
-000014e0: 6e61 7279 5f64 6174 6120 3d20 6177 6169  nary_data = awai
-000014f0: 7420 7365 6c66 2e73 6572 7669 6365 5f68  t self.service_h
-00001500: 616e 646c 6572 2875 726c 2c20 6461 7461  andler(url, data
-00001510: 2c20 636f 6e74 656e 745f 7479 7065 290d  , content_type).
-00001520: 0a0d 0a20 2020 2020 2020 2069 6620 616c  ...        if al
-00001530: 6c28 5b6d 6574 686f 6420 3d3d 2022 504f  l([method == "PO
-00001540: 5354 222c 2064 6174 6120 6973 204e 6f6e  ST", data is Non
-00001550: 655d 293a 0d0a 2020 2020 2020 2020 2020  e]):..          
-00001560: 2020 6865 6164 6572 735b 2243 4f4e 5445    headers["CONTE
-00001570: 4e54 2d54 5950 4522 5d20 3d20 2261 7070  NT-TYPE"] = "app
-00001580: 6c69 6361 7469 6f6e 2f6f 6374 6574 2d73  lication/octet-s
-00001590: 7472 6561 6d22 0d0a 0d0a 2020 2020 2020  tream"....      
-000015a0: 2020 7472 793a 0d0a 2020 2020 2020 2020    try:..        
-000015b0: 2020 2020 7374 6174 7573 5f63 6f64 652c      status_code,
-000015c0: 2063 6f6e 7465 6e74 203d 2061 7761 6974   content = await
-000015d0: 2073 656c 662e 7365 6e64 5f72 6571 7565   self.send_reque
-000015e0: 7374 280d 0a20 2020 2020 2020 2020 2020  st(..           
-000015f0: 2020 2020 206d 6574 686f 642c 2075 726c       method, url
-00001600: 2c20 6269 6e61 7279 5f64 6174 612c 2068  , binary_data, h
-00001610: 6561 6465 7273 2c20 636f 6e74 656e 745f  eaders, content_
-00001620: 7479 7065 0d0a 2020 2020 2020 2020 2020  type..          
-00001630: 2020 290d 0a20 2020 2020 2020 2065 7863    )..        exc
-00001640: 6570 7420 4578 6365 7074 696f 6e20 6173  ept Exception as
-00001650: 2065 3a0d 0a20 2020 2020 2020 2020 2020   e:..           
-00001660: 2070 7269 6e74 2865 290d 0a0d 0a20 2020   print(e)....   
-00001670: 2020 2020 2073 656c 662e 7072 696e 745f       self.print_
-00001680: 7265 7370 6f6e 7365 286d 6574 686f 643d  response(method=
-00001690: 6d65 7468 6f64 2c20 7572 6c3d 7572 6c2c  method, url=url,
-000016a0: 2073 7461 7475 735f 636f 6465 3d73 7461   status_code=sta
-000016b0: 7475 735f 636f 6465 290d 0a0d 0a20 2020  tus_code)....   
-000016c0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
-000016d0: 2e68 616e 646c 655f 7265 7370 6f6e 7365  .handle_response
-000016e0: 2873 7461 7475 735f 636f 6465 3d73 7461  (status_code=sta
-000016f0: 7475 735f 636f 6465 2c20 7265 7370 6f6e  tus_code, respon
-00001700: 7365 3d63 6f6e 7465 6e74 290d 0a0d 0a0d  se=content).....
-00001710: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
-00001720: 6572 7669 6365 5f68 616e 646c 6572 280d  ervice_handler(.
-00001730: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00001740: 662c 0d0a 2020 2020 2020 2020 2020 2020  f,..            
-00001750: 7572 6c3a 2073 7472 2c0d 0a20 2020 2020  url: str,..     
-00001760: 2020 2020 2020 2064 6174 613a 2055 6e69         data: Uni
-00001770: 6f6e 5b64 6963 742c 2062 7974 6573 2c20  on[dict, bytes, 
-00001780: 4e6f 6e65 5d20 3d20 4e6f 6e65 2c0d 0a20  None] = None,.. 
-00001790: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
-000017a0: 6e74 5f74 7970 653a 204f 7074 696f 6e61  nt_type: Optiona
-000017b0: 6c5b 7374 725d 203d 204e 6f6e 650d 0a20  l[str] = None.. 
-000017c0: 2020 2029 202d 3e20 5475 706c 655b 7374     ) -> Tuple[st
-000017d0: 722c 2064 6963 742c 2055 6e69 6f6e 5b64  r, dict, Union[d
-000017e0: 6963 742c 2062 7974 6573 2c20 4e6f 6e65  ict, bytes, None
-000017f0: 5d5d 3a0d 0a20 2020 2020 2020 2022 2222  ]]:..        """
-00001800: 0d0a 2020 2020 2020 2020 6073 6572 7669  ..        `servi
-00001810: 6365 5f68 616e 646c 6572 6020 2d20 5369  ce_handler` - Si
-00001820: 676e 7320 7468 6520 7265 7175 6573 7420  gns the request 
-00001830: 616e 6420 7265 7475 726e 7320 7468 6520  and returns the 
-00001840: 7365 7276 6963 6520 7572 6c2c 2068 6561  service url, hea
-00001850: 6465 7273 2061 6e64 2064 6174 610d 0a0d  ders and data...
-00001860: 0a20 2020 2020 2020 2060 2a2a 5061 7261  .        `**Para
-00001870: 6d65 7465 7273 2a2a 6060 0d0a 2020 2020  meters**``..    
-00001880: 2020 2020 2d20 6075 726c 6020 2d20 5468      - `url` - Th
-00001890: 6520 7572 6c20 746f 2073 656e 6420 7468  e url to send th
-000018a0: 6520 7265 7175 6573 7420 746f 2e0d 0a20  e request to... 
-000018b0: 2020 2020 2020 202d 2060 6461 7461 6020         - `data` 
-000018c0: 2d20 5468 6520 6461 7461 2074 6f20 7365  - The data to se
-000018d0: 6e64 2077 6974 6820 7468 6520 7265 7175  nd with the requ
-000018e0: 6573 742e 0d0a 2020 2020 2020 2020 2d20  est...        - 
-000018f0: 6063 6f6e 7465 6e74 5f74 7970 6560 202d  `content_type` -
-00001900: 2054 6865 2063 6f6e 7465 6e74 2074 7970   The content typ
-00001910: 6520 6f66 2074 6865 2064 6174 612e 0d0a  e of the data...
-00001920: 0d0a 2020 2020 2020 2020 602a 2a52 6574  ..        `**Ret
-00001930: 7572 6e73 2a2a 6060 0d0a 2020 2020 2020  urns**``..      
-00001940: 2020 2d20 6054 7570 6c65 5b73 7472 2c20    - `Tuple[str, 
-00001950: 6469 6374 2c20 556e 696f 6e5b 6469 6374  dict, Union[dict
-00001960: 2c20 6279 7465 732c 204e 6f6e 655d 5d60  , bytes, None]]`
-00001970: 202d 2054 6865 2073 6572 7669 6365 2075   - The service u
-00001980: 726c 2c20 6865 6164 6572 7320 616e 6420  rl, headers and 
-00001990: 6461 7461 2e0d 0a0d 0a20 2020 2020 2020  data.....       
-000019a0: 2022 2222 0d0a 0d0a 2020 2020 2020 2020   """....        
-000019b0: 6865 6164 6572 7320 3d20 7b22 4e44 4344  headers = {"NDCD
-000019c0: 4556 4943 4549 4422 3a20 6465 7669 6365  EVICEID": device
-000019d0: 5f69 6428 292c 202a 2a61 7761 6974 2073  _id(), **await s
-000019e0: 656c 662e 7365 7276 6963 655f 6865 6164  elf.service_head
-000019f0: 6572 7328 297d 0d0a 0d0a 2020 2020 2020  ers()}....      
-00001a00: 2020 6966 2064 6174 6120 6f72 2063 6f6e    if data or con
-00001a10: 7465 6e74 5f74 7970 653a 0d0a 2020 2020  tent_type:..    
-00001a20: 2020 2020 2020 2020 6865 6164 6572 732c          headers,
-00001a30: 2064 6174 6120 3d20 6177 6169 7420 7365   data = await se
-00001a40: 6c66 2e66 6574 6368 5f73 6967 6e61 7475  lf.fetch_signatu
-00001a50: 7265 2864 6174 612c 2068 6561 6465 7273  re(data, headers
-00001a60: 2c20 636f 6e74 656e 745f 7479 7065 290d  , content_type).
-00001a70: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
-00001a80: 6e20 7572 6c2c 2068 6561 6465 7273 2c20  n url, headers, 
-00001a90: 7365 6c66 2e65 6e73 7572 655f 7574 6638  self.ensure_utf8
-00001aa0: 2864 6174 6129 0d0a 0d0a 0d0a 2020 2020  (data)......    
-00001ab0: 6465 6620 656e 7375 7265 5f75 7466 3828  def ensure_utf8(
-00001ac0: 7365 6c66 2c20 6461 7461 3a20 556e 696f  self, data: Unio
-00001ad0: 6e5b 6469 6374 2c20 6279 7465 732c 204e  n[dict, bytes, N
-00001ae0: 6f6e 655d 2920 2d3e 2055 6e69 6f6e 5b64  one]) -> Union[d
-00001af0: 6963 742c 2062 7974 6573 2c20 4e6f 6e65  ict, bytes, None
-00001b00: 5d3a 0d0a 2020 2020 2020 2020 2222 220d  ]:..        """.
-00001b10: 0a20 2020 2020 2020 2060 656e 7375 7265  .        `ensure
-00001b20: 5f75 7466 3860 202d 2045 6e73 7572 6573  _utf8` - Ensures
-00001b30: 2074 6865 2064 6174 6120 6973 2075 7466   the data is utf
-00001b40: 2d38 2065 6e63 6f64 6564 0d0a 0d0a 2020  -8 encoded....  
-00001b50: 2020 2020 2020 602a 2a50 6172 616d 6574        `**Paramet
-00001b60: 6572 732a 2a60 600d 0a20 2020 2020 2020  ers**``..       
-00001b70: 202d 2060 6461 7461 6020 2d20 5468 6520   - `data` - The 
-00001b80: 6461 7461 2074 6f20 656e 636f 6465 2e0d  data to encode..
-00001b90: 0a0d 0a20 2020 2020 2020 2060 2a2a 5265  ...        `**Re
-00001ba0: 7475 726e 732a 2a60 600d 0a20 2020 2020  turns**``..     
-00001bb0: 2020 202d 2060 556e 696f 6e5b 6469 6374     - `Union[dict
-00001bc0: 2c20 6279 7465 732c 204e 6f6e 655d 6020  , bytes, None]` 
-00001bd0: 2d20 5468 6520 656e 636f 6465 6420 6461  - The encoded da
-00001be0: 7461 2e0d 0a0d 0a20 2020 2020 2020 2022  ta.....        "
-00001bf0: 2222 0d0a 0d0a 2020 2020 2020 2020 6966  ""....        if
-00001c00: 2064 6174 6120 6973 204e 6f6e 653a 0d0a   data is None:..
-00001c10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00001c20: 726e 2064 6174 610d 0a0d 0a20 2020 2020  rn data....     
-00001c30: 2020 2064 6566 2068 616e 646c 655f 6469     def handle_di
-00001c40: 6374 2864 6174 613a 2064 6963 7429 3a0d  ct(data: dict):.
-00001c50: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00001c60: 7572 6e20 7b6b 6579 3a20 7365 6c66 2e65  urn {key: self.e
-00001c70: 6e73 7572 655f 7574 6638 2876 616c 7565  nsure_utf8(value
-00001c80: 2920 666f 7220 6b65 792c 2076 616c 7565  ) for key, value
-00001c90: 2069 6e20 6461 7461 2e69 7465 6d73 2829   in data.items()
-00001ca0: 7d0d 0a0d 0a20 2020 2020 2020 2064 6566  }....        def
-00001cb0: 2068 616e 646c 655f 7374 7228 6461 7461   handle_str(data
-00001cc0: 3a20 7374 7229 3a0d 0a20 2020 2020 2020  : str):..       
-00001cd0: 2020 2020 2072 6574 7572 6e20 6461 7461       return data
-00001ce0: 2e65 6e63 6f64 6528 2275 7466 2d38 2229  .encode("utf-8")
-00001cf0: 0d0a 0d0a 2020 2020 2020 2020 6861 6e64  ....        hand
-00001d00: 6c65 7273 203d 207b 0d0a 2020 2020 2020  lers = {..      
-00001d10: 2020 2020 2020 6469 6374 3a20 6861 6e64        dict: hand
-00001d20: 6c65 5f64 6963 742c 0d0a 2020 2020 2020  le_dict,..      
-00001d30: 2020 2020 2020 7374 723a 2068 616e 646c        str: handl
-00001d40: 655f 7374 720d 0a20 2020 2020 2020 207d  e_str..        }
-00001d50: 0d0a 0d0a 2020 2020 2020 2020 7265 7475  ....        retu
-00001d60: 726e 2068 616e 646c 6572 732e 6765 7428  rn handlers.get(
-00001d70: 7479 7065 2864 6174 6129 2c20 6c61 6d62  type(data), lamb
-00001d80: 6461 2078 3a20 7829 2864 6174 6129 0d0a  da x: x)(data)..
-00001d90: 0d0a 0d0a 2020 2020 6173 796e 6320 6465  ....    async de
-00001da0: 6620 6665 7463 685f 7369 676e 6174 7572  f fetch_signatur
-00001db0: 6528 0d0a 2020 2020 2020 2020 2020 2020  e(..            
-00001dc0: 7365 6c66 2c0d 0a20 2020 2020 2020 2020  self,..         
-00001dd0: 2020 2064 6174 613a 2055 6e69 6f6e 5b64     data: Union[d
-00001de0: 6963 742c 2062 7974 6573 2c20 4e6f 6e65  ict, bytes, None
-00001df0: 5d2c 0d0a 2020 2020 2020 2020 2020 2020  ],..            
-00001e00: 6865 6164 6572 733a 2064 6963 742c 0d0a  headers: dict,..
-00001e10: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
-00001e20: 656e 745f 7479 7065 3a20 7374 7220 3d20  ent_type: str = 
-00001e30: 4e6f 6e65 0d0a 2020 2020 2920 2d3e 2054  None..    ) -> T
-00001e40: 7570 6c65 5b64 6963 742c 2055 6e69 6f6e  uple[dict, Union
-00001e50: 5b64 6963 742c 2062 7974 6573 2c20 4e6f  [dict, bytes, No
-00001e60: 6e65 5d5d 3a0d 0a20 2020 2020 2020 2022  ne]]:..        "
-00001e70: 2222 0d0a 2020 2020 2020 2020 6066 6574  ""..        `fet
-00001e80: 6368 5f73 6967 6e61 7475 7265 6020 2d20  ch_signature` - 
-00001e90: 4665 7463 6865 7320 7468 6520 7369 676e  Fetches the sign
-00001ea0: 6174 7572 6520 616e 6420 7265 7475 726e  ature and return
-00001eb0: 7320 7468 6520 6461 7461 2061 6e64 2075  s the data and u
-00001ec0: 7064 6174 6564 2068 6561 6465 7273 0d0a  pdated headers..
-00001ed0: 0d0a 2020 2020 2020 2020 602a 2a50 6172  ..        `**Par
-00001ee0: 616d 6574 6572 732a 2a60 600d 0a20 2020  ameters**``..   
-00001ef0: 2020 2020 202d 2060 6461 7461 6020 2d20       - `data` - 
-00001f00: 5468 6520 6461 7461 2074 6f20 7365 6e64  The data to send
-00001f10: 2077 6974 6820 7468 6520 7265 7175 6573   with the reques
-00001f20: 742e 0d0a 2020 2020 2020 2020 2d20 6068  t...        - `h
-00001f30: 6561 6465 7273 6020 2d20 5468 6520 6865  eaders` - The he
-00001f40: 6164 6572 7320 746f 2073 656e 6420 7769  aders to send wi
-00001f50: 7468 2074 6865 2072 6571 7565 7374 2e0d  th the request..
-00001f60: 0a20 2020 2020 2020 202d 2060 636f 6e74  .        - `cont
-00001f70: 656e 745f 7479 7065 6020 2d20 5468 6520  ent_type` - The 
-00001f80: 636f 6e74 656e 7420 7479 7065 206f 6620  content type of 
-00001f90: 7468 6520 6461 7461 2e0d 0a0d 0a20 2020  the data.....   
-00001fa0: 2020 2020 2060 2a2a 5265 7475 726e 732a       `**Returns*
-00001fb0: 2a60 600d 0a20 2020 2020 2020 202d 2060  *``..        - `
-00001fc0: 5475 706c 655b 6469 6374 2c20 556e 696f  Tuple[dict, Unio
-00001fd0: 6e5b 6469 6374 2c20 6279 7465 732c 204e  n[dict, bytes, N
-00001fe0: 6f6e 655d 5d60 202d 2054 6865 2068 6561  one]]` - The hea
-00001ff0: 6465 7273 2061 6e64 2064 6174 612e 0d0a  ders and data...
-00002000: 0d0a 2020 2020 2020 2020 2222 220d 0a0d  ..        """...
-00002010: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00002020: 6973 696e 7374 616e 6365 2864 6174 612c  isinstance(data,
-00002030: 2062 7974 6573 293a 0d0a 2020 2020 2020   bytes):..      
-00002040: 2020 2020 2020 6461 7461 203d 2028 0d0a        data = (..
-00002050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002060: 6f72 6a73 6f6e 5f64 756d 7073 2864 6174  orjson_dumps(dat
-00002070: 6129 0d0a 2020 2020 2020 2020 2020 2020  a)..            
-00002080: 2020 2020 6966 2073 656c 662e 6f72 6a73      if self.orjs
-00002090: 6f6e 0d0a 2020 2020 2020 2020 2020 2020  on..            
-000020a0: 2020 2020 656c 7365 2064 756d 7073 2864      else dumps(d
-000020b0: 6174 6129 0d0a 2020 2020 2020 2020 2020  ata)..          
-000020c0: 2020 292e 6465 636f 6465 2822 7574 662d    ).decode("utf-
-000020d0: 3822 290d 0a0d 0a20 2020 2020 2020 2068  8")....        h
-000020e0: 6561 6465 7273 2e75 7064 6174 6528 0d0a  eaders.update(..
-000020f0: 2020 2020 2020 2020 2020 2020 7b0d 0a20              {.. 
-00002100: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00002110: 434f 4e54 454e 542d 4c45 4e47 5448 223a  CONTENT-LENGTH":
-00002120: 2066 227b 6c65 6e28 6461 7461 297d 222c   f"{len(data)}",
-00002130: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002140: 2020 2243 4f4e 5445 4e54 2d54 5950 4522    "CONTENT-TYPE"
-00002150: 3a20 636f 6e74 656e 745f 7479 7065 206f  : content_type o
-00002160: 7220 2261 7070 6c69 6361 7469 6f6e 2f6a  r "application/j
-00002170: 736f 6e3b 2063 6861 7273 6574 3d75 7466  son; charset=utf
-00002180: 2d38 222c 0d0a 2020 2020 2020 2020 2020  -8",..          
-00002190: 2020 2020 2020 224e 4443 2d4d 5347 2d53        "NDC-MSG-S
-000021a0: 4947 223a 2067 656e 6572 6174 655f 7369  IG": generate_si
-000021b0: 676e 6174 7572 6528 6461 7461 292c 0d0a  gnature(data),..
-000021c0: 2020 2020 2020 2020 2020 2020 7d0d 0a20              }.. 
-000021d0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
-000021e0: 2020 7265 7475 726e 2068 6561 6465 7273    return headers
-000021f0: 2c20 6461 7461 0d0a 0d0a 0d0a 2020 2020  , data......    
-00002200: 6465 6620 7261 6973 655f 6572 726f 7228  def raise_error(
-00002210: 7365 6c66 2c20 7265 7370 6f6e 7365 3a20  self, response: 
-00002220: 6469 6374 2920 2d3e 204e 6f6e 653a 0d0a  dict) -> None:..
-00002230: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
-00002240: 2020 2020 2060 7261 6973 655f 6572 726f       `raise_erro
-00002250: 7260 202d 2052 6169 7365 7320 616e 2065  r` - Raises an e
-00002260: 7272 6f72 2069 6620 616e 2065 7272 6f72  rror if an error
-00002270: 2069 7320 696e 2074 6865 2072 6573 706f   is in the respo
-00002280: 6e73 650d 0a0d 0a20 2020 2020 2020 2060  nse....        `
-00002290: 2a2a 5061 7261 6d65 7465 7273 2a2a 6060  **Parameters**``
-000022a0: 0d0a 2020 2020 2020 2020 2d20 6072 6573  ..        - `res
-000022b0: 706f 6e73 6560 202d 2054 6865 2072 6573  ponse` - The res
-000022c0: 706f 6e73 6520 6672 6f6d 2074 6865 2072  ponse from the r
-000022d0: 6571 7565 7374 2e0d 0a0d 0a20 2020 2020  equest.....     
-000022e0: 2020 2060 2a2a 5265 7475 726e 732a 2a60     `**Returns**`
-000022f0: 600d 0a20 2020 2020 2020 202d 2060 4e6f  `..        - `No
-00002300: 6e65 6020 2d20 5261 6973 6573 2061 6e20  ne` - Raises an 
-00002310: 6572 726f 7220 6966 2074 6865 2073 7461  error if the sta
-00002320: 7475 7320 636f 6465 2069 7320 696e 2074  tus code is in t
-00002330: 6865 2072 6573 706f 6e73 6520 6d61 702e  he response map.
-00002340: 0d0a 0d0a 2020 2020 2020 2020 2222 220d  ....        """.
-00002350: 0a20 2020 2020 2020 2069 6620 616c 6c28  .        if all(
-00002360: 0d0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00002370: 2020 5b0d 0a20 2020 2020 2020 2020 2020    [..           
-00002380: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-00002390: 652e 6765 7428 2261 7069 3a73 7461 7475  e.get("api:statu
-000023a0: 7363 6f64 6522 2c20 3230 3029 203d 3d20  scode", 200) == 
-000023b0: 3130 352c 0d0a 2020 2020 2020 2020 2020  105,..          
-000023c0: 2020 2020 2020 2020 2020 6861 7361 7474            hasatt
-000023d0: 7228 7365 6c66 2c20 2265 6d61 696c 2229  r(self, "email")
-000023e0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-000023f0: 2020 2020 2020 2068 6173 6174 7472 2873         hasattr(s
-00002400: 656c 662c 2022 7061 7373 776f 7264 2229  elf, "password")
-00002410: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00002420: 2020 205d 0d0a 2020 2020 2020 2020 293a     ]..        ):
-00002430: 0d0a 2020 2020 2020 2020 2020 2020 7265  ..            re
-00002440: 7475 726e 2073 656c 662e 626f 742e 7275  turn self.bot.ru
-00002450: 6e28 7365 6c66 2e65 6d61 696c 2c20 7365  n(self.email, se
-00002460: 6c66 2e70 6173 7377 6f72 642c 2075 7365  lf.password, use
-00002470: 5f63 6163 6865 3d46 616c 7365 290d 0a0d  _cache=False)...
-00002480: 0a20 2020 2020 2020 2065 6c73 653a 0d0a  .        else:..
-00002490: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-000024a0: 6520 4150 4945 7863 6570 7469 6f6e 2872  e APIException(r
-000024b0: 6573 706f 6e73 6529 0d0a 0d0a 0d0a 2020  esponse)......  
-000024c0: 2020 6465 6620 6861 6e64 6c65 5f72 6573    def handle_res
-000024d0: 706f 6e73 6528 7365 6c66 2c20 7374 6174  ponse(self, stat
-000024e0: 7573 5f63 6f64 653a 2069 6e74 2c20 7265  us_code: int, re
-000024f0: 7370 6f6e 7365 3a20 7374 7229 202d 3e20  sponse: str) -> 
-00002500: 6469 6374 3a0d 0a20 2020 2020 2020 2022  dict:..        "
-00002510: 2222 0d0a 2020 2020 2020 2020 6068 616e  ""..        `han
-00002520: 646c 655f 7265 7370 6f6e 7365 6020 2d20  dle_response` - 
-00002530: 4861 6e64 6c65 7320 7468 6520 7265 7370  Handles the resp
-00002540: 6f6e 7365 2061 6e64 2072 6574 7572 6e73  onse and returns
-00002550: 2074 6865 2072 6573 706f 6e73 6520 6173   the response as
-00002560: 2061 2064 6963 740d 0a0d 0a20 2020 2020   a dict....     
-00002570: 2020 2060 2a2a 5061 7261 6d65 7465 7273     `**Parameters
-00002580: 2a2a 6060 0d0a 2020 2020 2020 2020 2d20  **``..        - 
-00002590: 6073 7461 7475 735f 636f 6465 6020 2d20  `status_code` - 
-000025a0: 5468 6520 7374 6174 7573 2063 6f64 6520  The status code 
-000025b0: 6f66 2074 6865 2072 6573 706f 6e73 652e  of the response.
-000025c0: 0d0a 2020 2020 2020 2020 2d20 6072 6573  ..        - `res
-000025d0: 706f 6e73 6560 202d 2054 6865 2072 6573  ponse` - The res
-000025e0: 706f 6e73 6520 746f 2068 616e 646c 652e  ponse to handle.
-000025f0: 0d0a 0d0a 2020 2020 2020 2020 602a 2a52  ....        `**R
-00002600: 6574 7572 6e73 2a2a 6060 0d0a 2020 2020  eturns**``..    
-00002610: 2020 2020 2d20 6064 6963 7460 202d 2054      - `dict` - T
-00002620: 6865 2072 6573 706f 6e73 6520 6173 2061  he response as a
-00002630: 2064 6963 742e 0d0a 0d0a 2020 2020 2020   dict.....      
-00002640: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
-00002650: 6620 7374 6174 7573 5f63 6f64 6520 696e  f status_code in
-00002660: 2073 656c 662e 7265 7370 6f6e 7365 5f6d   self.response_m
-00002670: 6170 3a0d 0a20 2020 2020 2020 2020 2020  ap:..           
-00002680: 2072 6169 7365 2073 656c 662e 7265 7370   raise self.resp
-00002690: 6f6e 7365 5f6d 6170 5b73 7461 7475 735f  onse_map[status_
-000026a0: 636f 6465 5d0d 0a0d 0a20 2020 2020 2020  code]....       
-000026b0: 2065 6c69 6620 7265 7370 6f6e 7365 2e73   elif response.s
-000026c0: 7461 7274 7377 6974 6828 226e 756c 6c22  tartswith("null"
-000026d0: 293a 0d0a 2020 2020 2020 2020 2020 2020  ):..            
-000026e0: 7261 6973 6520 4e75 6c6c 5265 7370 6f6e  raise NullRespon
-000026f0: 7365 0d0a 0d0a 2020 2020 2020 2020 656c  se....        el
-00002700: 7365 3a0d 0a0d 0a20 2020 2020 2020 2020  se:....         
-00002710: 2020 2074 7279 3a0d 0a20 2020 2020 2020     try:..       
-00002720: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
-00002730: 6520 3d20 280d 0a20 2020 2020 2020 2020  e = (..         
-00002740: 2020 2020 2020 2020 2020 206f 726a 736f             orjso
-00002750: 6e5f 6c6f 6164 7328 7265 7370 6f6e 7365  n_loads(response
-00002760: 290d 0a20 2020 2020 2020 2020 2020 2020  )..             
-00002770: 2020 2020 2020 2069 6620 7365 6c66 2e6f         if self.o
-00002780: 726a 736f 6e0d 0a20 2020 2020 2020 2020  rjson..         
-00002790: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-000027a0: 6c6f 6164 7328 7265 7370 6f6e 7365 290d  loads(response).
-000027b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000027c0: 2029 0d0a 2020 2020 2020 2020 2020 2020   )..            
-000027d0: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
-000027e0: 3a0d 0a20 2020 2020 2020 2020 2020 2020  :..             
-000027f0: 2020 2072 6573 706f 6e73 6520 3d20 6c6f     response = lo
-00002800: 6164 7328 7265 7370 6f6e 7365 290d 0a0d  ads(response)...
-00002810: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00002820: 7374 6174 7573 5f63 6f64 6520 213d 2032  status_code != 2
-00002830: 3030 3a0d 0a20 2020 2020 2020 2020 2020  00:..           
-00002840: 2020 2020 2073 656c 662e 7261 6973 655f       self.raise_
-00002850: 6572 726f 7228 7265 7370 6f6e 7365 290d  error(response).
-00002860: 0a0d 0a20 2020 2020 2020 2020 2020 2072  ...            r
-00002870: 6574 7572 6e20 7265 7370 6f6e 7365 0d0a  eturn response..
-00002880: 0d0a 0d0a 2020 2020 6465 6620 7072 696e  ....    def prin
-00002890: 745f 7265 7370 6f6e 7365 2873 656c 662c  t_response(self,
-000028a0: 206d 6574 686f 643a 2073 7472 2c20 7572   method: str, ur
-000028b0: 6c3a 2073 7472 2c20 7374 6174 7573 5f63  l: str, status_c
-000028c0: 6f64 653a 2069 6e74 293a 0d0a 2020 2020  ode: int):..    
-000028d0: 2020 2020 2222 220d 0a20 2020 2020 2020      """..       
-000028e0: 2060 7072 696e 745f 7265 7370 6f6e 7365   `print_response
-000028f0: 6020 2d20 5072 696e 7473 2074 6865 2072  ` - Prints the r
-00002900: 6573 706f 6e73 6520 6966 2064 6562 7567  esponse if debug
-00002910: 2069 7320 656e 6162 6c65 640d 0a0d 0a20   is enabled.... 
-00002920: 2020 2020 2020 2060 2a2a 5061 7261 6d65         `**Parame
-00002930: 7465 7273 2a2a 6060 0d0a 2020 2020 2020  ters**``..      
-00002940: 2020 2d20 606d 6574 686f 6460 202d 2054    - `method` - T
-00002950: 6865 2072 6571 7565 7374 206d 6574 686f  he request metho
-00002960: 6420 7573 6564 2e0d 0a20 2020 2020 2020  d used...       
-00002970: 202d 2060 7572 6c60 202d 2054 6865 2075   - `url` - The u
-00002980: 726c 2074 6865 2072 6571 7565 7374 2077  rl the request w
-00002990: 6173 2073 656e 7420 746f 2e0d 0a20 2020  as sent to...   
-000029a0: 2020 2020 202d 2060 7374 6174 7573 5f63       - `status_c
-000029b0: 6f64 6560 202d 2054 6865 2073 7461 7475  ode` - The statu
-000029c0: 7320 636f 6465 206f 6620 7468 6520 7265  s code of the re
-000029d0: 7370 6f6e 7365 2e0d 0a20 2020 2020 2020  sponse...       
-000029e0: 202d 2060 7265 7370 6f6e 7365 6020 2d20   - `response` - 
-000029f0: 5468 6520 7265 7370 6f6e 7365 2074 6f20  The response to 
-00002a00: 7072 696e 742e 0d0a 0d0a 2020 2020 2020  print.....      
-00002a10: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
-00002a20: 6620 7365 6c66 2e62 6f74 2e64 6562 7567  f self.bot.debug
-00002a30: 3a0d 0a20 2020 2020 2020 2020 2020 2063  :..            c
-00002a40: 6f6c 6f72 203d 2028 0d0a 2020 2020 2020  olor = (..      
-00002a50: 2020 2020 2020 2020 2020 466f 7265 2e52            Fore.R
-00002a60: 4544 0d0a 2020 2020 2020 2020 2020 2020  ED..            
-00002a70: 2020 2020 6966 2073 7461 7475 735f 636f      if status_co
-00002a80: 6465 2021 3d20 3230 300d 0a20 2020 2020  de != 200..     
-00002a90: 2020 2020 2020 2020 2020 2065 6c73 6520             else 
-00002aa0: 7b0d 0a20 2020 2020 2020 2020 2020 2020  {..             
-00002ab0: 2020 2020 2020 2022 4745 5422 3a20 466f         "GET": Fo
-00002ac0: 7265 2e42 4c55 452c 0d0a 2020 2020 2020  re.BLUE,..      
-00002ad0: 2020 2020 2020 2020 2020 2020 2020 2250                "P
-00002ae0: 4f53 5422 3a20 466f 7265 2e47 5245 454e  OST": Fore.GREEN
-00002af0: 2c0d 0a20 2020 2020 2020 2020 2020 2020  ,..             
-00002b00: 2020 2020 2020 2022 4445 4c45 5445 223a         "DELETE":
-00002b10: 2046 6f72 652e 4d41 4745 4e54 412c 0d0a   Fore.MAGENTA,..
-00002b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002b30: 2020 2020 224c 4954 4522 3a20 466f 7265      "LITE": Fore
-00002b40: 2e59 454c 4c4f 572c 0d0a 2020 2020 2020  .YELLOW,..      
-00002b50: 2020 2020 2020 2020 2020 7d2e 6765 7428            }.get(
-00002b60: 6d65 7468 6f64 2c20 466f 7265 2e52 4544  method, Fore.RED
-00002b70: 290d 0a20 2020 2020 2020 2020 2020 2029  )..            )
-00002b80: 0d0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
-00002b90: 696e 7428 6622 7b63 6f6c 6f72 7d7b 5374  int(f"{color}{St
-00002ba0: 796c 652e 4252 4947 4854 7d7b 6d65 7468  yle.BRIGHT}{meth
-00002bb0: 6f64 7d7b 5374 796c 652e 5245 5345 545f  od}{Style.RESET_
-00002bc0: 414c 4c7d 202d 207b 7572 6c7d 2229 0d0a  ALL} - {url}")..
-00002bd0: 0d0a 0d0a 2020 2020 6173 796e 6320 6465  ....    async de
-00002be0: 6620 636c 6f73 6528 7365 6c66 2920 2d3e  f close(self) ->
-00002bf0: 204e 6f6e 653a 0d0a 2020 2020 2020 2020   None:..        
-00002c00: 2222 2243 6c6f 7365 7320 7468 6520 4854  """Closes the HT
-00002c10: 5450 2073 6573 7369 6f6e 2e22 2222 0d0a  TP session."""..
-00002c20: 2020 2020 2020 2020 6177 6169 7420 7365          await se
-00002c30: 6c66 2e73 6573 7369 6f6e 2e63 6c6f 7365  lf.session.close
-00002c40: 2829                                     ()
+000004b0: 2046 616c 7365 0d0a 0d0a 2020 2020 2020   False....      
+000004c0: 2020 7365 6c66 2e70 726f 7879 203d 2070    self.proxy = p
+000004d0: 726f 7879 2069 6620 7072 6f78 7920 6973  roxy if proxy is
+000004e0: 206e 6f74 204e 6f6e 6520 656c 7365 204e   not None else N
+000004f0: 6f6e 650d 0a0d 0a20 2020 2020 2020 2073  one....        s
+00000500: 656c 662e 7265 7370 6f6e 7365 5f6d 6170  elf.response_map
+00000510: 203d 207b 0d0a 2020 2020 2020 2020 2020   = {..          
+00000520: 2020 3430 333a 2046 6f72 6269 6464 656e    403: Forbidden
+00000530: 2c0d 0a20 2020 2020 2020 2020 2020 2035  ,..            5
+00000540: 3032 3a20 4261 6447 6174 6577 6179 2c0d  02: BadGateway,.
+00000550: 0a20 2020 2020 2020 2020 2020 2035 3033  .            503
+00000560: 3a20 5365 7276 6963 6555 6e61 7661 696c  : ServiceUnavail
+00000570: 6162 6c65 0d0a 2020 2020 2020 2020 7d0d  able..        }.
+00000580: 0a0d 0a0d 0a20 2020 2061 7379 6e63 2064  .....    async d
+00000590: 6566 2069 6e69 7469 616c 697a 655f 7365  ef initialize_se
+000005a0: 7373 696f 6e28 7365 6c66 293a 0d0a 2020  ssion(self):..  
+000005b0: 2020 2020 2020 7365 6c66 2e73 6573 7369        self.sessi
+000005c0: 6f6e 203d 2043 6c69 656e 7453 6573 7369  on = ClientSessi
+000005d0: 6f6e 2829 0d0a 0d0a 0d0a 2020 2020 6173  on()......    as
+000005e0: 796e 6320 6465 6620 636c 6f73 655f 7365  ync def close_se
+000005f0: 7373 696f 6e28 7365 6c66 293a 0d0a 2020  ssion(self):..  
+00000600: 2020 2020 2020 6966 2073 656c 662e 7365        if self.se
+00000610: 7373 696f 6e20 6973 206e 6f74 204e 6f6e  ssion is not Non
+00000620: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000630: 6177 6169 7420 7365 6c66 2e73 6573 7369  await self.sessi
+00000640: 6f6e 2e63 6c6f 7365 2829 0d0a 0d0a 0d0a  on.close()......
+00000650: 2020 2020 6465 6620 7365 7276 6963 655f      def service_
+00000660: 7572 6c28 7365 6c66 2c20 7572 6c3a 2073  url(self, url: s
+00000670: 7472 2920 2d3e 2073 7472 3a0d 0a20 2020  tr) -> str:..   
+00000680: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00000690: 2020 6073 6572 7669 6365 5f75 726c 6020    `service_url` 
+000006a0: 2d20 4170 7065 6e64 7320 7468 6520 656e  - Appends the en
+000006b0: 6470 6f69 6e74 2074 6f20 7468 6520 7365  dpoint to the se
+000006c0: 7276 6963 6520 7572 6c0d 0a0d 0a20 2020  rvice url....   
+000006d0: 2020 2020 2060 2a2a 5061 7261 6d65 7465       `**Paramete
+000006e0: 7273 2a2a 6060 0d0a 2020 2020 2020 2020  rs**``..        
+000006f0: 2d20 6075 726c 6020 2d20 5468 6520 656e  - `url` - The en
+00000700: 6470 6f69 6e74 2074 6f20 6170 7065 6e64  dpoint to append
+00000710: 2074 6f20 7468 6520 7365 7276 6963 6520   to the service 
+00000720: 7572 6c2e 0d0a 0d0a 2020 2020 2020 2020  url.....        
+00000730: 602a 2a52 6574 7572 6e73 2a2a 6060 0d0a  `**Returns**``..
+00000740: 2020 2020 2020 2020 2d20 6073 7472 6020          - `str` 
+00000750: 2d20 5468 6520 7365 7276 6963 6520 7572  - The service ur
+00000760: 6c2e 0d0a 0d0a 2020 2020 2020 2020 2222  l.....        ""
+00000770: 220d 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+00000780: 6e20 6622 6874 7470 3a2f 2f73 6572 7669  n f"http://servi
+00000790: 6365 2e61 6d69 6e6f 6170 7073 2e63 6f6d  ce.aminoapps.com
+000007a0: 2f61 7069 2f76 317b 7572 6c7d 2220 6966  /api/v1{url}" if
+000007b0: 2075 726c 2e73 7461 7274 7377 6974 6828   url.startswith(
+000007c0: 222f 2229 2065 6c73 6520 7572 6c0d 0a0d  "/") else url...
+000007d0: 0a20 2020 2061 7379 6e63 2064 6566 2073  .    async def s
+000007e0: 6572 7669 6365 5f68 6561 6465 7273 2873  ervice_headers(s
+000007f0: 656c 6629 202d 3e20 6469 6374 3a0d 0a20  elf) -> dict:.. 
+00000800: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
+00000810: 7320 7468 6520 7365 7276 6963 6520 6865  s the service he
+00000820: 6164 6572 7322 2222 0d0a 2020 2020 2020  aders"""..      
+00000830: 2020 7265 7475 726e 207b 0d0a 2020 2020    return {..    
+00000840: 2020 2020 2020 2020 224e 4443 4c41 4e47          "NDCLANG
+00000850: 223a 2022 656e 222c 0d0a 2020 2020 2020  ": "en",..      
+00000860: 2020 2020 2020 2241 4343 4550 542d 4c41        "ACCEPT-LA
+00000870: 4e47 5541 4745 223a 2022 656e 2d55 5322  NGUAGE": "en-US"
+00000880: 2c0d 0a20 2020 2020 2020 2020 2020 2022  ,..            "
+00000890: 5553 4552 2d41 4745 4e54 223a 2022 4170  USER-AGENT": "Ap
+000008a0: 706c 6520 6950 686f 6e65 3133 2c34 2069  ple iPhone13,4 i
+000008b0: 4f53 2076 3135 2e36 2e31 204d 6169 6e2f  OS v15.6.1 Main/
+000008c0: 332e 3132 2e39 222c 0d0a 2020 2020 2020  3.12.9",..      
+000008d0: 2020 2020 2020 2248 4f53 5422 3a20 2273        "HOST": "s
+000008e0: 6572 7669 6365 2e61 6d69 6e6f 6170 7073  ervice.aminoapps
+000008f0: 2e63 6f6d 222c 0d0a 2020 2020 2020 2020  .com",..        
+00000900: 2020 2020 2243 4f4e 4e45 4354 494f 4e22      "CONNECTION"
+00000910: 3a20 224b 6565 702d 416c 6976 6522 2c0d  : "Keep-Alive",.
+00000920: 0a20 2020 2020 2020 2020 2020 2022 4143  .            "AC
+00000930: 4345 5054 2d45 4e43 4f44 494e 4722 3a20  CEPT-ENCODING": 
+00000940: 2267 7a69 702c 2064 6566 6c61 7465 2c20  "gzip, deflate, 
+00000950: 6272 222c 0d0a 2020 2020 2020 2020 2020  br",..          
+00000960: 2020 224e 4443 4155 5448 223a 2066 2273    "NDCAUTH": f"s
+00000970: 6964 3d7b 7365 6c66 2e73 6964 7d22 2c0d  id={self.sid}",.
+00000980: 0a20 2020 2020 2020 2020 2020 2022 4155  .            "AU
+00000990: 4944 223a 2073 656c 662e 7573 6572 4964  ID": self.userId
+000009a0: 206f 7220 7374 7228 7575 6964 3428 2929   or str(uuid4())
+000009b0: 0d0a 2020 2020 2020 2020 7d0d 0a0d 0a0d  ..        }.....
+000009c0: 0a20 2020 2061 7379 6e63 2064 6566 2066  .    async def f
+000009d0: 6574 6368 5f72 6571 7565 7374 2873 656c  etch_request(sel
+000009e0: 662c 206d 6574 686f 643a 2073 7472 2920  f, method: str) 
+000009f0: 2d3e 2043 616c 6c61 626c 653a 0d0a 2020  -> Callable:..  
+00000a00: 2020 2020 2020 2222 220d 0a20 2020 2020        """..     
+00000a10: 2020 2060 6665 7463 685f 7265 7175 6573     `fetch_reques
+00000a20: 7460 202d 2052 6574 7572 6e73 2074 6865  t` - Returns the
+00000a30: 2072 6571 7565 7374 206d 6574 686f 640d   request method.
+00000a40: 0a0d 0a20 2020 2020 2020 2060 2a2a 5061  ...        `**Pa
+00000a50: 7261 6d65 7465 7273 2a2a 6060 0d0a 2020  rameters**``..  
+00000a60: 2020 2020 2020 2d20 606d 6574 686f 6460        - `method`
+00000a70: 202d 2054 6865 2072 6571 7565 7374 206d   - The request m
+00000a80: 6574 686f 6420 746f 2072 6574 7572 6e2e  ethod to return.
+00000a90: 0d0a 0d0a 2020 2020 2020 2020 602a 2a52  ....        `**R
+00000aa0: 6574 7572 6e73 2a2a 6060 0d0a 2020 2020  eturns**``..    
+00000ab0: 2020 2020 2d20 6043 616c 6c61 626c 6560      - `Callable`
+00000ac0: 202d 2054 6865 2072 6571 7565 7374 206d   - The request m
+00000ad0: 6574 686f 642e 0d0a 0d0a 2020 2020 2020  ethod.....      
+00000ae0: 2020 2222 220d 0a20 2020 2020 2020 2072    """..        r
+00000af0: 6571 7565 7374 5f6d 6574 686f 6473 203d  equest_methods =
+00000b00: 207b 0d0a 2020 2020 2020 2020 2020 2020   {..            
+00000b10: 2247 4554 223a 2073 656c 662e 7365 7373  "GET": self.sess
+00000b20: 696f 6e2e 6765 742c 0d0a 2020 2020 2020  ion.get,..      
+00000b30: 2020 2020 2020 2250 4f53 5422 3a20 7365        "POST": se
+00000b40: 6c66 2e73 6573 7369 6f6e 2e70 6f73 742c  lf.session.post,
+00000b50: 0d0a 2020 2020 2020 2020 2020 2020 2244  ..            "D
+00000b60: 454c 4554 4522 3a20 7365 6c66 2e73 6573  ELETE": self.ses
+00000b70: 7369 6f6e 2e64 656c 6574 652c 0d0a 2020  sion.delete,..  
+00000b80: 2020 2020 2020 7d0d 0a20 2020 2020 2020        }..       
+00000b90: 2072 6574 7572 6e20 7265 7175 6573 745f   return request_
+00000ba0: 6d65 7468 6f64 735b 6d65 7468 6f64 5d0d  methods[method].
+00000bb0: 0a0d 0a0d 0a20 2020 2061 7379 6e63 2064  .....    async d
+00000bc0: 6566 2073 656e 645f 7265 7175 6573 7428  ef send_request(
+00000bd0: 0d0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+00000be0: 6c66 2c0d 0a20 2020 2020 2020 2020 2020  lf,..           
+00000bf0: 206d 6574 686f 643a 2073 7472 2c0d 0a20   method: str,.. 
+00000c00: 2020 2020 2020 2020 2020 2075 726c 3a20             url: 
+00000c10: 7374 722c 0d0a 2020 2020 2020 2020 2020  str,..          
+00000c20: 2020 6461 7461 3a20 556e 696f 6e5b 6469    data: Union[di
+00000c30: 6374 2c20 6279 7465 732c 204e 6f6e 655d  ct, bytes, None]
+00000c40: 2c0d 0a20 2020 2020 2020 2020 2020 2068  ,..            h
+00000c50: 6561 6465 7273 3a20 6469 6374 2c0d 0a20  eaders: dict,.. 
+00000c60: 2020 2020 2020 2020 2020 2063 6f6e 7465             conte
+00000c70: 6e74 5f74 7970 653a 204f 7074 696f 6e61  nt_type: Optiona
+00000c80: 6c5b 7374 725d 0d0a 2020 2020 2920 2d3e  l[str]..    ) ->
+00000c90: 2055 6e69 6f6e 5b69 6e74 2c20 7374 725d   Union[int, str]
+00000ca0: 3a0d 0a20 2020 2020 2020 2022 2222 0d0a  :..        """..
+00000cb0: 2020 2020 2020 2020 6073 656e 645f 7265          `send_re
+00000cc0: 7175 6573 7460 202d 2053 656e 6473 2061  quest` - Sends a
+00000cd0: 2072 6571 7565 7374 0d0a 0d0a 2020 2020   request....    
+00000ce0: 2020 2020 602a 2a50 6172 616d 6574 6572      `**Parameter
+00000cf0: 732a 2a60 600d 0a20 2020 2020 2020 202d  s**``..        -
+00000d00: 2060 6d65 7468 6f64 6020 2d20 5468 6520   `method` - The 
+00000d10: 7265 7175 6573 7420 6d65 7468 6f64 2074  request method t
+00000d20: 6f20 7573 652e 0d0a 2020 2020 2020 2020  o use...        
+00000d30: 2d20 6075 726c 6020 2d20 5468 6520 7572  - `url` - The ur
+00000d40: 6c20 746f 2073 656e 6420 7468 6520 7265  l to send the re
+00000d50: 7175 6573 7420 746f 2e0d 0a20 2020 2020  quest to...     
+00000d60: 2020 202d 2060 6461 7461 6020 2d20 5468     - `data` - Th
+00000d70: 6520 6461 7461 2074 6f20 7365 6e64 2077  e data to send w
+00000d80: 6974 6820 7468 6520 7265 7175 6573 742e  ith the request.
+00000d90: 0d0a 2020 2020 2020 2020 2d20 6068 6561  ..        - `hea
+00000da0: 6465 7273 6020 2d20 5468 6520 6865 6164  ders` - The head
+00000db0: 6572 7320 746f 2073 656e 6420 7769 7468  ers to send with
+00000dc0: 2074 6865 2072 6571 7565 7374 2e0d 0a20   the request... 
+00000dd0: 2020 2020 2020 202d 2060 636f 6e74 656e         - `conten
+00000de0: 745f 7479 7065 6020 2d20 5468 6520 636f  t_type` - The co
+00000df0: 6e74 656e 7420 7479 7065 206f 6620 7468  ntent type of th
+00000e00: 6520 6461 7461 2e0d 0a0d 0a20 2020 2020  e data.....     
+00000e10: 2020 2060 2a2a 5265 7475 726e 732a 2a60     `**Returns**`
+00000e20: 600d 0a20 2020 2020 2020 202d 2060 556e  `..        - `Un
+00000e30: 696f 6e5b 696e 742c 2073 7472 5d60 202d  ion[int, str]` -
+00000e40: 2054 6865 2073 7461 7475 7320 636f 6465   The status code
+00000e50: 2061 6e64 2072 6573 706f 6e73 6520 6672   and response fr
+00000e60: 6f6d 2074 6865 2072 6571 7565 7374 2e0d  om the request..
+00000e70: 0a0d 0a20 2020 2020 2020 2022 2222 0d0a  ...        """..
+00000e80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00000e90: 7365 7373 696f 6e20 6973 204e 6f6e 653a  session is None:
+00000ea0: 0d0a 2020 2020 2020 2020 2020 2020 6177  ..            aw
+00000eb0: 6169 7420 7365 6c66 2e69 6e69 7469 616c  ait self.initial
+00000ec0: 697a 655f 7365 7373 696f 6e28 290d 0a0d  ize_session()...
+00000ed0: 0a20 2020 2020 2020 2074 7279 3a0d 0a20  .        try:.. 
+00000ee0: 2020 2020 2020 2020 2020 2061 7379 6e63             async
+00000ef0: 2077 6974 6820 7365 6c66 2e73 6573 7369   with self.sessi
+00000f00: 6f6e 2e72 6571 7565 7374 280d 0a20 2020  on.request(..   
+00000f10: 2020 2020 2020 2020 2020 2020 206d 6574               met
+00000f20: 686f 642c 2075 726c 2c20 6461 7461 3d64  hod, url, data=d
+00000f30: 6174 612c 2068 6561 6465 7273 3d68 6561  ata, headers=hea
+00000f40: 6465 7273 2c20 7072 6f78 793d 7365 6c66  ders, proxy=self
+00000f50: 2e70 726f 7879 0d0a 2020 2020 2020 2020  .proxy..        
+00000f60: 2020 2020 2920 6173 2072 6573 706f 6e73      ) as respons
+00000f70: 653a 0d0a 2020 2020 2020 2020 2020 2020  e:..            
+00000f80: 2020 2020 7265 7475 726e 2072 6573 706f      return respo
+00000f90: 6e73 652e 7374 6174 7573 2c20 6177 6169  nse.status, awai
+00000fa0: 7420 7265 7370 6f6e 7365 2e74 6578 7428  t response.text(
+00000fb0: 290d 0a20 2020 2020 2020 2065 7863 6570  )..        excep
+00000fc0: 7420 280d 0a20 2020 2020 2020 2020 2020  t (..           
+00000fd0: 2054 7970 6545 7272 6f72 2c0d 0a20 2020   TypeError,..   
+00000fe0: 2020 2020 2020 2020 2043 6c69 656e 7445           ClientE
+00000ff0: 7272 6f72 2c0d 0a20 2020 2020 2020 2020  rror,..         
+00001000: 2020 2043 6c69 656e 7443 6f6e 6e65 6374     ClientConnect
+00001010: 696f 6e45 7272 6f72 2c0d 0a20 2020 2020  ionError,..     
+00001020: 2020 2020 2020 2043 6c69 656e 744f 5345         ClientOSE
+00001030: 7272 6f72 2c0d 0a20 2020 2020 2020 2020  rror,..         
+00001040: 2020 2043 6c69 656e 7443 6f6e 6e65 6374     ClientConnect
+00001050: 6f72 4572 726f 722c 0d0a 2020 2020 2020  orError,..      
+00001060: 2020 2020 2020 436c 6965 6e74 5072 6f78        ClientProx
+00001070: 7943 6f6e 6e65 6374 696f 6e45 7272 6f72  yConnectionError
+00001080: 2c0d 0a20 2020 2020 2020 2020 2020 2043  ,..            C
+00001090: 6c69 656e 7453 534c 4572 726f 722c 0d0a  lientSSLError,..
+000010a0: 2020 2020 2020 2020 2020 2020 436c 6965              Clie
+000010b0: 6e74 436f 6e6e 6563 746f 7253 534c 4572  ntConnectorSSLEr
+000010c0: 726f 722c 0d0a 2020 2020 2020 2020 2020  ror,..          
+000010d0: 2020 436c 6965 6e74 436f 6e6e 6563 746f    ClientConnecto
+000010e0: 7243 6572 7469 6669 6361 7465 4572 726f  rCertificateErro
+000010f0: 722c 0d0a 2020 2020 2020 2020 2020 2020  r,..            
+00001100: 5365 7276 6572 436f 6e6e 6563 7469 6f6e  ServerConnection
+00001110: 4572 726f 722c 0d0a 2020 2020 2020 2020  Error,..        
+00001120: 2020 2020 5365 7276 6572 5469 6d65 6f75      ServerTimeou
+00001130: 7445 7272 6f72 2c0d 0a20 2020 2020 2020  tError,..       
+00001140: 2020 2020 2053 6572 7665 7244 6973 636f       ServerDisco
+00001150: 6e6e 6563 7465 6445 7272 6f72 2c0d 0a20  nnectedError,.. 
+00001160: 2020 2020 2020 2020 2020 2053 6572 7665             Serve
+00001170: 7246 696e 6765 7270 7269 6e74 4d69 736d  rFingerprintMism
+00001180: 6174 6368 2c0d 0a20 2020 2020 2020 2020  atch,..         
+00001190: 2020 2043 6c69 656e 7452 6573 706f 6e73     ClientRespons
+000011a0: 6545 7272 6f72 2c0d 0a20 2020 2020 2020  eError,..       
+000011b0: 2020 2020 2043 6c69 656e 7448 7474 7050       ClientHttpP
+000011c0: 726f 7879 4572 726f 722c 0d0a 2020 2020  roxyError,..    
+000011d0: 2020 2020 2020 2020 5753 5365 7276 6572          WSServer
+000011e0: 4861 6e64 7368 616b 6545 7272 6f72 2c0d  HandshakeError,.
+000011f0: 0a20 2020 2020 2020 2029 3a0d 0a20 2020  .        ):..   
+00001200: 2020 2020 2020 2020 2061 7761 6974 2073           await s
+00001210: 656c 662e 6861 6e64 6c65 7228 6d65 7468  elf.handler(meth
+00001220: 6f64 2c20 7572 6c2c 2064 6174 612c 2063  od, url, data, c
+00001230: 6f6e 7465 6e74 5f74 7970 6529 0d0a 0d0a  ontent_type)....
+00001240: 0d0a 2020 2020 6173 796e 6320 6465 6620  ..    async def 
+00001250: 6861 6e64 6c65 7228 0d0a 2020 2020 2020  handler(..      
+00001260: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+00001270: 2020 2020 2020 2020 206d 6574 686f 643a           method:
+00001280: 2073 7472 2c0d 0a20 2020 2020 2020 2020   str,..         
+00001290: 2020 2075 726c 3a20 7374 722c 0d0a 2020     url: str,..  
+000012a0: 2020 2020 2020 2020 2020 6461 7461 3a20            data: 
+000012b0: 556e 696f 6e5b 6469 6374 2c20 6279 7465  Union[dict, byte
+000012c0: 732c 204e 6f6e 655d 203d 204e 6f6e 652c  s, None] = None,
+000012d0: 0d0a 2020 2020 2020 2020 2020 2020 636f  ..            co
+000012e0: 6e74 656e 745f 7479 7065 3a20 4f70 7469  ntent_type: Opti
+000012f0: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00001300: 0d0a 2020 2020 2920 2d3e 2064 6963 743a  ..    ) -> dict:
+00001310: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+00001320: 2020 2020 2020 2060 6861 6e64 6c65 7260         `handler`
+00001330: 202d 2048 616e 646c 6573 2061 6c6c 2072   - Handles all r
+00001340: 6571 7565 7374 730d 0a0d 0a20 2020 2020  equests....     
+00001350: 2020 2060 2a2a 5061 7261 6d65 7465 7273     `**Parameters
+00001360: 2a2a 6060 0d0a 2020 2020 2020 2020 2d20  **``..        - 
+00001370: 606d 6574 686f 6460 202d 2054 6865 2072  `method` - The r
+00001380: 6571 7565 7374 206d 6574 686f 6420 746f  equest method to
+00001390: 2075 7365 2e0d 0a20 2020 2020 2020 202d   use...        -
+000013a0: 2060 7572 6c60 202d 2054 6865 2075 726c   `url` - The url
+000013b0: 2074 6f20 7365 6e64 2074 6865 2072 6571   to send the req
+000013c0: 7565 7374 2074 6f2e 0d0a 2020 2020 2020  uest to...      
+000013d0: 2020 2d20 6064 6174 6160 202d 2054 6865    - `data` - The
+000013e0: 2064 6174 6120 746f 2073 656e 6420 7769   data to send wi
+000013f0: 7468 2074 6865 2072 6571 7565 7374 2e0d  th the request..
+00001400: 0a20 2020 2020 2020 202d 2060 636f 6e74  .        - `cont
+00001410: 656e 745f 7479 7065 6020 2d20 5468 6520  ent_type` - The 
+00001420: 636f 6e74 656e 7420 7479 7065 206f 6620  content type of 
+00001430: 7468 6520 6461 7461 2e0d 0a0d 0a20 2020  the data.....   
+00001440: 2020 2020 2060 2a2a 5265 7475 726e 732a       `**Returns*
+00001450: 2a60 600d 0a20 2020 2020 2020 202d 2060  *``..        - `
+00001460: 6469 6374 6020 2d20 5468 6520 7265 7370  dict` - The resp
+00001470: 6f6e 7365 2066 726f 6d20 7468 6520 7265  onse from the re
+00001480: 7175 6573 742e 0d0a 0d0a 2020 2020 2020  quest.....      
+00001490: 2020 2222 220d 0a20 2020 2020 2020 2075    """..        u
+000014a0: 726c 203d 2073 656c 662e 7365 7276 6963  rl = self.servic
+000014b0: 655f 7572 6c28 7572 6c29 0d0a 0d0a 2020  e_url(url)....  
+000014c0: 2020 2020 2020 7572 6c2c 2068 6561 6465        url, heade
+000014d0: 7273 2c20 6269 6e61 7279 5f64 6174 6120  rs, binary_data 
+000014e0: 3d20 6177 6169 7420 7365 6c66 2e73 6572  = await self.ser
+000014f0: 7669 6365 5f68 616e 646c 6572 2875 726c  vice_handler(url
+00001500: 2c20 6461 7461 2c20 636f 6e74 656e 745f  , data, content_
+00001510: 7479 7065 290d 0a0d 0a20 2020 2020 2020  type)....       
+00001520: 2069 6620 616c 6c28 5b6d 6574 686f 6420   if all([method 
+00001530: 3d3d 2022 504f 5354 222c 2064 6174 6120  == "POST", data 
+00001540: 6973 204e 6f6e 655d 293a 0d0a 2020 2020  is None]):..    
+00001550: 2020 2020 2020 2020 6865 6164 6572 735b          headers[
+00001560: 2243 4f4e 5445 4e54 2d54 5950 4522 5d20  "CONTENT-TYPE"] 
+00001570: 3d20 2261 7070 6c69 6361 7469 6f6e 2f6f  = "application/o
+00001580: 6374 6574 2d73 7472 6561 6d22 0d0a 0d0a  ctet-stream"....
+00001590: 2020 2020 2020 2020 7472 793a 0d0a 2020          try:..  
+000015a0: 2020 2020 2020 2020 2020 7374 6174 7573            status
+000015b0: 5f63 6f64 652c 2063 6f6e 7465 6e74 203d  _code, content =
+000015c0: 2061 7761 6974 2073 656c 662e 7365 6e64   await self.send
+000015d0: 5f72 6571 7565 7374 280d 0a20 2020 2020  _request(..     
+000015e0: 2020 2020 2020 2020 2020 206d 6574 686f             metho
+000015f0: 642c 2075 726c 2c20 6269 6e61 7279 5f64  d, url, binary_d
+00001600: 6174 612c 2068 6561 6465 7273 2c20 636f  ata, headers, co
+00001610: 6e74 656e 745f 7479 7065 0d0a 2020 2020  ntent_type..    
+00001620: 2020 2020 2020 2020 290d 0a20 2020 2020          )..     
+00001630: 2020 2065 7863 6570 7420 4578 6365 7074     except Except
+00001640: 696f 6e20 6173 2065 3a0d 0a20 2020 2020  ion as e:..     
+00001650: 2020 2020 2020 2070 7269 6e74 2865 290d         print(e).
+00001660: 0a0d 0a20 2020 2020 2020 2073 656c 662e  ...        self.
+00001670: 7072 696e 745f 7265 7370 6f6e 7365 286d  print_response(m
+00001680: 6574 686f 643d 6d65 7468 6f64 2c20 7572  ethod=method, ur
+00001690: 6c3d 7572 6c2c 2073 7461 7475 735f 636f  l=url, status_co
+000016a0: 6465 3d73 7461 7475 735f 636f 6465 290d  de=status_code).
+000016b0: 0a0d 0a20 2020 2020 2020 2072 6574 7572  ...        retur
+000016c0: 6e20 7365 6c66 2e68 616e 646c 655f 7265  n self.handle_re
+000016d0: 7370 6f6e 7365 2873 7461 7475 735f 636f  sponse(status_co
+000016e0: 6465 3d73 7461 7475 735f 636f 6465 2c20  de=status_code, 
+000016f0: 7265 7370 6f6e 7365 3d63 6f6e 7465 6e74  response=content
+00001700: 290d 0a0d 0a0d 0a20 2020 2061 7379 6e63  )......    async
+00001710: 2064 6566 2073 6572 7669 6365 5f68 616e   def service_han
+00001720: 646c 6572 280d 0a20 2020 2020 2020 2020  dler(..         
+00001730: 2020 2073 656c 662c 0d0a 2020 2020 2020     self,..      
+00001740: 2020 2020 2020 7572 6c3a 2073 7472 2c0d        url: str,.
+00001750: 0a20 2020 2020 2020 2020 2020 2064 6174  .            dat
+00001760: 613a 2055 6e69 6f6e 5b64 6963 742c 2062  a: Union[dict, b
+00001770: 7974 6573 2c20 4e6f 6e65 5d20 3d20 4e6f  ytes, None] = No
+00001780: 6e65 2c0d 0a20 2020 2020 2020 2020 2020  ne,..           
+00001790: 2063 6f6e 7465 6e74 5f74 7970 653a 204f   content_type: O
+000017a0: 7074 696f 6e61 6c5b 7374 725d 203d 204e  ptional[str] = N
+000017b0: 6f6e 650d 0a20 2020 2029 202d 3e20 5475  one..    ) -> Tu
+000017c0: 706c 655b 7374 722c 2064 6963 742c 2055  ple[str, dict, U
+000017d0: 6e69 6f6e 5b64 6963 742c 2062 7974 6573  nion[dict, bytes
+000017e0: 2c20 4e6f 6e65 5d5d 3a0d 0a20 2020 2020  , None]]:..     
+000017f0: 2020 2022 2222 0d0a 2020 2020 2020 2020     """..        
+00001800: 6073 6572 7669 6365 5f68 616e 646c 6572  `service_handler
+00001810: 6020 2d20 5369 676e 7320 7468 6520 7265  ` - Signs the re
+00001820: 7175 6573 7420 616e 6420 7265 7475 726e  quest and return
+00001830: 7320 7468 6520 7365 7276 6963 6520 7572  s the service ur
+00001840: 6c2c 2068 6561 6465 7273 2061 6e64 2064  l, headers and d
+00001850: 6174 610d 0a0d 0a20 2020 2020 2020 2060  ata....        `
+00001860: 2a2a 5061 7261 6d65 7465 7273 2a2a 6060  **Parameters**``
+00001870: 0d0a 2020 2020 2020 2020 2d20 6075 726c  ..        - `url
+00001880: 6020 2d20 5468 6520 7572 6c20 746f 2073  ` - The url to s
+00001890: 656e 6420 7468 6520 7265 7175 6573 7420  end the request 
+000018a0: 746f 2e0d 0a20 2020 2020 2020 202d 2060  to...        - `
+000018b0: 6461 7461 6020 2d20 5468 6520 6461 7461  data` - The data
+000018c0: 2074 6f20 7365 6e64 2077 6974 6820 7468   to send with th
+000018d0: 6520 7265 7175 6573 742e 0d0a 2020 2020  e request...    
+000018e0: 2020 2020 2d20 6063 6f6e 7465 6e74 5f74      - `content_t
+000018f0: 7970 6560 202d 2054 6865 2063 6f6e 7465  ype` - The conte
+00001900: 6e74 2074 7970 6520 6f66 2074 6865 2064  nt type of the d
+00001910: 6174 612e 0d0a 0d0a 2020 2020 2020 2020  ata.....        
+00001920: 602a 2a52 6574 7572 6e73 2a2a 6060 0d0a  `**Returns**``..
+00001930: 2020 2020 2020 2020 2d20 6054 7570 6c65          - `Tuple
+00001940: 5b73 7472 2c20 6469 6374 2c20 556e 696f  [str, dict, Unio
+00001950: 6e5b 6469 6374 2c20 6279 7465 732c 204e  n[dict, bytes, N
+00001960: 6f6e 655d 5d60 202d 2054 6865 2073 6572  one]]` - The ser
+00001970: 7669 6365 2075 726c 2c20 6865 6164 6572  vice url, header
+00001980: 7320 616e 6420 6461 7461 2e0d 0a0d 0a20  s and data..... 
+00001990: 2020 2020 2020 2022 2222 0d0a 0d0a 2020         """....  
+000019a0: 2020 2020 2020 6865 6164 6572 7320 3d20        headers = 
+000019b0: 7b22 4e44 4344 4556 4943 4549 4422 3a20  {"NDCDEVICEID": 
+000019c0: 6465 7669 6365 5f69 6428 292c 202a 2a61  device_id(), **a
+000019d0: 7761 6974 2073 656c 662e 7365 7276 6963  wait self.servic
+000019e0: 655f 6865 6164 6572 7328 297d 0d0a 0d0a  e_headers()}....
+000019f0: 2020 2020 2020 2020 6966 2064 6174 6120          if data 
+00001a00: 6f72 2063 6f6e 7465 6e74 5f74 7970 653a  or content_type:
+00001a10: 0d0a 2020 2020 2020 2020 2020 2020 6865  ..            he
+00001a20: 6164 6572 732c 2064 6174 6120 3d20 6177  aders, data = aw
+00001a30: 6169 7420 7365 6c66 2e66 6574 6368 5f73  ait self.fetch_s
+00001a40: 6967 6e61 7475 7265 2864 6174 612c 2068  ignature(data, h
+00001a50: 6561 6465 7273 2c20 636f 6e74 656e 745f  eaders, content_
+00001a60: 7479 7065 290d 0a0d 0a20 2020 2020 2020  type)....       
+00001a70: 2072 6574 7572 6e20 7572 6c2c 2068 6561   return url, hea
+00001a80: 6465 7273 2c20 7365 6c66 2e65 6e73 7572  ders, self.ensur
+00001a90: 655f 7574 6638 2864 6174 6129 0d0a 0d0a  e_utf8(data)....
+00001aa0: 0d0a 2020 2020 6465 6620 656e 7375 7265  ..    def ensure
+00001ab0: 5f75 7466 3828 7365 6c66 2c20 6461 7461  _utf8(self, data
+00001ac0: 3a20 556e 696f 6e5b 6469 6374 2c20 6279  : Union[dict, by
+00001ad0: 7465 732c 204e 6f6e 655d 2920 2d3e 2055  tes, None]) -> U
+00001ae0: 6e69 6f6e 5b64 6963 742c 2062 7974 6573  nion[dict, bytes
+00001af0: 2c20 4e6f 6e65 5d3a 0d0a 2020 2020 2020  , None]:..      
+00001b00: 2020 2222 220d 0a20 2020 2020 2020 2060    """..        `
+00001b10: 656e 7375 7265 5f75 7466 3860 202d 2045  ensure_utf8` - E
+00001b20: 6e73 7572 6573 2074 6865 2064 6174 6120  nsures the data 
+00001b30: 6973 2075 7466 2d38 2065 6e63 6f64 6564  is utf-8 encoded
+00001b40: 0d0a 0d0a 2020 2020 2020 2020 602a 2a50  ....        `**P
+00001b50: 6172 616d 6574 6572 732a 2a60 600d 0a20  arameters**``.. 
+00001b60: 2020 2020 2020 202d 2060 6461 7461 6020         - `data` 
+00001b70: 2d20 5468 6520 6461 7461 2074 6f20 656e  - The data to en
+00001b80: 636f 6465 2e0d 0a0d 0a20 2020 2020 2020  code.....       
+00001b90: 2060 2a2a 5265 7475 726e 732a 2a60 600d   `**Returns**``.
+00001ba0: 0a20 2020 2020 2020 202d 2060 556e 696f  .        - `Unio
+00001bb0: 6e5b 6469 6374 2c20 6279 7465 732c 204e  n[dict, bytes, N
+00001bc0: 6f6e 655d 6020 2d20 5468 6520 656e 636f  one]` - The enco
+00001bd0: 6465 6420 6461 7461 2e0d 0a0d 0a20 2020  ded data.....   
+00001be0: 2020 2020 2022 2222 0d0a 0d0a 2020 2020       """....    
+00001bf0: 2020 2020 6966 2064 6174 6120 6973 204e      if data is N
+00001c00: 6f6e 653a 0d0a 2020 2020 2020 2020 2020  one:..          
+00001c10: 2020 7265 7475 726e 2064 6174 610d 0a0d    return data...
+00001c20: 0a20 2020 2020 2020 2064 6566 2068 616e  .        def han
+00001c30: 646c 655f 6469 6374 2864 6174 613a 2064  dle_dict(data: d
+00001c40: 6963 7429 3a0d 0a20 2020 2020 2020 2020  ict):..         
+00001c50: 2020 2072 6574 7572 6e20 7b6b 6579 3a20     return {key: 
+00001c60: 7365 6c66 2e65 6e73 7572 655f 7574 6638  self.ensure_utf8
+00001c70: 2876 616c 7565 2920 666f 7220 6b65 792c  (value) for key,
+00001c80: 2076 616c 7565 2069 6e20 6461 7461 2e69   value in data.i
+00001c90: 7465 6d73 2829 7d0d 0a0d 0a20 2020 2020  tems()}....     
+00001ca0: 2020 2064 6566 2068 616e 646c 655f 7374     def handle_st
+00001cb0: 7228 6461 7461 3a20 7374 7229 3a0d 0a20  r(data: str):.. 
+00001cc0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00001cd0: 6e20 6461 7461 2e65 6e63 6f64 6528 2275  n data.encode("u
+00001ce0: 7466 2d38 2229 0d0a 0d0a 2020 2020 2020  tf-8")....      
+00001cf0: 2020 6861 6e64 6c65 7273 203d 207b 0d0a    handlers = {..
+00001d00: 2020 2020 2020 2020 2020 2020 6469 6374              dict
+00001d10: 3a20 6861 6e64 6c65 5f64 6963 742c 0d0a  : handle_dict,..
+00001d20: 2020 2020 2020 2020 2020 2020 7374 723a              str:
+00001d30: 2068 616e 646c 655f 7374 720d 0a20 2020   handle_str..   
+00001d40: 2020 2020 207d 0d0a 0d0a 2020 2020 2020       }....      
+00001d50: 2020 7265 7475 726e 2068 616e 646c 6572    return handler
+00001d60: 732e 6765 7428 7479 7065 2864 6174 6129  s.get(type(data)
+00001d70: 2c20 6c61 6d62 6461 2078 3a20 7829 2864  , lambda x: x)(d
+00001d80: 6174 6129 0d0a 0d0a 0d0a 2020 2020 6173  ata)......    as
+00001d90: 796e 6320 6465 6620 6665 7463 685f 7369  ync def fetch_si
+00001da0: 676e 6174 7572 6528 0d0a 2020 2020 2020  gnature(..      
+00001db0: 2020 2020 2020 7365 6c66 2c0d 0a20 2020        self,..   
+00001dc0: 2020 2020 2020 2020 2064 6174 613a 2055           data: U
+00001dd0: 6e69 6f6e 5b64 6963 742c 2062 7974 6573  nion[dict, bytes
+00001de0: 2c20 4e6f 6e65 5d2c 0d0a 2020 2020 2020  , None],..      
+00001df0: 2020 2020 2020 6865 6164 6572 733a 2064        headers: d
+00001e00: 6963 742c 0d0a 2020 2020 2020 2020 2020  ict,..          
+00001e10: 2020 636f 6e74 656e 745f 7479 7065 3a20    content_type: 
+00001e20: 7374 7220 3d20 4e6f 6e65 0d0a 2020 2020  str = None..    
+00001e30: 2920 2d3e 2054 7570 6c65 5b64 6963 742c  ) -> Tuple[dict,
+00001e40: 2055 6e69 6f6e 5b64 6963 742c 2062 7974   Union[dict, byt
+00001e50: 6573 2c20 4e6f 6e65 5d5d 3a0d 0a20 2020  es, None]]:..   
+00001e60: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00001e70: 2020 6066 6574 6368 5f73 6967 6e61 7475    `fetch_signatu
+00001e80: 7265 6020 2d20 4665 7463 6865 7320 7468  re` - Fetches th
+00001e90: 6520 7369 676e 6174 7572 6520 616e 6420  e signature and 
+00001ea0: 7265 7475 726e 7320 7468 6520 6461 7461  returns the data
+00001eb0: 2061 6e64 2075 7064 6174 6564 2068 6561   and updated hea
+00001ec0: 6465 7273 0d0a 0d0a 2020 2020 2020 2020  ders....        
+00001ed0: 602a 2a50 6172 616d 6574 6572 732a 2a60  `**Parameters**`
+00001ee0: 600d 0a20 2020 2020 2020 202d 2060 6461  `..        - `da
+00001ef0: 7461 6020 2d20 5468 6520 6461 7461 2074  ta` - The data t
+00001f00: 6f20 7365 6e64 2077 6974 6820 7468 6520  o send with the 
+00001f10: 7265 7175 6573 742e 0d0a 2020 2020 2020  request...      
+00001f20: 2020 2d20 6068 6561 6465 7273 6020 2d20    - `headers` - 
+00001f30: 5468 6520 6865 6164 6572 7320 746f 2073  The headers to s
+00001f40: 656e 6420 7769 7468 2074 6865 2072 6571  end with the req
+00001f50: 7565 7374 2e0d 0a20 2020 2020 2020 202d  uest...        -
+00001f60: 2060 636f 6e74 656e 745f 7479 7065 6020   `content_type` 
+00001f70: 2d20 5468 6520 636f 6e74 656e 7420 7479  - The content ty
+00001f80: 7065 206f 6620 7468 6520 6461 7461 2e0d  pe of the data..
+00001f90: 0a0d 0a20 2020 2020 2020 2060 2a2a 5265  ...        `**Re
+00001fa0: 7475 726e 732a 2a60 600d 0a20 2020 2020  turns**``..     
+00001fb0: 2020 202d 2060 5475 706c 655b 6469 6374     - `Tuple[dict
+00001fc0: 2c20 556e 696f 6e5b 6469 6374 2c20 6279  , Union[dict, by
+00001fd0: 7465 732c 204e 6f6e 655d 5d60 202d 2054  tes, None]]` - T
+00001fe0: 6865 2068 6561 6465 7273 2061 6e64 2064  he headers and d
+00001ff0: 6174 612e 0d0a 0d0a 2020 2020 2020 2020  ata.....        
+00002000: 2222 220d 0a0d 0a20 2020 2020 2020 2069  """....        i
+00002010: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
+00002020: 2864 6174 612c 2062 7974 6573 293a 0d0a  (data, bytes):..
+00002030: 2020 2020 2020 2020 2020 2020 6461 7461              data
+00002040: 203d 2028 0d0a 2020 2020 2020 2020 2020   = (..          
+00002050: 2020 2020 2020 6f72 6a73 6f6e 5f64 756d        orjson_dum
+00002060: 7073 2864 6174 6129 2e64 6563 6f64 6528  ps(data).decode(
+00002070: 2275 7466 2d38 2229 0d0a 2020 2020 2020  "utf-8")..      
+00002080: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00002090: 662e 6f72 6a73 6f6e 0d0a 2020 2020 2020  f.orjson..      
+000020a0: 2020 2020 2020 2020 2020 656c 7365 2064            else d
+000020b0: 756d 7073 2864 6174 6129 0d0a 2020 2020  umps(data)..    
+000020c0: 2020 2020 2020 2020 290d 0a0d 0a20 2020          )....   
+000020d0: 2020 2020 2068 6561 6465 7273 2e75 7064       headers.upd
+000020e0: 6174 6528 0d0a 2020 2020 2020 2020 2020  ate(..          
+000020f0: 2020 7b0d 0a20 2020 2020 2020 2020 2020    {..           
+00002100: 2020 2020 2022 434f 4e54 454e 542d 4c45       "CONTENT-LE
+00002110: 4e47 5448 223a 2066 227b 6c65 6e28 6461  NGTH": f"{len(da
+00002120: 7461 297d 222c 0d0a 2020 2020 2020 2020  ta)}",..        
+00002130: 2020 2020 2020 2020 2243 4f4e 5445 4e54          "CONTENT
+00002140: 2d54 5950 4522 3a20 636f 6e74 656e 745f  -TYPE": content_
+00002150: 7479 7065 206f 7220 2261 7070 6c69 6361  type or "applica
+00002160: 7469 6f6e 2f6a 736f 6e3b 2063 6861 7273  tion/json; chars
+00002170: 6574 3d75 7466 2d38 222c 0d0a 2020 2020  et=utf-8",..    
+00002180: 2020 2020 2020 2020 2020 2020 224e 4443              "NDC
+00002190: 2d4d 5347 2d53 4947 223a 2067 656e 6572  -MSG-SIG": gener
+000021a0: 6174 655f 7369 676e 6174 7572 6528 6461  ate_signature(da
+000021b0: 7461 292c 0d0a 2020 2020 2020 2020 2020  ta),..          
+000021c0: 2020 7d0d 0a20 2020 2020 2020 2029 0d0a    }..        )..
+000021d0: 2020 2020 2020 2020 7265 7475 726e 2068          return h
+000021e0: 6561 6465 7273 2c20 6461 7461 0d0a 0d0a  eaders, data....
+000021f0: 0d0a 2020 2020 6465 6620 7261 6973 655f  ..    def raise_
+00002200: 6572 726f 7228 7365 6c66 2c20 7265 7370  error(self, resp
+00002210: 6f6e 7365 3a20 6469 6374 2920 2d3e 204e  onse: dict) -> N
+00002220: 6f6e 653a 0d0a 2020 2020 2020 2020 2222  one:..        ""
+00002230: 220d 0a20 2020 2020 2020 2060 7261 6973  "..        `rais
+00002240: 655f 6572 726f 7260 202d 2052 6169 7365  e_error` - Raise
+00002250: 7320 616e 2065 7272 6f72 2069 6620 616e  s an error if an
+00002260: 2065 7272 6f72 2069 7320 696e 2074 6865   error is in the
+00002270: 2072 6573 706f 6e73 650d 0a0d 0a20 2020   response....   
+00002280: 2020 2020 2060 2a2a 5061 7261 6d65 7465       `**Paramete
+00002290: 7273 2a2a 6060 0d0a 2020 2020 2020 2020  rs**``..        
+000022a0: 2d20 6072 6573 706f 6e73 6560 202d 2054  - `response` - T
+000022b0: 6865 2072 6573 706f 6e73 6520 6672 6f6d  he response from
+000022c0: 2074 6865 2072 6571 7565 7374 2e0d 0a0d   the request....
+000022d0: 0a20 2020 2020 2020 2060 2a2a 5265 7475  .        `**Retu
+000022e0: 726e 732a 2a60 600d 0a20 2020 2020 2020  rns**``..       
+000022f0: 202d 2060 4e6f 6e65 6020 2d20 5261 6973   - `None` - Rais
+00002300: 6573 2061 6e20 6572 726f 7220 6966 2074  es an error if t
+00002310: 6865 2073 7461 7475 7320 636f 6465 2069  he status code i
+00002320: 7320 696e 2074 6865 2072 6573 706f 6e73  s in the respons
+00002330: 6520 6d61 702e 0d0a 0d0a 2020 2020 2020  e map.....      
+00002340: 2020 2222 220d 0a20 2020 2020 2020 2069    """..        i
+00002350: 6620 616c 6c28 0d0a 2020 2020 2020 2020  f all(..        
+00002360: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
+00002370: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002380: 6573 706f 6e73 652e 6765 7428 2261 7069  esponse.get("api
+00002390: 3a73 7461 7475 7363 6f64 6522 2c20 3230  :statuscode", 20
+000023a0: 3029 203d 3d20 3130 352c 0d0a 2020 2020  0) == 105,..    
+000023b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000023c0: 6861 7361 7474 7228 7365 6c66 2c20 2265  hasattr(self, "e
+000023d0: 6d61 696c 2229 2c0d 0a20 2020 2020 2020  mail"),..       
+000023e0: 2020 2020 2020 2020 2020 2020 2068 6173               has
+000023f0: 6174 7472 2873 656c 662c 2022 7061 7373  attr(self, "pass
+00002400: 776f 7264 2229 2c0d 0a20 2020 2020 2020  word"),..       
+00002410: 2020 2020 2020 2020 205d 0d0a 2020 2020           ]..    
+00002420: 2020 2020 293a 0d0a 2020 2020 2020 2020      ):..        
+00002430: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+00002440: 626f 742e 7275 6e28 7365 6c66 2e65 6d61  bot.run(self.ema
+00002450: 696c 2c20 7365 6c66 2e70 6173 7377 6f72  il, self.passwor
+00002460: 642c 2075 7365 5f63 6163 6865 3d46 616c  d, use_cache=Fal
+00002470: 7365 290d 0a0d 0a20 2020 2020 2020 2065  se)....        e
+00002480: 6c73 653a 0d0a 2020 2020 2020 2020 2020  lse:..          
+00002490: 2020 7261 6973 6520 4150 4945 7863 6570    raise APIExcep
+000024a0: 7469 6f6e 2872 6573 706f 6e73 6529 0d0a  tion(response)..
+000024b0: 0d0a 0d0a 2020 2020 6465 6620 6861 6e64  ....    def hand
+000024c0: 6c65 5f72 6573 706f 6e73 6528 7365 6c66  le_response(self
+000024d0: 2c20 7374 6174 7573 5f63 6f64 653a 2069  , status_code: i
+000024e0: 6e74 2c20 7265 7370 6f6e 7365 3a20 7374  nt, response: st
+000024f0: 7229 202d 3e20 6469 6374 3a0d 0a20 2020  r) -> dict:..   
+00002500: 2020 2020 2022 2222 0d0a 2020 2020 2020       """..      
+00002510: 2020 6068 616e 646c 655f 7265 7370 6f6e    `handle_respon
+00002520: 7365 6020 2d20 4861 6e64 6c65 7320 7468  se` - Handles th
+00002530: 6520 7265 7370 6f6e 7365 2061 6e64 2072  e response and r
+00002540: 6574 7572 6e73 2074 6865 2072 6573 706f  eturns the respo
+00002550: 6e73 6520 6173 2061 2064 6963 740d 0a0d  nse as a dict...
+00002560: 0a20 2020 2020 2020 2060 2a2a 5061 7261  .        `**Para
+00002570: 6d65 7465 7273 2a2a 6060 0d0a 2020 2020  meters**``..    
+00002580: 2020 2020 2d20 6073 7461 7475 735f 636f      - `status_co
+00002590: 6465 6020 2d20 5468 6520 7374 6174 7573  de` - The status
+000025a0: 2063 6f64 6520 6f66 2074 6865 2072 6573   code of the res
+000025b0: 706f 6e73 652e 0d0a 2020 2020 2020 2020  ponse...        
+000025c0: 2d20 6072 6573 706f 6e73 6560 202d 2054  - `response` - T
+000025d0: 6865 2072 6573 706f 6e73 6520 746f 2068  he response to h
+000025e0: 616e 646c 652e 0d0a 0d0a 2020 2020 2020  andle.....      
+000025f0: 2020 602a 2a52 6574 7572 6e73 2a2a 6060    `**Returns**``
+00002600: 0d0a 2020 2020 2020 2020 2d20 6064 6963  ..        - `dic
+00002610: 7460 202d 2054 6865 2072 6573 706f 6e73  t` - The respons
+00002620: 6520 6173 2061 2064 6963 742e 0d0a 0d0a  e as a dict.....
+00002630: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00002640: 2020 2020 2069 6620 7374 6174 7573 5f63       if status_c
+00002650: 6f64 6520 696e 2073 656c 662e 7265 7370  ode in self.resp
+00002660: 6f6e 7365 5f6d 6170 3a0d 0a20 2020 2020  onse_map:..     
+00002670: 2020 2020 2020 2072 6169 7365 2073 656c         raise sel
+00002680: 662e 7265 7370 6f6e 7365 5f6d 6170 5b73  f.response_map[s
+00002690: 7461 7475 735f 636f 6465 5d0d 0a0d 0a20  tatus_code].... 
+000026a0: 2020 2020 2020 2065 6c69 6620 7265 7370         elif resp
+000026b0: 6f6e 7365 2e73 7461 7274 7377 6974 6828  onse.startswith(
+000026c0: 226e 756c 6c22 293a 0d0a 2020 2020 2020  "null"):..      
+000026d0: 2020 2020 2020 7261 6973 6520 4e75 6c6c        raise Null
+000026e0: 5265 7370 6f6e 7365 0d0a 0d0a 2020 2020  Response....    
+000026f0: 2020 2020 656c 7365 3a0d 0a0d 0a20 2020      else:....   
+00002700: 2020 2020 2020 2020 2074 7279 3a0d 0a20           try:.. 
+00002710: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00002720: 6573 706f 6e73 6520 3d20 280d 0a20 2020  esponse = (..   
+00002730: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002740: 206f 726a 736f 6e5f 6c6f 6164 7328 7265   orjson_loads(re
+00002750: 7370 6f6e 7365 290d 0a20 2020 2020 2020  sponse)..       
+00002760: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00002770: 7365 6c66 2e6f 726a 736f 6e0d 0a20 2020  self.orjson..   
+00002780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002790: 2065 6c73 6520 6c6f 6164 7328 7265 7370   else loads(resp
+000027a0: 6f6e 7365 290d 0a20 2020 2020 2020 2020  onse)..         
+000027b0: 2020 2020 2020 2029 0d0a 2020 2020 2020         )..      
+000027c0: 2020 2020 2020 6578 6365 7074 2045 7863        except Exc
+000027d0: 6570 7469 6f6e 3a0d 0a20 2020 2020 2020  eption:..       
+000027e0: 2020 2020 2020 2020 2072 6573 706f 6e73           respons
+000027f0: 6520 3d20 6c6f 6164 7328 7265 7370 6f6e  e = loads(respon
+00002800: 7365 290d 0a0d 0a20 2020 2020 2020 2020  se)....         
+00002810: 2020 2069 6620 7374 6174 7573 5f63 6f64     if status_cod
+00002820: 6520 213d 2032 3030 3a0d 0a20 2020 2020  e != 200:..     
+00002830: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00002840: 7261 6973 655f 6572 726f 7228 7265 7370  raise_error(resp
+00002850: 6f6e 7365 290d 0a0d 0a20 2020 2020 2020  onse)....       
+00002860: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+00002870: 6f6e 7365 0d0a 0d0a 0d0a 2020 2020 6465  onse......    de
+00002880: 6620 7072 696e 745f 7265 7370 6f6e 7365  f print_response
+00002890: 2873 656c 662c 206d 6574 686f 643a 2073  (self, method: s
+000028a0: 7472 2c20 7572 6c3a 2073 7472 2c20 7374  tr, url: str, st
+000028b0: 6174 7573 5f63 6f64 653a 2069 6e74 293a  atus_code: int):
+000028c0: 0d0a 2020 2020 2020 2020 2222 220d 0a20  ..        """.. 
+000028d0: 2020 2020 2020 2060 7072 696e 745f 7265         `print_re
+000028e0: 7370 6f6e 7365 6020 2d20 5072 696e 7473  sponse` - Prints
+000028f0: 2074 6865 2072 6573 706f 6e73 6520 6966   the response if
+00002900: 2064 6562 7567 2069 7320 656e 6162 6c65   debug is enable
+00002910: 640d 0a0d 0a20 2020 2020 2020 2060 2a2a  d....        `**
+00002920: 5061 7261 6d65 7465 7273 2a2a 6060 0d0a  Parameters**``..
+00002930: 2020 2020 2020 2020 2d20 606d 6574 686f          - `metho
+00002940: 6460 202d 2054 6865 2072 6571 7565 7374  d` - The request
+00002950: 206d 6574 686f 6420 7573 6564 2e0d 0a20   method used... 
+00002960: 2020 2020 2020 202d 2060 7572 6c60 202d         - `url` -
+00002970: 2054 6865 2075 726c 2074 6865 2072 6571   The url the req
+00002980: 7565 7374 2077 6173 2073 656e 7420 746f  uest was sent to
+00002990: 2e0d 0a20 2020 2020 2020 202d 2060 7374  ...        - `st
+000029a0: 6174 7573 5f63 6f64 6560 202d 2054 6865  atus_code` - The
+000029b0: 2073 7461 7475 7320 636f 6465 206f 6620   status code of 
+000029c0: 7468 6520 7265 7370 6f6e 7365 2e0d 0a20  the response... 
+000029d0: 2020 2020 2020 202d 2060 7265 7370 6f6e         - `respon
+000029e0: 7365 6020 2d20 5468 6520 7265 7370 6f6e  se` - The respon
+000029f0: 7365 2074 6f20 7072 696e 742e 0d0a 0d0a  se to print.....
+00002a00: 2020 2020 2020 2020 2222 220d 0a20 2020          """..   
+00002a10: 2020 2020 2069 6620 7365 6c66 2e62 6f74       if self.bot
+00002a20: 2e64 6562 7567 3a0d 0a20 2020 2020 2020  .debug:..       
+00002a30: 2020 2020 2063 6f6c 6f72 203d 2028 0d0a       color = (..
+00002a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002a50: 466f 7265 2e52 4544 0d0a 2020 2020 2020  Fore.RED..      
+00002a60: 2020 2020 2020 2020 2020 6966 2073 7461            if sta
+00002a70: 7475 735f 636f 6465 2021 3d20 3230 300d  tus_code != 200.
+00002a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00002a90: 2065 6c73 6520 7b0d 0a20 2020 2020 2020   else {..       
+00002aa0: 2020 2020 2020 2020 2020 2020 2022 4745               "GE
+00002ab0: 5422 3a20 466f 7265 2e42 4c55 452c 0d0a  T": Fore.BLUE,..
+00002ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002ad0: 2020 2020 2250 4f53 5422 3a20 466f 7265      "POST": Fore
+00002ae0: 2e47 5245 454e 2c0d 0a20 2020 2020 2020  .GREEN,..       
+00002af0: 2020 2020 2020 2020 2020 2020 2022 4445               "DE
+00002b00: 4c45 5445 223a 2046 6f72 652e 4d41 4745  LETE": Fore.MAGE
+00002b10: 4e54 412c 0d0a 2020 2020 2020 2020 2020  NTA,..          
+00002b20: 2020 2020 2020 2020 2020 224c 4954 4522            "LITE"
+00002b30: 3a20 466f 7265 2e59 454c 4c4f 572c 0d0a  : Fore.YELLOW,..
+00002b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002b50: 7d2e 6765 7428 6d65 7468 6f64 2c20 466f  }.get(method, Fo
+00002b60: 7265 2e52 4544 290d 0a20 2020 2020 2020  re.RED)..       
+00002b70: 2020 2020 2029 0d0a 2020 2020 2020 2020       )..        
+00002b80: 2020 2020 7072 696e 7428 6622 7b63 6f6c      print(f"{col
+00002b90: 6f72 7d7b 5374 796c 652e 4252 4947 4854  or}{Style.BRIGHT
+00002ba0: 7d7b 6d65 7468 6f64 7d7b 5374 796c 652e  }{method}{Style.
+00002bb0: 5245 5345 545f 414c 4c7d 202d 207b 7572  RESET_ALL} - {ur
+00002bc0: 6c7d 2229 0d0a 0d0a 0d0a 2020 2020 6173  l}")......    as
+00002bd0: 796e 6320 6465 6620 636c 6f73 6528 7365  ync def close(se
+00002be0: 6c66 2920 2d3e 204e 6f6e 653a 0d0a 2020  lf) -> None:..  
+00002bf0: 2020 2020 2020 2222 2243 6c6f 7365 7320        """Closes 
+00002c00: 7468 6520 4854 5450 2073 6573 7369 6f6e  the HTTP session
+00002c10: 2e22 2222 0d0a 2020 2020 2020 2020 6177  ."""..        aw
+00002c20: 6169 7420 7365 6c66 2e73 6573 7369 6f6e  ait self.session
+00002c30: 2e63 6c6f 7365 2829                      .close()
```

### Comparing `pymino-1.1.8.4/pymino/ext/utilities/commands.py` & `pymino-1.1.8.5/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/utilities/generate.py` & `pymino-1.1.8.5/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino/ext/utilities/request_handler.py` & `pymino-1.1.8.5/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/pymino.egg-info/PKG-INFO` & `pymino-1.1.8.5/pymino.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.8.4
+Version: 1.1.8.5
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.8.4 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.8.5 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.8.4/pymino.egg-info/SOURCES.txt` & `pymino-1.1.8.5/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.8.4/setup.cfg` & `pymino-1.1.8.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e38 2e34 0d0a 6175  on = 1.1.8.4..au
+00000020: 6f6e 203d 2031 2e31 2e38 2e35 0d0a 6175  on = 1.1.8.5..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.8.4/setup.py` & `pymino-1.1.8.5/setup.py`

 * *Files identical despite different names*


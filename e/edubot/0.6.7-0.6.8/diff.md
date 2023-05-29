# Comparing `tmp/edubot-0.6.7.tar.gz` & `tmp/edubot-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edubot-0.6.7.tar", max compression
+gzip compressed data, was "edubot-0.6.8.tar", max compression
```

## Comparing `edubot-0.6.7.tar` & `edubot-0.6.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-02-13 07:21:16.493245 edubot-0.6.7/LICENSE
--rw-r--r--   0        0        0     1400 2023-05-04 15:06:07.555469 edubot-0.6.7/README.md
--rw-r--r--   0        0        0      894 2023-05-05 09:01:03.030249 edubot-0.6.7/edubot/__init__.py
--rw-r--r--   0        0        0    19121 2023-05-05 11:34:06.447210 edubot-0.6.7/edubot/bot.py
--rw-r--r--   0        0        0     2950 2023-02-13 07:21:16.496579 edubot-0.6.7/edubot/sql.py
--rw-r--r--   0        0        0      636 2023-05-05 09:45:44.455107 edubot-0.6.7/edubot/types.py
--rw-r--r--   0        0        0      632 2023-05-05 11:34:18.684158 edubot-0.6.7/pyproject.toml
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 edubot-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-13 07:21:16.493245 edubot-0.6.8/LICENSE
+-rw-r--r--   0        0        0     1400 2023-05-04 15:06:07.555469 edubot-0.6.8/README.md
+-rw-r--r--   0        0        0      894 2023-05-05 09:01:03.030249 edubot-0.6.8/edubot/__init__.py
+-rw-r--r--   0        0        0    19428 2023-05-29 09:39:28.101401 edubot-0.6.8/edubot/bot.py
+-rw-r--r--   0        0        0     2950 2023-02-13 07:21:16.496579 edubot-0.6.8/edubot/sql.py
+-rw-r--r--   0        0        0      636 2023-05-05 09:45:44.455107 edubot-0.6.8/edubot/types.py
+-rw-r--r--   0        0        0      632 2023-05-29 09:44:42.044374 edubot-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 edubot-0.6.8/PKG-INFO
```

### Comparing `edubot-0.6.7/LICENSE` & `edubot-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `edubot-0.6.7/README.md` & `edubot-0.6.8/README.md`

 * *Files identical despite different names*

### Comparing `edubot-0.6.7/edubot/__init__.py` & `edubot-0.6.8/edubot/__init__.py`

 * *Files identical despite different names*

### Comparing `edubot-0.6.7/edubot/bot.py` & `edubot-0.6.8/edubot/bot.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 from edubot import DREAMSTUDIO_KEY, OPENAI_KEY, REPLICATE_KEY
 from edubot.sql import Bot, Completion, Message, Session, Thread
 from edubot.types import CompletionInfo, ImageInfo, MessageInfo
 
 # The maximum number of GPT tokens that chat context can be.
 # The limit for GPT-4 is 8192.
-# We limit to 7800 to allow extra room for the response and the personality.
+# We limit to 7200 to allow extra room for the response and the personality.
 MAX_GPT_TOKENS = 7200
 
 # The maximum allowed size of images in megabytes
 MAX_IMAGE_SIZE_MB = 50
 
 # Prompt for GPT to summarise web pages
 WEB_SUMMARY_PROMPT = (
@@ -199,16 +199,19 @@
 
         system_messages = [
             {"role": "system", "content": "You are a chatbot named " + self.username},
             {"role": "system", "content": f"Your personality is: {personality}"},
             {
                 "role": "system",
                 "content": "You should pretend you can view images. "
-                "A description of images will be saved in the chat logs, you can use that to get a sense of "
-                "what the images are about.",
+                "Descriptions of images posted to the chat will be saved to the database. "
+                "These descriptions are in the form: '*A picture of ____'. "
+                "When you spot these descriptions you should pretend you can see the image, using the description. "
+                "Do not mention that you cannot see the image, or that you are instead viewing a description of"
+                "the image. Just pretend like you can see it.",
             },
             {
                 "role": "system",
                 "content": f"The current year is: {datetime.datetime.now().year}",
             },
             {
                 "role": "system",
@@ -314,41 +317,41 @@
                 if row_as_msg_info not in new_context:
                     existing_context.append(row_as_msg_info)
 
             # The existing context in this timeframe + the new messages
             complete_context: list[MessageInfo] = []
 
             for index, msg in enumerate(new_context):
-                # If the message is already in the database
-                if self.__get_message(msg) is not None:
-                    continue
-
-                # If the message was written by a bot
-                if self.__get_bot(msg["username"]) is not None:
-                    continue
-
-                row: dict = msg
-                row["thread"] = thread.id
-
-                session.add(Message(**row))
-
                 # Figure out where to insert the extra context chronologically
                 for extra_msg in existing_context:
                     check = extra_msg["time"] < msg["time"]
                     if index > 0:
                         check = (
                             check and extra_msg["time"] > new_context[index - 1]["time"]
                         )
 
                     if check:
                         complete_context.append(extra_msg)
                         existing_context.remove(extra_msg)
 
                 complete_context.append(msg)
 
+                # If the message is already in the database
+                if self.__get_message(msg) is not None:
+                    continue
+
+                # If the message was written by a bot
+                if self.__get_bot(msg["username"]) is not None:
+                    continue
+
+                row: dict = msg
+                row["thread"] = thread.id
+
+                session.add(Message(**row))
+
             session.commit()
 
         gpt_context = self.__format_context(
             complete_context, personality_override=personality_override
         )
 
         try:
```

### Comparing `edubot-0.6.7/edubot/sql.py` & `edubot-0.6.8/edubot/sql.py`

 * *Files identical despite different names*

### Comparing `edubot-0.6.7/edubot/types.py` & `edubot-0.6.8/edubot/types.py`

 * *Files identical despite different names*

### Comparing `edubot-0.6.7/pyproject.toml` & `edubot-0.6.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edubot"
-version = "0.6.7"
+version = "0.6.8"
 description = ""
 authors = ["exciteabletom <tom@digitalnook.net>", "moodler <martin@moodle.com>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `edubot-0.6.7/PKG-INFO` & `edubot-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edubot
-Version: 0.6.7
+Version: 0.6.8
 Summary: 
 License: GPLv3
 Author: exciteabletom
 Author-email: tom@digitalnook.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```


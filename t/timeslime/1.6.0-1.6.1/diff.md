# Comparing `tmp/timeslime-1.6.0-py3-none-any.whl.zip` & `tmp/timeslime-1.6.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 14639 bytes, number of entries: 19
--rw-r--r--  2.0 unx        0 b- defN 23-May-21 18:19 timeslime/__init__.py
--rw-r--r--  2.0 unx       52 b- defN 23-May-21 18:19 timeslime/__main__.py
--rw-r--r--  2.0 unx     6904 b- defN 23-May-21 18:19 timeslime/cli.py
--rw-r--r--  2.0 unx     1983 b- defN 23-May-21 18:19 timeslime/models.py
--rw-r--r--  2.0 unx     4429 b- defN 23-May-21 18:19 timeslime/serializer.py
--rw-r--r--  2.0 unx      489 b- defN 23-May-21 18:19 timeslime/handler/__init__.py
--rw-r--r--  2.0 unx     5997 b- defN 23-May-21 18:19 timeslime/handler/database_handler.py
--rw-r--r--  2.0 unx     1565 b- defN 23-May-21 18:19 timeslime/handler/ntp_server_handler.py
--rw-r--r--  2.0 unx     4287 b- defN 23-May-21 18:19 timeslime/handler/settings_handler.py
--rw-r--r--  2.0 unx     1092 b- defN 23-May-21 18:19 timeslime/handler/state_handler.py
--rw-r--r--  2.0 unx     7315 b- defN 23-May-21 18:19 timeslime/handler/timeslime_handler.py
--rw-r--r--  2.0 unx     5328 b- defN 23-May-21 18:19 timeslime/handler/timeslime_server_handler.py
--rw-rw-rw-  2.0 unx      534 b- defN 23-May-21 18:19 timeslime/update/1.2_to_1.3.sql
--rw-rw-rw-  2.0 unx     1072 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3073 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       54 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1617 b- defN 23-May-21 18:20 timeslime-1.6.0.dist-info/RECORD
-19 files, 45893 bytes uncompressed, 11971 bytes compressed:  73.9%
+Zip file size: 15067 bytes, number of entries: 19
+-rw-r--r--  2.0 unx        0 b- defN 23-May-29 17:19 timeslime/__init__.py
+-rw-r--r--  2.0 unx       52 b- defN 23-May-29 17:19 timeslime/__main__.py
+-rw-r--r--  2.0 unx     7047 b- defN 23-May-29 17:19 timeslime/cli.py
+-rw-r--r--  2.0 unx     1983 b- defN 23-May-29 17:19 timeslime/models.py
+-rw-r--r--  2.0 unx     4429 b- defN 23-May-29 17:19 timeslime/serializer.py
+-rw-r--r--  2.0 unx      489 b- defN 23-May-29 17:19 timeslime/handler/__init__.py
+-rw-r--r--  2.0 unx     5997 b- defN 23-May-29 17:19 timeslime/handler/database_handler.py
+-rw-r--r--  2.0 unx     1565 b- defN 23-May-29 17:19 timeslime/handler/ntp_server_handler.py
+-rw-r--r--  2.0 unx     4287 b- defN 23-May-29 17:19 timeslime/handler/settings_handler.py
+-rw-r--r--  2.0 unx     1092 b- defN 23-May-29 17:19 timeslime/handler/state_handler.py
+-rw-r--r--  2.0 unx     8726 b- defN 23-May-29 17:19 timeslime/handler/timeslime_handler.py
+-rw-r--r--  2.0 unx     5328 b- defN 23-May-29 17:19 timeslime/handler/timeslime_server_handler.py
+-rw-rw-rw-  2.0 unx      534 b- defN 23-May-29 17:19 timeslime/update/1.2_to_1.3.sql
+-rw-rw-rw-  2.0 unx     1072 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3073 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       54 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1617 b- defN 23-May-29 17:20 timeslime-1.6.1.dist-info/RECORD
+19 files, 47447 bytes uncompressed, 12399 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -33,26 +33,26 @@
 
 Filename: timeslime/handler/timeslime_server_handler.py
 Comment: 
 
 Filename: timeslime/update/1.2_to_1.3.sql
 Comment: 
 
-Filename: timeslime-1.6.0.dist-info/LICENSE
+Filename: timeslime-1.6.1.dist-info/LICENSE
 Comment: 
 
-Filename: timeslime-1.6.0.dist-info/METADATA
+Filename: timeslime-1.6.1.dist-info/METADATA
 Comment: 
 
-Filename: timeslime-1.6.0.dist-info/WHEEL
+Filename: timeslime-1.6.1.dist-info/WHEEL
 Comment: 
 
-Filename: timeslime-1.6.0.dist-info/entry_points.txt
+Filename: timeslime-1.6.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: timeslime-1.6.0.dist-info/top_level.txt
+Filename: timeslime-1.6.1.dist-info/top_level.txt
 Comment: 
 
-Filename: timeslime-1.6.0.dist-info/RECORD
+Filename: timeslime-1.6.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## timeslime/cli.py

```diff
@@ -41,25 +41,31 @@
 @click.option('--database', default=DATABASE_PATH, help='Defines path to the database. [ default: ~/.timeslime/data.db ]')
 @click.pass_context
 def main(ctx, database):
     """It's a tool to track your time."""
     ctx.ensure_object(dict)
     ctx.obj['database'] = database
 
-@main.command('start', short_help='Start your time')
+
+@main.command("start", short_help="Start your time")
+@click.argument("time", required=False)
 @click.pass_context
-def start(ctx):
+def start(ctx, time):
+    """start time"""
     timeslime_handler = boot(ctx.obj)
-    timeslime_handler.start_time()
+    timeslime_handler.start_time(time)
+
 
-@main.command('stop', short_help='Stop your time')
+@main.command("stop", short_help="Stop your time")
+@click.argument("time", required=False)
 @click.pass_context
-def stop(ctx):
+def stop(ctx, time):
+    """stop time"""
     timeslime_handler = boot(ctx.obj)
-    timeslime_handler.stop_time()
+    timeslime_handler.stop_time(time)
 
 @main.command('display', short_help='Display your time')
 @click.pass_context
 def display(ctx):
     timeslime_handler = boot(ctx.obj)
     elapsed_time = str(abs(timeslime_handler.get_elapsed_time()))
     print(elapsed_time)
```

## timeslime/handler/timeslime_handler.py

```diff
@@ -1,10 +1,11 @@
 """timeslime handler class"""
 from ast import literal_eval
 from datetime import date, datetime, timedelta, timezone
+from typing import Optional
 
 from peewee import DoesNotExist
 from requests.exceptions import ConnectionError as RequestConnectionError
 
 from timeslime.handler import (
     DatabaseHandler,
     NtpServerHandler,
@@ -20,22 +21,26 @@
     def __init__(
         self,
         settings_handler: SettingsHandler,
         database_handler: DatabaseHandler,
         ntp_server_handler: NtpServerHandler,
         state_handler: StateHandler = None,
         timeslime_server_handler: TimeslimeServerHandler = None,
+        today: Optional[datetime] = None,
     ):
+        """initialize timeslime handler
+        :param today: just for testing"""
         self.settings_handler = settings_handler
         self.database_handler = database_handler
         self.ntp_server_handler = ntp_server_handler
         self.state_handler = state_handler
         self.timeslime_server_handler = timeslime_server_handler
         self.on_start = None
         self.on_stop = None
+        self.today = today
 
         if self.settings_handler:
             self.settings_handler.sync()
             self._set_daily_working_time(self.settings_handler, date.today().weekday())
             self._set_timeslime_server_handler(self.settings_handler)
             self.sync()
 
@@ -64,45 +69,82 @@
             password = settings_handler.get("password")
             self.timeslime_server_handler = TimeslimeServerHandler(
                 timeslime_server.value, username.value, password.value
             )
         else:
             self.timeslime_server_handler = None
 
-    def start_time(self):
-        if not self.ntp_server_handler.ntp_server_is_synchronized:
-            print('NTP server is not synchronized yet. Wait a few seconds to get an accurate time tracking.')
-            return
+    def start_time(self, start_time_str: str = "") -> datetime:
+        """start time at current system time or at `start_time_str`
+        :param start_time_str: start time must be a valid time (e.g.: 8:00)"""
+        current_time = self.__get_time(start_time_str)
         self.stop_time()
         self.timespan = Timespan()
-        self.timespan.start_time = datetime.now(tz=timezone.utc)
+        self.timespan.start_time = current_time
         self.timespan = self.database_handler.save_timespan(self.timespan)
         if self.timeslime_server_handler is not None:
             try:
                 self.timeslime_server_handler.send_timespan(self.timespan)
             except RequestConnectionError:
                 pass
         if self.on_start is not None:
             self.on_start()
 
-    def stop_time(self):
-        if not self.ntp_server_handler.ntp_server_is_synchronized:
-            print('NTP server is not synchronized yet. Wait a few seconds to get an accurate time tracking.')
-            return
+        return self.timespan.start_time
+
+    def stop_time(self, stop_time_str: str = "") -> Optional[datetime]:
+        """stop time at current system time or at `stop_time_str`
+        :param stop_time_str: stop time must be a valid time (e.g.: 8:00)"""
+        current_time = self.__get_time(stop_time_str)
         if self.timespan is not None and self.timespan.start_time is not None and self.timespan.stop_time is None:
-            self.timespan.stop_time = datetime.now(tz=timezone.utc)
+            self.timespan.stop_time = current_time
             self.timespan = self.database_handler.save_timespan(self.timespan)
             if self.timeslime_server_handler is not None:
                 try:
                     self.timeslime_server_handler.send_timespan(self.timespan)
                 except RequestConnectionError:
                     pass
         if self.on_stop is not None:
             self.on_stop()
 
+        if self.timespan:
+            return self.timespan.stop_time
+
+        return None
+
+    def __get_time(self, time_str: str = ""):
+        """get time"""
+        if time_str:
+            if not self.today:
+                now = datetime.now()
+            else:
+                now = self.today
+            try:
+                requested_time = datetime.strptime(time_str, "%H:%M")
+            except ValueError as value_error:
+                raise ValueError(
+                    "Time must be in the format HH:mm (eg. 8:00)!"
+                ) from value_error
+            time = now.replace(
+                hour=requested_time.hour,
+                minute=requested_time.minute,
+                second=0,
+                microsecond=0,
+            )
+            time = time.astimezone(timezone.utc)
+        elif not self.ntp_server_handler.ntp_server_is_synchronized:
+            raise ValueError(
+                "NTP server is not synchronized yet. "
+                "Wait a few seconds to get an accurate time tracking."
+            )
+        else:
+            time = datetime.now(tz=timezone.utc)
+
+        return time
+
     def get_elapsed_time(self) -> bool:
         if not self.ntp_server_handler.ntp_server_is_synchronized:
             print('NTP server is not synchronized yet. Wait a few seconds to get an accurate time tracking.')
             return
         daily_sum_in_seconds = self.database_handler.get_tracked_time_in_seconds(
             datetime.now()
         )
```

## Comparing `timeslime-1.6.0.dist-info/LICENSE` & `timeslime-1.6.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `timeslime-1.6.0.dist-info/METADATA` & `timeslime-1.6.1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: timeslime
-Version: 1.6.0
+Version: 1.6.1
 Author: Christian Decker
 Author-email: christian.decker@lookslikematrix.de
 License: MIT
 Project-URL: Donate, https://www.buymeacoffee.com/lookslikematrix
 Project-URL: Source Code, https://gitlab.com/lookslikematrix/timeslime
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

## Comparing `timeslime-1.6.0.dist-info/RECORD` & `timeslime-1.6.1.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 timeslime/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 timeslime/__main__.py,sha256=D-c9Wts6p0sR6ES-shgtXLmF1nVCS_53ixj0OJ9IsMU,52
-timeslime/cli.py,sha256=me63ItWNoME_Tc9mklpi5SCva_f_PkE3bBuTRGFtVO0,6904
+timeslime/cli.py,sha256=HUsg4bAztn5QW56h_Fj86YS7q1nAPT9xm-D9FdjKei4,7047
 timeslime/models.py,sha256=maP58Mclu1aQgtEBAgdcf6U3iOAY4JxvRQoooJiDDLk,1983
 timeslime/serializer.py,sha256=M9V3jR722miV7IoXkxcjKVUfP1UOKIkQXzqwHZJqbhg,4429
 timeslime/handler/__init__.py,sha256=DgB8v_mx-6g0vIT5HBIO0GYCRbmBviytzDoT_eib4AI,489
 timeslime/handler/database_handler.py,sha256=f1hucZy8FUYMmR096TREf-dOgw5qES82pI8W4BHiKj8,5997
 timeslime/handler/ntp_server_handler.py,sha256=da6K6OX10MxvZaFDe5uHpjMGaEKpq0T7ew3x2SP8naQ,1565
 timeslime/handler/settings_handler.py,sha256=e59rOUrmBKnP7D8JbKXIAf0QI7QUXh_mkYtZyJCuObU,4287
 timeslime/handler/state_handler.py,sha256=4NbHzLnddWpPBqKZiQeMbJiF9DTc-2gDyB1gO7J6xx8,1092
-timeslime/handler/timeslime_handler.py,sha256=3Mg1JM5oRtGf-5AJm0vVPiIhb-zhNO02ZPmeUZHO0dk,7315
+timeslime/handler/timeslime_handler.py,sha256=FhfpHGIqAcYNZLfhCjI_11CO3R-GcLqKCDps3Nhejoo,8726
 timeslime/handler/timeslime_server_handler.py,sha256=4pmMifFKQHYGI9u-MQ-0jg7oninHzBY9Kv_vRugAAAI,5328
 timeslime/update/1.2_to_1.3.sql,sha256=LLuT0LCA9W4J-5kGuiqxJ9rEgq8cSr94v1GLC-oIRBA,534
-timeslime-1.6.0.dist-info/LICENSE,sha256=LiRYlunBxa9UIPdfV7F9IRSRSISLC7bCz-DubILGtgs,1072
-timeslime-1.6.0.dist-info/METADATA,sha256=0WhEHNcjGUS22PaKvTdi686Nwa-erNVzd3IxhpkZTpI,3073
-timeslime-1.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-timeslime-1.6.0.dist-info/entry_points.txt,sha256=MT9_31puJx5fzANMynwiNIhyhYsl0KWKYNkzK8PZB-g,54
-timeslime-1.6.0.dist-info/top_level.txt,sha256=kToBlgsTKvfE41ILjN4v6ZIQYLxFlROmu21LJPKmz8M,10
-timeslime-1.6.0.dist-info/RECORD,,
+timeslime-1.6.1.dist-info/LICENSE,sha256=LiRYlunBxa9UIPdfV7F9IRSRSISLC7bCz-DubILGtgs,1072
+timeslime-1.6.1.dist-info/METADATA,sha256=KKMysfH16H0u1367m3HHL8TWf0h9iDw9d5bSkhIc9-k,3073
+timeslime-1.6.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+timeslime-1.6.1.dist-info/entry_points.txt,sha256=MT9_31puJx5fzANMynwiNIhyhYsl0KWKYNkzK8PZB-g,54
+timeslime-1.6.1.dist-info/top_level.txt,sha256=kToBlgsTKvfE41ILjN4v6ZIQYLxFlROmu21LJPKmz8M,10
+timeslime-1.6.1.dist-info/RECORD,,
```


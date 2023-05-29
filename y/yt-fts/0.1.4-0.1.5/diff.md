# Comparing `tmp/yt-fts-0.1.4.tar.gz` & `tmp/yt-fts-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-fts-0.1.4.tar", last modified: Sun May 28 20:48:27 2023, max compression
+gzip compressed data, was "yt-fts-0.1.5.tar", last modified: Mon May 29 06:14:00 2023, max compression
```

## Comparing `yt-fts-0.1.4.tar` & `yt-fts-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 20:48:27.756508 yt-fts-0.1.4/
--rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 20:45:24.000000 yt-fts-0.1.4/LICENSE
--rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-28 20:48:27.755960 yt-fts-0.1.4/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     3718 2023-05-28 20:45:24.000000 yt-fts-0.1.4/README.md
--rw-r--r--   0 home       (501) staff       (20)       38 2023-05-28 20:48:27.756669 yt-fts-0.1.4/setup.cfg
--rw-r--r--   0 home       (501) staff       (20)      969 2023-05-28 20:47:54.000000 yt-fts-0.1.4/setup.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 20:48:27.750537 yt-fts-0.1.4/yt_fts/
--rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 20:45:24.000000 yt-fts-0.1.4/yt_fts/__init__.py
--rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 20:45:24.000000 yt-fts-0.1.4/yt_fts/__main__.py
--rw-r--r--   0 home       (501) staff       (20)     3203 2023-05-28 20:45:24.000000 yt-fts-0.1.4/yt_fts/db_scripts.py
--rw-r--r--   0 home       (501) staff       (20)    10150 2023-05-28 20:45:24.000000 yt-fts-0.1.4/yt_fts/yt_fts.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-28 20:48:27.755092 yt-fts-0.1.4/yt_fts.egg-info/
--rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)      284 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/SOURCES.txt
--rw-r--r--   0 home       (501) staff       (20)        1 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/dependency_links.txt
--rw-r--r--   0 home       (501) staff       (20)       45 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/entry_points.txt
--rw-r--r--   0 home       (501) staff       (20)      180 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/requires.txt
--rw-r--r--   0 home       (501) staff       (20)        7 2023-05-28 20:48:27.000000 yt-fts-0.1.4/yt_fts.egg-info/top_level.txt
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:14:00.162823 yt-fts-0.1.5/
+-rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 20:45:24.000000 yt-fts-0.1.5/LICENSE
+-rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-29 06:14:00.162170 yt-fts-0.1.5/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     3718 2023-05-28 20:45:24.000000 yt-fts-0.1.5/README.md
+-rw-r--r--   0 home       (501) staff       (20)       38 2023-05-29 06:14:00.163022 yt-fts-0.1.5/setup.cfg
+-rw-r--r--   0 home       (501) staff       (20)      969 2023-05-29 06:13:47.000000 yt-fts-0.1.5/setup.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:14:00.157585 yt-fts-0.1.5/yt_fts/
+-rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 20:45:24.000000 yt-fts-0.1.5/yt_fts/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 20:45:24.000000 yt-fts-0.1.5/yt_fts/__main__.py
+-rw-r--r--   0 home       (501) staff       (20)     2873 2023-05-29 05:22:56.000000 yt-fts-0.1.5/yt_fts/db_scripts.py
+-rw-r--r--   0 home       (501) staff       (20)    10682 2023-05-29 06:11:35.000000 yt-fts-0.1.5/yt_fts/yt_fts.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:14:00.161149 yt-fts-0.1.5/yt_fts.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-29 06:14:00.000000 yt-fts-0.1.5/yt_fts.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)      284 2023-05-29 06:14:00.000000 yt-fts-0.1.5/yt_fts.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2023-05-29 06:14:00.000000 yt-fts-0.1.5/yt_fts.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       45 2023-05-29 06:14:00.000000 yt-fts-0.1.5/yt_fts.egg-info/entry_points.txt
+-rw-r--r--   0 home       (501) staff       (20)      180 2023-05-29 06:14:00.000000 yt-fts-0.1.5/yt_fts.egg-info/requires.txt
+-rw-r--r--   0 home       (501) staff       (20)        7 2023-05-29 06:14:00.000000 yt-fts-0.1.5/yt_fts.egg-info/top_level.txt
```

### Comparing `yt-fts-0.1.4/LICENSE` & `yt-fts-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.4/PKG-INFO` & `yt-fts-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-fts
-Version: 0.1.4
+Version: 0.1.5
 Summary: yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.
 Home-page: https://github.com/NotJoeMartinez/yt-fts
 Author: NotJoeMartinez
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `yt-fts-0.1.4/README.md` & `yt-fts-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.4/setup.py` & `yt-fts-0.1.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'console_scripts': [
         'yt-fts=yt_fts.yt_fts:cli',
     ],
 }
 
 setup(
     name='yt-fts', 
-    version='0.1.4',
+    version='0.1.5',
     description='yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     author='NotJoeMartinez',
     url='https://github.com/NotJoeMartinez/yt-fts',  
     packages=find_packages(),
     install_requires=dependencies,
```

### Comparing `yt-fts-0.1.4/yt_fts/yt_fts.py` & `yt-fts-0.1.5/yt_fts/yt_fts.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 from yt_fts.db_scripts import *
 
 @click.group()
 def cli():
     make_db()
 
+
 @click.command(help="Lists channels")
 def list():
     click.echo("Listing channels")
     channels = get_channels()
     print(tabulate(channels, headers=["channel_id","channel_name", "channel_url"]))
 
 
@@ -39,29 +40,34 @@
         print("Error finding channel id try --channel-id option")
 
 
 @click.command( help='search [channel id] [search text]')
 @click.argument('channel_id', required=True)
 @click.argument('search_text', required=True)
 def search(channel_id, search_text):
-    click.echo(f'Searching for quotes in channel {channel_id} for text {search_text}')
+    if len(search_text) > 40:
+        show_message("search_too_long")
+        return
+    click.echo(f'Searching in channel {channel_id}')
     get_quotes(channel_id, search_text)
 
 
 @click.command( help='export [channel id] [search text] ')
 @click.argument('channel_id', required=True)
 @click.argument('search_text', required=True)
 def export(channel_id, search_text):
+    if len(search_text) > 40:
+        show_message("search_too_long")
+        return
     timestamp = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
     file_name = f'{channel_id}_{timestamp}.csv'
     click.echo(f'Exporting search results to csv: {file_name}')
     search_to_csv(channel_id, search_text, file_name)
 
 
-
 @click.command( help='delete [channel id]')
 @click.argument('channel_id', required=True)
 def delete(channel_id):
     channel_name = get_channel_name_from_db(channel_id) 
     print(f"Deleting channel {channel_name}")
     print("Are you sure you want to delete this channel and all its data?")
     confirm = input("y/n: ")
@@ -74,14 +80,15 @@
 
 cli.add_command(list)
 cli.add_command(download)
 cli.add_command(search)
 cli.add_command(delete)
 cli.add_command(export)
 
+
 def download_channel(channel_id, channel_name, language, number_of_jobs, s):
     print("Downloading channel")
     with tempfile.TemporaryDirectory() as tmp_dir:
         print('Saving vtt files to', tmp_dir)
 
         channel_url = f"https://www.youtube.com/channel/{channel_id}/videos"
         list_of_videos_urls = get_videos_list(channel_url)
@@ -195,67 +202,66 @@
     return result 
 
 
 def get_quotes(channel_id, text):
     res = search_channel(channel_id, text)
 
     if len(res) == 0:
-        print("No matches found")
+        show_message("no_matches_found")
     else:
 
         shown_titles = []
         shown_stamps = []
 
-        for quote in res: 
-            sub_id = quote[0]
-            vid_title = get_title_from_db(sub_id)
-            vid_id = quote[1]
-            time_stamp = quote[2]
-            subs = quote[3]
-
-            id_stamp =  vid_id + time_stamp[:-4]  
+        for quote in res:
+            video_id = quote["video_id"]
+            video_title = get_title_from_db(video_id)
+            video_title = video_title[0]
+            time_stamp = quote["timestamp"]
+            subs = quote["text"]
+            id_stamp =  video_id + time_stamp[:-4]  
 
             time = time_to_secs(time_stamp) 
 
-            if vid_title not in shown_titles:
-                print(f"\nVideo title\"{vid_title}\"")
-                shown_titles.append(vid_title)
-
+            if video_title not in shown_titles:
+                print(f"\nVideo Title: \"{video_title}\"")
+                shown_titles.append(video_title)
 
             if id_stamp not in shown_stamps:
                 print(f"\n") 
                 print(f"    Quote: \"{subs.strip()}\"")
                 print(f"    Time Stamp: {time_stamp}")
-                print(f"    Link: https://youtu.be/{vid_id}?t={time}")
+                print(f"    Link: https://youtu.be/{video_id}?t={time}\n")
                 shown_stamps.append(id_stamp)
 
 
 def search_to_csv(channel_id, text, file_name):
     res = search_channel(channel_id, text)
 
     if len(res) == 0:
-        print("No matches found")
+        show_message("no_matches_found")
     else:
         with open(file_name, 'w', newline='') as csvfile:
             writer = csv.writer(csvfile)
             writer.writerow(['Video Title', 'Quote', 'Time Stamp', 'Link'])
             
             shown_stamps = []
 
-            for quote in res: 
-                sub_id = quote[0]
-                vid_title = get_title_from_db(sub_id)
-                vid_id = quote[1]
-                time_stamp = quote[2]
-                subs = quote[3]
-                id_stamp =  vid_id + time_stamp[:-4]  
+            for quote in res:
+                video_id = quote["video_id"]
+                video_title = get_title_from_db(video_id)
+                video_title = video_title[0]
+                time_stamp = quote["timestamp"]
+                subs = quote["text"]
+                id_stamp =  video_id + time_stamp[:-4]  
+
                 time = time_to_secs(time_stamp) 
 
                 if id_stamp not in shown_stamps:
-                    writer.writerow([vid_title, subs.strip(), time_stamp, f"https://youtu.be/{vid_id}?t={time}"])
+                    writer.writerow([video_title, subs.strip(), time_stamp, f"https://youtu.be/{video_id}?t={time}"])
                     shown_stamps.append(id_stamp)
 
 
 def time_to_secs(time_str):
 
     time_rex = re.search("^(\d\d):(\d\d):(\d\d)",time_str )
     hours = int(time_rex.group(1)) * 3600 
@@ -327,7 +333,14 @@
                 "bl":m.group(1),
                 "hl":"de",
                 "set_eom":"true"
             }
             s.post("https://consent.youtube.com/save", data=data)
 
 
+def show_message(code):
+    error_dict = {
+        "search_too_long": "Error: Search text must be less than 40 characters",
+        "no_matches_found": "No matches found.\n- Try shortening the search text or use wildcards to match partial words."
+    }
+
+    print(error_dict[code])
```

### Comparing `yt-fts-0.1.4/yt_fts.egg-info/PKG-INFO` & `yt-fts-0.1.5/yt_fts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-fts
-Version: 0.1.4
+Version: 0.1.5
 Summary: yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.
 Home-page: https://github.com/NotJoeMartinez/yt-fts
 Author: NotJoeMartinez
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
```


# Comparing `tmp/yt-fts-0.1.7.tar.gz` & `tmp/yt-fts-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yt-fts-0.1.7.tar", last modified: Mon May 29 06:41:17 2023, max compression
+gzip compressed data, was "yt-fts-0.1.8.tar", last modified: Mon May 29 17:46:11 2023, max compression
```

## Comparing `yt-fts-0.1.7.tar` & `yt-fts-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:41:17.183439 yt-fts-0.1.7/
--rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 20:45:24.000000 yt-fts-0.1.7/LICENSE
--rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-29 06:41:17.182860 yt-fts-0.1.7/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)     3718 2023-05-28 20:45:24.000000 yt-fts-0.1.7/README.md
--rw-r--r--   0 home       (501) staff       (20)       38 2023-05-29 06:41:17.183813 yt-fts-0.1.7/setup.cfg
--rw-r--r--   0 home       (501) staff       (20)      969 2023-05-29 06:40:23.000000 yt-fts-0.1.7/setup.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:41:17.177447 yt-fts-0.1.7/yt_fts/
--rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 20:45:24.000000 yt-fts-0.1.7/yt_fts/__init__.py
--rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 20:45:24.000000 yt-fts-0.1.7/yt_fts/__main__.py
--rw-r--r--   0 home       (501) staff       (20)     2873 2023-05-29 05:22:56.000000 yt-fts-0.1.7/yt_fts/db_scripts.py
--rw-r--r--   0 home       (501) staff       (20)    10682 2023-05-29 06:11:35.000000 yt-fts-0.1.7/yt_fts/yt_fts.py
-drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 06:41:17.181741 yt-fts-0.1.7/yt_fts.egg-info/
--rw-r--r--   0 home       (501) staff       (20)     4261 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/PKG-INFO
--rw-r--r--   0 home       (501) staff       (20)      284 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/SOURCES.txt
--rw-r--r--   0 home       (501) staff       (20)        1 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/dependency_links.txt
--rw-r--r--   0 home       (501) staff       (20)       45 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/entry_points.txt
--rw-r--r--   0 home       (501) staff       (20)      288 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/requires.txt
--rw-r--r--   0 home       (501) staff       (20)        7 2023-05-29 06:41:17.000000 yt-fts-0.1.7/yt_fts.egg-info/top_level.txt
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 17:46:11.124924 yt-fts-0.1.8/
+-rw-r--r--   0 home       (501) staff       (20)     1211 2023-05-28 20:45:24.000000 yt-fts-0.1.8/LICENSE
+-rw-r--r--   0 home       (501) staff       (20)     4705 2023-05-29 17:46:11.124205 yt-fts-0.1.8/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)     4162 2023-05-29 17:04:59.000000 yt-fts-0.1.8/README.md
+-rw-r--r--   0 home       (501) staff       (20)       38 2023-05-29 17:46:11.125157 yt-fts-0.1.8/setup.cfg
+-rw-r--r--   0 home       (501) staff       (20)      969 2023-05-29 17:46:03.000000 yt-fts-0.1.8/setup.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 17:46:11.116939 yt-fts-0.1.8/tests/
+-rw-r--r--   0 home       (501) staff       (20)      325 2023-05-29 14:19:36.000000 yt-fts-0.1.8/tests/test_search_all.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 17:46:11.119100 yt-fts-0.1.8/yt_fts/
+-rw-r--r--   0 home       (501) staff       (20)        0 2023-05-28 20:45:24.000000 yt-fts-0.1.8/yt_fts/__init__.py
+-rw-r--r--   0 home       (501) staff       (20)       65 2023-05-28 20:45:24.000000 yt-fts-0.1.8/yt_fts/__main__.py
+-rw-r--r--   0 home       (501) staff       (20)     3204 2023-05-29 17:38:10.000000 yt-fts-0.1.8/yt_fts/db_scripts.py
+-rw-r--r--   0 home       (501) staff       (20)    10975 2023-05-29 17:41:42.000000 yt-fts-0.1.8/yt_fts/yt_fts.py
+drwxr-xr-x   0 home       (501) staff       (20)        0 2023-05-29 17:46:11.123252 yt-fts-0.1.8/yt_fts.egg-info/
+-rw-r--r--   0 home       (501) staff       (20)     4705 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/PKG-INFO
+-rw-r--r--   0 home       (501) staff       (20)      309 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/SOURCES.txt
+-rw-r--r--   0 home       (501) staff       (20)        1 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/dependency_links.txt
+-rw-r--r--   0 home       (501) staff       (20)       45 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/entry_points.txt
+-rw-r--r--   0 home       (501) staff       (20)      288 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/requires.txt
+-rw-r--r--   0 home       (501) staff       (20)        7 2023-05-29 17:46:11.000000 yt-fts-0.1.8/yt_fts.egg-info/top_level.txt
```

### Comparing `yt-fts-0.1.7/LICENSE` & `yt-fts-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yt-fts-0.1.7/PKG-INFO` & `yt-fts-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-fts
-Version: 0.1.7
+Version: 0.1.8
 Summary: yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.
 Home-page: https://github.com/NotJoeMartinez/yt-fts
 Author: NotJoeMartinez
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -55,17 +55,17 @@
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   delete    delete [channel id]
   download  download [channel url]
-  export    export [channel id] [search text]
+  export    export [search text] [channel id]
   list      Lists channels
-  search    search [channel id] [search text]
+  search    search [search text] [channel id]
 ```
 
 ### `download`
 Will download all of a channels vtt files into your database 
 ```bash
 yt-fts download "https://www.youtube.com/@TimDillonShow/videos"
 ```
@@ -104,49 +104,63 @@
 channel_id                channel_name         channel_url
 ------------------------  -------------------  ---------------------------------------------------------------
 UC4woSp8ITBoYDmjkukhEhxg  The Tim Dillon Show  https://www.youtube.com/channel/UC4woSp8ITBoYDmjkukhEhxg/videos
 ```
 
 ### `search`
 Search a channel for text based off the channel id you give it and 
-print a url to that point in the video
+print a url to that point in the video. The search string does not 
+have to be a word for word and match is limited to 40 characters. 
+
 ```bash
-yt-fts search [channel_id] "text you want to find"
+yt-fts search "text you want to find" [channel_id]
 ```
-**EX:**
-
+**Ex:**
 ```bash
-yt-fts search UC4woSp8ITBoYDmjkukhEhxg "life in the big city"
+yt-fts search "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 output:
 ```
-Video title"("#208 - Let's Have A Party | The Tim Dillon Show - YouTube",)"
+Video Title: "164 - Life In The Big City - YouTube"
+
+    Quote: "van in the driveway life in the big city"
+    Time Stamp: 00:30:44.580
+    Link: https://youtu.be/dqGyCTbzYmc?t=1841
+
+Video Title: "154 - The 3 AM Episode - YouTube"
+
+    Quote: "Dennis would go hey life in the big city"
+    Time Stamp: 00:58:53.789
+    Link: https://youtu.be/MhaG3Yfv1cU?t=3530
+```
 
-    Quote: "life in the big city Dan is wearing the"
-    Time Stamp: 01:50:07.790
-    Link: https://youtu.be/CJ_KAsz8rjQ?t=6604
+### Advanced Search Syntax
 
-Video title"('#176 - The Florida Project | The Tim Dillon Show - YouTube',)"
+The search string supports sqlite [Enhanced Query Syntax](https://www.sqlite.org/fts3.html#full_text_index_queries).
+which includes things like [prefix queries](https://www.sqlite.org/fts3.html#termprefix) which you can use to match parts of a word.  
 
-    Quote: "the show life in the big city love these"
-    Time Stamp: 00:31:05.669
-    Link: https://youtu.be/nKcqbHQndFQ?t=1862
+**Ex:**
 
-Video title"('164 - Life In The Big City - YouTube',)"
+```bash
+yt-fts search "rea* kni* Mali*" UC4woSp8ITBoYDmjkukhEhxg 
+```
+output:
+```
+Video Title: "#200 - Knife Fights In Malibu | The Tim Dillon Show - YouTube"
 
-    Quote: "life in the big city it was one of my"
-    Time Stamp: 00:27:17.549
-    Link: https://youtu.be/dqGyCTbzYmc?t=1634
+    Quote: "real knife fight down here in Malibu I"
+    Time Stamp: 00:45:39.420
+    Link: https://youtu.be/e79H5nxS65Q?t=2736
 ```
 
 ### `Export`
 Similar to `search` except it will export all of the search results to a csv 
 with the format: `Video Title,Quote,Time Stamp,Link` as it's headers
 ```bash
-yt-fts export UC4woSp8ITBoYDmjkukhEhxg "life in the big city" 
+yt-fts export "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 
 ### `Delete` 
 Will delete a channel from your database 
 ```bash
 yt-fts delete [channel_id]
 ```
```

### Comparing `yt-fts-0.1.7/README.md` & `yt-fts-0.1.8/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   delete    delete [channel id]
   download  download [channel url]
-  export    export [channel id] [search text]
+  export    export [search text] [channel id]
   list      Lists channels
-  search    search [channel id] [search text]
+  search    search [search text] [channel id]
 ```
 
 ### `download`
 Will download all of a channels vtt files into your database 
 ```bash
 yt-fts download "https://www.youtube.com/@TimDillonShow/videos"
 ```
@@ -94,49 +94,63 @@
 channel_id                channel_name         channel_url
 ------------------------  -------------------  ---------------------------------------------------------------
 UC4woSp8ITBoYDmjkukhEhxg  The Tim Dillon Show  https://www.youtube.com/channel/UC4woSp8ITBoYDmjkukhEhxg/videos
 ```
 
 ### `search`
 Search a channel for text based off the channel id you give it and 
-print a url to that point in the video
+print a url to that point in the video. The search string does not 
+have to be a word for word and match is limited to 40 characters. 
+
 ```bash
-yt-fts search [channel_id] "text you want to find"
+yt-fts search "text you want to find" [channel_id]
 ```
-**EX:**
-
+**Ex:**
 ```bash
-yt-fts search UC4woSp8ITBoYDmjkukhEhxg "life in the big city"
+yt-fts search "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 output:
 ```
-Video title"("#208 - Let's Have A Party | The Tim Dillon Show - YouTube",)"
+Video Title: "164 - Life In The Big City - YouTube"
+
+    Quote: "van in the driveway life in the big city"
+    Time Stamp: 00:30:44.580
+    Link: https://youtu.be/dqGyCTbzYmc?t=1841
+
+Video Title: "154 - The 3 AM Episode - YouTube"
+
+    Quote: "Dennis would go hey life in the big city"
+    Time Stamp: 00:58:53.789
+    Link: https://youtu.be/MhaG3Yfv1cU?t=3530
+```
 
-    Quote: "life in the big city Dan is wearing the"
-    Time Stamp: 01:50:07.790
-    Link: https://youtu.be/CJ_KAsz8rjQ?t=6604
+### Advanced Search Syntax
 
-Video title"('#176 - The Florida Project | The Tim Dillon Show - YouTube',)"
+The search string supports sqlite [Enhanced Query Syntax](https://www.sqlite.org/fts3.html#full_text_index_queries).
+which includes things like [prefix queries](https://www.sqlite.org/fts3.html#termprefix) which you can use to match parts of a word.  
 
-    Quote: "the show life in the big city love these"
-    Time Stamp: 00:31:05.669
-    Link: https://youtu.be/nKcqbHQndFQ?t=1862
+**Ex:**
 
-Video title"('164 - Life In The Big City - YouTube',)"
+```bash
+yt-fts search "rea* kni* Mali*" UC4woSp8ITBoYDmjkukhEhxg 
+```
+output:
+```
+Video Title: "#200 - Knife Fights In Malibu | The Tim Dillon Show - YouTube"
 
-    Quote: "life in the big city it was one of my"
-    Time Stamp: 00:27:17.549
-    Link: https://youtu.be/dqGyCTbzYmc?t=1634
+    Quote: "real knife fight down here in Malibu I"
+    Time Stamp: 00:45:39.420
+    Link: https://youtu.be/e79H5nxS65Q?t=2736
 ```
 
 ### `Export`
 Similar to `search` except it will export all of the search results to a csv 
 with the format: `Video Title,Quote,Time Stamp,Link` as it's headers
 ```bash
-yt-fts export UC4woSp8ITBoYDmjkukhEhxg "life in the big city" 
+yt-fts export "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 
 ### `Delete` 
 Will delete a channel from your database 
 ```bash
 yt-fts delete [channel_id]
 ```
```

### Comparing `yt-fts-0.1.7/setup.py` & `yt-fts-0.1.8/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     'console_scripts': [
         'yt-fts=yt_fts.yt_fts:cli',
     ],
 }
 
 setup(
     name='yt-fts', 
-    version='0.1.7',
+    version='0.1.8',
     description='yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.',
     long_description=long_description,
     long_description_content_type='text/markdown', 
     author='NotJoeMartinez',
     url='https://github.com/NotJoeMartinez/yt-fts',  
     packages=find_packages(),
     install_requires=dependencies,
```

### Comparing `yt-fts-0.1.7/yt_fts/db_scripts.py` & `yt-fts-0.1.8/yt_fts/db_scripts.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,22 +92,32 @@
 
     return list(db["Subtitles"].search(text, where=f"video_id IN (SELECT video_id FROM Videos WHERE channel_id = '{channel_id}')"))
 
 
 def get_title_from_db(video_id):
     db = Database(db_name)
 
-    return db.execute(f"SELECT video_title FROM Videos WHERE video_id = ?", [video_id]).fetchone()
+    return db.execute(f"SELECT video_title FROM Videos WHERE video_id = ?", [video_id]).fetchone()[0]
 
 
-def get_channel_name_from_db(channel_id):
+def search_all(text):
+    db = Database(db_name)
+
+    return list(db["Subtitles"].search(text))
+
+
+def get_channel_name_from_id(channel_id):
     db = Database(db_name)
 
     return db.execute(f"SELECT channel_name FROM Channels WHERE channel_id = ?", [channel_id]).fetchone()[0]
 
+def get_channel_name_from_video_id(video_id):
+    db = Database(db_name)
+
+    return db.execute(f"SELECT channel_name FROM Channels WHERE channel_id = (SELECT channel_id FROM Videos WHERE video_id = ?)", [video_id]).fetchone()[0]
 
 def delete_channel(channel_id):
     conn = sqlite3.connect(db_name)
     cur = conn.cursor()
 
     cur.execute("DELETE FROM Channels WHERE channel_id = ?", (channel_id,))
     cur.execute("DELETE FROM Subtitles WHERE video_id IN (SELECT video_id FROM Videos WHERE channel_id = ?)", (channel_id,))
```

### Comparing `yt-fts-0.1.7/yt_fts/yt_fts.py` & `yt-fts-0.1.8/yt_fts/yt_fts.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,41 +37,58 @@
     if channel_id:
         download_channel(channel_id, channel_name, language, number_of_jobs, s)
     else:
         print("Error finding channel id try --channel-id option")
 
 
 @click.command( help='search [channel id] [search text]')
-@click.argument('channel_id', required=True)
 @click.argument('search_text', required=True)
-def search(channel_id, search_text):
+@click.option('--all', is_flag=True, help='Search in all channels')
+@click.argument('channel_id', required=False)
+def search(channel_id, search_text, all):
     if len(search_text) > 40:
         show_message("search_too_long")
         return
-    click.echo(f'Searching in channel {channel_id}')
-    get_quotes(channel_id, search_text)
+    if all:
+        click.echo('Searching in all channels')
+        get_quotes("all", search_text)
+    else:
+        if channel_id is None:
+            click.echo('Error: Channel ID is required when not using --all option')
+            return
+        click.echo(f'Searching in channel {channel_id}')
+        get_quotes(channel_id, search_text)
 
 
-@click.command( help='export [channel id] [search text] ')
-@click.argument('channel_id', required=True)
-@click.argument('search_text', required=True)
-def export(channel_id, search_text):
+@click.command( help="export [channel id] [search text]")
+@click.argument("search_text", required=True)
+@click.option("--all", is_flag=True, help="Export from all channels")
+@click.argument("channel_id", required=False)
+def export(channel_id, search_text, all):
     if len(search_text) > 40:
         show_message("search_too_long")
         return
     timestamp = datetime.datetime.now().strftime("%Y%m%d_%H%M%S")
-    file_name = f'{channel_id}_{timestamp}.csv'
-    click.echo(f'Exporting search results to csv: {file_name}')
-    search_to_csv(channel_id, search_text, file_name)
+    if all:
+        file_name = f"all_{timestamp}.csv"
+        click.echo(f"Exporting search results from all channels to csv: {file_name}")
+        search_to_csv("all", search_text, file_name)
+    else:
+        if channel_id is None:
+            click.echo("Error: Channel ID is required when not using --all option")
+            return
+        file_name = f"{channel_id}_{timestamp}.csv"
+        click.echo(f"Exporting search results to csv: {file_name}")
+        search_to_csv(channel_id, search_text, file_name)
 
 
-@click.command( help='delete [channel id]')
-@click.argument('channel_id', required=True)
+@click.command( help="delete [channel id]")
+@click.argument("channel_id", required=True)
 def delete(channel_id):
-    channel_name = get_channel_name_from_db(channel_id) 
+    channel_name = get_channel_name_from_id(channel_id) 
     print(f"Deleting channel {channel_name}")
     print("Are you sure you want to delete this channel and all its data?")
     confirm = input("y/n: ")
     if confirm == "y":
         click.echo(f'deleting channel {channel_name}')
         delete_channel(channel_id)
     else:
@@ -84,23 +101,21 @@
 cli.add_command(delete)
 cli.add_command(export)
 
 
 def download_channel(channel_id, channel_name, language, number_of_jobs, s):
     print("Downloading channel")
     with tempfile.TemporaryDirectory() as tmp_dir:
-        print('Saving vtt files to', tmp_dir)
 
         channel_url = f"https://www.youtube.com/channel/{channel_id}/videos"
         list_of_videos_urls = get_videos_list(channel_url)
 
         download_vtts(number_of_jobs, list_of_videos_urls, language, tmp_dir)
         add_channel_info(channel_id, channel_name, channel_url)
 
-        print("Adding VTT data to db")
         vtt_to_db(channel_id, tmp_dir, s)
 
 
 def download_vtts(number_of_jobs, list_of_videos_urls, language ,tmp_dir):
     executor = ThreadPoolExecutor(number_of_jobs)
     futures = []
     for video_id in list_of_videos_urls:
@@ -115,15 +130,14 @@
 def get_vtt(tmp_dir, video_url, language):
     subprocess.run([
         "yt-dlp",
         "-o", f"{tmp_dir}/%(id)s.%(ext)s",
         "--write-auto-sub",
         "--convert-subs", "vtt",
         "--skip-download",
-            "--sub-langs", f"{language},-live_chat",
         "--sub-langs", f"{language},-live_chat",
         video_url
     ])
 
 
 def get_videos_list(channel_url):
     cmd = [
@@ -178,96 +192,98 @@
 
     result = []
 
     time_pattern = "^(.*) align:start position:0%"
 
     with open(file_path, "r") as f:
         lines = f.readlines()
-        for count, line in enumerate(lines):
-            time_match = re.match(time_pattern, line)
-
-            if time_match:
-                start = re.search("^(.*) -->",time_match.group(1))
-                end = re.search("--> (.*)",time_match.group(1))
 
-                start_time = start.group(1)
-                end_time = end.group(1)
-
-                sub_titles = lines[count + 1]
+    for count, line in enumerate(lines):
+        time_match = re.match(time_pattern, line)
 
+        if time_match:
+            start = re.search("^(.*) -->",time_match.group(1))
+            start_time = start.group(1)
+            sub_titles = lines[count + 1]
+
+            # prevent duplicate entries
+            if result and result[-1]['text'] == sub_titles.strip('\n'):
+                continue
+            else:   
                 result.append({
                     'start_time': start_time,
                     'text': sub_titles.strip('\n'),
                 })
-        
+
     return result 
 
 
 def get_quotes(channel_id, text):
-    res = search_channel(channel_id, text)
+
+    if channel_id == "all":
+        res = search_all(text)
+    else:
+        res = search_channel(channel_id, text)
 
     if len(res) == 0:
         show_message("no_matches_found")
+        exit()
+
+    for quote in res:
+        video_id = quote["video_id"]
+
+        video_title = get_title_from_db(video_id)
+
+        channel_name = get_channel_name_from_video_id(video_id)
+
+        time_stamp = quote["timestamp"]
+        subs = quote["text"]
+
+        time = time_to_secs(time_stamp) 
+
+        print("")
+        print(f"{channel_name}: \"{video_title}\"")
+        print(f"") 
+        print(f"    Quote: \"{subs.strip()}\"")
+        print(f"    Time Stamp: {time_stamp}")
+        print(f"    Link: https://youtu.be/{video_id}?t={time}\n")
+
+
+def search_to_csv(channel_id, text, file_name):
+    if channel_id == "all":
+        res = search_all(text)
     else:
+        res = search_channel(channel_id, text)
 
-        shown_titles = []
-        shown_stamps = []
+    if len(res) == 0:
+        show_message("no_matches_found")
+        exit()
 
+    with open(file_name, 'w', newline='') as csvfile:
+        writer = csv.writer(csvfile)
+        writer.writerow(['Channel Name','Video Title', 'Quote', 'Time Stamp', 'Link'])
+        
         for quote in res:
             video_id = quote["video_id"]
+
+            channel_name = get_channel_name_from_video_id(video_id)
+
             video_title = get_title_from_db(video_id)
-            video_title = video_title[0]
+
             time_stamp = quote["timestamp"]
             subs = quote["text"]
-            id_stamp =  video_id + time_stamp[:-4]  
 
             time = time_to_secs(time_stamp) 
 
-            if video_title not in shown_titles:
-                print(f"\nVideo Title: \"{video_title}\"")
-                shown_titles.append(video_title)
-
-            if id_stamp not in shown_stamps:
-                print(f"\n") 
-                print(f"    Quote: \"{subs.strip()}\"")
-                print(f"    Time Stamp: {time_stamp}")
-                print(f"    Link: https://youtu.be/{video_id}?t={time}\n")
-                shown_stamps.append(id_stamp)
-
-
-def search_to_csv(channel_id, text, file_name):
-    res = search_channel(channel_id, text)
-
-    if len(res) == 0:
-        show_message("no_matches_found")
-    else:
-        with open(file_name, 'w', newline='') as csvfile:
-            writer = csv.writer(csvfile)
-            writer.writerow(['Video Title', 'Quote', 'Time Stamp', 'Link'])
-            
-            shown_stamps = []
-
-            for quote in res:
-                video_id = quote["video_id"]
-                video_title = get_title_from_db(video_id)
-                video_title = video_title[0]
-                time_stamp = quote["timestamp"]
-                subs = quote["text"]
-                id_stamp =  video_id + time_stamp[:-4]  
-
-                time = time_to_secs(time_stamp) 
-
-                if id_stamp not in shown_stamps:
-                    writer.writerow([video_title, subs.strip(), time_stamp, f"https://youtu.be/{video_id}?t={time}"])
-                    shown_stamps.append(id_stamp)
+            writer.writerow([channel_name,video_title, subs.strip(), time_stamp, f"https://youtu.be/{video_id}?t={time}"])
 
 
 def time_to_secs(time_str):
 
-    time_rex = re.search("^(\d\d):(\d\d):(\d\d)",time_str )
+    time_rex = re.search("^(\d\d):(\d\d):(\d\d)",time_str)
     hours = int(time_rex.group(1)) * 3600 
     mins = int(time_rex.group(2)) * 60
     secs = int(time_rex.group(3)) 
 
     total_secs =  hours + mins + secs
     return total_secs - 3
```

### Comparing `yt-fts-0.1.7/yt_fts.egg-info/PKG-INFO` & `yt-fts-0.1.8/yt_fts.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yt-fts
-Version: 0.1.7
+Version: 0.1.8
 Summary: yt-fts is a simple python script that uses yt-dlp to scrape all of a youtube channels subtitles and load them into an sqlite database that is searchable from the command line. It allows you to query a channel for specific key word or phrase and will generate time stamped youtube urls to the video containing the keyword.
 Home-page: https://github.com/NotJoeMartinez/yt-fts
 Author: NotJoeMartinez
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -55,17 +55,17 @@
 
 Options:
   --help  Show this message and exit.
 
 Commands:
   delete    delete [channel id]
   download  download [channel url]
-  export    export [channel id] [search text]
+  export    export [search text] [channel id]
   list      Lists channels
-  search    search [channel id] [search text]
+  search    search [search text] [channel id]
 ```
 
 ### `download`
 Will download all of a channels vtt files into your database 
 ```bash
 yt-fts download "https://www.youtube.com/@TimDillonShow/videos"
 ```
@@ -104,49 +104,63 @@
 channel_id                channel_name         channel_url
 ------------------------  -------------------  ---------------------------------------------------------------
 UC4woSp8ITBoYDmjkukhEhxg  The Tim Dillon Show  https://www.youtube.com/channel/UC4woSp8ITBoYDmjkukhEhxg/videos
 ```
 
 ### `search`
 Search a channel for text based off the channel id you give it and 
-print a url to that point in the video
+print a url to that point in the video. The search string does not 
+have to be a word for word and match is limited to 40 characters. 
+
 ```bash
-yt-fts search [channel_id] "text you want to find"
+yt-fts search "text you want to find" [channel_id]
 ```
-**EX:**
-
+**Ex:**
 ```bash
-yt-fts search UC4woSp8ITBoYDmjkukhEhxg "life in the big city"
+yt-fts search "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 output:
 ```
-Video title"("#208 - Let's Have A Party | The Tim Dillon Show - YouTube",)"
+Video Title: "164 - Life In The Big City - YouTube"
+
+    Quote: "van in the driveway life in the big city"
+    Time Stamp: 00:30:44.580
+    Link: https://youtu.be/dqGyCTbzYmc?t=1841
+
+Video Title: "154 - The 3 AM Episode - YouTube"
+
+    Quote: "Dennis would go hey life in the big city"
+    Time Stamp: 00:58:53.789
+    Link: https://youtu.be/MhaG3Yfv1cU?t=3530
+```
 
-    Quote: "life in the big city Dan is wearing the"
-    Time Stamp: 01:50:07.790
-    Link: https://youtu.be/CJ_KAsz8rjQ?t=6604
+### Advanced Search Syntax
 
-Video title"('#176 - The Florida Project | The Tim Dillon Show - YouTube',)"
+The search string supports sqlite [Enhanced Query Syntax](https://www.sqlite.org/fts3.html#full_text_index_queries).
+which includes things like [prefix queries](https://www.sqlite.org/fts3.html#termprefix) which you can use to match parts of a word.  
 
-    Quote: "the show life in the big city love these"
-    Time Stamp: 00:31:05.669
-    Link: https://youtu.be/nKcqbHQndFQ?t=1862
+**Ex:**
 
-Video title"('164 - Life In The Big City - YouTube',)"
+```bash
+yt-fts search "rea* kni* Mali*" UC4woSp8ITBoYDmjkukhEhxg 
+```
+output:
+```
+Video Title: "#200 - Knife Fights In Malibu | The Tim Dillon Show - YouTube"
 
-    Quote: "life in the big city it was one of my"
-    Time Stamp: 00:27:17.549
-    Link: https://youtu.be/dqGyCTbzYmc?t=1634
+    Quote: "real knife fight down here in Malibu I"
+    Time Stamp: 00:45:39.420
+    Link: https://youtu.be/e79H5nxS65Q?t=2736
 ```
 
 ### `Export`
 Similar to `search` except it will export all of the search results to a csv 
 with the format: `Video Title,Quote,Time Stamp,Link` as it's headers
 ```bash
-yt-fts export UC4woSp8ITBoYDmjkukhEhxg "life in the big city" 
+yt-fts export "life in the big city" UC4woSp8ITBoYDmjkukhEhxg 
 ```
 
 ### `Delete` 
 Will delete a channel from your database 
 ```bash
 yt-fts delete [channel_id]
 ```
```


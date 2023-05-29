# Comparing `tmp/spotify_to_ytmusic-0.1.4.tar.gz` & `tmp/spotify_to_ytmusic-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spotify_to_ytmusic-0.1.4.tar", last modified: Sat Apr 22 07:01:23 2023, max compression
+gzip compressed data, was "spotify_to_ytmusic-0.2.0.tar", last modified: Mon May 29 12:44:32 2023, max compression
```

## Comparing `spotify_to_ytmusic-0.1.4.tar` & `spotify_to_ytmusic-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.437120 spotify_to_ytmusic-0.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.429120 spotify_to_ytmusic-0.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.433120 spotify_to_ytmusic-0.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)      650 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-22 07:01:23.437120 spotify_to_ytmusic-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3250 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-22 07:01:23.437120 spotify_to_ytmusic-0.1.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.433120 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2455 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/controllers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/match.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/settings.ini.example
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/spotify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/ytmusic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.433120 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-22 07:01:23.000000 spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:23.437120 spotify_to_ytmusic-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/tests/test_spotipy.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 07:01:09.000000 spotify_to_ytmusic-0.1.4/tests/test_youtube.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:44:32.788610 spotify_to_ytmusic-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:44:32.784610 spotify_to_ytmusic-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:44:32.784610 spotify_to_ytmusic-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      650 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-29 12:44:32.788610 spotify_to_ytmusic-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 12:44:32.788610 spotify_to_ytmusic-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:44:32.788610 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3160 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/match.py
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/settings.ini.example
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/spotify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/ytmusic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:44:32.788610 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-29 12:44:32.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-29 12:44:32.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 12:44:32.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-29 12:44:32.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 12:44:32.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-29 12:44:32.000000 spotify_to_ytmusic-0.2.0/spotify_to_ytmusic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 12:44:32.788610 spotify_to_ytmusic-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/tests/test_spotipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 12:44:16.000000 spotify_to_ytmusic-0.2.0/tests/test_youtube.py
```

### Comparing `spotify_to_ytmusic-0.1.4/.github/workflows/coverage.yml` & `spotify_to_ytmusic-0.2.0/.github/workflows/coverage.yml`

 * *Files 15% similar despite different names*

```diff
@@ -11,18 +11,20 @@
     - name: Setup Python
       uses: actions/setup-python@master
       with:
         python-version: 3.x
     - name: Generate coverage report
       env:
         SETTINGS_INI: ${{ secrets.SETTINGS_INI }}
+        SPOTIPY_CACHE: ${{ secrets.SPOTIPY_CACHE }}
       run: |
         pip install -e .
         pip install coverage
         cat <<< "$SETTINGS_INI" > spotify_to_ytmusic/settings.ini
+        cat <<< "$SPOTIPY_CACHE" > .cache
         coverage run
         coverage xml
     - name: Upload coverage to Codecov
       uses: codecov/codecov-action@v3
       with:
         file: coverage.xml
         flags: unittests
```

### Comparing `spotify_to_ytmusic-0.1.4/.github/workflows/pythonpublish.yml` & `spotify_to_ytmusic-0.2.0/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.4/.gitignore` & `spotify_to_ytmusic-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.4/LICENSE` & `spotify_to_ytmusic-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.4/PKG-INFO` & `spotify_to_ytmusic-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify_to_ytmusic
-Version: 0.1.4
+Version: 0.2.0
 Summary: Transfer Spotify playlists to YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,14 +88,17 @@
 
 .. code-block::
 
     spotify_to_ytmusic setup
 
 For backwards compatibility you can also create your own file and pass it using ``--file settings.ini``.
 
+If you want to transfer private playlists from Spotify (i.e. liked songs), choose "yes" for oAuth authentication, otherwise choose "no".
+For oAuth authentication you should set ``http://localhost`` as redirect URI for your app in Spotify's developer dashboard.
+
 Usage
 ------
 
 After you've completed setup, you can simply run the script from the command line using:
 
 .. code-block::
 
@@ -110,14 +113,26 @@
 
 For migration purposes, it is possible to transfer all public playlists of a user by using the Spotify user's ID (unique username).
 
 .. code-block::
 
     spotify_to_ytmusic all <spotifyuserid>
 
+Transfer liked tracks of the Spotify user
+-----------------------------------------
+
+**You must you oAuth authentication for transferring liked songs.**
+
+.. code-block::
+
+   spotify_to_ytmusic liked
+
+This command will open browser where you should give access to your account (if you haven't done that before).
+After authorization you will be redirected to localhost, copy link you were redirected to (looks like localhost/?code=...) and paste to command line.
+
 Command line options
 ---------------------
 
 There are some additional command line options for setting the playlist name and determining whether it's public or not. To view them, run
 
 .. code::
```

### Comparing `spotify_to_ytmusic-0.1.4/README.rst` & `spotify_to_ytmusic-0.2.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 
 .. code-block::
 
     spotify_to_ytmusic setup
 
 For backwards compatibility you can also create your own file and pass it using ``--file settings.ini``.
 
+If you want to transfer private playlists from Spotify (i.e. liked songs), choose "yes" for oAuth authentication, otherwise choose "no".
+For oAuth authentication you should set ``http://localhost`` as redirect URI for your app in Spotify's developer dashboard.
+
 Usage
 ------
 
 After you've completed setup, you can simply run the script from the command line using:
 
 .. code-block::
 
@@ -70,14 +73,26 @@
 
 For migration purposes, it is possible to transfer all public playlists of a user by using the Spotify user's ID (unique username).
 
 .. code-block::
 
     spotify_to_ytmusic all <spotifyuserid>
 
+Transfer liked tracks of the Spotify user
+-----------------------------------------
+
+**You must you oAuth authentication for transferring liked songs.**
+
+.. code-block::
+
+   spotify_to_ytmusic liked
+
+This command will open browser where you should give access to your account (if you haven't done that before).
+After authorization you will be redirected to localhost, copy link you were redirected to (looks like localhost/?code=...) and paste to command line.
+
 Command line options
 ---------------------
 
 There are some additional command line options for setting the playlist name and determining whether it's public or not. To view them, run
 
 .. code::
```

### Comparing `spotify_to_ytmusic-0.1.4/pyproject.toml` & `spotify_to_ytmusic-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/controllers.py` & `spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/controllers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import time
 from datetime import datetime
 
+import spotipy
+
 from spotify_to_ytmusic.setup import setup as setup_func
 from spotify_to_ytmusic.spotify import Spotify
 from spotify_to_ytmusic.ytmusic import YTMusicTransfer
 
 
 def _get_spotify_playlist(spotify, playlist):
     try:
@@ -12,14 +14,21 @@
     except Exception as ex:
         print(
             "Could not get Spotify playlist. Please check the playlist link.\n Error: " + repr(ex)
         )
         return
 
 
+def _print_success(name, playlistId):
+    print(
+        f"Success: created playlist '{name}' at\n"
+        f"https://music.youtube.com/playlist?list={playlistId}"
+    )
+
+
 def _init():
     return Spotify(), YTMusicTransfer()
 
 
 def all(args):
     spotify, ytmusic = _init()
     pl = spotify.getUserPlaylists(args.user)
@@ -33,37 +42,45 @@
             videoIds = ytmusic.search_songs(playlist["tracks"])
             playlist_id = ytmusic.create_playlist(
                 p["name"],
                 p["description"],
                 "PUBLIC" if p["public"] else "PRIVATE",
                 videoIds,
             )
-            print(playlist_id)
+            _print_success(p["name"], playlist_id)
         except Exception as ex:
             print(f"Could not transfer playlist {p['name']}. {str(ex)}")
 
 
-def create(args):
-    spotify, ytmusic = _init()
+def _create_ytmusic(args, playlist, ytmusic):
     date = ""
     if args.date:
         date = " " + datetime.today().strftime("%m/%d/%Y")
-
-    playlist = _get_spotify_playlist(spotify, args.playlist)
     name = args.name + date if args.name else playlist["name"] + date
     info = playlist["description"] if (args.info is None) else args.info
     videoIds = ytmusic.search_songs(playlist["tracks"])
+
     playlistId = ytmusic.create_playlist(
         name, info, "PUBLIC" if args.public else "PRIVATE", videoIds
     )
+    _print_success(name, playlistId)
 
-    print(
-        f"Success: created playlist {name}\n"
-        f"https://music.youtube.com/playlist?list={playlistId}"
-    )
+
+def create(args):
+    spotify, ytmusic = _init()
+    playlist = _get_spotify_playlist(spotify, args.playlist)
+    _create_ytmusic(args, playlist, ytmusic)
+
+
+def liked(args):
+    spotify, ytmusic = _init()
+    if not isinstance(spotify.api.auth_manager, spotipy.SpotifyOAuth):
+        raise Exception("OAuth not configured, please run setup and set OAuth to 'yes'")
+    playlist = spotify.getLikedPlaylist()
+    _create_ytmusic(args, playlist, ytmusic)
 
 
 def update(args):
     spotify, ytmusic = _init()
     playlist = _get_spotify_playlist(spotify, args.playlist)
     playlistId = ytmusic.get_playlist_id(args.name)
     videoIds = ytmusic.search_songs(playlist["tracks"])
```

### Comparing `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/main.py` & `spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,45 +11,52 @@
     setup_parser = subparsers.add_parser("setup", help="Set up credentials")
     setup_parser.set_defaults(func=controllers.setup)
     setup_parser.add_argument("--file", type=Path, help="Optional path to a settings.ini file")
 
     spotify_playlist = argparse.ArgumentParser(add_help=False)
     spotify_playlist.add_argument("playlist", type=str, help="Provide a playlist Spotify link.")
 
-    create_parser = subparsers.add_parser(
-        "create",
-        help="Create a new playlist on YouTube Music.",
-        parents=[spotify_playlist],
-    )
-    create_parser.set_defaults(func=controllers.create)
-    create_parser.add_argument(
+    spotify_playlist_create = argparse.ArgumentParser(add_help=False)
+    spotify_playlist_create.add_argument(
         "-d",
         "--date",
         action="store_true",
         help="Append the current date to the playlist name",
     )
-    create_parser.add_argument(
+    spotify_playlist_create.add_argument(
         "-i",
         "--info",
         type=str,
         help="Provide description information for the YouTube Music Playlist. Default: Spotify playlist description",
     )
-    create_parser.add_argument(
+    spotify_playlist_create.add_argument(
         "-n",
         "--name",
         type=str,
         help="Provide a name for the YouTube Music playlist. Default: Spotify playlist name",
     )
-    create_parser.add_argument(
+    spotify_playlist_create.add_argument(
         "-p",
         "--public",
         action="store_true",
         help="Make created playlist public. Default: private",
     )
 
+    create_parser = subparsers.add_parser(
+        "create",
+        help="Create a new playlist on YouTube Music.",
+        parents=[spotify_playlist, spotify_playlist_create],
+    )
+    create_parser.set_defaults(func=controllers.create)
+
+    liked_parser = subparsers.add_parser(
+        "liked", help="Transfer all liked songs of the user.", parents=[spotify_playlist_create]
+    )
+    liked_parser.set_defaults(func=controllers.liked)
+
     update_parser = subparsers.add_parser(
         "update",
         help="Delete all entries in the provided Google Play Music playlist and update the playlist with entries from the Spotify playlist.",
         parents=[spotify_playlist],
     )
     update_parser.set_defaults(func=controllers.update)
     update_parser.add_argument(
```

### Comparing `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/match.py` & `spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/match.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,19 @@
     :param ytm_results: List of ytmusicapi search results
     :param spoti: Spotify track
     :return: videoId of best matching result
     """
     match_score = {}
     title_score = {}
     for ytm in ytm_results:
-        if "resultType" not in ytm or ytm["resultType"] not in ["song", "video"]:
+        if (
+            "resultType" not in ytm
+            or ytm["resultType"] not in ["song", "video"]
+            or not ytm["title"]
+        ):
             continue
 
         duration_match_score = None
         if "duration" in ytm and ytm["duration"] and spoti["duration"]:
             duration_items = ytm["duration"].split(":")
             duration = int(duration_items[0]) * 60 + int(duration_items[1])
             duration_match_score = 1 - abs(duration - spoti["duration"]) * 2 / spoti["duration"]
```

### Comparing `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/settings.py` & `spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/settings.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/setup.py` & `spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -35,18 +35,19 @@
     settings["youtube"]["headers"] = json.dumps(ytmusicapi.setup_oauth())
     settings.save()
 
 
 def setup_spotify():
     settings = Settings()
     credentials = {
-        "client_id": input(
-            "Paste your client id from the Spotify developer dashboard:"
-        ),
+        "client_id": input("Paste your client id from the Spotify developer dashboard:"),
         "client_secret": input("Paste your client secret from the Spotify developer dashboard:"),
+        "use_oauth": input(
+            "Use OAuth method for authorization to transfer private playlists (yes/no):"
+        ),
     }
     settings["spotify"].update(credentials)
     settings.save()
 
 
 def setup_file(file: Path):
     if not file:
```

### Comparing `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/spotify.py` & `spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/spotify.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import html
 import string
 from urllib.parse import urlparse
 
 import spotipy
-from spotipy.oauth2 import SpotifyClientCredentials
+from spotipy.oauth2 import SpotifyClientCredentials, SpotifyOAuth
 
 from spotify_to_ytmusic.settings import Settings
 
 
 class Spotify:
     def __init__(self):
         settings = Settings()
@@ -18,18 +18,28 @@
             string.hexdigits
         ), f"Spotify client_id not set or invalid: {client_id}"
         client_secret = conf["client_secret"]
         assert set(client_secret).issubset(
             string.hexdigits
         ), f"Spotify client_secret not set or invalid: {client_secret}"
 
-        client_credentials_manager = SpotifyClientCredentials(
-            client_id=client_id, client_secret=client_secret
-        )
-        self.api = spotipy.Spotify(client_credentials_manager=client_credentials_manager)
+        use_oauth = conf.getboolean("use_oauth")
+        if use_oauth:
+            auth = SpotifyOAuth(
+                client_id=client_id,
+                client_secret=client_secret,
+                redirect_uri="http://localhost",
+                scope="user-library-read",
+            )
+            self.api = spotipy.Spotify(auth_manager=auth)
+        else:
+            client_credentials_manager = SpotifyClientCredentials(
+                client_id=client_id, client_secret=client_secret
+            )
+            self.api = spotipy.Spotify(client_credentials_manager=client_credentials_manager)
 
     def getSpotifyPlaylist(self, url):
         playlistId = get_id_from_url(url)
         if len(playlistId) != 22:
             raise Exception(f"Bad playlist id: {playlistId}")
 
         print("Getting Spotify tracks...")
@@ -60,14 +70,27 @@
             results = self.api.user_playlists(user, offset=count * 50)["items"]
             pl.extend(results)
             more = len(results) == 50
             count = count + 1
 
         return [p for p in pl if p["owner"]["id"] == user and p["tracks"]["total"] > 0]
 
+    def getLikedPlaylist(self):
+        response = self.api.current_user_saved_tracks(limit=50)
+        tracks = response["items"]
+        while response["next"] is not None:
+            response = self.api.current_user_saved_tracks(limit=50, offset=response["offset"] + 50)
+            tracks.extend(response["items"])
+
+        return {
+            "tracks": build_results(tracks),
+            "name": "Liked songs (Spotify)",
+            "description": "Your liked tracks from spotify",
+        }
+
 
 def build_results(tracks, album=None):
     results = []
     for track in tracks:
         if "track" in track:
             track = track["track"]
         if not track or track["duration_ms"] == 0:
```

### Comparing `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic/ytmusic.py` & `spotify_to_ytmusic-0.2.0/spotify_to_ytmusic/ytmusic.py`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/PKG-INFO` & `spotify_to_ytmusic-0.2.0/spotify_to_ytmusic.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spotify-to-ytmusic
-Version: 0.1.4
+Version: 0.2.0
 Summary: Transfer Spotify playlists to YouTube Music
 Author-email: sigma67 <ytmusicapi@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 sigma67
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -88,14 +88,17 @@
 
 .. code-block::
 
     spotify_to_ytmusic setup
 
 For backwards compatibility you can also create your own file and pass it using ``--file settings.ini``.
 
+If you want to transfer private playlists from Spotify (i.e. liked songs), choose "yes" for oAuth authentication, otherwise choose "no".
+For oAuth authentication you should set ``http://localhost`` as redirect URI for your app in Spotify's developer dashboard.
+
 Usage
 ------
 
 After you've completed setup, you can simply run the script from the command line using:
 
 .. code-block::
 
@@ -110,14 +113,26 @@
 
 For migration purposes, it is possible to transfer all public playlists of a user by using the Spotify user's ID (unique username).
 
 .. code-block::
 
     spotify_to_ytmusic all <spotifyuserid>
 
+Transfer liked tracks of the Spotify user
+-----------------------------------------
+
+**You must you oAuth authentication for transferring liked songs.**
+
+.. code-block::
+
+   spotify_to_ytmusic liked
+
+This command will open browser where you should give access to your account (if you haven't done that before).
+After authorization you will be redirected to localhost, copy link you were redirected to (looks like localhost/?code=...) and paste to command line.
+
 Command line options
 ---------------------
 
 There are some additional command line options for setting the playlist name and determining whether it's public or not. To view them, run
 
 .. code::
```

### Comparing `spotify_to_ytmusic-0.1.4/spotify_to_ytmusic.egg-info/SOURCES.txt` & `spotify_to_ytmusic-0.2.0/spotify_to_ytmusic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `spotify_to_ytmusic-0.1.4/tests/test_cli.py` & `spotify_to_ytmusic-0.2.0/tests/test_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,20 +19,27 @@
         args = get_args(["create", "playlist-link"])
         self.assertEqual(len(vars(args)), 7)
         args = get_args(["update", "playlist-link", "playlist-name"])
         self.assertEqual(len(vars(args)), 5)
         args = get_args(["setup"])
         self.assertEqual(len(vars(args)), 3)
 
+    def test_liked(self):
+        with mock.patch(
+            "sys.argv", ["", "liked", "-n", "spotify_to_ytmusic", "-d", "-i", "test liked"]
+        ):
+            main()
+
     def test_create(self):
         with mock.patch("sys.argv", ["", "all", "sigmatics"]):
             main()
 
         with mock.patch(
-            "sys.argv", ["", "create", TEST_PLAYLIST, "-n", "spotify_to_ytmusic", "-i", "test-playlist", "-d"]
+            "sys.argv",
+            ["", "create", TEST_PLAYLIST, "-n", "spotify_to_ytmusic", "-i", "test-playlist", "-d"],
         ):
             main()
 
         time.sleep(2)
         with mock.patch("sys.argv", ["", "update", TEST_PLAYLIST, "spotify_to_ytmusic"]):
             main()
 
@@ -46,24 +53,24 @@
             )  # assert number of lines deleted
 
     def test_setup(self):
         tmp_path = Path(__file__).parent.joinpath("settings.tmp")
         example_path = Settings.filepath.parent.joinpath("settings.ini.example")
         shutil.copy(example_path, tmp_path)
         with mock.patch("sys.argv", ["", "setup"]), mock.patch(
-            "builtins.input", return_value="3"
+            "builtins.input", side_effect=["3", "a", "b", "yes", ""]
         ), mock.patch(
             "ytmusicapi.auth.oauth.YTMusicOAuth.get_token_from_code",
             return_value=json.loads(Settings()["youtube"]["headers"]),
         ):
             main()
             assert tmp_path.is_file()
             settings = Settings()
-            assert settings["spotify"]["client_id"] == "3"
-            assert settings["spotify"]["client_secret"] == "3"
+            assert settings["spotify"]["client_id"] == "a"
+            assert settings["spotify"]["client_secret"] == "b"
             tmp_path.unlink()
 
         with mock.patch("sys.argv", ["", "setup", "--file", example_path.as_posix()]), mock.patch(
             "spotify_to_ytmusic.settings.Settings.filepath", tmp_path
         ):
             main()
             assert tmp_path.is_file()
```

### Comparing `spotify_to_ytmusic-0.1.4/tests/test_spotipy.py` & `spotify_to_ytmusic-0.2.0/tests/test_spotipy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import unittest
 
 from spotify_to_ytmusic.spotify import Spotify
 
 
 class TestSpotify(unittest.TestCase):
-
     def setUp(self) -> None:
         self.spotify = Spotify()
 
     def test_getSpotifyPlaylist(self):
-        data = self.spotify.getSpotifyPlaylist("https://open.spotify.com/playlist/03ICMYsVsC4I2SZnERcQJb")
+        data = self.spotify.getSpotifyPlaylist(
+            "https://open.spotify.com/playlist/03ICMYsVsC4I2SZnERcQJb"
+        )
         self.assertEqual(len(data), 3)
         self.assertGreater(len(data["tracks"]), 190)
 
     def test_getUserPlaylists(self):
         playlists = self.spotify.getUserPlaylists("spinninrecordsofficial")
         self.assertGreater(len(playlists), 50)
```

